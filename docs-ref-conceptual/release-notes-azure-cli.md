---
title: Notes de publication d’Azure CLI
description: En savoir plus sur les dernières mises à jour d’Azure CLI
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 08/06/2020
ms.topic: article
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: f81f5a69bd5806d2081a8eaa9b62a5b00b56edf9
ms.sourcegitcommit: 04d3b43d7c960ff0e6188c9672d27046b45da6ed
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/06/2020
ms.locfileid: "87855931"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="69d51-103">Notes de publication d’Azure CLI</span><span class="sxs-lookup"><span data-stu-id="69d51-103">Azure CLI release notes</span></span>

# <a name="current-release-notes"></a>[<span data-ttu-id="69d51-104">Notes de publication de la version actuelle</span><span class="sxs-lookup"><span data-stu-id="69d51-104">Current release notes</span></span>](#tab/azure-cli)

## <a name="august-11-2020"></a><span data-ttu-id="69d51-105">11 août 2020</span><span class="sxs-lookup"><span data-stu-id="69d51-105">August 11, 2020</span></span>

<span data-ttu-id="69d51-106">Version 2.10.1</span><span class="sxs-lookup"><span data-stu-id="69d51-106">Version 2.10.1</span></span>

### <a name="app-service"></a><span data-ttu-id="69d51-107">App Service</span><span class="sxs-lookup"><span data-stu-id="69d51-107">App Service</span></span>

* <span data-ttu-id="69d51-108">Correctif n°9887 webapp et functionapp : prise en charge de l’affectation/la suppression des identités managées utilisateur</span><span class="sxs-lookup"><span data-stu-id="69d51-108">Fix #9887 webapp and functionapp, support assigning/removing user managed identity</span></span>
* <span data-ttu-id="69d51-109">Correctif n°1382, n°14055 : Mise à jour des messages d’erreur pour az webapp create et az webapp config container set</span><span class="sxs-lookup"><span data-stu-id="69d51-109">Fix #1382, #14055: Update error messages for az webapp create and az webapp config container set</span></span>
* <span data-ttu-id="69d51-110">`az webapp up`: Correction de la logique de sélection ASP par défaut lorsque le paramètre --plan n’est pas fourni</span><span class="sxs-lookup"><span data-stu-id="69d51-110">`az webapp up`: Fix default ASP selection logic when --plan parameter is not provided</span></span>

### <a name="appconfig"></a><span data-ttu-id="69d51-111">AppConfig</span><span class="sxs-lookup"><span data-stu-id="69d51-111">AppConfig</span></span>

* <span data-ttu-id="69d51-112">Prise en charge de l’activation/la désactivation de PublicNetworkAccess pendant la création du magasin</span><span class="sxs-lookup"><span data-stu-id="69d51-112">Support enabling/disabling PublicNetworkAccess during store creation</span></span>

### <a name="compute"></a><span data-ttu-id="69d51-113">Calcul</span><span class="sxs-lookup"><span data-stu-id="69d51-113">Compute</span></span>

* <span data-ttu-id="69d51-114">Prise en charge de l’association de disques et d’instantanés à une ressource d’accès au disque</span><span class="sxs-lookup"><span data-stu-id="69d51-114">Support associating disk and snapshot with a disk-access resource</span></span>

### <a name="lab"></a><span data-ttu-id="69d51-115">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="69d51-115">Lab</span></span>

* <span data-ttu-id="69d51-116">Correction du problème n°7904 où se trouvait un bogue de validation de date lors de la création de machines virtuelles de labo</span><span class="sxs-lookup"><span data-stu-id="69d51-116">Fix for issue #7904 date validation bug in lab vm creation</span></span>

### <a name="storage"></a><span data-ttu-id="69d51-117">Stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-117">Storage</span></span>

* <span data-ttu-id="69d51-118">`az storage blob upload-batch`: Correction du problème n°14660 où se trouvaient des arguments sans position</span><span class="sxs-lookup"><span data-stu-id="69d51-118">`az storage blob upload-batch`: Fix issue #14660 with unpositional arguments</span></span>

## <a name="august-04-2020"></a><span data-ttu-id="69d51-119">4 août 2020</span><span class="sxs-lookup"><span data-stu-id="69d51-119">August 04, 2020</span></span>

<span data-ttu-id="69d51-120">Version 2.10.0</span><span class="sxs-lookup"><span data-stu-id="69d51-120">Version 2.10.0</span></span>

### <a name="aks"></a><span data-ttu-id="69d51-121">AKS</span><span class="sxs-lookup"><span data-stu-id="69d51-121">AKS</span></span>

* <span data-ttu-id="69d51-122">`az aks update`: Modification de l’argument --enable-aad pour migrer un cluster non AAD pour lequel RBAC est activé vers un cluster AAD géré par AKS</span><span class="sxs-lookup"><span data-stu-id="69d51-122">`az aks update`: Change --enable-aad argument to migrate a RBAC-enabled non-AAD cluster to a AKS-managed AAD cluster</span></span>
* <span data-ttu-id="69d51-123">`az aks install-cli`: Ajout des arguments --kubelogin-version et --kubelogin-install-location pour installer kubelogin</span><span class="sxs-lookup"><span data-stu-id="69d51-123">`az aks install-cli`: Add --kubelogin-version and --kubelogin-install-location arguments to install kubelogin</span></span>
* <span data-ttu-id="69d51-124">Ajout de la commande az aks nodepool get-upgrades</span><span class="sxs-lookup"><span data-stu-id="69d51-124">Add az aks nodepool get-upgrades command</span></span>

### <a name="ams"></a><span data-ttu-id="69d51-125">AMS</span><span class="sxs-lookup"><span data-stu-id="69d51-125">AMS</span></span>

* <span data-ttu-id="69d51-126">Correctif n° 14021 : az ams account sp n’est pas idempotent</span><span class="sxs-lookup"><span data-stu-id="69d51-126">Fix #14021: az ams account sp is not idempotent</span></span>

### <a name="apim"></a><span data-ttu-id="69d51-127">APIM</span><span class="sxs-lookup"><span data-stu-id="69d51-127">APIM</span></span>

* <span data-ttu-id="69d51-128">Importation d’API APIM : prise en charge de l’importation d’API et amélioration d’autres commandes CLI au niveau de l’API</span><span class="sxs-lookup"><span data-stu-id="69d51-128">apim api import: support API import and enchance other api level cli commands</span></span>

### <a name="app-service"></a><span data-ttu-id="69d51-129">App Service</span><span class="sxs-lookup"><span data-stu-id="69d51-129">App Service</span></span>

* <span data-ttu-id="69d51-130">Correctif n° 13035 : Ajout de la validation pour az webapp config access-restriction afin d’éviter l’ajout de doublons</span><span class="sxs-lookup"><span data-stu-id="69d51-130">Fix #13035: Add validation for az webapp config access-restriction to avoid adding duplicates</span></span>

### <a name="appconfig"></a><span data-ttu-id="69d51-131">AppConfig</span><span class="sxs-lookup"><span data-stu-id="69d51-131">AppConfig</span></span>

* <span data-ttu-id="69d51-132">La valeur par défaut est la référence SKU standard si elle n’est pas spécifiée</span><span class="sxs-lookup"><span data-stu-id="69d51-132">Default to standard sku if not specified</span></span>
* <span data-ttu-id="69d51-133">[CHANGEMENT CASSANT] Paramètres de prise en charge avec le type de contenu JSON</span><span class="sxs-lookup"><span data-stu-id="69d51-133">[BREAKING CHANGE] Support settings with JSON content type</span></span>

### <a name="arm"></a><span data-ttu-id="69d51-134">ARM</span><span class="sxs-lookup"><span data-stu-id="69d51-134">ARM</span></span>

* <span data-ttu-id="69d51-135">`az resource tag`: Correction du bogue concernant le marquage managedApp et certains problèmes de test associés</span><span class="sxs-lookup"><span data-stu-id="69d51-135">`az resource tag`: Fix the bug of managedApp tagging and some related test issues</span></span>
* <span data-ttu-id="69d51-136">`az deployment mg/tenant what-if`: Ajout de la prise en charge au scénario de déploiement au niveau du locataire et du groupe d’administration</span><span class="sxs-lookup"><span data-stu-id="69d51-136">`az deployment mg/tenant what-if`: Add support to management group and tenant level deployment What-If</span></span>
* <span data-ttu-id="69d51-137">`az deployment mg/tenant create`: Ajout du paramètre --confirm-with-what-if/-c.</span><span class="sxs-lookup"><span data-stu-id="69d51-137">`az deployment mg/tenant create`: Add --confirm-with-what-if/-c parameter.</span></span>
* <span data-ttu-id="69d51-138">`az deployment mg/tenant create`: Ajout du paramètre --what-if-result-format/-r.</span><span class="sxs-lookup"><span data-stu-id="69d51-138">`az deployment mg/tenant create`: Add --what-if-result-format/-r parameter.</span></span>
* <span data-ttu-id="69d51-139">`az deployment mg/tenant create`: Ajout du paramètre --what-if-exclude-change-types/-x.</span><span class="sxs-lookup"><span data-stu-id="69d51-139">`az deployment mg/tenant create`: Add --what-if-exclude-change-types/-x parameter.</span></span>
* <span data-ttu-id="69d51-140">`az tag` : prise en charge de la balise az pour le paramètre d’ID de ressource</span><span class="sxs-lookup"><span data-stu-id="69d51-140">`az tag`: az tag support for resource id parameter</span></span>

### <a name="backup"></a><span data-ttu-id="69d51-141">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="69d51-141">Backup</span></span>

* <span data-ttu-id="69d51-142">Déclenchement de la découverte de conteneur/d’élément AFS uniquement si nécessaire</span><span class="sxs-lookup"><span data-stu-id="69d51-142">Trigger AFS container/item discovery only when needed</span></span>

### <a name="cdn"></a><span data-ttu-id="69d51-143">CDN</span><span class="sxs-lookup"><span data-stu-id="69d51-143">CDN</span></span>

* <span data-ttu-id="69d51-144">Ajout de champs de liaison privée à l’origine</span><span class="sxs-lookup"><span data-stu-id="69d51-144">Add private link fields to origin</span></span>

### <a name="compute"></a><span data-ttu-id="69d51-145">Calcul</span><span class="sxs-lookup"><span data-stu-id="69d51-145">Compute</span></span>

* <span data-ttu-id="69d51-146">`az vm/vmss create`: Sélection d’un nom d’utilisateur valide pour l’utilisateur si le nom d’utilisateur par défaut n’est pas valide</span><span class="sxs-lookup"><span data-stu-id="69d51-146">`az vm/vmss create`: Select a valid username for user if the default username is invalid</span></span>
* <span data-ttu-id="69d51-147">`az vm update` : prise en charge de l’image entre locataires</span><span class="sxs-lookup"><span data-stu-id="69d51-147">`az vm update`: support cross tenant image</span></span>
* <span data-ttu-id="69d51-148">`az disk-access`: Ajout d’un nouveau groupe de commandes pour utiliser la ressource d’accès au disque</span><span class="sxs-lookup"><span data-stu-id="69d51-148">`az disk-access`: Add new command group to operate disk access resource</span></span>
* <span data-ttu-id="69d51-149">Prise en charge de la sélection élective automatique du groupe hôte dédié</span><span class="sxs-lookup"><span data-stu-id="69d51-149">Support dedicated host group automatic placement</span></span>
* <span data-ttu-id="69d51-150">Prise en charge de ppg et spg dans le mode d’orchestration de groupe identique de machines virtuelles</span><span class="sxs-lookup"><span data-stu-id="69d51-150">Support ppg and spg in VMSS orchestration mode</span></span>

### <a name="config"></a><span data-ttu-id="69d51-151">Config</span><span class="sxs-lookup"><span data-stu-id="69d51-151">Config</span></span>

* <span data-ttu-id="69d51-152">`az config`: Ajout d’un nouveau module de commande `config`</span><span class="sxs-lookup"><span data-stu-id="69d51-152">`az config`: Add new `config` command module</span></span>

### <a name="extension"></a><span data-ttu-id="69d51-153">Extension</span><span class="sxs-lookup"><span data-stu-id="69d51-153">Extension</span></span>

* <span data-ttu-id="69d51-154">Prise en charge de l’installation automatique d’une extension si l’extension d’une commande n’est pas installée</span><span class="sxs-lookup"><span data-stu-id="69d51-154">Support automatically installing an extension if the extension of a command is not installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="69d51-155">HDInsight</span><span class="sxs-lookup"><span data-stu-id="69d51-155">HDInsight</span></span>

* <span data-ttu-id="69d51-156">Ajout de 3 paramètres à la commande `az hdinsight create` pour prendre en charge la fonctionnalité de liaison privée et chiffrement en transit :</span><span class="sxs-lookup"><span data-stu-id="69d51-156">Add 3 parameters to the command `az hdinsight create` to support private link and encryption in transit feature:</span></span>

### <a name="iot-hub"></a><span data-ttu-id="69d51-157">IoT Hub</span><span class="sxs-lookup"><span data-stu-id="69d51-157">Iot Hub</span></span>

* <span data-ttu-id="69d51-158">Correctif n° 7792 : iot hub create n’est pas idempotent</span><span class="sxs-lookup"><span data-stu-id="69d51-158">Fix #7792: IoT Hub Create is not idempotent</span></span>

### <a name="iot-central"></a><span data-ttu-id="69d51-159">IoT Central</span><span class="sxs-lookup"><span data-stu-id="69d51-159">IoT Central</span></span>

* <span data-ttu-id="69d51-160">Ajout d’une liste d’options de paramètre pour iot central</span><span class="sxs-lookup"><span data-stu-id="69d51-160">Add paramater option list for iot central</span></span>

### <a name="keyvault"></a><span data-ttu-id="69d51-161">KeyVault</span><span class="sxs-lookup"><span data-stu-id="69d51-161">KeyVault</span></span>

* <span data-ttu-id="69d51-162">`az keyvault key encrypt/decrypt` : ajout du paramètre `--data-type` pour spécifier explicitement le type de données d’origine</span><span class="sxs-lookup"><span data-stu-id="69d51-162">`az keyvault key encrypt/decrypt`: add parameter `--data-type` for explicitly specifing the type of original data</span></span>

### <a name="monitor"></a><span data-ttu-id="69d51-163">Superviser</span><span class="sxs-lookup"><span data-stu-id="69d51-163">Monitor</span></span>

* <span data-ttu-id="69d51-164">`az monitor log-analytics workspace data-export` : prise en charge de l’espace de noms Event Hub comme destination.</span><span class="sxs-lookup"><span data-stu-id="69d51-164">`az monitor log-analytics workspace data-export`: support event hub namespace as the destination.</span></span>
* <span data-ttu-id="69d51-165">`az monitor autoscale` : prise en charge de l’espace de noms et des dimensions pour --condition</span><span class="sxs-lookup"><span data-stu-id="69d51-165">`az monitor autoscale`: support namespace and dimensions for --condition</span></span>

### <a name="netappfiles"></a><span data-ttu-id="69d51-166">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="69d51-166">NetAppFiles</span></span>

* <span data-ttu-id="69d51-167">`az volume revert`:  Ajout de Rétablissement du volume pour rétablir un volume dans l’état de l’un de ses instantanés.</span><span class="sxs-lookup"><span data-stu-id="69d51-167">`az volume revert`:  Add Volume Revert to revert a volume to one of its snapshots.</span></span>
* <span data-ttu-id="69d51-168">[CHANGEMENT CASSANT] Suppression de `az netappfiles mount-target`.</span><span class="sxs-lookup"><span data-stu-id="69d51-168">[BREAKING CHANGE] Remove `az netappfiles mount-target`.</span></span>
* <span data-ttu-id="69d51-169">`az volume show`: Ajout de site aux propriétés Active Directory</span><span class="sxs-lookup"><span data-stu-id="69d51-169">`az volume show`: Add site to Active Directory Properties</span></span>

### <a name="network"></a><span data-ttu-id="69d51-170">Réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-170">Network</span></span>

* <span data-ttu-id="69d51-171">`az application-gateway private-link add` : prise en charge de la spécification d’un sous-réseau existant par ID</span><span class="sxs-lookup"><span data-stu-id="69d51-171">`az application-gateway private-link add`: support to specify an existing subnet by ID</span></span>
* <span data-ttu-id="69d51-172">`az network application-gateway waf-policy create` : prise en charge de la version et du type</span><span class="sxs-lookup"><span data-stu-id="69d51-172">`az network application-gateway waf-policy create`: support version and type</span></span>

### <a name="storage"></a><span data-ttu-id="69d51-173">Stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-173">Storage</span></span>

* <span data-ttu-id="69d51-174">Correctif n° 10302 : prise en charge de l’estimation du type de contenu lors de la synchronisation des fichiers</span><span class="sxs-lookup"><span data-stu-id="69d51-174">Fix #10302: Support guess content-type when synchronizing files</span></span>
* <span data-ttu-id="69d51-175">`az storage blob lease`: Application d’une nouvelle version d’API pour les opérations de bail d’objets blob</span><span class="sxs-lookup"><span data-stu-id="69d51-175">`az storage blob lease`: Apply new api version for blob lease operations</span></span>
* <span data-ttu-id="69d51-176">`az storage fs access`: Prise en charge des informations d’identification AAD dans la gestion du contrôle d’accès pour le compte ADLS Gen2</span><span class="sxs-lookup"><span data-stu-id="69d51-176">`az storage fs access`: Support AAD credential in managing access control for ADLS Gen2 account</span></span>
* <span data-ttu-id="69d51-177">`az storage share-rm create/update` : ajout de --access-tier pour prendre en charge le niveau d’accès</span><span class="sxs-lookup"><span data-stu-id="69d51-177">`az storage share-rm create/update`: add --access-tier to support access tier</span></span>

## <a name="july-16-2020"></a><span data-ttu-id="69d51-178">16 juillet 2020</span><span class="sxs-lookup"><span data-stu-id="69d51-178">July 16, 2020</span></span>

<span data-ttu-id="69d51-179">Version 2.9.1</span><span class="sxs-lookup"><span data-stu-id="69d51-179">Version 2.9.1</span></span>

### <a name="aks"></a><span data-ttu-id="69d51-180">AKS</span><span class="sxs-lookup"><span data-stu-id="69d51-180">AKS</span></span>

* <span data-ttu-id="69d51-181">Suppression du paramètre explicite de VMSS dans l’exemple de commande Windows puisqu’il est maintenant par défaut</span><span class="sxs-lookup"><span data-stu-id="69d51-181">Remove explicit setting of VMSS in Windows example command since it is now default</span></span>

### <a name="iot"></a><span data-ttu-id="69d51-182">IoT</span><span class="sxs-lookup"><span data-stu-id="69d51-182">IoT</span></span>

* <span data-ttu-id="69d51-183">[CHANGEMENT CASSANT] `az iot pnp` : Suppression des commandes IoT PNP en préversion de l’interface CLI principale</span><span class="sxs-lookup"><span data-stu-id="69d51-183">[BREAKING CHANGE] `az iot pnp`: Remove IoT PNP preview commands from core CLI</span></span>

### <a name="rest"></a><span data-ttu-id="69d51-184">REST</span><span class="sxs-lookup"><span data-stu-id="69d51-184">REST</span></span>

* <span data-ttu-id="69d51-185">Correctif #14152 : `az rest` : URL ARM acceptées sans ID d’abonnement</span><span class="sxs-lookup"><span data-stu-id="69d51-185">Fix #14152: `az rest`: Accept ARM URLs without subscription ID</span></span>

### <a name="storage"></a><span data-ttu-id="69d51-186">Stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-186">Storage</span></span>

* <span data-ttu-id="69d51-187">Correctif #14138 : Autorisations rendues facultatives</span><span class="sxs-lookup"><span data-stu-id="69d51-187">Fix #14138: Make some permissions optional</span></span>

## <a name="july-14-2020"></a><span data-ttu-id="69d51-188">14 juillet 2020</span><span class="sxs-lookup"><span data-stu-id="69d51-188">July 14, 2020</span></span>

<span data-ttu-id="69d51-189">Version 2.9.0</span><span class="sxs-lookup"><span data-stu-id="69d51-189">Version 2.9.0</span></span>

### <a name="acr"></a><span data-ttu-id="69d51-190">ACR</span><span class="sxs-lookup"><span data-stu-id="69d51-190">ACR</span></span>

* <span data-ttu-id="69d51-191">Gestion du lien d’artefact de journal du Registre pour le streaming de journaux</span><span class="sxs-lookup"><span data-stu-id="69d51-191">Handle log artifact link from Registry to stream logs</span></span>
* <span data-ttu-id="69d51-192">Dépréciation des commandes helm2</span><span class="sxs-lookup"><span data-stu-id="69d51-192">Deprecate helm2 commands</span></span>

### <a name="aks"></a><span data-ttu-id="69d51-193">AKS</span><span class="sxs-lookup"><span data-stu-id="69d51-193">AKS</span></span>

* <span data-ttu-id="69d51-194">`az aks create` : ajout de l’argument --enable-aad</span><span class="sxs-lookup"><span data-stu-id="69d51-194">`az aks create`: add --enable-aad argument</span></span>
* <span data-ttu-id="69d51-195">`az aks update` : ajout de l’argument --enable-aad</span><span class="sxs-lookup"><span data-stu-id="69d51-195">`az aks update`: add --enable-aad argument</span></span>

### <a name="apim"></a><span data-ttu-id="69d51-196">APIM</span><span class="sxs-lookup"><span data-stu-id="69d51-196">APIM</span></span>

* <span data-ttu-id="69d51-197">Ajout de commandes d’API az apim générales</span><span class="sxs-lookup"><span data-stu-id="69d51-197">Added general az apim api commands</span></span>

### <a name="appconfig"></a><span data-ttu-id="69d51-198">AppConfig</span><span class="sxs-lookup"><span data-stu-id="69d51-198">AppConfig</span></span>

* <span data-ttu-id="69d51-199">Ajout d’un exemple d’utilisation de --fields dans appconfig revision</span><span class="sxs-lookup"><span data-stu-id="69d51-199">Add example for using --fields in appconfig revision</span></span>

### <a name="appservice"></a><span data-ttu-id="69d51-200">AppService</span><span class="sxs-lookup"><span data-stu-id="69d51-200">AppService</span></span>

* <span data-ttu-id="69d51-201">`az functionapp create`: prise en charge de Java 11 et de PowerShell 7.</span><span class="sxs-lookup"><span data-stu-id="69d51-201">`az functionapp create`: Added support for Java 11 and Powershell 7.</span></span> <span data-ttu-id="69d51-202">Prise en charge de l’API Stacks.</span><span class="sxs-lookup"><span data-stu-id="69d51-202">Added Stacks API Support.</span></span>
* <span data-ttu-id="69d51-203">Correction du problème #14208 entraînant l’échec de la création d’applications multiconteneurs</span><span class="sxs-lookup"><span data-stu-id="69d51-203">Fix #14208 multi-container app creation fails</span></span>
* <span data-ttu-id="69d51-204">Correction de az webapp create : utilisation de piles d’exécution codées en dur</span><span class="sxs-lookup"><span data-stu-id="69d51-204">Fix az webapp create - use hardcoded runtime stacks</span></span>

### <a name="arm"></a><span data-ttu-id="69d51-205">ARM</span><span class="sxs-lookup"><span data-stu-id="69d51-205">ARM</span></span>

* <span data-ttu-id="69d51-206">`az resource tag`: correction du problème concernant l’étiquetage des ressources avec le type de ressource `Microsoft.ContainerInstance/containerGroups`</span><span class="sxs-lookup"><span data-stu-id="69d51-206">`az resource tag`: Fix the problem of tagging resources with resource type `Microsoft.ContainerInstance/containerGroups`</span></span>

### <a name="compute"></a><span data-ttu-id="69d51-207">Calcul</span><span class="sxs-lookup"><span data-stu-id="69d51-207">Compute</span></span>

* <span data-ttu-id="69d51-208">Changement de version pour les disques (2020-05-01) et la capacité de calcul (2020-06-01)</span><span class="sxs-lookup"><span data-stu-id="69d51-208">Bump version disks 2020-05-01, compute 2020-06-01</span></span>
* <span data-ttu-id="69d51-209">Double chiffrement du jeu de chiffrement de disque</span><span class="sxs-lookup"><span data-stu-id="69d51-209">Double encryption of disk encryption set</span></span>
* <span data-ttu-id="69d51-210">`az vmss update` : prise en charge de la spécification d’une image interlocataire.</span><span class="sxs-lookup"><span data-stu-id="69d51-210">`az vmss update`: support specify cross tenant image.</span></span>
* <span data-ttu-id="69d51-211">`az sig image-version create` : prise en charge de la spécification d’une image interlocataire.</span><span class="sxs-lookup"><span data-stu-id="69d51-211">`az sig image-version create`: support specify cross tenant image.</span></span>
* <span data-ttu-id="69d51-212">vm/vmss create : chiffrement du cache et des données en transit pour les disques de système d’exploitation/de données et les disques temporaires pour les machines virtuelles et VMSS</span><span class="sxs-lookup"><span data-stu-id="69d51-212">vm/vmss create: Encryption of cache & data-in-transit for OS/Data disks and temp disks for VM & VMSS</span></span>
* <span data-ttu-id="69d51-213">Ajout d’une opération simulate-eviction pour les machines virtuelles et VMSS</span><span class="sxs-lookup"><span data-stu-id="69d51-213">Add simulate-eviction operation for VM and VMSS</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="69d51-214">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="69d51-214">CosmosDB</span></span>

* <span data-ttu-id="69d51-215">Fonctionnalités récentes : mise à l’échelle automatique, IpRules, EnableFreeTier et EnableAnalyticalStorage</span><span class="sxs-lookup"><span data-stu-id="69d51-215">Recent features: Autoscale, IpRules, EnableFreeTier and EnableAnalyticalStorage</span></span>

### <a name="eventgrid"></a><span data-ttu-id="69d51-216">EventGrid</span><span class="sxs-lookup"><span data-stu-id="69d51-216">EventGrid</span></span>

* <span data-ttu-id="69d51-217">Prise en charge de l’interface CLI pour 2020-04-01-preview et signalement des fonctionnalités en préversion avec is_Preview=True</span><span class="sxs-lookup"><span data-stu-id="69d51-217">Add CLI support for 2020-04-01-preview and mark preview features with is_Preview=True</span></span>

### <a name="find"></a><span data-ttu-id="69d51-218">Rechercher</span><span class="sxs-lookup"><span data-stu-id="69d51-218">Find</span></span>

* <span data-ttu-id="69d51-219">Correction du problème #14094 lié à az find entraînant l’échec des requêtes en l’absence de connexion et en cas de désactivation de la télémétrie</span><span class="sxs-lookup"><span data-stu-id="69d51-219">Fix #14094 az find Fix Queries failing when not logged in and when telemetry is disabled</span></span>

### <a name="hdinsight"></a><span data-ttu-id="69d51-220">HDInsight</span><span class="sxs-lookup"><span data-stu-id="69d51-220">HDInsight</span></span>

* <span data-ttu-id="69d51-221">Ajout de deux commandes pour prendre en charge la fonctionnalité de redémarrage de nœud HDInsight</span><span class="sxs-lookup"><span data-stu-id="69d51-221">Add two commands to support hdinsight node reboot feature</span></span>

### <a name="monitor"></a><span data-ttu-id="69d51-222">Superviser</span><span class="sxs-lookup"><span data-stu-id="69d51-222">Monitor</span></span>

* <span data-ttu-id="69d51-223">Suppression de l’indicateur de préversion pour les commandes sous l’espace de travail Log Analytics</span><span class="sxs-lookup"><span data-stu-id="69d51-223">Remove preview flag for commands under Log Analytics workspace</span></span>
* <span data-ttu-id="69d51-224">`az monitor diagnostic-settings subscription`: Prise en charge des paramètres de diagnostic pour l’abonnement</span><span class="sxs-lookup"><span data-stu-id="69d51-224">`az monitor diagnostic-settings subscription`: Support diagnositc settings for subscription</span></span>
* <span data-ttu-id="69d51-225">`az monitor metrics` : prise en charge de « , » et de « | » dans le nom des métriques</span><span class="sxs-lookup"><span data-stu-id="69d51-225">`az monitor metrics`: support ',' and '|' in metric name</span></span>
* <span data-ttu-id="69d51-226">`az monitor log-analytics workspace data-export` : prise en charge de l’exportation de données Log Analytics</span><span class="sxs-lookup"><span data-stu-id="69d51-226">`az monitor log-analytics workspace data-export`: support log analytics data export</span></span>

### <a name="network"></a><span data-ttu-id="69d51-227">Réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-227">Network</span></span>

* <span data-ttu-id="69d51-228">`az network application-gateway frontend-ip update`: Dépréciation du paramètre --public-ip-address</span><span class="sxs-lookup"><span data-stu-id="69d51-228">`az network application-gateway frontend-ip update`: Deprecating the --public-ip-address parameter</span></span>
* <span data-ttu-id="69d51-229">Passage à azure-mgmt-network 11.0.0</span><span class="sxs-lookup"><span data-stu-id="69d51-229">Bump azure-mgmt-network to 11.0.0</span></span>
* <span data-ttu-id="69d51-230">`az network express-route gateway connection` : prise en charge de la configuration du routage</span><span class="sxs-lookup"><span data-stu-id="69d51-230">`az network express-route gateway connection`: support routing configuration</span></span>
* <span data-ttu-id="69d51-231">`az network virtual-appliance`: prise en charge d’une appliance virtuelle réseau Azure.</span><span class="sxs-lookup"><span data-stu-id="69d51-231">`az network virtual-appliance`: Support Azure network virtual appliance.</span></span>
* <span data-ttu-id="69d51-232">Fonctionnalité de liaison privée prise en charge par Application Gateway</span><span class="sxs-lookup"><span data-stu-id="69d51-232">Application Gateway support private link feature</span></span>

### <a name="policyinsights"></a><span data-ttu-id="69d51-233">PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="69d51-233">PolicyInsights</span></span>

* <span data-ttu-id="69d51-234">`az policy state` : ajout de la commande trigger-scan pour déclencher des évaluations de conformité de la stratégie</span><span class="sxs-lookup"><span data-stu-id="69d51-234">`az policy state`: add trigger-scan command to trigger policy compliance evaluations</span></span>
* <span data-ttu-id="69d51-235">`az policy state list` : exposition des versions des entités de stratégie dans chaque enregistrement de conformité</span><span class="sxs-lookup"><span data-stu-id="69d51-235">`az policy state list`: expose versions of policy entities in each compliance record</span></span>

### <a name="profile"></a><span data-ttu-id="69d51-236">Profil</span><span class="sxs-lookup"><span data-stu-id="69d51-236">Profile</span></span>

* <span data-ttu-id="69d51-237">`az account get-access-token`: expiresOn visible pour l’identité managée</span><span class="sxs-lookup"><span data-stu-id="69d51-237">`az account get-access-token`: Show expiresOn for Managed Identity</span></span>

### <a name="rdbms"></a><span data-ttu-id="69d51-238">SGBDR</span><span class="sxs-lookup"><span data-stu-id="69d51-238">RDBMS</span></span>

* <span data-ttu-id="69d51-239">Prise en charge de la version TLS minimale</span><span class="sxs-lookup"><span data-stu-id="69d51-239">Support Minimum TLS version</span></span>
* <span data-ttu-id="69d51-240">Ajout du chiffrement d’infrastructure pour Azure Postgres et MySQL</span><span class="sxs-lookup"><span data-stu-id="69d51-240">Add Infrastructure Encryption for Azure Postgres and MySQL</span></span>

### <a name="security"></a><span data-ttu-id="69d51-241">Sécurité</span><span class="sxs-lookup"><span data-stu-id="69d51-241">Security</span></span>

* <span data-ttu-id="69d51-242">Ajout des commandes allowed_connections</span><span class="sxs-lookup"><span data-stu-id="69d51-242">Add allowed_connections commands</span></span>
* <span data-ttu-id="69d51-243">Ajout de commandes de renforcement du réseau adaptatif</span><span class="sxs-lookup"><span data-stu-id="69d51-243">Add Adaptive network hardeningss commands</span></span>
* <span data-ttu-id="69d51-244">Ajout des commandes adaptive_application_controls</span><span class="sxs-lookup"><span data-stu-id="69d51-244">Add adaptive_application_controls commands</span></span>
* <span data-ttu-id="69d51-245">Ajout de az security iot-solution/ iot-alerts/iot-recommendations/iot-analytics (REST) à Azure CLI</span><span class="sxs-lookup"><span data-stu-id="69d51-245">Addition of az security iot-solution/ iot-alerts/iot-recommendations/iot-analytics REST to Azure CLI</span></span>
* <span data-ttu-id="69d51-246">Ajout d’une interface CLI conforme à la réglementation</span><span class="sxs-lookup"><span data-stu-id="69d51-246">Add regulatory compliance CLI</span></span>

### <a name="signalr"></a><span data-ttu-id="69d51-247">SignalR</span><span class="sxs-lookup"><span data-stu-id="69d51-247">SignalR</span></span>

* <span data-ttu-id="69d51-248">Ajout de fonctionnalités, notamment la gestion des connexions de point de terminaison privé, des règles réseau et du trafic en amont</span><span class="sxs-lookup"><span data-stu-id="69d51-248">Add features including managing private endpoint connections, network rules and upstream</span></span>

### <a name="sql"></a><span data-ttu-id="69d51-249">SQL</span><span class="sxs-lookup"><span data-stu-id="69d51-249">SQL</span></span>

* <span data-ttu-id="69d51-250">`az sql mi create`, `az sql mi update` : ajout du paramètre `--tags` pour prendre en charge l’étiquetage des ressources</span><span class="sxs-lookup"><span data-stu-id="69d51-250">`az sql mi create`, `az sql mi update`: Add `--tags` parameter to support resource tagging</span></span>
* <span data-ttu-id="69d51-251">`az sql mi failover`: prise en charge du basculement à partir du point principal ou secondaire</span><span class="sxs-lookup"><span data-stu-id="69d51-251">`az sql mi failover`: Support failover from primary or secondary point</span></span>

### <a name="storage"></a><span data-ttu-id="69d51-252">Stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-252">Storage</span></span>

* <span data-ttu-id="69d51-253">`az storage account create/update`: ajout de --allow-blob-public-access pour autoriser ou interdire l’accès public pour les objets blob et les conteneurs</span><span class="sxs-lookup"><span data-stu-id="69d51-253">`az storage account create/update`: Add --allow-blob-public-access to allow or disallow public access for blob and containers</span></span>
* <span data-ttu-id="69d51-254">`az storage account create/update`: ajout de `--min-tls-version` pour prendre en charge la configuration de la version TLS minimale à autoriser sur les demandes de stockage.</span><span class="sxs-lookup"><span data-stu-id="69d51-254">`az storage account create/update`: Add `--min-tls-version` to support setting the minimum TLS version to be permitted on requests to storage.</span></span>
* <span data-ttu-id="69d51-255">Suppression de l’archivage des informations d’identification des jetons</span><span class="sxs-lookup"><span data-stu-id="69d51-255">Remove check in token credential</span></span>
* <span data-ttu-id="69d51-256">Correction du nom du compte de stockage dans les exemples</span><span class="sxs-lookup"><span data-stu-id="69d51-256">Fix the storage account name in examples</span></span>

### <a name="webapp"></a><span data-ttu-id="69d51-257">Webapp</span><span class="sxs-lookup"><span data-stu-id="69d51-257">Webapp</span></span>

* <span data-ttu-id="69d51-258">Correction d’un bogue lié à az webapp log deployment show : des journaux de déploiement sont retournés au lieu de métadonnées de journaux</span><span class="sxs-lookup"><span data-stu-id="69d51-258">Bugfix: az webapp log deployment show - return deployment logs instead of log metadata</span></span>
* <span data-ttu-id="69d51-259">Correction d’un bogue lié à az webapp vnet-integration add : correction de la gestion des erreurs en cas de nom de réseau virtuel incorrect et prise en charge de l’ID de ressource de réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="69d51-259">Bugfix: az webapp vnet-integration add - fix error handling if bad vnet name, support vnet resource ID</span></span>

## <a name="june-23-2020"></a><span data-ttu-id="69d51-260">23 juin 2020</span><span class="sxs-lookup"><span data-stu-id="69d51-260">June 23, 2020</span></span>

<span data-ttu-id="69d51-261">Version 2.8.0</span><span class="sxs-lookup"><span data-stu-id="69d51-261">Version 2.8.0</span></span>

### <a name="acr"></a><span data-ttu-id="69d51-262">ACR</span><span class="sxs-lookup"><span data-stu-id="69d51-262">ACR</span></span>

* <span data-ttu-id="69d51-263">Prise en charge de la désactivation du routage/du point de terminaison d’une région</span><span class="sxs-lookup"><span data-stu-id="69d51-263">Add support for region endpoint disable / routing disable</span></span>
* <span data-ttu-id="69d51-264">[CHANGEMENT CASSANT] `az acr login --expose-token` n’accepte pas un nom d’utilisateur et un mot de passe</span><span class="sxs-lookup"><span data-stu-id="69d51-264">[BREAKING CHANGE] `az acr login --expose-token` does not accept username and password</span></span>

### <a name="acs"></a><span data-ttu-id="69d51-265">ACS</span><span class="sxs-lookup"><span data-stu-id="69d51-265">ACS</span></span>

* <span data-ttu-id="69d51-266">Suppression du cluster privé et de l’API 2019-10-27-preview</span><span class="sxs-lookup"><span data-stu-id="69d51-266">Remove private cluster and 2019-10-27-preview API</span></span>

### <a name="aks"></a><span data-ttu-id="69d51-267">AKS</span><span class="sxs-lookup"><span data-stu-id="69d51-267">AKS</span></span>

* <span data-ttu-id="69d51-268">Prise en charge de --yes pour la commande az aks upgrade</span><span class="sxs-lookup"><span data-stu-id="69d51-268">Support --yes for az aks upgrade</span></span>
* <span data-ttu-id="69d51-269">Rétablissement du « remplacement de la référence SKU de machine virtuelle par défaut par Standard_D2s_v3 (#13541) »</span><span class="sxs-lookup"><span data-stu-id="69d51-269">Revert "change default vm sku to Standard_D2s_v3 (#13541)"</span></span>
* <span data-ttu-id="69d51-270">Ajout de « az aks update --uptime-sla »</span><span class="sxs-lookup"><span data-stu-id="69d51-270">Add "az aks update --uptime-sla"</span></span>
* <span data-ttu-id="69d51-271">Correction d’une faute de frappe dans la commande az aks update</span><span class="sxs-lookup"><span data-stu-id="69d51-271">Fix typo in az aks update command</span></span>
* <span data-ttu-id="69d51-272">Prise en charge d’un pool d’agents avec 0 nœud et blocage de la mise à l’échelle manuelle pour le pool compatible CAS</span><span class="sxs-lookup"><span data-stu-id="69d51-272">Change to support 0 node agent pool and block manual scale for CAS enabled pool</span></span>
* <span data-ttu-id="69d51-273">Correction d’une faute de frappe dans VirtualMachineScaleSets et mise à jour des références avec les versions de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="69d51-273">Fix typo on VirtualMachineScaleSets and update references to Kubernetes versions</span></span>

### <a name="ams"></a><span data-ttu-id="69d51-274">AMS</span><span class="sxs-lookup"><span data-stu-id="69d51-274">AMS</span></span>

* <span data-ttu-id="69d51-275">Remplacement du texte d’aide pour le paramètre « --expiry ».</span><span class="sxs-lookup"><span data-stu-id="69d51-275">CHANGE help text for "--expiry" parameter.</span></span>

### <a name="appservice"></a><span data-ttu-id="69d51-276">AppService</span><span class="sxs-lookup"><span data-stu-id="69d51-276">AppService</span></span>

* <span data-ttu-id="69d51-277">`az webapp log deployment show`: Affichage du dernier journal de déploiement ou des journaux de déploiement d’un déploiement spécifique si deployment-id est spécifié</span><span class="sxs-lookup"><span data-stu-id="69d51-277">`az webapp log deployment show`: Show the latest deployment log, or the deployment logs of a specific deployment if deployment-id is specified</span></span>
* <span data-ttu-id="69d51-278">`az webapp log deployment list`: Liste des journaux de déploiement disponible</span><span class="sxs-lookup"><span data-stu-id="69d51-278">`az webapp log deployment list`: List of deployment logs available</span></span>
* <span data-ttu-id="69d51-279">Correctif : Affichage d’une erreur quand le nom webapp fourni n’est pas valide</span><span class="sxs-lookup"><span data-stu-id="69d51-279">Fix: Surface error when invalid webapp name provided</span></span>
* <span data-ttu-id="69d51-280">Correctif #13261 : az webapp list-runtimes utilise une liste statique jusqu’à ce qu’une nouvelle API Available Stacks soit disponible</span><span class="sxs-lookup"><span data-stu-id="69d51-280">Fix #13261 az webapp list-runtimes use static list until new Available Stacks API is available</span></span>
* <span data-ttu-id="69d51-281">`az appservice ase create`: Correction d’un problème de création (#13361)</span><span class="sxs-lookup"><span data-stu-id="69d51-281">`az appservice ase create`: Fix create issue #13361</span></span>
* <span data-ttu-id="69d51-282">`az appservice ase list-addresses`: Correction d’un problème de changement de SDK (#13140).</span><span class="sxs-lookup"><span data-stu-id="69d51-282">`az appservice ase list-addresses`: Fix change of SDK #13140.</span></span>
* <span data-ttu-id="69d51-283">Correction d’un problème de création d’une application web/d’un emplacement pour les conteneurs Windows</span><span class="sxs-lookup"><span data-stu-id="69d51-283">Fix webapp/slot creation for Windows Containers</span></span>
* <span data-ttu-id="69d51-284">`az webapp auth update`: Ajout d’un paramètre facultatif pour mettre à jour runtime-version</span><span class="sxs-lookup"><span data-stu-id="69d51-284">`az webapp auth update`: Add optional parameter to update runtime-version</span></span>
* <span data-ttu-id="69d51-285">Prise en charge des commandes list, delete, approve et reject sur une connexion de point de terminaison privée pour une application web dans CLI</span><span class="sxs-lookup"><span data-stu-id="69d51-285">Support list, delete, approve and reject private endpoint connection for webapp in CLI</span></span>
* <span data-ttu-id="69d51-286">Correctif #13888 : Prise en charge des commandes get, list et create pour les applications web statiques</span><span class="sxs-lookup"><span data-stu-id="69d51-286">Fix #13888 : Add support for Static WebApps: get, list, create commands</span></span>
* <span data-ttu-id="69d51-287">Amélioration des messages d’erreur pour la connexion du tunnel SSH</span><span class="sxs-lookup"><span data-stu-id="69d51-287">Improved error messages for SSH Tunnel Connection</span></span>

### <a name="arm"></a><span data-ttu-id="69d51-288">ARM</span><span class="sxs-lookup"><span data-stu-id="69d51-288">ARM</span></span>

* <span data-ttu-id="69d51-289">`az tag`: Ajout d’exemples pour -h</span><span class="sxs-lookup"><span data-stu-id="69d51-289">`az tag`: Add examples for -h</span></span>
* <span data-ttu-id="69d51-290">`az deployment group/sub what-if`: Ajout du paramètre --exclude-change-types/-x.</span><span class="sxs-lookup"><span data-stu-id="69d51-290">`az deployment group/sub what-if`: Add --exclude-change-types/-x parameter.</span></span>
* <span data-ttu-id="69d51-291">`az deployment group/sub/mg/tenant create`: Ajout du paramètre --what-if-exclude-change-types/-x.</span><span class="sxs-lookup"><span data-stu-id="69d51-291">`az deployment group/sub/mg/tenant create`: Add --what-if-exclude-change-types/-x parameter.</span></span>
* <span data-ttu-id="69d51-292">`az deployment group/sub/mg/tenant validate`: Amélioration du format des messages d’erreur.</span><span class="sxs-lookup"><span data-stu-id="69d51-292">`az deployment group/sub/mg/tenant validate`: Show error messages in a better format.</span></span>
* <span data-ttu-id="69d51-293">`az group export`: Ajout des nouveaux paramètres `--skip-resource-name-params` et `--skip-all-params` pour ignorer le paramétrage</span><span class="sxs-lookup"><span data-stu-id="69d51-293">`az group export`: Add new parameters `--skip-resource-name-params` and `--skip-all-params` to support skip parameterization</span></span>
* <span data-ttu-id="69d51-294">Ajout de az feature unregister api</span><span class="sxs-lookup"><span data-stu-id="69d51-294">Add az feature unregister api</span></span>

### <a name="aro"></a><span data-ttu-id="69d51-295">ARO</span><span class="sxs-lookup"><span data-stu-id="69d51-295">ARO</span></span>

* <span data-ttu-id="69d51-296">Ajout de Public et de Private aux paramètres pour améliorer la visibilité de l’entrée/du serveur d’API</span><span class="sxs-lookup"><span data-stu-id="69d51-296">Add Public, Private to params for help with ingress/apiserver visibility</span></span>

### <a name="batch"></a><span data-ttu-id="69d51-297">Batch</span><span class="sxs-lookup"><span data-stu-id="69d51-297">Batch</span></span>

* <span data-ttu-id="69d51-298">`az batch account create`: Ajout du nouveau paramètre `--public-network-access`</span><span class="sxs-lookup"><span data-stu-id="69d51-298">`az batch account create`: Add new parameter `--public-network-access`</span></span>
* <span data-ttu-id="69d51-299">`az batch account create`: Ajout du nouveau paramètre `--identity-type`</span><span class="sxs-lookup"><span data-stu-id="69d51-299">`az batch account create`: Add new parameter `--identity-type`</span></span>
* <span data-ttu-id="69d51-300">`az batch account set`: Ajout du nouveau paramètre `--identity-type`</span><span class="sxs-lookup"><span data-stu-id="69d51-300">`az batch account set`: Add new parameter `--identity-type`</span></span>
* <span data-ttu-id="69d51-301">[CHANGEMENT CASSANT] az batch pool create : Si vous créez un pool à l’aide d’une image personnalisée, la propriété --image ne peut désormais faire référence qu’à une image de Shared Image Gallery.</span><span class="sxs-lookup"><span data-stu-id="69d51-301">[BREAKING CHANGE] az batch pool create: When creating a pool using a custom image, the --image property of can now only refer to a Shared Image Gallery image.</span></span>
* <span data-ttu-id="69d51-302">[CHANGEMENT CASSANT] az batch pool create : Si vous créez un pool avec l’option --json-file et spécifiez networkConfiguration, la propriété publicIPs se trouve désormais dans la nouvelle propriété publicIPAddressConfiguration.</span><span class="sxs-lookup"><span data-stu-id="69d51-302">[BREAKING CHANGE] az batch pool create: When creating a pool with --json-file option and specifying a networkConfiguration, the publicIPs property has moved in to a new property publicIPAddressConfiguration.</span></span> <span data-ttu-id="69d51-303">Cette nouvelle propriété accepte également une nouvelle propriété ipAddressProvisioningType qui spécifie comment le pool doit allouer les adresses IP ainsi qu’une propriété publicIPs qui permet de configurer une liste de ressources PublicIP à utiliser si ipAddressProvisioningType a la valeur UserManaged.</span><span class="sxs-lookup"><span data-stu-id="69d51-303">This new property also supports a new ipAddressProvisioningType property which specifies how the pool should allocate IP's and a publicIPs property which allows for configuration of a list of PublicIP resources to use in the case ipAddressProvisioningType is set to UserManaged</span></span>
* <span data-ttu-id="69d51-304">`az network private-link-resource`: Prise en charge de la ressource Microsoft.Batch batchAccount</span><span class="sxs-lookup"><span data-stu-id="69d51-304">`az network private-link-resource`: Add support for the Microsoft.Batch batchAccount resource</span></span>
* <span data-ttu-id="69d51-305">`az network private-endpoint-connection`: Prise en charge de la ressource Microsoft.Batch batchAccount</span><span class="sxs-lookup"><span data-stu-id="69d51-305">`az network private-endpoint-connection`: Add support for the Microsoft.Batch batchAccount resource</span></span>

### <a name="cdn"></a><span data-ttu-id="69d51-306">CDN</span><span class="sxs-lookup"><span data-stu-id="69d51-306">CDN</span></span>

* <span data-ttu-id="69d51-307">`az cdn custom-domain enable-https`: Prise en charge de BYOC.</span><span class="sxs-lookup"><span data-stu-id="69d51-307">`az cdn custom-domain enable-https`: Add BYOC support.</span></span>
* <span data-ttu-id="69d51-308">`az cdn custom-domain enable-https`: Correction de l’activation du protocole HTTPS personnalisé avec des certificats gérés par CDN pour les références SKU Standard_Verizon et Standard_Microsoft.</span><span class="sxs-lookup"><span data-stu-id="69d51-308">`az cdn custom-domain enable-https`: Fix enabling custom HTTPS with CDN managed certificates for Standard_Verizon and Standard_Microsoft SKUs.</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="69d51-309">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="69d51-309">Cognitive Services</span></span>

* <span data-ttu-id="69d51-310">[CHANGEMENT CASSANT] `az cognitiveservices account` présente maintenant une structure unifiée pour toutes les commandes.</span><span class="sxs-lookup"><span data-stu-id="69d51-310">[BREAKING CHANGE] `az cognitiveservices account` now have a unified structure for all commands.</span></span>
* <span data-ttu-id="69d51-311">`az cognitiveservices account identity`: Ajout de la gestion des identités pour Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="69d51-311">`az cognitiveservices account identity`: Add identity management for Cognitive Services.</span></span>

### <a name="compute"></a><span data-ttu-id="69d51-312">Calcul</span><span class="sxs-lookup"><span data-stu-id="69d51-312">Compute</span></span>

* <span data-ttu-id="69d51-313">`az image builder`: Mise à niveau vers la version d’API 2020-02-14</span><span class="sxs-lookup"><span data-stu-id="69d51-313">`az image builder`: Upgrade API version to 2020-02-14</span></span>
* <span data-ttu-id="69d51-314">`az image builder create`: Ajout de `--identity` pour prendre en charge la configuration d’identité</span><span class="sxs-lookup"><span data-stu-id="69d51-314">`az image builder create`: Add `--identity` to support identity configuration</span></span>
* <span data-ttu-id="69d51-315">`az image builder customizer add`: Prise en charge du personnalisateur de mise à jour de Windows</span><span class="sxs-lookup"><span data-stu-id="69d51-315">`az image builder customizer add`: Support Windows update customizer</span></span>
* <span data-ttu-id="69d51-316">Nouvelle commande `az image builder cancel`</span><span class="sxs-lookup"><span data-stu-id="69d51-316">New command `az image builder cancel`</span></span>
* <span data-ttu-id="69d51-317">Affiche un avertissement quand un utilisateur déploie un VMSS épinglé à une version d’image spécifique plutôt que la dernière version</span><span class="sxs-lookup"><span data-stu-id="69d51-317">Show a warning when a user deploys a VMSS pinned to a specific image version rather than latest</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="69d51-318">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="69d51-318">Cosmos DB</span></span>

* <span data-ttu-id="69d51-319">`az cosmosdb`: Ajout de la commande exists à la base de données et aux groupes de conteneurs</span><span class="sxs-lookup"><span data-stu-id="69d51-319">`az cosmosdb`: Add exists command to database and container groups</span></span>
* <span data-ttu-id="69d51-320">Création de collections fixes</span><span class="sxs-lookup"><span data-stu-id="69d51-320">Allow creating fixed collections</span></span>

### <a name="eventhub"></a><span data-ttu-id="69d51-321">Event Hub</span><span class="sxs-lookup"><span data-stu-id="69d51-321">EventHub</span></span>

* <span data-ttu-id="69d51-322">`az eventhubs namespace create` : Ajout de paramètres liés aux identités managées</span><span class="sxs-lookup"><span data-stu-id="69d51-322">`az eventhubs namespace create` : Add managed identity parameters</span></span>

### <a name="extension"></a><span data-ttu-id="69d51-323">Extension</span><span class="sxs-lookup"><span data-stu-id="69d51-323">Extension</span></span>

* <span data-ttu-id="69d51-324">Ajout de --version pour prendre en charge une installation à partir d’une version spécifique</span><span class="sxs-lookup"><span data-stu-id="69d51-324">Add --version to support to install from a specific version</span></span>
* <span data-ttu-id="69d51-325">Activation des extensions CLI pour inclure des packages dans l’espace de noms « azure »</span><span class="sxs-lookup"><span data-stu-id="69d51-325">Enable CLI extensions to include packages in the 'azure' namespace</span></span>

### <a name="iot-hub"></a><span data-ttu-id="69d51-326">IoT Hub</span><span class="sxs-lookup"><span data-stu-id="69d51-326">Iot Hub</span></span>

* <span data-ttu-id="69d51-327">[CHANGEMENT CASSANT] az iot hub job : Suppression des commandes de tâches dépréciées</span><span class="sxs-lookup"><span data-stu-id="69d51-327">[BREAKING CHANGE] az iot hub job: Remove deprecated job commands</span></span>

### <a name="keyvault"></a><span data-ttu-id="69d51-328">KeyVault</span><span class="sxs-lookup"><span data-stu-id="69d51-328">KeyVault</span></span>

* <span data-ttu-id="69d51-329">`az keyvault key import`: Prend en charge l’importation à partir de chaînes avec deux nouveaux paramètres.</span><span class="sxs-lookup"><span data-stu-id="69d51-329">`az keyvault key import`: Supports importing from strings via two new parameters.</span></span>
* <span data-ttu-id="69d51-330">Prend en charge le chiffrement et le déchiffrement des chaînes/octets avec des clés stockées</span><span class="sxs-lookup"><span data-stu-id="69d51-330">Support string/bytes encryption and decryption with stored keys</span></span>

### <a name="monitor"></a><span data-ttu-id="69d51-331">Superviser</span><span class="sxs-lookup"><span data-stu-id="69d51-331">Monitor</span></span>

* <span data-ttu-id="69d51-332">Prend en charge la création d’un cluster sans attente</span><span class="sxs-lookup"><span data-stu-id="69d51-332">Support no wait for cluster creation</span></span>
* <span data-ttu-id="69d51-333">`az monitor log-analytics workspace saved-search`: Prendre en charge de nouvelles commandes pour la recherche enregistrée</span><span class="sxs-lookup"><span data-stu-id="69d51-333">`az monitor log-analytics workspace saved-search`: Support new commands for saved search</span></span>

### <a name="network"></a><span data-ttu-id="69d51-334">Réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-334">Network</span></span>

* <span data-ttu-id="69d51-335">`az network application-gateway address-pool update`: Amélioration du message d’aide et ajout d’exemples.</span><span class="sxs-lookup"><span data-stu-id="69d51-335">`az network application-gateway address-pool update`: Refine help message and add examples.</span></span>
* <span data-ttu-id="69d51-336">`az network vnet create`: Prise en charge de l’argument --nsg</span><span class="sxs-lookup"><span data-stu-id="69d51-336">`az network vnet create`: Support --nsg argument</span></span>
* <span data-ttu-id="69d51-337">`az network lb address-pool`: Prise en charge la création de pool de back-ends lb avec une adresse de back-end.</span><span class="sxs-lookup"><span data-stu-id="69d51-337">`az network lb address-pool`: Support create lb backend pool with backend address.</span></span>
* <span data-ttu-id="69d51-338">`az network application-gateway address-pool`: Ajout d’un correctif pour l’argument --add</span><span class="sxs-lookup"><span data-stu-id="69d51-338">`az network application-gateway address-pool`: Fix for --add argument</span></span>

### <a name="rbac"></a><span data-ttu-id="69d51-339">RBAC</span><span class="sxs-lookup"><span data-stu-id="69d51-339">RBAC</span></span>

* <span data-ttu-id="69d51-340">`az ad sp create-for-rabc`: Prise en charge des noms avec un espace, une barre oblique et une barre oblique inverse</span><span class="sxs-lookup"><span data-stu-id="69d51-340">`az ad sp create-for-rabc`: Support name with space, slash and back slash</span></span>
* <span data-ttu-id="69d51-341">`az ad sp create-for-rbac`: Amélioration du message d’erreur si l’utilisateur spécifie une étendue non valide</span><span class="sxs-lookup"><span data-stu-id="69d51-341">`az ad sp create-for-rbac`: Refine error message when user specify an invalid scope</span></span>

### <a name="security"></a><span data-ttu-id="69d51-342">Sécurité</span><span class="sxs-lookup"><span data-stu-id="69d51-342">Security</span></span>

* <span data-ttu-id="69d51-343">Ajout de commandes d’évaluation de la sécurité</span><span class="sxs-lookup"><span data-stu-id="69d51-343">Add security assessment commands</span></span>

### <a name="sql"></a><span data-ttu-id="69d51-344">SQL</span><span class="sxs-lookup"><span data-stu-id="69d51-344">SQL</span></span>

* <span data-ttu-id="69d51-345">`az sql db ltr-policy/ltr-backup` : mise à jour/affichage de la stratégie de conservation à long terme, affichage/suppression des sauvegardes de conservation à long terme, restauration de la sauvegarde de conservation à long terme</span><span class="sxs-lookup"><span data-stu-id="69d51-345">`az sql db ltr-policy/ltr-backup`: update/show long term retention policy, show/delete long term retention backups, restore long term retention backup</span></span>

### <a name="storage"></a><span data-ttu-id="69d51-346">Stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-346">Storage</span></span>

* <span data-ttu-id="69d51-347">Résolution d’un problème d’authentification pour prendre en charge l’obtention d’un jeton pour --subscription</span><span class="sxs-lookup"><span data-stu-id="69d51-347">Fix authentication issue to support get token for --subscription</span></span>
* <span data-ttu-id="69d51-348">`az storage remove`: Résolution du problème #13459 pour lever une exception en cas d’échec de l’opération</span><span class="sxs-lookup"><span data-stu-id="69d51-348">`az storage remove`: Fix issue #13459 to raise exception for operation failure</span></span>
* <span data-ttu-id="69d51-349">Résolution des problèmes #13012, #13632 et #13657 pour supprimer les arguments inutilisés pour les commandes associées à generate-sas</span><span class="sxs-lookup"><span data-stu-id="69d51-349">Fix issues #13012, #13632 and #13657 to remove unused arguments for generate-sas related commands</span></span>
* <span data-ttu-id="69d51-350">`az storage logging update`: Ajout d’une vérification de la version de journalisation</span><span class="sxs-lookup"><span data-stu-id="69d51-350">`az storage logging update`: Add check for logging version</span></span>
* <span data-ttu-id="69d51-351">`az storage blob show`: Ajout de propriétés supplémentaires à l’objet blob avec le SDK Track 2</span><span class="sxs-lookup"><span data-stu-id="69d51-351">`az storage blob show`: Add more properties for blob with track 2 SDK</span></span>
* <span data-ttu-id="69d51-352">Correctif #13708 : Amélioration du message d’avertissement relatif aux informations d’identification</span><span class="sxs-lookup"><span data-stu-id="69d51-352">Fix #13708: Refine warning message for credential</span></span>
* <span data-ttu-id="69d51-353">`az storage share-rm create/update`: Prise en charge du protocole NFS et du squash racine</span><span class="sxs-lookup"><span data-stu-id="69d51-353">`az storage share-rm create/update`: Add NFS protocol and root squash support</span></span>
* <span data-ttu-id="69d51-354">`az storage account create`: Prise en charge du double chiffrement</span><span class="sxs-lookup"><span data-stu-id="69d51-354">`az storage account create`: Add support for double encryption</span></span>
* <span data-ttu-id="69d51-355">[CHANGEMENT CASSANT] `az storage blob/container/file/share/table/queue generate-sas` : --expiry et --permissions sont obligatoires</span><span class="sxs-lookup"><span data-stu-id="69d51-355">[BREAKING CHANGE] `az storage blob/container/file/share/table/queue generate-sas`: make --expiry and --permissions required</span></span>
* <span data-ttu-id="69d51-356">`az storage blob set-tier`: Migration vers Track 2 pour prendre en charge la définition de la priorité de réhydratation</span><span class="sxs-lookup"><span data-stu-id="69d51-356">`az storage blob set-tier`: Migrate to Track 2 to support setting rehydrate priority</span></span>

## <a name="june-02-2020"></a><span data-ttu-id="69d51-357">2 juin 2020</span><span class="sxs-lookup"><span data-stu-id="69d51-357">June 02, 2020</span></span>

<span data-ttu-id="69d51-358">Version 2.7.0</span><span class="sxs-lookup"><span data-stu-id="69d51-358">Version 2.7.0</span></span>

### <a name="acr"></a><span data-ttu-id="69d51-359">ACR</span><span class="sxs-lookup"><span data-stu-id="69d51-359">ACR</span></span>

* <span data-ttu-id="69d51-360">Correction d’une faute de frappe dans un message d’erreur de création de jeton</span><span class="sxs-lookup"><span data-stu-id="69d51-360">Fix a typo in an error message of token creation</span></span>

### <a name="aks"></a><span data-ttu-id="69d51-361">AKS</span><span class="sxs-lookup"><span data-stu-id="69d51-361">AKS</span></span>

* <span data-ttu-id="69d51-362">Remplacement de la référence SKU de machine virtuelle par défaut par Standard_D2s_v3</span><span class="sxs-lookup"><span data-stu-id="69d51-362">Change default vm sku to Standard_D2s_v3</span></span>
* <span data-ttu-id="69d51-363">Correction de la création d’attribution de rôle pour le cluster MSI plus le sous-réseau personnalisé</span><span class="sxs-lookup"><span data-stu-id="69d51-363">Fix creating role assignment for MSI clsuter plus custom subnet</span></span>

### <a name="appservice"></a><span data-ttu-id="69d51-364">AppService</span><span class="sxs-lookup"><span data-stu-id="69d51-364">AppService</span></span>

* <span data-ttu-id="69d51-365">Correctif #12739 az appservice list-locations retourne des emplacements non valides</span><span class="sxs-lookup"><span data-stu-id="69d51-365">Fix #12739 az appservice list-locations returns some invalid locations</span></span>

### <a name="arm"></a><span data-ttu-id="69d51-366">ARM</span><span class="sxs-lookup"><span data-stu-id="69d51-366">ARM</span></span>

* <span data-ttu-id="69d51-367">`az deployment`: Correction du problème #13159 concernant un message JSON incorrect après la suppression de commentaires et la compression</span><span class="sxs-lookup"><span data-stu-id="69d51-367">`az deployment`: Fix issue #13159 of incorrect message of JSON after removing comments and compressing</span></span>
* <span data-ttu-id="69d51-368">`az resource tag`: Correction du problème #13255 concernant l’étiquetage des ressources avec le type de ressource `Microsoft.ContainerRegistry/registries/webhooks`</span><span class="sxs-lookup"><span data-stu-id="69d51-368">`az resource tag`: Fix issue #13255 of tagging resources with resource type `Microsoft.ContainerRegistry/registries/webhooks`</span></span>
* <span data-ttu-id="69d51-369">Amélioration des exemples pour le module de ressources</span><span class="sxs-lookup"><span data-stu-id="69d51-369">Improve the examples for the resource module</span></span>

### <a name="aro"></a><span data-ttu-id="69d51-370">ARO</span><span class="sxs-lookup"><span data-stu-id="69d51-370">ARO</span></span>

* <span data-ttu-id="69d51-371">Remplacement de CLIError par un indicateur correct pour --worker-vm-disk-size-gb</span><span class="sxs-lookup"><span data-stu-id="69d51-371">Change CLIError to correct flag for --worker-vm-disk-size-gb</span></span>

### <a name="eventhub"></a><span data-ttu-id="69d51-372">Event Hub</span><span class="sxs-lookup"><span data-stu-id="69d51-372">EventHub</span></span>

* <span data-ttu-id="69d51-373">Correction du problème #12406 où l’argument --capture-interval ne mettait pas à jour « intervalInSeconds »</span><span class="sxs-lookup"><span data-stu-id="69d51-373">Fix for issue #12406 Argument --capture-interval does not update the "intervalInSeconds"</span></span>

### <a name="hdinsight"></a><span data-ttu-id="69d51-374">HDInsight</span><span class="sxs-lookup"><span data-stu-id="69d51-374">HDInsight</span></span>

* <span data-ttu-id="69d51-375">Remplacement de get_json_object par shell_safe_json_parse</span><span class="sxs-lookup"><span data-stu-id="69d51-375">Change get_json_object to shell_safe_json_parse</span></span>

### <a name="monitor"></a><span data-ttu-id="69d51-376">Superviser</span><span class="sxs-lookup"><span data-stu-id="69d51-376">Monitor</span></span>

* <span data-ttu-id="69d51-377">`az monitor metrics alert` : amélioration de plusieurs messages d’aide</span><span class="sxs-lookup"><span data-stu-id="69d51-377">`az monitor metrics alert`: refine several help messages</span></span>
* <span data-ttu-id="69d51-378">`az monitor diagnostic-settings create` : prise en charge de l’argument --export-to-resource-specific</span><span class="sxs-lookup"><span data-stu-id="69d51-378">`az monitor diagnostic-settings create`: support --export-to-resource-specific argument</span></span>
* <span data-ttu-id="69d51-379">Prise en charge de la récupération de l’espace de travail LA</span><span class="sxs-lookup"><span data-stu-id="69d51-379">Support LA workspace recover</span></span>

### <a name="network"></a><span data-ttu-id="69d51-380">Réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-380">Network</span></span>

* <span data-ttu-id="69d51-381">`az network dns zone` : prise en charge du caractère -</span><span class="sxs-lookup"><span data-stu-id="69d51-381">`az network dns zone`: support - character</span></span>
* <span data-ttu-id="69d51-382">`az network vpn-connection ipsec-policy` : remplacement de --sa-lifetime et --sa-max-size par de plus grandes valeurs dans l’exemple</span><span class="sxs-lookup"><span data-stu-id="69d51-382">`az network vpn-connection ipsec-policy`: change the --sa-lifetime and --sa-max-size to larger values in example</span></span>
* <span data-ttu-id="69d51-383">Passage du réseau à 2020-04-01</span><span class="sxs-lookup"><span data-stu-id="69d51-383">Bump network to 2020-04-01</span></span>
* <span data-ttu-id="69d51-384">`az network private-endpoint-connection` : prise en charge de la grille d’événement</span><span class="sxs-lookup"><span data-stu-id="69d51-384">`az network private-endpoint-connection`: support event grid</span></span>
* <span data-ttu-id="69d51-385">`az network express-route list-route-tables` : correction du bogue qui empêchait de lister les routes sous forme de table</span><span class="sxs-lookup"><span data-stu-id="69d51-385">`az network express-route list-route-tables`: fix bug that cannot list routes as table</span></span>

### <a name="packaging"></a><span data-ttu-id="69d51-386">Packaging</span><span class="sxs-lookup"><span data-stu-id="69d51-386">Packaging</span></span>

* <span data-ttu-id="69d51-387">Ajout du package Ubuntu Focal</span><span class="sxs-lookup"><span data-stu-id="69d51-387">Add Ubuntu Focal Package</span></span>

### <a name="rbac"></a><span data-ttu-id="69d51-388">RBAC</span><span class="sxs-lookup"><span data-stu-id="69d51-388">RBAC</span></span>

* <span data-ttu-id="69d51-389">`az ad sp credential reset` : modification de la génération d’informations d’identification pour éviter des caractères spéciaux posant problème</span><span class="sxs-lookup"><span data-stu-id="69d51-389">`az ad sp credential reset`: modify credential generation to avoid troublesome special characters</span></span>

### <a name="redis"></a><span data-ttu-id="69d51-390">Redis</span><span class="sxs-lookup"><span data-stu-id="69d51-390">Redis</span></span>

* <span data-ttu-id="69d51-391">Correctif #13529 : Modification de la documentation du paramètre enable_non_ssl_port</span><span class="sxs-lookup"><span data-stu-id="69d51-391">Fix #13529: Change documentation of parameter enable_non_ssl_port</span></span>

### <a name="storage"></a><span data-ttu-id="69d51-392">Stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-392">Storage</span></span>

* <span data-ttu-id="69d51-393">`az storage copy`: Ajout du paramètre `--follow-symlinks` pour prendre en charge les symlinks</span><span class="sxs-lookup"><span data-stu-id="69d51-393">`az storage copy`: Add parameter `--follow-symlinks` to support symlinks</span></span>
* <span data-ttu-id="69d51-394">Activer le contexte local pour le compte de stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-394">Enable local context for storage account</span></span>
* <span data-ttu-id="69d51-395">`az storage logging`: Correction du problème #11969 pour améliorer le message d’erreur</span><span class="sxs-lookup"><span data-stu-id="69d51-395">`az storage logging`: Fix issue #11969 to refine error message</span></span>

## <a name="may-19-2020"></a><span data-ttu-id="69d51-396">19 mai 2020</span><span class="sxs-lookup"><span data-stu-id="69d51-396">May 19, 2020</span></span>

<span data-ttu-id="69d51-397">Version 2.6.0</span><span class="sxs-lookup"><span data-stu-id="69d51-397">Version 2.6.0</span></span>

### <a name="acr"></a><span data-ttu-id="69d51-398">ACR</span><span class="sxs-lookup"><span data-stu-id="69d51-398">ACR</span></span>

* <span data-ttu-id="69d51-399">Ajout du délai d’expiration par défaut de 5 minutes pour toute demande à ACR</span><span class="sxs-lookup"><span data-stu-id="69d51-399">Add default timeout of 5 minutes for any requests to ACR</span></span>
* <span data-ttu-id="69d51-400">Prise en charge de la désactivation de l’accès au réseau public</span><span class="sxs-lookup"><span data-stu-id="69d51-400">Support disable public network access</span></span>
* <span data-ttu-id="69d51-401">`az acr token create` : exposition de l’argument --days</span><span class="sxs-lookup"><span data-stu-id="69d51-401">`az acr token create`: expose --days argument</span></span>
* <span data-ttu-id="69d51-402">`az acr import` : acceptation des valeurs de l’argument --source qui contiennent le nom du serveur de connexion résultant d’une correction côté du client</span><span class="sxs-lookup"><span data-stu-id="69d51-402">`az acr import`: accept --source argument values which contain login in server name through client end correction</span></span>

### <a name="acs"></a><span data-ttu-id="69d51-403">ACS</span><span class="sxs-lookup"><span data-stu-id="69d51-403">ACS</span></span>

* <span data-ttu-id="69d51-404">Correctif de bogue : suppression du nettoyage des champs pour les champs qui n’existent plus</span><span class="sxs-lookup"><span data-stu-id="69d51-404">Bug fix: remove fields cleanup for fields that no longer exist</span></span>

### <a name="aks"></a><span data-ttu-id="69d51-405">AKS</span><span class="sxs-lookup"><span data-stu-id="69d51-405">AKS</span></span>

* <span data-ttu-id="69d51-406">Mise à jour du contexte de l’aide pour la commande uptime-sla</span><span class="sxs-lookup"><span data-stu-id="69d51-406">Update uptime-sla command help context</span></span>
* <span data-ttu-id="69d51-407">Suppression de la vérification de plage pour la mise à jour du nombre minimal pour l’autoscaler</span><span class="sxs-lookup"><span data-stu-id="69d51-407">Remove range check for updating min count for autoscaler</span></span>
* <span data-ttu-id="69d51-408">Correction de l’interface CLI qui n’échoue pas quand l’utilisateur spécifie uniquement un mot de passe Windows</span><span class="sxs-lookup"><span data-stu-id="69d51-408">Fix that cli doe not fail when user only specifies Windows password</span></span>

### <a name="ams"></a><span data-ttu-id="69d51-409">AMS</span><span class="sxs-lookup"><span data-stu-id="69d51-409">AMS</span></span>

* <span data-ttu-id="69d51-410">`az ams transform create`: Ajout de la possibilité de créer une transformation avec une présélection FaceDetector</span><span class="sxs-lookup"><span data-stu-id="69d51-410">`az ams transform create`: Add ability to create a transform with a FaceDetector preset</span></span>
* <span data-ttu-id="69d51-411">`az ams content-key-policy create` : Ajout de la possibilité de créer une stratégie de clé de contenu FairPlay avec une configuration de location hors connexion</span><span class="sxs-lookup"><span data-stu-id="69d51-411">`az ams content-key-policy create` : Add ability to create a FairPlay content key policy with an offline rental configuration</span></span>

### <a name="appconfig"></a><span data-ttu-id="69d51-412">AppConfig</span><span class="sxs-lookup"><span data-stu-id="69d51-412">AppConfig</span></span>

* <span data-ttu-id="69d51-413">Correction de bogue pour les valeurs de clé de liste avec champs</span><span class="sxs-lookup"><span data-stu-id="69d51-413">Bug fix for list key values with fields</span></span>

### <a name="appservice"></a><span data-ttu-id="69d51-414">AppService</span><span class="sxs-lookup"><span data-stu-id="69d51-414">AppService</span></span>

* <span data-ttu-id="69d51-415">`az functionapp create`: AzureWebJobsDashboard ne sera défini que si AppInsights est désactivé</span><span class="sxs-lookup"><span data-stu-id="69d51-415">`az functionapp create`: AzureWebJobsDashboard will only be set if AppInsights is disabled</span></span>
* <span data-ttu-id="69d51-416">Correctif #10664 – Intégration de réseau virtuel – Problème de vérification d’emplacement et correctif #13257 – Échec d’az webapp up quand un groupe de ressources doit être créé</span><span class="sxs-lookup"><span data-stu-id="69d51-416">Fix #10664- VNet Integration - Location Check Issue & fix #13257- az webapp up failing when RG needs to be created</span></span>
* <span data-ttu-id="69d51-417">`az webapp|functionapp config ssl import`: Recherche dans le coffre de clés des groupes de ressources d’un abonnement et amélioration de l’aide et des exemples.</span><span class="sxs-lookup"><span data-stu-id="69d51-417">`az webapp|functionapp config ssl import`: Lookup key vault across resources groups in subscription and improve help and examples.</span></span>
* <span data-ttu-id="69d51-418">Intégration du contexte local pour App Service</span><span class="sxs-lookup"><span data-stu-id="69d51-418">Onboard local context for app service</span></span>

### <a name="arm"></a><span data-ttu-id="69d51-419">ARM</span><span class="sxs-lookup"><span data-stu-id="69d51-419">ARM</span></span>

* <span data-ttu-id="69d51-420">`az deployment`: Correction du problème lié à l’absence de retour de templateLink pendant le déploiement ou la validation de template-uri</span><span class="sxs-lookup"><span data-stu-id="69d51-420">`az deployment`: Fix the problem that the templateLink will not be returned when deploying or validating template-uri</span></span>
* <span data-ttu-id="69d51-421">`az deployment`: Correction du problème lié au fait que les caractères spécialement encodés ne sont pas pris en charge par le déploiement/la validation</span><span class="sxs-lookup"><span data-stu-id="69d51-421">`az deployment`: Fix the problem that deployment/validate does not support specially encoded character</span></span>
* <span data-ttu-id="69d51-422">`az deployment sub/group what-if`: Correction de l’alignement de tableau et gestion des erreurs</span><span class="sxs-lookup"><span data-stu-id="69d51-422">`az deployment sub/group what-if`: Fix array alignment and error handling</span></span>
* <span data-ttu-id="69d51-423">`az deployment operation`: Modification des informations de dépréciation</span><span class="sxs-lookup"><span data-stu-id="69d51-423">`az deployment operation`: Modify the deprecate information</span></span>

### <a name="aro"></a><span data-ttu-id="69d51-424">ARO</span><span class="sxs-lookup"><span data-stu-id="69d51-424">ARO</span></span>

* <span data-ttu-id="69d51-425">Ajout d’exemples pour az aro create, list, list-credentials, show, delete</span><span class="sxs-lookup"><span data-stu-id="69d51-425">Add examples to az aro create, list, list-credentials, show, delete</span></span>
* <span data-ttu-id="69d51-426">Ajout de la fonction generate_random_id</span><span class="sxs-lookup"><span data-stu-id="69d51-426">Add generate_random_id function</span></span>

### <a name="backup"></a><span data-ttu-id="69d51-427">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="69d51-427">Backup</span></span>

* <span data-ttu-id="69d51-428">Autorisation de FriendlyName dans la commande d’activation de la protection pour AzureFileShare</span><span class="sxs-lookup"><span data-stu-id="69d51-428">Allow FriendlyName in enable protection for AzureFileShare command</span></span>
* <span data-ttu-id="69d51-429">Correction dans la commande IaasVM restore-disks</span><span class="sxs-lookup"><span data-stu-id="69d51-429">Fix in IaasVM restore-disks Command</span></span>
* <span data-ttu-id="69d51-430">Ajout de BackupManagementType « MAB » à la commande item list</span><span class="sxs-lookup"><span data-stu-id="69d51-430">Add "MAB" BackupManagementType to item list command</span></span>
* <span data-ttu-id="69d51-431">Ajout de la prise en charge des nouvelles tentatives de mise à jour de stratégie pour les éléments en échec.</span><span class="sxs-lookup"><span data-stu-id="69d51-431">Add support for retrying policy update for failed items.</span></span>
* <span data-ttu-id="69d51-432">Ajout d’une fonctionnalité de reprise de protection pour Machine Virtuelle Azure</span><span class="sxs-lookup"><span data-stu-id="69d51-432">Add Resume Protection functionality for Azure Virtual Machine</span></span>
* <span data-ttu-id="69d51-433">Ajout d’une prise en charge permettant de spécifier ResourceGroup pour stocker instantRP pendant la création ou la modification d’une stratégie</span><span class="sxs-lookup"><span data-stu-id="69d51-433">Add support to specify ResourceGroup for storing instantRP during Create or Modify Policy</span></span>

### <a name="ci"></a><span data-ttu-id="69d51-434">CI</span><span class="sxs-lookup"><span data-stu-id="69d51-434">CI</span></span>

* <span data-ttu-id="69d51-435">Prise en charge de flake8 3.8.0</span><span class="sxs-lookup"><span data-stu-id="69d51-435">Support flake8 3.8.0</span></span>

### <a name="compute"></a><span data-ttu-id="69d51-436">Calcul</span><span class="sxs-lookup"><span data-stu-id="69d51-436">Compute</span></span>

* <span data-ttu-id="69d51-437">Nouvelle commande az vm auto-shutdown</span><span class="sxs-lookup"><span data-stu-id="69d51-437">New command az vm auto-shutdown</span></span>
* <span data-ttu-id="69d51-438">`az vm list-skus`: Mise à jour du comportement de --zone ; retourne désormais tous les types de références SKU</span><span class="sxs-lookup"><span data-stu-id="69d51-438">`az vm list-skus`: Update --zone behavior, return all type skus now</span></span>

### <a name="core"></a><span data-ttu-id="69d51-439">Core</span><span class="sxs-lookup"><span data-stu-id="69d51-439">Core</span></span>

* <span data-ttu-id="69d51-440">Mise à jour de l’état activé/désactivé du contexte local vers le niveau utilisateur global</span><span class="sxs-lookup"><span data-stu-id="69d51-440">Update local context on/off status to global user level</span></span>

### <a name="extension"></a><span data-ttu-id="69d51-441">Extension</span><span class="sxs-lookup"><span data-stu-id="69d51-441">Extension</span></span>

* <span data-ttu-id="69d51-442">`az extension add`: Ajout de --system pour permettre l’installation d’extensions dans un chemin système</span><span class="sxs-lookup"><span data-stu-id="69d51-442">`az extension add`: Add --system to enable installing extensions in a system path</span></span>
* <span data-ttu-id="69d51-443">Prise en charge de .egg-info pour stocker les métadonnées d’extension de type wheel</span><span class="sxs-lookup"><span data-stu-id="69d51-443">Support .egg-info to store wheel type extension metadata</span></span>

### <a name="iot"></a><span data-ttu-id="69d51-444">IoT</span><span class="sxs-lookup"><span data-stu-id="69d51-444">IoT</span></span>

* <span data-ttu-id="69d51-445">`az iot`: Mise à jour du message de reconnaissance de la première extension exécutée par le module de commande IoT vers l’ID moderne non déconseillé `azure-iot`.</span><span class="sxs-lookup"><span data-stu-id="69d51-445">`az iot`: Update the IoT command module first run extension awareness message to the accurate, non-deprecated modern Id `azure-iot`.</span></span>

### <a name="iot-hub"></a><span data-ttu-id="69d51-446">IoT Hub</span><span class="sxs-lookup"><span data-stu-id="69d51-446">IoT Hub</span></span>

* <span data-ttu-id="69d51-447">Prise en charge des commandes de l’API 2020-03-01 et de l’isolement réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-447">Support for 2020-03-01 API and Network Isolation commands</span></span>

### <a name="netappfiles"></a><span data-ttu-id="69d51-448">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="69d51-448">NetAppFiles</span></span>

* <span data-ttu-id="69d51-449">`az volume create`: Ajout de snapshot-id en tant que paramètre pour créer un volume, permettant ainsi aux utilisateurs de créer un volume à partir d’une capture instantanée existante.</span><span class="sxs-lookup"><span data-stu-id="69d51-449">`az volume create`: Adds snapshot-id as a parameter to create volume this will allow users to create a volume from existing snapshot.</span></span>

### <a name="network"></a><span data-ttu-id="69d51-450">Réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-450">Network</span></span>

* <span data-ttu-id="69d51-451">Correction du changement non souhaité de la valeur TTL pour dns add-record</span><span class="sxs-lookup"><span data-stu-id="69d51-451">Fix ttl value changed unintended for dns add-record</span></span>
* <span data-ttu-id="69d51-452">`az network public-ip create`: Information à l’intention des clients pour les prévenir d’un changement cassant imminent</span><span class="sxs-lookup"><span data-stu-id="69d51-452">`az network public-ip create`: Inform customers of a coming breaking change</span></span>
* <span data-ttu-id="69d51-453">Prise en charge des commandes génériques pour un scénario de liaison privée</span><span class="sxs-lookup"><span data-stu-id="69d51-453">Support generic commands for private link scenario</span></span>
* <span data-ttu-id="69d51-454">`az network private-endpoint-connection`: Prise en charge des types mysql, postgre et mariadb</span><span class="sxs-lookup"><span data-stu-id="69d51-454">`az network private-endpoint-connection`: Support mysql, postgre and mariadb types</span></span>
* <span data-ttu-id="69d51-455">`az network private-endpoint-connection`: Prise en charge des types cosmosdb</span><span class="sxs-lookup"><span data-stu-id="69d51-455">`az network private-endpoint-connection`: Support cosmosdb types</span></span>
* <span data-ttu-id="69d51-456">`az network private-endpoint` : dépréciation de --group-ids et redirection vers --group-id</span><span class="sxs-lookup"><span data-stu-id="69d51-456">`az network private-endpoint`: deprecate --group-ids and redirect to --group-id</span></span>

### <a name="output"></a><span data-ttu-id="69d51-457">Output</span><span class="sxs-lookup"><span data-stu-id="69d51-457">Output</span></span>

* <span data-ttu-id="69d51-458">Affichage de l’instruction update dans find, feedback et --help</span><span class="sxs-lookup"><span data-stu-id="69d51-458">Show update instruction in find, feedback and --help</span></span>

### <a name="packaging"></a><span data-ttu-id="69d51-459">Packaging</span><span class="sxs-lookup"><span data-stu-id="69d51-459">Packaging</span></span>

* <span data-ttu-id="69d51-460">Génération de packages MSI/Homebrew avec les dépendances résolues selon requirements.txt</span><span class="sxs-lookup"><span data-stu-id="69d51-460">Build MSI/Homebrew packages with dependecies resolved from requirements.txt</span></span>

### <a name="rbac"></a><span data-ttu-id="69d51-461">RBAC</span><span class="sxs-lookup"><span data-stu-id="69d51-461">RBAC</span></span>

* <span data-ttu-id="69d51-462">`az ad sp credential reset` : correction de la génération d’informations d’identification faibles</span><span class="sxs-lookup"><span data-stu-id="69d51-462">`az ad sp credential reset`: fix weak credential generation</span></span>

### <a name="storage"></a><span data-ttu-id="69d51-463">Stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-463">Storage</span></span>

* <span data-ttu-id="69d51-464">`az storage account file-service-properties update/show`: Ajout de la prise en charge des propriétés de fichier pour le compte de stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-464">`az storage account file-service-properties update/show`: Add File Properties Support for Storage Account</span></span>
* <span data-ttu-id="69d51-465">`az storage container create`: Correction #13373 par l’ajout d’un validateur pour l’accès public</span><span class="sxs-lookup"><span data-stu-id="69d51-465">`az storage container create`: Fix #13373 by adding validator for public access</span></span>
* <span data-ttu-id="69d51-466">Ajout de la prise en charge d’ADLS Gen2 track2</span><span class="sxs-lookup"><span data-stu-id="69d51-466">Add ADLS Gen2 track2 support</span></span>
* <span data-ttu-id="69d51-467">`az storage blob sync`: Prise en charge d’`--connection-string`</span><span class="sxs-lookup"><span data-stu-id="69d51-467">`az storage blob sync`: Support `--connection-string`</span></span>
* <span data-ttu-id="69d51-468">`az storage blob sync`: Correction du message d’erreur incorrect quand azcopy ne trouve pas l’emplacement d’installation</span><span class="sxs-lookup"><span data-stu-id="69d51-468">`az storage blob sync`: Fix the incorrect error message when azcopy cannot find the installation location</span></span>

## <a name="april-30-2020"></a><span data-ttu-id="69d51-469">30 avril 2020</span><span class="sxs-lookup"><span data-stu-id="69d51-469">April 30, 2020</span></span>

<span data-ttu-id="69d51-470">Version 2.5.1</span><span class="sxs-lookup"><span data-stu-id="69d51-470">Version 2.5.1</span></span>

### <a name="acr"></a><span data-ttu-id="69d51-471">ACR</span><span class="sxs-lookup"><span data-stu-id="69d51-471">ACR</span></span>

* <span data-ttu-id="69d51-472">`az acr check-health`: Correction de « DOCKER_PULL_ERROR » sur Windows</span><span class="sxs-lookup"><span data-stu-id="69d51-472">`az acr check-health`: Fix "DOCKER_PULL_ERROR" on Windows</span></span>

### <a name="compute"></a><span data-ttu-id="69d51-473">Calcul</span><span class="sxs-lookup"><span data-stu-id="69d51-473">Compute</span></span>

* <span data-ttu-id="69d51-474">`az vm list-ip-addresses`: Gestion des erreurs</span><span class="sxs-lookup"><span data-stu-id="69d51-474">`az vm list-ip-addresses`: Error handling</span></span>
* <span data-ttu-id="69d51-475">Correction d’un bogue de vm create si endpoint_vm_image_alias_doc n’est pas défini dans le profil cloud</span><span class="sxs-lookup"><span data-stu-id="69d51-475">Fix a bug of vm create if endpoint_vm_image_alias_doc is not set in cloud profile</span></span>
* <span data-ttu-id="69d51-476">`az vmss create`: Ajout de --os-disk-size-gb</span><span class="sxs-lookup"><span data-stu-id="69d51-476">`az vmss create`: Add --os-disk-size-gb</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="69d51-477">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="69d51-477">Cosmos DB</span></span>

* <span data-ttu-id="69d51-478">`az cosmosdb create/update` : ajout de la prise en charge de add --enable-public-network</span><span class="sxs-lookup"><span data-stu-id="69d51-478">`az cosmosdb create/update`: add --enable-public-network support</span></span>

### <a name="extension"></a><span data-ttu-id="69d51-479">Extension</span><span class="sxs-lookup"><span data-stu-id="69d51-479">Extension</span></span>

* <span data-ttu-id="69d51-480">Correction du chargement des métadonnées incorrectes pour l’extension du type de roulette</span><span class="sxs-lookup"><span data-stu-id="69d51-480">Fix loading wrong metadata for wheel type extension</span></span>

### <a name="packaging"></a><span data-ttu-id="69d51-481">Packaging</span><span class="sxs-lookup"><span data-stu-id="69d51-481">Packaging</span></span>

* <span data-ttu-id="69d51-482">Ajout du script az pour Git Bash/Cygwin sur Windows</span><span class="sxs-lookup"><span data-stu-id="69d51-482">Add az script for Git Bash/Cygwin on Windows</span></span>

### <a name="sql"></a><span data-ttu-id="69d51-483">SQL</span><span class="sxs-lookup"><span data-stu-id="69d51-483">SQL</span></span>

* <span data-ttu-id="69d51-484">`az sql instance-pool`: Ajout d’un groupe de commandes pour les pools d’instances</span><span class="sxs-lookup"><span data-stu-id="69d51-484">`az sql instance-pool`: Add instance pools command group</span></span>

### <a name="storage"></a><span data-ttu-id="69d51-485">Stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-485">Storage</span></span>

* <span data-ttu-id="69d51-486">Mise à niveau du package azure-multiapi-storage vers 0.3.0</span><span class="sxs-lookup"><span data-stu-id="69d51-486">Upgrade package azure-multiapi-storage to 0.3.0</span></span>
* <span data-ttu-id="69d51-487">Prise en charge de GZRS pour la création et la mise à jour de comptes de stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-487">Support GZRS for storage account creation and update</span></span>
* <span data-ttu-id="69d51-488">`az storage account failover`: Ajout de la prise en charge du basculement de comptes de stockage grs/gzrs</span><span class="sxs-lookup"><span data-stu-id="69d51-488">`az storage account failover`: Add support for grs/gzrs storage account failover</span></span>
* <span data-ttu-id="69d51-489">`az storage blob upload`: Ajout du paramètre --encryption-scope pour prendre en charge la spécification des informations d’étendue du chiffrement</span><span class="sxs-lookup"><span data-stu-id="69d51-489">`az storage blob upload`: Add --encryption-scope parameter to support specifying encryption scope information</span></span>

## <a name="april-28-2020"></a><span data-ttu-id="69d51-490">28 avril 2020</span><span class="sxs-lookup"><span data-stu-id="69d51-490">April 28, 2020</span></span>

<span data-ttu-id="69d51-491">Version 2.5.0</span><span class="sxs-lookup"><span data-stu-id="69d51-491">Version 2.5.0</span></span>

### <a name="acs"></a><span data-ttu-id="69d51-492">ACS</span><span class="sxs-lookup"><span data-stu-id="69d51-492">ACS</span></span>

* <span data-ttu-id="69d51-493">[CHANGEMENT CASSANT] du paramètre az openshift create: remove --vnet-peer.</span><span class="sxs-lookup"><span data-stu-id="69d51-493">[BREAKING CHANGE] az openshift create: remove --vnet-peer parameter.</span></span>
* <span data-ttu-id="69d51-494">`az openshift create` : Ajout d’indicateurs pour prendre en charge un cluster privé.</span><span class="sxs-lookup"><span data-stu-id="69d51-494">`az openshift create`: add flags to support private cluster.</span></span>
* <span data-ttu-id="69d51-495">`az openshift` : Mise à niveau vers la version d’API `2019-10-27-preview`.</span><span class="sxs-lookup"><span data-stu-id="69d51-495">`az openshift`: upgrade to `2019-10-27-preview` API version.</span></span>
* <span data-ttu-id="69d51-496">`az openshift` : Ajout de la commande `update`.</span><span class="sxs-lookup"><span data-stu-id="69d51-496">`az openshift`: add `update` command.</span></span>

### <a name="aks"></a><span data-ttu-id="69d51-497">AKS</span><span class="sxs-lookup"><span data-stu-id="69d51-497">AKS</span></span>

* <span data-ttu-id="69d51-498">`az aks create`: Ajout de la prise en charge de Windows</span><span class="sxs-lookup"><span data-stu-id="69d51-498">`az aks create`: Add support for Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="69d51-499">AppService</span><span class="sxs-lookup"><span data-stu-id="69d51-499">AppService</span></span>

* <span data-ttu-id="69d51-500">`az webapp deployment source config-zip` : Suppression de sleep après request.get()</span><span class="sxs-lookup"><span data-stu-id="69d51-500">`az webapp deployment source config-zip`: remove sleep after request.get()</span></span>

### <a name="arm"></a><span data-ttu-id="69d51-501">ARM</span><span class="sxs-lookup"><span data-stu-id="69d51-501">ARM</span></span>

* <span data-ttu-id="69d51-502">Ajout de commandes What-If de déploiement de modèles</span><span class="sxs-lookup"><span data-stu-id="69d51-502">Add template deployment What-If commands</span></span>

### <a name="aro"></a><span data-ttu-id="69d51-503">ARO</span><span class="sxs-lookup"><span data-stu-id="69d51-503">ARO</span></span>

* <span data-ttu-id="69d51-504">`az aro`: Correction de la sortie de table</span><span class="sxs-lookup"><span data-stu-id="69d51-504">`az aro`: Fix table output</span></span>

### <a name="ci"></a><span data-ttu-id="69d51-505">CI</span><span class="sxs-lookup"><span data-stu-id="69d51-505">CI</span></span>

* <span data-ttu-id="69d51-506">Intégration de pytest et dépréciation de nose pour le test d’automatisation</span><span class="sxs-lookup"><span data-stu-id="69d51-506">Onboard pytest and deprecate nose for Automation Test</span></span>

### <a name="compute"></a><span data-ttu-id="69d51-507">Calcul</span><span class="sxs-lookup"><span data-stu-id="69d51-507">Compute</span></span>

* <span data-ttu-id="69d51-508">`az vmss disk detach` : Correction du problème NoneType du disque de données</span><span class="sxs-lookup"><span data-stu-id="69d51-508">`az vmss disk detach`: fix data disk NoneType issue</span></span>
* <span data-ttu-id="69d51-509">`az vm availability-set list`: Prise en charge de l’affichage de la liste de machines virtuelles</span><span class="sxs-lookup"><span data-stu-id="69d51-509">`az vm availability-set list`: Support showing VM list</span></span>
* <span data-ttu-id="69d51-510">`az vm list-skus`: Correction du problème d’affichage du format de table</span><span class="sxs-lookup"><span data-stu-id="69d51-510">`az vm list-skus`: Fix display problem of table format</span></span>

### <a name="keyvault"></a><span data-ttu-id="69d51-511">KeyVault</span><span class="sxs-lookup"><span data-stu-id="69d51-511">KeyVault</span></span>

* <span data-ttu-id="69d51-512">Ajout d’un nouveau paramètre `--enable-rbac-authorization` lors de la création ou de la mise à jour</span><span class="sxs-lookup"><span data-stu-id="69d51-512">Add new parameter `--enable-rbac-authorization` during creating or updating</span></span>

### <a name="monitor"></a><span data-ttu-id="69d51-513">Superviser</span><span class="sxs-lookup"><span data-stu-id="69d51-513">Monitor</span></span>

* <span data-ttu-id="69d51-514">Prise en charge des fonctionnalités CMK de cluster LA</span><span class="sxs-lookup"><span data-stu-id="69d51-514">Support LA cluster CMK features</span></span>
* <span data-ttu-id="69d51-515">`az monitor log-analytics workspace linked-storage` : Prise en charge des fonctionnalités BYOS</span><span class="sxs-lookup"><span data-stu-id="69d51-515">`az monitor log-analytics workspace linked-storage`: supports BYOS features</span></span>

### <a name="network"></a><span data-ttu-id="69d51-516">Réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-516">Network</span></span>

* <span data-ttu-id="69d51-517">`az network security-partner` : Prise en charge du fournisseur de partenaire de sécurité</span><span class="sxs-lookup"><span data-stu-id="69d51-517">`az network security-partner`: support security partner provider</span></span>

### <a name="privatedns"></a><span data-ttu-id="69d51-518">Privatedns</span><span class="sxs-lookup"><span data-stu-id="69d51-518">Privatedns</span></span>

* <span data-ttu-id="69d51-519">Ajout d’une fonctionnalité dans une zone DNS privée pour importer/exporter un fichier de zone</span><span class="sxs-lookup"><span data-stu-id="69d51-519">Add feature in private DNS zone to import export zone file</span></span>

## <a name="april-21-2020"></a><span data-ttu-id="69d51-520">21 avril 2020</span><span class="sxs-lookup"><span data-stu-id="69d51-520">April 21, 2020</span></span>

<span data-ttu-id="69d51-521">Version 2.4.0</span><span class="sxs-lookup"><span data-stu-id="69d51-521">Version 2.4.0</span></span>

### <a name="acr"></a><span data-ttu-id="69d51-522">ACR</span><span class="sxs-lookup"><span data-stu-id="69d51-522">ACR</span></span>

* <span data-ttu-id="69d51-523">`az acr run --cmd` : désactivation du remplacement du répertoire de travail</span><span class="sxs-lookup"><span data-stu-id="69d51-523">`az acr run --cmd`: disable working directory override</span></span>
* <span data-ttu-id="69d51-524">Prise en charge du point de terminaison de données dédié</span><span class="sxs-lookup"><span data-stu-id="69d51-524">Support dedicated data endpoint</span></span>

### <a name="aks"></a><span data-ttu-id="69d51-525">AKS</span><span class="sxs-lookup"><span data-stu-id="69d51-525">AKS</span></span>

* <span data-ttu-id="69d51-526">`az aks list -o table` doit afficher privateFqdn comme nom de domaine complet pour les clusters privés</span><span class="sxs-lookup"><span data-stu-id="69d51-526">`az aks list -o table` should show privateFqdn as fqdn for private clusters</span></span>
* <span data-ttu-id="69d51-527">Ajout de --uptime-sla</span><span class="sxs-lookup"><span data-stu-id="69d51-527">Add --uptime-sla</span></span>
* <span data-ttu-id="69d51-528">Mise à jour du package containerservice</span><span class="sxs-lookup"><span data-stu-id="69d51-528">Update containerservice package</span></span>
* <span data-ttu-id="69d51-529">Ajout de la prise en charge de l’adresse IP publique de nœud</span><span class="sxs-lookup"><span data-stu-id="69d51-529">Add node public IP support</span></span>
* <span data-ttu-id="69d51-530">Correction d’une faute de frappe dans la commande d’aide</span><span class="sxs-lookup"><span data-stu-id="69d51-530">Fix typo in the help command</span></span>

### <a name="appconfig"></a><span data-ttu-id="69d51-531">AppConfig</span><span class="sxs-lookup"><span data-stu-id="69d51-531">AppConfig</span></span>

* <span data-ttu-id="69d51-532">Résolution de la référence du coffre de clés pour la liste Key Vault et les commandes d’exportation</span><span class="sxs-lookup"><span data-stu-id="69d51-532">Resolve key vault reference for kv list and export commands</span></span>
* <span data-ttu-id="69d51-533">Résolution de bogue pour les valeurs de clé de liste</span><span class="sxs-lookup"><span data-stu-id="69d51-533">Bug fix for list key values</span></span>

### <a name="appservice"></a><span data-ttu-id="69d51-534">AppService</span><span class="sxs-lookup"><span data-stu-id="69d51-534">AppService</span></span>

* <span data-ttu-id="69d51-535">`az functionapp create`: Modification de la façon dont linuxFxVersion était défini pour les applications de fonction dotnet linux.</span><span class="sxs-lookup"><span data-stu-id="69d51-535">`az functionapp create`: Changed the way linuxFxVersion was being set for dotnet linux function apps.</span></span> <span data-ttu-id="69d51-536">Cela doit résoudre un bogue qui empêchait la création d’applications de consommation dotnet linux</span><span class="sxs-lookup"><span data-stu-id="69d51-536">This should fix a bug that was preventing dotnet linux consumption apps from being created</span></span>
* <span data-ttu-id="69d51-537">[CHANGEMENT CASSANT] `az webapp create` : correctif pour conserver les paramètres d’application existants avec az webapp create</span><span class="sxs-lookup"><span data-stu-id="69d51-537">[BREAKING CHANGE] `az webapp create`: fix to keep existing AppSettings with az webapp create</span></span>
* <span data-ttu-id="69d51-538">[CHANGEMENT CASSANT] `az webapp up` : correctif pour créer un groupe de ressources pour la commande az webapp up lors de l’utilisation de l’indicateur -g</span><span class="sxs-lookup"><span data-stu-id="69d51-538">[BREAKING CHANGE] `az webapp up`: fix to create RG for az webapp up command when using -g flag</span></span>
* <span data-ttu-id="69d51-539">[CHANGEMENT CASSANT] `az webapp config` : correctif pour afficher des valeurs pour la sortie non-JSON avec la liste de chaînes de connexion az webapp config</span><span class="sxs-lookup"><span data-stu-id="69d51-539">[BREAKING CHANGE] `az webapp config`: fix to show values for non-JSON output with az webapp config connection-string list</span></span>

### <a name="arm"></a><span data-ttu-id="69d51-540">ARM</span><span class="sxs-lookup"><span data-stu-id="69d51-540">ARM</span></span>

* <span data-ttu-id="69d51-541">`az deployment create/validate`: Ajout d’un paramètre `--no-prompt` pour prendre en charge le saut de l’invite de paramètres manquants pour le modèle ARM</span><span class="sxs-lookup"><span data-stu-id="69d51-541">`az deployment create/validate`: Add parameter `--no-prompt` to support skipping the prompt of missing parameters for ARM template</span></span>
* <span data-ttu-id="69d51-542">`az deployment group/mg/sub/tenant validate`: Prise en charge de commentaires dans le fichier de paramètres de déploiement</span><span class="sxs-lookup"><span data-stu-id="69d51-542">`az deployment group/mg/sub/tenant validate`: Support comments in deployment parameter file</span></span>
* <span data-ttu-id="69d51-543">`az deployment`: Suppression de `is_preview` pour le paramètre `--handle-extended-json-format`</span><span class="sxs-lookup"><span data-stu-id="69d51-543">`az deployment`: Remove `is_preview` for parameter `--handle-extended-json-format`</span></span>
* <span data-ttu-id="69d51-544">`az deployment group/mg/sub/tenant cancel`: Prise en charge de l’annulation du déploiement pour le modèle ARM</span><span class="sxs-lookup"><span data-stu-id="69d51-544">`az deployment group/mg/sub/tenant cancel`: Support cancel deployment for ARM template</span></span>
* <span data-ttu-id="69d51-545">`az deployment group/mg/sub/tenant validate`: Amélioration du message d’erreur lors de l’échec de la vérification du déploiement</span><span class="sxs-lookup"><span data-stu-id="69d51-545">`az deployment group/mg/sub/tenant validate`: Improve the error message when deployment verification fails</span></span>
* <span data-ttu-id="69d51-546">`az deployment-scripts`: Ajout de nouvelles commandes pour DeploymentScripts</span><span class="sxs-lookup"><span data-stu-id="69d51-546">`az deployment-scripts`: Add new commands for DeploymentScripts</span></span>
* <span data-ttu-id="69d51-547">`az resource tag`: Ajout du paramètre `--is-incremental` pour prendre en charge l’ajout incrémentiel de balises aux ressources</span><span class="sxs-lookup"><span data-stu-id="69d51-547">`az resource tag`: Add parameter `--is-incremental` to support adding tags to resource incrementally</span></span>

### <a name="aro"></a><span data-ttu-id="69d51-548">ARO</span><span class="sxs-lookup"><span data-stu-id="69d51-548">ARO</span></span>

* <span data-ttu-id="69d51-549">`az aro`:  Ajout du module de commande aro Azure RedHat OpenShift V4</span><span class="sxs-lookup"><span data-stu-id="69d51-549">`az aro`:  Add Azure RedHat OpenShift V4 aro command module</span></span>

### <a name="batch"></a><span data-ttu-id="69d51-550">Batch</span><span class="sxs-lookup"><span data-stu-id="69d51-550">Batch</span></span>

* <span data-ttu-id="69d51-551">Mise à jour de l’API Batch</span><span class="sxs-lookup"><span data-stu-id="69d51-551">Update Batch API</span></span>

### <a name="compute"></a><span data-ttu-id="69d51-552">Calcul</span><span class="sxs-lookup"><span data-stu-id="69d51-552">Compute</span></span>

* <span data-ttu-id="69d51-553">`az sig image-version create`: Ajout d’un type de compte de stockage Premium_LRS</span><span class="sxs-lookup"><span data-stu-id="69d51-553">`az sig image-version create`: Add storage account type Premium_LRS</span></span>
* <span data-ttu-id="69d51-554">`az vmss update`: Correction d’un problème de mise à jour de notification d’arrêt</span><span class="sxs-lookup"><span data-stu-id="69d51-554">`az vmss update`: Fix terminate notification update issue</span></span>
* <span data-ttu-id="69d51-555">`az vm/vmss create`: Ajout de la prise en charge de la version d’image spécialisée</span><span class="sxs-lookup"><span data-stu-id="69d51-555">`az vm/vmss create`: Add support for specialized image version</span></span>
* <span data-ttu-id="69d51-556">Version de l’API SIG 2019-12-01</span><span class="sxs-lookup"><span data-stu-id="69d51-556">SIG API Version 2019-12-01</span></span>
* <span data-ttu-id="69d51-557">`az sig image-version create`: Ajout de --target-region-encryption</span><span class="sxs-lookup"><span data-stu-id="69d51-557">`az sig image-version create`: Add --target-region-encryption</span></span>
* <span data-ttu-id="69d51-558">Correction de l’échec des tests lors d’une exécution en série en raison d’un nom de coffre de clés en double dans le cache en mémoire global</span><span class="sxs-lookup"><span data-stu-id="69d51-558">Fix tests fail when running in serial due to keyvault name is duplicated in global in-momery cache</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="69d51-559">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="69d51-559">CosmosDB</span></span>

* <span data-ttu-id="69d51-560">Prise en charge d’`az cosmosdb private-link-resource/private-endpoint-connection`</span><span class="sxs-lookup"><span data-stu-id="69d51-560">Support `az cosmosdb private-link-resource/private-endpoint-connection`</span></span>

### <a name="iot-central"></a><span data-ttu-id="69d51-561">IoT Central</span><span class="sxs-lookup"><span data-stu-id="69d51-561">IoT Central</span></span>

* <span data-ttu-id="69d51-562">Dépréciation d’`az iotcentral`</span><span class="sxs-lookup"><span data-stu-id="69d51-562">Deprecate `az iotcentral`</span></span>
* <span data-ttu-id="69d51-563">Ajout du module de commande `az iot central`</span><span class="sxs-lookup"><span data-stu-id="69d51-563">Add `az iot central` command module</span></span>

### <a name="monitor"></a><span data-ttu-id="69d51-564">Superviser</span><span class="sxs-lookup"><span data-stu-id="69d51-564">Monitor</span></span>

* <span data-ttu-id="69d51-565">Prise en charge du scénario de lien privé pour la supervision</span><span class="sxs-lookup"><span data-stu-id="69d51-565">Support private link scenario for monitor</span></span>
* <span data-ttu-id="69d51-566">Correction du mode de simulation incorrect dans test_monitor_general_operations.py</span><span class="sxs-lookup"><span data-stu-id="69d51-566">Fix wrong mocking way in test_monitor_general_operations.py</span></span>

### <a name="network"></a><span data-ttu-id="69d51-567">Réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-567">Network</span></span>

* <span data-ttu-id="69d51-568">Dépréciation de la référence sku pour la commande de mise à jour de l’adresse IP publique</span><span class="sxs-lookup"><span data-stu-id="69d51-568">Deprecate sku for public ip update command</span></span>
* <span data-ttu-id="69d51-569">`az network private-endpoint`: Prise en charge du groupe de zones DNS privées</span><span class="sxs-lookup"><span data-stu-id="69d51-569">`az network private-endpoint`: Support private dns zone group</span></span>
* <span data-ttu-id="69d51-570">Activation de la fonctionnalité de contexte local pour le paramètre de réseau virtuel/sous-réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-570">Enable local context feature for vnet/subnet parameter</span></span>
* <span data-ttu-id="69d51-571">Correction d’un exemple d’utilisation incorrect dans test_nw_flow_log_delete</span><span class="sxs-lookup"><span data-stu-id="69d51-571">Fix wrong usage example in test_nw_flow_log_delete</span></span>

### <a name="packaging"></a><span data-ttu-id="69d51-572">Packaging</span><span class="sxs-lookup"><span data-stu-id="69d51-572">Packaging</span></span>

* <span data-ttu-id="69d51-573">Suppression de la prise en charge d’un package Ubuntu/Disco</span><span class="sxs-lookup"><span data-stu-id="69d51-573">Drop support for Ubuntu/Disco package</span></span>

### <a name="rbac"></a><span data-ttu-id="69d51-574">RBAC</span><span class="sxs-lookup"><span data-stu-id="69d51-574">RBAC</span></span>

* <span data-ttu-id="69d51-575">`az ad app create/update` : prise en charge de --optional-claims en tant que paramètre</span><span class="sxs-lookup"><span data-stu-id="69d51-575">`az ad app create/update`: support --optional-claims as a parameter</span></span>

### <a name="rdbms"></a><span data-ttu-id="69d51-576">SGBDR</span><span class="sxs-lookup"><span data-stu-id="69d51-576">RDBMS</span></span>

* <span data-ttu-id="69d51-577">Ajout des commandes d’administrateur Azure Active Directory pour PostgreSQL et MySQL</span><span class="sxs-lookup"><span data-stu-id="69d51-577">Add Azure active directory administrator commands for PostgreSQL and MySQL</span></span>

### <a name="service-fabric"></a><span data-ttu-id="69d51-578">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="69d51-578">Service Fabric</span></span>

* <span data-ttu-id="69d51-579">Correctif n  12891 : `az sf application update --application-parameters` supprime les anciens paramètres qui ne sont pas dans la demande</span><span class="sxs-lookup"><span data-stu-id="69d51-579">Fix #12891: `az sf application update --application-parameters` removes old parameters that are not in the request</span></span>
* <span data-ttu-id="69d51-580">Correctif n  12470, az sf create cluster, résolution de bogues dans la durabilité et la fiabilité des mises à jour, et recherche de groupes identiques de machines virtuelles correctement dans le code en fonction d’un nom de type de nœud</span><span class="sxs-lookup"><span data-stu-id="69d51-580">Fix #12470 az sf create cluster, fix bugs in update durability and reliability and find vmss correctly through the code given a node type name</span></span>

### <a name="sql"></a><span data-ttu-id="69d51-581">SQL</span><span class="sxs-lookup"><span data-stu-id="69d51-581">SQL</span></span>

* <span data-ttu-id="69d51-582">Ajout d’`az sql mi op list`, `az sql mi op get`, `az sql mi op cancel`</span><span class="sxs-lookup"><span data-stu-id="69d51-582">Add `az sql mi op list`, `az sql mi op get`, `az sql mi op cancel`</span></span>
* <span data-ttu-id="69d51-583">`az sql midb` : mise à jour/affichage de la stratégie de conservation à long terme, affichage/suppression des sauvegardes de conservation à long terme, restauration de la sauvegarde de conservation à long terme</span><span class="sxs-lookup"><span data-stu-id="69d51-583">`az sql midb`: update/show long term retention policy,  show/delete long term retention backups, restore long term retention backup</span></span>

### <a name="storage"></a><span data-ttu-id="69d51-584">Stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-584">Storage</span></span>

* <span data-ttu-id="69d51-585">Mise à niveau d’azure-mgmt-storage vers 9.0.0</span><span class="sxs-lookup"><span data-stu-id="69d51-585">Upgrade azure-mgmt-storage to 9.0.0</span></span>
* <span data-ttu-id="69d51-586">`az storage logging off`: Prise en charge de la désactivation de la journalisation pour un compte de stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-586">`az storage logging off`: Support turning off logging for a storage account</span></span>
* <span data-ttu-id="69d51-587">`az storage account update`: Activation de la rotation automatique de la clé pour CMK</span><span class="sxs-lookup"><span data-stu-id="69d51-587">`az storage account update`: Enable key auto-rotated for CMK</span></span>
* <span data-ttu-id="69d51-588">`az storage account encryption-scope create/update/list/show`: Ajout de la prise en charge de la personnalisation de l’étendue du chiffrement</span><span class="sxs-lookup"><span data-stu-id="69d51-588">`az storage account encryption-scope create/update/list/show`: Add support to customize encryption scope</span></span>
* <span data-ttu-id="69d51-589">`az storage container create`: Ajout de --default-encryption-scope et --deny-encryption-scope-override pour définir l’étendue du chiffrement de niveau de conteneur</span><span class="sxs-lookup"><span data-stu-id="69d51-589">`az storage container create`: Add --default-encryption-scope and --deny-encryption-scope-override to set encryption scope for container level</span></span>

### <a name="survey"></a><span data-ttu-id="69d51-590">Enquête</span><span class="sxs-lookup"><span data-stu-id="69d51-590">Survey</span></span>

* <span data-ttu-id="69d51-591">Ajout d’une instruction switch pour désactiver le lien d’enquête</span><span class="sxs-lookup"><span data-stu-id="69d51-591">Add switch to turn off survey link</span></span>

## <a name="april-01-2020"></a><span data-ttu-id="69d51-592">01 avril 2020</span><span class="sxs-lookup"><span data-stu-id="69d51-592">April 01, 2020</span></span>

<span data-ttu-id="69d51-593">Version 2.3.1</span><span class="sxs-lookup"><span data-stu-id="69d51-593">Version 2.3.1</span></span>

### <a name="acr"></a><span data-ttu-id="69d51-594">ACR</span><span class="sxs-lookup"><span data-stu-id="69d51-594">ACR</span></span>

* <span data-ttu-id="69d51-595">Correction d’une version incorrecte d’azure-mgmt-containerregistry pour Linux</span><span class="sxs-lookup"><span data-stu-id="69d51-595">Fix wrong version of azure-mgmt-containerregistry for Linux</span></span>

### <a name="profile"></a><span data-ttu-id="69d51-596">Profil</span><span class="sxs-lookup"><span data-stu-id="69d51-596">Profile</span></span>

* <span data-ttu-id="69d51-597">az login : Correction des échecs de connexion avec les profils cloud autres que `latest`</span><span class="sxs-lookup"><span data-stu-id="69d51-597">az login: Fix login failure with cloud profiles other than `latest`</span></span>

## <a name="march-31-2020"></a><span data-ttu-id="69d51-598">31 mars 2020</span><span class="sxs-lookup"><span data-stu-id="69d51-598">March 31, 2020</span></span>

<span data-ttu-id="69d51-599">Version 2.3.0</span><span class="sxs-lookup"><span data-stu-id="69d51-599">Version 2.3.0</span></span>

### <a name="acr"></a><span data-ttu-id="69d51-600">ACR</span><span class="sxs-lookup"><span data-stu-id="69d51-600">ACR</span></span>

* <span data-ttu-id="69d51-601">'az acr task update' : exception du pointeur null</span><span class="sxs-lookup"><span data-stu-id="69d51-601">'az acr task update': null pointer exception</span></span>
* <span data-ttu-id="69d51-602">`az acr import`: Modification de l’aide et du message d’erreur pour clarifier l’utilisation de --source et --registry</span><span class="sxs-lookup"><span data-stu-id="69d51-602">`az acr import`: Modify help and error message to clarify the usage of --source and --registry</span></span>
* <span data-ttu-id="69d51-603">Ajout d’un validateur pour l’argument 'registry_name'</span><span class="sxs-lookup"><span data-stu-id="69d51-603">Add a validator for argument 'registry_name'</span></span>
* <span data-ttu-id="69d51-604">`az acr login` : Suppression de l’indicateur de préversion sur '--expose-token'</span><span class="sxs-lookup"><span data-stu-id="69d51-604">`az acr login`:Remove the preview flag on '--expose-token'</span></span>
* <span data-ttu-id="69d51-605">[CHANGEMENT CASSANT] Suppression du paramètre de branche 'az acr task create/update'</span><span class="sxs-lookup"><span data-stu-id="69d51-605">[BREAKING CHANGE] 'az acr task create/update' Branch parameter is removed</span></span>
* <span data-ttu-id="69d51-606">'az acr task update' : Le client peut maintenant mettre à jour le contexte, git-token et/ou les déclencheurs individuellement</span><span class="sxs-lookup"><span data-stu-id="69d51-606">'az acr task update' Customer now can update context, git-token, and or triggers individually</span></span>
* <span data-ttu-id="69d51-607">'az acr agentpool' : nouvelle fonctionnalité</span><span class="sxs-lookup"><span data-stu-id="69d51-607">'az acr agentpool': new feature</span></span>

### <a name="aks"></a><span data-ttu-id="69d51-608">AKS</span><span class="sxs-lookup"><span data-stu-id="69d51-608">AKS</span></span>

* <span data-ttu-id="69d51-609">Correction d’apiServerAccessProfile lors de la mise à jour de --api-server-authorized-ip-ranges</span><span class="sxs-lookup"><span data-stu-id="69d51-609">Fix apiServerAccessProfile when updating --api-server-authorized-ip-ranges</span></span>
* <span data-ttu-id="69d51-610">aks update : Remplacement des adresses IP sortantes par des valeurs d’entrée lors de la mise à jour</span><span class="sxs-lookup"><span data-stu-id="69d51-610">aks update: Override outbound IPs with input values when update</span></span>
* <span data-ttu-id="69d51-611">Pas de création de SPN pour les clusters MSI et prise en charge de l’attachement d’acr à des clusters MSI</span><span class="sxs-lookup"><span data-stu-id="69d51-611">Do not create SPN for MSI clusters and support attach acr to MSI clusters</span></span>

### <a name="ams"></a><span data-ttu-id="69d51-612">AMS</span><span class="sxs-lookup"><span data-stu-id="69d51-612">AMS</span></span>

* <span data-ttu-id="69d51-613">Correctif #12469 : échec de l’ajout de Fairplay content-key-policy en raison de problèmes avec le paramètre « ask »</span><span class="sxs-lookup"><span data-stu-id="69d51-613">Fix #12469: adding Fairplay content-key-policy fails due to problems with 'ask' parameter</span></span>

### <a name="appconfig"></a><span data-ttu-id="69d51-614">AppConfig</span><span class="sxs-lookup"><span data-stu-id="69d51-614">AppConfig</span></span>

* <span data-ttu-id="69d51-615">Ajout de --skip-keyvault pour l’exportation de kv</span><span class="sxs-lookup"><span data-stu-id="69d51-615">Add --skip-keyvault for kv export</span></span>

### <a name="appservice"></a><span data-ttu-id="69d51-616">AppService</span><span class="sxs-lookup"><span data-stu-id="69d51-616">AppService</span></span>

* <span data-ttu-id="69d51-617">Correctif #12509 : Suppression de la balise d’az webapp up par défaut</span><span class="sxs-lookup"><span data-stu-id="69d51-617">Fix #12509: Remove the tag to az webapp up by default</span></span>
* <span data-ttu-id="69d51-618">az functionapp create : Mise à jour du menu d’aide --runtime-version et ajout d’un avertissement quand l’utilisateur spécifie --runtime-version pour dotnet</span><span class="sxs-lookup"><span data-stu-id="69d51-618">az functionapp create: Updated --runtime-version help menu and added warning when user specifies --runtime-version for dotnet</span></span>
* <span data-ttu-id="69d51-619">az functionapp create : Mise à jour du mode de définition de javaVersion pour les applications de fonction Windows</span><span class="sxs-lookup"><span data-stu-id="69d51-619">az functionapp create: Updated the way javaVersion was being set for Windows function apps</span></span>

### <a name="arm"></a><span data-ttu-id="69d51-620">ARM</span><span class="sxs-lookup"><span data-stu-id="69d51-620">ARM</span></span>

* <span data-ttu-id="69d51-621">az deployment create/validate : Utilisation du --handle-extended-json-format par défaut</span><span class="sxs-lookup"><span data-stu-id="69d51-621">az deployment create/validate: Use --handle-extended-json-format by default</span></span>
* <span data-ttu-id="69d51-622">az lock create : Ajout d’exemples de création de sous-ressources dans la documentation d’aide</span><span class="sxs-lookup"><span data-stu-id="69d51-622">az lock create: Add examples of creating subresource in the help documentation</span></span>
* <span data-ttu-id="69d51-623">az deployment {group/mg/sub/tenant} list : Prise en charge du filtrage provisioningState</span><span class="sxs-lookup"><span data-stu-id="69d51-623">az deployment {group/mg/sub/tenant} list: Support provisioningState filtering</span></span>
* <span data-ttu-id="69d51-624">az deployment : Correction du bogue d’analyse pour les commentaires sous le dernier argument</span><span class="sxs-lookup"><span data-stu-id="69d51-624">az deployment: Fix the parse bug for comment under the last argument</span></span>

### <a name="backup"></a><span data-ttu-id="69d51-625">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="69d51-625">Backup</span></span>

* <span data-ttu-id="69d51-626">Ajout de plusieurs fonctionnalités de restauration de fichiers</span><span class="sxs-lookup"><span data-stu-id="69d51-626">Added multiple files restore capabilities</span></span>
* <span data-ttu-id="69d51-627">Ajout de la prise en charge de la sauvegarde des disques de système d’exploitation uniquement</span><span class="sxs-lookup"><span data-stu-id="69d51-627">Added support for Backing up OS Disks only</span></span>
* <span data-ttu-id="69d51-628">Ajout du paramètre restore-as-unmanaged-disk pour spécifier une restauration non gérée</span><span class="sxs-lookup"><span data-stu-id="69d51-628">Added restore-as-unmanaged-disk parameter to specify unmanaged restore</span></span>

### <a name="compute"></a><span data-ttu-id="69d51-629">Calcul</span><span class="sxs-lookup"><span data-stu-id="69d51-629">Compute</span></span>

* <span data-ttu-id="69d51-630">az vm create : Ajout de l’option NONE de --nsg-rule</span><span class="sxs-lookup"><span data-stu-id="69d51-630">az vm create: Add NONE option of --nsg-rule</span></span>
* <span data-ttu-id="69d51-631">az vmss create/update : suppression de la balise d’aperçu des réparations automatiques vmss</span><span class="sxs-lookup"><span data-stu-id="69d51-631">az vmss create/update: remove vmss automatic repairs preview tag</span></span>
* <span data-ttu-id="69d51-632">az vm update : Prise en charge de --workspace</span><span class="sxs-lookup"><span data-stu-id="69d51-632">az vm update: Support --workspace</span></span>
* <span data-ttu-id="69d51-633">Correction d’un bogue dans le code d’initialisation VirtualMachineScaleSetExtension</span><span class="sxs-lookup"><span data-stu-id="69d51-633">Fix a bug in VirtualMachineScaleSetExtension initialization code</span></span>
* <span data-ttu-id="69d51-634">Mise à niveau de VMAccessAgent vers la version 2.4</span><span class="sxs-lookup"><span data-stu-id="69d51-634">Upgrade VMAccessAgent version to 2.4</span></span>
* <span data-ttu-id="69d51-635">az vmss set-orchestration-service-state : prise en charge de l’état de la définition du service d’orchestration vmss</span><span class="sxs-lookup"><span data-stu-id="69d51-635">az vmss set-orchestration-service-state: support vmss set orchestration service state</span></span>
* <span data-ttu-id="69d51-636">Mise à niveau de la version d’API de disque vers la version 2019-11-01</span><span class="sxs-lookup"><span data-stu-id="69d51-636">Upgrade disk API version to 2019-11-01</span></span>
* <span data-ttu-id="69d51-637">az disk create: add --disk-iops-read-only, --disk-mbps-read-only, --max-shares, --image-reference, --image-reference-lun, --gallery-image-reference, --gallery-image-reference-lun</span><span class="sxs-lookup"><span data-stu-id="69d51-637">az disk create: add --disk-iops-read-only, --disk-mbps-read-only, --max-shares, --image-reference, --image-reference-lun, --gallery-image-reference, --gallery-image-reference-lun</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="69d51-638">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="69d51-638">Cosmos DB</span></span>

* <span data-ttu-id="69d51-639">Correction de l’option --type manquante pour les redirections de dépréciation</span><span class="sxs-lookup"><span data-stu-id="69d51-639">Fix missing --type option for deprecation redirections</span></span>

### <a name="docker"></a><span data-ttu-id="69d51-640">Docker</span><span class="sxs-lookup"><span data-stu-id="69d51-640">Docker</span></span>

* <span data-ttu-id="69d51-641">Mise à jour vers Alpine 3.11 et Python 3.6.10</span><span class="sxs-lookup"><span data-stu-id="69d51-641">Update to Alpine 3.11 and Python 3.6.10</span></span>

### <a name="extension"></a><span data-ttu-id="69d51-642">Extension</span><span class="sxs-lookup"><span data-stu-id="69d51-642">Extension</span></span>

* <span data-ttu-id="69d51-643">Autorisation de charger des extensions dans le chemin système via des packages</span><span class="sxs-lookup"><span data-stu-id="69d51-643">Allow to load extensions in the system path via packages</span></span>

### <a name="hdinsight"></a><span data-ttu-id="69d51-644">HDInsight</span><span class="sxs-lookup"><span data-stu-id="69d51-644">HDInsight</span></span>

* <span data-ttu-id="69d51-645">(az hdinsight create:) Les clients du support spécifient une version TLS minimale prise en charge à l’aide du paramètre `--minimal-tls-version`.</span><span class="sxs-lookup"><span data-stu-id="69d51-645">(az hdinsight create:) Support customers specify minimal supported tls version by using parameter `--minimal-tls-version`.</span></span> <span data-ttu-id="69d51-646">La valeur autorisée est 1.0,1.1,1.2</span><span class="sxs-lookup"><span data-stu-id="69d51-646">The allowed value is 1.0,1.1,1.2</span></span>

### <a name="iot"></a><span data-ttu-id="69d51-647">IoT</span><span class="sxs-lookup"><span data-stu-id="69d51-647">IoT</span></span>

* <span data-ttu-id="69d51-648">Ajout de codeowner</span><span class="sxs-lookup"><span data-stu-id="69d51-648">Add codeowner</span></span>
* <span data-ttu-id="69d51-649">az iot hub create : changement de la référence SKU par défaut S1 en F1</span><span class="sxs-lookup"><span data-stu-id="69d51-649">az iot hub create : Change default sku to S1 from F1</span></span>
* <span data-ttu-id="69d51-650">iot hub : Prise en charge d’IotHub dans le profil de 2019-03-01-hybrid</span><span class="sxs-lookup"><span data-stu-id="69d51-650">iot hub: Support IotHub in the profile of 2019-03-01-hybrid</span></span>

### <a name="iotcentral"></a><span data-ttu-id="69d51-651">IotCentral</span><span class="sxs-lookup"><span data-stu-id="69d51-651">IoTCentral</span></span>

* <span data-ttu-id="69d51-652">Mise à jour des détails d’erreur, du modèle d’application par défaut et du message d’invite</span><span class="sxs-lookup"><span data-stu-id="69d51-652">Update error details, update default application template and prompt message</span></span>

### <a name="keyvault"></a><span data-ttu-id="69d51-653">KeyVault</span><span class="sxs-lookup"><span data-stu-id="69d51-653">KeyVault</span></span>

* <span data-ttu-id="69d51-654">Prise en charge de la sauvegarde/restauration de certificat</span><span class="sxs-lookup"><span data-stu-id="69d51-654">Support certificate backup/restore</span></span>
* <span data-ttu-id="69d51-655">keyvault create/update : Prise en charge de --retention-days</span><span class="sxs-lookup"><span data-stu-id="69d51-655">keyvault create/update: Support --retention-days</span></span>
* <span data-ttu-id="69d51-656">Plus d’affichage des clés/secrets managés lors du listing</span><span class="sxs-lookup"><span data-stu-id="69d51-656">No longer display managed keys/secrets while listing</span></span>
* <span data-ttu-id="69d51-657">az keyvault create : prise en charge de `--network-acls`, `--network-acls-ips` et `--network-acls-vnets` pour spécifier des règles réseau lors de la création de coffres</span><span class="sxs-lookup"><span data-stu-id="69d51-657">az keyvault create: support `--network-acls`, `--network-acls-ips` and `--network-acls-vnets` for specifying network rules while creating vault</span></span>

### <a name="lock"></a><span data-ttu-id="69d51-658">Verrouillage</span><span class="sxs-lookup"><span data-stu-id="69d51-658">Lock</span></span>

* <span data-ttu-id="69d51-659">Correction de bogue pour az lock delete : az lock delete ne fonctionne pas sur Microsoft.DocumentDB</span><span class="sxs-lookup"><span data-stu-id="69d51-659">az lock delete fix bug: az lock delete does not work on Microsoft.DocumentDB</span></span>

### <a name="monitor"></a><span data-ttu-id="69d51-660">Superviser</span><span class="sxs-lookup"><span data-stu-id="69d51-660">Monitor</span></span>

* <span data-ttu-id="69d51-661">az monitor clone : prise en charge des règles de clonage de métriques d’une ressource à une autre</span><span class="sxs-lookup"><span data-stu-id="69d51-661">az monitor clone: support clone metric rules from one resource to another</span></span>
* <span data-ttu-id="69d51-662">Correctif IcM179210086 : impossible de créer une alerte de métrique personnalisée pour la métrique Application Insights</span><span class="sxs-lookup"><span data-stu-id="69d51-662">Fix IcM179210086: unable to create custom metric alert for their Application Insights metric</span></span>

### <a name="netappfiles"></a><span data-ttu-id="69d51-663">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="69d51-663">NetAppFiles</span></span>

* <span data-ttu-id="69d51-664">az volume create : Autorisation des volumes de protection des données à ajouter des opérations de réplication : approuver, suspendre, reprendre, état, supprimer</span><span class="sxs-lookup"><span data-stu-id="69d51-664">az volume create: Allow data protection volumes adding replication operations: approve, suspend, resume, status, remove</span></span>

### <a name="network"></a><span data-ttu-id="69d51-665">Réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-665">Network</span></span>

* <span data-ttu-id="69d51-666">az network application-gateway waf-policy managed-rule rule-set add : prise en charge de Microsoft_BotManagerRuleSet</span><span class="sxs-lookup"><span data-stu-id="69d51-666">az network application-gateway waf-policy managed-rule rule-set add: support Microsoft_BotManagerRuleSet</span></span>
* <span data-ttu-id="69d51-667">network watcher flow-log show: correction d’une information de dépréciation fausse</span><span class="sxs-lookup"><span data-stu-id="69d51-667">network watcher flow-log show: fix wrong deprecating info</span></span>
* <span data-ttu-id="69d51-668">Prise en charge des noms d’hôte dans l’écouteur de passerelle d’application</span><span class="sxs-lookup"><span data-stu-id="69d51-668">support host names in application gateway listener</span></span>
* <span data-ttu-id="69d51-669">az network nat gateway : prise en charge de la création d’une ressource vide sans IP publique ni préfixe d’IP publique</span><span class="sxs-lookup"><span data-stu-id="69d51-669">az network nat gateway: support create empty resource without public ip or public ip prefix</span></span>
* <span data-ttu-id="69d51-670">Prise en charge de la génération de passerelles VPN</span><span class="sxs-lookup"><span data-stu-id="69d51-670">Support vpn gateway generation</span></span>
* <span data-ttu-id="69d51-671">Prise en charge de `--if-none-match` dans `az network dns record-set {} add-record`</span><span class="sxs-lookup"><span data-stu-id="69d51-671">Support `--if-none-match` in `az network dns record-set {} add-record`</span></span>

### <a name="packaging"></a><span data-ttu-id="69d51-672">Packaging</span><span class="sxs-lookup"><span data-stu-id="69d51-672">Packaging</span></span>

* <span data-ttu-id="69d51-673">Arrêt de la prise en charge de Python 3.5</span><span class="sxs-lookup"><span data-stu-id="69d51-673">Drop support for python 3.5</span></span>

### <a name="profile"></a><span data-ttu-id="69d51-674">Profil</span><span class="sxs-lookup"><span data-stu-id="69d51-674">Profile</span></span>

* <span data-ttu-id="69d51-675">az login : Affichage d’un avertissement pour l’erreur MFA</span><span class="sxs-lookup"><span data-stu-id="69d51-675">az login: Show warning for MFA error</span></span>

### <a name="rdbms"></a><span data-ttu-id="69d51-676">SGBDR</span><span class="sxs-lookup"><span data-stu-id="69d51-676">RDBMS</span></span>

* <span data-ttu-id="69d51-677">Ajout de commandes de gestion de clés de chiffrement de données de serveur pour PostgreSQL et MySQL</span><span class="sxs-lookup"><span data-stu-id="69d51-677">Add server data encryption key management commands for PostgreSQL and MySQL</span></span>

## <a name="march-10-2020"></a><span data-ttu-id="69d51-678">10 mars 2020</span><span class="sxs-lookup"><span data-stu-id="69d51-678">March 10, 2020</span></span>

<span data-ttu-id="69d51-679">Version 2.2.0</span><span class="sxs-lookup"><span data-stu-id="69d51-679">Version 2.2.0</span></span>

### <a name="acr"></a><span data-ttu-id="69d51-680">ACR</span><span class="sxs-lookup"><span data-stu-id="69d51-680">ACR</span></span>

* <span data-ttu-id="69d51-681">Correctif : `az acr login` déclenche une erreur de manière erronée</span><span class="sxs-lookup"><span data-stu-id="69d51-681">Fix: `az acr login` wrongly raise error</span></span>
* <span data-ttu-id="69d51-682">Ajout d’une nouvelle commande `az acr helm install-cli`</span><span class="sxs-lookup"><span data-stu-id="69d51-682">Add new command `az acr helm install-cli`</span></span>
* <span data-ttu-id="69d51-683">Ajout d’un lien privé et de la prise en charge CMK</span><span class="sxs-lookup"><span data-stu-id="69d51-683">Add private link and CMK support</span></span>
* <span data-ttu-id="69d51-684">Ajout de la commande « private-link-resource list »</span><span class="sxs-lookup"><span data-stu-id="69d51-684">add 'private-link-resource list' command</span></span>

### <a name="aks"></a><span data-ttu-id="69d51-685">AKS</span><span class="sxs-lookup"><span data-stu-id="69d51-685">AKS</span></span>

* <span data-ttu-id="69d51-686">Correction de la navigation aks dans Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="69d51-686">fix the aks browse in cloud shell</span></span>
* <span data-ttu-id="69d51-687">az aks : correction de la supervision des erreurs NoneType addon et agentpool</span><span class="sxs-lookup"><span data-stu-id="69d51-687">az aks: Fix monitoring addon and agentpool NoneType errors</span></span>
* <span data-ttu-id="69d51-688">Ajout de --nodepool-tags au pool de nœuds lors de la création de cluster Azure Kubernetes</span><span class="sxs-lookup"><span data-stu-id="69d51-688">Add --nodepool-tags to node pool when creating azure kubernetes cluster</span></span>
* <span data-ttu-id="69d51-689">Ajout de --tags lors de l’ajout ou de la mise à jour d’un nodepool à un cluster</span><span class="sxs-lookup"><span data-stu-id="69d51-689">Add --tags when adding or updating a nodepool to cluster</span></span>
* <span data-ttu-id="69d51-690">aks create : ajout de `--enable-private-cluster`</span><span class="sxs-lookup"><span data-stu-id="69d51-690">aks create: add `--enable-private-cluster`</span></span>
* <span data-ttu-id="69d51-691">Ajout de --nodepool-labels lors de la création de cluster Azure Kubernetes</span><span class="sxs-lookup"><span data-stu-id="69d51-691">add --nodepool-labels when creating azure kubernetes cluster</span></span>
* <span data-ttu-id="69d51-692">Ajout de --labels lors de l’ajout d’un nouveau nodepool à un cluster Azure Kubernetes</span><span class="sxs-lookup"><span data-stu-id="69d51-692">add --labels when adding a new nodepool to azure kubernetes cluster</span></span>
* <span data-ttu-id="69d51-693">Ajout d’un caractère / manquant à l’URL de tableau de bord</span><span class="sxs-lookup"><span data-stu-id="69d51-693">add missing / in the dashboard url</span></span>
* <span data-ttu-id="69d51-694">Prise en charge de la création de clusters AKS activant l’identité managée</span><span class="sxs-lookup"><span data-stu-id="69d51-694">Support create aks clusters enabling managed identity</span></span>
* <span data-ttu-id="69d51-695">az aks : validation du plug-in réseau pour qu’il soit « azure » ou « kubenet »</span><span class="sxs-lookup"><span data-stu-id="69d51-695">az aks: Validate network plugin to be either "azure" or "kubenet"</span></span>
* <span data-ttu-id="69d51-696">az aks : Ajout de la prise en charge des clés de session AAD</span><span class="sxs-lookup"><span data-stu-id="69d51-696">az aks: Add aad session key support</span></span>
* <span data-ttu-id="69d51-697">[CHANGEMENT CASSANT] az aks : prise en charge des modifications MSI pour GF et BF pour omsagent (supervision de conteneur) (#1)</span><span class="sxs-lookup"><span data-stu-id="69d51-697">[BREAKING CHANGE] az aks: support msi changes for GF and BF for omsagent (Container monitoring)(#1)</span></span>
* <span data-ttu-id="69d51-698">az aks use-dev-spaces : ajout de l’option de type de point de terminaison à la commande use-dev-spaces pour personnaliser le point de terminaison créé sur un contrôleur Azure Dev Spaces</span><span class="sxs-lookup"><span data-stu-id="69d51-698">az aks use-dev-spaces: Adding endpoint type option to the use-dev-spaces command to customize the endpoint created on an Azure Dev Spaces controller</span></span>

### <a name="appconfig"></a><span data-ttu-id="69d51-699">AppConfig</span><span class="sxs-lookup"><span data-stu-id="69d51-699">AppConfig</span></span>

* <span data-ttu-id="69d51-700">Déblocage de l’utilisation de « kv set » pour ajouter la fonctionnalité et la référence de coffre de clés</span><span class="sxs-lookup"><span data-stu-id="69d51-700">Unblock using "kv set" to add keyvault reference and feature …</span></span>

### <a name="appservice"></a><span data-ttu-id="69d51-701">AppService</span><span class="sxs-lookup"><span data-stu-id="69d51-701">AppService</span></span>

* <span data-ttu-id="69d51-702">az webapp create : résolution d’un problème lors de l’exécution de la commande avec --runtime</span><span class="sxs-lookup"><span data-stu-id="69d51-702">az webapp create : Fix issue when running the command with --runtime</span></span>
* <span data-ttu-id="69d51-703">az functionapp deployment source config-zip : ajout d’un message d’erreur si le nom du groupe de ressources ou de la fonction n’est pas valide ou n’existe pas</span><span class="sxs-lookup"><span data-stu-id="69d51-703">az functionapp deployment source config-zip: Add an error message if resource group or function name are invalid/don't exist</span></span>
* <span data-ttu-id="69d51-704">functionapp create : correction du message d’avertissement qui s’affiche aujourd’hui avec `functionapp create`, qui mentionne un indicateur `--functions_version` mais utilise de manière erronée un `_` au lieu d’un `-` dans le nom de l’indicateur.</span><span class="sxs-lookup"><span data-stu-id="69d51-704">functionapp create: Fix the warning message that appears with `functionapp create` today which cites a `--functions_version` flag but erroneously uses a `_` instead of a `-` in the flag name</span></span>
* <span data-ttu-id="69d51-705">az functionapp create : mise à jour de la façon dont linuxFxVersion et le nom de l’image conteneur étaient définis pour les applications de fonction Linux</span><span class="sxs-lookup"><span data-stu-id="69d51-705">az functionapp create: Updated the way linuxFxVersion and container image name were being set for linux function apps</span></span>
* <span data-ttu-id="69d51-706">az functionapp deployment source config-zip : résolution d’un problème dû à une condition de concurrence en cas de modification des paramètres d’application pendant le déploiement de fichier zip, provoquant des erreurs 5xx lors du déploiement</span><span class="sxs-lookup"><span data-stu-id="69d51-706">az functionapp deployment source config-zip: Fix an issue caused by app settings change racing condition during zip deploy, giving 5xx errors during deployment</span></span>
* <span data-ttu-id="69d51-707">Correctif 5720946 : az webapp backup ne parvient pas à définir le nom</span><span class="sxs-lookup"><span data-stu-id="69d51-707">Fix #5720946: az webapp backup fails to set name</span></span>

### <a name="arm"></a><span data-ttu-id="69d51-708">ARM</span><span class="sxs-lookup"><span data-stu-id="69d51-708">ARM</span></span>

* <span data-ttu-id="69d51-709">az resource : amélioration des exemples du module de ressources</span><span class="sxs-lookup"><span data-stu-id="69d51-709">az resource: Improve the examples of the resource module</span></span>
* <span data-ttu-id="69d51-710">az policy assignment list : prise en charge de l’énumération des affectations de stratégie au niveau de l’étendue du groupe d’administration</span><span class="sxs-lookup"><span data-stu-id="69d51-710">az policy assignment list: Support listing policy assignments at Management Group scope</span></span>
* <span data-ttu-id="69d51-711">Ajout de `az deployment group` et `az deployment operation group` pour le déploiement de modèle au niveau des groupes de ressources.</span><span class="sxs-lookup"><span data-stu-id="69d51-711">Add `az deployment group` and `az deployment operation group` for template deployment at resource groups.</span></span> <span data-ttu-id="69d51-712">Il s’agit d’un doublon de `az group deployment` et `az group deployment operation`</span><span class="sxs-lookup"><span data-stu-id="69d51-712">This is a duplicate of `az group deployment` and `az group deployment operation`</span></span>
* <span data-ttu-id="69d51-713">Ajout de `az deployment sub` et `az deployment operation sub` pour le déploiement de modèle à l’étendue de l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="69d51-713">Add `az deployment sub` and `az deployment operation sub` for template deployment at subscription scope.</span></span> <span data-ttu-id="69d51-714">Il s’agit d’un doublon de `az deployment` et `az deployment operation`</span><span class="sxs-lookup"><span data-stu-id="69d51-714">This is a duplicate of `az deployment` and `az deployment operation`</span></span>
* <span data-ttu-id="69d51-715">Ajout de `az deployment mg` et `az deployment operation mg` pour le déploiement de modèle au niveau des groupes de gestion</span><span class="sxs-lookup"><span data-stu-id="69d51-715">Add `az deployment mg` and `az deployment operation mg` for template deployment at management groups</span></span>
* <span data-ttu-id="69d51-716">Ajout de `az deployment tenant` et `az deployment operation tenant` pour le déploiement de modèle à l’étendue du locataire</span><span class="sxs-lookup"><span data-stu-id="69d51-716">Add `az deployment tenant` and `az deployment operation tenant` for template deployment at tenant scope</span></span>
* <span data-ttu-id="69d51-717">az policy assignment create : ajout d’une description au paramètre `--location`</span><span class="sxs-lookup"><span data-stu-id="69d51-717">az policy assignment create: Add a description to the `--location` parameter</span></span>
* <span data-ttu-id="69d51-718">az group deployment create : ajout du paramètre `--aux-tenants` pour prendre en charge les locataires croisés</span><span class="sxs-lookup"><span data-stu-id="69d51-718">az group deployment create: Add parameter `--aux-tenants` to support cross tenants</span></span>

### <a name="cdn"></a><span data-ttu-id="69d51-719">CDN</span><span class="sxs-lookup"><span data-stu-id="69d51-719">CDN</span></span>

* <span data-ttu-id="69d51-720">Ajouter de commandes WAF CDN</span><span class="sxs-lookup"><span data-stu-id="69d51-720">Add CDN WAF commands</span></span>

### <a name="compute"></a><span data-ttu-id="69d51-721">Calcul</span><span class="sxs-lookup"><span data-stu-id="69d51-721">Compute</span></span>

* <span data-ttu-id="69d51-722">az sig image-version : ajout de --data-snapshot-luns</span><span class="sxs-lookup"><span data-stu-id="69d51-722">az sig image-version: add --data-snapshot-luns</span></span>
* <span data-ttu-id="69d51-723">az ppg show: ajout de --colocation-status pour permettre l’extraction de l’état de colocalisation de toutes les ressources dans le groupe de placement de proximité</span><span class="sxs-lookup"><span data-stu-id="69d51-723">az ppg show: add --colocation-status to enable fetching the colocation status of all the resources in the proximity placement group</span></span>
* <span data-ttu-id="69d51-724">az vmss create/update : prise en charge des réparations automatiques</span><span class="sxs-lookup"><span data-stu-id="69d51-724">az vmss create/update: support automatic repairs</span></span>
* <span data-ttu-id="69d51-725">[CHANGEMENT CASSANT] az image template : template a été renommé builder</span><span class="sxs-lookup"><span data-stu-id="69d51-725">[BREAKING CHANGE] az image template: rename template to builder</span></span>
* <span data-ttu-id="69d51-726">az image builder create : ajout de --image-template</span><span class="sxs-lookup"><span data-stu-id="69d51-726">az image builder create: add --image-template</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="69d51-727">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="69d51-727">Cosmos DB</span></span>

* <span data-ttu-id="69d51-728">Ajout d’applets de commande de déclencheur, de procédure stockée SQL et de fonctions définies par l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="69d51-728">Add Sql stored procedure, udf and trigger cmdlets</span></span>
* <span data-ttu-id="69d51-729">az cosmosdb create : ajout de --key-uri pour prendre en charge l’ajout d’informations de chiffrement de coffre de clés</span><span class="sxs-lookup"><span data-stu-id="69d51-729">az cosmosdb create: add --key-uri to support adding key vault encryption information</span></span>

### <a name="keyvault"></a><span data-ttu-id="69d51-730">KeyVault</span><span class="sxs-lookup"><span data-stu-id="69d51-730">KeyVault</span></span>

* <span data-ttu-id="69d51-731">keyvault create : activation de la suppression réversible par défaut</span><span class="sxs-lookup"><span data-stu-id="69d51-731">keyvault create: enable soft-delete by default</span></span>

### <a name="monitor"></a><span data-ttu-id="69d51-732">Superviser</span><span class="sxs-lookup"><span data-stu-id="69d51-732">Monitor</span></span>

* <span data-ttu-id="69d51-733">az monitor metrics alert create : prise en charge de `~` dans `--condition`</span><span class="sxs-lookup"><span data-stu-id="69d51-733">az monitor metrics alert create: support `~` in `--condition`</span></span>

### <a name="network"></a><span data-ttu-id="69d51-734">Réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-734">Network</span></span>

* <span data-ttu-id="69d51-735">az network application-gateway rewrite-rule create : prise en charge de la configuration d’URL</span><span class="sxs-lookup"><span data-stu-id="69d51-735">az network application-gateway rewrite-rule create: support url configuration</span></span>
* <span data-ttu-id="69d51-736">az network dns zone import : --zone-name respectera la casse à l’avenir</span><span class="sxs-lookup"><span data-stu-id="69d51-736">az network dns zone import: --zone-name will be case insensitive in the future</span></span>
* <span data-ttu-id="69d51-737">az network private-endpoint/private-link-service : suppression de l’étiquette d’aperçu</span><span class="sxs-lookup"><span data-stu-id="69d51-737">az network private-endpoint/private-link-service: remove preview label</span></span>
* <span data-ttu-id="69d51-738">az network bastion : prise en charge de bastion</span><span class="sxs-lookup"><span data-stu-id="69d51-738">az network bastion: support bastion</span></span>
* <span data-ttu-id="69d51-739">az network vnet list-available-ips : prise en charge de l’énumération des adresses IP disponibles sur un réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="69d51-739">az network vnet list-available-ips: support list available ips in a vnet</span></span>
* <span data-ttu-id="69d51-740">az network watcher flow-log create/list/delete/update : ajout de nouvelles commandes pour gérer le journal de flux d’observateur et l’exposition de --location pour identifier explicitement l’observateur</span><span class="sxs-lookup"><span data-stu-id="69d51-740">az network watcher flow-log create/list/delete/update: add new commands to manage watcher flow log and exposing --location to identify watcher explicitly</span></span>
* <span data-ttu-id="69d51-741">az network watcher flow-log configure : dépréciée</span><span class="sxs-lookup"><span data-stu-id="69d51-741">az network watcher flow-log configure: deprecated</span></span>
* <span data-ttu-id="69d51-742">az network watcher flow-log show : prise en charge de --location et de --name pour obtenir un résultat au format ARM. L’ancienne sortie mise en forme est dépréciée</span><span class="sxs-lookup"><span data-stu-id="69d51-742">az network watcher flow-log show: support --location and --name to get ARM-formatted result, deprecated old formatted output</span></span>

### <a name="policy"></a><span data-ttu-id="69d51-743">Policy</span><span class="sxs-lookup"><span data-stu-id="69d51-743">Policy</span></span>

* <span data-ttu-id="69d51-744">az policy assignment create : correction du bogue qui générait automatiquement un nom d’attribution de stratégie dépassant la limite</span><span class="sxs-lookup"><span data-stu-id="69d51-744">az policy assignment create: Fix the bug that automatically generated name of policy assignment exceeds the limit</span></span>

### <a name="rbac"></a><span data-ttu-id="69d51-745">RBAC</span><span class="sxs-lookup"><span data-stu-id="69d51-745">RBAC</span></span>

* <span data-ttu-id="69d51-746">az ad group show : correction du bogue qui faisait que --group était traité comme un problème Regex</span><span class="sxs-lookup"><span data-stu-id="69d51-746">az ad group show: fix --group value treated as regex problem</span></span>

### <a name="rdbms"></a><span data-ttu-id="69d51-747">SGBDR</span><span class="sxs-lookup"><span data-stu-id="69d51-747">RDBMS</span></span>

* <span data-ttu-id="69d51-748">Passage du SDK azure-mgmt-rdbms à la version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="69d51-748">Bump the azure-mgmt-rdbms SDK version to 2.0.0</span></span>
* <span data-ttu-id="69d51-749">az postgres private-endpoint-connection : gestion des connexions de point de terminaison privé postgres</span><span class="sxs-lookup"><span data-stu-id="69d51-749">az postgres private-endpoint-connection: manage postgres private endpoint connections</span></span>
* <span data-ttu-id="69d51-750">az postgres private-link-resource : gestion des ressources de lien privé postgres</span><span class="sxs-lookup"><span data-stu-id="69d51-750">az postgres private-link-resource: manage postgres private link resources</span></span>
* <span data-ttu-id="69d51-751">az mysql private-endpoint-connection : gestion des connexions de point de terminaison privé mysql</span><span class="sxs-lookup"><span data-stu-id="69d51-751">az mysql private-endpoint-connection: manage mysql private endpoint connections</span></span>
* <span data-ttu-id="69d51-752">az mysql private-link-resource : gestion des ressources de lien privé mysql</span><span class="sxs-lookup"><span data-stu-id="69d51-752">az mysql private-link-resource: manage mysql private link resources</span></span>
* <span data-ttu-id="69d51-753">az mariadb private-endpoint-connection : gestion des connexions de point de terminaison privé mariadb</span><span class="sxs-lookup"><span data-stu-id="69d51-753">az mariadb private-endpoint-connection: manage mariadb private endpoint connections</span></span>
* <span data-ttu-id="69d51-754">az mariadb private-link-resource : gestion des ressources de lien privé mariadb</span><span class="sxs-lookup"><span data-stu-id="69d51-754">az mariadb private-link-resource: manage mariadb private link resources</span></span>
* <span data-ttu-id="69d51-755">Mise à jour des tests de point de terminaison privé SGBDR</span><span class="sxs-lookup"><span data-stu-id="69d51-755">Updating RDBMS Private Endpoint Tests</span></span>

### <a name="sql"></a><span data-ttu-id="69d51-756">SQL</span><span class="sxs-lookup"><span data-stu-id="69d51-756">SQL</span></span>

* <span data-ttu-id="69d51-757">Sql midb ; ajout de list-deleted, show-deleted, update-retention, show-retention</span><span class="sxs-lookup"><span data-stu-id="69d51-757">Sql midb Add: list-deleted, show-deleted, update-retention, show-retention</span></span>
* <span data-ttu-id="69d51-758">(sql server create :) Ajout de l’indicateur facultatif « Enable »/« Disable » d’accès au réseau public à sql server create</span><span class="sxs-lookup"><span data-stu-id="69d51-758">(sql server create:) Add optional public-network-access 'Enable'/'Disable' flag to sql server create</span></span>
* <span data-ttu-id="69d51-759">(sql server update :) modifications du client</span><span class="sxs-lookup"><span data-stu-id="69d51-759">(sql server update:) make some customer-facing change</span></span>
* <span data-ttu-id="69d51-760">Ajout de propriété minimal_tls_version pour MI et SQL DB</span><span class="sxs-lookup"><span data-stu-id="69d51-760">Add minimal_tls_version property for MI and SQL DB</span></span>

### <a name="storage"></a><span data-ttu-id="69d51-761">Stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-761">Storage</span></span>

* <span data-ttu-id="69d51-762">az storage blob delete-batch : comportement incorrect de l’indicateur `--dryrun`</span><span class="sxs-lookup"><span data-stu-id="69d51-762">az storage blob delete-batch: Misbehaving `--dryrun` flag</span></span>
* <span data-ttu-id="69d51-763">az storage account network-rule add (correctif de bogue) : l’opération d’ajout doit être idempotent</span><span class="sxs-lookup"><span data-stu-id="69d51-763">az storage account network-rule add (bug fix): add operation should be idempotent</span></span>
* <span data-ttu-id="69d51-764">az storage account create/update : Ajout de la prise en charge des préférences de routage</span><span class="sxs-lookup"><span data-stu-id="69d51-764">az storage account create/update: Add Routing Preference support</span></span>
* <span data-ttu-id="69d51-765">Mise à niveau de la version azure-mgmt-storage vers 8.0.0</span><span class="sxs-lookup"><span data-stu-id="69d51-765">Upgrade azure-mgmt-storage version to 8.0.0</span></span>
* <span data-ttu-id="69d51-766">az storage container immutability create : ajout du paramètre --allow-protected-append-write</span><span class="sxs-lookup"><span data-stu-id="69d51-766">az storage container immutability create: add --allow-protected-append-write parameter</span></span>
* <span data-ttu-id="69d51-767">az storage account private-link-resource list : ajout de la prise en charge de l’énumération des ressources de lien privé pour le compte de stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-767">az storage account private-link-resource list: Add support to list private link resources for storage account</span></span>
* <span data-ttu-id="69d51-768">az storage account private-endpoint-connection approve/reject/show/delete : prise en charge de la gestion des connexions de point de terminaison privé</span><span class="sxs-lookup"><span data-stu-id="69d51-768">az storage account private-endpoint-connection approve/reject/show/delete: Support to manage private endpoint connections</span></span>
* <span data-ttu-id="69d51-769">az storage account blob-service-properties update : ajout de --enable-restore-policy et --restore-days</span><span class="sxs-lookup"><span data-stu-id="69d51-769">az storage account blob-service-properties update: add --enable-restore-policy and --restore-days</span></span>
* <span data-ttu-id="69d51-770">az storage blob restore : ajout de la prise en charge de la restauration des plages d’objets blob</span><span class="sxs-lookup"><span data-stu-id="69d51-770">az storage blob restore: Add support to restore blob ranges</span></span>

## <a name="february-18-2020"></a><span data-ttu-id="69d51-771">18 février 2020</span><span class="sxs-lookup"><span data-stu-id="69d51-771">February 18, 2020</span></span>

<span data-ttu-id="69d51-772">Version 2.1.0</span><span class="sxs-lookup"><span data-stu-id="69d51-772">Version 2.1.0</span></span>

### <a name="acr"></a><span data-ttu-id="69d51-773">ACR</span><span class="sxs-lookup"><span data-stu-id="69d51-773">ACR</span></span>

* <span data-ttu-id="69d51-774">Ajoute un nouvel argument `--expose-token` pour `az acr login`</span><span class="sxs-lookup"><span data-stu-id="69d51-774">Add a new argument `--expose-token` for `az acr login`</span></span>
* <span data-ttu-id="69d51-775">Corrige la sortie incorrecte de `az acr task identity show -n Name -r Registry -o table`</span><span class="sxs-lookup"><span data-stu-id="69d51-775">Fix the incorrect output of `az acr task identity show -n Name -r Registry -o table`</span></span>
* <span data-ttu-id="69d51-776">az acr login : lève une CLIError si des erreurs sont retournées par la commande docker</span><span class="sxs-lookup"><span data-stu-id="69d51-776">az acr login: Throw a CLIError if there are errors returned by docker command</span></span>

### <a name="acs"></a><span data-ttu-id="69d51-777">ACS</span><span class="sxs-lookup"><span data-stu-id="69d51-777">ACS</span></span>

* <span data-ttu-id="69d51-778">aks create/update : ajoute la validation `--vnet-subnet-id`</span><span class="sxs-lookup"><span data-stu-id="69d51-778">aks create/update: add `--vnet-subnet-id` validation</span></span>

### <a name="aladdin"></a><span data-ttu-id="69d51-779">Aladdin</span><span class="sxs-lookup"><span data-stu-id="69d51-779">Aladdin</span></span>

* <span data-ttu-id="69d51-780">Analyse les exemples générés dans le _help.py des commandes</span><span class="sxs-lookup"><span data-stu-id="69d51-780">Parse generated examples into commands' _help.py</span></span>

### <a name="ams"></a><span data-ttu-id="69d51-781">AMS</span><span class="sxs-lookup"><span data-stu-id="69d51-781">AMS</span></span>

* <span data-ttu-id="69d51-782">az ams est désormais en disponibilité générale</span><span class="sxs-lookup"><span data-stu-id="69d51-782">az ams is GA now</span></span>

### <a name="appconfig"></a><span data-ttu-id="69d51-783">AppConfig</span><span class="sxs-lookup"><span data-stu-id="69d51-783">AppConfig</span></span>

* <span data-ttu-id="69d51-784">Modifie le message d’aide pour exclure les filtres de clé ou d’étiquette non pris en charge</span><span class="sxs-lookup"><span data-stu-id="69d51-784">Revise help message to exclude unsupported key/label filter</span></span>
* <span data-ttu-id="69d51-785">Supprimer l’étiquette d’aperçu pour la plupart des commandes, à l’exception des indicateurs d’identité managée et de fonctionnalités</span><span class="sxs-lookup"><span data-stu-id="69d51-785">Remove preview tag for most commands excluding managed identity and feature flags</span></span>
* <span data-ttu-id="69d51-786">Ajoute une clé gérée par le client lors de la mise à jour des magasins</span><span class="sxs-lookup"><span data-stu-id="69d51-786">Add customer managed key when updating stores</span></span>

### <a name="appservice"></a><span data-ttu-id="69d51-787">AppService</span><span class="sxs-lookup"><span data-stu-id="69d51-787">AppService</span></span>

* <span data-ttu-id="69d51-788">az webapp list-runtimes : correction du bogue concernant list-runtimes</span><span class="sxs-lookup"><span data-stu-id="69d51-788">az webapp list-runtimes: Fix the bug for list-runtimes</span></span>
* <span data-ttu-id="69d51-789">Ajoute az webapp|functionapp config ssl create</span><span class="sxs-lookup"><span data-stu-id="69d51-789">Add az webapp|functionapp config ssl create</span></span>
* <span data-ttu-id="69d51-790">Ajoute la prise en charge des applications de fonction v3 et du nœud 12</span><span class="sxs-lookup"><span data-stu-id="69d51-790">Add support for v3 function apps and node 12</span></span>

### <a name="arm"></a><span data-ttu-id="69d51-791">ARM</span><span class="sxs-lookup"><span data-stu-id="69d51-791">ARM</span></span>

* <span data-ttu-id="69d51-792">az policy assignment create : correction du message d’erreur lorsque le paramètre `--policy` n’est pas valide</span><span class="sxs-lookup"><span data-stu-id="69d51-792">az policy assignment create: Fix the error message when the `--policy` parameter is invalid</span></span>
* <span data-ttu-id="69d51-793">az group deployment create : correction de l’erreur « stat: path too long for Windows » (Chemin trop long pour Windows) lors de l’utilisation d’un fichier parameters.json volumineux</span><span class="sxs-lookup"><span data-stu-id="69d51-793">az group deployment create: Fix "stat: path too long for Windows" error when using large parameters.json file</span></span>

### <a name="backup"></a><span data-ttu-id="69d51-794">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="69d51-794">Backup</span></span>

* <span data-ttu-id="69d51-795">Correction du flux de récupération au niveau de l’élément dans OLR</span><span class="sxs-lookup"><span data-stu-id="69d51-795">Fix for item level recovery flow in OLR</span></span>
* <span data-ttu-id="69d51-796">Ajout de la prise en charge de la restauration sous forme de fichiers pour les bases de données SQL et SAP</span><span class="sxs-lookup"><span data-stu-id="69d51-796">Add restore as files support for SQL and SAP Databases</span></span>

### <a name="compute"></a><span data-ttu-id="69d51-797">Calcul</span><span class="sxs-lookup"><span data-stu-id="69d51-797">Compute</span></span>

* <span data-ttu-id="69d51-798">vm/vmss/availability-set update: add --ppg to allowing updating ProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="69d51-798">vm/vmss/availability-set update: add --ppg to allowing updating ProximityPlacementGroup</span></span>
* <span data-ttu-id="69d51-799">vmss create: add --data-disk-iops and --data-disk-mbps</span><span class="sxs-lookup"><span data-stu-id="69d51-799">vmss create: add --data-disk-iops and --data-disk-mbps</span></span>
* <span data-ttu-id="69d51-800">az vm host : supprime l’étiquette d’aperçu pour `vm host` et `vm host group`</span><span class="sxs-lookup"><span data-stu-id="69d51-800">az vm host: remove preview tag for `vm host` and `vm host group`</span></span>
* <span data-ttu-id="69d51-801">[CHANGEMENT CASSANT] Correctif n° 10728 : `az vm create` Création automatique d’un sous-réseau si un réseau virtuel est spécifié et s’il n’existe pas de sous-réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-801">[BREAKING CHANGE] Fix #10728: `az vm create`: create subnet automatically if vnet is specified and subnet not exists</span></span>
* <span data-ttu-id="69d51-802">Amélioration de la robustesse de la liste d’images de machines virtuelles</span><span class="sxs-lookup"><span data-stu-id="69d51-802">Increase robustness of vm image list</span></span>

### <a name="eventhub"></a><span data-ttu-id="69d51-803">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="69d51-803">Eventhub</span></span>

* <span data-ttu-id="69d51-804">Prise en charge d’Azure Stack pour le profil 2019-03-01-hybrid</span><span class="sxs-lookup"><span data-stu-id="69d51-804">Azure Stack support for 2019-03-01-hybrid profile</span></span>

### <a name="keyvault"></a><span data-ttu-id="69d51-805">KeyVault</span><span class="sxs-lookup"><span data-stu-id="69d51-805">KeyVault</span></span>

* <span data-ttu-id="69d51-806">az keyvault key create : ajouter une nouvelle valeur `import` pour le paramètre `--ops`</span><span class="sxs-lookup"><span data-stu-id="69d51-806">az keyvault key create: add a new value `import` for parameter `--ops`</span></span>
* <span data-ttu-id="69d51-807">az keyvault key list-versions : prise en charge du paramètre `--id` pour la spécification des clés</span><span class="sxs-lookup"><span data-stu-id="69d51-807">az keyvault key list-versions: support parameter `--id` for specifying keys</span></span>
* <span data-ttu-id="69d51-808">Prise en charge des connexions de points de terminaison privés</span><span class="sxs-lookup"><span data-stu-id="69d51-808">Support private endpoint connections</span></span>

### <a name="network"></a><span data-ttu-id="69d51-809">Réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-809">Network</span></span>

* <span data-ttu-id="69d51-810">Passage à azure-mgmt-network 9.0.0</span><span class="sxs-lookup"><span data-stu-id="69d51-810">Bump to azure-mgmt-network 9.0.0</span></span>
* <span data-ttu-id="69d51-811">az network private-link-service update/create: support --enable-proxy-protocol</span><span class="sxs-lookup"><span data-stu-id="69d51-811">az network private-link-service update/create: support --enable-proxy-protocol</span></span>
* <span data-ttu-id="69d51-812">Ajout de la fonctionnalité Moniteur de connexion v2</span><span class="sxs-lookup"><span data-stu-id="69d51-812">Add connection Monitor V2 feature</span></span>

### <a name="packaging"></a><span data-ttu-id="69d51-813">Packaging</span><span class="sxs-lookup"><span data-stu-id="69d51-813">Packaging</span></span>

* <span data-ttu-id="69d51-814">[CHANGEMENT CASSANT] Python 2.7 n’est plus pris en charge</span><span class="sxs-lookup"><span data-stu-id="69d51-814">[BREAKING CHANGE] Drop support for Python 2.7</span></span>

### <a name="profile"></a><span data-ttu-id="69d51-815">Profil</span><span class="sxs-lookup"><span data-stu-id="69d51-815">Profile</span></span>

* <span data-ttu-id="69d51-816">Aperçu : Ajoutez les nouveaux attributs `homeTenantId` et `managedByTenants` aux comptes d’abonnement.</span><span class="sxs-lookup"><span data-stu-id="69d51-816">Preview: Add new attributes `homeTenantId` and `managedByTenants` to subscription accounts.</span></span> <span data-ttu-id="69d51-817">Réexécutez `az login` pour que les modifications soient prises en compte.</span><span class="sxs-lookup"><span data-stu-id="69d51-817">Please re-run `az login` for the changes to take effect</span></span>
* <span data-ttu-id="69d51-818">az login : affiche un avertissement lorsqu’un abonnement est listé par plusieurs locataires et s’affiche par défaut pour le premier.</span><span class="sxs-lookup"><span data-stu-id="69d51-818">az login: Show a warning when a subscription is listed from more than one tenants and default to the first one.</span></span> <span data-ttu-id="69d51-819">Pour sélectionner un locataire lors de l’accès à cet abonnement, ajoutez `--tenant` dans `az login`</span><span class="sxs-lookup"><span data-stu-id="69d51-819">To select a specific tenant when accessing this subscription, please include `--tenant` in `az login`</span></span>

### <a name="role"></a><span data-ttu-id="69d51-820">Role</span><span class="sxs-lookup"><span data-stu-id="69d51-820">Role</span></span>

* <span data-ttu-id="69d51-821">az role assignment create : correction de l’erreur lors de laquelle l’attribution d’un rôle à un principal de service par nom d’affichage générait une erreur HTTP 400</span><span class="sxs-lookup"><span data-stu-id="69d51-821">az role assignment create: Fix the error that assigning a role to a service principal by display name yields a HTTP 400</span></span>

### <a name="sql"></a><span data-ttu-id="69d51-822">SQL</span><span class="sxs-lookup"><span data-stu-id="69d51-822">SQL</span></span>

* <span data-ttu-id="69d51-823">Mise à jour de l’applet de commande SQL Managed Instance `az sql mi update` avec deux nouveaux paramètres : tier et family</span><span class="sxs-lookup"><span data-stu-id="69d51-823">Update SQL Managed Instance cmdlet `az sql mi update` with two new parameters: tier and family</span></span>

### <a name="storage"></a><span data-ttu-id="69d51-824">Stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-824">Storage</span></span>

* <span data-ttu-id="69d51-825">[CHANGEMENT CASSANT] `az storage account create` : Remplacement du type de compte de stockage par défaut par StorageV2</span><span class="sxs-lookup"><span data-stu-id="69d51-825">[BREAKING CHANGE] `az storage account create`: Change default storage account kind to StorageV2</span></span>

## <a name="february-04-2020"></a><span data-ttu-id="69d51-826">4 février 2020</span><span class="sxs-lookup"><span data-stu-id="69d51-826">February 04, 2020</span></span>

<span data-ttu-id="69d51-827">Version 2.0.81</span><span class="sxs-lookup"><span data-stu-id="69d51-827">Version 2.0.81</span></span>

### <a name="acs"></a><span data-ttu-id="69d51-828">ACS</span><span class="sxs-lookup"><span data-stu-id="69d51-828">ACS</span></span>

* <span data-ttu-id="69d51-829">Ajout de la prise en charge de la définition des ports alloués sortants et des délais d’inactivité sur l’équilibreur de charge standard</span><span class="sxs-lookup"><span data-stu-id="69d51-829">Add support to set outbound allocated ports and idle timeouts on standard load balancer</span></span>
* <span data-ttu-id="69d51-830">Mise à jour vers la version d’API 2019-11-01</span><span class="sxs-lookup"><span data-stu-id="69d51-830">Update to API Version 2019-11-01</span></span>

### <a name="acr"></a><span data-ttu-id="69d51-831">ACR</span><span class="sxs-lookup"><span data-stu-id="69d51-831">ACR</span></span>

* <span data-ttu-id="69d51-832">[CHANGEMENT CASSANT] `az acr delete` affiche une invite</span><span class="sxs-lookup"><span data-stu-id="69d51-832">[BREAKING CHANGE] `az acr delete` will prompt</span></span>
* <span data-ttu-id="69d51-833">[CHANGEMENT CASSANT] 'az acr task delete' affiche une invite</span><span class="sxs-lookup"><span data-stu-id="69d51-833">[BREAKING CHANGE] 'az acr task delete' will prompt</span></span>
* <span data-ttu-id="69d51-834">Ajout du nouveau groupe de commandes 'az acr taskrun show/list/delete' pour la gestion de l’exécution des tâches</span><span class="sxs-lookup"><span data-stu-id="69d51-834">Add a new command group 'az acr taskrun show/list/delete' for taskrun management</span></span>

### <a name="aks"></a><span data-ttu-id="69d51-835">AKS</span><span class="sxs-lookup"><span data-stu-id="69d51-835">AKS</span></span>

* <span data-ttu-id="69d51-836">Chaque cluster obtient un principal de service distinct pour améliorer l’isolation</span><span class="sxs-lookup"><span data-stu-id="69d51-836">Each cluster gets a separate service principal to improve isolation</span></span>

### <a name="appconfig"></a><span data-ttu-id="69d51-837">AppConfig</span><span class="sxs-lookup"><span data-stu-id="69d51-837">AppConfig</span></span>

* <span data-ttu-id="69d51-838">Prise en charge de l’importation/exportation des références keyvault depuis/vers appservice</span><span class="sxs-lookup"><span data-stu-id="69d51-838">Support import/export of keyvault references from/to appservice</span></span>
* <span data-ttu-id="69d51-839">Prise en charge de l’importation/exportation de toutes les étiquettes depuis appconfig vers appconfig</span><span class="sxs-lookup"><span data-stu-id="69d51-839">Support import/export of all labels from appconfig to appconfig</span></span>
* <span data-ttu-id="69d51-840">Validation des noms de clés et de fonctionnalités avant la définition et l’importation</span><span class="sxs-lookup"><span data-stu-id="69d51-840">Validate key and feature names before setting and importing</span></span>
* <span data-ttu-id="69d51-841">Exposition du changement de référence SKU pour le magasin de configurations.</span><span class="sxs-lookup"><span data-stu-id="69d51-841">Expose sku modification for configuration store.</span></span>
* <span data-ttu-id="69d51-842">Ajout d’un groupe de commandes pour l’identité managée.</span><span class="sxs-lookup"><span data-stu-id="69d51-842">Add command group for managed identity.</span></span>

### <a name="appservice"></a><span data-ttu-id="69d51-843">AppService</span><span class="sxs-lookup"><span data-stu-id="69d51-843">AppService</span></span>

* <span data-ttu-id="69d51-844">Azure Stack : commandes de surface sous le profil de 2019-03-01-hybrid</span><span class="sxs-lookup"><span data-stu-id="69d51-844">Azure Stack: surface commands under the profile of 2019-03-01-hybrid</span></span>
* <span data-ttu-id="69d51-845">functionapp : Ajout de la possibilité de créer des applications de fonction Java sur Linux</span><span class="sxs-lookup"><span data-stu-id="69d51-845">functionapp: Add ability to create Java function apps in Linux</span></span>

### <a name="arm"></a><span data-ttu-id="69d51-846">ARM</span><span class="sxs-lookup"><span data-stu-id="69d51-846">ARM</span></span>

* <span data-ttu-id="69d51-847">Résolution du problème #10246 : `az resource tag` plante quand le paramètre `--ids` transmis est un ID de groupe de ressources</span><span class="sxs-lookup"><span data-stu-id="69d51-847">Fix issue #10246: `az resource tag` crashes when the parameter `--ids` passed in is resource group ID</span></span>
* <span data-ttu-id="69d51-848">Résolution du problème #11658 : La commande `az group export` ne prend pas en charge les paramètres `--query` et `--output`</span><span class="sxs-lookup"><span data-stu-id="69d51-848">Fix issue #11658: `az group export` command does not support `--query` and `--output` parameters</span></span>
* <span data-ttu-id="69d51-849">Correction du problème #10279 : Le code de sortie de `az group deployment validate` est 0 en cas d’échec de la vérification</span><span class="sxs-lookup"><span data-stu-id="69d51-849">Fix issue #10279: The exit code of `az group deployment validate` is 0 when the verification fails</span></span>
* <span data-ttu-id="69d51-850">Correction du problème #9916 : Amélioration du message d’erreur du conflit entre l’étiquette et les autres conditions de filtre pour la commande `az resource list`</span><span class="sxs-lookup"><span data-stu-id="69d51-850">Fix issue #9916: Improve the error message of the conflict between tag and other filter conditions for `az resource list` command</span></span>
* <span data-ttu-id="69d51-851">Ajout du nouveau paramètre `--managed-by` pour prendre en charge l’ajout d’informations managedBy pour la commande `az group create`</span><span class="sxs-lookup"><span data-stu-id="69d51-851">Add new parameter `--managed-by` to support adding managedBy information for command `az group create`</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="69d51-852">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="69d51-852">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="69d51-853">Ajout du sous-groupe `monitor` pour gérer la supervision Log Analytics dans le cluster Azure Red Hat OpensShift</span><span class="sxs-lookup"><span data-stu-id="69d51-853">Add `monitor` subgroup to manage Log Analytics monitoring in Azure Red Hat OpensShift cluster</span></span>

### <a name="botservice"></a><span data-ttu-id="69d51-854">BotService</span><span class="sxs-lookup"><span data-stu-id="69d51-854">BotService</span></span>

* <span data-ttu-id="69d51-855">Résolution du problème #11697 : `az bot create` n’est pas idempotent</span><span class="sxs-lookup"><span data-stu-id="69d51-855">Fix issue #11697: `az bot create` is not idempotent</span></span>
* <span data-ttu-id="69d51-856">Changement des tests de correction de nom à exécuter en mode réel uniquement</span><span class="sxs-lookup"><span data-stu-id="69d51-856">Change name-correcting tests to run in Live-mode only</span></span>

### <a name="cdn"></a><span data-ttu-id="69d51-857">CDN</span><span class="sxs-lookup"><span data-stu-id="69d51-857">CDN</span></span>

* <span data-ttu-id="69d51-858">Ajout de la prise en charge de la fonctionnalité rulesEngine</span><span class="sxs-lookup"><span data-stu-id="69d51-858">Add support for rulesEngine feature</span></span>
* <span data-ttu-id="69d51-859">Ajout d’un nouveau groupe de commandes 'cdn endpoint rule' pour gérer les règles</span><span class="sxs-lookup"><span data-stu-id="69d51-859">Add new commands group 'cdn endpoint rule' to manage rules</span></span>
* <span data-ttu-id="69d51-860">Mise à jour de la version azure-mgmt-cdn vers la version 4.0.0 pour utiliser la version d’API 2019-04-15</span><span class="sxs-lookup"><span data-stu-id="69d51-860">Update azure-mgmt-cdn version to 4.0.0 to use api version 2019-04-15</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="69d51-861">Deployment Manager</span><span class="sxs-lookup"><span data-stu-id="69d51-861">Deployment Manager</span></span>

* <span data-ttu-id="69d51-862">Ajout d’une opération de liste pour toutes les ressources.</span><span class="sxs-lookup"><span data-stu-id="69d51-862">Add list operation for all resources.</span></span>
* <span data-ttu-id="69d51-863">Amélioration de la ressource d’étape pour le nouveau type d’étape.</span><span class="sxs-lookup"><span data-stu-id="69d51-863">Enhance step resource for new step type.</span></span>
* <span data-ttu-id="69d51-864">Mise à jour du package azure-mgmt-deploymentmanager pour utiliser la version 0.2.0.</span><span class="sxs-lookup"><span data-stu-id="69d51-864">Update azure-mgmt-deploymentmanager package to use version 0.2.0.</span></span>

### <a name="iot"></a><span data-ttu-id="69d51-865">IoT</span><span class="sxs-lookup"><span data-stu-id="69d51-865">IoT</span></span>

* <span data-ttu-id="69d51-866">Dépréciation des commandes 'IoT hub Job'.</span><span class="sxs-lookup"><span data-stu-id="69d51-866">Deprecate 'IoT hub Job' commands.</span></span>

### <a name="iot-central"></a><span data-ttu-id="69d51-867">IoT Central</span><span class="sxs-lookup"><span data-stu-id="69d51-867">IoT Central</span></span>

* <span data-ttu-id="69d51-868">Prise en charge de la création/mise à jour d’applications avec le nouveau nom de référence SKU ST0, ST1, ST2.</span><span class="sxs-lookup"><span data-stu-id="69d51-868">Support app creation/update with the new sku name ST0, ST1, ST2.</span></span>

### <a name="key-vault"></a><span data-ttu-id="69d51-869">Key Vault</span><span class="sxs-lookup"><span data-stu-id="69d51-869">Key Vault</span></span>

* <span data-ttu-id="69d51-870">Ajout de la nouvelle commande `az keyvault key download` pour télécharger des clés.</span><span class="sxs-lookup"><span data-stu-id="69d51-870">Add a new command `az keyvault key download` for downloading keys.</span></span>

### <a name="misc"></a><span data-ttu-id="69d51-871">Divers</span><span class="sxs-lookup"><span data-stu-id="69d51-871">Misc</span></span>

* <span data-ttu-id="69d51-872">Correctif #6371 : Prise en charge de la complétion du nom de fichier et de la variable d’environnement dans Bash</span><span class="sxs-lookup"><span data-stu-id="69d51-872">Fix #6371: Support filename and environment variable completion in Bash</span></span>

### <a name="network"></a><span data-ttu-id="69d51-873">Réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-873">Network</span></span>

* <span data-ttu-id="69d51-874">Correctif #2092 : avertissement az network dns record-set add/remove: add quand l’ensemble d’enregistrements est introuvable.</span><span class="sxs-lookup"><span data-stu-id="69d51-874">Fix #2092: az network dns record-set add/remove: add warning when record-set is not found.</span></span> <span data-ttu-id="69d51-875">À l’avenir, un argument supplémentaire sera pris en charge pour confirmer cette création automatique.</span><span class="sxs-lookup"><span data-stu-id="69d51-875">In the future, an extra argument will be supported to confirm this auto creation.</span></span>

### <a name="policy"></a><span data-ttu-id="69d51-876">Policy</span><span class="sxs-lookup"><span data-stu-id="69d51-876">Policy</span></span>

* <span data-ttu-id="69d51-877">Ajout de la nouvelle commande `az policy metadata` pour récupérer des ressources de métadonnées de stratégie riches</span><span class="sxs-lookup"><span data-stu-id="69d51-877">Add new command `az policy metadata` to retrieve rich policy metadata resources</span></span>
* <span data-ttu-id="69d51-878">`az policy remediation create`: Indication si la conformité doit être réévaluée avant correction avec le paramètre `--resource-discovery-mode`</span><span class="sxs-lookup"><span data-stu-id="69d51-878">`az policy remediation create`: Specify whether compliance should be re-evaluated prior to remediation with the `--resource-discovery-mode` parameter</span></span>

### <a name="profile"></a><span data-ttu-id="69d51-879">Profil</span><span class="sxs-lookup"><span data-stu-id="69d51-879">Profile</span></span>

* <span data-ttu-id="69d51-880">`az account get-access-token`: Ajout du paramètre `--tenant` pour acquérir directement un jeton pour le locataire, sans avoir à spécifier un abonnement</span><span class="sxs-lookup"><span data-stu-id="69d51-880">`az account get-access-token`: Add `--tenant` parameter to acquire token for the tenant directly, needless to specify a subscription</span></span>

### <a name="rbac"></a><span data-ttu-id="69d51-881">RBAC</span><span class="sxs-lookup"><span data-stu-id="69d51-881">RBAC</span></span>

* <span data-ttu-id="69d51-882">[CHANGEMENT CASSANT] Correctif #11883 : `az role assignment create` : une étendue vide entraîne une erreur</span><span class="sxs-lookup"><span data-stu-id="69d51-882">[BREAKING CHANGE] Fix #11883: `az role assignment create`: empty scope will prompt error</span></span>

### <a name="security"></a><span data-ttu-id="69d51-883">Sécurité</span><span class="sxs-lookup"><span data-stu-id="69d51-883">Security</span></span>

* <span data-ttu-id="69d51-884">Ajout des nouvelles commandes `az atp show` et `az atp update` pour voir et gérer les paramètres de protection avancée contre les menaces pour les comptes de stockage.</span><span class="sxs-lookup"><span data-stu-id="69d51-884">Add new commands `az atp show` and `az atp update` to view and manage advanced threat protection settings for storage accounts.</span></span>

### <a name="sql"></a><span data-ttu-id="69d51-885">SQL</span><span class="sxs-lookup"><span data-stu-id="69d51-885">SQL</span></span>

* <span data-ttu-id="69d51-886">`sql dw create` : dépréciation des paramètres `--zone-redundant` et `--read-replica-count`.</span><span class="sxs-lookup"><span data-stu-id="69d51-886">`sql dw create`: deprecate `--zone-redundant` and `--read-replica-count` parameters.</span></span> <span data-ttu-id="69d51-887">Ces paramètres ne s’appliquent pas à DataWarehouse.</span><span class="sxs-lookup"><span data-stu-id="69d51-887">These parameters do not apply to DataWarehouse.</span></span>
* <span data-ttu-id="69d51-888">[CHANGEMENT CASSANT] `az sql db create` : Suppression de « WideWorldImportersStd » et « WideWorldImportersFull » comme valeurs autorisées documentées pour "az sql db create --sample-name".</span><span class="sxs-lookup"><span data-stu-id="69d51-888">[BREAKING CHANGE] `az sql db create`: Remove "WideWorldImportersStd" and "WideWorldImportersFull" as documented allowed values for "az sql db create --sample-name".</span></span> <span data-ttu-id="69d51-889">Ces exemples de bases de données entraînaient systématiquement l’échec de la création.</span><span class="sxs-lookup"><span data-stu-id="69d51-889">These sample databases would always cause creation to fail.</span></span>
* <span data-ttu-id="69d51-890">Ajout des nouvelles commandes `sql db classification show/list/update/delete` et `sql db classification recommendation list/enable/disable` afin de gérer les classifications de sensibilité pour les bases de données SQL.</span><span class="sxs-lookup"><span data-stu-id="69d51-890">Add New commands `sql db classification show/list/update/delete` and `sql db classification recommendation list/enable/disable` to manage sensitivity classifications for SQL databases.</span></span>
* <span data-ttu-id="69d51-891">`az sql db audit-policy`: Correction pour les groupes et actions d’audit vides</span><span class="sxs-lookup"><span data-stu-id="69d51-891">`az sql db audit-policy`: Fix for empty audit actions and groups</span></span>

### <a name="storage"></a><span data-ttu-id="69d51-892">Stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-892">Storage</span></span>

* <span data-ttu-id="69d51-893">Ajout du nouveau groupe de commandes `az storage share-rm` afin d’utiliser le fournisseur de ressources Microsoft.Storage pour les opérations de gestion de partage de fichiers Azure.</span><span class="sxs-lookup"><span data-stu-id="69d51-893">Add a new command group `az storage share-rm` to use the Microsoft.Storage resource provider for Azure file share management operations.</span></span>
* <span data-ttu-id="69d51-894">Correction du problème #11415 : erreur d’autorisation pour `az storage blob update`</span><span class="sxs-lookup"><span data-stu-id="69d51-894">Fix issue #11415: permission error for `az storage blob update`</span></span>
* <span data-ttu-id="69d51-895">Intégration d’Azcopy 10.3.3 et prise en charge de Win32.</span><span class="sxs-lookup"><span data-stu-id="69d51-895">Integrate Azcopy 10.3.3 and support Win32.</span></span>
* <span data-ttu-id="69d51-896">`az storage copy`: Ajout des paramètres `--include-path`, `--include-pattern`, `--exclude-path` et `--exclude-pattern`</span><span class="sxs-lookup"><span data-stu-id="69d51-896">`az storage copy`: Add `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="69d51-897">`az storage remove`: Remplacement des paramètres `--inlcude` et `--exclude` par les paramètres `--include-path`, `--include-pattern`, `--exclude-path` et `--exclude-pattern`</span><span class="sxs-lookup"><span data-stu-id="69d51-897">`az storage remove`: Change `--inlcude` and `--exclude` parameters to `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="69d51-898">`az storage sync`: Ajout des paramètres `--include-pattern`, `--exclude-path` et `--exclude-pattern`</span><span class="sxs-lookup"><span data-stu-id="69d51-898">`az storage sync`: Add `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>

### <a name="servicefabric"></a><span data-ttu-id="69d51-899">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="69d51-899">ServiceFabric</span></span>

* <span data-ttu-id="69d51-900">Ajout de nouvelles commandes pour gérer les applications et les services.</span><span class="sxs-lookup"><span data-stu-id="69d51-900">Add new commands to manage appliaction and services.</span></span>

## <a name="january-13-2020"></a><span data-ttu-id="69d51-901">13 janvier 2020</span><span class="sxs-lookup"><span data-stu-id="69d51-901">January 13, 2020</span></span>

<span data-ttu-id="69d51-902">Version 2.0.80</span><span class="sxs-lookup"><span data-stu-id="69d51-902">Version 2.0.80</span></span>

### <a name="compute"></a><span data-ttu-id="69d51-903">Calcul</span><span class="sxs-lookup"><span data-stu-id="69d51-903">Compute</span></span>

* <span data-ttu-id="69d51-904">mise à jour de disque : Ajout de --disk-encryption-set et de --encryption-type</span><span class="sxs-lookup"><span data-stu-id="69d51-904">disk update: Add --disk-encryption-set and --encryption-type</span></span>
* <span data-ttu-id="69d51-905">création/mise à jour d’instantanés : Ajout de --disk-encryption-set et de --encryption-type</span><span class="sxs-lookup"><span data-stu-id="69d51-905">snapshot create/update: Add --disk-encryption-set and --encryption-type</span></span>

### <a name="storage"></a><span data-ttu-id="69d51-906">Stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-906">Storage</span></span>

* <span data-ttu-id="69d51-907">Mise à niveau de la version azure-mgmt-storage vers 7.1.0</span><span class="sxs-lookup"><span data-stu-id="69d51-907">Upgrade azure-mgmt-storage version to 7.1.0</span></span>
* <span data-ttu-id="69d51-908">`az storage account create`: Ajout de `--encryption-key-type-for-table` et de `--encryption-key-type-for-queue` pour prendre en charge le service de chiffrement de table et de file d’attente</span><span class="sxs-lookup"><span data-stu-id="69d51-908">`az storage account create`: Add `--encryption-key-type-for-table` and `--encryption-key-type-for-queue` to support Table and Queue Encryption Service</span></span>

## <a name="january-07-2020"></a><span data-ttu-id="69d51-909">7 janvier 2020</span><span class="sxs-lookup"><span data-stu-id="69d51-909">January 07, 2020</span></span>

<span data-ttu-id="69d51-910">Version 2.0.79</span><span class="sxs-lookup"><span data-stu-id="69d51-910">Version 2.0.79</span></span>

### <a name="acr"></a><span data-ttu-id="69d51-911">ACR</span><span class="sxs-lookup"><span data-stu-id="69d51-911">ACR</span></span>

* <span data-ttu-id="69d51-912">[CHANGEMENT CASSANT] Suppression du paramètre « --os » pour « acr build », « acr task create/update », « acr run » et « acr pack ».</span><span class="sxs-lookup"><span data-stu-id="69d51-912">[BREAKING CHANGE] Remove '--os' parameter for 'acr build', 'acr task create/update', 'acr run', and 'acr pack'.</span></span> <span data-ttu-id="69d51-913">Utilisez « --platform » à la place.</span><span class="sxs-lookup"><span data-stu-id="69d51-913">Use '--platform' instead.</span></span>

### <a name="appconfig"></a><span data-ttu-id="69d51-914">AppConfig</span><span class="sxs-lookup"><span data-stu-id="69d51-914">AppConfig</span></span>

* <span data-ttu-id="69d51-915">Ajout de la prise en charge de l’importation/exportation des indicateurs de fonctionnalité</span><span class="sxs-lookup"><span data-stu-id="69d51-915">Add support for importing/exporting feature flags</span></span>
* <span data-ttu-id="69d51-916">Ajout de la nouvelle commande « az appconfig kv set-keyvault » pour la création d’une référence KeyVault</span><span class="sxs-lookup"><span data-stu-id="69d51-916">Add new command 'az appconfig kv set-keyvault' for creating keyvault reference</span></span>
* <span data-ttu-id="69d51-917">Prise en charge de différentes conventions de nommage lors de l’exportation d’indicateurs de fonctionnalité dans un fichier</span><span class="sxs-lookup"><span data-stu-id="69d51-917">Support various naming conventions when exporting feature flags to file</span></span>

### <a name="appservice"></a><span data-ttu-id="69d51-918">AppService</span><span class="sxs-lookup"><span data-stu-id="69d51-918">AppService</span></span>

* <span data-ttu-id="69d51-919">Résolution du problème #7154 : Mise à jour de la documentation pour la commande <> afin d’utiliser des accents graves (backtick) plutôt que des guillemets simples</span><span class="sxs-lookup"><span data-stu-id="69d51-919">Fix issue #7154: Updating documentation for command <> to use back ticks instead of single quotes</span></span>
* <span data-ttu-id="69d51-920">Résolution du problème #11287 : webapp up : Faire en sorte que l’application créée à l’aide de « up » ait « SSL activé » par défaut</span><span class="sxs-lookup"><span data-stu-id="69d51-920">Fix issue #11287: webapp up: By default make the app created using up 'should be 'SSL enabled'</span></span>
* <span data-ttu-id="69d51-921">Résolution du problème #11592 : Ajout de la commande az webapp up flag pour les sites statiques HTML</span><span class="sxs-lookup"><span data-stu-id="69d51-921">Fix issue #11592: Add az webapp up flag for html static sites</span></span>

### <a name="arm"></a><span data-ttu-id="69d51-922">ARM</span><span class="sxs-lookup"><span data-stu-id="69d51-922">ARM</span></span>

* <span data-ttu-id="69d51-923">Correction de `az resource tag` : Impossible de mettre à jour les balises du coffre Recovery Services</span><span class="sxs-lookup"><span data-stu-id="69d51-923">Fix `az resource tag`: Recovery Services Vault tags cannot be updated</span></span>

### <a name="backup"></a><span data-ttu-id="69d51-924">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="69d51-924">Backup</span></span>

* <span data-ttu-id="69d51-925">Ajout de la nouvelle commande « backup protection undelete » pour activer la fonctionnalité de suppression réversible pour la charge de travail IaasVM</span><span class="sxs-lookup"><span data-stu-id="69d51-925">Added new command 'backup protection undelete' to enable soft-delete feature for IaasVM workload</span></span>
* <span data-ttu-id="69d51-926">Ajout du nouveau paramètre « --soft-delete-feature-state » pour définir la commande backup-properties</span><span class="sxs-lookup"><span data-stu-id="69d51-926">Added new parameter '--soft-delete-feature-state' to set backup-properties command</span></span>
* <span data-ttu-id="69d51-927">Ajout de la prise en charge de l’exclusion de disque pour la charge de travail IaasVM</span><span class="sxs-lookup"><span data-stu-id="69d51-927">Added disk exclusion support for IaasVM workload</span></span>

### <a name="compute"></a><span data-ttu-id="69d51-928">Calcul</span><span class="sxs-lookup"><span data-stu-id="69d51-928">Compute</span></span>

* <span data-ttu-id="69d51-929">Résolution de l’échec de `vm create` dans le profil Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="69d51-929">Fix `vm create` failure in Azure Stack profile.</span></span>
* <span data-ttu-id="69d51-930">vm monitor metrics tail/list-definitions : prise en charge des définitions de métriques et de listes pour une machine virtuelle.</span><span class="sxs-lookup"><span data-stu-id="69d51-930">vm monitor metrics tail/list-definitions: support query metric and list definitions for a vm.</span></span>
* <span data-ttu-id="69d51-931">Ajout d’une nouvelle action de réapplication de commande pour az vm</span><span class="sxs-lookup"><span data-stu-id="69d51-931">Add new reapply command action for az vm</span></span>

### <a name="hdinsight"></a><span data-ttu-id="69d51-932">HDInsight</span><span class="sxs-lookup"><span data-stu-id="69d51-932">HDInsight</span></span>

* <span data-ttu-id="69d51-933">Prise en charge de la création d’un cluster Kafka avec le proxy Rest Kafka</span><span class="sxs-lookup"><span data-stu-id="69d51-933">Support for creating a Kafka cluster with Kafka Rest Proxy</span></span>
* <span data-ttu-id="69d51-934">Mise à niveau d’azure-mgmt-hdinsight vers 1.3.0</span><span class="sxs-lookup"><span data-stu-id="69d51-934">Upgrade azure-mgmt-hdinsight to 1.3.0</span></span>

### <a name="misc"></a><span data-ttu-id="69d51-935">Divers</span><span class="sxs-lookup"><span data-stu-id="69d51-935">Misc.</span></span>

* <span data-ttu-id="69d51-936">Ajout de la commande d’aperçu `az version show` pour afficher les versions des modules et extensions Azure CLI au format JSON par défaut ou au format configuré par --output</span><span class="sxs-lookup"><span data-stu-id="69d51-936">Add preview command `az version show` to show the versions of Azure CLI modules and extensions in JSON format by default or format configured by --output</span></span>

### <a name="event-hubs"></a><span data-ttu-id="69d51-937">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="69d51-937">Event Hubs</span></span>

* <span data-ttu-id="69d51-938">[CHANGEMENT CASSANT] Suppression de l’option d’état « ReceiveDisabled » des commandes « az eventhubs eventhub update » et « az eventhubs eventhub create ».</span><span class="sxs-lookup"><span data-stu-id="69d51-938">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az eventhubs eventhub update' and 'az eventhubs eventhub create'.</span></span> <span data-ttu-id="69d51-939">Cette option n’est pas valide pour les entités Event Hub.</span><span class="sxs-lookup"><span data-stu-id="69d51-939">This option is not valid for Event Hub entities.</span></span>

### <a name="service-bus"></a><span data-ttu-id="69d51-940">Service Bus</span><span class="sxs-lookup"><span data-stu-id="69d51-940">Service Bus</span></span>

* <span data-ttu-id="69d51-941">[CHANGEMENT CASSANT] Suppression de l’option d’état « ReceiveDisabled » des commandes « az servicebus topic create », « az servicebus topic update », « az servicebus queue create » et « az servicebus queue update ».</span><span class="sxs-lookup"><span data-stu-id="69d51-941">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az servicebus topic create', 'az servicebus topic update', 'az servicebus queue create', and 'az servicebus queue update'.</span></span> <span data-ttu-id="69d51-942">Cette option n’est pas valide pour les rubriques et files d’attente Service Bus.</span><span class="sxs-lookup"><span data-stu-id="69d51-942">This option is not valid for Service Bus topics and queues.</span></span>

### <a name="rbac"></a><span data-ttu-id="69d51-943">RBAC</span><span class="sxs-lookup"><span data-stu-id="69d51-943">RBAC</span></span>

* <span data-ttu-id="69d51-944">Correctif 11712 : `az ad app/sp show` ne retourne pas le code de sortie 3 quand le principal d’application ou de service n’existe pas</span><span class="sxs-lookup"><span data-stu-id="69d51-944">Fix #11712: `az ad app/sp show` does not return exit code 3 when the application or service principal does not exist</span></span>

### <a name="storage"></a><span data-ttu-id="69d51-945">Stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-945">Storage</span></span>

* <span data-ttu-id="69d51-946">`az storage account create`: Suppression de l’indicateur d’aperçu pour le paramètre --enable-hierarchical-namespace</span><span class="sxs-lookup"><span data-stu-id="69d51-946">`az storage account create`: Remove preview flag for --enable-hierarchical-namespace parameter</span></span>
* <span data-ttu-id="69d51-947">Mise à jour de la version d’azure-mgmt-storage vers la version 7.0.0 pour utiliser la version d’API du 01/06/2019</span><span class="sxs-lookup"><span data-stu-id="69d51-947">Update azure-mgmt-storage version to 7.0.0 to use api version 2019-06-01</span></span>
* <span data-ttu-id="69d51-948">Ajout des nouveaux paramètres `--enable-delete-retention` et `--delete-retention-days` afin de prendre en charge la gestion de la stratégie de conservation de suppression pour les propriétés blob-service du compte de stockage.</span><span class="sxs-lookup"><span data-stu-id="69d51-948">Add new parameters `--enable-delete-retention` and `--delete-retention-days` to support managing delete retention policy for storage account blob-service-properties.</span></span>

## <a name="december-17-2019"></a><span data-ttu-id="69d51-949">17 décembre 2019</span><span class="sxs-lookup"><span data-stu-id="69d51-949">December 17, 2019</span></span>

<span data-ttu-id="69d51-950">2.0.78</span><span class="sxs-lookup"><span data-stu-id="69d51-950">2.0.78</span></span>

### <a name="acr"></a><span data-ttu-id="69d51-951">ACR</span><span class="sxs-lookup"><span data-stu-id="69d51-951">ACR</span></span>

* <span data-ttu-id="69d51-952">Ajout de la prise en charge du contexte local dans acr task run</span><span class="sxs-lookup"><span data-stu-id="69d51-952">Added support Local context in acr task run</span></span>

### <a name="acs"></a><span data-ttu-id="69d51-953">ACS</span><span class="sxs-lookup"><span data-stu-id="69d51-953">ACS</span></span>

* <span data-ttu-id="69d51-954">[CHANGEMENT CASSANT]az openshift create : renommage de `--workspace-resource-id` en `--workspace-id`.</span><span class="sxs-lookup"><span data-stu-id="69d51-954">[BREAKING CHANGE]az openshift create: rename `--workspace-resource-id` to `--workspace-id`.</span></span>

### <a name="ams"></a><span data-ttu-id="69d51-955">AMS</span><span class="sxs-lookup"><span data-stu-id="69d51-955">AMS</span></span>

* <span data-ttu-id="69d51-956">Mise à jour des commandes show pour retourner 3 quand la ressource est introuvable</span><span class="sxs-lookup"><span data-stu-id="69d51-956">Updated show commands to return 3 when resource not found</span></span>

### <a name="appconfig"></a><span data-ttu-id="69d51-957">AppConfig</span><span class="sxs-lookup"><span data-stu-id="69d51-957">AppConfig</span></span>

* <span data-ttu-id="69d51-958">Correction d’un bogue lié à l’ajout de la version d’API à l’URL de demande.</span><span class="sxs-lookup"><span data-stu-id="69d51-958">Fixed bug when appending api-version to request url.</span></span> <span data-ttu-id="69d51-959">La solution existante ne fonctionne pas avec la pagination.</span><span class="sxs-lookup"><span data-stu-id="69d51-959">The existing solution doesn't work with pagination.</span></span>
* <span data-ttu-id="69d51-960">Ajout de la prise en charge de l’affichage des langues en plus de l’anglais comme notre Unicode de support du service back-end pour la globalisation.</span><span class="sxs-lookup"><span data-stu-id="69d51-960">Added support for showing languages besides English as our backend service support unicode for globalization.</span></span>

### <a name="appservice"></a><span data-ttu-id="69d51-961">AppService</span><span class="sxs-lookup"><span data-stu-id="69d51-961">AppService</span></span>

* <span data-ttu-id="69d51-962">Résolution du problème #11217 : webapp : az webapp config ssl upload doit prendre en charge le paramètre d’emplacement (slot)</span><span class="sxs-lookup"><span data-stu-id="69d51-962">Fixed issue #11217: webapp: az webapp config ssl upload should support slot parameter</span></span>
* <span data-ttu-id="69d51-963">Résolution du problème #10965 : Erreur : Le nom n'est pas vide.</span><span class="sxs-lookup"><span data-stu-id="69d51-963">Fixed issue #10965: Error: Name cannot be empty.</span></span> <span data-ttu-id="69d51-964">Autoriser la suppression par adresse IP (ip_address) et sous-réseau (subnet)</span><span class="sxs-lookup"><span data-stu-id="69d51-964">Allow remove by ip_address and subnet</span></span>
* <span data-ttu-id="69d51-965">Ajout de la prise en charge de l’importation de certificats à partir du coffre de clés `az webapp config ssl import`</span><span class="sxs-lookup"><span data-stu-id="69d51-965">Added support for importing certificates from Key Vault `az webapp config ssl import`</span></span>

### <a name="arm"></a><span data-ttu-id="69d51-966">ARM</span><span class="sxs-lookup"><span data-stu-id="69d51-966">ARM</span></span>

* <span data-ttu-id="69d51-967">Mise à jour du package azure-mgmt-resource pour utiliser la version 6.0.0</span><span class="sxs-lookup"><span data-stu-id="69d51-967">Updated azure-mgmt-resource package to use 6.0.0</span></span>
* <span data-ttu-id="69d51-968">Prise en charge interlocataire pour la commande `az group deployment create` en ajoutant le nouveau paramètre `--aux-subs`</span><span class="sxs-lookup"><span data-stu-id="69d51-968">Cross Tenant Support for `az group deployment create` command by adding new parameter `--aux-subs`</span></span>
* <span data-ttu-id="69d51-969">Ajout du nouveau paramètre `--metadata` afin de prendre en charge l’ajout d’informations de métadonnées pour les définitions d’ensemble de stratégie.</span><span class="sxs-lookup"><span data-stu-id="69d51-969">Added new parameter `--metadata` to support adding metadata information for policy set definitions.</span></span>

### <a name="backup"></a><span data-ttu-id="69d51-970">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="69d51-970">Backup</span></span>

* <span data-ttu-id="69d51-971">Ajout de la prise en charge de la sauvegarde pour la charge de travail SQL et SAP Hana.</span><span class="sxs-lookup"><span data-stu-id="69d51-971">Added Backup support for SQL and SAP Hana workload.</span></span>

### <a name="botservice"></a><span data-ttu-id="69d51-972">BotService</span><span class="sxs-lookup"><span data-stu-id="69d51-972">BotService</span></span>

* <span data-ttu-id="69d51-973">[Changement cassant] Suppression de l’indicateur « --version » de la commande d’aperçu « az bot create ».</span><span class="sxs-lookup"><span data-stu-id="69d51-973">[Breaking change] Remove '--version' flag from preview command 'az bot create'.</span></span> <span data-ttu-id="69d51-974">Seuls les bots du SDK v4 sont pris en charge.</span><span class="sxs-lookup"><span data-stu-id="69d51-974">Only v4 SDK bots are supported.</span></span>
* <span data-ttu-id="69d51-975">Ajout de la vérification de la disponibilité du nom pour « az bot create ».</span><span class="sxs-lookup"><span data-stu-id="69d51-975">Added name availability check for 'az bot create'.</span></span>
* <span data-ttu-id="69d51-976">Ajout de la prise en charge de la mise à jour de l’URL d’icône pour un bot par le biais de « az bot update ».</span><span class="sxs-lookup"><span data-stu-id="69d51-976">Added support for updating the icon URL for a bot via 'az bot update'.</span></span>
* <span data-ttu-id="69d51-977">Ajout de la prise en charge de la mise à jour d’un canal Direct Line par le biais de « az bot directline update ».</span><span class="sxs-lookup"><span data-stu-id="69d51-977">Added support for updating a Direct Line channel via 'az bot directline update'.</span></span>
* <span data-ttu-id="69d51-978">Ajout de la prise en charge de l’indicateur « --enable-enhanced-auth » à « az bot directline create ».</span><span class="sxs-lookup"><span data-stu-id="69d51-978">Added '--enable-enhanced-auth' flag support to 'az bot directline create'.</span></span>
* <span data-ttu-id="69d51-979">Les groupes de commandes suivants sont en disponibilité générale et non en préversion : « az bot authsetting ».</span><span class="sxs-lookup"><span data-stu-id="69d51-979">The following command groups are GA and not in preview: 'az bot authsetting'.</span></span>
* <span data-ttu-id="69d51-980">Les commandes suivantes dans « az bot » sont en disponibilité générale et non en préversion : « create », « prepare-deploy », « show », « delete », « update ».</span><span class="sxs-lookup"><span data-stu-id="69d51-980">The following commands in 'az bot' are GA and not in preview: 'create', 'prepare-deploy', 'show', 'delete', 'update'.</span></span>
* <span data-ttu-id="69d51-981">Résolution du problème lié au fait que « az bot prepare-deploy » convertit la valeur « --proj-file-path » en minuscules (par exemple, « Test.csproj » en « test.csproj »).</span><span class="sxs-lookup"><span data-stu-id="69d51-981">Fixed 'az bot prepare-deploy' changing '--proj-file-path' value to lower case (e.g. "Test.csproj" to "test.csproj").</span></span>

### <a name="compute"></a><span data-ttu-id="69d51-982">Calcul</span><span class="sxs-lookup"><span data-stu-id="69d51-982">Compute</span></span>

* <span data-ttu-id="69d51-983">vmss create/update : Ajout de --scale-in-policy, qui détermine quelles machines virtuelles sont choisies pour la suppression quand un groupe de machines virtuelles identiques (VMSS) fait l’objet d’un scale-in.</span><span class="sxs-lookup"><span data-stu-id="69d51-983">vmss create/update: Added --scale-in-policy, which decides which virtual machines are chosen for removal when a VMSS is scaled-in.</span></span>
* <span data-ttu-id="69d51-984">vm/vmss update : Ajout de --priority.</span><span class="sxs-lookup"><span data-stu-id="69d51-984">vm/vmss update: Added --priority.</span></span>
* <span data-ttu-id="69d51-985">vm/vmss update : Ajout de --max-price.</span><span class="sxs-lookup"><span data-stu-id="69d51-985">vm/vmss update: Added --max-price.</span></span>
* <span data-ttu-id="69d51-986">Ajout du groupe de commandes disk-encryption-set (create, show, update, delete, list).</span><span class="sxs-lookup"><span data-stu-id="69d51-986">Added disk-encryption-set command group (create, show, update, delete, list).</span></span>
* <span data-ttu-id="69d51-987">disk create : Ajout de --encryption-type et de --disk-encryption-set.</span><span class="sxs-lookup"><span data-stu-id="69d51-987">disk create: Added --encryption-type and --disk-encryption-set.</span></span>
* <span data-ttu-id="69d51-988">vm/vmss create : Ajout de --os-disk-encryption-set et de --data-disk-encryption-sets.</span><span class="sxs-lookup"><span data-stu-id="69d51-988">vm/vmss create: Added --os-disk-encryption-set and --data-disk-encryption-sets.</span></span>

### <a name="core"></a><span data-ttu-id="69d51-989">Core</span><span class="sxs-lookup"><span data-stu-id="69d51-989">Core</span></span>

* <span data-ttu-id="69d51-990">Suppression de la prise en charge pour Python 3.4</span><span class="sxs-lookup"><span data-stu-id="69d51-990">Removed support for Python 3.4</span></span>
* <span data-ttu-id="69d51-991">Intégrer l’enquête HaTS à plusieurs commandes</span><span class="sxs-lookup"><span data-stu-id="69d51-991">Plug in HaTS survey in multiple commands</span></span>

### <a name="dls"></a><span data-ttu-id="69d51-992">DLS</span><span class="sxs-lookup"><span data-stu-id="69d51-992">DLS</span></span>

* <span data-ttu-id="69d51-993">Mise à jour de la version du SDK ADLS (0.0.48).</span><span class="sxs-lookup"><span data-stu-id="69d51-993">Updated ADLS sdk version (0.0.48).</span></span>

### <a name="install"></a><span data-ttu-id="69d51-994">Installer</span><span class="sxs-lookup"><span data-stu-id="69d51-994">Install</span></span>

* <span data-ttu-id="69d51-995">Prise en charge du script d’installation pour Python 3.8</span><span class="sxs-lookup"><span data-stu-id="69d51-995">Install script support python 3.8</span></span>

### <a name="iot"></a><span data-ttu-id="69d51-996">IOT</span><span class="sxs-lookup"><span data-stu-id="69d51-996">IOT</span></span>

* <span data-ttu-id="69d51-997">[CHANGEMENT CASSANT] Suppression du paramètre --failover-region du basculement manuel.</span><span class="sxs-lookup"><span data-stu-id="69d51-997">[BREAKING CHANGE] Removed --failover-region parameter from manual-failover.</span></span> <span data-ttu-id="69d51-998">À présent, le basculement s’effectuera vers la région secondaire géographiquement associée.</span><span class="sxs-lookup"><span data-stu-id="69d51-998">Now it will failover to assigned geo-paired secondary region.</span></span>

### <a name="key-vault"></a><span data-ttu-id="69d51-999">Key Vault</span><span class="sxs-lookup"><span data-stu-id="69d51-999">Key Vault</span></span>

* <span data-ttu-id="69d51-1000">Résolution du problème #8095 : `az keyvault storage remove` : amélioration du message d’aide</span><span class="sxs-lookup"><span data-stu-id="69d51-1000">Fixed #8095: `az keyvault storage remove`: improve the help message</span></span>
* <span data-ttu-id="69d51-1001">Résolution du problème #8921 : `az keyvault key/secret/certificate list/list-deleted/list-versions` : correction du bogue de validation sur le paramètre `--maxresults`</span><span class="sxs-lookup"><span data-stu-id="69d51-1001">Fixed #8921: `az keyvault key/secret/certificate list/list-deleted/list-versions`: fix the validation bug on parameter `--maxresults`</span></span>
* <span data-ttu-id="69d51-1002">Résolution du problème #10512 : `az keyvault set-policy` : amélioration du message d’erreur quand aucune des valeurs `--object-id`, `--spn` ou `--upn` n’est spécifiée</span><span class="sxs-lookup"><span data-stu-id="69d51-1002">Fixed #10512: `az keyvault set-policy`: improve the error message when none of `--object-id`, `--spn` or `--upn` is specified</span></span>
* <span data-ttu-id="69d51-1003">Résolution du problème #10846 : `az keyvault secret show-deleted` : quand la valeur `--id` est spécifiée, `--name/-n` n’est pas nécessaire</span><span class="sxs-lookup"><span data-stu-id="69d51-1003">Fixed #10846: `az keyvault secret show-deleted`: when `--id` is specified, `--name/-n` is not required</span></span>
* <span data-ttu-id="69d51-1004">Résolution du problème #11084 : `az keyvault secret download` : amélioration du message d’aide du paramètre `--encoding`</span><span class="sxs-lookup"><span data-stu-id="69d51-1004">Fixed #11084: `az keyvault secret download`: improve the help message of parameter `--encoding`</span></span>

### <a name="network"></a><span data-ttu-id="69d51-1005">Réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-1005">Network</span></span>

* <span data-ttu-id="69d51-1006">az network application-gateway probe : Ajout de la prise en charge de l’option --port afin de spécifier un port pour la détection des serveurs back-end lors d’une opération de création et de mise à jour</span><span class="sxs-lookup"><span data-stu-id="69d51-1006">az network application-gateway probe: Added support --port option to specify a port for probing backend servers when create and update</span></span>
* <span data-ttu-id="69d51-1007">az network application-gateway url-path-map create/update : correction du bogue pour `--waf-policy`</span><span class="sxs-lookup"><span data-stu-id="69d51-1007">az network application-gateway url-path-map create/update: bug fix for `--waf-policy`</span></span>
* <span data-ttu-id="69d51-1008">az network application-gateway : Ajout de la prise en charge de `--rewrite-rule-set`</span><span class="sxs-lookup"><span data-stu-id="69d51-1008">az network application-gateway: Added support `--rewrite-rule-set`</span></span>
* <span data-ttu-id="69d51-1009">az network list-service-aliases : Ajout de la prise en charge du listage des alias de service qui peuvent être utilisés pour les stratégies de point de terminaison de service</span><span class="sxs-lookup"><span data-stu-id="69d51-1009">az network list-service-aliases: Added support list service aliases which can be used for Service Endpoint Policies</span></span>
* <span data-ttu-id="69d51-1010">az network dns zone import : Ajout de la prise en charge de .@ dans le nom des enregistrements</span><span class="sxs-lookup"><span data-stu-id="69d51-1010">az network dns zone import: Added support .@ in record name</span></span>

### <a name="packaging"></a><span data-ttu-id="69d51-1011">Packaging</span><span class="sxs-lookup"><span data-stu-id="69d51-1011">Packaging</span></span>

* <span data-ttu-id="69d51-1012">Rajout de builds edge pour pip install</span><span class="sxs-lookup"><span data-stu-id="69d51-1012">Added back edge builds for pip install</span></span>
* <span data-ttu-id="69d51-1013">Ajout du package Ubuntu eoan</span><span class="sxs-lookup"><span data-stu-id="69d51-1013">Added Ubuntu eoan package</span></span>

### <a name="policy"></a><span data-ttu-id="69d51-1014">Policy</span><span class="sxs-lookup"><span data-stu-id="69d51-1014">Policy</span></span>

* <span data-ttu-id="69d51-1015">Ajout de la prise en charge de l’API des stratégies version 2019-09-01.</span><span class="sxs-lookup"><span data-stu-id="69d51-1015">Added support for Policy API version 2019-09-01.</span></span>
* <span data-ttu-id="69d51-1016">az policy set-definition : Ajout de la prise en charge du regroupement dans les définitions d’ensemble de stratégies avec le paramètre `--definition-groups`</span><span class="sxs-lookup"><span data-stu-id="69d51-1016">az policy set-definition: Added support grouping within policy set definitions with `--definition-groups` parameter</span></span>

### <a name="redis"></a><span data-ttu-id="69d51-1017">Redis</span><span class="sxs-lookup"><span data-stu-id="69d51-1017">Redis</span></span>

* <span data-ttu-id="69d51-1018">Ajout du paramètre d’aperçu `--replicas-per-master` à la commande `az redis create`</span><span class="sxs-lookup"><span data-stu-id="69d51-1018">Added preview param `--replicas-per-master` to `az redis create` command</span></span>
* <span data-ttu-id="69d51-1019">Mise à jour d’azure-mgmt-redis version 6.0.0 vers la version 7.0.0 RC1</span><span class="sxs-lookup"><span data-stu-id="69d51-1019">Updated azure-mgmt-redis from 6.0.0 to 7.0.0rc1</span></span>

### <a name="servicefabric"></a><span data-ttu-id="69d51-1020">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="69d51-1020">ServiceFabric</span></span>

* <span data-ttu-id="69d51-1021">Correction du problème #10963 lié à la logique d’ajout de type de nœud : L’ajout d’un nouveau type de nœud avec le niveau de durabilité Gold générera toujours une erreur CLI</span><span class="sxs-lookup"><span data-stu-id="69d51-1021">Fixed in node-type add logic including #10963: Adding new node type with durability level Gold will always throw CLI error</span></span>
* <span data-ttu-id="69d51-1022">Mise à jour de la version de ServiceFabricNodeVmExt vers la version 1.1 dans le modèle de création</span><span class="sxs-lookup"><span data-stu-id="69d51-1022">Updated ServiceFabricNodeVmExt version to 1.1 in creation template</span></span>

### <a name="sql"></a><span data-ttu-id="69d51-1023">SQL</span><span class="sxs-lookup"><span data-stu-id="69d51-1023">SQL</span></span>

* <span data-ttu-id="69d51-1024">Ajout de paramètres « --read-scale » et « --read-replicas » aux commandes sql db create et sql db update pour prendre en charge la gestion de l’échelle lecture.</span><span class="sxs-lookup"><span data-stu-id="69d51-1024">Added "--read-scale" and "--read-replicas" parameters to sql db create and update commands, to support read scale management.</span></span>

### <a name="storage"></a><span data-ttu-id="69d51-1025">Stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-1025">Storage</span></span>

* <span data-ttu-id="69d51-1026">Propriété Partages de fichiers volumineux de la version en disponibilité générale pour les commandes storage account create et storage account update</span><span class="sxs-lookup"><span data-stu-id="69d51-1026">GA Release Large File Shares property for storage account create and update command</span></span>
* <span data-ttu-id="69d51-1027">Prise en charge des jetons SAS de délégation d’utilisateur de la version en disponibilité générale</span><span class="sxs-lookup"><span data-stu-id="69d51-1027">GA Release User Delegation SAS token Support</span></span>
* <span data-ttu-id="69d51-1028">Ajout des nouvelles commandes `az storage account blob-service-properties show` et `az storage account blob-service-properties update --enable-change-feed` afin de gérer les propriétés du service blob pour le compte de stockage.</span><span class="sxs-lookup"><span data-stu-id="69d51-1028">Added new commands `az storage account blob-service-properties show` and `az storage account blob-service-properties update --enable-change-feed` to manage blob service properties for storage account.</span></span>
* <span data-ttu-id="69d51-1029">[CHANGEMENT CASSANT À VENIR] `az storage copy` : le caractère `*` n’est plus pris en charge comme caractère générique dans l’URL, mais les nouveaux paramètres --include-pattern et --exclude-pattern seront ajoutés avec une prise en charge du caractère générique `*`.</span><span class="sxs-lookup"><span data-stu-id="69d51-1029">[COMING BREAKING CHANGE] `az storage copy`: `*` character is no longer supported as a wildcard in URL, but new parameters --include-pattern and --exclude-pattern will be added with `*` wildcard support.</span></span>
* <span data-ttu-id="69d51-1030">Résolution du problème #11043 : Ajout de la prise en charge de la suppression de l’intégralité du conteneur/partage dans la commande `az storage remove`</span><span class="sxs-lookup"><span data-stu-id="69d51-1030">Fixed issue #11043: Added support to remove whole container/share in `az storage remove` command</span></span>

## <a name="november-26-2019"></a><span data-ttu-id="69d51-1031">26 novembre 2019</span><span class="sxs-lookup"><span data-stu-id="69d51-1031">November 26, 2019</span></span>

<span data-ttu-id="69d51-1032">Version 2.0.77</span><span class="sxs-lookup"><span data-stu-id="69d51-1032">Version 2.0.77</span></span>

### <a name="acr"></a><span data-ttu-id="69d51-1033">ACR</span><span class="sxs-lookup"><span data-stu-id="69d51-1033">ACR</span></span>

* <span data-ttu-id="69d51-1034">Dépréciation du paramètre `--branch` dans acr task create/update</span><span class="sxs-lookup"><span data-stu-id="69d51-1034">Deprecated parameter `--branch` from acr task create/update</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="69d51-1035">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="69d51-1035">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="69d51-1036">Ajout de l’indicateur `--workspace-resource-id` pour permettre la création d’un cluster Azure Red Hat OpenShift avec supervision</span><span class="sxs-lookup"><span data-stu-id="69d51-1036">Added `--workspace-resource-id` flag to allow creation of Azure Red Hat Openshift cluster with monitoring</span></span>
* <span data-ttu-id="69d51-1037">Ajout de `monitor_profile` pour créer un cluster Azure Red Hat OpenShift avec supervision</span><span class="sxs-lookup"><span data-stu-id="69d51-1037">Added `monitor_profile` to create Azure Red Hat OpenShift cluster with monitoring</span></span>

### <a name="aks"></a><span data-ttu-id="69d51-1038">AKS</span><span class="sxs-lookup"><span data-stu-id="69d51-1038">AKS</span></span>

* <span data-ttu-id="69d51-1039">Ajout de la prise en charge de l’opération de rotation des certificats de cluster à l’aide de la commande « az aks rotate-certs ».</span><span class="sxs-lookup"><span data-stu-id="69d51-1039">Added support cluster certificate rotation operation using "az aks rotate-certs".</span></span>

### <a name="appconfig"></a><span data-ttu-id="69d51-1040">AppConfig</span><span class="sxs-lookup"><span data-stu-id="69d51-1040">AppConfig</span></span>

* <span data-ttu-id="69d51-1041">Ajout de la prise en charge de l’utilisation de « : » pour le séparateur `as az appconfig kv import`</span><span class="sxs-lookup"><span data-stu-id="69d51-1041">Added support for using ":" for `as az appconfig kv import` separator</span></span>
* <span data-ttu-id="69d51-1042">Résolution du problème de listage des valeurs de clés avec plusieurs étiquettes, y compris une étiquette Null.</span><span class="sxs-lookup"><span data-stu-id="69d51-1042">Fixed issue for listing key values with multiple labels including null label.</span></span> 
* <span data-ttu-id="69d51-1043">Mise à jour du SDK du plan de gestion, azure-mgmt-appconfiguration, vers la version 0.3.0.</span><span class="sxs-lookup"><span data-stu-id="69d51-1043">Updated management plane sdk, azure-mgmt-appconfiguration, to version 0.3.0.</span></span> 

### <a name="appservice"></a><span data-ttu-id="69d51-1044">AppService</span><span class="sxs-lookup"><span data-stu-id="69d51-1044">AppService</span></span>

* <span data-ttu-id="69d51-1045">Résolution du problème #11100 : Erreur d’attribut pour az webapp up lors de la création du plan de service</span><span class="sxs-lookup"><span data-stu-id="69d51-1045">Fixed issue #11100: AttributeError for az webapp up when create service plan</span></span>
* <span data-ttu-id="69d51-1046">az webapp up : En forçant la création ou le déploiement sur un site pour les langues prises en charge, aucune valeur par défaut n’est utilisée.</span><span class="sxs-lookup"><span data-stu-id="69d51-1046">az webapp up: Forcing the creation or deployment to a site for supported languages, no defaults used.</span></span>
* <span data-ttu-id="69d51-1047">Ajout de la prise en charge d’App Service Environment : az appservice ase show | list | list-addresses | list-plans | create | update | delete</span><span class="sxs-lookup"><span data-stu-id="69d51-1047">Added support for App Service Environment: az appservice ase show | list | list-addresses | list-plans | create | update | delete</span></span>

### <a name="backup"></a><span data-ttu-id="69d51-1048">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="69d51-1048">Backup</span></span>

* <span data-ttu-id="69d51-1049">Résolution du problème dans az backup policy list-associated-items.</span><span class="sxs-lookup"><span data-stu-id="69d51-1049">Fixed issue in az backup policy list-associated-items.</span></span> <span data-ttu-id="69d51-1050">Ajout du paramètre BackupManagementType facultatif.</span><span class="sxs-lookup"><span data-stu-id="69d51-1050">Added optional BackupManagementType parameter.</span></span>

### <a name="compute"></a><span data-ttu-id="69d51-1051">Calcul</span><span class="sxs-lookup"><span data-stu-id="69d51-1051">Compute</span></span>

* <span data-ttu-id="69d51-1052">Mise à jour de la version de l’API de calcul, des disques et des captures instantanées vers 2019-07-01</span><span class="sxs-lookup"><span data-stu-id="69d51-1052">Upgraded API version of compute, disks, snapshots to 2019-07-01</span></span>
* <span data-ttu-id="69d51-1053">vmss create : amélioration pour --orchestration-mode</span><span class="sxs-lookup"><span data-stu-id="69d51-1053">vmss create: Improvement for --orchestration-mode</span></span>
* <span data-ttu-id="69d51-1054">sig image-definition create : ajout de --os-state pour permettre de spécifier si les machines virtuelles créées sous cette image sont « généralisées » ou « spécialisées »</span><span class="sxs-lookup"><span data-stu-id="69d51-1054">sig image-definition create: Added --os-state to allow specifying whether the virtual machines created under this image are 'Generalized' or 'Specialized'</span></span>
* <span data-ttu-id="69d51-1055">sig image-definition create : ajout de --hyper-v-generation pour permettre la spécification de la génération de l’hyperviseur</span><span class="sxs-lookup"><span data-stu-id="69d51-1055">sig image-definition create: Added --hyper-v-generation to allow specifying the hypervisor generation</span></span>
* <span data-ttu-id="69d51-1056">sig image-version create : ajout de la prise en charge de --os-snapshot et de --data-snapshots</span><span class="sxs-lookup"><span data-stu-id="69d51-1056">sig image-version create: Added support --os-snapshot and --data-snapshots</span></span>
* <span data-ttu-id="69d51-1057">image create : ajout de --data-disk-caching pour autoriser la spécification du paramètre de mise en cache des disques de données</span><span class="sxs-lookup"><span data-stu-id="69d51-1057">image create: Added --data-disk-caching to allow specifying caching setting of data disks</span></span>
* <span data-ttu-id="69d51-1058">Mise à niveau du SDK Python Compute vers la version 10.0.0</span><span class="sxs-lookup"><span data-stu-id="69d51-1058">Upgraded Python Compute SDK to 10.0.0</span></span>
* <span data-ttu-id="69d51-1059">vm/vmss create : ajout de « Spot » à la propriété d’énumération « Priority »</span><span class="sxs-lookup"><span data-stu-id="69d51-1059">vm/vmss create: Added 'Spot' to 'Priority' enum property</span></span>
* <span data-ttu-id="69d51-1060">[Changement cassant] le paramètre « --max-billing » a été renommé « --max-price », pour les machines virtuelles et VMSS, à des fins de cohérence avec les applets de commande PowerShell et Swagger</span><span class="sxs-lookup"><span data-stu-id="69d51-1060">[Breaking change] Renamed '--max-billing' parameter to '--max-price', for both VM and VMSS, to be consistent with Swagger and Powershell cmdlets</span></span>
* <span data-ttu-id="69d51-1061">vm monitor log show : ajout de la prise en charge de l’interrogation du journal via l’espace de travail Log Analytics lié.</span><span class="sxs-lookup"><span data-stu-id="69d51-1061">vm monitor log show: Added support for querying log over linked log analytics workspace.</span></span>

### <a name="iot"></a><span data-ttu-id="69d51-1062">IOT</span><span class="sxs-lookup"><span data-stu-id="69d51-1062">IOT</span></span>

* <span data-ttu-id="69d51-1063">Correctif #2531 : ajout d’arguments facilitant la mise à jour des hubs.</span><span class="sxs-lookup"><span data-stu-id="69d51-1063">Fix #2531: Added convenience arguments for hub update.</span></span>
* <span data-ttu-id="69d51-1064">Correctif #8323 : ajout de paramètres manquants pour créer un point de terminaison personnalisé de stockage.</span><span class="sxs-lookup"><span data-stu-id="69d51-1064">Fix #8323: Added missing parameters to create storage custom endpoint.</span></span>
* <span data-ttu-id="69d51-1065">Correction d’un bogue de régression : restauration des modifications qui remplacent le point de terminaison de stockage par défaut.</span><span class="sxs-lookup"><span data-stu-id="69d51-1065">Fix regression bug: Reverted the changes which overrides the default storage endpoint.</span></span>

### <a name="key-vault"></a><span data-ttu-id="69d51-1066">Key Vault</span><span class="sxs-lookup"><span data-stu-id="69d51-1066">Key Vault</span></span>

* <span data-ttu-id="69d51-1067">Résolution du problème #11121 : lors de l’utilisation de `az keyvault certificate list`, le passage de `--include-pending` n’a plus besoin d’une valeur `true` ou `false`</span><span class="sxs-lookup"><span data-stu-id="69d51-1067">Fixed #11121: When using `az keyvault certificate list`, passing `--include-pending` now doesn't require a value of `true` or `false`</span></span>

### <a name="netappfiles"></a><span data-ttu-id="69d51-1068">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="69d51-1068">NetAppFiles</span></span>

* <span data-ttu-id="69d51-1069">Mise à niveau d’azure-mgmt-netapp vers 0.7.0, qui comprend des propriétés de volume supplémentaires associées aux opérations de réplication à venir</span><span class="sxs-lookup"><span data-stu-id="69d51-1069">Upgraded azure-mgmt-netapp to 0.7.0 which includes some additional volume properties associated with upcoming replication operations</span></span>

### <a name="network"></a><span data-ttu-id="69d51-1070">Réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-1070">Network</span></span>

* <span data-ttu-id="69d51-1071">application-gateway waf-config : déprécié</span><span class="sxs-lookup"><span data-stu-id="69d51-1071">application-gateway waf-config: deprecated</span></span>
* <span data-ttu-id="69d51-1072">application-gateway waf-policy : ajout de règles managées par sous-groupes pour gérer des ensembles de règles managées et des règles d’exclusion</span><span class="sxs-lookup"><span data-stu-id="69d51-1072">application-gateway waf-policy: Added subgroup managed-rules to manage managed rule sets and exclusion rules</span></span>
* <span data-ttu-id="69d51-1073">application-gateway waf-policy : ajout d’un paramètre de stratégie de sous-groupe pour gérer la configuration globale d’une stratégie WAF</span><span class="sxs-lookup"><span data-stu-id="69d51-1073">application-gateway waf-policy: Added subgroup policy-setting to manage global configuration of a waf-policy</span></span>
* <span data-ttu-id="69d51-1074">[CHANGEMENT CASSANT] application-gateway waf-policy : règle de sous-groupe renommée en custom-rule</span><span class="sxs-lookup"><span data-stu-id="69d51-1074">[BREAKING CHANGE] application-gateway waf-policy: Renamed subgroup rule to custom-rule</span></span>
* <span data-ttu-id="69d51-1075">application-gateway http-listener : ajout de --firewall-policy lors de la création</span><span class="sxs-lookup"><span data-stu-id="69d51-1075">application-gateway http-listener: Added --firewall-policy when create</span></span>
* <span data-ttu-id="69d51-1076">application-gateway url-path-map rule : ajout de --firewall-policy lors de la création</span><span class="sxs-lookup"><span data-stu-id="69d51-1076">application-gateway url-path-map rule: Added --firewall-policy when create</span></span>

### <a name="packaging"></a><span data-ttu-id="69d51-1077">Packaging</span><span class="sxs-lookup"><span data-stu-id="69d51-1077">Packaging</span></span>

* <span data-ttu-id="69d51-1078">Réécriture du wrapper az dans Python</span><span class="sxs-lookup"><span data-stu-id="69d51-1078">Rewrote the az wrapper in Python</span></span>
* <span data-ttu-id="69d51-1079">Ajout de la prise en charge de Python 3.8</span><span class="sxs-lookup"><span data-stu-id="69d51-1079">Added support for Python 3.8</span></span>
* <span data-ttu-id="69d51-1080">Remplacement par Python 3 pour le package RPM</span><span class="sxs-lookup"><span data-stu-id="69d51-1080">Changed to Python 3 for RPM package</span></span>

### <a name="profile"></a><span data-ttu-id="69d51-1081">Profil</span><span class="sxs-lookup"><span data-stu-id="69d51-1081">Profile</span></span>

* <span data-ttu-id="69d51-1082">Suppression d’une erreur liée à l’exécution de `az login -u {} -p {}` avec un compte Microsoft</span><span class="sxs-lookup"><span data-stu-id="69d51-1082">Polished error when running `az login -u {} -p {}` with Microsoft account</span></span>
* <span data-ttu-id="69d51-1083">Suppression de `SSLError` liée à l’exécution de `az login` derrière un proxy avec un certificat racine auto-signé</span><span class="sxs-lookup"><span data-stu-id="69d51-1083">Polished `SSLError` when running `az login` behind a proxy with self-signed root certificate</span></span>
* <span data-ttu-id="69d51-1084">Résolution du problème #10578 : `az login` se bloque quand plusieurs instances sont lancées en même temps sur Windows ou WSL</span><span class="sxs-lookup"><span data-stu-id="69d51-1084">Fixed #10578: `az login` hangs when more than one instances are launched at the same time on Windows or WSL</span></span>
* <span data-ttu-id="69d51-1085">Résolution du problème #11059 : `az login --allow-no-subscriptions` échoue s’il existe des abonnements dans le locataire</span><span class="sxs-lookup"><span data-stu-id="69d51-1085">Fixed #11059: `az login --allow-no-subscriptions` fails if there are subscriptions in the tenant</span></span>
* <span data-ttu-id="69d51-1086">Résolution du problème #11238 : après avoir renommé un abonnement, la connexion avec MSI entraîne l’affichage du même abonnement deux fois</span><span class="sxs-lookup"><span data-stu-id="69d51-1086">Fixed #11238: After renaming a subscription, logging in with MSI will result in the same subscription appearing twice</span></span>

### <a name="rbac"></a><span data-ttu-id="69d51-1087">RBAC</span><span class="sxs-lookup"><span data-stu-id="69d51-1087">RBAC</span></span>

* <span data-ttu-id="69d51-1088">Résolution du problème #10996 : suppression de l’erreur liée à `--force-change-password-next-login` dans `az ad user update` quand `--password` n’est pas spécifié</span><span class="sxs-lookup"><span data-stu-id="69d51-1088">Fixed #10996: Polish error for `--force-change-password-next-login` in `az ad user update` when `--password` is not specified</span></span>

### <a name="redis"></a><span data-ttu-id="69d51-1089">Redis</span><span class="sxs-lookup"><span data-stu-id="69d51-1089">Redis</span></span>

* <span data-ttu-id="69d51-1090">Résolution de l’erreur #2902 : éviter de définir des configurations de mémoire lors de la mise à jour du cache de référence SKU de base</span><span class="sxs-lookup"><span data-stu-id="69d51-1090">Fixed #2902: Avoid setting memory configs while updating Basic SKU cache</span></span>

### <a name="reservations"></a><span data-ttu-id="69d51-1091">Réservations</span><span class="sxs-lookup"><span data-stu-id="69d51-1091">Reservations</span></span>

* <span data-ttu-id="69d51-1092">Mise à niveau du SDK vers 0.6.0</span><span class="sxs-lookup"><span data-stu-id="69d51-1092">Upgraded SDK Version to 0.6.0</span></span>
* <span data-ttu-id="69d51-1093">Ajout d’informations détaillées sur le plan de facturation après l’appel de Get-Gatalogs</span><span class="sxs-lookup"><span data-stu-id="69d51-1093">Added billingplan details info after calling Get-Gatalogs</span></span>
* <span data-ttu-id="69d51-1094">Ajout d’une nouvelle commande `az reservations reservation-order calculate` pour calculer le prix d’une réservation</span><span class="sxs-lookup"><span data-stu-id="69d51-1094">Added new command `az reservations reservation-order calculate` to calculate the price for a reservation</span></span>
* <span data-ttu-id="69d51-1095">Ajout d’une nouvelle commande `az reservations reservation-order purchase` pour acheter une nouvelle réservation</span><span class="sxs-lookup"><span data-stu-id="69d51-1095">Added new command `az reservations reservation-order purchase` to purchase a new reservation</span></span>

### <a name="rest"></a><span data-ttu-id="69d51-1096">Rest</span><span class="sxs-lookup"><span data-stu-id="69d51-1096">Rest</span></span>
* <span data-ttu-id="69d51-1097">`az rest` désormais mis à la disposition générale</span><span class="sxs-lookup"><span data-stu-id="69d51-1097">Changed `az rest` to GA</span></span>

### <a name="sql"></a><span data-ttu-id="69d51-1098">SQL</span><span class="sxs-lookup"><span data-stu-id="69d51-1098">SQL</span></span>

* <span data-ttu-id="69d51-1099">Mise à jour d’azure-mgmt-sql vers la version 0.15.0.</span><span class="sxs-lookup"><span data-stu-id="69d51-1099">Updated azure-mgmt-sql to version 0.15.0.</span></span>

### <a name="storage"></a><span data-ttu-id="69d51-1100">Stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-1100">Storage</span></span>

* <span data-ttu-id="69d51-1101">storage account create : ajout de --enable-hierarchical-namespace pour prendre en charge la sémantique du système de fichiers dans le service BLOB.</span><span class="sxs-lookup"><span data-stu-id="69d51-1101">storage account create: Added --enable-hierarchical-namespace to support filesystem semantics in blob service.</span></span>
* <span data-ttu-id="69d51-1102">Suppression de l’exception non liée du message d’erreur</span><span class="sxs-lookup"><span data-stu-id="69d51-1102">Removed unrelated exception from error message</span></span>
* <span data-ttu-id="69d51-1103">Résolution des problèmes liés à un message d’erreur incorrect « Vous ne disposez pas des autorisations nécessaires pour effectuer cette opération. »</span><span class="sxs-lookup"><span data-stu-id="69d51-1103">Fixed issues with incorrect error message "You do not have the required permissions needed to perform this operation."</span></span> <span data-ttu-id="69d51-1104">en cas de blocage par des règles de réseau ou AuthenticationFailed.</span><span class="sxs-lookup"><span data-stu-id="69d51-1104">when blocked by network rules or AuthenticationFailed.</span></span>

## <a name="november-4-2019"></a><span data-ttu-id="69d51-1105">4 novembre 2019</span><span class="sxs-lookup"><span data-stu-id="69d51-1105">November 4, 2019</span></span>

<span data-ttu-id="69d51-1106">Version 2.0.76</span><span class="sxs-lookup"><span data-stu-id="69d51-1106">Version 2.0.76</span></span>

### <a name="acr"></a><span data-ttu-id="69d51-1107">ACR</span><span class="sxs-lookup"><span data-stu-id="69d51-1107">ACR</span></span>

* <span data-ttu-id="69d51-1108">Ajout d’un paramètre d’aperçu `--pack-image-tag` à la commande `az acr pack build`.</span><span class="sxs-lookup"><span data-stu-id="69d51-1108">Added a preview parameter `--pack-image-tag` to command `az acr pack build`.</span></span>
* <span data-ttu-id="69d51-1109">Ajout de la prise en charge de l’activation de l’audit lors de la création d’un registre</span><span class="sxs-lookup"><span data-stu-id="69d51-1109">Added support for enabling auditing on creating a registry</span></span>
* <span data-ttu-id="69d51-1110">Ajout de la prise en charge du contrôle d’accès en fonction du rôle délimité par le dépôt</span><span class="sxs-lookup"><span data-stu-id="69d51-1110">Added support for Repository-scoped RBAC</span></span>

### <a name="aks"></a><span data-ttu-id="69d51-1111">AKS</span><span class="sxs-lookup"><span data-stu-id="69d51-1111">AKS</span></span>

* <span data-ttu-id="69d51-1112">Ajout de `--enable-cluster-autoscaler`, `--min-count` et `--max-count` à la commande `az aks create`, ce qui active l’autoscaler de cluster pour le pool de nœuds.</span><span class="sxs-lookup"><span data-stu-id="69d51-1112">Added `--enable-cluster-autoscaler`, `--min-count` and `--max-count` to the `az aks create` command, which enables cluster autoscaler for the node pool.</span></span>
* <span data-ttu-id="69d51-1113">Ajout des indicateurs ci-dessus ainsi que de `--update-cluster-autoscaler` et `--disable-cluster-autoscaler` à la commande `az aks update`, ce qui permet d’effectuer des mises à jour de l’autoscaler de cluster.</span><span class="sxs-lookup"><span data-stu-id="69d51-1113">Added the above flags as well as `--update-cluster-autoscaler` and `--disable-cluster-autoscaler` to the `az aks update` command, allowing updates to cluster autoscaler.</span></span>

### <a name="appconfig"></a><span data-ttu-id="69d51-1114">AppConfig</span><span class="sxs-lookup"><span data-stu-id="69d51-1114">AppConfig</span></span>

* <span data-ttu-id="69d51-1115">Ajout du groupe de commandes de fonctionnalités appconfig pour gérer les indicateurs de fonctionnalité stockés dans une configuration d’application.</span><span class="sxs-lookup"><span data-stu-id="69d51-1115">Added appconfig feature command group to manage feature flags stored in an App Configuration.</span></span>
* <span data-ttu-id="69d51-1116">Correction de bogue mineur pour la commande Exporter vers un fichier appconfig kv.</span><span class="sxs-lookup"><span data-stu-id="69d51-1116">Fixed minor bug for appconfig kv export to file command.</span></span> <span data-ttu-id="69d51-1117">Arrêt de la lecture du contenu du fichier de destination pendant l’exportation.</span><span class="sxs-lookup"><span data-stu-id="69d51-1117">Stop reading dest file contents during export.</span></span>

### <a name="appservice"></a><span data-ttu-id="69d51-1118">AppService</span><span class="sxs-lookup"><span data-stu-id="69d51-1118">AppService</span></span>

* <span data-ttu-id="69d51-1119">`az appservice plan create`: Ajout de la prise en charge de la définition de « persitescaling » sur appservice plan create.</span><span class="sxs-lookup"><span data-stu-id="69d51-1119">`az appservice plan create`: Added support to set 'persitescaling' on appservice plan create.</span></span>
* <span data-ttu-id="69d51-1120">Résolution d’un problème où l’opération de liaison SSL de la configuration webapp supprimait les balises existantes de la ressource</span><span class="sxs-lookup"><span data-stu-id="69d51-1120">Fixed an issue where webapp config ssl bind operation was removing existing tags from the resource</span></span>
* <span data-ttu-id="69d51-1121">Ajout de l’indicateur `--build-remote` pour `az functionapp deployment source config-zip` afin de prendre en charge l’action de génération distante pendant le déploiement de l’application de fonction.</span><span class="sxs-lookup"><span data-stu-id="69d51-1121">Added `--build-remote` flag for `az functionapp deployment source config-zip` to support remote build action during function app deployment.</span></span>
* <span data-ttu-id="69d51-1122">Remplacement de la version du nœud par défaut sur les applications de fonction par ~10 pour Windows</span><span class="sxs-lookup"><span data-stu-id="69d51-1122">Changed default node version on function apps to ~10 for Windows</span></span>
* <span data-ttu-id="69d51-1123">Ajout de la propriété `--runtime-version` à `az functionapp create`</span><span class="sxs-lookup"><span data-stu-id="69d51-1123">Added `--runtime-version` property to `az functionapp create`</span></span>

### <a name="arm"></a><span data-ttu-id="69d51-1124">ARM</span><span class="sxs-lookup"><span data-stu-id="69d51-1124">ARM</span></span>

* <span data-ttu-id="69d51-1125">`az deployment/group deployment validate`: Ajout du paramètre `--handle-extended-json-format` pour prendre en charge le format multiligne et les commentaires dans le modèle json lors du déploiement.</span><span class="sxs-lookup"><span data-stu-id="69d51-1125">`az deployment/group deployment validate`: Added `--handle-extended-json-format` parameter to support multiline and comments in json template when deployment.</span></span>
* <span data-ttu-id="69d51-1126">Passage d’azure-mgmt-resource à 2019-07-01</span><span class="sxs-lookup"><span data-stu-id="69d51-1126">Bumped azure-mgmt-resource to 2019-07-01</span></span>

### <a name="backup"></a><span data-ttu-id="69d51-1127">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="69d51-1127">Backup</span></span>

* <span data-ttu-id="69d51-1128">Ajout de la prise en charge de la sauvegarde AzureFiles</span><span class="sxs-lookup"><span data-stu-id="69d51-1128">Added AzureFiles backup support</span></span>

### <a name="compute"></a><span data-ttu-id="69d51-1129">Calcul</span><span class="sxs-lookup"><span data-stu-id="69d51-1129">Compute</span></span>

* <span data-ttu-id="69d51-1130">`az vm create`: Ajout d’un avertissement lors de la spécification de la mise en réseau accélérée avec une carte réseau existante.</span><span class="sxs-lookup"><span data-stu-id="69d51-1130">`az vm create`: Added warning when specifying accelerated networking and an existing NIC together.</span></span>
* <span data-ttu-id="69d51-1131">`az vm create`: Ajout de `--vmss` pour spécifier un groupe identique de machines virtuelles existant auquel la machine virtuelle doit être affectée.</span><span class="sxs-lookup"><span data-stu-id="69d51-1131">`az vm create`: Added `--vmss` to specify an existing virtual machine scale set that the virtual machine should be assigned to.</span></span>
* <span data-ttu-id="69d51-1132">`az vm/vmss create`: Ajout d’une copie locale du fichier d’alias d’image afin qu’il soit accessible dans un environnement réseau restreint.</span><span class="sxs-lookup"><span data-stu-id="69d51-1132">`az vm/vmss create`: Added a local copy of image alias file so that it can be accessed in a restricted network environment.</span></span>
* <span data-ttu-id="69d51-1133">`az vmss create`: Ajout de `--orchestration-mode` pour spécifier la façon dont les machines virtuelles sont gérées par le groupe identique.</span><span class="sxs-lookup"><span data-stu-id="69d51-1133">`az vmss create`: Added `--orchestration-mode` to specify how virtual machines are managed by the scale set.</span></span>
* <span data-ttu-id="69d51-1134">`az vm/vmss update`: Ajout de `--ultra-ssd-enabled` pour autoriser la mise à jour du paramètre SSD Ultra.</span><span class="sxs-lookup"><span data-stu-id="69d51-1134">`az vm/vmss update`: Added `--ultra-ssd-enabled` to allow updating ultra SSD setting.</span></span>
* <span data-ttu-id="69d51-1135">[CHANGEMENT CASSANT] `az vm extension set` : Correction d’un bogue qui empêchait les utilisateurs de définir une extension sur une machine virtuelle avec `--ids`.</span><span class="sxs-lookup"><span data-stu-id="69d51-1135">[BREAKING CHANGE] `az vm extension set`: Fixed bug where users could not set an extension on a VM with `--ids`.</span></span>
* <span data-ttu-id="69d51-1136">Ajout de nouvelles commandes `az vm image terms accept/cancel/show` pour gérer les termes de l’image de la Place de marché Azure.</span><span class="sxs-lookup"><span data-stu-id="69d51-1136">Added new commands `az vm image terms accept/cancel/show` to manage Azure Marketplace image terms.</span></span>
* <span data-ttu-id="69d51-1137">Mise à jour de VMAccessForLinux vers la version 1.5</span><span class="sxs-lookup"><span data-stu-id="69d51-1137">Updated VMAccessForLinux to version 1.5</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="69d51-1138">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="69d51-1138">CosmosDB</span></span>

* <span data-ttu-id="69d51-1139">[CHANGEMENT CASSANT] `az sql container create` : Modification de `--partition-key-path` en paramètre obligatoire</span><span class="sxs-lookup"><span data-stu-id="69d51-1139">[BREAKING CHANGE] `az sql container create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="69d51-1140">[CHANGEMENT CASSANT] `az gremlin graph create` : Modification de `--partition-key-path` en paramètre obligatoire</span><span class="sxs-lookup"><span data-stu-id="69d51-1140">[BREAKING CHANGE] `az gremlin graph create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="69d51-1141">`az sql container create`: Ajout de `--unique-key-policy` et `--conflict-resolution-policy`</span><span class="sxs-lookup"><span data-stu-id="69d51-1141">`az sql container create`: Added `--unique-key-policy` and `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="69d51-1142">`az sql container create/update`: Mise à jour du schéma par défaut `--idx`</span><span class="sxs-lookup"><span data-stu-id="69d51-1142">`az sql container create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="69d51-1143">`gremlin graph create`: Ajout de `--conflict-resolution-policy`</span><span class="sxs-lookup"><span data-stu-id="69d51-1143">`gremlin graph create`: Added `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="69d51-1144">`gremlin graph create/update`: Mise à jour du schéma par défaut `--idx`</span><span class="sxs-lookup"><span data-stu-id="69d51-1144">`gremlin graph create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="69d51-1145">Faute de frappe corrigée dans un message d’aide</span><span class="sxs-lookup"><span data-stu-id="69d51-1145">Fixed typo in help message</span></span>
* <span data-ttu-id="69d51-1146">base de données : Ajout d’informations de dépréciation</span><span class="sxs-lookup"><span data-stu-id="69d51-1146">database: Added deprecation information</span></span>
* <span data-ttu-id="69d51-1147">collection : Ajout d’informations de dépréciation</span><span class="sxs-lookup"><span data-stu-id="69d51-1147">collection: Added deprecation information</span></span>

### <a name="iot"></a><span data-ttu-id="69d51-1148">IoT</span><span class="sxs-lookup"><span data-stu-id="69d51-1148">IoT</span></span>

* <span data-ttu-id="69d51-1149">Ajout d’un nouveau type de source de routage : DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="69d51-1149">Added new routing source type: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="69d51-1150">Correction des fonctionnalités manquantes dans `az iot hub create`</span><span class="sxs-lookup"><span data-stu-id="69d51-1150">Fixed missing features in `az iot hub create`</span></span>

### <a name="key-vault"></a><span data-ttu-id="69d51-1151">Key Vault</span><span class="sxs-lookup"><span data-stu-id="69d51-1151">Key Vault</span></span>

* <span data-ttu-id="69d51-1152">Correction d’une erreur inattendue lorsque le fichier de certificat n’existe pas</span><span class="sxs-lookup"><span data-stu-id="69d51-1152">Fixed an unexpected error when certificate file does not exist</span></span>
* <span data-ttu-id="69d51-1153">Résolution de `az keyvault recover/purge` qui ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="69d51-1153">Fixed `az keyvault recover/purge` not working</span></span>

### <a name="netappfiles"></a><span data-ttu-id="69d51-1154">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="69d51-1154">NetAppFiles</span></span>

* <span data-ttu-id="69d51-1155">Mise à niveau d’azure-mgmt-netapp vers 0.6.0 pour utiliser la version d’API 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="69d51-1155">Upgraded azure-mgmt-netapp to 0.6.0 to use API version 2019-07-01.</span></span> <span data-ttu-id="69d51-1156">Cette nouvelle version d’API comprend les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="69d51-1156">This new API version includes:</span></span>

    - <span data-ttu-id="69d51-1157">La création de volume `--protocol-types` accepte maintenant « NFSv4.1 » et non « NFSv4 »</span><span class="sxs-lookup"><span data-stu-id="69d51-1157">Volume creation `--protocol-types` accepts now "NFSv4.1" not "NFSv4"</span></span>
    - <span data-ttu-id="69d51-1158">La propriété de stratégie d’exportation de volume est maintenant nommée « nfsv41 » et non « nfsv4 »</span><span class="sxs-lookup"><span data-stu-id="69d51-1158">Volume export policy property now named 'nfsv41' not 'nfsv4'</span></span>
    - <span data-ttu-id="69d51-1159">Le volume `--creation-token` est renommé en `--file-path`</span><span class="sxs-lookup"><span data-stu-id="69d51-1159">Volume `--creation-token` renamed to `--file-path`</span></span>
    - <span data-ttu-id="69d51-1160">La date de création de l’instantané porte maintenant juste le nom « créé »</span><span class="sxs-lookup"><span data-stu-id="69d51-1160">Snapshot creation date now named just 'created'</span></span>

### <a name="network"></a><span data-ttu-id="69d51-1161">Réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-1161">Network</span></span>

* <span data-ttu-id="69d51-1162">`az network private-dns link vnet create/update`: Prise en charge de la liaison de réseau virtuel entre locataires.</span><span class="sxs-lookup"><span data-stu-id="69d51-1162">`az network private-dns link vnet create/update`: Support cross-tenant virtual network linking.</span></span>
* <span data-ttu-id="69d51-1163">[CHANGEMENT CASSANT] `az network vnet subnet list` : Modification de `--resource-group` et `--vnet-name` pour être maintenant nécessaires.</span><span class="sxs-lookup"><span data-stu-id="69d51-1163">[BREAKING CHANGE] `az network vnet subnet list`: Changed `--resource-group` and `--vnet-name` to be required now.</span></span>
* <span data-ttu-id="69d51-1164">`az network public-ip prefix create`: Ajout de la prise en charge de la spécification de la version d’adresse IP (IPv4, IPv6) lors de la création</span><span class="sxs-lookup"><span data-stu-id="69d51-1164">`az network public-ip prefix create`: Added support to specify IP address version (IPv4, IPv6) when creation</span></span>
* <span data-ttu-id="69d51-1165">Passage d’azure-mgmt-network à 7.0.0 et d’api-version à 2019-09-01</span><span class="sxs-lookup"><span data-stu-id="69d51-1165">Bumped azure-mgmt-network to 7.0.0 and api-version to 2019-09-01</span></span>
* <span data-ttu-id="69d51-1166">`az network vrouter`: Ajout de la prise en charge du nouveau routeur virtuel de service et de l’appairage de routeur virtuel</span><span class="sxs-lookup"><span data-stu-id="69d51-1166">`az network vrouter`: Added support for new service virtual router and virtual router peering</span></span>
* <span data-ttu-id="69d51-1167">`az network express-route gateway connection`: Ajout de la prise en charge de `--internet-security`</span><span class="sxs-lookup"><span data-stu-id="69d51-1167">`az network express-route gateway connection`: Added support for `--internet-security`</span></span>

### <a name="profile"></a><span data-ttu-id="69d51-1168">Profil</span><span class="sxs-lookup"><span data-stu-id="69d51-1168">Profile</span></span>

* <span data-ttu-id="69d51-1169">Résolution de `az account get-access-token --resource-type ms-graph` qui ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="69d51-1169">Fixed `az account get-access-token --resource-type ms-graph` not working</span></span>
* <span data-ttu-id="69d51-1170">Suppression de l’avertissement de `az login`</span><span class="sxs-lookup"><span data-stu-id="69d51-1170">Removed warning from `az login`</span></span>

### <a name="rbac"></a><span data-ttu-id="69d51-1171">RBAC</span><span class="sxs-lookup"><span data-stu-id="69d51-1171">RBAC</span></span>

* <span data-ttu-id="69d51-1172">Résolution de `az ad app update --id {} --display-name {}` qui ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="69d51-1172">Fixed `az ad app update --id {} --display-name {}` doesn't work</span></span>

### <a name="servicefabric"></a><span data-ttu-id="69d51-1173">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="69d51-1173">ServiceFabric</span></span>

* <span data-ttu-id="69d51-1174">`az sf cluster create`: Résolution d’un problème en modifiant le groupe identique de machines virtuelles de calcul template.json Service Fabric Linux et Windows de disques standard en disques managés</span><span class="sxs-lookup"><span data-stu-id="69d51-1174">`az sf cluster create`: Fixed an issue by modifying service fabric linux and windows template.json compute vmss from standard to managed disks</span></span>

### <a name="sql"></a><span data-ttu-id="69d51-1175">SQL</span><span class="sxs-lookup"><span data-stu-id="69d51-1175">SQL</span></span>

* <span data-ttu-id="69d51-1176">Ajout de paramètres `--compute-model`, `--auto-pause-delay` et `--min-capacity` afin de prendre en charge les opérations CRUD pour la nouvelle offre SQL Database : Modèle de calcul serverless.</span><span class="sxs-lookup"><span data-stu-id="69d51-1176">Added `--compute-model`, `--auto-pause-delay`, and `--min-capacity` parameters to support CRUD operations for new SQL Database offering: Serverless compute model.</span></span>

### <a name="storage"></a><span data-ttu-id="69d51-1177">Stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-1177">Storage</span></span>

* <span data-ttu-id="69d51-1178">`az storage account create/update`: Ajout du paramètre --enable-files-adds et du groupe d’arguments de propriétés Azure Active Directory pour prendre en charge l’authentification de service de domaine Azure Files Active Directory</span><span class="sxs-lookup"><span data-stu-id="69d51-1178">`az storage account create/update`: Added --enable-files-adds parameter and Azure Active Directory Properties Argument group to support Azure Files Active Directory Domain Service Authentication</span></span>
* <span data-ttu-id="69d51-1179">Développement de `az storage account keys list/renew` pour prendre en charge le listing ou la regénération des clés Kerberos du compte de stockage.</span><span class="sxs-lookup"><span data-stu-id="69d51-1179">Expanded `az storage account keys list/renew` to support listing or regenerating Kerberos keys of storage account.</span></span>

## <a name="october-15-2019"></a><span data-ttu-id="69d51-1180">15 octobre 2019</span><span class="sxs-lookup"><span data-stu-id="69d51-1180">October 15, 2019</span></span>

<span data-ttu-id="69d51-1181">Version 2.0.75</span><span class="sxs-lookup"><span data-stu-id="69d51-1181">Version 2.0.75</span></span>

### <a name="aks"></a><span data-ttu-id="69d51-1182">AKS</span><span class="sxs-lookup"><span data-stu-id="69d51-1182">AKS</span></span>

* <span data-ttu-id="69d51-1183">Remplacement de la valeur par défaut `--load-balancer-sku` par `standard` si elle est prise en charge par la version kubernetes</span><span class="sxs-lookup"><span data-stu-id="69d51-1183">Changed `--load-balancer-sku` default value to `standard` if supported by the kubernetes version</span></span>
* <span data-ttu-id="69d51-1184">Remplacement de la valeur par défaut `--vm-set-type` par `virtualmachinescalesets` si elle est prise en charge par la version kubernetes</span><span class="sxs-lookup"><span data-stu-id="69d51-1184">Changed `--vm-set-type` default value to `virtualmachinescalesets` if supported by the kubernetes version</span></span>

### <a name="ams"></a><span data-ttu-id="69d51-1185">AMS</span><span class="sxs-lookup"><span data-stu-id="69d51-1185">AMS</span></span>

* <span data-ttu-id="69d51-1186">[CHANGEMENT CASSANT] Remplacement du nom `job start` par `job create`</span><span class="sxs-lookup"><span data-stu-id="69d51-1186">[BREAKING CHANGE] Changed the name of `job start` to `job create`</span></span>
* <span data-ttu-id="69d51-1187">[CHANGEMENT CASSANT] Changement du paramètre `--ask` de `content-key-policy create` pour utiliser une chaîne hexadécimale de 32 caractères au lieu d’UTF8</span><span class="sxs-lookup"><span data-stu-id="69d51-1187">[BREAKING CHANGE] Changed the `--ask` parameter of `content-key-policy create` to use a 32-character hex string instead of UTF8</span></span>

### <a name="appservice"></a><span data-ttu-id="69d51-1188">AppService</span><span class="sxs-lookup"><span data-stu-id="69d51-1188">AppService</span></span>

* <span data-ttu-id="69d51-1189">Ajout des commandes `webapp config access-restriction show|set|add|remove`</span><span class="sxs-lookup"><span data-stu-id="69d51-1189">Added commands `webapp config access-restriction show|set|add|remove`</span></span>
* <span data-ttu-id="69d51-1190">Ajout d’une meilleure gestion des erreurs à `webapp up`</span><span class="sxs-lookup"><span data-stu-id="69d51-1190">Added better error handling to `webapp up`</span></span>
* <span data-ttu-id="69d51-1191">Ajout de la prise en charge de la référence SKU `Isolated` pour `appservice plan update`</span><span class="sxs-lookup"><span data-stu-id="69d51-1191">Added support for `Isolated` SKU to `appservice plan update`</span></span>

### <a name="arm"></a><span data-ttu-id="69d51-1192">ARM</span><span class="sxs-lookup"><span data-stu-id="69d51-1192">ARM</span></span>

* <span data-ttu-id="69d51-1193">Ajout du paramètre `--handle-extended-json-format` à `deployment create` pour prendre en charge le format multiligne et les commentaires dans le modèle json</span><span class="sxs-lookup"><span data-stu-id="69d51-1193">Added `--handle-extended-json-format` parameter `deployment create` to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="69d51-1194">Calcul</span><span class="sxs-lookup"><span data-stu-id="69d51-1194">Compute</span></span>

* <span data-ttu-id="69d51-1195">Ajout du paramètre `--enable-agent` pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="69d51-1195">Added `--enable-agent` parameter to `vm create`</span></span>
* <span data-ttu-id="69d51-1196">Changement de `vm create` pour utiliser automatiquement la référence SKU d’adresse IP publique standard lors de l’utilisation de zones</span><span class="sxs-lookup"><span data-stu-id="69d51-1196">Changed `vm create` to use standard public IP SKU automatically when using zones</span></span>
* <span data-ttu-id="69d51-1197">Changement de `vm create` pour créer automatiquement un nom d’ordinateur valide pour une machine virtuelle si aucun n’est fourni</span><span class="sxs-lookup"><span data-stu-id="69d51-1197">Changed `vm create` to automatically create a valid computer name for a VM if none is provided</span></span>
* <span data-ttu-id="69d51-1198">Ajout du paramètre `--computer-name-prefix` à `vmss create` pour prendre en charge le préfixe de nom d’ordinateur personnalisé des machines virtuelles dans VMSS</span><span class="sxs-lookup"><span data-stu-id="69d51-1198">Added `--computer-name-prefix` parameter to `vmss create` to support custom computer name prefix of virtual machines in the VMSS</span></span>
* <span data-ttu-id="69d51-1199">Ajout du paramètre `--workspace` à `vm create` pour activer automatiquement l’espace de travail Log Analytics</span><span class="sxs-lookup"><span data-stu-id="69d51-1199">Add `--workspace` parameter to `vm create` to enable log analytics workspace automatically</span></span>
* <span data-ttu-id="69d51-1200">Mise à jour de la version de l’API des galeries vers 2019-07-01</span><span class="sxs-lookup"><span data-stu-id="69d51-1200">Updated galleries API version to 2019-07-01</span></span>

### <a name="core"></a><span data-ttu-id="69d51-1201">Core</span><span class="sxs-lookup"><span data-stu-id="69d51-1201">Core</span></span>

* <span data-ttu-id="69d51-1202">Ajout de la vérification de la syntaxe pour le paramètre `--set` dans la commande de mise à jour générique</span><span class="sxs-lookup"><span data-stu-id="69d51-1202">Added syntax check for `--set` parameter in generic update command</span></span>

### <a name="iot"></a><span data-ttu-id="69d51-1203">IoT</span><span class="sxs-lookup"><span data-stu-id="69d51-1203">IoT</span></span>

* <span data-ttu-id="69d51-1204">Résolution d’un problème où `iot hub show` entraînait une erreur incorrecte « ressource introuvable »</span><span class="sxs-lookup"><span data-stu-id="69d51-1204">Fixed an issue where `iot hub show` would incorrectly error with "resource not found"</span></span>

### <a name="monitor"></a><span data-ttu-id="69d51-1205">Superviser</span><span class="sxs-lookup"><span data-stu-id="69d51-1205">Monitor</span></span>

* <span data-ttu-id="69d51-1206">Ajout de la prise en charge de CRUD dans `monitor log-analytics workspace`</span><span class="sxs-lookup"><span data-stu-id="69d51-1206">Added support for CRUD to `monitor log-analytics workspace`</span></span>

### <a name="network"></a><span data-ttu-id="69d51-1207">Réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-1207">Network</span></span>

* <span data-ttu-id="69d51-1208">Ajout de la prise en charge de la liaison virtuelle interlocataire dans `network private-dns link vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69d51-1208">Added support for cross-tenant virtual linking to `network private-dns link vnet [create|update]`</span></span>
* <span data-ttu-id="69d51-1209">[CHANGEMENT CASSANT] Changement de `network vnet subnet list` pour exiger les paramètres `--resource-group` et `--vnet-name`</span><span class="sxs-lookup"><span data-stu-id="69d51-1209">[BREAKING CHANGE] Changed `network vnet subnet list` to require `--resource-group` and `--vnet-name` parameters</span></span>

### <a name="sql"></a><span data-ttu-id="69d51-1210">SQL</span><span class="sxs-lookup"><span data-stu-id="69d51-1210">SQL</span></span>

* <span data-ttu-id="69d51-1211">Ajout de commandes à `sql mi ad-admin` qui prennent en charge la définition d’un administrateur AAD sur des instances managées</span><span class="sxs-lookup"><span data-stu-id="69d51-1211">Added commands to `sql mi ad-admin` that support setting an AAD administrator on managed instances</span></span>

### <a name="storage"></a><span data-ttu-id="69d51-1212">Stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-1212">Storage</span></span>

* <span data-ttu-id="69d51-1213">Ajout du paramètre `--preserve-s2s-access-tier` à `storage copy` pour préserver le niveau d’accès lors d’une copie de service à service</span><span class="sxs-lookup"><span data-stu-id="69d51-1213">Added `--preserve-s2s-access-tier` parameter `storage copy` to preserve access tier during service to service copy</span></span>
* <span data-ttu-id="69d51-1214">Ajout du paramètre `--enable-large-file-share` à `storage account [create|update]` afin de prendre en charge les gros partages de fichiers pour le compte de stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-1214">Added `--enable-large-file-share` parameter to `storage account [create|update]` to support large file shares for storage account</span></span>

## <a name="september-24-2019"></a><span data-ttu-id="69d51-1215">24 septembre 2019</span><span class="sxs-lookup"><span data-stu-id="69d51-1215">September 24, 2019</span></span>

<span data-ttu-id="69d51-1216">Version 2.0.74</span><span class="sxs-lookup"><span data-stu-id="69d51-1216">Version 2.0.74</span></span>

### <a name="acr"></a><span data-ttu-id="69d51-1217">ACR</span><span class="sxs-lookup"><span data-stu-id="69d51-1217">ACR</span></span>

* <span data-ttu-id="69d51-1218">Ajout d’un paramètre `--type` obligatoire à `acr config retention update`</span><span class="sxs-lookup"><span data-stu-id="69d51-1218">Added a required `--type` parameter to `acr config retention update`</span></span>
* <span data-ttu-id="69d51-1219">[CHANGEMENT CASSANT] Renommage du paramètre `--name -n` en `--registry -r ` pour le groupe de commandes `acr config`</span><span class="sxs-lookup"><span data-stu-id="69d51-1219">[BREAKING CHANGE] Renamed parameter `--name -n` changed to `--registry -r ` for `acr config` command group</span></span>

### <a name="aks"></a><span data-ttu-id="69d51-1220">AKS</span><span class="sxs-lookup"><span data-stu-id="69d51-1220">AKS</span></span>

* <span data-ttu-id="69d51-1221">Ajout du paramètre `--load-balancer-sku` à la commande `aks create`, ce qui permet de créer un cluster AKS avec SLB</span><span class="sxs-lookup"><span data-stu-id="69d51-1221">Added `--load-balancer-sku` parameter to `aks create` command, which allows for creating AKS cluster with SLB</span></span>
* <span data-ttu-id="69d51-1222">Ajout des paramètres `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` et `--load-balancer-outbound-ip-prefixes` aux commandes `aks [create|update]`, ce qui permet de mettre à jour le profil d’équilibreur de charge d’un cluster AKS avec SLB</span><span class="sxs-lookup"><span data-stu-id="69d51-1222">Added `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` and `--load-balancer-outbound-ip-prefixes` parameters to `aks [create|update]` commands, which allow for updating load balancer profile of an AKS cluster with SLB</span></span>
* <span data-ttu-id="69d51-1223">Ajout du paramètre `--vm-set-type` à la commande `aks create`, ce qui permet de spécifier les types de machines virtuelles d’un cluster AKS (vmas ou vmss)</span><span class="sxs-lookup"><span data-stu-id="69d51-1223">Added `--vm-set-type` parameter to `aks create` command, which allows to specify vm types of an AKS Cluster (vmas or vmss)</span></span>

### <a name="arm"></a><span data-ttu-id="69d51-1224">ARM</span><span class="sxs-lookup"><span data-stu-id="69d51-1224">ARM</span></span>

* <span data-ttu-id="69d51-1225">Ajout du paramètre `--handle-extended-json-format` à la commande `group deployment create` pour prendre en charge les lignes multiples et les commentaires dans le modèle JSON</span><span class="sxs-lookup"><span data-stu-id="69d51-1225">Added `--handle-extended-json-format` parameter to `group deployment create` command to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="69d51-1226">Calcul</span><span class="sxs-lookup"><span data-stu-id="69d51-1226">Compute</span></span>

* <span data-ttu-id="69d51-1227">Ajout du paramètre `--terminate-notification-time` aux commandes `vmss [create|update]` pour prendre en charge la configuration de l’événement planifié d’arrêt</span><span class="sxs-lookup"><span data-stu-id="69d51-1227">Added `--terminate-notification-time` parameter to `vmss [create|update]` commands to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="69d51-1228">Ajout du paramètre `--enable-terminate-notification` à la commande `vmss update` pour prendre en charge la configuration de l’événement planifié d’arrêt</span><span class="sxs-lookup"><span data-stu-id="69d51-1228">Added `--enable-terminate-notification` parameter to `vmss update` command to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="69d51-1229">Ajout des paramètres `--priority,``--eviction-policy,``--max-billing` aux commandes `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="69d51-1229">Added `--priority,` `--eviction-policy,` `--max-billing` parameters to `[vm|vmss] create` commands</span></span>
* <span data-ttu-id="69d51-1230">Modification de `disk create` pour autoriser la spécification de la taille exacte du chargement de disque</span><span class="sxs-lookup"><span data-stu-id="69d51-1230">Changed `disk create` to allow specifying the exact size of the disk upload</span></span>
* <span data-ttu-id="69d51-1231">Ajout de la prise en charge des instantanés incrémentiels pour les disques managés à `snapshot create`</span><span class="sxs-lookup"><span data-stu-id="69d51-1231">Added support for incremental snapshots for managed disks to `snapshot create`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="69d51-1232">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="69d51-1232">Cosmos DB</span></span>

* <span data-ttu-id="69d51-1233">Ajout du paramètre `--type <key-type>` à la commande `cosmosdb keys list` pour afficher la clé, les clés en lecture seule ou les chaînes de connexion</span><span class="sxs-lookup"><span data-stu-id="69d51-1233">Added `--type <key-type>` parameter to `cosmosdb keys list` command to show key, read only keys or connection strings</span></span>
* <span data-ttu-id="69d51-1234">Ajout de la commande `cosmosdb keys regenerate`</span><span class="sxs-lookup"><span data-stu-id="69d51-1234">Added `cosmosdb keys regenerate` command</span></span>
* <span data-ttu-id="69d51-1235">[DÉPRÉCIATION] Dépréciation des commandes `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` et `cosmosdb list-read-only-keys`</span><span class="sxs-lookup"><span data-stu-id="69d51-1235">[DEPRECATED] Deprecated `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` and `cosmosdb list-read-only-keys` commands</span></span>

### <a name="eventgrid"></a><span data-ttu-id="69d51-1236">EventGrid</span><span class="sxs-lookup"><span data-stu-id="69d51-1236">EventGrid</span></span>

* <span data-ttu-id="69d51-1237">Correction du texte d’aide du point de terminaison de manière à faire référence au bon paramètre</span><span class="sxs-lookup"><span data-stu-id="69d51-1237">Fixed the endpoint help text to refer to the right parameter</span></span>

### <a name="key-vault"></a><span data-ttu-id="69d51-1238">Key Vault</span><span class="sxs-lookup"><span data-stu-id="69d51-1238">Key Vault</span></span>

* <span data-ttu-id="69d51-1239">Résolution d’un problème de connexion avec un locataire (`login -t`) qui pouvait provoquer l’échec de `keyvault create`</span><span class="sxs-lookup"><span data-stu-id="69d51-1239">Fixed issue where logging in with a tenant (`login -t`) could cause `keyvault create` to fail</span></span>

### <a name="monitor"></a><span data-ttu-id="69d51-1240">Superviser</span><span class="sxs-lookup"><span data-stu-id="69d51-1240">Monitor</span></span>

* <span data-ttu-id="69d51-1241">Résolution d’un problème où le caractère `:` n’était pas autorisé dans l’argument `--condition` de `monitor metrics alert create`</span><span class="sxs-lookup"><span data-stu-id="69d51-1241">Fixed issue where `:` character was not allowed in `--condition` argument to `monitor metrics alert create`</span></span>

### <a name="policy"></a><span data-ttu-id="69d51-1242">Policy</span><span class="sxs-lookup"><span data-stu-id="69d51-1242">Policy</span></span>

* <span data-ttu-id="69d51-1243">Ajout de la prise en charge de l’API Policy version 2019-06-01</span><span class="sxs-lookup"><span data-stu-id="69d51-1243">Added support for Policy API version 2019-06-01</span></span>
* <span data-ttu-id="69d51-1244">Ajout du paramètre `--enforcement-mode` à la commande `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="69d51-1244">Added `--enforcement-mode` parameter to `policy assignment create` command</span></span>

### <a name="storage"></a><span data-ttu-id="69d51-1245">Stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-1245">Storage</span></span>

* <span data-ttu-id="69d51-1246">Ajout du paramètre `--blob-type` à la commande `az storage copy`</span><span class="sxs-lookup"><span data-stu-id="69d51-1246">Added `--blob-type` parameter to `az storage copy` command</span></span>

## <a name="september-10-2019"></a><span data-ttu-id="69d51-1247">10 septembre 2019</span><span class="sxs-lookup"><span data-stu-id="69d51-1247">September 10, 2019</span></span>

### <a name="acr"></a><span data-ttu-id="69d51-1248">ACR</span><span class="sxs-lookup"><span data-stu-id="69d51-1248">ACR</span></span>

* <span data-ttu-id="69d51-1249">Ajout du groupe de commandes `acr config retention` pour configurer une stratégie de conservation</span><span class="sxs-lookup"><span data-stu-id="69d51-1249">Added command group `acr config retention` to configure retention policy</span></span>

### <a name="aks"></a><span data-ttu-id="69d51-1250">AKS</span><span class="sxs-lookup"><span data-stu-id="69d51-1250">AKS</span></span>

* <span data-ttu-id="69d51-1251">Ajout de la prise en charge de l’intégration ACR avec les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="69d51-1251">Added support for ACR integration with the following commands:</span></span>
  * <span data-ttu-id="69d51-1252">Ajout du paramètre `--attach-acr` à `aks [create|update]` pour attacher un ACR à un cluster AKS</span><span class="sxs-lookup"><span data-stu-id="69d51-1252">Added `--attach-acr` parameter to `aks [create|update]` to attach an ACR to an AKS cluster</span></span>
  * <span data-ttu-id="69d51-1253">Ajout du paramètre `--detach-acr` à `aks update` pour détacher l’ACR d’un cluster AKS</span><span class="sxs-lookup"><span data-stu-id="69d51-1253">Added `--detach-acr` parameter to `aks update` to detach the ACR from an AKS cluster</span></span>

### <a name="arm"></a><span data-ttu-id="69d51-1254">ARM</span><span class="sxs-lookup"><span data-stu-id="69d51-1254">ARM</span></span>

* <span data-ttu-id="69d51-1255">Mis à jour pour utiliser la version d’API 2019-05-10</span><span class="sxs-lookup"><span data-stu-id="69d51-1255">Updated to use API version 2019-05-10</span></span>

### <a name="batch"></a><span data-ttu-id="69d51-1256">Batch</span><span class="sxs-lookup"><span data-stu-id="69d51-1256">Batch</span></span>

* <span data-ttu-id="69d51-1257">Ajout de nouveaux paramètres de configuration JSON à `--json-file` pour `batch pool create` :</span><span class="sxs-lookup"><span data-stu-id="69d51-1257">Added new JSON configuration settings to `--json-file` for `batch pool create`:</span></span>
  * <span data-ttu-id="69d51-1258">Ajout de `MountConfigurations` pour les montages de système de fichiers (voir https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body pour les détails)</span><span class="sxs-lookup"><span data-stu-id="69d51-1258">Added `MountConfigurations` for file system mounts (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
  * <span data-ttu-id="69d51-1259">Ajout de la propriété facultative `publicIPs` sur `NetworkConfiguration` pour les adresses IP publiques sur les pools (voir https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body pour les détails)</span><span class="sxs-lookup"><span data-stu-id="69d51-1259">Added optional property `publicIPs` on `NetworkConfiguration` for public IPs on pools (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
* <span data-ttu-id="69d51-1260">Ajout de la prise en charge des galeries d’images partagées à `--image`</span><span class="sxs-lookup"><span data-stu-id="69d51-1260">Added support for shared image galleries to `--image`</span></span>
* <span data-ttu-id="69d51-1261">[CHANGEMENT CASSANT] Changement de la valeur par défaut `--start-task-wait-for-success` sur `batch pool create` qui devient `true`</span><span class="sxs-lookup"><span data-stu-id="69d51-1261">[BREAKING CHANGE] Changed default value of `--start-task-wait-for-success` on `batch pool create` to be `true`</span></span>
* <span data-ttu-id="69d51-1262">[CHANGEMENT CASSANT] Changement de la valeur par défaut pour `Scope` sur `AutoUserSpecification` pour qu’elle soit toujours Pool (était `Task` sur les nœuds Windows, `Pool` sur les nœuds Linux)</span><span class="sxs-lookup"><span data-stu-id="69d51-1262">[BREAKING CHANGE] Changed default value for `Scope` on `AutoUserSpecification` to always be Pool (was `Task` on Windows nodes, `Pool` on Linux nodes)</span></span>
  * <span data-ttu-id="69d51-1263">Cet argument ne peut être défini qu’à partir d’une configuration JSON avec `--json-file`</span><span class="sxs-lookup"><span data-stu-id="69d51-1263">This argument can only be set from a JSON configuration with `--json-file`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="69d51-1264">HDInsight</span><span class="sxs-lookup"><span data-stu-id="69d51-1264">HDInsight</span></span>

* <span data-ttu-id="69d51-1265">Version mise à la disposition générale</span><span class="sxs-lookup"><span data-stu-id="69d51-1265">GA release</span></span>
* <span data-ttu-id="69d51-1266">[CHANGEMENT CASSANT] Changement du paramètre `--workernode-count/-c` de `az hdinsight resize` pour le rendre obligatoire.</span><span class="sxs-lookup"><span data-stu-id="69d51-1266">[BREAKING CHANGE] Changed parameter `--workernode-count/-c` of `az hdinsight resize` to be required.</span></span>

### <a name="key-vault"></a><span data-ttu-id="69d51-1267">Key Vault</span><span class="sxs-lookup"><span data-stu-id="69d51-1267">Key Vault</span></span>

* <span data-ttu-id="69d51-1268">Résolution d’un problème où les sous-réseaux ne pouvaient pas être supprimés des règles réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-1268">Fixed issue where subnets couldn't be deleted from network rules</span></span>
* <span data-ttu-id="69d51-1269">Résolution d’un problème où des sous-réseaux et des adresses IP dupliqués pouvaient être ajoutés aux règles réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-1269">Fixed issue where duplicated subnets and IP addresses could be added to network rules</span></span>

### <a name="network"></a><span data-ttu-id="69d51-1270">Réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-1270">Network</span></span>

* <span data-ttu-id="69d51-1271">Ajout du paramètre `--interval` à `network watcher flow-log` pour définir la valeur d’intervalle de l’analyse du trafic</span><span class="sxs-lookup"><span data-stu-id="69d51-1271">Added `--interval` parameter to `network watcher flow-log` to set traffic analysis interval value</span></span>
* <span data-ttu-id="69d51-1272">Ajout de `network application-gateway identity` pour gérer l’identité de la passerelle</span><span class="sxs-lookup"><span data-stu-id="69d51-1272">Added `network application-gateway identity` to manage gateway identity</span></span>
* <span data-ttu-id="69d51-1273">Ajout de la prise en charge de la définition de l’ID Key Vault sur `network application-gateway ssl-cert`</span><span class="sxs-lookup"><span data-stu-id="69d51-1273">Added support for setting Key Vault ID to `network application-gateway ssl-cert`</span></span>
* <span data-ttu-id="69d51-1274">Ajout de `network express-route peering peer-connection [show|list]`</span><span class="sxs-lookup"><span data-stu-id="69d51-1274">Added `network express-route peering peer-connection [show|list]`</span></span>

### <a name="policy"></a><span data-ttu-id="69d51-1275">Policy</span><span class="sxs-lookup"><span data-stu-id="69d51-1275">Policy</span></span>

* <span data-ttu-id="69d51-1276">Mis à jour pour utiliser la version d’API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="69d51-1276">Updated to use API version 2019-01-01</span></span>

## <a name="august-27-2019"></a><span data-ttu-id="69d51-1277">27 août 2019</span><span class="sxs-lookup"><span data-stu-id="69d51-1277">August 27, 2019</span></span>

<span data-ttu-id="69d51-1278">Version 2.0.72</span><span class="sxs-lookup"><span data-stu-id="69d51-1278">Version 2.0.72</span></span>

### <a name="acr"></a><span data-ttu-id="69d51-1279">ACR</span><span class="sxs-lookup"><span data-stu-id="69d51-1279">ACR</span></span>

* <span data-ttu-id="69d51-1280">[CHANGEMENT CASSANT] Suppression de la prise en charge de la référence SKU `classic`</span><span class="sxs-lookup"><span data-stu-id="69d51-1280">[BREAKING CHANGE] Removed support for the `classic` SKU</span></span>

### <a name="api-management"></a><span data-ttu-id="69d51-1281">Gestion des API</span><span class="sxs-lookup"><span data-stu-id="69d51-1281">API Management</span></span>

* <span data-ttu-id="69d51-1282">[PRÉVERSION] Ajout du groupe de commandes `apim`</span><span class="sxs-lookup"><span data-stu-id="69d51-1282">[PREVIEW] Added `apim` command group</span></span>

### <a name="appservice"></a><span data-ttu-id="69d51-1283">AppService</span><span class="sxs-lookup"><span data-stu-id="69d51-1283">AppService</span></span>

* <span data-ttu-id="69d51-1284">Résolution du problème avec la commande `webapp webjob continuous start` lors de la spécification d’un emplacement</span><span class="sxs-lookup"><span data-stu-id="69d51-1284">Fixed issue with `webapp webjob continuous start` command when specifying a slot</span></span>
* <span data-ttu-id="69d51-1285">Modification de `webapp up` pour détecter le dossier `env` et le supprimer du fichier utilisé pour le déploiement</span><span class="sxs-lookup"><span data-stu-id="69d51-1285">Changed `webapp up` to detect `env` folder and remove it from the file used for deployment</span></span>

### <a name="keyvault"></a><span data-ttu-id="69d51-1286">KeyVault</span><span class="sxs-lookup"><span data-stu-id="69d51-1286">Keyvault</span></span>

* <span data-ttu-id="69d51-1287">Correction d’un bogue dans `keyvault secret set` qui ignorait l’argument `--expires`</span><span class="sxs-lookup"><span data-stu-id="69d51-1287">Fixed a bug in `keyvault secret set` that igored the `--expires` argument</span></span>

### <a name="network"></a><span data-ttu-id="69d51-1288">Réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-1288">Network</span></span>

* <span data-ttu-id="69d51-1289">Ajout de la prise en charge des adresses IPv6 pour les arguments `--private-ip-address-version`</span><span class="sxs-lookup"><span data-stu-id="69d51-1289">Added support for IPv6 addresses to `--private-ip-address-version` arguments</span></span>
* <span data-ttu-id="69d51-1290">Ajout des nouvelles commandes `network private-endpoint [create|update|list-types]` pour la gestion des points de terminaison privés</span><span class="sxs-lookup"><span data-stu-id="69d51-1290">Added new commands `network private-endpoint [create|update|list-types]` for private endpoint management</span></span>
* <span data-ttu-id="69d51-1291">Ajout du groupe de commandes `network private-link-service`</span><span class="sxs-lookup"><span data-stu-id="69d51-1291">Added command group `network private-link-service`</span></span>
* <span data-ttu-id="69d51-1292">Ajout des arguments `--private-endpoint-network-policies` et `--private-link-service-network-policies` à `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="69d51-1292">Added `--private-endpoint-network-policies` and `--private-link-service-network-policies` arguments to `network vnet subnet update`</span></span>

### <a name="rbac"></a><span data-ttu-id="69d51-1293">RBAC</span><span class="sxs-lookup"><span data-stu-id="69d51-1293">RBAC</span></span>

* <span data-ttu-id="69d51-1294">Correction du problème `ad app update --homepage` où la page d’accueil ne se mettait pas à jour</span><span class="sxs-lookup"><span data-stu-id="69d51-1294">Fixed issue with `ad app update --homepage` where homepage would not be updated</span></span>

### <a name="servicefabric"></a><span data-ttu-id="69d51-1295">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="69d51-1295">ServiceFabric</span></span>

* <span data-ttu-id="69d51-1296">Ajout de la prise en charge pour les noms Key Vault en casse mixte</span><span class="sxs-lookup"><span data-stu-id="69d51-1296">Added support for mixed-case Key Vault names</span></span>
* <span data-ttu-id="69d51-1297">Résolution du problème lors de l’utilisation de certificats dans Key Vault</span><span class="sxs-lookup"><span data-stu-id="69d51-1297">Fixed issue when using certificates in Key Vault</span></span>
* <span data-ttu-id="69d51-1298">Résolution du problème lors de l’utilisation des fichiers de certificat PFX</span><span class="sxs-lookup"><span data-stu-id="69d51-1298">Fixed issue with using PFX certificate files</span></span>
* <span data-ttu-id="69d51-1299">Correction du problème avec `sf cluster certificate add` quand le groupe de ressources Key Vault n’était pas spécifié</span><span class="sxs-lookup"><span data-stu-id="69d51-1299">Fixed issue with `sf cluster certificate add` when Key Vault resource group wasn't specified</span></span>
* <span data-ttu-id="69d51-1300">Correction du problème où `sf cluster set` ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="69d51-1300">Fixed issue with `sf cluster set` not working</span></span>

### <a name="signalr"></a><span data-ttu-id="69d51-1301">SignalR</span><span class="sxs-lookup"><span data-stu-id="69d51-1301">SignalR</span></span>

* <span data-ttu-id="69d51-1302">Ajout de nouvelles commandes :</span><span class="sxs-lookup"><span data-stu-id="69d51-1302">Added new commands:</span></span>
  * <span data-ttu-id="69d51-1303">`signalr cors`: Gérer SignalR CORS</span><span class="sxs-lookup"><span data-stu-id="69d51-1303">`signalr cors`: Manage SignalR CORS</span></span>
  * <span data-ttu-id="69d51-1304">`signalr restart`: Redémarrer un service SignalR</span><span class="sxs-lookup"><span data-stu-id="69d51-1304">`signalr restart`: Restart a SignalR service</span></span>
  * <span data-ttu-id="69d51-1305">`signalr update`: Mettre à jour un service SignalR</span><span class="sxs-lookup"><span data-stu-id="69d51-1305">`signalr update`: Update a SignalR service</span></span>
* <span data-ttu-id="69d51-1306">Ajout de l’argument `--service-mode` à `signalr create`</span><span class="sxs-lookup"><span data-stu-id="69d51-1306">Added `--service-mode` argument to `signalr create`</span></span>

### <a name="storage"></a><span data-ttu-id="69d51-1307">Stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-1307">Storage</span></span>

* <span data-ttu-id="69d51-1308">Ajout de la commande `storage account revoke-delegation-keys`</span><span class="sxs-lookup"><span data-stu-id="69d51-1308">Added `storage account revoke-delegation-keys` command</span></span>

## <a name="august-13-2019"></a><span data-ttu-id="69d51-1309">13 août 2019</span><span class="sxs-lookup"><span data-stu-id="69d51-1309">August 13, 2019</span></span>

<span data-ttu-id="69d51-1310">Version 2.0.71</span><span class="sxs-lookup"><span data-stu-id="69d51-1310">Version 2.0.71</span></span>

### <a name="appservice"></a><span data-ttu-id="69d51-1311">AppService</span><span class="sxs-lookup"><span data-stu-id="69d51-1311">AppService</span></span>

* <span data-ttu-id="69d51-1312">Correction d’un problème entraînant l’échec des commandes `webapp webjob continuous` pour les emplacements</span><span class="sxs-lookup"><span data-stu-id="69d51-1312">Fixed issue where `webapp webjob continuous` commands were failing for slots</span></span>

### <a name="botservice"></a><span data-ttu-id="69d51-1313">BotService</span><span class="sxs-lookup"><span data-stu-id="69d51-1313">BotService</span></span>

* <span data-ttu-id="69d51-1314">[CHANGEMENT CASSANT] Suppression de la prise en charge de la création de bots SDK v3</span><span class="sxs-lookup"><span data-stu-id="69d51-1314">[BREAKING CHANGE] Removed support for creating v3 SDK bots</span></span>

### <a name="cognitiveservices"></a><span data-ttu-id="69d51-1315">CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="69d51-1315">CognitiveServices</span></span>

* <span data-ttu-id="69d51-1316">Ajout des commandes `cognitiveservices account network-rule`</span><span class="sxs-lookup"><span data-stu-id="69d51-1316">Added `cognitiveservices account network-rule` commands</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="69d51-1317">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="69d51-1317">Cosmos DB</span></span>

* <span data-ttu-id="69d51-1318">Suppression de l’avertissement lors de la mise à jour de plusieurs emplacements d’écriture</span><span class="sxs-lookup"><span data-stu-id="69d51-1318">Removed warning when updating multiple write locations</span></span>
* <span data-ttu-id="69d51-1319">Ajout de commandes CRUD pour les ressources CosmosDB SQL, MongoDB, Cassandra, Gremlin et Table et le débit de la ressource</span><span class="sxs-lookup"><span data-stu-id="69d51-1319">Added CRUD commands for CosmosDB SQL, MongoDB, Cassandra, Gremlin and Table resources and resource's throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="69d51-1320">HDInsight</span><span class="sxs-lookup"><span data-stu-id="69d51-1320">HDInsight</span></span>

<span data-ttu-id="69d51-1321">Cette version contient un grand nombre de modifications conséquentes.</span><span class="sxs-lookup"><span data-stu-id="69d51-1321">This release contains a large number of breaking changes.</span></span>

* <span data-ttu-id="69d51-1322">[CHANGEMENT CASSANT] Renommage des paramètres pour `hdinsight create` :</span><span class="sxs-lookup"><span data-stu-id="69d51-1322">[BREAKING CHANGE] Renamed parameters for `hdinsight create`:</span></span>
  * <span data-ttu-id="69d51-1323">`--storage-default-container` renommé en `--storage-container`</span><span class="sxs-lookup"><span data-stu-id="69d51-1323">Renamed `--storage-default-container` to `--storage-container`</span></span>
  * <span data-ttu-id="69d51-1324">`--storage-default-filesystem` renommé en `--storage-filesystem`</span><span class="sxs-lookup"><span data-stu-id="69d51-1324">Renamed `--storage-default-filesystem` to `--storage-filesystem`</span></span>
* <span data-ttu-id="69d51-1325">[CHANGEMENT CASSANT] Modification de l’argument `--name` de `application create` pour représenter le nom de l’application à la place du nom du cluster</span><span class="sxs-lookup"><span data-stu-id="69d51-1325">[BREAKING CHANGE] Changed the `--name` argument of `application create` to represent the application name instead of the cluster name</span></span>
* <span data-ttu-id="69d51-1326">Ajout d’un argument `--cluster-name` à `application create` pour remplacer l’ancienne fonctionnalité `--name`</span><span class="sxs-lookup"><span data-stu-id="69d51-1326">Added `--cluster-name` argument to `application create` to replace old `--name` functionality</span></span>
* <span data-ttu-id="69d51-1327">[CHANGEMENT CASSANT] Renommage des paramètres pour `application create` :</span><span class="sxs-lookup"><span data-stu-id="69d51-1327">[BREAKING CHANGE] Renamed parameters for `application create`:</span></span>
  * <span data-ttu-id="69d51-1328">`--application-type` renommé en `--type`</span><span class="sxs-lookup"><span data-stu-id="69d51-1328">Renamed `--application-type` to `--type`</span></span>
  * <span data-ttu-id="69d51-1329">`--marketplace-identifier` renommé en `--marketplace-id`</span><span class="sxs-lookup"><span data-stu-id="69d51-1329">Renamed `--marketplace-identifier` to `--marketplace-id`</span></span>
  * <span data-ttu-id="69d51-1330">`--https-endpoint-access-mode` renommé en `--access-mode`</span><span class="sxs-lookup"><span data-stu-id="69d51-1330">Renamed `--https-endpoint-access-mode` to `--access-mode`</span></span>
  * <span data-ttu-id="69d51-1331">`--https-endpoint-destination-port` renommé en `--destination-port`</span><span class="sxs-lookup"><span data-stu-id="69d51-1331">Renamed  `--https-endpoint-destination-port` to `--destination-port`</span></span>
* <span data-ttu-id="69d51-1332">[CHANGEMENT CASSANT] Suppression des paramètres pour `application create` :</span><span class="sxs-lookup"><span data-stu-id="69d51-1332">[BREAKING CHANGE] Removed parameters for `application create`:</span></span>
  * `--https-endpoint-location`
  * `--https-endpoint-public-port`
  * `--ssh-endpoint-destination-port`
  * `--ssh-endpoint-location`
  * `--ssh-endpoint-public-port`
* <span data-ttu-id="69d51-1333">MODIFICATION CONSÉQUENTE Renommage de `--target-instance-count` en `--workernode-count` pour `hdinsight resize`</span><span class="sxs-lookup"><span data-stu-id="69d51-1333">[BREAKING CHNAGE] Renamed `--target-instance-count` to `--workernode-count` for `hdinsight resize`</span></span>
* <span data-ttu-id="69d51-1334">[CHANGEMENT CASSANT] Modification de toutes les commandes du groupe `hdinsight script-action` pour utiliser le paramètre `--name` comme nom de l’action de script.</span><span class="sxs-lookup"><span data-stu-id="69d51-1334">[BREAKING CHANGE] Changed all commands in the `hdinsight script-action` group to use the `--name` parameter as the name of the script action.</span></span>
* <span data-ttu-id="69d51-1335">Ajout d’un argument `--cluster-name` à toutes les commandes `hdinsight script-action` pour remplacer l’ancienne fonctionnalité `--name`</span><span class="sxs-lookup"><span data-stu-id="69d51-1335">Added `--cluster-name` argument to all `hdinsight script-action` commands to replace old `--name` functionality</span></span>
* <span data-ttu-id="69d51-1336">[CHANGEMENT CASSANT] Renommage de l’option `--script-execution-id` en `--execution-id` pour toutes les commandes `hdinsight script-action`</span><span class="sxs-lookup"><span data-stu-id="69d51-1336">[BREAKING CHANGE] Renamed `--script-execution-id` to `--execution-id` for all `hdinsight script-action` commands</span></span>
* <span data-ttu-id="69d51-1337">[CHANGEMENT CASSANT] Renommage de `hdinsight script-action show` en `hdinsight script-action show-execution-details`</span><span class="sxs-lookup"><span data-stu-id="69d51-1337">[BREAKING CHANGE] Renamed `hdinsight script-action show` to `hdinsight script-action show-execution-details`</span></span>
* <span data-ttu-id="69d51-1338">[MODIFICATION CONSÉQUENTE] Modification des paramètres sur `hdinsight script-action execute --roles` pour qu’ils soient séparés par des espaces et non par des virgules</span><span class="sxs-lookup"><span data-stu-id="69d51-1338">[BREAKING CHNAGE] Changed parameters to `hdinsight script-action execute --roles` to be space-separated instead of comma-separated</span></span>
* <span data-ttu-id="69d51-1339">[CHANGEMENT CASSANT] Suppression du paramètre `--persisted` de `hdinsight script-action list`</span><span class="sxs-lookup"><span data-stu-id="69d51-1339">[BREAKING CHANGE] Removed the `--persisted` parameter of `hdinsight script-action list`</span></span>
* <span data-ttu-id="69d51-1340">Modification du paramètre `hdinsight create --cluster-configurations` pour qu’il accepte un chemin d’accès à un fichier JSON local ou une chaîne JSON</span><span class="sxs-lookup"><span data-stu-id="69d51-1340">Changed the `hdinsight create --cluster-configurations` parameter to accept a path to a local JSON file or a JSON string</span></span>
* <span data-ttu-id="69d51-1341">Ajout de la commande `hdinsight script-action list-execution-history`</span><span class="sxs-lookup"><span data-stu-id="69d51-1341">Added command `hdinsight script-action list-execution-history`</span></span>
* <span data-ttu-id="69d51-1342">Modification de `hdinsight monitor enable --workspace` pour qu’il accepte un ID ou un nom d’espace de travail Log Analytics</span><span class="sxs-lookup"><span data-stu-id="69d51-1342">Changed `hdinsight monitor enable --workspace` to accept a Log Analytics workspace ID or workspace name</span></span>
* <span data-ttu-id="69d51-1343">Ajout de l’argument `hdinsight monitor enable --primary-key`, qui est nécessaire si un ID d’espace de travail est fourni en tant que paramètre</span><span class="sxs-lookup"><span data-stu-id="69d51-1343">Added the `hdinsight monitor enable --primary-key` argument, which is needed if a workspace ID is provided as the parameter</span></span>
* <span data-ttu-id="69d51-1344">Ajout de plus d’exemples et mise à jour des descriptions des messages d’aide</span><span class="sxs-lookup"><span data-stu-id="69d51-1344">Added more examples and updated descriptions for help messages</span></span>

### <a name="interactive"></a><span data-ttu-id="69d51-1345">Interactive</span><span class="sxs-lookup"><span data-stu-id="69d51-1345">Interactive</span></span>

* <span data-ttu-id="69d51-1346">Résolution d’une erreur de chargement</span><span class="sxs-lookup"><span data-stu-id="69d51-1346">Fixed a loading error</span></span>

### <a name="kubernetes"></a><span data-ttu-id="69d51-1347">Kubernetes</span><span class="sxs-lookup"><span data-stu-id="69d51-1347">Kubernetes</span></span>

* <span data-ttu-id="69d51-1348">Modification pour utiliser `https` si le port du conteneur du tableau de bord utilise `https`</span><span class="sxs-lookup"><span data-stu-id="69d51-1348">Changed to use `https` if dashboard container port is using `https`</span></span>

### <a name="network"></a><span data-ttu-id="69d51-1349">Réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-1349">Network</span></span>

* <span data-ttu-id="69d51-1350">Ajout de l’argument `--yes``network dns record-set cname delete`</span><span class="sxs-lookup"><span data-stu-id="69d51-1350">Added `--yes` argument `network dns record-set cname delete`</span></span>

### <a name="profile"></a><span data-ttu-id="69d51-1351">Profil</span><span class="sxs-lookup"><span data-stu-id="69d51-1351">Profile</span></span>

* <span data-ttu-id="69d51-1352">Ajout de l’argument `--resource-type` à `account get-access-token` pour obtenir des jetons d’accès aux ressources</span><span class="sxs-lookup"><span data-stu-id="69d51-1352">Added `--resource-type` argument to `account get-access-token` to get resource access tokens</span></span>

### <a name="servicefabric"></a><span data-ttu-id="69d51-1353">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="69d51-1353">ServiceFabric</span></span>

* <span data-ttu-id="69d51-1354">Ajout de toutes les versions de système d’exploitation prises en charge pour sf cluster create</span><span class="sxs-lookup"><span data-stu-id="69d51-1354">Added all supported os version for sf cluster create</span></span>
* <span data-ttu-id="69d51-1355">Résolution d’un bogue principal de validation de certificat</span><span class="sxs-lookup"><span data-stu-id="69d51-1355">Fixed primary certificate validation bug</span></span>

### <a name="storage"></a><span data-ttu-id="69d51-1356">Stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-1356">Storage</span></span>

* <span data-ttu-id="69d51-1357">Ajout de la commande `storage copy`</span><span class="sxs-lookup"><span data-stu-id="69d51-1357">Added command `storage copy`</span></span>

## <a name="july-30-2019"></a><span data-ttu-id="69d51-1358">30 juillet 2019</span><span class="sxs-lookup"><span data-stu-id="69d51-1358">July 30, 2019</span></span>

<span data-ttu-id="69d51-1359">Version 2.0.70</span><span class="sxs-lookup"><span data-stu-id="69d51-1359">Version 2.0.70</span></span>

### <a name="acr"></a><span data-ttu-id="69d51-1360">ACR</span><span class="sxs-lookup"><span data-stu-id="69d51-1360">ACR</span></span>

* <span data-ttu-id="69d51-1361">Correction du problème #9952 (régression dans la commande `acr pack build`)</span><span class="sxs-lookup"><span data-stu-id="69d51-1361">Fixed issue #9952 (a regression in the `acr pack build` command)</span></span>
* <span data-ttu-id="69d51-1362">Suppression du nom de l’image du générateur par défaut dans `acr pack build`</span><span class="sxs-lookup"><span data-stu-id="69d51-1362">Removed the default builder image name in `acr pack build`</span></span>

### <a name="appservice"></a><span data-ttu-id="69d51-1363">AppService</span><span class="sxs-lookup"><span data-stu-id="69d51-1363">Appservice</span></span>

* <span data-ttu-id="69d51-1364">Modification de `webapp config ssl` pour afficher un message si une ressource est introuvable</span><span class="sxs-lookup"><span data-stu-id="69d51-1364">Changed `webapp config ssl` to show a message if a resource is not found</span></span>
* <span data-ttu-id="69d51-1365">Correction du problème où `functionapp create` n’acceptait pas le type de compte de stockage `Standard_RAGRS`</span><span class="sxs-lookup"><span data-stu-id="69d51-1365">Fixed issue where `functionapp create` does not accept `Standard_RAGRS` storage account type</span></span>
* <span data-ttu-id="69d51-1366">Correction d’un problème où `webapp up` échouait s’il était exécuté avec des versions antérieures de Python</span><span class="sxs-lookup"><span data-stu-id="69d51-1366">Fixed an issue where `webapp up` would fail if run using older versions of python</span></span>

### <a name="network"></a><span data-ttu-id="69d51-1367">Réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-1367">Network</span></span>

* <span data-ttu-id="69d51-1368">Suppression du paramètre non valide `--ids` de `network nic ip-config add` (correctifs #9861)</span><span class="sxs-lookup"><span data-stu-id="69d51-1368">Removed invalid parameter `--ids` from `network nic ip-config add` (fixes #9861)</span></span>
* <span data-ttu-id="69d51-1369">Correctifs #9604.</span><span class="sxs-lookup"><span data-stu-id="69d51-1369">Fixes #9604.</span></span> <span data-ttu-id="69d51-1370">Ajout du paramètre `--root-certs` à `network application-gateway http-settings [create|update]` pour prendre en charge les certificats racines approuvés associés à l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="69d51-1370">Added `--root-certs` parameter to `network application-gateway http-settings [create|update]` to support user associate trusted root certificates.</span></span>
* <span data-ttu-id="69d51-1371">Correction de l’argument `--subscription` pour `network dns record-set ns create` (#9965)</span><span class="sxs-lookup"><span data-stu-id="69d51-1371">Fixed arguent `--subscription` for `network dns record-set ns create` (#9965)</span></span>

### <a name="rbac"></a><span data-ttu-id="69d51-1372">RBAC</span><span class="sxs-lookup"><span data-stu-id="69d51-1372">RBAC</span></span>

* <span data-ttu-id="69d51-1373">Ajout de la commande `user update`</span><span class="sxs-lookup"><span data-stu-id="69d51-1373">Added `user update` command</span></span>
* <span data-ttu-id="69d51-1374">[DÉPRÉCIATION] Dépréciation de `--upn-or-object-id` des commandes associées à l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="69d51-1374">[DEPRECATED] Deprecated `--upn-or-object-id` from user-related commands</span></span>
    * <span data-ttu-id="69d51-1375">Utiliser l’argument de remplacement `--id`</span><span class="sxs-lookup"><span data-stu-id="69d51-1375">Use replacement argument `--id`</span></span>
* <span data-ttu-id="69d51-1376">Ajout de l’argument `--id` aux commandes associées à l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="69d51-1376">Added `--id` argument to user-related commands</span></span>

### <a name="sql"></a><span data-ttu-id="69d51-1377">SQL</span><span class="sxs-lookup"><span data-stu-id="69d51-1377">SQL</span></span>

* <span data-ttu-id="69d51-1378">Ajout de commandes de gestion pour les clés d’instance managée et le protecteur TDE</span><span class="sxs-lookup"><span data-stu-id="69d51-1378">Added management commands for managed instance keys and TDE protector</span></span>

### <a name="storage"></a><span data-ttu-id="69d51-1379">Stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-1379">Storage</span></span>

* <span data-ttu-id="69d51-1380">Ajout de la commande `storage remove`</span><span class="sxs-lookup"><span data-stu-id="69d51-1380">Added `storage remove` command</span></span>
* <span data-ttu-id="69d51-1381">Correction d’un problème avec `storage blob update`</span><span class="sxs-lookup"><span data-stu-id="69d51-1381">Fixed an issue with `storage blob update`</span></span>

### <a name="vm"></a><span data-ttu-id="69d51-1382">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="69d51-1382">VM</span></span>

* <span data-ttu-id="69d51-1383">Changement de `list-skus` pour utiliser une version API plus récente dans les détails de la zone de sortie</span><span class="sxs-lookup"><span data-stu-id="69d51-1383">Changed `list-skus` to use newer api-version to output zone details</span></span>
* <span data-ttu-id="69d51-1384">Remplacement de la valeur par défaut `--single-placement-group` par `false` pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="69d51-1384">Changed default of `--single-placement-group` to `false` for `vmss create`</span></span>
* <span data-ttu-id="69d51-1385">Ajout de la possibilité de sélectionner des références SKU de stockage ZRS pour `[snapshot|disk] create`</span><span class="sxs-lookup"><span data-stu-id="69d51-1385">Added ability to select ZRS storage SKUs for `[snapshot|disk] create`</span></span>
* <span data-ttu-id="69d51-1386">Ajout d’un nouveau groupe de commandes `vm host` pour prendre en charge des hôtes dédiés</span><span class="sxs-lookup"><span data-stu-id="69d51-1386">Added new command group `vm host` to support dedicated hosts</span></span>
* <span data-ttu-id="69d51-1387">Ajout des paramètres `--host` et `--host-group` sur `vm create` pour définir l’hôte dédié à la machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="69d51-1387">Added parameters `--host` and `--host-group` on `vm create` to set VM dedicated host</span></span>

## <a name="july-16-2019"></a><span data-ttu-id="69d51-1388">16 juillet 2019</span><span class="sxs-lookup"><span data-stu-id="69d51-1388">July 16, 2019</span></span>

<span data-ttu-id="69d51-1389">Version 2.0.69</span><span class="sxs-lookup"><span data-stu-id="69d51-1389">Version 2.0.69</span></span>

### <a name="appservice"></a><span data-ttu-id="69d51-1390">AppService</span><span class="sxs-lookup"><span data-stu-id="69d51-1390">Appservice</span></span>

* <span data-ttu-id="69d51-1391">Changement des commandes `webapp identity` pour retourner un message d’erreur approprié si le nom de ResourceGroupName ou de l’application n’est pas valide</span><span class="sxs-lookup"><span data-stu-id="69d51-1391">Changed `webapp identity` commands to return a proper error message if ResourceGroupName or App name are invalid</span></span>
* <span data-ttu-id="69d51-1392">Correction de `webapp list` pour retourner la valeur correcte pour le nombre de sites si aucun groupe de ressources n’a été fourni</span><span class="sxs-lookup"><span data-stu-id="69d51-1392">Fixed `webapp list` to return the correct value for numberOfSites if no ResourceGroup was provided</span></span>
* <span data-ttu-id="69d51-1393">Correction des effets secondaires de `appservice plan create` et de `webapp create`</span><span class="sxs-lookup"><span data-stu-id="69d51-1393">Fixed side-effects of `appservice plan create` and `webapp create`</span></span>

### <a name="core"></a><span data-ttu-id="69d51-1394">Core</span><span class="sxs-lookup"><span data-stu-id="69d51-1394">Core</span></span>

* <span data-ttu-id="69d51-1395">Résolution du problème où `--subscription` s’affichait alors qu’il ne devait pas</span><span class="sxs-lookup"><span data-stu-id="69d51-1395">Fixed issue where `--subscription` would appear despite being not applicable</span></span>

### <a name="batch"></a><span data-ttu-id="69d51-1396">Batch</span><span class="sxs-lookup"><span data-stu-id="69d51-1396">Batch</span></span>

* <span data-ttu-id="69d51-1397">[CHANGEMENT CASSANT] Remplacement de `batch pool node-agent-skus list` par `batch pool supported-images list`</span><span class="sxs-lookup"><span data-stu-id="69d51-1397">[BREAKING CHANGE] Replaced `batch pool node-agent-skus list` with `batch pool supported-images list`</span></span>
* <span data-ttu-id="69d51-1398">Ajout de la prise en charge des règles de sécurité bloquant l’accès réseau à un pool basé sur le port source du trafic lors de l’utilisation de l’option `--json-file` de `batch pool create network`</span><span class="sxs-lookup"><span data-stu-id="69d51-1398">Added support for security rules blocking network access to a pool based on the source port of the traffic when using the `--json-file` option of `batch pool create network`</span></span>
* <span data-ttu-id="69d51-1399">Ajout de la prise en charge de l’exécution de la tâche dans le répertoire de travail du conteneur ou dans le répertoire de travail de la tâche Batch lors de l’utilisation de l’option `--json-file` de `batch task create`</span><span class="sxs-lookup"><span data-stu-id="69d51-1399">Added support for executing the task in the container working directory or in the Batch task working directory when using the `--json-file` option of `batch task create`</span></span>
* <span data-ttu-id="69d51-1400">Correction d’une erreur dans l’option `--application-package-references` de `batch pool create` où elle fonctionnait uniquement avec les valeurs par défaut</span><span class="sxs-lookup"><span data-stu-id="69d51-1400">Fixed error in `--application-package-references` option of `batch pool create` where it would only work with defaults</span></span>

### <a name="eventhubs"></a><span data-ttu-id="69d51-1401">Eventhubs</span><span class="sxs-lookup"><span data-stu-id="69d51-1401">Eventhubs</span></span>

* <span data-ttu-id="69d51-1402">Ajout d’une validation pour le paramètre `--rights` des commandes `authorizationrule`</span><span class="sxs-lookup"><span data-stu-id="69d51-1402">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="rdbms"></a><span data-ttu-id="69d51-1403">SGBDR</span><span class="sxs-lookup"><span data-stu-id="69d51-1403">RDBMS</span></span>

* <span data-ttu-id="69d51-1404">Ajout d’un paramètre facultatif pour spécifier la référence SKU de réplica pour la commande de création de réplica</span><span class="sxs-lookup"><span data-stu-id="69d51-1404">Added optional parameter to specify replica SKU for create replica command</span></span>
* <span data-ttu-id="69d51-1405">Correction d’un problème d’échec des tests CI lors de la création du réplica MySQL</span><span class="sxs-lookup"><span data-stu-id="69d51-1405">Fixed the issue with CI test failure with creating MySQL replica</span></span>

### <a name="relay"></a><span data-ttu-id="69d51-1406">Relais</span><span class="sxs-lookup"><span data-stu-id="69d51-1406">Relay</span></span>

* <span data-ttu-id="69d51-1407">Correction d’un problème de connexion hybride quand l’autorisation du client est désactivée [#8775](https://github.com/azure/azure-cli/issues/8775)</span><span class="sxs-lookup"><span data-stu-id="69d51-1407">Fixed issue with hybrid connection when client authroization disabled [#8775](https://github.com/azure/azure-cli/issues/8775)</span></span>
* <span data-ttu-id="69d51-1408">Ajout du paramètre `--requires-transport-security` à `relay wcfrelay create`</span><span class="sxs-lookup"><span data-stu-id="69d51-1408">Added parameter `--requires-transport-security` to `relay wcfrelay create`</span></span>

### <a name="servicebus"></a><span data-ttu-id="69d51-1409">Servicebus</span><span class="sxs-lookup"><span data-stu-id="69d51-1409">Servicebus</span></span>

* <span data-ttu-id="69d51-1410">Ajout d’une validation pour le paramètre `--rights` des commandes `authorizationrule`</span><span class="sxs-lookup"><span data-stu-id="69d51-1410">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="storage"></a><span data-ttu-id="69d51-1411">Stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-1411">Storage</span></span>

* <span data-ttu-id="69d51-1412">Activation des fichiers AADDS pour la mise à jour du compte de stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-1412">Enable Files AADDS for storage account update</span></span>
* <span data-ttu-id="69d51-1413">Problème résolu `storage blob service-properties update --set`</span><span class="sxs-lookup"><span data-stu-id="69d51-1413">Fixed issue `storage blob service-properties update --set`</span></span>

## <a name="july-2-2019"></a><span data-ttu-id="69d51-1414">2 juillet 2019</span><span class="sxs-lookup"><span data-stu-id="69d51-1414">July 2, 2019</span></span>

<span data-ttu-id="69d51-1415">Version 2.0.68</span><span class="sxs-lookup"><span data-stu-id="69d51-1415">Version 2.0.68</span></span>

### <a name="core"></a><span data-ttu-id="69d51-1416">Core</span><span class="sxs-lookup"><span data-stu-id="69d51-1416">Core</span></span>

* <span data-ttu-id="69d51-1417">Les modules de commande sont désormais consolidés en un seul distribuable Python.</span><span class="sxs-lookup"><span data-stu-id="69d51-1417">Command modules are now consolidated into a single Python distributable.</span></span> <span data-ttu-id="69d51-1418">L’utilisation directe de nombreux packages `azure-cli-` sur PyPI est donc dépréciée.</span><span class="sxs-lookup"><span data-stu-id="69d51-1418">This deprecates direct use of many `azure-cli-` packages on PyPI.</span></span>
  <span data-ttu-id="69d51-1419">Cela doit réduire la taille de l’installation et affecter uniquement les utilisateurs ayant procédé à une installation directe par le biais de `pip`.</span><span class="sxs-lookup"><span data-stu-id="69d51-1419">This should reduce install size and only affect users who have directly installed via `pip`.</span></span>

### <a name="acr"></a><span data-ttu-id="69d51-1420">ACR</span><span class="sxs-lookup"><span data-stu-id="69d51-1420">ACR</span></span>

* <span data-ttu-id="69d51-1421">Ajout de la prise en charge des déclencheurs de minuteur à la tâche</span><span class="sxs-lookup"><span data-stu-id="69d51-1421">Added support for Timer Triggers to Task</span></span>

### <a name="appservice"></a><span data-ttu-id="69d51-1422">AppService</span><span class="sxs-lookup"><span data-stu-id="69d51-1422">Appservice</span></span>

* <span data-ttu-id="69d51-1423">Modification de `functionapp create` pour activer Application Insights par défaut</span><span class="sxs-lookup"><span data-stu-id="69d51-1423">Changed `functionapp create` to enable application insights by default</span></span>
* <span data-ttu-id="69d51-1424">[CHANGEMENT CASSANT] Suppression de la commande `functionapp devops-build` dépréciée.</span><span class="sxs-lookup"><span data-stu-id="69d51-1424">[BREAKING CHANGE] Removed deprecated `functionapp devops-build` command.</span></span>
  *  <span data-ttu-id="69d51-1425">Utilisez la nouvelle commande `az functionapp devops-pipeline` à la place</span><span class="sxs-lookup"><span data-stu-id="69d51-1425">Use the new command `az functionapp devops-pipeline` instead</span></span>
* <span data-ttu-id="69d51-1426">Ajout de la prise en charge du plan d’application de fonction Consommation Linux à `functionapp deployment config-zip`</span><span class="sxs-lookup"><span data-stu-id="69d51-1426">Added Linux Consumption function app plan support to `functionapp deployment config-zip`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="69d51-1427">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="69d51-1427">Cosmos DB</span></span>

* <span data-ttu-id="69d51-1428">Ajout de la prise en charge de la désactivation de TTL</span><span class="sxs-lookup"><span data-stu-id="69d51-1428">Added support for disabling TTL</span></span>

### <a name="dls"></a><span data-ttu-id="69d51-1429">DLS</span><span class="sxs-lookup"><span data-stu-id="69d51-1429">DLS</span></span>

* <span data-ttu-id="69d51-1430">Mise à jour de la version d’ADLS (0.0.45)</span><span class="sxs-lookup"><span data-stu-id="69d51-1430">Updated ADLS version (0.0.45)</span></span>

### <a name="feedback"></a><span data-ttu-id="69d51-1431">Commentaires</span><span class="sxs-lookup"><span data-stu-id="69d51-1431">Feedback</span></span>

* <span data-ttu-id="69d51-1432">Lors du signalement d’une commande d’extension ayant échoué, `az feedback` tente à présent d’ouvrir le navigateur à l’URL du projet/dépôt de l’extension à partir de l’index</span><span class="sxs-lookup"><span data-stu-id="69d51-1432">When reporting a failed extension command, `az feedback` now attempts to open the browser to the project/repo url of the extension from the index</span></span>

### <a name="hdinsight"></a><span data-ttu-id="69d51-1433">HDInsight</span><span class="sxs-lookup"><span data-stu-id="69d51-1433">HDInsight</span></span>

* <span data-ttu-id="69d51-1434">[CHANGEMENT CASSANT] Remplacement du nom du groupe de commandes `oms` par `monitor`</span><span class="sxs-lookup"><span data-stu-id="69d51-1434">[BREAKING CHANGE] Changed `oms` command group name to `monitor`</span></span>
* <span data-ttu-id="69d51-1435">[CHANGEMENT CASSANT] Paramètre `--http-password/-p` désormais obligatoire</span><span class="sxs-lookup"><span data-stu-id="69d51-1435">[BREAKING CHANGE] Made `--http-password/-p` a required parameter</span></span> 
* <span data-ttu-id="69d51-1436">Ajout de compléteurs pour le compléteur des paramètres `--cluster-admin-account` et `cluster-users-group-dns`</span><span class="sxs-lookup"><span data-stu-id="69d51-1436">Added completers for `--cluster-admin-account` and `cluster-users-group-dns` parameters completer</span></span> 
* <span data-ttu-id="69d51-1437">Paramètre `cluster-users-group-dns` désormais obligatoire quand `—esp` est présent</span><span class="sxs-lookup"><span data-stu-id="69d51-1437">Changed `cluster-users-group-dns` parameter to be required when `—esp` is present</span></span>
* <span data-ttu-id="69d51-1438">Ajout d’un délai d’expiration pour tous les compléteurs automatiques d’arguments existants</span><span class="sxs-lookup"><span data-stu-id="69d51-1438">Added a timeout for all existing argument auto-completers</span></span>
* <span data-ttu-id="69d51-1439">Ajout d’un délai d’expiration pour la transformation d’un nom de ressource en ID de ressource</span><span class="sxs-lookup"><span data-stu-id="69d51-1439">Added a timeout for transforming resource name to resource id</span></span>
* <span data-ttu-id="69d51-1440">Modification des compléteurs automatiques pour sélectionner des ressources à partir de n’importe quel groupe de ressources.</span><span class="sxs-lookup"><span data-stu-id="69d51-1440">Changed Auto-completers to select resources from any resource group.</span></span> <span data-ttu-id="69d51-1441">Le groupe de ressources peut être différent de celui spécifié avec `-g`</span><span class="sxs-lookup"><span data-stu-id="69d51-1441">It can be a different resource group than the one specified with `-g`</span></span>
* <span data-ttu-id="69d51-1442">Ajout de la prise en charge des paramètres `--sub-domain-suffix` et `--disable_gateway_auth` dans la commande `hdinsight application create`</span><span class="sxs-lookup"><span data-stu-id="69d51-1442">Added support for `--sub-domain-suffix` and `--disable_gateway_auth` parameters in the `hdinsight application create` command</span></span>

### <a name="managed-services"></a><span data-ttu-id="69d51-1443">Services gérés</span><span class="sxs-lookup"><span data-stu-id="69d51-1443">Managed Services</span></span>

* <span data-ttu-id="69d51-1444">Introduction du module de commande des services gérés en préversion</span><span class="sxs-lookup"><span data-stu-id="69d51-1444">Introducing managed service command module in preview</span></span>

### <a name="profile"></a><span data-ttu-id="69d51-1445">Profil</span><span class="sxs-lookup"><span data-stu-id="69d51-1445">Profile</span></span>
* <span data-ttu-id="69d51-1446">Suppression de l’argument `--subscription` pour la commande de déconnexion</span><span class="sxs-lookup"><span data-stu-id="69d51-1446">Suppress `--subscription` argument for logout command</span></span>

### <a name="rbac"></a><span data-ttu-id="69d51-1447">RBAC</span><span class="sxs-lookup"><span data-stu-id="69d51-1447">RBAC</span></span>

* <span data-ttu-id="69d51-1448">[CHANGEMENT CASSANT] Suppression de l’argument `--password` pour `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="69d51-1448">[BREAKING CHANGE] Removed `--password` argument for `create-for-rbac`</span></span>
* <span data-ttu-id="69d51-1449">Ajout du paramètre `--assignee-principal-type` à la commande `create` pour éviter les défaillances intermittentes dues à la latence de réplication du serveur de graphique AAD</span><span class="sxs-lookup"><span data-stu-id="69d51-1449">Added `--assignee-principal-type` parameter to `create` command to avoid intermittent failures caused by AAD graph server replication latency</span></span>
* <span data-ttu-id="69d51-1450">Correction d’un incident dans `ad signed-in-user` lors de l’énumération des objets détenus</span><span class="sxs-lookup"><span data-stu-id="69d51-1450">Fixed a crash in `ad signed-in-user` when listing owned objects</span></span>
* <span data-ttu-id="69d51-1451">Correction d’un incident lié au fait que `ad sp` ne trouve pas la bonne application à partir d’un principal de service</span><span class="sxs-lookup"><span data-stu-id="69d51-1451">Fixed issue where `ad sp` would not find the right application from a service principal</span></span>

### <a name="rdbms"></a><span data-ttu-id="69d51-1452">SGBDR</span><span class="sxs-lookup"><span data-stu-id="69d51-1452">RDBMS</span></span>

* <span data-ttu-id="69d51-1453">Ajout de la prise en charge de la réplication pour MariaDB</span><span class="sxs-lookup"><span data-stu-id="69d51-1453">Added support for replication for MariaDB</span></span>

### <a name="sql"></a><span data-ttu-id="69d51-1454">SQL</span><span class="sxs-lookup"><span data-stu-id="69d51-1454">SQL</span></span>

* <span data-ttu-id="69d51-1455">Valeurs autorisées documentées pour `sql db create --sample-name`</span><span class="sxs-lookup"><span data-stu-id="69d51-1455">Documented allowed values for `sql db create --sample-name`</span></span>

### <a name="storage"></a><span data-ttu-id="69d51-1456">Stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-1456">Storage</span></span>

* <span data-ttu-id="69d51-1457">Ajout de la prise en charge des jetons SAS de délégation d’utilisateur avec `--as-user` à `storage blob generate-sas`</span><span class="sxs-lookup"><span data-stu-id="69d51-1457">Added user delegation SAS token support with `--as-user` to `storage blob generate-sas`</span></span> 
* <span data-ttu-id="69d51-1458">Ajout de la prise en charge des jetons SAS de délégation d’utilisateur avec `--as-user` à `storage container generate-sas`</span><span class="sxs-lookup"><span data-stu-id="69d51-1458">Added user delegation SAS token support with `--as-user` to `storage container generate-sas`</span></span> 

### <a name="vm"></a><span data-ttu-id="69d51-1459">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="69d51-1459">VM</span></span>

* <span data-ttu-id="69d51-1460">Correction d’un bogue contraignant `vmss create` à retourner un message d’erreur en cas d’exécution avec `--no-wait`</span><span class="sxs-lookup"><span data-stu-id="69d51-1460">Fixed bug where `vmss create` returns an error message when run with `--no-wait`</span></span>
* <span data-ttu-id="69d51-1461">Suppression de la validation côté client pour `vmss create --single-placement-group`.</span><span class="sxs-lookup"><span data-stu-id="69d51-1461">Removed client-side validation for `vmss create --single-placement-group`.</span></span> <span data-ttu-id="69d51-1462">N’échoue pas si `--single-placement-group` a la valeur `true` et si `--instance-count` est supérieur à 100 ou si des zones de disponibilité sont spécifiées, mais laisse cette validation au service de calcul</span><span class="sxs-lookup"><span data-stu-id="69d51-1462">Does not fail if `--single-placement-group` is set to `true` and`--instance-count` is greater than 100 or availability zones are specified, but leaves this validation to the compute service</span></span>
* <span data-ttu-id="69d51-1463">Correction d’un bogue entraînant l’échec de `[vm|vmss] extension image list` en cas d’utilisation avec `--latest`</span><span class="sxs-lookup"><span data-stu-id="69d51-1463">Fixed bug where `[vm|vmss] extension image list` fails when used with `--latest`</span></span>


## <a name="june-18-2019"></a><span data-ttu-id="69d51-1464">18 juin 2019</span><span class="sxs-lookup"><span data-stu-id="69d51-1464">June 18, 2019</span></span>

<span data-ttu-id="69d51-1465">Version 2.0.67</span><span class="sxs-lookup"><span data-stu-id="69d51-1465">Version 2.0.67</span></span>

### <a name="core"></a><span data-ttu-id="69d51-1466">Core</span><span class="sxs-lookup"><span data-stu-id="69d51-1466">Core</span></span>

<span data-ttu-id="69d51-1467">Cette version introduit une nouvelle étiquette [Préversion] qui permet d’indiquer plus clairement aux clients la présence d’un groupe de commandes, d’une commande ou d’un argument en préversion.</span><span class="sxs-lookup"><span data-stu-id="69d51-1467">This release introduces a new [Preview] tag to more clearly communicate to customers when a command group, command or argument is in preview status.</span></span> <span data-ttu-id="69d51-1468">Auparavant, cet état était mentionné dans le texte de l’aide ou communiqué implicitement par le numéro de version du module de commande.</span><span class="sxs-lookup"><span data-stu-id="69d51-1468">This was previously called out in help text or communicated implicitly by the command module version number.</span></span>
<span data-ttu-id="69d51-1469">À l’avenir, l’interface CLI supprimera les numéros de version des packages individuels.</span><span class="sxs-lookup"><span data-stu-id="69d51-1469">The CLI will be removing version numbers for individual packages in the future.</span></span> <span data-ttu-id="69d51-1470">Si une commande est en préversion, tous ses arguments le sont également.</span><span class="sxs-lookup"><span data-stu-id="69d51-1470">If a command is in preview, all of its arguments are as well.</span></span> <span data-ttu-id="69d51-1471">Si un groupe de commandes est étiqueté comme étant en préversion, toutes les commandes et tous les arguments sont également considérés comme étant en préversion.</span><span class="sxs-lookup"><span data-stu-id="69d51-1471">If a command group is labeled as being in preview, then all commands and arguments are considered to be in preview as well.</span></span>

<span data-ttu-id="69d51-1472">Conséquence de ce changement, plusieurs groupes de commandes peuvent « soudainement » apparaître comme étant en préversion avec cette version.</span><span class="sxs-lookup"><span data-stu-id="69d51-1472">As a result of this change, several command groups may seem to "suddenly" appear to be in a preview status with this release.</span></span> <span data-ttu-id="69d51-1473">En fait, la plupart des packages étaient en préversion, mais ils sont considérés comme étant dans un état de disponibilité générale avec cette version.</span><span class="sxs-lookup"><span data-stu-id="69d51-1473">What actually happened is that most packages were in a preview status, but are being deemed GA with this release</span></span>

### <a name="acr"></a><span data-ttu-id="69d51-1474">ACR</span><span class="sxs-lookup"><span data-stu-id="69d51-1474">ACR</span></span>
* <span data-ttu-id="69d51-1475">Ajout de la commande « acr check-health »</span><span class="sxs-lookup"><span data-stu-id="69d51-1475">Added 'acr check-health' command</span></span>
* <span data-ttu-id="69d51-1476">Amélioration de la gestion des erreurs pour les jetons AAD et pour la récupération des commandes externes</span><span class="sxs-lookup"><span data-stu-id="69d51-1476">Improved error handling for AAD tokens and for retrieving external commands</span></span>

### <a name="acs"></a><span data-ttu-id="69d51-1477">ACS</span><span class="sxs-lookup"><span data-stu-id="69d51-1477">ACS</span></span>
* <span data-ttu-id="69d51-1478">Les commandes ACS dépréciées sont désormais masquées de l’affichage de l’aide</span><span class="sxs-lookup"><span data-stu-id="69d51-1478">Deprecated ACS commands are now hidden from help view</span></span>

### <a name="ams"></a><span data-ttu-id="69d51-1479">AMS</span><span class="sxs-lookup"><span data-stu-id="69d51-1479">AMS</span></span>
* <span data-ttu-id="69d51-1480">[CHANGEMENT CASSANT] Changement apporté pour retourner les chaînes de temps ISO 8601 pour archive-window-length et key-frame-interval-duration</span><span class="sxs-lookup"><span data-stu-id="69d51-1480">[BREAKING CHANGE] Changed to return ISO 8601 time strings for archive-window-length and key-frame-interval-duration</span></span>

### <a name="appservice"></a><span data-ttu-id="69d51-1481">AppService</span><span class="sxs-lookup"><span data-stu-id="69d51-1481">AppService</span></span>
* <span data-ttu-id="69d51-1482">Ajout du routage basé sur l’emplacement pour `webapp deleted list` et `webapp deleted restore`</span><span class="sxs-lookup"><span data-stu-id="69d51-1482">Added location based routing for `webapp deleted list` and `webapp deleted restore`</span></span>
* <span data-ttu-id="69d51-1483">Correction d’un problème lié à l’impossibilité de cliquer sur l’URL cible journalisée d’une application web (« Vous pouvez lancer l’application... ») dans Azure Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="69d51-1483">Fixed issue where webapp up logged target URL ("You can launch the app at...") was not clickable in Azure Cloud Shell</span></span>
* <span data-ttu-id="69d51-1484">Correction d’un problème entraînant l’échec de la création d’applications avec certaines références SKU (erreur AlwaysOn)</span><span class="sxs-lookup"><span data-stu-id="69d51-1484">Fixed an issue where creating apps with the some SKUs was failing with an AlwaysOn error</span></span>
* <span data-ttu-id="69d51-1485">Ajout d’une fonction de prévalidation à `[appservice|webapp] create`</span><span class="sxs-lookup"><span data-stu-id="69d51-1485">Added pre-validation to `[appservice|webapp] create`</span></span>
* <span data-ttu-id="69d51-1486">Correction de `[webapp|functionapp] traffic-routing` de manière à utiliser le bon actionHostName</span><span class="sxs-lookup"><span data-stu-id="69d51-1486">Fixed `[webapp|functionapp] traffic-routing` to use the correct actionHostName</span></span>
* <span data-ttu-id="69d51-1487">Ajout de la prise en charge de l’emplacement aux commandes `functionapp`</span><span class="sxs-lookup"><span data-stu-id="69d51-1487">Added slot support to `functionapp` commands</span></span>

### <a name="batch"></a><span data-ttu-id="69d51-1488">Batch</span><span class="sxs-lookup"><span data-stu-id="69d51-1488">Batch</span></span>
* <span data-ttu-id="69d51-1489">Correction de la régression d’authentification AAD provoquée par un rapport d’erreur trop agressif pour l’authentification par clé partagée</span><span class="sxs-lookup"><span data-stu-id="69d51-1489">Fixed AAD auth regression caused by over-aggressive error reporting for Shared Key Auth</span></span>

### <a name="batchai"></a><span data-ttu-id="69d51-1490">Batch AI</span><span class="sxs-lookup"><span data-stu-id="69d51-1490">BatchAI</span></span>
* <span data-ttu-id="69d51-1491">Les commandes BatchAI sont maintenant dépréciées et masquées</span><span class="sxs-lookup"><span data-stu-id="69d51-1491">BatchAI commands are now deprecated and hidden</span></span>

### <a name="botservice"></a><span data-ttu-id="69d51-1492">BotService</span><span class="sxs-lookup"><span data-stu-id="69d51-1492">BotService</span></span>
* <span data-ttu-id="69d51-1493">Ajout de messages d’avertissement « support interrompu »/« mode maintenance » pour les commandes prenant en charge le SDK v3</span><span class="sxs-lookup"><span data-stu-id="69d51-1493">Added "discontinued support"/"maintenance mode" warning messages for commands that support the v3 SDK</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="69d51-1494">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="69d51-1494">CosmosDB</span></span>
* <span data-ttu-id="69d51-1495">[DÉPRÉCIATION] Dépréciation de la commande `cosmosdb list-keys`</span><span class="sxs-lookup"><span data-stu-id="69d51-1495">[DEPRECATED] Deprecated the `cosmosdb list-keys` command</span></span>
* <span data-ttu-id="69d51-1496">Ajout de la commande `cosmosdb keys list` (remplace `cosmosdb list-keys`)</span><span class="sxs-lookup"><span data-stu-id="69d51-1496">Added the `cosmosdb keys list` command - replaces `cosmosdb list-keys`</span></span>
* <span data-ttu-id="69d51-1497">`cosmsodb create/update`: Ajout d’un nouveau format pour --location afin d’autoriser la définition de la propriété « isZoneRedundant ».</span><span class="sxs-lookup"><span data-stu-id="69d51-1497">`cosmsodb create/update`: Added new format for --location to allow setting "isZoneRedundant" property.</span></span> <span data-ttu-id="69d51-1498">Ancien format déprécié</span><span class="sxs-lookup"><span data-stu-id="69d51-1498">Deprecated old format</span></span>

### <a name="eventgrid"></a><span data-ttu-id="69d51-1499">EventGrid</span><span class="sxs-lookup"><span data-stu-id="69d51-1499">EventGrid</span></span>
* <span data-ttu-id="69d51-1500">Ajout de commandes `eventgrid domain` pour les opérations CRUD liées aux domaines</span><span class="sxs-lookup"><span data-stu-id="69d51-1500">Added `eventgrid domain` commands for domain CRUD operations</span></span>
* <span data-ttu-id="69d51-1501">Ajout de commandes `eventgrid domain topic` pour les opérations CRUD liées aux rubriques de domaine</span><span class="sxs-lookup"><span data-stu-id="69d51-1501">Added `eventgrid domain topic` commands for domain topics CRUD operations</span></span>
* <span data-ttu-id="69d51-1502">Ajout de l’argument `--odata-query` à `eventgrid [topic|event-subscription] list` pour filtrer les résultats à l’aide de la syntaxe OData</span><span class="sxs-lookup"><span data-stu-id="69d51-1502">Added `--odata-query` argument to `eventgrid [topic|event-subscription] list` for filtering results using OData syntax</span></span>
* <span data-ttu-id="69d51-1503">`event-subscription create/update`: Ajout de servicebusqueue comme nouvelle valeur pour le paramètre `--endpoint-type`</span><span class="sxs-lookup"><span data-stu-id="69d51-1503">`event-subscription create/update`: Added servicebusqueue as new values for the `--endpoint-type` parameter</span></span>
* <span data-ttu-id="69d51-1504">[CHANGEMENT CASSANT] Suppression de la prise en charge de `--included-event-types All` avec `eventgrid event-subscription [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69d51-1504">[BREAKING CHANGE] Removed support for `--included-event-types All` with `eventgrid event-subscription [create|update]`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="69d51-1505">HDInsight</span><span class="sxs-lookup"><span data-stu-id="69d51-1505">HDInsight</span></span>
* <span data-ttu-id="69d51-1506">Ajout de la prise en charge du paramètre `--ssh-public-key` dans la commande `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="69d51-1506">Added support for `--ssh-public-key` parameter in `hdinsight create` command</span></span>

### <a name="iot"></a><span data-ttu-id="69d51-1507">IoT</span><span class="sxs-lookup"><span data-stu-id="69d51-1507">IoT</span></span>
* <span data-ttu-id="69d51-1508">Ajout de la prise en charge pour régénérer les clés de stratégie d’autorisation</span><span class="sxs-lookup"><span data-stu-id="69d51-1508">Added support to regenerate authorization policy keys</span></span>
* <span data-ttu-id="69d51-1509">Ajout du SDK et de la prise en charge du service de provisionnement de dépôt DigitalTwin</span><span class="sxs-lookup"><span data-stu-id="69d51-1509">Added SDK and support for DigitalTwin Repository Provisioning Service</span></span>

### <a name="network"></a><span data-ttu-id="69d51-1510">Réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-1510">Network</span></span>
* <span data-ttu-id="69d51-1511">Ajout de la prise en charge de la zone pour NAT Gateway</span><span class="sxs-lookup"><span data-stu-id="69d51-1511">Added Zone support for Nat Gateway</span></span>
* <span data-ttu-id="69d51-1512">Ajout de la commande `network list-service-tags`</span><span class="sxs-lookup"><span data-stu-id="69d51-1512">Added command `network list-service-tags`</span></span>
* <span data-ttu-id="69d51-1513">Correction d’un problème avec `dns zone import` empêchant les utilisateurs d’importer les enregistrements A génériques</span><span class="sxs-lookup"><span data-stu-id="69d51-1513">Fixed issue with `dns zone import` where users could not import wildcard A records</span></span>
* <span data-ttu-id="69d51-1514">Correction d’un problème avec `watcher flow-log configure` empêchant l’activation de la journalisation de flux dans certaines régions</span><span class="sxs-lookup"><span data-stu-id="69d51-1514">Fixed issue with `watcher flow-log configure` where flow logging could not be enabled in certain regions</span></span>

### <a name="resource"></a><span data-ttu-id="69d51-1515">Ressource</span><span class="sxs-lookup"><span data-stu-id="69d51-1515">Resource</span></span>
* <span data-ttu-id="69d51-1516">Ajout de la commande `az rest` pour passer des appels REST</span><span class="sxs-lookup"><span data-stu-id="69d51-1516">Added `az rest` command for making REST calls</span></span>
* <span data-ttu-id="69d51-1517">Correction d’une erreur liée à l’utilisation de `policy assignment list` avec un groupe de ressources ou un niveau d’abonnement `--scope`</span><span class="sxs-lookup"><span data-stu-id="69d51-1517">Fixed error when using `policy assignment list` with a resource group or subscription level `--scope`</span></span>

### <a name="servicebus"></a><span data-ttu-id="69d51-1518">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="69d51-1518">ServiceBus</span></span>
* <span data-ttu-id="69d51-1519">Résolution d’un problème lié à `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span><span class="sxs-lookup"><span data-stu-id="69d51-1519">Fixed issue with `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span></span>

### <a name="sql"></a><span data-ttu-id="69d51-1520">SQL</span><span class="sxs-lookup"><span data-stu-id="69d51-1520">SQL</span></span>
* <span data-ttu-id="69d51-1521">Modification apportée à `--location` pour le rendre facultatif pour `sql [server|mi] create` : utilise l’emplacement du groupe de ressources s’il n’est pas spécifié</span><span class="sxs-lookup"><span data-stu-id="69d51-1521">Changed `--location` to be optional for `sql [server|mi] create` - uses resource group location if not specified</span></span>
* <span data-ttu-id="69d51-1522">Correction de l’erreur « L’objet 'NoneType' n’est pas itérable » pour `sql db list-editions --available`</span><span class="sxs-lookup"><span data-stu-id="69d51-1522">Fixed "'NoneType' object is not iterable" error for `sql db list-editions --available`</span></span>

### <a name="sqlvm"></a><span data-ttu-id="69d51-1523">SQLVm</span><span class="sxs-lookup"><span data-stu-id="69d51-1523">SQLVm</span></span>
* <span data-ttu-id="69d51-1524">[CHANGEMENT CASSANT] Modification de `sql vm create` pour exiger le paramètre `--license-type`</span><span class="sxs-lookup"><span data-stu-id="69d51-1524">[BREAKING CHNAGE] Changed `sql vm create` to require `--license-type` parameter</span></span>
* <span data-ttu-id="69d51-1525">Modification apportée pour autoriser la définition d’une référence SKU d’image SQL lors de la création ou de la mise à jour d’une machine virtuelle SQL</span><span class="sxs-lookup"><span data-stu-id="69d51-1525">Changed to allow setting SQL image SKU when creating or updating a sql vm</span></span>

### <a name="storage"></a><span data-ttu-id="69d51-1526">Stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-1526">Storage</span></span>
* <span data-ttu-id="69d51-1527">Correction d’un problème lié à une clé de compte manquante pour `storage container generate-sas`</span><span class="sxs-lookup"><span data-stu-id="69d51-1527">Fixed issue with missing account key for `storage container generate-sas`</span></span>
* <span data-ttu-id="69d51-1528">Correction d’un problème lié à `storage blob sync` sur Linux</span><span class="sxs-lookup"><span data-stu-id="69d51-1528">Fixed issue with `storage blob sync` on Linux</span></span>

### <a name="vm"></a><span data-ttu-id="69d51-1529">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="69d51-1529">VM</span></span>
* <span data-ttu-id="69d51-1530">[PRÉVERSION] Ajout de commandes `vm image template` pour générer des images de machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="69d51-1530">[PREVIEW] Added `vm image template` commands to build VM images</span></span>

## <a name="june-4-2019"></a><span data-ttu-id="69d51-1531">4 juin 2019</span><span class="sxs-lookup"><span data-stu-id="69d51-1531">June 4, 2019</span></span>

<span data-ttu-id="69d51-1532">Version 2.0.66</span><span class="sxs-lookup"><span data-stu-id="69d51-1532">Version 2.0.66</span></span>

### <a name="core"></a><span data-ttu-id="69d51-1533">Core</span><span class="sxs-lookup"><span data-stu-id="69d51-1533">Core</span></span>
* <span data-ttu-id="69d51-1534">Correction du bogue où des commandes échouent si `--output yaml` est utilisé avec `--query`</span><span class="sxs-lookup"><span data-stu-id="69d51-1534">Fixed bug where commands fail if `--output yaml` is used with `--query`</span></span>

### <a name="acr"></a><span data-ttu-id="69d51-1535">ACR</span><span class="sxs-lookup"><span data-stu-id="69d51-1535">ACR</span></span>
* <span data-ttu-id="69d51-1536">Ajout du groupe de commandes « acr pack » pour la création de tâches de génération rapide à l’aide de Buildpacks.</span><span class="sxs-lookup"><span data-stu-id="69d51-1536">Added 'acr pack' command group for creating quick build Tasks using Buildpacks.</span></span>

### <a name="acs"></a><span data-ttu-id="69d51-1537">ACS</span><span class="sxs-lookup"><span data-stu-id="69d51-1537">ACS</span></span>
* <span data-ttu-id="69d51-1538">Autoriser l’activation/la désactivation du module complémentaire kube-dashboard AKS</span><span class="sxs-lookup"><span data-stu-id="69d51-1538">Allow enabling/disabling AKS kube-dashboard addon</span></span>
* <span data-ttu-id="69d51-1539">Afficher un message convivial lorsque l’abonnement n’est pas autorisé à utiliser Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="69d51-1539">Print a friendly message when the subscription is not whitelisted to use Azure Red Hat OpenShift</span></span>

### <a name="batch"></a><span data-ttu-id="69d51-1540">Batch</span><span class="sxs-lookup"><span data-stu-id="69d51-1540">Batch</span></span>
* <span data-ttu-id="69d51-1541">Amélioration de la gestion des erreurs en l’absence de connexion à un compte \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span><span class="sxs-lookup"><span data-stu-id="69d51-1541">Improved error handling when not logged in to an account \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span></span>

### <a name="iot"></a><span data-ttu-id="69d51-1542">IoT</span><span class="sxs-lookup"><span data-stu-id="69d51-1542">IoT</span></span>
* <span data-ttu-id="69d51-1543">Ajout de la prise en charge du basculement manuel</span><span class="sxs-lookup"><span data-stu-id="69d51-1543">Added support for manual failover</span></span>

### <a name="network"></a><span data-ttu-id="69d51-1544">Réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-1544">Network</span></span>
* <span data-ttu-id="69d51-1545">Ajout de commandes `network application-gateway waf-policy` pour prendre en charge des règles de pare-feu d’applications web personnalisées.</span><span class="sxs-lookup"><span data-stu-id="69d51-1545">Added `network application-gateway waf-policy` commands to support custom WAF rules.</span></span>
* <span data-ttu-id="69d51-1546">Ajout des arguments `--waf-policy` et `--max-capacity` à `network application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69d51-1546">Added `--waf-policy` and `--max-capacity` arguments to `network application-gateway [create|update]`</span></span> 

### <a name="resource"></a><span data-ttu-id="69d51-1547">Ressource</span><span class="sxs-lookup"><span data-stu-id="69d51-1547">Resource</span></span>
* <span data-ttu-id="69d51-1548">Amélioration du message d’erreur émis par la commande `deployment create` quand aucun appareil TTY n’est disponible</span><span class="sxs-lookup"><span data-stu-id="69d51-1548">Improved error message from `deployment create` when there is no TTY available</span></span>

### <a name="role"></a><span data-ttu-id="69d51-1549">Role</span><span class="sxs-lookup"><span data-stu-id="69d51-1549">Role</span></span>
* <span data-ttu-id="69d51-1550">Mise à jour du texte d’aide</span><span class="sxs-lookup"><span data-stu-id="69d51-1550">Updated help text.</span></span>

### <a name="compute"></a><span data-ttu-id="69d51-1551">Calcul</span><span class="sxs-lookup"><span data-stu-id="69d51-1551">Compute</span></span>
* <span data-ttu-id="69d51-1552">Ajout de la prise en charge dans `vm create` des machines virtuelles à partir d’une image managée avec des LUN de disque de données qui ne démarrent pas de 0 ou qui ignorent des nombres</span><span class="sxs-lookup"><span data-stu-id="69d51-1552">Added support to `vm create` for VMs from a managed image with data-disk luns that do not start from 0 or that skip numbers</span></span>

## <a name="may-21-2019"></a><span data-ttu-id="69d51-1553">21 mai 2019</span><span class="sxs-lookup"><span data-stu-id="69d51-1553">May 21, 2019</span></span>

<span data-ttu-id="69d51-1554">Version 2.0.65</span><span class="sxs-lookup"><span data-stu-id="69d51-1554">Version 2.0.65</span></span>

### <a name="core"></a><span data-ttu-id="69d51-1555">Core</span><span class="sxs-lookup"><span data-stu-id="69d51-1555">Core</span></span>
* <span data-ttu-id="69d51-1556">Ajout de meilleurs commentaires pour les erreurs d’authentification</span><span class="sxs-lookup"><span data-stu-id="69d51-1556">Added better feedback for authentication errors</span></span>
* <span data-ttu-id="69d51-1557">Correction d’un problème où l’interface CLI chargeait des extensions qui n’étaient pas compatibles avec sa version principale</span><span class="sxs-lookup"><span data-stu-id="69d51-1557">Fixed issue where the CLI would load extensions that were not compatible with its core version</span></span>
* <span data-ttu-id="69d51-1558">Correction d’un problème lié au lancement lorsque `clouds.config` est endommagé</span><span class="sxs-lookup"><span data-stu-id="69d51-1558">Fixed issue with launching when `clouds.config` is corrupted</span></span>

### <a name="acr"></a><span data-ttu-id="69d51-1559">ACR</span><span class="sxs-lookup"><span data-stu-id="69d51-1559">ACR</span></span>
* <span data-ttu-id="69d51-1560">Ajout de la prise en charge des identités managées aux tâches</span><span class="sxs-lookup"><span data-stu-id="69d51-1560">Added support for Managed Identities to Tasks</span></span>

### <a name="acs"></a><span data-ttu-id="69d51-1561">ACS</span><span class="sxs-lookup"><span data-stu-id="69d51-1561">ACS</span></span>
* <span data-ttu-id="69d51-1562">Correction de la commande `openshift create` lorsqu’elle est utilisée avec le client AAD du client</span><span class="sxs-lookup"><span data-stu-id="69d51-1562">Fixed `openshift create` command when used with customer AAD client</span></span>

### <a name="appservice"></a><span data-ttu-id="69d51-1563">AppService</span><span class="sxs-lookup"><span data-stu-id="69d51-1563">AppService</span></span>
* <span data-ttu-id="69d51-1564">[DÉPRÉCIATION] Commande `functionapp devops-build` dépréciée (Elle sera supprimée de la prochaine version)</span><span class="sxs-lookup"><span data-stu-id="69d51-1564">[DEPRECATED] Deprecated `functionapp devops-build` command - will be removed in next release</span></span>
* <span data-ttu-id="69d51-1565">Changement apporté à `functionapp devops-pipeline` pour extraire un journal de génération d’Azure DevOps en mode détaillé</span><span class="sxs-lookup"><span data-stu-id="69d51-1565">Changed `functionapp devops-pipeline` to fetch build log from Azure DevOps in verbose mode</span></span>
* <span data-ttu-id="69d51-1566">[CHANGEMENT CASSANT] Suppression de l’indicateur `--use_local_settings` de la commande `functionapp devops-pipeline` (aucune opération)</span><span class="sxs-lookup"><span data-stu-id="69d51-1566">[BREAKING CHANGE] Removed `--use_local_settings` flag from `functionapp devops-pipeline` command - was a no-op</span></span>
* <span data-ttu-id="69d51-1567">Changement apporté à `webapp up` pour retourner une sortie JSON si `--logs` n’est pas utilisé</span><span class="sxs-lookup"><span data-stu-id="69d51-1567">Changed `webapp up` to return JSON output if `--logs` is not used</span></span>
* <span data-ttu-id="69d51-1568">Ajout de la prise en charge de l’écriture de ressources par défaut à la configuration locale pour `webapp up`</span><span class="sxs-lookup"><span data-stu-id="69d51-1568">Added support for writing default resources to local config for `webapp up`</span></span>
* <span data-ttu-id="69d51-1569">Ajout de la prise en charge à `webapp up` pour redéployer une application sans utiliser l’argument `--location`</span><span class="sxs-lookup"><span data-stu-id="69d51-1569">Added support to `webapp up` for redeploying an app without using the `--location` argument</span></span>
* <span data-ttu-id="69d51-1570">Résolution d’un problème où, lors de la création ASP de la référence SKU Gratuite, la valeur de référence Gratuit ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="69d51-1570">Fixed an issue where for Linux Free SKU ASP creation use Free as SKU value was not working</span></span>

### <a name="botservice"></a><span data-ttu-id="69d51-1571">BotService</span><span class="sxs-lookup"><span data-stu-id="69d51-1571">BotService</span></span>
* <span data-ttu-id="69d51-1572">Modification autorisant toutes les casses pour les paramètres `--lang` des commandes</span><span class="sxs-lookup"><span data-stu-id="69d51-1572">Changed to allow all casing for `--lang` parameters for commands</span></span>
* <span data-ttu-id="69d51-1573">Mise à jour de la description du module de commande</span><span class="sxs-lookup"><span data-stu-id="69d51-1573">Updated description for command module</span></span>

### <a name="consumption"></a><span data-ttu-id="69d51-1574">Consommation</span><span class="sxs-lookup"><span data-stu-id="69d51-1574">Consumption</span></span>
* <span data-ttu-id="69d51-1575">Ajout du paramètre obligatoire manquant lors de l’exécution de `consumption usage list --billing-period-name`</span><span class="sxs-lookup"><span data-stu-id="69d51-1575">Added missing required parameter when running `consumption usage list --billing-period-name`</span></span>

### <a name="iot"></a><span data-ttu-id="69d51-1576">IoT</span><span class="sxs-lookup"><span data-stu-id="69d51-1576">IoT</span></span>
* <span data-ttu-id="69d51-1577">Ajout de la prise en charge permettant de répertorier toutes les clés</span><span class="sxs-lookup"><span data-stu-id="69d51-1577">Added support to list all keys</span></span>

### <a name="network"></a><span data-ttu-id="69d51-1578">Réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-1578">Network</span></span>
* [CHANGEMENT CASSANT]: Removed `network interface-endpoints` command group - use `network private-endpoints`
[BREAKING CHANGE]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* <span data-ttu-id="69d51-1580">Ajout de l’argument `--nat-gateway` à `network vnet subnet [create|update]` pour attacher à une passerelle NAT</span><span class="sxs-lookup"><span data-stu-id="69d51-1580">Added `--nat-gateway` argument to `network vnet subnet [create|update]` for attaching to a NAT gateway</span></span>
* <span data-ttu-id="69d51-1581">Correction d’un problème avec `dns zone import` où les noms d’enregistrement pouvaient ne pas correspondre à un type d’enregistrement</span><span class="sxs-lookup"><span data-stu-id="69d51-1581">Fixed issue with `dns zone import` where record names could not match a record type</span></span>

### <a name="rdbms"></a><span data-ttu-id="69d51-1582">SGBDR</span><span class="sxs-lookup"><span data-stu-id="69d51-1582">RDBMS</span></span>
* <span data-ttu-id="69d51-1583">Ajout de la prise en charge de MySQL et Postgres pour la géoréplication</span><span class="sxs-lookup"><span data-stu-id="69d51-1583">Added postgres and mysql support for geo replication</span></span>

### <a name="rbac"></a><span data-ttu-id="69d51-1584">RBAC</span><span class="sxs-lookup"><span data-stu-id="69d51-1584">RBAC</span></span>
* <span data-ttu-id="69d51-1585">Ajout de la prise en charge de l’étendue du groupe de gestion dans `role assignment`</span><span class="sxs-lookup"><span data-stu-id="69d51-1585">Added support for management group scope to `role assignment`</span></span>

### <a name="storage"></a><span data-ttu-id="69d51-1586">Stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-1586">Storage</span></span>
* <span data-ttu-id="69d51-1587">`storage blob sync` : ajout de la commande de synchronisation pour le blob de stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-1587">`storage blob sync`: add sync command for storage blob</span></span>

### <a name="compute"></a><span data-ttu-id="69d51-1588">Calcul</span><span class="sxs-lookup"><span data-stu-id="69d51-1588">Compute</span></span>
* <span data-ttu-id="69d51-1589">Ajout de `--computer-name` à `vm create` pour définir le nom d’une machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="69d51-1589">Added `--computer-name` to `vm create` for setting a VM's computer name</span></span>
* <span data-ttu-id="69d51-1590">`--ssh-key-value` renommé en `--ssh-key-values` pour `[vm|vmss] create` - peut maintenant accepter plusieurs chemins d’accès ou valeurs de clé publique SSH</span><span class="sxs-lookup"><span data-stu-id="69d51-1590">Renamed `--ssh-key-value` renamed to `--ssh-key-values` for `[vm|vmss] create` - can now accept multiple ssh public key values or paths</span></span>
  * <span data-ttu-id="69d51-1591">__Remarque__ : il ne s’agit **pas** d’un changement cassant - `--ssh-key-value` sera analysé correctement, car il correspond uniquement à `--ssh-key-values`</span><span class="sxs-lookup"><span data-stu-id="69d51-1591">__Note__: This is **not** a breaking change - `--ssh-key-value` will be parsed correctly as it matches only `--ssh-key-values`</span></span>
* <span data-ttu-id="69d51-1592">Modification de l’argument `--type` qui devient facultatif dans `ppg create`</span><span class="sxs-lookup"><span data-stu-id="69d51-1592">Changed the `--type` argument of `ppg create` to be optional</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="69d51-1593">6 mai 2019</span><span class="sxs-lookup"><span data-stu-id="69d51-1593">May 6, 2019</span></span>

<span data-ttu-id="69d51-1594">Version 2.0.64</span><span class="sxs-lookup"><span data-stu-id="69d51-1594">Version 2.0.64</span></span>

### <a name="acs"></a><span data-ttu-id="69d51-1595">ACS</span><span class="sxs-lookup"><span data-stu-id="69d51-1595">ACS</span></span>
* <span data-ttu-id="69d51-1596">[CHANGEMENT CASSANT] Suppression de l’indicateur `--fqdn` sur les commandes `openshift`</span><span class="sxs-lookup"><span data-stu-id="69d51-1596">[BREAKING CHANGE] Removed `--fqdn` flag on `openshift` commands</span></span>
* <span data-ttu-id="69d51-1597">Modification permettant d’utiliser la version d’API en disponibilité générale d’Azure Red Hat Openshift</span><span class="sxs-lookup"><span data-stu-id="69d51-1597">Changed to use Azure Red Hat Openshift GA API Version</span></span>
* <span data-ttu-id="69d51-1598">Ajout de l’indicateur `customer-admin-group-id` à `openshift create`</span><span class="sxs-lookup"><span data-stu-id="69d51-1598">Added `customer-admin-group-id` flag to `openshift create`</span></span>
* <span data-ttu-id="69d51-1599">[Mise à la disposition générale] Suppression de `(PREVIEW)` de l’option `aks create``--network-policy`</span><span class="sxs-lookup"><span data-stu-id="69d51-1599">[GA] Removed `(PREVIEW)` from `aks create` option `--network-policy`</span></span>

### <a name="appservice"></a><span data-ttu-id="69d51-1600">AppService</span><span class="sxs-lookup"><span data-stu-id="69d51-1600">Appservice</span></span>
* <span data-ttu-id="69d51-1601">[DÉPRÉCIATION] Commande `functionapp devops-build` dépréciée</span><span class="sxs-lookup"><span data-stu-id="69d51-1601">[DEPRECATED] Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="69d51-1602">Renommée `functionapp devops-pipeline`</span><span class="sxs-lookup"><span data-stu-id="69d51-1602">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="69d51-1603">Correction du processus d’obtention du nom d’utilisateur pour Cloud Shell qui provoquait l’échec de `webapp up`</span><span class="sxs-lookup"><span data-stu-id="69d51-1603">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="69d51-1604">Mise à jour de la documentation `appservice plan --sku` pour refléter les plans App Service pris en charge</span><span class="sxs-lookup"><span data-stu-id="69d51-1604">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="69d51-1605">Ajout d’arguments facultatifs pour le groupe et le plan de ressources à `webapp up`</span><span class="sxs-lookup"><span data-stu-id="69d51-1605">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="69d51-1606">Ajout de dispositifs de prise en charge à `webapp ssh` pour respecter la variable d’environnement `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`</span><span class="sxs-lookup"><span data-stu-id="69d51-1606">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="69d51-1607">Ajout de la prise en charge de `appserviceplan create` pour la référence SKU Linux gratuite</span><span class="sxs-lookup"><span data-stu-id="69d51-1607">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="69d51-1608">Mise en veille de 30 s de `webapp up` après la définition de `SCM_DO_BUILD_DURING_DEPLOYMENT=true` pour gérer le démarrage à froid de kudu</span><span class="sxs-lookup"><span data-stu-id="69d51-1608">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="69d51-1609">Ajout de la prise en charge du runtime `powershell` à `functionapp create` sur Windows</span><span class="sxs-lookup"><span data-stu-id="69d51-1609">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="69d51-1610">Ajout de la commande `create-remote-connection`</span><span class="sxs-lookup"><span data-stu-id="69d51-1610">Added `create-remote-connection` command</span></span>

### <a name="batch"></a><span data-ttu-id="69d51-1611">Batch</span><span class="sxs-lookup"><span data-stu-id="69d51-1611">Batch</span></span>
* <span data-ttu-id="69d51-1612">Correction du bogue dans le validateur pour les options `--application-package-references`</span><span class="sxs-lookup"><span data-stu-id="69d51-1612">Fixed bug in validator for `--application-package-references` options</span></span>

### <a name="botservice"></a><span data-ttu-id="69d51-1613">Botservice</span><span class="sxs-lookup"><span data-stu-id="69d51-1613">Botservice</span></span>
* <span data-ttu-id="69d51-1614">[CHANGEMENT CASSANT] Modification apportée à `bot create -v v4 -k webapp` pour créer un bot d’application web vide par défaut (autrement dit, aucun bot n’est déployé sur App Service)</span><span class="sxs-lookup"><span data-stu-id="69d51-1614">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to create an empty Web App Bot by default (i.e. no bot is deployed to the App Service)</span></span>
* <span data-ttu-id="69d51-1615">Ajout de l’indicateur `--echo` à `bot create` pour utiliser l’ancien comportement avec `-v v4`</span><span class="sxs-lookup"><span data-stu-id="69d51-1615">Added `--echo` flag to `bot create` to use the old behavior with `-v v4`</span></span>
* <span data-ttu-id="69d51-1616">[CHANGEMENT CASSANT] Modification de la valeur par défaut de `--version` qui devient `v4`</span><span class="sxs-lookup"><span data-stu-id="69d51-1616">[BREAKING CHANGE] Changed the default value of  `--version` to `v4`</span></span>
  * <span data-ttu-id="69d51-1617">__REMARQUE :__ `bot prepare-publish` utilise toujours son ancienne valeur par défaut</span><span class="sxs-lookup"><span data-stu-id="69d51-1617">__NOTE:__ `bot prepare-publish` still uses the its old default</span></span>
* <span data-ttu-id="69d51-1618">[CHANGEMENT CASSANT] Modification de `--lang` qui n’a plus la valeur par défaut `Csharp`.</span><span class="sxs-lookup"><span data-stu-id="69d51-1618">[BREAKING CHANGE] Changed `--lang` to no longer default to `Csharp`.</span></span> <span data-ttu-id="69d51-1619">Si la commande nécessite `--lang` et que celui-ci n’est pas fourni, la commande génère à présent une erreur</span><span class="sxs-lookup"><span data-stu-id="69d51-1619">If the command requires `--lang` and it is not provided, the command will now error out</span></span>
* <span data-ttu-id="69d51-1620">[CHANGEMENT CASSANT] Modification des arguments `--appid` et `--password` de `bot create` afin que ceux-ci soient requis et puisse maintenant être créés via `ad app create`</span><span class="sxs-lookup"><span data-stu-id="69d51-1620">[BREAKING CHANGE] Changed the `--appid` and `--password` args for `bot create` to be required and can now be created via `ad app create`</span></span>
* <span data-ttu-id="69d51-1621">Ajout de la validation `--appid` et `--password`</span><span class="sxs-lookup"><span data-stu-id="69d51-1621">Added `--appid` and `--password` validation</span></span>
* <span data-ttu-id="69d51-1622">[CHANGEMENT CASSANT] Modification apportée à la commande `bot create -v v4` afin qu’elle ne crée ni n’utilise un compte de stockage ou Application Insights</span><span class="sxs-lookup"><span data-stu-id="69d51-1622">[BREAKING CHANGE] Changed `bot create -v v4` to not create or use a Storage Account or Application Insights</span></span>
* <span data-ttu-id="69d51-1623">[CHANGEMENT CASSANT] Modification de `bot create -v v3` pour exiger une région où Application Insights est disponible</span><span class="sxs-lookup"><span data-stu-id="69d51-1623">[BREAKING CHANGE] Changed `bot create -v v3` to require a region where Application Insights is available</span></span>
* <span data-ttu-id="69d51-1624">[CHANGEMENT CASSANT] Modification de `bot update` qui affecte maintenant uniquement les propriétés spécifiques d’un bot</span><span class="sxs-lookup"><span data-stu-id="69d51-1624">[BREAKING CHANGE] Changed `bot update` to now affect only specific properties of a bot</span></span>
* <span data-ttu-id="69d51-1625">[CHANGEMENT CASSANT] Modification des indicateurs `--lang` qui acceptent `Javascript` au lieu de `Node`</span><span class="sxs-lookup"><span data-stu-id="69d51-1625">[BREAKING CHANGE] Changed `--lang` flags to accept `Javascript` instead of `Node`</span></span>
* <span data-ttu-id="69d51-1626">[CHANGEMENT CASSANT] Suppression de `Node` comme valeur `--lang` autorisée</span><span class="sxs-lookup"><span data-stu-id="69d51-1626">[BREAKING CHANGE] Removed `Node` as an allowed `--lang` value</span></span>
* <span data-ttu-id="69d51-1627">[CHANGEMENT CASSANT] Modification de `bot create -v v4 -k webapp` afin que `SCM_DO_BUILD_DURING_DEPLOYMENT` ne soit plus défini sur True.</span><span class="sxs-lookup"><span data-stu-id="69d51-1627">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to no longer set `SCM_DO_BUILD_DURING_DEPLOYMENT` to true.</span></span> <span data-ttu-id="69d51-1628">Tous les déploiements via Kudu agissent conformément à leur comportement par défaut</span><span class="sxs-lookup"><span data-stu-id="69d51-1628">All deployments through Kudu will act according to their default behavior</span></span>
* <span data-ttu-id="69d51-1629">Modification de la commande `bot download` pour des bots sans fichiers `.bot` afin de créer le fichier de configuration spécifique à une langue avec des valeurs de paramètres d’application pour le bot</span><span class="sxs-lookup"><span data-stu-id="69d51-1629">Changed `bot download` for bots without `.bot` files to create the language-specific configuration file with values from the Application Settings for the bot</span></span>
* <span data-ttu-id="69d51-1630">Ajout de la prise en charge de `Typescript` pour `bot prepare-deploy`</span><span class="sxs-lookup"><span data-stu-id="69d51-1630">Added `Typescript` support to `bot prepare-deploy`</span></span>
* <span data-ttu-id="69d51-1631">Ajout du message d’avertissement à `bot prepare-deploy` pour les bots `Javascript` et `Typescript` quand `--code-dir` ne contient pas `package.json`</span><span class="sxs-lookup"><span data-stu-id="69d51-1631">Added warning message to `bot prepare-deploy` for `Javascript` and `Typescript` bots for when `--code-dir` does not contain `package.json`</span></span>
* <span data-ttu-id="69d51-1632">Modification de `bot prepare-deploy` qui retourne `true` en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="69d51-1632">Changed `bot prepare-deploy` to return `true` if successful</span></span>
* <span data-ttu-id="69d51-1633">Ajout de la journalisation commentée à `bot prepare-deploy`</span><span class="sxs-lookup"><span data-stu-id="69d51-1633">Added verbose logging to `bot prepare-deploy`</span></span>
* <span data-ttu-id="69d51-1634">Ajout d’un plus grand nombre de régions Application Insights disponibles dans `az bot create -v v3`</span><span class="sxs-lookup"><span data-stu-id="69d51-1634">Added more available Application Insights regions to `az bot create -v v3`</span></span>

### <a name="configure"></a><span data-ttu-id="69d51-1635">Configurer</span><span class="sxs-lookup"><span data-stu-id="69d51-1635">Configure</span></span>
* <span data-ttu-id="69d51-1636">Ajout de la prise en charge des configurations de valeur par défaut d’argument en fonction d’un dossier</span><span class="sxs-lookup"><span data-stu-id="69d51-1636">Added support for folder based argument default value configurations</span></span>

### <a name="eventhubs"></a><span data-ttu-id="69d51-1637">Eventhubs</span><span class="sxs-lookup"><span data-stu-id="69d51-1637">Eventhubs</span></span>
* <span data-ttu-id="69d51-1638">Ajout des commandes `namespace network-rule`</span><span class="sxs-lookup"><span data-stu-id="69d51-1638">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="69d51-1639">Ajout de l’argument `--default-action` pour les règles réseau à `namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69d51-1639">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="69d51-1640">Réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-1640">Network</span></span>
* <span data-ttu-id="69d51-1641">[CHANGEMENT CASSANT] Remplacement de l’argument `--cache` par `--defer` pour `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69d51-1641">[BREAKING CHANGE] Replaced `--cache` arugment with `--defer` for `vnet [create|update]`</span></span> 

### <a name="policy-insights"></a><span data-ttu-id="69d51-1642">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="69d51-1642">Policy Insights</span></span>
* <span data-ttu-id="69d51-1643">Ajout de la prise en charge pour `--expand PolicyEvaluationDetails` pour interroger les détails de l’évaluation de stratégie sur la ressource</span><span class="sxs-lookup"><span data-stu-id="69d51-1643">Added support for `--expand PolicyEvaluationDetails` to query policy evaluation details on the resource</span></span>

### <a name="role"></a><span data-ttu-id="69d51-1644">Role</span><span class="sxs-lookup"><span data-stu-id="69d51-1644">Role</span></span>
* <span data-ttu-id="69d51-1645">[DÉPRÉCIATION] Changement apporté à `create-for-rbac` concernant le masquage de l’argument '--password' - Fin de la prise en charge en mai 2019</span><span class="sxs-lookup"><span data-stu-id="69d51-1645">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

### <a name="service-bus"></a><span data-ttu-id="69d51-1646">Service Bus</span><span class="sxs-lookup"><span data-stu-id="69d51-1646">Service Bus</span></span>
* <span data-ttu-id="69d51-1647">Ajout des commandes `namespace network-rule`</span><span class="sxs-lookup"><span data-stu-id="69d51-1647">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="69d51-1648">Ajout de l’argument `--default-action` pour les règles réseau à `namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69d51-1648">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>
* <span data-ttu-id="69d51-1649">Correction de `topic [create|update]` qui autorise `--max-size` à prendre en charge les valeurs 10, 20, 40 et 80 Go avec la référence SKU Premium</span><span class="sxs-lookup"><span data-stu-id="69d51-1649">Fixed `topic [create|update]` to allow `--max-size` support for 10, 20, 40 and 80GB values with premium SKU</span></span>

### <a name="sql"></a><span data-ttu-id="69d51-1650">SQL</span><span class="sxs-lookup"><span data-stu-id="69d51-1650">SQL</span></span>
* <span data-ttu-id="69d51-1651">Ajout des commandes `sql virtual-cluster [list|show|delete]`</span><span class="sxs-lookup"><span data-stu-id="69d51-1651">Added `sql virtual-cluster [list|show|delete]` commands</span></span>

### <a name="vm"></a><span data-ttu-id="69d51-1652">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="69d51-1652">VM</span></span>
* <span data-ttu-id="69d51-1653">Ajout de `--protect-from-scale-in` et `--protect-from-scale-set-actions` à `vmss update` pour activer les mises à jour de la stratégie de protection des instances de machine virtuelle VMSS</span><span class="sxs-lookup"><span data-stu-id="69d51-1653">Added `--protect-from-scale-in` and `--protect-from-scale-set-actions` to `vmss update` to enable updates to the protection policy of VMSS VM instances</span></span>
* <span data-ttu-id="69d51-1654">Ajout de `--instance-id` à `vmss update` pour activer la mise à jour générique des instances de machine virtuelle VMSS</span><span class="sxs-lookup"><span data-stu-id="69d51-1654">Added `--instance-id` to `vmss update` to enable generic update of VMSS VM instances</span></span>
* <span data-ttu-id="69d51-1655">Ajout de `--instance-id` à `vmss wait`</span><span class="sxs-lookup"><span data-stu-id="69d51-1655">Added `--instance-id` to `vmss wait`</span></span>
* <span data-ttu-id="69d51-1656">Ajout du nouveau groupe de commandes `ppg` pour gérer les groupes de placements de proximité</span><span class="sxs-lookup"><span data-stu-id="69d51-1656">Added new `ppg` command group for managing Proximity Placement Groups</span></span>
* <span data-ttu-id="69d51-1657">Ajout de `--ppg` à `[vm|vmss] create` et `vm availability-set create` pour la gestion des groupes de placements de proximité</span><span class="sxs-lookup"><span data-stu-id="69d51-1657">Added `--ppg` to `[vm|vmss] create` and `vm availability-set create` for managing PPGs</span></span>
* <span data-ttu-id="69d51-1658">Ajout du paramètre `--hyper-v-generation` pour `image create`</span><span class="sxs-lookup"><span data-stu-id="69d51-1658">Added `--hyper-v-generation` parameter to `image create`</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="69d51-1659">23 avril 2019</span><span class="sxs-lookup"><span data-stu-id="69d51-1659">April 23, 2019</span></span>

<span data-ttu-id="69d51-1660">Version 2.0.63</span><span class="sxs-lookup"><span data-stu-id="69d51-1660">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="69d51-1661">ACS</span><span class="sxs-lookup"><span data-stu-id="69d51-1661">ACS</span></span>
* <span data-ttu-id="69d51-1662">Changement apporté à `aks get-credentials` pour demander confirmation en cas de remplacement de valeurs dupliquées</span><span class="sxs-lookup"><span data-stu-id="69d51-1662">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="69d51-1663">Suppression de `(PREVIEW)` des commandes Dev Spaces « aks use-dev-spaces » et « aks remove-dev-spaces »</span><span class="sxs-lookup"><span data-stu-id="69d51-1663">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="69d51-1664">AMS</span><span class="sxs-lookup"><span data-stu-id="69d51-1664">AMS</span></span>
* <span data-ttu-id="69d51-1665">Correction d’un bogue lié à la mise à jour des filtres de composant et de compte</span><span class="sxs-lookup"><span data-stu-id="69d51-1665">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="69d51-1666">AppService</span><span class="sxs-lookup"><span data-stu-id="69d51-1666">AppService</span></span>
* <span data-ttu-id="69d51-1667">Ajout de la prise en charge d’ASE et de délais d’expiration à `webapp ssh`</span><span class="sxs-lookup"><span data-stu-id="69d51-1667">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="69d51-1668">Ajout de la prise en charge de l’établissement de CI/CD dans un pipeline Azure DevOps entre un dépôt Github et des applications de fonction</span><span class="sxs-lookup"><span data-stu-id="69d51-1668">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="69d51-1669">Ajout de l’argument `--github-pat` à `functionapp devops-build create` pour accepter un jeton d’accès personnel Github</span><span class="sxs-lookup"><span data-stu-id="69d51-1669">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="69d51-1670">Ajout de l’argument `--github-repository` à `functionapp devops-build create` pour accepter un dépôt Github contenant le code source d’une application de fonction</span><span class="sxs-lookup"><span data-stu-id="69d51-1670">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="69d51-1671">Résolution d’un problème provoquant l’échec de `az webapp up --logs` avec une erreur et la mise à jour de la version par défaut NETCORE avec la version 2.1</span><span class="sxs-lookup"><span data-stu-id="69d51-1671">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="69d51-1672">Suppression des paramètres d’application de fonction inutiles lors de la création d’une telle application avec un plan de consommation</span><span class="sxs-lookup"><span data-stu-id="69d51-1672">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="69d51-1673">Changement apporté à `webapp up` pour ajouter un numéro à la fin de la chaîne asp par défaut afin de créer un ASP basé sur les options de la référence SKU</span><span class="sxs-lookup"><span data-stu-id="69d51-1673">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="69d51-1674">Ajout de `-b` en tant qu’option à `webapp up` pour lancer l’application dans le navigateur</span><span class="sxs-lookup"><span data-stu-id="69d51-1674">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="69d51-1675">Changement apporté à `webapp deployment source config zip` pour gérer la variable d’environnement `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`</span><span class="sxs-lookup"><span data-stu-id="69d51-1675">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="69d51-1676">Deployment Manager</span><span class="sxs-lookup"><span data-stu-id="69d51-1676">Deployment Manager</span></span>
* <span data-ttu-id="69d51-1677">[PRÉVERSION] Création et gestion d’artefacts prenant en charge les lancements</span><span class="sxs-lookup"><span data-stu-id="69d51-1677">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="69d51-1678">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="69d51-1678">Lab</span></span>
* <span data-ttu-id="69d51-1679">Correction d’un bogue provoquant une sortie anticipée</span><span class="sxs-lookup"><span data-stu-id="69d51-1679">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="69d51-1680">Réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-1680">Network</span></span>
* <span data-ttu-id="69d51-1681">Ajout d’une délégation de serveurs nommés automatiquement à `dns zone create` dans le parent durant la création d’une zone enfant</span><span class="sxs-lookup"><span data-stu-id="69d51-1681">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="69d51-1682">Ressource</span><span class="sxs-lookup"><span data-stu-id="69d51-1682">Resource</span></span>
* <span data-ttu-id="69d51-1683">[DÉPRÉCIATION] Dépréciation des arguments `--link-id`, `--target-id` et `--filter-string` de `resource link`</span><span class="sxs-lookup"><span data-stu-id="69d51-1683">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="69d51-1684">Arguments remplacés par `--link`, `--target` et `--filter`</span><span class="sxs-lookup"><span data-stu-id="69d51-1684">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="69d51-1685">Correction d’un problème empêchant le fonctionnement des commandes `resource link [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69d51-1685">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="69d51-1686">Correction d’un problème où une suppression effectuée à l’aide d’un ID de ressource pouvait entraîner un plantage en cas d’erreur</span><span class="sxs-lookup"><span data-stu-id="69d51-1686">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="69d51-1687">SQL</span><span class="sxs-lookup"><span data-stu-id="69d51-1687">SQL</span></span>
* <span data-ttu-id="69d51-1688">Ajout de la prise en charge d’un fuseau horaire personnalisé sur les instances managées</span><span class="sxs-lookup"><span data-stu-id="69d51-1688">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="69d51-1689">Changement apporté pour autoriser l’utilisation d’un nom de pool élastique avec `sql db update`</span><span class="sxs-lookup"><span data-stu-id="69d51-1689">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="69d51-1690">Ajout de la prise en charge de `--no-wait` pour `sql server [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69d51-1690">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="69d51-1691">Ajout de la commande `sql server wait`</span><span class="sxs-lookup"><span data-stu-id="69d51-1691">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="69d51-1692">Stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-1692">Storage</span></span>
* <span data-ttu-id="69d51-1693">Résolution du problème lié aux jetons SAS à double encodage dans `storage blob generate-sas`</span><span class="sxs-lookup"><span data-stu-id="69d51-1693">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="69d51-1694">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="69d51-1694">VM</span></span>
* <span data-ttu-id="69d51-1695">Ajout de l’indicateur `--skip-shutdown` à `vm|vmss stop` pour mettre hors tension les machines virtuelles sans les arrêter</span><span class="sxs-lookup"><span data-stu-id="69d51-1695">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="69d51-1696">Ajout de l’argument `--storage-account-type` à `sig image-version create` pour définir le type de compte du profil de publication</span><span class="sxs-lookup"><span data-stu-id="69d51-1696">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="69d51-1697">Ajout de l’argument `--target-regions` à `sig image-version create` pour autoriser la définition de types de comptes de stockage spécifiques à une région</span><span class="sxs-lookup"><span data-stu-id="69d51-1697">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="69d51-1698">9 avril 2019</span><span class="sxs-lookup"><span data-stu-id="69d51-1698">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="69d51-1699">Core</span><span class="sxs-lookup"><span data-stu-id="69d51-1699">Core</span></span>
* <span data-ttu-id="69d51-1700">Correction du problème où certaines extensions affichaient une version `Unknown` et ne pouvaient pas être mises à jour</span><span class="sxs-lookup"><span data-stu-id="69d51-1700">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="69d51-1701">ACR</span><span class="sxs-lookup"><span data-stu-id="69d51-1701">ACR</span></span>
* <span data-ttu-id="69d51-1702">Ajout de la prise en charge de l’exécution d’une image sans contexte</span><span class="sxs-lookup"><span data-stu-id="69d51-1702">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="69d51-1703">AMS</span><span class="sxs-lookup"><span data-stu-id="69d51-1703">AMS</span></span>
* [DÉPRÉCIATION]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [CHANGEMENT CASSANT]: Renamed the `--bitrate` parameter to `--first-quality`
[BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="69d51-1706">Ajout de la prise en charge de nouveaux paramètres de chiffrement dans `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="69d51-1706">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="69d51-1707">Ajout du nouveau paramètre `--filters` à `ams streaming-locator create`</span><span class="sxs-lookup"><span data-stu-id="69d51-1707">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="69d51-1708">AppService</span><span class="sxs-lookup"><span data-stu-id="69d51-1708">AppService</span></span>
* <span data-ttu-id="69d51-1709">Ajout de la prise en charge de `--logs` pour `webapp up`</span><span class="sxs-lookup"><span data-stu-id="69d51-1709">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="69d51-1710">Correction des problèmes de génération de `azure-pipelines.yml` avec la commande `functionapp devops-build create`</span><span class="sxs-lookup"><span data-stu-id="69d51-1710">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="69d51-1711">Amélioration des indicateurs et de la gestion des erreurs `unctionapp devops-build create`</span><span class="sxs-lookup"><span data-stu-id="69d51-1711">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="69d51-1712">[CHANGEMENT CASSANT] Suppression de l’indicateur `--local-git` pour la commande `devops-build` ; la détection et la gestion d’un Git local sont obligatoires pour créer des pipelines Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="69d51-1712">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="69d51-1713">Ajout de la prise en charge de la création de plan de fonction pour Linux</span><span class="sxs-lookup"><span data-stu-id="69d51-1713">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="69d51-1714">Ajout de la possibilité de changer de plan sous une application de fonction avec `functionapp update --plan`</span><span class="sxs-lookup"><span data-stu-id="69d51-1714">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="69d51-1715">Ajout de la prise en charge de paramètres de scale-out pour le plan Azure Functions Premium</span><span class="sxs-lookup"><span data-stu-id="69d51-1715">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="69d51-1716">CDN</span><span class="sxs-lookup"><span data-stu-id="69d51-1716">CDN</span></span>
* <span data-ttu-id="69d51-1717">Ajout de la prise en charge de `Microsoft_Standard` et de `Standard_ChinaCdn`</span><span class="sxs-lookup"><span data-stu-id="69d51-1717">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="69d51-1718">Commentaires</span><span class="sxs-lookup"><span data-stu-id="69d51-1718">Feedback</span></span>
* <span data-ttu-id="69d51-1719">Changement apporté à `feedback` pour afficher les métadonnées sur les commandes exécutées récemment</span><span class="sxs-lookup"><span data-stu-id="69d51-1719">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="69d51-1720">Changement apporté à `feedback` pour inviter l’utilisateur à ouvrir un navigateur et à utiliser un modèle de message de problème afin de faciliter le processus de création du ticket</span><span class="sxs-lookup"><span data-stu-id="69d51-1720">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="69d51-1721">Changement apporté à `feedback` pour afficher le corps du message du problème quand la commande est exécutée avec '--verbose'</span><span class="sxs-lookup"><span data-stu-id="69d51-1721">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="69d51-1722">Superviser</span><span class="sxs-lookup"><span data-stu-id="69d51-1722">Monitor</span></span>
* <span data-ttu-id="69d51-1723">Correction du problème où « count » n’était pas une valeur autorisée avec `metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69d51-1723">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="69d51-1724">Réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-1724">Network</span></span>
* <span data-ttu-id="69d51-1725">Correction du problème empêchant l’affichage du format de table avec `vnet-gateway list-bgp-peer-status`</span><span class="sxs-lookup"><span data-stu-id="69d51-1725">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="69d51-1726">Ajout des commandes `list-request-headers` et `list-response-headers` à `application-gateway rewrite-rule`</span><span class="sxs-lookup"><span data-stu-id="69d51-1726">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="69d51-1727">Ajout de la commande `list-server-variables` à `application-gateway rewrite-rule condition`</span><span class="sxs-lookup"><span data-stu-id="69d51-1727">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="69d51-1728">Correction du problème où la mise à jour de l’état d’une liaison sur un port express-route levait une exception d’attribut inconnu `express-route port update`</span><span class="sxs-lookup"><span data-stu-id="69d51-1728">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="69d51-1729">PrivateDNS</span><span class="sxs-lookup"><span data-stu-id="69d51-1729">PrivateDNS</span></span>
* <span data-ttu-id="69d51-1730">Ajout de `network private-dns` pour les zones de DNS privé</span><span class="sxs-lookup"><span data-stu-id="69d51-1730">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="69d51-1731">Ressource</span><span class="sxs-lookup"><span data-stu-id="69d51-1731">Resource</span></span>
* <span data-ttu-id="69d51-1732">Correction du problème avec `deployment create` et `group deployment create` où un fichier de paramètres avec un ensemble de paramètres vide ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="69d51-1732">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="69d51-1733">Role</span><span class="sxs-lookup"><span data-stu-id="69d51-1733">Role</span></span>
* <span data-ttu-id="69d51-1734">Correction de `create-for-rbac` pour gérer `--years` correctement</span><span class="sxs-lookup"><span data-stu-id="69d51-1734">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="69d51-1735">[CHANGEMENT CASSANT] Changement apporté à `role assignment delete` pour afficher une invite lors d’une suppression sans condition de toutes les attributions sous l’abonnement</span><span class="sxs-lookup"><span data-stu-id="69d51-1735">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="69d51-1736">SQL</span><span class="sxs-lookup"><span data-stu-id="69d51-1736">SQL</span></span>
* <span data-ttu-id="69d51-1737">Mise à jour de `sql mi [create|update]` avec les propriétés proxyOverride et publicDataEndpointEnabledd</span><span class="sxs-lookup"><span data-stu-id="69d51-1737">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="69d51-1738">Stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-1738">Storage</span></span>
* <span data-ttu-id="69d51-1739">[CHANGEMENT CASSANT] Suppression du résultat de `storage blob delete`</span><span class="sxs-lookup"><span data-stu-id="69d51-1739">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="69d51-1740">Ajout de `--full-uri` à `storage blob generate-sas` pour créer l’URI complet pour l’objet blob avec SAS</span><span class="sxs-lookup"><span data-stu-id="69d51-1740">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="69d51-1741">Ajout de `--file-snapshot` à `storage file copy start` pour copier le fichier à partir de l’instantané</span><span class="sxs-lookup"><span data-stu-id="69d51-1741">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="69d51-1742">Changement apporté à `storage blob copy cancel` pour afficher uniquement l’erreur au lieu de l’exception pour NoPendingCopyOperation</span><span class="sxs-lookup"><span data-stu-id="69d51-1742">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="69d51-1743">26 mars 2019</span><span class="sxs-lookup"><span data-stu-id="69d51-1743">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="69d51-1744">Core</span><span class="sxs-lookup"><span data-stu-id="69d51-1744">Core</span></span>
* <span data-ttu-id="69d51-1745">Résolution des problèmes d’incompatibilité des extensions de développement</span><span class="sxs-lookup"><span data-stu-id="69d51-1745">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="69d51-1746">La gestion des erreurs redirige les clients vers la page des problèmes</span><span class="sxs-lookup"><span data-stu-id="69d51-1746">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="69d51-1747">Cloud</span><span class="sxs-lookup"><span data-stu-id="69d51-1747">Cloud</span></span>
* <span data-ttu-id="69d51-1748">Correction d’une erreur « abonnement introuvable » dans `cloud set`</span><span class="sxs-lookup"><span data-stu-id="69d51-1748">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="69d51-1749">ACR</span><span class="sxs-lookup"><span data-stu-id="69d51-1749">ACR</span></span>
* <span data-ttu-id="69d51-1750">Correction d’un problème concernant des sources redondantes lors de l’importation d’images</span><span class="sxs-lookup"><span data-stu-id="69d51-1750">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="69d51-1751">Ajout de `--auth-mode` aux commandes `acr build`, `acr run`, `acr task create` et `acr task update`</span><span class="sxs-lookup"><span data-stu-id="69d51-1751">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="69d51-1752">Ajout du groupe de commandes 'acr task credential' pour la gestion des informations d’identification pour une tâche</span><span class="sxs-lookup"><span data-stu-id="69d51-1752">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="69d51-1753">Ajout de '--no-wait' à la commande `acr build`</span><span class="sxs-lookup"><span data-stu-id="69d51-1753">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="69d51-1754">AppService</span><span class="sxs-lookup"><span data-stu-id="69d51-1754">AppService</span></span>
* <span data-ttu-id="69d51-1755">Correction du bogue où `webapp up` ne gérait pas correctement l’exécution dans un scénario de répertoire vide ou de code inconnu</span><span class="sxs-lookup"><span data-stu-id="69d51-1755">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="69d51-1756">Correction du bogue où les emplacements ne fonctionnaient pas pour `[webapp|functionapp] config ssl bind`</span><span class="sxs-lookup"><span data-stu-id="69d51-1756">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="69d51-1757">Service BOT</span><span class="sxs-lookup"><span data-stu-id="69d51-1757">BOT Service</span></span>
* <span data-ttu-id="69d51-1758">Ajout de `bot prepare-deploy` pour préparer le déploiement de bots via `webapp`</span><span class="sxs-lookup"><span data-stu-id="69d51-1758">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="69d51-1759">Modification de `bot create --kind registration` pour afficher le mot de passe si celui-ci n’est pas fourni</span><span class="sxs-lookup"><span data-stu-id="69d51-1759">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="69d51-1760">[CHANGEMENT CASSANT] Changement de `--endpoint` dans `bot create --kind registration` pour qu’il soit par défaut dans une chaîne vide au lieu d’être requis</span><span class="sxs-lookup"><span data-stu-id="69d51-1760">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="69d51-1761">Ajout de `SCM_DO_BUILD_DURING_DEPLOYMENT` aux paramètres d’application du modèle ARM pour Web App Bots v4</span><span class="sxs-lookup"><span data-stu-id="69d51-1761">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="69d51-1762">CDN</span><span class="sxs-lookup"><span data-stu-id="69d51-1762">CDN</span></span>
* <span data-ttu-id="69d51-1763">Ajout de la prise en charge de `--no-wait` pour `cdn endpoint [create|update|start|stop|delete|load|purge]`</span><span class="sxs-lookup"><span data-stu-id="69d51-1763">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* <span data-ttu-id="69d51-1764">[CHANGEMENT CASSANT] : Changement du comportement de mise en cache de chaînes de requête par défaut de `cdn endpoint create`.</span><span class="sxs-lookup"><span data-stu-id="69d51-1764">[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour.</span></span> <span data-ttu-id="69d51-1765">Sa valeur par défaut n’est plus « IgnoreQueryString ».</span><span class="sxs-lookup"><span data-stu-id="69d51-1765">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="69d51-1766">Il est maintenant défini par le service</span><span class="sxs-lookup"><span data-stu-id="69d51-1766">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="69d51-1767">Cosmosdb</span><span class="sxs-lookup"><span data-stu-id="69d51-1767">Cosmosdb</span></span>
* <span data-ttu-id="69d51-1768">Ajout de la prise en charge de `--enable-multiple-write-locations` lors de la mise à jour de compte</span><span class="sxs-lookup"><span data-stu-id="69d51-1768">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="69d51-1769">Ajout du sous-groupe `network-rule` avec les commandes `add`, `remove` et `list` pour gérer les règles de réseau virtuel d’un compte Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="69d51-1769">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="69d51-1770">Interactive</span><span class="sxs-lookup"><span data-stu-id="69d51-1770">Interactive</span></span>
* <span data-ttu-id="69d51-1771">Correction d’une incompatibilité avec l’extension Interactive installée via azdev</span><span class="sxs-lookup"><span data-stu-id="69d51-1771">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="69d51-1772">Superviser</span><span class="sxs-lookup"><span data-stu-id="69d51-1772">Monitor</span></span>
* <span data-ttu-id="69d51-1773">Changement visant à autoriser la valeur de dimension `*` pour `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69d51-1773">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="69d51-1774">Réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-1774">Network</span></span>
* <span data-ttu-id="69d51-1775">Ajout du groupe de commandes `rewrite-rule` à `application-gateway`</span><span class="sxs-lookup"><span data-stu-id="69d51-1775">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="69d51-1776">Profil</span><span class="sxs-lookup"><span data-stu-id="69d51-1776">Profile</span></span>
* <span data-ttu-id="69d51-1777">Ajout de la prise en charge du compte de niveau locataire pour Managed Service Identity dans `login`</span><span class="sxs-lookup"><span data-stu-id="69d51-1777">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="69d51-1778">Postgres</span><span class="sxs-lookup"><span data-stu-id="69d51-1778">Postgres</span></span> 
* <span data-ttu-id="69d51-1779">Ajout des commandes `replica` et de la commande `restart server` postgresql</span><span class="sxs-lookup"><span data-stu-id="69d51-1779">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="69d51-1780">Changement permettant d’obtenir l’emplacement par défaut du groupe de ressources lorsqu’il n’a pas été fourni, pour la création de serveurs et l’ajout d’une validation pour les jours de conservation</span><span class="sxs-lookup"><span data-stu-id="69d51-1780">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="69d51-1781">Ressource</span><span class="sxs-lookup"><span data-stu-id="69d51-1781">Resource</span></span>
* <span data-ttu-id="69d51-1782">Amélioration de la sortie de table pour `deployment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="69d51-1782">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="69d51-1783">Correction du problème avec `deployment [create|validate]` où le secureObject de type n’était pas reconnu</span><span class="sxs-lookup"><span data-stu-id="69d51-1783">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="69d51-1784">Graph</span><span class="sxs-lookup"><span data-stu-id="69d51-1784">Graph</span></span>
* <span data-ttu-id="69d51-1785">Ajout de la prise en charge de `--end-date` pour `ad [app|sp] credential reset`</span><span class="sxs-lookup"><span data-stu-id="69d51-1785">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="69d51-1786">Ajout de la prise en charge permettant d’ajouter des autorisations avec `ad app permission add`</span><span class="sxs-lookup"><span data-stu-id="69d51-1786">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="69d51-1787">Correction d’un bogue avec `ad app permission list` où il n’existait aucune autorisation</span><span class="sxs-lookup"><span data-stu-id="69d51-1787">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="69d51-1788">Modification de `ad sp delete` pour ignorer la suppression d’attribution de rôle si le compte actuel n’a aucun abonnement</span><span class="sxs-lookup"><span data-stu-id="69d51-1788">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="69d51-1789">Modification de `ad app create` pour avoir `--identifier-uris` par défaut dans une liste vide si non fourni</span><span class="sxs-lookup"><span data-stu-id="69d51-1789">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="69d51-1790">storage</span><span class="sxs-lookup"><span data-stu-id="69d51-1790">storage</span></span>
* <span data-ttu-id="69d51-1791">Ajout de `--snapshot` à `storage file download-batch` pour télécharger depuis un instantané de partage</span><span class="sxs-lookup"><span data-stu-id="69d51-1791">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="69d51-1792">Modification de la barre de progression `storage blob [download-batch|upload-batch]` pour qu’elle soit moins détaillée et qu’elle indique les objets blob actuels</span><span class="sxs-lookup"><span data-stu-id="69d51-1792">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="69d51-1793">Correction du problème avec `storage account update` lors de la mise à jour des paramètres de chiffrement</span><span class="sxs-lookup"><span data-stu-id="69d51-1793">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="69d51-1794">Correction d’un problème où `storage blob show` échouait quand oauth était utilisé (`--auth-mode=login`)</span><span class="sxs-lookup"><span data-stu-id="69d51-1794">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="69d51-1795">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="69d51-1795">VM</span></span>
* <span data-ttu-id="69d51-1796">Ajout de la commande `image update`</span><span class="sxs-lookup"><span data-stu-id="69d51-1796">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="69d51-1797">12 mars 2019</span><span class="sxs-lookup"><span data-stu-id="69d51-1797">March 12, 2019</span></span>

<span data-ttu-id="69d51-1798">Version 2.0.60</span><span class="sxs-lookup"><span data-stu-id="69d51-1798">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="69d51-1799">Core</span><span class="sxs-lookup"><span data-stu-id="69d51-1799">Core</span></span>

* <span data-ttu-id="69d51-1800">Correction d’une erreur dans `cloud set` concernant un abonnement introuvable</span><span class="sxs-lookup"><span data-stu-id="69d51-1800">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="69d51-1801">ACR</span><span class="sxs-lookup"><span data-stu-id="69d51-1801">ACR</span></span>

* <span data-ttu-id="69d51-1802">Correction d’un problème concernant des sources redondantes lors de l’importation d’images</span><span class="sxs-lookup"><span data-stu-id="69d51-1802">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="69d51-1803">ACS</span><span class="sxs-lookup"><span data-stu-id="69d51-1803">ACS</span></span>

* <span data-ttu-id="69d51-1804">Changement apporté pour que le paramètre `--listen-address` dans `aks browse` soit ignoré s’il n’est pas pris en charge par kubectl</span><span class="sxs-lookup"><span data-stu-id="69d51-1804">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="69d51-1805">AppService</span><span class="sxs-lookup"><span data-stu-id="69d51-1805">AppService</span></span>

* <span data-ttu-id="69d51-1806">Ajout de `[webapp|functionapp] deployment list-publishing-credentials` pour obtenir l’URL de publication Kudu et ses informations d’identification</span><span class="sxs-lookup"><span data-stu-id="69d51-1806">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="69d51-1807">Suppression d’une instruction print erronée pour `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="69d51-1807">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="69d51-1808">Correction de `functionapp` pour définir la bonne image runtime dans les plans App Service Linux</span><span class="sxs-lookup"><span data-stu-id="69d51-1808">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="69d51-1809">Suppression de l’étiquette de préversion pour `webapp up` et ajout d’améliorations à la commande</span><span class="sxs-lookup"><span data-stu-id="69d51-1809">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="69d51-1810">Botservice</span><span class="sxs-lookup"><span data-stu-id="69d51-1810">Botservice</span></span>

* <span data-ttu-id="69d51-1811">Ajout de `SCM_DO_BUILD_DURING_DEPLOYMENT` aux paramètres d’application du modèle ARM pour Web App Bots v4</span><span class="sxs-lookup"><span data-stu-id="69d51-1811">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="69d51-1812">Ajout de `Microsoft-BotFramework-AppId` et de `Microsoft-BotFramework-AppPassword` aux paramètres d’application du modèle ARM pour Web App Bots v4</span><span class="sxs-lookup"><span data-stu-id="69d51-1812">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="69d51-1813">Suppression des guillemets simples dans la sortie de la commande `bot publish`, à la fin de `bot create`</span><span class="sxs-lookup"><span data-stu-id="69d51-1813">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="69d51-1814">Modification de `bot publish` pour le rendre asynchrone</span><span class="sxs-lookup"><span data-stu-id="69d51-1814">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="69d51-1815">Conteneur</span><span class="sxs-lookup"><span data-stu-id="69d51-1815">Container</span></span>

* <span data-ttu-id="69d51-1816">Ajout de l’argument `--no-wait` à `container [start|restart]`</span><span class="sxs-lookup"><span data-stu-id="69d51-1816">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="69d51-1817">Event Hub</span><span class="sxs-lookup"><span data-stu-id="69d51-1817">EventHub</span></span>

* <span data-ttu-id="69d51-1818">Ajout de l’indicateur `--skip-empty-archives` à `eventhub create|update` pour prendre en charge les archives vides dans les captures</span><span class="sxs-lookup"><span data-stu-id="69d51-1818">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="69d51-1819">Rechercher</span><span class="sxs-lookup"><span data-stu-id="69d51-1819">Find</span></span>

* <span data-ttu-id="69d51-1820">Mise à jour importante de fonctionnalités</span><span class="sxs-lookup"><span data-stu-id="69d51-1820">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="69d51-1821">HDInsight</span><span class="sxs-lookup"><span data-stu-id="69d51-1821">HDInsight</span></span>

* <span data-ttu-id="69d51-1822">Ajout du paramètre `--storage-account-managed-identity` à `hdinsight create` pour prendre en charge le MSI ADLS Gen2</span><span class="sxs-lookup"><span data-stu-id="69d51-1822">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="69d51-1823">Réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-1823">Network</span></span>

* <span data-ttu-id="69d51-1824">Correction d’un problème concernant `vpn-connection update`, qui provoquait l’échec de la mise à jour d’une connexion VPN établie entre deux passerelles appartenant à des abonnements différents</span><span class="sxs-lookup"><span data-stu-id="69d51-1824">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="69d51-1825">Rdbms</span><span class="sxs-lookup"><span data-stu-id="69d51-1825">Rdbms</span></span>

* <span data-ttu-id="69d51-1826">Correctifs mineurs permettant d’obtenir l’emplacement par défaut du groupe de ressources lorsqu’il n’a pas été fourni, pour la création de serveurs et l’ajout d’une validation pour les jours de rétention</span><span class="sxs-lookup"><span data-stu-id="69d51-1826">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="69d51-1827">Role</span><span class="sxs-lookup"><span data-stu-id="69d51-1827">Role</span></span>

* <span data-ttu-id="69d51-1828">Correction de `role definition update` pour utiliser l’ID afin de résoudre correctement les définitions</span><span class="sxs-lookup"><span data-stu-id="69d51-1828">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="69d51-1829">Modification de `ad app credential reset` pour ne plus partir du principe que le principal de service de l’application existe toujours</span><span class="sxs-lookup"><span data-stu-id="69d51-1829">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="69d51-1830">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="69d51-1830">Service Fabric</span></span>

* <span data-ttu-id="69d51-1831">Correction du problème où `sf cluster list` n’était pas itérable</span><span class="sxs-lookup"><span data-stu-id="69d51-1831">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="69d51-1832">26 février 2019</span><span class="sxs-lookup"><span data-stu-id="69d51-1832">February 26, 2019</span></span>

<span data-ttu-id="69d51-1833">Version 2.0.59</span><span class="sxs-lookup"><span data-stu-id="69d51-1833">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="69d51-1834">Core</span><span class="sxs-lookup"><span data-stu-id="69d51-1834">Core</span></span>

* <span data-ttu-id="69d51-1835">Correction du problème où l’utilisation de `--subscription NAME` levait une exception dans certains cas</span><span class="sxs-lookup"><span data-stu-id="69d51-1835">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="69d51-1836">ACR</span><span class="sxs-lookup"><span data-stu-id="69d51-1836">ACR</span></span>

* <span data-ttu-id="69d51-1837">Ajout du paramètre `--target` pour les commandes `acr build`, `acr task create` et `acr task update`</span><span class="sxs-lookup"><span data-stu-id="69d51-1837">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="69d51-1838">Amélioration de la gestion des erreurs pour les commandes de runtime quand vous n’êtes pas connecté à Azure</span><span class="sxs-lookup"><span data-stu-id="69d51-1838">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="69d51-1839">ACS</span><span class="sxs-lookup"><span data-stu-id="69d51-1839">ACS</span></span>

* <span data-ttu-id="69d51-1840">Ajout de l’option `--listen-address` à `aks port-forward`</span><span class="sxs-lookup"><span data-stu-id="69d51-1840">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="69d51-1841">AppService</span><span class="sxs-lookup"><span data-stu-id="69d51-1841">AppService</span></span>

* <span data-ttu-id="69d51-1842">Ajout de la commande `functionapp devops-build`</span><span class="sxs-lookup"><span data-stu-id="69d51-1842">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="69d51-1843">Batch</span><span class="sxs-lookup"><span data-stu-id="69d51-1843">Batch</span></span>
* <span data-ttu-id="69d51-1844">[CHANGEMENT CASSANT] Suppression de la commande `batch pool upgrade os`</span><span class="sxs-lookup"><span data-stu-id="69d51-1844">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="69d51-1845">[CHANGEMENT CASSANT] Suppression de la propriété `Pacakges` des réponses `Application`</span><span class="sxs-lookup"><span data-stu-id="69d51-1845">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="69d51-1846">Ajout de la commande `batch application package list` pour lister les packages d’une application</span><span class="sxs-lookup"><span data-stu-id="69d51-1846">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="69d51-1847">[CHANGEMENT CASSANT] Remplacement de `--application-id` par `--application-name` dans toutes les commandes `batch application`</span><span class="sxs-lookup"><span data-stu-id="69d51-1847">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="69d51-1848">Ajout de l’argument `--json-file` aux commandes permettant de demander la réponse d’API brute</span><span class="sxs-lookup"><span data-stu-id="69d51-1848">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="69d51-1849">Mise à jour de la validation pour inclure automatiquement `https://` dans tous les points de terminaison si manquant</span><span class="sxs-lookup"><span data-stu-id="69d51-1849">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="69d51-1850">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="69d51-1850">CosmosDB</span></span>

* <span data-ttu-id="69d51-1851">Ajout du sous-groupe `network-rule` avec les commandes `add`, `remove` et `list` pour gérer les règles de réseau virtuel d’un compte Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="69d51-1851">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="69d51-1852">Kusto</span><span class="sxs-lookup"><span data-stu-id="69d51-1852">Kusto</span></span>

* <span data-ttu-id="69d51-1853">[CHANGEMENT CASSANT] Changement des types `hot_cache_period` et `soft_delete_period` de la base de données en format de durée ISO8601</span><span class="sxs-lookup"><span data-stu-id="69d51-1853">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="69d51-1854">Réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-1854">Network</span></span>

* <span data-ttu-id="69d51-1855">Ajout de l’argument `--express-route-gateway-bypass` à `vpn-connection [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69d51-1855">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="69d51-1856">Ajout de groupes de commandes à partir des extensions `express-route`</span><span class="sxs-lookup"><span data-stu-id="69d51-1856">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="69d51-1857">Ajout des groupes de commandes `express-route gateway` et `express-route port`</span><span class="sxs-lookup"><span data-stu-id="69d51-1857">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="69d51-1858">Ajout d’un argument `--legacy-mode` à `express-route peering [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69d51-1858">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="69d51-1859">Ajout des arguments `--allow-classic-operations` et `--express-route-port` à `express-route [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69d51-1859">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="69d51-1860">Ajout de l’argument `--gateway-default-site` à `vnet-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69d51-1860">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="69d51-1861">Ajout des commandes `ipsec-policy` à `vnet-gateway`</span><span class="sxs-lookup"><span data-stu-id="69d51-1861">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="69d51-1862">Ressource</span><span class="sxs-lookup"><span data-stu-id="69d51-1862">Resource</span></span>

* <span data-ttu-id="69d51-1863">Correction du problème de `deployment create` où le champ de type n’était pas sensible à la casse</span><span class="sxs-lookup"><span data-stu-id="69d51-1863">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="69d51-1864">Ajout de la prise en charge du fichier de paramètres basé sur l’URI sur `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="69d51-1864">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="69d51-1865">Ajout de la prise en charge des définitions et des paramètres basés sur l’URI sur `policy set-definition update`</span><span class="sxs-lookup"><span data-stu-id="69d51-1865">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="69d51-1866">Correction de la gestion des paramètres et des règles pour `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="69d51-1866">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="69d51-1867">Correction du problème avec `resource show/update/delete/tag/invoke-action` où les ID inter-abonnements n’honoraient pas correctement l’ID d’abonnement</span><span class="sxs-lookup"><span data-stu-id="69d51-1867">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="69d51-1868">Role</span><span class="sxs-lookup"><span data-stu-id="69d51-1868">Role</span></span>

* <span data-ttu-id="69d51-1869">Ajout de la prise en charge des rôles d’application sur `ad app [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69d51-1869">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="69d51-1870">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="69d51-1870">VM</span></span>

* <span data-ttu-id="69d51-1871">Correction du problème avec `vm create where `--accelerated-networking\` qui n’était pas activé par défaut pour Ubuntu 18.0</span><span class="sxs-lookup"><span data-stu-id="69d51-1871">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="69d51-1872">12 février 2019</span><span class="sxs-lookup"><span data-stu-id="69d51-1872">February 12, 2019</span></span>

<span data-ttu-id="69d51-1873">Version 2.0.58</span><span class="sxs-lookup"><span data-stu-id="69d51-1873">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="69d51-1874">Core</span><span class="sxs-lookup"><span data-stu-id="69d51-1874">Core</span></span>

* <span data-ttu-id="69d51-1875">`az --version` affiche désormais une notification si vous avez des packages qui peuvent être mis à jour</span><span class="sxs-lookup"><span data-stu-id="69d51-1875">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="69d51-1876">Correction de la régression où `--ids` ne pouvait plus être utilisé avec une sortie JSON</span><span class="sxs-lookup"><span data-stu-id="69d51-1876">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="69d51-1877">ACR</span><span class="sxs-lookup"><span data-stu-id="69d51-1877">ACR</span></span>
* <span data-ttu-id="69d51-1878">[CHANGEMENT CASSANT] Suppression du groupe de commandes `acr build-task`</span><span class="sxs-lookup"><span data-stu-id="69d51-1878">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="69d51-1879">[CHANGEMENT CASSANT] Suppression des options `--tag` et `--manifest` dans `acr repository delete`</span><span class="sxs-lookup"><span data-stu-id="69d51-1879">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="69d51-1880">ACS</span><span class="sxs-lookup"><span data-stu-id="69d51-1880">ACS</span></span>
* <span data-ttu-id="69d51-1881">Ajout de la prise en charge des noms qui ne respectent pas la casse à `aks [enable-addons|disable-addons]`</span><span class="sxs-lookup"><span data-stu-id="69d51-1881">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="69d51-1882">Ajout de la prise en charge de l’opération de mise à jour d’Azure Active Directory à l’aide de `aks update-credentials --reset-aad`</span><span class="sxs-lookup"><span data-stu-id="69d51-1882">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="69d51-1883">Ajout d’une clarification indiquant que `--output` est ignoré pour `aks get-credentials`</span><span class="sxs-lookup"><span data-stu-id="69d51-1883">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="69d51-1884">AMS</span><span class="sxs-lookup"><span data-stu-id="69d51-1884">AMS</span></span>
* <span data-ttu-id="69d51-1885">Ajout des commandes `ams streaming-endpoint [start | stop | create | update] wait`</span><span class="sxs-lookup"><span data-stu-id="69d51-1885">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="69d51-1886">Ajout des commandes `ams live-event [create | start | stop | reset] wait`</span><span class="sxs-lookup"><span data-stu-id="69d51-1886">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="69d51-1887">AppService</span><span class="sxs-lookup"><span data-stu-id="69d51-1887">Appservice</span></span>
* <span data-ttu-id="69d51-1888">Ajout des possibilités de création et de configuration de fonctions à l’aide de conteneurs ACR</span><span class="sxs-lookup"><span data-stu-id="69d51-1888">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="69d51-1889">Ajout de la prise en charge de la mise à jour des configurations d’applications web via JSON</span><span class="sxs-lookup"><span data-stu-id="69d51-1889">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="69d51-1890">Amélioration de l’aide pour `appservice-plan-update`</span><span class="sxs-lookup"><span data-stu-id="69d51-1890">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="69d51-1891">Ajout de la prise en charge d’Application Insights sur functionapp create</span><span class="sxs-lookup"><span data-stu-id="69d51-1891">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="69d51-1892">Résolution des problèmes liés à webapp SSH</span><span class="sxs-lookup"><span data-stu-id="69d51-1892">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="69d51-1893">Botservice</span><span class="sxs-lookup"><span data-stu-id="69d51-1893">Botservice</span></span>
* <span data-ttu-id="69d51-1894">Amélioration de l’expérience utilisateur pour `bot publish`</span><span class="sxs-lookup"><span data-stu-id="69d51-1894">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="69d51-1895">Ajout d’un avertissement pour les délais d’expiration au moment de l’exécution de `npm install` durant `az bot publish`</span><span class="sxs-lookup"><span data-stu-id="69d51-1895">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="69d51-1896">Suppression du caractère non valide `.` de `--name` dans `az bot create`</span><span class="sxs-lookup"><span data-stu-id="69d51-1896">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="69d51-1897">Changement apporté pour mettre fin aux noms de ressources aléatoires durant la création du Stockage Azure, du plan App Service, de Function App/Web App et d’Application Insights</span><span class="sxs-lookup"><span data-stu-id="69d51-1897">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="69d51-1898">[DÉPRÉCIATION] Dépréciation de l’argument `--proj-name` en faveur de `--proj-file-path`</span><span class="sxs-lookup"><span data-stu-id="69d51-1898">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="69d51-1899">Changement apporté à `az bot publish` pour supprimer les fichiers de déploiements IIS Node.js récupérés (fetch), s’ils n’existent pas déjà</span><span class="sxs-lookup"><span data-stu-id="69d51-1899">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="69d51-1900">Ajout de l’argument `--keep-node-modules` à `az bot publish` pour éviter la suppression du dossier `node_modules` dans App Service</span><span class="sxs-lookup"><span data-stu-id="69d51-1900">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="69d51-1901">Ajout de la paire clé/valeur `"publishCommand"` à la sortie de `az bot create` au moment de la création d’une fonction Azure ou d’un bot Web App</span><span class="sxs-lookup"><span data-stu-id="69d51-1901">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="69d51-1902">La valeur de `"publishCommand"` est une commande `az bot publish` préremplie avec les paramètres obligatoires pour publier le bot venant d’être créé</span><span class="sxs-lookup"><span data-stu-id="69d51-1902">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="69d51-1903">Mise à jour de `"WEBSITE_NODE_DEFAULT_VERSION"` dans le modèle ARM pour permettre aux bots du kit SDK v4 d’utiliser la version 10.14.1 au lieu de la version 8.9.4</span><span class="sxs-lookup"><span data-stu-id="69d51-1903">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="69d51-1904">Key Vault</span><span class="sxs-lookup"><span data-stu-id="69d51-1904">Key Vault</span></span>
* <span data-ttu-id="69d51-1905">Correction du problème lié à `keyvault secret backup`, où certains utilisateurs recevaient une erreur `unexpected_keyword` quand ils utilisaient `--id`</span><span class="sxs-lookup"><span data-stu-id="69d51-1905">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="69d51-1906">Superviser</span><span class="sxs-lookup"><span data-stu-id="69d51-1906">Monitor</span></span>
* <span data-ttu-id="69d51-1907">Changement apporté à `monitor metrics alert [create|update]` pour autoriser la valeur de dimension `*`</span><span class="sxs-lookup"><span data-stu-id="69d51-1907">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="69d51-1908">Réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-1908">Network</span></span>
* <span data-ttu-id="69d51-1909">Changement apporté à `dns zone export` pour que les enregistrements CNAME exportés soient des noms de domaine complets</span><span class="sxs-lookup"><span data-stu-id="69d51-1909">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="69d51-1910">Ajout du paramètre `--gateway-name` à `nic ip-config address-pool [add|remove]` pour permettre la prise en charge des pools d’adresses back-end d’Application Gateway</span><span class="sxs-lookup"><span data-stu-id="69d51-1910">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="69d51-1911">Ajout des arguments `--traffic-analytics` et `--workspace` à `network watcher flow-log configure` pour permettre la prise en charge de l’analyse du trafic via un espace de travail Log Analytics</span><span class="sxs-lookup"><span data-stu-id="69d51-1911">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="69d51-1912">Ajout de `--idle-timeout` et `--floating-ip` à `lb inbound-nat-pool [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69d51-1912">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="69d51-1913">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="69d51-1913">Policy Insights</span></span>
* <span data-ttu-id="69d51-1914">Ajout des commandes `policy remediation` pour permettre la prise en charge des fonctionnalités de correction des stratégies de ressources</span><span class="sxs-lookup"><span data-stu-id="69d51-1914">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="69d51-1915">SGBDR</span><span class="sxs-lookup"><span data-stu-id="69d51-1915">RDBMS</span></span>
* <span data-ttu-id="69d51-1916">Amélioration du message d’aide et des paramètres de commande</span><span class="sxs-lookup"><span data-stu-id="69d51-1916">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="69d51-1917">Redis</span><span class="sxs-lookup"><span data-stu-id="69d51-1917">Redis</span></span>
* <span data-ttu-id="69d51-1918">Ajout de commandes pour la gestion des règles de pare-feu (create, update, delete, show, list)</span><span class="sxs-lookup"><span data-stu-id="69d51-1918">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="69d51-1919">Ajout de commandes pour la gestion de la liaison avec le serveur (create, delete, show, list)</span><span class="sxs-lookup"><span data-stu-id="69d51-1919">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="69d51-1920">Ajout de commandes pour la gestion de la planification des correctifs (create, update, delete, show)</span><span class="sxs-lookup"><span data-stu-id="69d51-1920">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="69d51-1921">Ajout de la prise en charge des zones de disponibilité et de la version minimale de TLS dans redis create</span><span class="sxs-lookup"><span data-stu-id="69d51-1921">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="69d51-1922">[CHANGEMENT CASSANT] Suppression des commandes `redis update-settings` et `redis list-all`</span><span class="sxs-lookup"><span data-stu-id="69d51-1922">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="69d51-1923">[CHANGEMENT CASSANT] Le paramètre de `redis create` : « paramètres du locataire » n’est pas accepté au format clé[=valeur]</span><span class="sxs-lookup"><span data-stu-id="69d51-1923">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="69d51-1924">[DÉPRÉCIATION] Ajout d’un message d’avertissement concernant la dépréciation de la commande `redis import-method`</span><span class="sxs-lookup"><span data-stu-id="69d51-1924">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="69d51-1925">Role</span><span class="sxs-lookup"><span data-stu-id="69d51-1925">Role</span></span>
* <span data-ttu-id="69d51-1926">[CHANGEMENT CASSANT] Déplacement de la commande `az identity` ici à partir des commandes `vm`</span><span class="sxs-lookup"><span data-stu-id="69d51-1926">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="69d51-1927">Machine virtuelle SQL</span><span class="sxs-lookup"><span data-stu-id="69d51-1927">SQL VM</span></span>
* <span data-ttu-id="69d51-1928">[DÉPRÉCIATION] Dépréciation de l’argument `--boostrap-acc-pwd` en raison d’une faute de frappe</span><span class="sxs-lookup"><span data-stu-id="69d51-1928">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="69d51-1929">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="69d51-1929">VM</span></span>
* <span data-ttu-id="69d51-1930">Changement de `vm list-skus` pour autoriser l’utilisation de `--all` à la place de `--all true`</span><span class="sxs-lookup"><span data-stu-id="69d51-1930">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="69d51-1931">Ajout de `vmss run-command [invoke | list | show]`</span><span class="sxs-lookup"><span data-stu-id="69d51-1931">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="69d51-1932">Correction d’un bogue qui entraînait l’échec de `vmss encryption enable`, s’il était exécuté</span><span class="sxs-lookup"><span data-stu-id="69d51-1932">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="69d51-1933">[CHANGEMENT CASSANT] Déplacement de la commande `az identity` vers les commandes `role`</span><span class="sxs-lookup"><span data-stu-id="69d51-1933">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="69d51-1934">31 janvier 2019</span><span class="sxs-lookup"><span data-stu-id="69d51-1934">January 31, 2019</span></span>

<span data-ttu-id="69d51-1935">Version 2.0.57</span><span class="sxs-lookup"><span data-stu-id="69d51-1935">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="69d51-1936">Core</span><span class="sxs-lookup"><span data-stu-id="69d51-1936">Core</span></span>

* <span data-ttu-id="69d51-1937">Correctif pour le [problème 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="69d51-1937">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="69d51-1938">28 janvier 2019</span><span class="sxs-lookup"><span data-stu-id="69d51-1938">January 28, 2019</span></span>

<span data-ttu-id="69d51-1939">Version 2.0.56</span><span class="sxs-lookup"><span data-stu-id="69d51-1939">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="69d51-1940">ACR</span><span class="sxs-lookup"><span data-stu-id="69d51-1940">ACR</span></span>
* <span data-ttu-id="69d51-1941">Ajout de la prise en charge des règles de réseau virtuel (VNet)/d’adresses IP</span><span class="sxs-lookup"><span data-stu-id="69d51-1941">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="69d51-1942">ACS</span><span class="sxs-lookup"><span data-stu-id="69d51-1942">ACS</span></span>
* <span data-ttu-id="69d51-1943">Ajout de l’aperçu des nœuds virtuels</span><span class="sxs-lookup"><span data-stu-id="69d51-1943">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="69d51-1944">Ajout des commandes d’OpenShift managé</span><span class="sxs-lookup"><span data-stu-id="69d51-1944">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="69d51-1945">Ajout de la prise en charge des mises à jour du principal de service avec `aks update-credentials -reset-service-principal`</span><span class="sxs-lookup"><span data-stu-id="69d51-1945">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="69d51-1946">AMS</span><span class="sxs-lookup"><span data-stu-id="69d51-1946">AMS</span></span>
* <span data-ttu-id="69d51-1947">[CHANGEMENT CASSANT] Renommage de `ams asset get-streaming-locators` en `ams asset list-streaming-locators`</span><span class="sxs-lookup"><span data-stu-id="69d51-1947">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="69d51-1948">[CHANGEMENT CASSANT] Renommage de `ams streaming-locator get-content-keys` en `ams streaming-locator list-content-keys`</span><span class="sxs-lookup"><span data-stu-id="69d51-1948">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="69d51-1949">AppService</span><span class="sxs-lookup"><span data-stu-id="69d51-1949">Appservice</span></span>
* <span data-ttu-id="69d51-1950">Ajout de la prise en charge d’Application Insights sur `functionapp create`</span><span class="sxs-lookup"><span data-stu-id="69d51-1950">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="69d51-1951">Ajout de la prise en charge de la création de plans App Service (notamment Elastic Premium) à Function App</span><span class="sxs-lookup"><span data-stu-id="69d51-1951">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="69d51-1952">Correction de problèmes de configuration des applications avec les plans Elastic Premium</span><span class="sxs-lookup"><span data-stu-id="69d51-1952">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="69d51-1953">Conteneur</span><span class="sxs-lookup"><span data-stu-id="69d51-1953">Container</span></span>
* <span data-ttu-id="69d51-1954">Ajout de la commande `container start`</span><span class="sxs-lookup"><span data-stu-id="69d51-1954">Added `container start` command</span></span>
* <span data-ttu-id="69d51-1955">Changements apportés afin de permettre l’utilisation de valeurs décimales pour le processeur durant la création d’un conteneur</span><span class="sxs-lookup"><span data-stu-id="69d51-1955">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="69d51-1956">EventGrid</span><span class="sxs-lookup"><span data-stu-id="69d51-1956">EventGrid</span></span>
* <span data-ttu-id="69d51-1957">Ajout du paramètre `--deadletter-endpoint` pour `event-subscription [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69d51-1957">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="69d51-1958">Ajout de storagequeue et hybridconnection en tant que nouvelles valeurs pour « event-subscription [create|update] --endpoint-type »</span><span class="sxs-lookup"><span data-stu-id="69d51-1958">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="69d51-1959">Ajout des paramètres `--max-delivery-attempts` et `--event-ttl` à `event-subscription create` pour spécifier la stratégie de nouvelles tentatives des événements</span><span class="sxs-lookup"><span data-stu-id="69d51-1959">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="69d51-1960">Ajout d’un message d’avertissement à `event-subscription [create|update]` en cas d’utilisation de Webhook en tant que destination pour un abonnement à un événement</span><span class="sxs-lookup"><span data-stu-id="69d51-1960">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="69d51-1961">Ajout du paramètre source-resource-id pour toutes les commandes relatives à un abonnement aux événements et marquage de tous les autres paramètres relatifs aux ressources sources comme étant dépréciés</span><span class="sxs-lookup"><span data-stu-id="69d51-1961">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="69d51-1962">HDInsight</span><span class="sxs-lookup"><span data-stu-id="69d51-1962">HDInsight</span></span>
* <span data-ttu-id="69d51-1963">[CHANGEMENT CASSANT] Suppression des paramètres `--virtual-network` et `--subnet-name` dans `hdinsight [application] create`</span><span class="sxs-lookup"><span data-stu-id="69d51-1963">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="69d51-1964">[CHANGEMENT CASSANT] Changement apporté à `hdinsight create --storage-account` pour accepter le nom ou l’ID du compte de stockage à la place des points de terminaison d’objet blob</span><span class="sxs-lookup"><span data-stu-id="69d51-1964">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="69d51-1965">Ajout des paramètres `--vnet-name` et `--subnet-name` à `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="69d51-1965">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="69d51-1966">Ajout de la prise en charge du Pack Sécurité Entreprise et du chiffrement de disque à `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="69d51-1966">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="69d51-1967">Ajout de la commande `hdinsight rotate-disk-encryption-key`</span><span class="sxs-lookup"><span data-stu-id="69d51-1967">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="69d51-1968">Ajout de la commande `hdinsight update`</span><span class="sxs-lookup"><span data-stu-id="69d51-1968">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="69d51-1969">IoT</span><span class="sxs-lookup"><span data-stu-id="69d51-1969">IoT</span></span>
* <span data-ttu-id="69d51-1970">Ajout du format d’encodage à la commande routing-endpoint</span><span class="sxs-lookup"><span data-stu-id="69d51-1970">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="69d51-1971">Kusto</span><span class="sxs-lookup"><span data-stu-id="69d51-1971">Kusto</span></span>
* <span data-ttu-id="69d51-1972">Préversion</span><span class="sxs-lookup"><span data-stu-id="69d51-1972">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="69d51-1973">Superviser</span><span class="sxs-lookup"><span data-stu-id="69d51-1973">Monitor</span></span>
* <span data-ttu-id="69d51-1974">Changement apporté à la comparaison d’ID pour qu’elle ne respecte pas la casse</span><span class="sxs-lookup"><span data-stu-id="69d51-1974">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="69d51-1975">Profil</span><span class="sxs-lookup"><span data-stu-id="69d51-1975">Profile</span></span>
* <span data-ttu-id="69d51-1976">Activation du compte de niveau locataire pour la fonctionnalité Managed Service Identity pour `login`</span><span class="sxs-lookup"><span data-stu-id="69d51-1976">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="69d51-1977">Réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-1977">Network</span></span>
* <span data-ttu-id="69d51-1978">Correction d’un problème lié à `express-route update` où l’argument `--bandwidth` était ignoré</span><span class="sxs-lookup"><span data-stu-id="69d51-1978">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="69d51-1979">Correction d’un problème lié à `ddos-protection update` où set comprehension entraînait la génération d’un rapport des appels de procédure</span><span class="sxs-lookup"><span data-stu-id="69d51-1979">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="69d51-1980">Ressource</span><span class="sxs-lookup"><span data-stu-id="69d51-1980">Resource</span></span>
* <span data-ttu-id="69d51-1981">Ajout de la prise en charge du fichier de paramètres d’URI à `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="69d51-1981">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="69d51-1982">Ajout de la prise en charge de l’identité managée à `policy assignment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="69d51-1982">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="69d51-1983">Machine virtuelle SQL</span><span class="sxs-lookup"><span data-stu-id="69d51-1983">SQL Virtual Machine</span></span>
* <span data-ttu-id="69d51-1984">Préversion</span><span class="sxs-lookup"><span data-stu-id="69d51-1984">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="69d51-1985">Stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-1985">Storage</span></span>
* <span data-ttu-id="69d51-1986">Changement d’une correction pour mettre à jour uniquement les propriétés modifiées sur le même objet</span><span class="sxs-lookup"><span data-stu-id="69d51-1986">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="69d51-1987">Correction (n° 8021). Les données binaires sont encodées au format base 64 quand elles sont retournées</span><span class="sxs-lookup"><span data-stu-id="69d51-1987">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="69d51-1988">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="69d51-1988">VM</span></span>
* <span data-ttu-id="69d51-1989">Changement apporté à `vm encryption enable` pour valider le coffre de clés de chiffrement de disque et vérifier l’existence du coffre de clés de chiffrement à clé</span><span class="sxs-lookup"><span data-stu-id="69d51-1989">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="69d51-1990">Ajout de l’indicateur `--force` à `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="69d51-1990">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="69d51-1991">15 janvier 2019</span><span class="sxs-lookup"><span data-stu-id="69d51-1991">January 15, 2019</span></span>

<span data-ttu-id="69d51-1992">Version 2.0.55</span><span class="sxs-lookup"><span data-stu-id="69d51-1992">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="69d51-1993">ACR</span><span class="sxs-lookup"><span data-stu-id="69d51-1993">ACR</span></span>
* <span data-ttu-id="69d51-1994">Changement apporté pour forcer l’envoi (push) d’un chart Helm qui n’existe pas</span><span class="sxs-lookup"><span data-stu-id="69d51-1994">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="69d51-1995">changement apporté pour autoriser les opérations de runtime sans requêtes ARM</span><span class="sxs-lookup"><span data-stu-id="69d51-1995">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="69d51-1996">[DÉPRÉCIATION] Dépréciation du paramètre `--resource-group` dans les commandes :</span><span class="sxs-lookup"><span data-stu-id="69d51-1996">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="69d51-1997">ACS</span><span class="sxs-lookup"><span data-stu-id="69d51-1997">ACS</span></span>
* <span data-ttu-id="69d51-1998">Ajout de la prise en charge des nouvelles régions ACI</span><span class="sxs-lookup"><span data-stu-id="69d51-1998">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="69d51-1999">AppService</span><span class="sxs-lookup"><span data-stu-id="69d51-1999">Appservice</span></span>
* <span data-ttu-id="69d51-2000">Correction d’un problème lié au chargement des certificats des applications hébergées sur un ASE, où ASE RG et App RG sont différents</span><span class="sxs-lookup"><span data-stu-id="69d51-2000">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="69d51-2001">Changement apporté à `webapp up` pour utiliser la référence (SKU) P1V1 en tant que valeur par défaut pour Linux</span><span class="sxs-lookup"><span data-stu-id="69d51-2001">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="69d51-2002">Correction apporté à `[webapp|functionapp] deployment source config-zip` pour afficher le message d’erreur approprié en cas d’échec d’un déploiement</span><span class="sxs-lookup"><span data-stu-id="69d51-2002">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="69d51-2003">Ajout de la commande `webapp ssh`</span><span class="sxs-lookup"><span data-stu-id="69d51-2003">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="69d51-2004">Botservice</span><span class="sxs-lookup"><span data-stu-id="69d51-2004">Botservice</span></span>
* <span data-ttu-id="69d51-2005">Ajout de mises à jour de l’état de déploiement à `bot create`</span><span class="sxs-lookup"><span data-stu-id="69d51-2005">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="69d51-2006">Configurer</span><span class="sxs-lookup"><span data-stu-id="69d51-2006">Configure</span></span>
* <span data-ttu-id="69d51-2007">Ajout de `none` en tant que format de sortie configurable</span><span class="sxs-lookup"><span data-stu-id="69d51-2007">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="69d51-2008">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="69d51-2008">CosmosDB</span></span>
* <span data-ttu-id="69d51-2009">Ajout de la prise en charge de la création d’une base de données avec débit partagé</span><span class="sxs-lookup"><span data-stu-id="69d51-2009">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="69d51-2010">HDInsight</span><span class="sxs-lookup"><span data-stu-id="69d51-2010">HDInsight</span></span>
* <span data-ttu-id="69d51-2011">Ajout de commandes pour la gestion des applications</span><span class="sxs-lookup"><span data-stu-id="69d51-2011">Added commands for managing applications</span></span>
* <span data-ttu-id="69d51-2012">Ajout de commandes pour la gestion des actions de script</span><span class="sxs-lookup"><span data-stu-id="69d51-2012">Added commands for managing script actions</span></span>
* <span data-ttu-id="69d51-2013">Ajout de commandes pour la gestion d’OMS (Operations Management Suite)</span><span class="sxs-lookup"><span data-stu-id="69d51-2013">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="69d51-2014">Ajout de la prise en charge permettant de lister l’utilisation régionale à `hdinsight list-usage`</span><span class="sxs-lookup"><span data-stu-id="69d51-2014">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="69d51-2015">[CHANGEMENT CASSANT] Suppression du type de cluster par défaut dans `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="69d51-2015">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="69d51-2016">Réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-2016">Network</span></span>
* <span data-ttu-id="69d51-2017">Ajout des arguments `--custom-headers` et `--status-code-ranges` à `traffic-manager profile [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69d51-2017">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="69d51-2018">Ajout de nouveaux types de routage : Sous-réseau et valeurs multiples</span><span class="sxs-lookup"><span data-stu-id="69d51-2018">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="69d51-2019">Ajout des arguments `--custom-headers` et `--subnets` à `traffic-manager endpoint [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69d51-2019">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="69d51-2020">Correction du problème où la fourniture de `--vnets ""` à `ddos-protection update` provoquait une erreur</span><span class="sxs-lookup"><span data-stu-id="69d51-2020">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="69d51-2021">Role</span><span class="sxs-lookup"><span data-stu-id="69d51-2021">Role</span></span>
* <span data-ttu-id="69d51-2022">[DÉPRÉCIATION] Dépréciation de l’argument `--password` pour `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="69d51-2022">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="69d51-2023">Utilisation de mots de passe sécurisés générés par l’interface CLI à la place</span><span class="sxs-lookup"><span data-stu-id="69d51-2023">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="69d51-2024">Sécurité</span><span class="sxs-lookup"><span data-stu-id="69d51-2024">Security</span></span>
* <span data-ttu-id="69d51-2025">Version initiale</span><span class="sxs-lookup"><span data-stu-id="69d51-2025">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="69d51-2026">Stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-2026">Storage</span></span>
* <span data-ttu-id="69d51-2027">[CHANGEMENT CASSANT] Changement apporté à `storage [blob|file|container|share] list` pour que le nombre par défaut de résultats soit de 5 000.</span><span class="sxs-lookup"><span data-stu-id="69d51-2027">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="69d51-2028">Utilisation de `--num-results *` pour que le comportement d’origine permette de retourner tous les résultats</span><span class="sxs-lookup"><span data-stu-id="69d51-2028">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="69d51-2029">Ajout du paramètre `--marker` pour `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="69d51-2029">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="69d51-2030">Ajout du marqueur de journal de la page suivante à STDERR pour `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="69d51-2030">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="69d51-2031">Ajout de la commande `storage blob service-properties update` avec prise en charge des sites web statiques</span><span class="sxs-lookup"><span data-stu-id="69d51-2031">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="69d51-2032">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="69d51-2032">VM</span></span>
* <span data-ttu-id="69d51-2033">Changement apporté à `vm [disk|unmanaged-disk]` et `vmss disk` pour avoir des paramètres plus cohérents</span><span class="sxs-lookup"><span data-stu-id="69d51-2033">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="69d51-2034">Ajout de la prise en charge du référencement d’images entre locataires à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="69d51-2034">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="69d51-2035">Résolution d’un bogue lié à la configuration par défaut dans `vm diagnostics get-default-config --windows-os`</span><span class="sxs-lookup"><span data-stu-id="69d51-2035">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="69d51-2036">Ajout de l’argument `--provision-after-extensions` à `vmss extension set` pour définir les extensions à provisionner avant de définir l’extension</span><span class="sxs-lookup"><span data-stu-id="69d51-2036">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="69d51-2037">Ajout de l’argument `--replica-count` à `sig image-version update` pour définir le nombre de réplications par défaut</span><span class="sxs-lookup"><span data-stu-id="69d51-2037">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="69d51-2038">Résolution d’un bogue lié à `image create --source` où le disque d’OS source est confondu avec une machine virtuelle portant le même nom, même si l’ID de ressource complet est fourni</span><span class="sxs-lookup"><span data-stu-id="69d51-2038">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="69d51-2039">20 décembre 2018</span><span class="sxs-lookup"><span data-stu-id="69d51-2039">December 20, 2018</span></span>

<span data-ttu-id="69d51-2040">Version 2.0.54</span><span class="sxs-lookup"><span data-stu-id="69d51-2040">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="69d51-2041">AppService</span><span class="sxs-lookup"><span data-stu-id="69d51-2041">Appservice</span></span>
* <span data-ttu-id="69d51-2042">Correction d’un problème qui causait l’échec du redéploiement pour `webapp up`</span><span class="sxs-lookup"><span data-stu-id="69d51-2042">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="69d51-2043">Ajout de la prise en charge du référencement et de la restauration des instantanés d’applications web</span><span class="sxs-lookup"><span data-stu-id="69d51-2043">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="69d51-2044">Ajout de la prise en charge pour l’indicateur `--runtime` aux applications de fonction Windows</span><span class="sxs-lookup"><span data-stu-id="69d51-2044">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="69d51-2045">IotCentral</span><span class="sxs-lookup"><span data-stu-id="69d51-2045">IoTCentral</span></span>
* <span data-ttu-id="69d51-2046">Correction de l’appel d’API des commandes de mise à jour</span><span class="sxs-lookup"><span data-stu-id="69d51-2046">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="69d51-2047">Role</span><span class="sxs-lookup"><span data-stu-id="69d51-2047">Role</span></span>
* <span data-ttu-id="69d51-2048">[CHANGEMENT CASSANT] Remplacement de `ad [app|sp] list` par une liste des 100 premiers objets par défaut uniquement</span><span class="sxs-lookup"><span data-stu-id="69d51-2048">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="69d51-2049">SQL</span><span class="sxs-lookup"><span data-stu-id="69d51-2049">SQL</span></span>
* <span data-ttu-id="69d51-2050">Ajout de la prise en charge du classement personnalisé sur les instances managées</span><span class="sxs-lookup"><span data-stu-id="69d51-2050">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="69d51-2051">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="69d51-2051">VM</span></span>
* <span data-ttu-id="69d51-2052">Ajout du paramètre `---os-type` pour `disk create`</span><span class="sxs-lookup"><span data-stu-id="69d51-2052">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="69d51-2053">18 décembre 2018</span><span class="sxs-lookup"><span data-stu-id="69d51-2053">December 18, 2018</span></span>

<span data-ttu-id="69d51-2054">Version 2.0.53</span><span class="sxs-lookup"><span data-stu-id="69d51-2054">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="69d51-2055">ACR</span><span class="sxs-lookup"><span data-stu-id="69d51-2055">ACR</span></span>
* <span data-ttu-id="69d51-2056">Ajout de la prise en charge de l’importation d’image à partir des registres de conteneurs externes</span><span class="sxs-lookup"><span data-stu-id="69d51-2056">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="69d51-2057">Condensé de la disposition du tableau pour la liste des tâches</span><span class="sxs-lookup"><span data-stu-id="69d51-2057">Condensed the table layout for task list</span></span>
* <span data-ttu-id="69d51-2058">Ajout de la prise en charge des URL Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="69d51-2058">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="69d51-2059">ACS</span><span class="sxs-lookup"><span data-stu-id="69d51-2059">ACS</span></span>
* <span data-ttu-id="69d51-2060">Ajout de l’aperçu des nœuds virtuels</span><span class="sxs-lookup"><span data-stu-id="69d51-2060">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="69d51-2061">Suppression du mot « (PRÉVERSION) » des arguments AAD pour `aks create`</span><span class="sxs-lookup"><span data-stu-id="69d51-2061">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="69d51-2062">[DÉPRÉCIATION] Dépréciation des commandes `az acs`.</span><span class="sxs-lookup"><span data-stu-id="69d51-2062">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="69d51-2063">Le service ACS sera mis hors service le 31 janvier 2020.</span><span class="sxs-lookup"><span data-stu-id="69d51-2063">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="69d51-2064">Ajout de la prise en charge de la stratégie de réseau lors de la création de clusters AKS</span><span class="sxs-lookup"><span data-stu-id="69d51-2064">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="69d51-2065">Suppression du caractère obligatoire de l’argument `--nodepool-name` pour `aks scale` s’il n’existe qu’un seul pool de nœuds</span><span class="sxs-lookup"><span data-stu-id="69d51-2065">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="69d51-2066">AppService</span><span class="sxs-lookup"><span data-stu-id="69d51-2066">Appservice</span></span>
* <span data-ttu-id="69d51-2067">Problème résolu quand `webapp config container` n’honore pas le paramètre `--slot`</span><span class="sxs-lookup"><span data-stu-id="69d51-2067">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="69d51-2068">Botservice</span><span class="sxs-lookup"><span data-stu-id="69d51-2068">Botservice</span></span>
* <span data-ttu-id="69d51-2069">Ajout de la prise en charge de l’analyse de fichier `.bot` lors de l’appel de `bot show`</span><span class="sxs-lookup"><span data-stu-id="69d51-2069">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="69d51-2070">Correction du bogue d’approvisionnement AppInsights</span><span class="sxs-lookup"><span data-stu-id="69d51-2070">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="69d51-2071">Correction du bogue d’espace blanc lors du traitement de chemins d’accès de fichier</span><span class="sxs-lookup"><span data-stu-id="69d51-2071">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="69d51-2072">Réduction des appels réseau Kudu</span><span class="sxs-lookup"><span data-stu-id="69d51-2072">Reduced Kudu network calls</span></span>
* <span data-ttu-id="69d51-2073">Amélioration de l’expérience utilisateur des commandes générales</span><span class="sxs-lookup"><span data-stu-id="69d51-2073">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="69d51-2074">Consommation</span><span class="sxs-lookup"><span data-stu-id="69d51-2074">Consumption</span></span>
* <span data-ttu-id="69d51-2075">Correction des bogues dans l’API de budget pour afficher les notifications</span><span class="sxs-lookup"><span data-stu-id="69d51-2075">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="69d51-2076">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="69d51-2076">CosmosDB</span></span>
* <span data-ttu-id="69d51-2077">Ajout de la prise en charge de la mise à jour de compte (multimaître vers maître unique)</span><span class="sxs-lookup"><span data-stu-id="69d51-2077">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="69d51-2078">Cartes</span><span class="sxs-lookup"><span data-stu-id="69d51-2078">Maps</span></span>
* <span data-ttu-id="69d51-2079">Ajout de la prise en charge de la référence (SKU) S1 pour `maps account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69d51-2079">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="69d51-2080">Réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-2080">Network</span></span>
* <span data-ttu-id="69d51-2081">Ajout de la prise en charge de `--format`, `--log-version` et `watcher flow-log configure`</span><span class="sxs-lookup"><span data-stu-id="69d51-2081">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="69d51-2082">Correction du problème avec `dns zone update`, où l’utilisation de "" pour effacer les réseaux virtuels de résolution d’inscription ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="69d51-2082">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="69d51-2083">Ressource</span><span class="sxs-lookup"><span data-stu-id="69d51-2083">Resource</span></span>
* <span data-ttu-id="69d51-2084">Correction de la gestion du paramètre d’étendue pour les groupes d’administration dans `policy assignment [create|list|delete|show|update]`</span><span class="sxs-lookup"><span data-stu-id="69d51-2084">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="69d51-2085">Ajout de la commande `resource wait`</span><span class="sxs-lookup"><span data-stu-id="69d51-2085">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="69d51-2086">Stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-2086">Storage</span></span>
*  <span data-ttu-id="69d51-2087">Possibilité de mettre à jour la version de schéma de journal pour les services de stockage dans `storage logging update`</span><span class="sxs-lookup"><span data-stu-id="69d51-2087">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="69d51-2088">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="69d51-2088">VM</span></span>
* <span data-ttu-id="69d51-2089">Correction d’incident dans `vm identity remove`, lorsque la machine virtuelle spécifiée n’a aucune identité de service managé affectée</span><span class="sxs-lookup"><span data-stu-id="69d51-2089">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="69d51-2090">4 décembre 2018</span><span class="sxs-lookup"><span data-stu-id="69d51-2090">December 4, 2018</span></span>

<span data-ttu-id="69d51-2091">Version 2.0.52</span><span class="sxs-lookup"><span data-stu-id="69d51-2091">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="69d51-2092">Core</span><span class="sxs-lookup"><span data-stu-id="69d51-2092">Core</span></span>
* <span data-ttu-id="69d51-2093">L’approvisionnement des ressources entre locataires est désormais pris en charge pour le principal du service multi-locataire.</span><span class="sxs-lookup"><span data-stu-id="69d51-2093">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="69d51-2094">Les ID d’une commande avec sortie TSV n’étaient pas analysés correctement. Ce bogue a été corrigé.</span><span class="sxs-lookup"><span data-stu-id="69d51-2094">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="69d51-2095">AppService</span><span class="sxs-lookup"><span data-stu-id="69d51-2095">Appservice</span></span>
* <span data-ttu-id="69d51-2096">[APERÇU] Une commande `webapp up` a été ajoutée pour faciliter la création et le déploiement de contenu dans l’application.</span><span class="sxs-lookup"><span data-stu-id="69d51-2096">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="69d51-2097">Le bogue qui survenait sur les applications Windows basées sur des conteneurs en raison du changement de serveur principal a été corrigé.</span><span class="sxs-lookup"><span data-stu-id="69d51-2097">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="69d51-2098">Réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-2098">Network</span></span>
* <span data-ttu-id="69d51-2099">L’argument `--exclusion` a été ajouté à `application-gateway waf-config set` pour prendre en charge les exclusions WAF</span><span class="sxs-lookup"><span data-stu-id="69d51-2099">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="69d51-2100">Role</span><span class="sxs-lookup"><span data-stu-id="69d51-2100">Role</span></span>
* <span data-ttu-id="69d51-2101">Les identificateurs personnalisés sont désormais pris en charge pour l’authentification par mot de passe.</span><span class="sxs-lookup"><span data-stu-id="69d51-2101">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="69d51-2102">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="69d51-2102">VM</span></span>
* <span data-ttu-id="69d51-2103">[DÉPRÉCIATION] Dépréciation du paramètre `vm extension [show|wait] --expand`</span><span class="sxs-lookup"><span data-stu-id="69d51-2103">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="69d51-2104">Le paramètre `--force` a été ajouté à `vm restart` pour redéployer les machines virtuelles qui ne répondent pas.</span><span class="sxs-lookup"><span data-stu-id="69d51-2104">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="69d51-2105">Le paramètre `[vm|vmss] create --authentication-type` a été modifié pour accepter la valeur « all » pour créer une machine virtuelle avec à la fois un mot de passe et une authentification SSH.</span><span class="sxs-lookup"><span data-stu-id="69d51-2105">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="69d51-2106">Le paramètre `image create --os-disk-caching` a été ajouté pour définir la mise en cache du disque du système d’exploitation pour une image.</span><span class="sxs-lookup"><span data-stu-id="69d51-2106">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="69d51-2107">20 novembre 2018</span><span class="sxs-lookup"><span data-stu-id="69d51-2107">November 20, 2018</span></span>

<span data-ttu-id="69d51-2108">Version 2.0.51</span><span class="sxs-lookup"><span data-stu-id="69d51-2108">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="69d51-2109">Core</span><span class="sxs-lookup"><span data-stu-id="69d51-2109">Core</span></span>
* <span data-ttu-id="69d51-2110">Modification du nom de connexion MSI pour ne pas réutiliser le nom d’abonnement dans une identité</span><span class="sxs-lookup"><span data-stu-id="69d51-2110">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="69d51-2111">ACR</span><span class="sxs-lookup"><span data-stu-id="69d51-2111">ACR</span></span>
* <span data-ttu-id="69d51-2112">Ajout d’un jeton de contexte à l’étape de tâche</span><span class="sxs-lookup"><span data-stu-id="69d51-2112">Added context token to task step</span></span>
* <span data-ttu-id="69d51-2113">Ajout de prise en charge pour la configuration des secrets dans acr run pour refléter acr task</span><span class="sxs-lookup"><span data-stu-id="69d51-2113">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="69d51-2114">Amélioration de la prise en charge de `--top` et `--orderby` pour les commandes `show-tags` et `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="69d51-2114">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="69d51-2115">AppService</span><span class="sxs-lookup"><span data-stu-id="69d51-2115">Appservice</span></span>
* <span data-ttu-id="69d51-2116">Augmentation du délai d’expiration par défaut du déploiement zip pour interroger l’état à 5 min, ce qui ajoute également une propriété de délai d’expiration pour personnaliser cette valeur</span><span class="sxs-lookup"><span data-stu-id="69d51-2116">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="69d51-2117">Mise à jour de la valeur par défaut `node_version`.</span><span class="sxs-lookup"><span data-stu-id="69d51-2117">Updated the default `node_version`.</span></span> <span data-ttu-id="69d51-2118">La réinitialisation d’une action d’échange d’emplacements pendant un échange en deux phases conserve toutes les chaînes de connexion et paramètres d’application</span><span class="sxs-lookup"><span data-stu-id="69d51-2118">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="69d51-2119">Suppression de la vérification de référence SKU côté client pour app service plan create de Linux</span><span class="sxs-lookup"><span data-stu-id="69d51-2119">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="69d51-2120">Correction de l’erreur qui survenait lors de tentatives d’obtention de l’état zipdeploy</span><span class="sxs-lookup"><span data-stu-id="69d51-2120">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="69d51-2121">IotCentral</span><span class="sxs-lookup"><span data-stu-id="69d51-2121">IotCentral</span></span>
* <span data-ttu-id="69d51-2122">Ajouter de la vérification de disponibilité du sous-domaine lors de la création d’une application IoT Central</span><span class="sxs-lookup"><span data-stu-id="69d51-2122">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="69d51-2123">KeyVault</span><span class="sxs-lookup"><span data-stu-id="69d51-2123">KeyVault</span></span>
* <span data-ttu-id="69d51-2124">Correction du bogue dans lequel des erreurs pouvaient avoir été ignorées</span><span class="sxs-lookup"><span data-stu-id="69d51-2124">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="69d51-2125">Réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-2125">Network</span></span>
* <span data-ttu-id="69d51-2126">Ajout de sous-commandes `root-cert` à `application-gateway` pour traiter les certificats racine de confiance</span><span class="sxs-lookup"><span data-stu-id="69d51-2126">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="69d51-2127">Ajout des options `--min-capacity` et `--custom-error-pages` à `application-gateway [create|update]` :</span><span class="sxs-lookup"><span data-stu-id="69d51-2127">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="69d51-2128">Ajout de `--zones` pour la prise en charge de zone de disponibilité à `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="69d51-2128">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="69d51-2129">Ajout des arguments `--file-upload-limit`, `--max-request-body-size` et `--request-body-check` à `application-gateway waf-config set`</span><span class="sxs-lookup"><span data-stu-id="69d51-2129">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="69d51-2130">Rdbms</span><span class="sxs-lookup"><span data-stu-id="69d51-2130">Rdbms</span></span>
* <span data-ttu-id="69d51-2131">Ajouts de commandes mariadb vnet</span><span class="sxs-lookup"><span data-stu-id="69d51-2131">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="69d51-2132">Contrôle d’accès en fonction du rôle (RBAC)</span><span class="sxs-lookup"><span data-stu-id="69d51-2132">Rbac</span></span>
* <span data-ttu-id="69d51-2133">Résolution d’un problème qui survenait lors de tentatives de mise à jour d’informations d’identification immuables dans `ad app update`</span><span class="sxs-lookup"><span data-stu-id="69d51-2133">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="69d51-2134">Ajout d’avertissements de sortie pour indiquer des changements cassants dans un futur proche pour `ad [app|sp] list`</span><span class="sxs-lookup"><span data-stu-id="69d51-2134">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="69d51-2135">Stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-2135">Storage</span></span>
* <span data-ttu-id="69d51-2136">Amélioration du traitement des « corner cases » pour les commandes de copie de stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-2136">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="69d51-2137">Résolution d’un problème où `storage blob copy start-batch` n’utilisait pas les informations d’identification de connexion lorsque les comptes source et de destination étaient identiques</span><span class="sxs-lookup"><span data-stu-id="69d51-2137">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="69d51-2138">Correction du bogue avec `storage [blob|file] url` où `sas_token` n’était pas intégré dans l’URL</span><span class="sxs-lookup"><span data-stu-id="69d51-2138">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="69d51-2139">Ajout d’un avertissement de changement cassant à `[blob|container] list` : bientôt, seuls les 5 000 premiers résultats seront affichés par défaut dans la sortie</span><span class="sxs-lookup"><span data-stu-id="69d51-2139">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="69d51-2140">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="69d51-2140">VM</span></span>
* <span data-ttu-id="69d51-2141">Ajout de la prise en charge de `[vm|vmss] create --storage-sku` pour spécifier la référence SKU de compte de stockage pour les disques de données et de système d’exploitation managés de façon distincte</span><span class="sxs-lookup"><span data-stu-id="69d51-2141">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="69d51-2142">Remplacement des paramètres de nom de version `sig image-version` par `--image-version -e`</span><span class="sxs-lookup"><span data-stu-id="69d51-2142">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="69d51-2143">Version déconseillée de la valeur `--image-version-name` d’argument `sig image-version` remplacée par `--image-version`</span><span class="sxs-lookup"><span data-stu-id="69d51-2143">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="69d51-2144">Ajout de la prise en charge pour utiliser le disque de système d’exploitation local pour `[vm|vmss] create --ephemeral-os-disk`</span><span class="sxs-lookup"><span data-stu-id="69d51-2144">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="69d51-2145">Ajout de la prise en charge de `--no-wait` pour `snapshot create/update`</span><span class="sxs-lookup"><span data-stu-id="69d51-2145">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="69d51-2146">Ajout de la commande `snapshot wait`</span><span class="sxs-lookup"><span data-stu-id="69d51-2146">Added `snapshot wait` command</span></span>
* <span data-ttu-id="69d51-2147">Ajout de la prise en charge pour utiliser le nom d’instance avec `[vm|vmss] extension set --extension-instance-name`</span><span class="sxs-lookup"><span data-stu-id="69d51-2147">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="69d51-2148">6 novembre 2018</span><span class="sxs-lookup"><span data-stu-id="69d51-2148">November 6, 2018</span></span>

<span data-ttu-id="69d51-2149">Version 2.0.50</span><span class="sxs-lookup"><span data-stu-id="69d51-2149">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="69d51-2150">Core</span><span class="sxs-lookup"><span data-stu-id="69d51-2150">Core</span></span>
* <span data-ttu-id="69d51-2151">Ajout de la prise en charge pour le principal de service sn+issuer auth</span><span class="sxs-lookup"><span data-stu-id="69d51-2151">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="69d51-2152">ACR</span><span class="sxs-lookup"><span data-stu-id="69d51-2152">ACR</span></span>
* <span data-ttu-id="69d51-2153">Ajout de la prise en charge pour les événements git de demande d’envoi et de tirage pour le déclencheur de tâche source</span><span class="sxs-lookup"><span data-stu-id="69d51-2153">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="69d51-2154">Modification de l’utilisation de fichiers Dockerfile par défaut s’il n’est pas spécifié dans la commande build</span><span class="sxs-lookup"><span data-stu-id="69d51-2154">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="69d51-2155">ACS</span><span class="sxs-lookup"><span data-stu-id="69d51-2155">ACS</span></span>
* <span data-ttu-id="69d51-2156">[Changement cassant] : `enable_cloud_console_aks_browse` supprimé pour activer « az aks browse » par défaut</span><span class="sxs-lookup"><span data-stu-id="69d51-2156">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="69d51-2157">Advisor</span><span class="sxs-lookup"><span data-stu-id="69d51-2157">Advisor</span></span>
* <span data-ttu-id="69d51-2158">Version mise à la disposition générale</span><span class="sxs-lookup"><span data-stu-id="69d51-2158">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="69d51-2159">AMS</span><span class="sxs-lookup"><span data-stu-id="69d51-2159">AMS</span></span>
* <span data-ttu-id="69d51-2160">Ajout de nouveaux groupes de commandes :</span><span class="sxs-lookup"><span data-stu-id="69d51-2160">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="69d51-2161">Ajout de nouvelles commandes :</span><span class="sxs-lookup"><span data-stu-id="69d51-2161">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="69d51-2162">Ajout de la prise en charge des paramètres de chiffrement de `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="69d51-2162">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="69d51-2163">Ajout de la prise en charge de `ams transform output remove` qui peut désormais être effectuée en transmettant le chemin de l’index pour le supprimer</span><span class="sxs-lookup"><span data-stu-id="69d51-2163">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="69d51-2164">Ajout des arguments `--correlation-data` et `--label` au groupe de commandes `ams job`</span><span class="sxs-lookup"><span data-stu-id="69d51-2164">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="69d51-2165">Ajout des arguments `--storage-account` et `--container` au groupe de commandes `ams asset`</span><span class="sxs-lookup"><span data-stu-id="69d51-2165">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="69d51-2166">Ajout des valeurs par défaut pour le délai d’expiration (présent + 23h) et les autorisations (lecture) dans la commande `ams asset get-sas-url`</span><span class="sxs-lookup"><span data-stu-id="69d51-2166">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="69d51-2167">[Changement cassant] : commande `ams streaming locator` remplacée par `ams streaming-locator`</span><span class="sxs-lookup"><span data-stu-id="69d51-2167">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="69d51-2168">[Changement cassant] : mise à jour de l’argument `--content-keys` de `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="69d51-2168">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="69d51-2169">[Changement cassant] : `--content-policy-name` renommé en `--content-key-policy-name` dans la commande `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="69d51-2169">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="69d51-2170">[Changement cassant] : commande `ams streaming policy` remplacée par `ams streaming-policy`</span><span class="sxs-lookup"><span data-stu-id="69d51-2170">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="69d51-2171">[Changement cassant] : argument `--preset-names` remplacé par `--preset` dans le groupe de commandes `ams transform`.</span><span class="sxs-lookup"><span data-stu-id="69d51-2171">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="69d51-2172">À présent vous ne pouvez définir qu’une sortie/présélection à la fois (pour en ajouter d’autres, vous devez exécuter `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="69d51-2172">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="69d51-2173">En outre, vous pouvez définir StandardEncoderPreset de façon personnalisée en transmettant le chemin à votre JSON personnalisé</span><span class="sxs-lookup"><span data-stu-id="69d51-2173">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="69d51-2174">[Changement cassant] : `--output-asset-names ` renommé en `--output-assets` dans la commande `ams job start`.</span><span class="sxs-lookup"><span data-stu-id="69d51-2174">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="69d51-2175">Il accepte désormais une liste de ressources séparée par des espaces au format « assetName=label ».</span><span class="sxs-lookup"><span data-stu-id="69d51-2175">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="69d51-2176">Une ressource sans étiquette peut être envoyée comme ceci : « assetName= »</span><span class="sxs-lookup"><span data-stu-id="69d51-2176">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="69d51-2177">AppService</span><span class="sxs-lookup"><span data-stu-id="69d51-2177">AppService</span></span>
* <span data-ttu-id="69d51-2178">Correction d’un bogue dans `az webapp config backup update` qui empêche de définir une planification de sauvegarde si elle n’est pas déjà définie</span><span class="sxs-lookup"><span data-stu-id="69d51-2178">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="69d51-2179">Configurer</span><span class="sxs-lookup"><span data-stu-id="69d51-2179">Configure</span></span>
* <span data-ttu-id="69d51-2180">Ajout de YAML aux options de format de sortie</span><span class="sxs-lookup"><span data-stu-id="69d51-2180">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="69d51-2181">Conteneur</span><span class="sxs-lookup"><span data-stu-id="69d51-2181">Container</span></span>
* <span data-ttu-id="69d51-2182">Modification pour afficher l’identité lors de l’exportation d’un groupe de conteneurs vers yaml</span><span class="sxs-lookup"><span data-stu-id="69d51-2182">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="69d51-2183">Event Hub</span><span class="sxs-lookup"><span data-stu-id="69d51-2183">EventHub</span></span>
* <span data-ttu-id="69d51-2184">Ajout d’un indicateur `--enable-kafka` pour prendre en charge Kafka dans `eventhub namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69d51-2184">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="69d51-2185">Interactive</span><span class="sxs-lookup"><span data-stu-id="69d51-2185">Interactive</span></span>
* <span data-ttu-id="69d51-2186">Interactive installe maintenant l’extension `interactive`, ce qui permettra des mises à jour et prises en charge plus rapides</span><span class="sxs-lookup"><span data-stu-id="69d51-2186">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="69d51-2187">Superviser</span><span class="sxs-lookup"><span data-stu-id="69d51-2187">Monitor</span></span>
* <span data-ttu-id="69d51-2188">Ajout de la prise en charge pour les noms de métriques qui incluent les caractères barre oblique (/) et point (.) à `--condition` dans `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69d51-2188">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="69d51-2189">Réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-2189">Network</span></span>
* <span data-ttu-id="69d51-2190">Noms de commande `network interface-endpoint` déconseillés en faveur de `network private-endpoint`</span><span class="sxs-lookup"><span data-stu-id="69d51-2190">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="69d51-2191">Problème résolu à l’endroit où l’argument `--peer-circuit` n’accepte pas d’ID dans `express-route peering connection create`</span><span class="sxs-lookup"><span data-stu-id="69d51-2191">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="69d51-2192">Problème résolu à l’endroit où `--ip-tags` ne fonctionnait pas correctement avec `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="69d51-2192">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="69d51-2193">Profil</span><span class="sxs-lookup"><span data-stu-id="69d51-2193">Profile</span></span>
* <span data-ttu-id="69d51-2194">Ajout de `--use-cert-sn-issuer` à `az login` pour la connexion principale du service à l’aide du certificat de déploiement automatique</span><span class="sxs-lookup"><span data-stu-id="69d51-2194">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="69d51-2195">SGBDR</span><span class="sxs-lookup"><span data-stu-id="69d51-2195">RDBMS</span></span>
* <span data-ttu-id="69d51-2196">Ajout de commandes de réplica mysql</span><span class="sxs-lookup"><span data-stu-id="69d51-2196">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="69d51-2197">Ressource</span><span class="sxs-lookup"><span data-stu-id="69d51-2197">Resource</span></span>
* <span data-ttu-id="69d51-2198">Ajout de la prise en charge pour les groupes d’administration et les abonnements aux commandes `policy definition|set-definition`</span><span class="sxs-lookup"><span data-stu-id="69d51-2198">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="69d51-2199">Role</span><span class="sxs-lookup"><span data-stu-id="69d51-2199">Role</span></span>
* <span data-ttu-id="69d51-2200">Ajout de la prise en charge pour la gestion d’autorisation API, les utilisateurs connectés ainsi que la gestion des mots de passe et informations d’identification des certificats de l’application</span><span class="sxs-lookup"><span data-stu-id="69d51-2200">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="69d51-2201">Modification de `ad sp create-for-rbac` pour clarifier la confusion entre displayName et le nom de principal du service</span><span class="sxs-lookup"><span data-stu-id="69d51-2201">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="69d51-2202">Ajout de la prise en charge pour attribuer les autorisations aux applications AAD</span><span class="sxs-lookup"><span data-stu-id="69d51-2202">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="69d51-2203">Stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-2203">Storage</span></span>
* <span data-ttu-id="69d51-2204">Ajout de la prise en charge pour vous connecter aux services de stockage uniquement avec les signatures d’accès partagé et les points de terminaison (sans nom de compte ou clé), comme décrit dans `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span><span class="sxs-lookup"><span data-stu-id="69d51-2204">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="69d51-2205">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="69d51-2205">VM</span></span>
* <span data-ttu-id="69d51-2206">Ajout de l’argument `storage-sku` à `image create` pour définir le type de compte de stockage par défaut de l’image</span><span class="sxs-lookup"><span data-stu-id="69d51-2206">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="69d51-2207">Correction du bogue avec `vm resize` à l’endroit où l’option `--no-wait` a entraîné un incident avec la commande</span><span class="sxs-lookup"><span data-stu-id="69d51-2207">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="69d51-2208">Modification du format de sortie de la table `vm encryption show` pour afficher l’état</span><span class="sxs-lookup"><span data-stu-id="69d51-2208">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="69d51-2209">Modification de `vm secret format` pour exiger la sortie json/jsonc</span><span class="sxs-lookup"><span data-stu-id="69d51-2209">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="69d51-2210">Avertit l’utilisateur et les valeurs par défaut à la sortie json si un format de sortie indésirable est sélectionné</span><span class="sxs-lookup"><span data-stu-id="69d51-2210">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="69d51-2211">Amélioration de la validation de l’argument pour `vm create --image`</span><span class="sxs-lookup"><span data-stu-id="69d51-2211">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="69d51-2212">23 octobre 2018</span><span class="sxs-lookup"><span data-stu-id="69d51-2212">October 23, 2018</span></span>

<span data-ttu-id="69d51-2213">Version 2.0.49</span><span class="sxs-lookup"><span data-stu-id="69d51-2213">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="69d51-2214">Core</span><span class="sxs-lookup"><span data-stu-id="69d51-2214">Core</span></span>
* <span data-ttu-id="69d51-2215">Correction du problème avec `--ids` où `--subscription` serait prioritaire sur l’abonnement dans `--ids`</span><span class="sxs-lookup"><span data-stu-id="69d51-2215">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="69d51-2216">Ajout d’avertissements explicites lorsque les paramètres sont ignorés par `--ids`</span><span class="sxs-lookup"><span data-stu-id="69d51-2216">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="69d51-2217">ACR</span><span class="sxs-lookup"><span data-stu-id="69d51-2217">ACR</span></span>
* <span data-ttu-id="69d51-2218">Correction d’un problème de codage ACR Build dans Python2</span><span class="sxs-lookup"><span data-stu-id="69d51-2218">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="69d51-2219">CDN</span><span class="sxs-lookup"><span data-stu-id="69d51-2219">CDN</span></span>
* <span data-ttu-id="69d51-2220">[CHANGEMENT CASSANT] Modification du comportement de mise en cache de chaîne de requête par défaut de `cdn endpoint create` afin que ce ne soit plus « IgnoreQueryString » par défaut.</span><span class="sxs-lookup"><span data-stu-id="69d51-2220">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="69d51-2221">Il est maintenant défini par le service</span><span class="sxs-lookup"><span data-stu-id="69d51-2221">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="69d51-2222">Conteneur</span><span class="sxs-lookup"><span data-stu-id="69d51-2222">Container</span></span>
* <span data-ttu-id="69d51-2223">Ajout de `Private` comme un type valide pour passer à «--ip-address»</span><span class="sxs-lookup"><span data-stu-id="69d51-2223">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="69d51-2224">Modification pour permettre l’utilisation d’un seul ID de sous-réseau pour configurer un réseau virtuel pour le groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="69d51-2224">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="69d51-2225">Modification pour permettre l’utilisation d’un nom de réseau virtuel ou d’un ID de ressource pour permettre l’utilisation de réseaux virtuels à partir de groupes de ressources différents</span><span class="sxs-lookup"><span data-stu-id="69d51-2225">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="69d51-2226">Ajout de `--assign-identity` pour ajouter une identité MSI à un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="69d51-2226">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="69d51-2227">Ajout de `--scope` pour créer une attribution de rôle pour l’identité MSI attribuée par le système</span><span class="sxs-lookup"><span data-stu-id="69d51-2227">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="69d51-2228">Ajout d’un avertissement lors de la création d’un groupe de conteneurs avec une image sans processus à long terme</span><span class="sxs-lookup"><span data-stu-id="69d51-2228">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="69d51-2229">Correction de problèmes de sortie de table pour les commandes `list` et `show`</span><span class="sxs-lookup"><span data-stu-id="69d51-2229">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="69d51-2230">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="69d51-2230">CosmosDB</span></span>
* <span data-ttu-id="69d51-2231">Ajout de la prise en charge de `--enable-multiple-write-locations` pour `cosmosdb create`</span><span class="sxs-lookup"><span data-stu-id="69d51-2231">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="69d51-2232">Interactive</span><span class="sxs-lookup"><span data-stu-id="69d51-2232">Interactive</span></span>
* <span data-ttu-id="69d51-2233">Modifié pour assurer l’apparition du paramètre d’abonnement global dans les paramètres</span><span class="sxs-lookup"><span data-stu-id="69d51-2233">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="69d51-2234">IoT Central</span><span class="sxs-lookup"><span data-stu-id="69d51-2234">IoT Central</span></span>
* <span data-ttu-id="69d51-2235">Ajout d’options de modèle et de nom d’affichage pour la création de l’application IoT central</span><span class="sxs-lookup"><span data-stu-id="69d51-2235">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="69d51-2236">[CHANGEMENT CASSANT] Suppression de la prise en charge de la référence SKU F1, utilisez la référence SKU S1 à la place</span><span class="sxs-lookup"><span data-stu-id="69d51-2236">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="69d51-2237">Superviser</span><span class="sxs-lookup"><span data-stu-id="69d51-2237">Monitor</span></span>
* <span data-ttu-id="69d51-2238">Change en `monitor activity-log list` :</span><span class="sxs-lookup"><span data-stu-id="69d51-2238">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="69d51-2239">Prise en charge ajoutée pour répertorier tous les événements au niveau de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="69d51-2239">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="69d51-2240">Ajout du paramètre `--offset` pour créer plus facilement des requêtes de temps</span><span class="sxs-lookup"><span data-stu-id="69d51-2240">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="69d51-2241">Amélioration de la validation pour `--start-time` et `--end-time` pour utiliser des plages de formats ISO8601 plus larges et des formats dateHeure plus conviviaux</span><span class="sxs-lookup"><span data-stu-id="69d51-2241">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="69d51-2242">Ajout de `--namespace` comme alias pour l’option déconseillée `--resource-provider`</span><span class="sxs-lookup"><span data-stu-id="69d51-2242">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="69d51-2243">`--filters` déconseillé, car aucune valeur autre que celles avec des options fortement typées ne sont prises en charge par le service</span><span class="sxs-lookup"><span data-stu-id="69d51-2243">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="69d51-2244">Change en `monitor metrics list` :</span><span class="sxs-lookup"><span data-stu-id="69d51-2244">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="69d51-2245">Ajout du paramètre `--offset` pour créer plus facilement des requêtes de temps</span><span class="sxs-lookup"><span data-stu-id="69d51-2245">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="69d51-2246">Amélioration de la validation pour `--start-time` et `--end-time` pour utiliser des plages de formats ISO8601 plus larges et des formats dateHeure plus conviviaux</span><span class="sxs-lookup"><span data-stu-id="69d51-2246">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="69d51-2247">Amélioration de la validation pour les arguments `--event-hub` et `--event-hub-rule` à `monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="69d51-2247">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="69d51-2248">Réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-2248">Network</span></span>
* <span data-ttu-id="69d51-2249">Ajout des arguments `--app-gateway-address-pools` et `--gateway-name` à `nic create`, pour prendre en charge l’ajout de pools d’adresses principaux Application Gateway à une carte réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-2249">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="69d51-2250">Ajout des arguments `--app-gateway-address-pools` et `--gateway-name` à `nic ip-config create/update`, pour prendre en charge l’ajout de pools d’adresses principaux Application Gateway à une carte réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-2250">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="69d51-2251">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="69d51-2251">ServiceBus</span></span>
* <span data-ttu-id="69d51-2252">Ajout de `migration_state` en lecture seule à MigrationConfigProperties pour afficher l’état actuel de migration d’espace de noms Standard à Premium de Service Bus</span><span class="sxs-lookup"><span data-stu-id="69d51-2252">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="69d51-2253">SQL</span><span class="sxs-lookup"><span data-stu-id="69d51-2253">SQL</span></span>
* <span data-ttu-id="69d51-2254">`sql failover-group create` et `sql failover-group update` corrigés pour fonctionner avec la stratégie de basculement manuel</span><span class="sxs-lookup"><span data-stu-id="69d51-2254">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="69d51-2255">Stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-2255">Storage</span></span>
* <span data-ttu-id="69d51-2256">Formatage de sortie de `az storage cors list` corrigé, tous les éléments affichent une clé de « Service » correcte</span><span class="sxs-lookup"><span data-stu-id="69d51-2256">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="69d51-2257">Ajout du paramètre `--bypass-immutability-policy` pour la suppression du conteneur de stratégie d’immuabilité bloquée</span><span class="sxs-lookup"><span data-stu-id="69d51-2257">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="69d51-2258">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="69d51-2258">VM</span></span>
* <span data-ttu-id="69d51-2259">Mode de mise en cache configuré sur `None` pour la série de machines Lv/Lv2 dans `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="69d51-2259">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="69d51-2260">Mise à jour de la liste des tailles prises en charge, prenant en charge l’accélérateur de mise en réseau pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="69d51-2260">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="69d51-2261">Ajout des arguments fortement typés pour les configurations d’E/S et Mbits/s Ultrassd pour `disk create`</span><span class="sxs-lookup"><span data-stu-id="69d51-2261">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="69d51-2262">16 octobre 2018</span><span class="sxs-lookup"><span data-stu-id="69d51-2262">October 16, 2018</span></span>

<span data-ttu-id="69d51-2263">Version 2.0.48</span><span class="sxs-lookup"><span data-stu-id="69d51-2263">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="69d51-2264">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="69d51-2264">VM</span></span>
* <span data-ttu-id="69d51-2265">Résolution du problème de kit de développement logiciel qui a provoqué l’échec d’installation de Homebrew</span><span class="sxs-lookup"><span data-stu-id="69d51-2265">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="69d51-2266">9 octobre 2018</span><span class="sxs-lookup"><span data-stu-id="69d51-2266">October 9, 2018</span></span>

<span data-ttu-id="69d51-2267">Version 2.0.47</span><span class="sxs-lookup"><span data-stu-id="69d51-2267">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="69d51-2268">Core</span><span class="sxs-lookup"><span data-stu-id="69d51-2268">Core</span></span>
* <span data-ttu-id="69d51-2269">Gestion améliorée des erreurs « Demande incorrecte »</span><span class="sxs-lookup"><span data-stu-id="69d51-2269">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="69d51-2270">ACR</span><span class="sxs-lookup"><span data-stu-id="69d51-2270">ACR</span></span>
* <span data-ttu-id="69d51-2271">Prise en charge de format de tableau similaire, comme le client helm</span><span class="sxs-lookup"><span data-stu-id="69d51-2271">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="69d51-2272">ACS</span><span class="sxs-lookup"><span data-stu-id="69d51-2272">ACS</span></span>
* <span data-ttu-id="69d51-2273">Ajout de `aks [create|scale] --nodepool-name` pour configurer le nom du pool de nœuds, tronqué à 12 caractères, par défaut : nodepool1</span><span class="sxs-lookup"><span data-stu-id="69d51-2273">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="69d51-2274">Correction d’une erreur pour revenir à « scp » lorsque Parimiko échoue</span><span class="sxs-lookup"><span data-stu-id="69d51-2274">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="69d51-2275">Modification de `aks create` pour ne plus nécessiter `--aad-tenant-id`</span><span class="sxs-lookup"><span data-stu-id="69d51-2275">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="69d51-2276">Fusion améliorée des informations d'identification Kubernetes lorsque des entrées dupliquées sont présentes</span><span class="sxs-lookup"><span data-stu-id="69d51-2276">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="69d51-2277">Conteneur</span><span class="sxs-lookup"><span data-stu-id="69d51-2277">Container</span></span>
* <span data-ttu-id="69d51-2278">Modification de `functionapp create` pour prendre en charge la création d’un type de plan de consommation Linux avec un runtime spécifique</span><span class="sxs-lookup"><span data-stu-id="69d51-2278">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="69d51-2279">[PRÉVERSION] Prise en charge de l’hébergement d’applications web sur les conteneurs Windows</span><span class="sxs-lookup"><span data-stu-id="69d51-2279">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="69d51-2280">Event Hub</span><span class="sxs-lookup"><span data-stu-id="69d51-2280">Event Hub</span></span>
* <span data-ttu-id="69d51-2281">Correction de la commande `eventhub update`</span><span class="sxs-lookup"><span data-stu-id="69d51-2281">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="69d51-2282">[CHANGEMENT CASSANT] Modification des commandes `list` pour gérer des erreurs resource(s) NotFound(404) d’une manière habituelle au lieu d’afficher une liste vide</span><span class="sxs-lookup"><span data-stu-id="69d51-2282">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="69d51-2283">Extensions</span><span class="sxs-lookup"><span data-stu-id="69d51-2283">Extensions</span></span>
* <span data-ttu-id="69d51-2284">Correction d’une erreur de tentative d’ajout d’une extension déjà installée</span><span class="sxs-lookup"><span data-stu-id="69d51-2284">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="69d51-2285">HDInsight</span><span class="sxs-lookup"><span data-stu-id="69d51-2285">HDInsight</span></span>
* <span data-ttu-id="69d51-2286">Version initiale</span><span class="sxs-lookup"><span data-stu-id="69d51-2286">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="69d51-2287">IoT</span><span class="sxs-lookup"><span data-stu-id="69d51-2287">IoT</span></span>
* <span data-ttu-id="69d51-2288">Ajout de la commande d’installation de l’extension à une bannière pour la première exécution</span><span class="sxs-lookup"><span data-stu-id="69d51-2288">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="69d51-2289">KeyVault</span><span class="sxs-lookup"><span data-stu-id="69d51-2289">KeyVault</span></span>
* <span data-ttu-id="69d51-2290">Modification pour restreindre les commandes de stockage keyvault au dernier profil API</span><span class="sxs-lookup"><span data-stu-id="69d51-2290">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="69d51-2291">Réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-2291">Network</span></span>
* <span data-ttu-id="69d51-2292">Correction de `network dns zone create` : la commande réussit même si l’utilisateur a configuré un emplacement par défaut.</span><span class="sxs-lookup"><span data-stu-id="69d51-2292">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="69d51-2293">Voir #6052</span><span class="sxs-lookup"><span data-stu-id="69d51-2293">See #6052</span></span>
* <span data-ttu-id="69d51-2294">Remplacement de `--remote-vnet-id` pour `network vnet peering create`</span><span class="sxs-lookup"><span data-stu-id="69d51-2294">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="69d51-2295">Ajout de `--remote-vnet` à `network vnet peering create`, qui accepte un nom ou ID</span><span class="sxs-lookup"><span data-stu-id="69d51-2295">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="69d51-2296">Prise en charge de multiples préfixes de sous-réseau pour `network vnet create` avec `--subnet-prefixes`</span><span class="sxs-lookup"><span data-stu-id="69d51-2296">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="69d51-2297">Prise en charge de multiples préfixes de sous-réseau pour `network vnet subnet [create|update]` avec `--address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="69d51-2297">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="69d51-2298">Correction d’une erreur relative à `network application-gateway create` qui empêchait la création de passerelles avec les références SKU `WAF_v2` ou `Standard_v2`</span><span class="sxs-lookup"><span data-stu-id="69d51-2298">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="69d51-2299">Ajout de l’argument d’usage `--service-endpoint-policy` à `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="69d51-2299">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="69d51-2300">Role</span><span class="sxs-lookup"><span data-stu-id="69d51-2300">Role</span></span>
* <span data-ttu-id="69d51-2301">Prise en charge du listing des propriétaires d’applications Azure AD à `ad app owner`</span><span class="sxs-lookup"><span data-stu-id="69d51-2301">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="69d51-2302">Prise en charge du listing des propriétaires de principaux de service Azure AD à `ad sp owner`</span><span class="sxs-lookup"><span data-stu-id="69d51-2302">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="69d51-2303">Modification pour garantir que les commandes de mise à jour et de création de définition de rôle acceptent les configurations à autorisations multiples</span><span class="sxs-lookup"><span data-stu-id="69d51-2303">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="69d51-2304">Modification de `ad sp create-for-rbac` pour garantir que l’URI de la page d’accueil est toujours « https »</span><span class="sxs-lookup"><span data-stu-id="69d51-2304">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="69d51-2305">Service Bus</span><span class="sxs-lookup"><span data-stu-id="69d51-2305">Service Bus</span></span>
* <span data-ttu-id="69d51-2306">[CHANGEMENT CASSANT] Modification des commandes `list` pour gérer des erreurs resource(s) NotFound(404) d’une manière habituelle au lieu d’afficher une liste vide</span><span class="sxs-lookup"><span data-stu-id="69d51-2306">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="69d51-2307">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="69d51-2307">VM</span></span>
* <span data-ttu-id="69d51-2308">Correction du champ vide `accessSas` dans `disk grant-access`</span><span class="sxs-lookup"><span data-stu-id="69d51-2308">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="69d51-2309">Modification de `vmss create` pour réserver une plage de port de frontend assez large pour gérer le surprovisionnement</span><span class="sxs-lookup"><span data-stu-id="69d51-2309">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="69d51-2310">Correction des commandes de mise à jour pour `sig`</span><span class="sxs-lookup"><span data-stu-id="69d51-2310">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="69d51-2311">Prise en charge `--no-wait` de la gestion de versions d’images dans `sig`</span><span class="sxs-lookup"><span data-stu-id="69d51-2311">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="69d51-2312">Modification de `vm list-ip-addresses` pour afficher la zone de disponibilité des adresses IP publiques</span><span class="sxs-lookup"><span data-stu-id="69d51-2312">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="69d51-2313">Modification de `[vm|vmss] disk attach` pour définir le numéro d’identité logique (LUN) par défaut du disque sur le premier emplacement disponible</span><span class="sxs-lookup"><span data-stu-id="69d51-2313">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="69d51-2314">21 septembre 2018</span><span class="sxs-lookup"><span data-stu-id="69d51-2314">September 21, 2018</span></span>

<span data-ttu-id="69d51-2315">Version 2.0.46</span><span class="sxs-lookup"><span data-stu-id="69d51-2315">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="69d51-2316">ACR</span><span class="sxs-lookup"><span data-stu-id="69d51-2316">ACR</span></span>
* <span data-ttu-id="69d51-2317">Ajout de commandes de tâche ACR</span><span class="sxs-lookup"><span data-stu-id="69d51-2317">Added ACR Task commands</span></span>
* <span data-ttu-id="69d51-2318">Ajout de la commande d’exécution rapide</span><span class="sxs-lookup"><span data-stu-id="69d51-2318">Added quick run command</span></span>
* <span data-ttu-id="69d51-2319">Groupe de commandes `build-task` déconseillé</span><span class="sxs-lookup"><span data-stu-id="69d51-2319">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="69d51-2320">Ajout du groupe de commandes `helm` pour prendre en charge la gestion des graphiques Helm avec ACR</span><span class="sxs-lookup"><span data-stu-id="69d51-2320">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="69d51-2321">Ajout de la prise en charge de la création idempotent pour les registres managés</span><span class="sxs-lookup"><span data-stu-id="69d51-2321">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="69d51-2322">Ajout d’un indicateur de non-format pour l’affichage des journaux d’activité de génération</span><span class="sxs-lookup"><span data-stu-id="69d51-2322">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="69d51-2323">ACS</span><span class="sxs-lookup"><span data-stu-id="69d51-2323">ACS</span></span>
* <span data-ttu-id="69d51-2324">Modification de la commande `install-connector` pour configurer le nom de domaine complet maître AKS</span><span class="sxs-lookup"><span data-stu-id="69d51-2324">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="69d51-2325">Correction de la création d’attribution de rôle pour vnet-subnet-id lorsque le principal de service n’est pas spécifié, et pour skip-role-assignemnt</span><span class="sxs-lookup"><span data-stu-id="69d51-2325">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="69d51-2326">AppService</span><span class="sxs-lookup"><span data-stu-id="69d51-2326">AppService</span></span>

* <span data-ttu-id="69d51-2327">Ajout de la prise en charge de la gestion des opérations (continues et déclenchées) des Webjobs</span><span class="sxs-lookup"><span data-stu-id="69d51-2327">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="69d51-2328">az webapp config set prend en charge la propriété FTS-state. Aussi ajout de la prise en charge de az functionapp config set & show</span><span class="sxs-lookup"><span data-stu-id="69d51-2328">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="69d51-2329">Ajout de la prise en charge de Bring Your Own Storage pour les applications web</span><span class="sxs-lookup"><span data-stu-id="69d51-2329">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="69d51-2330">Ajout de la prise en charge du référencement et de la restauration des applications web supprimées</span><span class="sxs-lookup"><span data-stu-id="69d51-2330">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="69d51-2331">Batch</span><span class="sxs-lookup"><span data-stu-id="69d51-2331">Batch</span></span>
* <span data-ttu-id="69d51-2332">Modification de l’ajout des tâches via `--json-file` pour prendre en charge la syntaxe AddTaskCollectionParameter</span><span class="sxs-lookup"><span data-stu-id="69d51-2332">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="69d51-2333">Mise à jour de la documentation des formats `--json-file` acceptés</span><span class="sxs-lookup"><span data-stu-id="69d51-2333">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="69d51-2334">Ajout de `--max-tasks-per-node-option` à `batch pool create`</span><span class="sxs-lookup"><span data-stu-id="69d51-2334">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="69d51-2335">Modification du comportement de `batch account` pour afficher la connexion au compte si aucune option n’est spécifiée</span><span class="sxs-lookup"><span data-stu-id="69d51-2335">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="69d51-2336">Batch AI</span><span class="sxs-lookup"><span data-stu-id="69d51-2336">Batch AI</span></span> 
* <span data-ttu-id="69d51-2337">Correction de l’échec de création de compte de stockage automatique dans la commande `batchai cluster create`</span><span class="sxs-lookup"><span data-stu-id="69d51-2337">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="69d51-2338">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="69d51-2338">Cognitive Services</span></span>
* <span data-ttu-id="69d51-2339">Ajout de Completer pour les arguments `--sku`, `--kind` et `--location`</span><span class="sxs-lookup"><span data-stu-id="69d51-2339">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="69d51-2340">Ajout de la commande `cognitiveservices account list-usage`</span><span class="sxs-lookup"><span data-stu-id="69d51-2340">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="69d51-2341">Ajout de la commande `cognitiveservices account list-kinds`</span><span class="sxs-lookup"><span data-stu-id="69d51-2341">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="69d51-2342">Ajout de la commande `cognitiveservices account list`</span><span class="sxs-lookup"><span data-stu-id="69d51-2342">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="69d51-2343">`cognitiveservices list` déconseillé</span><span class="sxs-lookup"><span data-stu-id="69d51-2343">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="69d51-2344">Modification de `--name` afin de le rendre facultatif pour `cognitiveservices account list-skus`</span><span class="sxs-lookup"><span data-stu-id="69d51-2344">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="69d51-2345">Conteneur</span><span class="sxs-lookup"><span data-stu-id="69d51-2345">Container</span></span>
* <span data-ttu-id="69d51-2346">Ajout de la possibilité de redémarrer et d’arrêter un groupe de conteneurs en cours d’exécution</span><span class="sxs-lookup"><span data-stu-id="69d51-2346">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="69d51-2347">Ajout de `--network-profile` pour autoriser le passage dans un profil réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-2347">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="69d51-2348">Ajout de `--subnet` et `--vnet_name` pour autoriser la création de groupes de conteneurs dans un réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="69d51-2348">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="69d51-2349">Modification de la sortie de table pour afficher l’état du groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="69d51-2349">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="69d51-2350">DataLake</span><span class="sxs-lookup"><span data-stu-id="69d51-2350">Datalake</span></span>
* <span data-ttu-id="69d51-2351">Ajout de commandes pour les règles de réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="69d51-2351">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="69d51-2352">Shell interactif</span><span class="sxs-lookup"><span data-stu-id="69d51-2352">Interactive Shell</span></span>
* <span data-ttu-id="69d51-2353">Correction des erreurs sur Windows où les commandes ne s’exécutent pas correctement</span><span class="sxs-lookup"><span data-stu-id="69d51-2353">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="69d51-2354">Correction du problème de chargement de commande dans le Shell interactif provoqué par les objets déconseillés</span><span class="sxs-lookup"><span data-stu-id="69d51-2354">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="69d51-2355">IoT</span><span class="sxs-lookup"><span data-stu-id="69d51-2355">IoT</span></span>
* <span data-ttu-id="69d51-2356">Ajout de la prise en charge du routage des hubs IoT</span><span class="sxs-lookup"><span data-stu-id="69d51-2356">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="69d51-2357">Key Vault</span><span class="sxs-lookup"><span data-stu-id="69d51-2357">Key Vault</span></span>
* <span data-ttu-id="69d51-2358">Correction de l’importation de la clé Key Vault pour les clés RSA</span><span class="sxs-lookup"><span data-stu-id="69d51-2358">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="69d51-2359">Réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-2359">Network</span></span>
* <span data-ttu-id="69d51-2360">Ajout des commandes `network public-ip prefix` pour prendre en charge les fonctionnalités de préfixes d’adresses IP publiques</span><span class="sxs-lookup"><span data-stu-id="69d51-2360">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="69d51-2361">Ajout des commandes `network service-endpoint` pour prendre en charge les fonctionnalités de stratégie de point de terminaison de service</span><span class="sxs-lookup"><span data-stu-id="69d51-2361">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="69d51-2362">Ajout des commandes `network lb outbound-rule` pour prendre en charge la création de règles de trafic sortant d’un équilibreur de charge standard</span><span class="sxs-lookup"><span data-stu-id="69d51-2362">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="69d51-2363">Ajout de `--public-ip-prefix` à `network lb frontend-ip create/update` pour prendre en charge les configurations IP frontales à l’aide de préfixes d’adresses IP publiques</span><span class="sxs-lookup"><span data-stu-id="69d51-2363">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="69d51-2364">Ajout de `--enable-tcp-reset` à `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span><span class="sxs-lookup"><span data-stu-id="69d51-2364">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="69d51-2365">Ajout de `--disable-outbound-snat` à `network lb rule create/update`</span><span class="sxs-lookup"><span data-stu-id="69d51-2365">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="69d51-2366">Autoriser `network watcher flow-log show/configure` à être utilisé avec des groupes de sécurité réseau classiques</span><span class="sxs-lookup"><span data-stu-id="69d51-2366">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="69d51-2367">Ajouter la commande `network watcher run-configuration-diagnostic`</span><span class="sxs-lookup"><span data-stu-id="69d51-2367">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="69d51-2368">Correction de la commande `network watcher test-connectivity` et ajout des propriétés `--method`, `--valid-status-codes` et `--headers`</span><span class="sxs-lookup"><span data-stu-id="69d51-2368">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="69d51-2369">`network express-route create/update`: ajout de l’indicateur `--allow-global-reach`</span><span class="sxs-lookup"><span data-stu-id="69d51-2369">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="69d51-2370">`network vnet subnet create/update`: ajout de la prise en charge de `--delegation`</span><span class="sxs-lookup"><span data-stu-id="69d51-2370">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="69d51-2371">Ajout de la commande `network vnet subnet list-available-delegations`</span><span class="sxs-lookup"><span data-stu-id="69d51-2371">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="69d51-2372">`network traffic-manager profile create/update`: ajout de la prise en charge de `--interval`, `--timeout` et `--max-failures` pour les options Deprecated de configuration du moniteur `--monitor-path`, `--monitor-port` et `--monitor-protocol` en faveur de `--path`, `--port`, `--protocol`</span><span class="sxs-lookup"><span data-stu-id="69d51-2372">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="69d51-2373">`network lb frontend-ip create/update`: correction de la logique de réglage de la méthode d’allocation d’adresses IP privées. Si une adresse IP privée est fournie, l’allocation sera statique. Si aucune adresse IP privée n’est fournie, ou qu’une chaîne vide est fournie pour l’adresse IP privée, l’allocation est dynamique.</span><span class="sxs-lookup"><span data-stu-id="69d51-2373">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="69d51-2374">`dns record-set * create/update`: ajout de la prise en charge de `--target-resource`</span><span class="sxs-lookup"><span data-stu-id="69d51-2374">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="69d51-2375">Ajout des commandes `network interface-endpoint` pour interroger les objets de point de terminaison de l’interface</span><span class="sxs-lookup"><span data-stu-id="69d51-2375">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="69d51-2376">Ajout de `network profile show/list/delete` pour la gestion partielle des profils de réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-2376">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="69d51-2377">Ajout des commandes `network express-route peering connection` pour gérer les connexions de peering entre les routes ExpressRoutes</span><span class="sxs-lookup"><span data-stu-id="69d51-2377">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="69d51-2378">SGBDR</span><span class="sxs-lookup"><span data-stu-id="69d51-2378">RDBMS</span></span>
* <span data-ttu-id="69d51-2379">Ajout de la prise en charge du service MariaDB</span><span class="sxs-lookup"><span data-stu-id="69d51-2379">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="69d51-2380">Réservation</span><span class="sxs-lookup"><span data-stu-id="69d51-2380">Reservation</span></span>
* <span data-ttu-id="69d51-2381">Ajout de CosmosDb dans le type d’énumération des ressources réservées</span><span class="sxs-lookup"><span data-stu-id="69d51-2381">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="69d51-2382">Ajout de la propriété de nom dans un modèle Patch</span><span class="sxs-lookup"><span data-stu-id="69d51-2382">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="69d51-2383">Gérer l’application</span><span class="sxs-lookup"><span data-stu-id="69d51-2383">Manage App</span></span>
* <span data-ttu-id="69d51-2384">Correction du bogue dans `managedapp create --kind MarketPlace` à l’origine du blocage de la création d’instance d’une application Marketplace gérée</span><span class="sxs-lookup"><span data-stu-id="69d51-2384">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="69d51-2385">Modification des commandes `feature` afin qu’elles soient limitées aux profils pris en charge</span><span class="sxs-lookup"><span data-stu-id="69d51-2385">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="69d51-2386">Role</span><span class="sxs-lookup"><span data-stu-id="69d51-2386">Role</span></span>
* <span data-ttu-id="69d51-2387">Ajout de la prise en charge pour répertorier les appartenances de l’utilisateur à des groupes</span><span class="sxs-lookup"><span data-stu-id="69d51-2387">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="69d51-2388">SignalR</span><span class="sxs-lookup"><span data-stu-id="69d51-2388">SignalR</span></span>
* <span data-ttu-id="69d51-2389">Première version</span><span class="sxs-lookup"><span data-stu-id="69d51-2389">First release</span></span>

### <a name="storage"></a><span data-ttu-id="69d51-2390">Stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-2390">Storage</span></span>
* <span data-ttu-id="69d51-2391">Ajout du paramètre `--auth-mode login` pour l’utilisation des informations d’identification de l’utilisateur pour autoriser les objets blob et les files d’attente</span><span class="sxs-lookup"><span data-stu-id="69d51-2391">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="69d51-2392">Ajout de `storage container immutability-policy/legal-hold` pour gérer le stockage immuable</span><span class="sxs-lookup"><span data-stu-id="69d51-2392">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="69d51-2393">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="69d51-2393">VM</span></span>
* <span data-ttu-id="69d51-2394">Correction d’un problème `vm create --generate-ssh-keys` qui remplace le fichier de clé privée si le fichier de clé publique est manquant (#4725, #6780)</span><span class="sxs-lookup"><span data-stu-id="69d51-2394">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="69d51-2395">Ajout de la prise en charge pour la galerie d’images partagée via `az sig`</span><span class="sxs-lookup"><span data-stu-id="69d51-2395">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="69d51-2396">28 Août 2018</span><span class="sxs-lookup"><span data-stu-id="69d51-2396">August 28, 2018</span></span>

<span data-ttu-id="69d51-2397">Version 2.0.45</span><span class="sxs-lookup"><span data-stu-id="69d51-2397">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="69d51-2398">Core</span><span class="sxs-lookup"><span data-stu-id="69d51-2398">Core</span></span>

* <span data-ttu-id="69d51-2399">Résolution du problème de chargement de fichier de configuration vide</span><span class="sxs-lookup"><span data-stu-id="69d51-2399">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="69d51-2400">Ajout de la prise en charge du profil `2018-03-01-hybrid` pour Azure Stack</span><span class="sxs-lookup"><span data-stu-id="69d51-2400">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="69d51-2401">ACR</span><span class="sxs-lookup"><span data-stu-id="69d51-2401">ACR</span></span>

* <span data-ttu-id="69d51-2402">Ajout d’une solution pour les opérations d’exécution sans les requêtes ARM</span><span class="sxs-lookup"><span data-stu-id="69d51-2402">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="69d51-2403">Exclusion des fichiers de contrôle de version (par exemple, .git, .gitignore) chargés par défaut dans les fichiers tar dans la commande `build`</span><span class="sxs-lookup"><span data-stu-id="69d51-2403">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="69d51-2404">ACS</span><span class="sxs-lookup"><span data-stu-id="69d51-2404">ACS</span></span>

* <span data-ttu-id="69d51-2405">Modification de `aks create` à la valeur par défaut sur les machines virtuelles `Standard_DS2_v2`</span><span class="sxs-lookup"><span data-stu-id="69d51-2405">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="69d51-2406">Modification de `aks get-credentials` afin d’appeler de nouvelles API pour l’obtention des informations d’identification des clusters</span><span class="sxs-lookup"><span data-stu-id="69d51-2406">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="69d51-2407">AppService</span><span class="sxs-lookup"><span data-stu-id="69d51-2407">AppService</span></span>

* <span data-ttu-id="69d51-2408">Prise en charge de CORS sur functionapp et webapp</span><span class="sxs-lookup"><span data-stu-id="69d51-2408">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="69d51-2409">Ajout de la prise en charge de la balise ARM sur les commandes de création</span><span class="sxs-lookup"><span data-stu-id="69d51-2409">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="69d51-2410">Modification de `[webapp|functionapp] identity show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="69d51-2410">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="69d51-2411">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="69d51-2411">Backup</span></span>

* <span data-ttu-id="69d51-2412">Modification de `backup vault backup-properties show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="69d51-2412">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="69d51-2413">Service de robot</span><span class="sxs-lookup"><span data-stu-id="69d51-2413">Bot Service</span></span>

* <span data-ttu-id="69d51-2414">Version initiale de l’interface CLI de Bot Service</span><span class="sxs-lookup"><span data-stu-id="69d51-2414">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="69d51-2415">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="69d51-2415">Cognitive Services</span></span>

* <span data-ttu-id="69d51-2416">Ajout du nouveau paramètre `--api-properties,` requis pour la création de certains services</span><span class="sxs-lookup"><span data-stu-id="69d51-2416">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="69d51-2417">IoT</span><span class="sxs-lookup"><span data-stu-id="69d51-2417">IoT</span></span>

* <span data-ttu-id="69d51-2418">Résolution du problème relatif à l’association de hubs liés</span><span class="sxs-lookup"><span data-stu-id="69d51-2418">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="69d51-2419">Superviser</span><span class="sxs-lookup"><span data-stu-id="69d51-2419">Monitor</span></span>

* <span data-ttu-id="69d51-2420">Ajout des commandes `monitor metrics alert` permettant de recevoir des alertes sur les métriques quasiment en temps réel</span><span class="sxs-lookup"><span data-stu-id="69d51-2420">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="69d51-2421">Commandes `monitor alert` déconseillées</span><span class="sxs-lookup"><span data-stu-id="69d51-2421">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="69d51-2422">Réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-2422">Network</span></span>

* <span data-ttu-id="69d51-2423">Modification de `network application-gateway ssl-policy predefined show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="69d51-2423">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="69d51-2424">Ressource</span><span class="sxs-lookup"><span data-stu-id="69d51-2424">Resource</span></span>

* <span data-ttu-id="69d51-2425">Modification de `provider operation show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="69d51-2425">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="69d51-2426">Stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-2426">Storage</span></span>

* <span data-ttu-id="69d51-2427">Modification de `storage share policy show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="69d51-2427">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="69d51-2428">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="69d51-2428">VM</span></span>

* <span data-ttu-id="69d51-2429">Modification de `vm/vmss identity show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="69d51-2429">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="69d51-2430">Remplacement de `--storage-caching` pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="69d51-2430">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="69d51-2431">14 août 2018</span><span class="sxs-lookup"><span data-stu-id="69d51-2431">Auguest 14, 2018</span></span>

<span data-ttu-id="69d51-2432">Version 2.0.44</span><span class="sxs-lookup"><span data-stu-id="69d51-2432">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="69d51-2433">Core</span><span class="sxs-lookup"><span data-stu-id="69d51-2433">Core</span></span>

* <span data-ttu-id="69d51-2434">Correction de l’affichage numérique dans la sortie `table`</span><span class="sxs-lookup"><span data-stu-id="69d51-2434">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="69d51-2435">Ajout du format de sortie YAML</span><span class="sxs-lookup"><span data-stu-id="69d51-2435">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="69d51-2436">Télémétrie</span><span class="sxs-lookup"><span data-stu-id="69d51-2436">Telemetry</span></span>

* <span data-ttu-id="69d51-2437">Amélioration des rapports de télémétrie</span><span class="sxs-lookup"><span data-stu-id="69d51-2437">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="69d51-2438">ACR</span><span class="sxs-lookup"><span data-stu-id="69d51-2438">ACR</span></span>

* <span data-ttu-id="69d51-2439">Ajout des commandes `content-trust policy`</span><span class="sxs-lookup"><span data-stu-id="69d51-2439">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="69d51-2440">Résolution du problème où `.dockerignore` n’était pas honorée</span><span class="sxs-lookup"><span data-stu-id="69d51-2440">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="69d51-2441">ACS</span><span class="sxs-lookup"><span data-stu-id="69d51-2441">ACS</span></span>

* <span data-ttu-id="69d51-2442">Modification de `az acs/aks install-cli` afin d’effectuer l’installation sous `%USERPROFILE%\.azure-kubectl` sur Windows</span><span class="sxs-lookup"><span data-stu-id="69d51-2442">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="69d51-2443">Modification de `az aks install-connector` afin de détecter si le cluster dispose du contrôle RBAC et de configurer le connecteur ACI correctement</span><span class="sxs-lookup"><span data-stu-id="69d51-2443">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="69d51-2444">Remplacement par l’attribution de rôle au sous-réseau lorsque l’attribution est fournie</span><span class="sxs-lookup"><span data-stu-id="69d51-2444">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="69d51-2445">Ajout de l’option nouveau « ignorer attribution de rôle » pour le sous-réseau lorsque l’attribution est fournie</span><span class="sxs-lookup"><span data-stu-id="69d51-2445">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="69d51-2446">Modification ignorant l’attribution de rôle au sous-réseau lorsque l’attribution existe déjà</span><span class="sxs-lookup"><span data-stu-id="69d51-2446">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="69d51-2447">AppService</span><span class="sxs-lookup"><span data-stu-id="69d51-2447">AppService</span></span>

* <span data-ttu-id="69d51-2448">Correction d’un bogue empêchant de créer une application de fonction à l’aide de comptes de stockage dans les groupes de ressources externes</span><span class="sxs-lookup"><span data-stu-id="69d51-2448">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="69d51-2449">Correction d’un incident lors du déploiement de dossier zip</span><span class="sxs-lookup"><span data-stu-id="69d51-2449">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="69d51-2450">Batch AI</span><span class="sxs-lookup"><span data-stu-id="69d51-2450">BatchAI</span></span>

* <span data-ttu-id="69d51-2451">Modification de la sortie de l’enregistreur d’événements pour la création du compte de stockage automatique afin de spécifier l’information « ressource *groupe*».</span><span class="sxs-lookup"><span data-stu-id="69d51-2451">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="69d51-2452">Conteneur</span><span class="sxs-lookup"><span data-stu-id="69d51-2452">Container</span></span>

* <span data-ttu-id="69d51-2453">Ajout de `--secure-environment-variables` pour transmettre des variables d’environnement sécurisées vers un conteneur</span><span class="sxs-lookup"><span data-stu-id="69d51-2453">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="69d51-2454">IoT</span><span class="sxs-lookup"><span data-stu-id="69d51-2454">IoT</span></span>

* <span data-ttu-id="69d51-2455">[CHANGEMENT CASSANT] Suppression des commandes obsolètes déplacées vers l’extension iot</span><span class="sxs-lookup"><span data-stu-id="69d51-2455">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="69d51-2456">Mise à jour des éléments afin de ne pas prendre en compte le domaine `azure-devices.net`</span><span class="sxs-lookup"><span data-stu-id="69d51-2456">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="69d51-2457">Iot Central</span><span class="sxs-lookup"><span data-stu-id="69d51-2457">Iot Central</span></span>

* <span data-ttu-id="69d51-2458">Version initiale du module IoT Central</span><span class="sxs-lookup"><span data-stu-id="69d51-2458">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="69d51-2459">KeyVault</span><span class="sxs-lookup"><span data-stu-id="69d51-2459">KeyVault</span></span>


* <span data-ttu-id="69d51-2460">Ajout des commandes pour la gestion des comptes de stockage et les définitions SAS</span><span class="sxs-lookup"><span data-stu-id="69d51-2460">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="69d51-2461">Ajout de commandes pour les règles réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-2461">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="69d51-2462">Ajout du paramètre `--id` aux opérations relatives au mots de passe confidentiels, clés et certificats</span><span class="sxs-lookup"><span data-stu-id="69d51-2462">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="69d51-2463">Ajout de la prise en charge pour la version multi-api avec gestion des coffres de clés</span><span class="sxs-lookup"><span data-stu-id="69d51-2463">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="69d51-2464">Ajout de la prise en charge pour la version multi-api avec plan de données des coffres de clés</span><span class="sxs-lookup"><span data-stu-id="69d51-2464">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="69d51-2465">Relais</span><span class="sxs-lookup"><span data-stu-id="69d51-2465">Relay</span></span>

* <span data-ttu-id="69d51-2466">Version initiale</span><span class="sxs-lookup"><span data-stu-id="69d51-2466">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="69d51-2467">SQL</span><span class="sxs-lookup"><span data-stu-id="69d51-2467">Sql</span></span>

* <span data-ttu-id="69d51-2468">Ajout des commandes `sql failover-group`</span><span class="sxs-lookup"><span data-stu-id="69d51-2468">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="69d51-2469">Stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-2469">Storage</span></span>

* <span data-ttu-id="69d51-2470">[CHANGEMENT CASSANT] Modification de `storage account show-usage` afin d’exiger le paramètre `--location` et de répertorier par région</span><span class="sxs-lookup"><span data-stu-id="69d51-2470">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="69d51-2471">Modification du paramètre `--resource-group` afin de le rendre facultatif pour les commandes `storage account`</span><span class="sxs-lookup"><span data-stu-id="69d51-2471">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="69d51-2472">Suppression des avertissements concernant l’échec de la condition préalable pour les défaillances isolées dans les commandes batch pour les messages agrégés uniques</span><span class="sxs-lookup"><span data-stu-id="69d51-2472">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="69d51-2473">Modification des commandes `[blob|file] delete-batch` afin de ne plus produire des tableaux ayant la valeur null</span><span class="sxs-lookup"><span data-stu-id="69d51-2473">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="69d51-2474">Modification des commandes `blob [download|upload|delete-batch]` afin de lire le jeton de SAS à partir de l’url du conteneur</span><span class="sxs-lookup"><span data-stu-id="69d51-2474">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="69d51-2475">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="69d51-2475">VM</span></span>

* <span data-ttu-id="69d51-2476">Ajout des filtres courants à `vm list-skus` pour une plus grande simplicité d’utilisation</span><span class="sxs-lookup"><span data-stu-id="69d51-2476">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="69d51-2477">31 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="69d51-2477">July 31, 2018</span></span>

<span data-ttu-id="69d51-2478">Version 2.0.43</span><span class="sxs-lookup"><span data-stu-id="69d51-2478">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="69d51-2479">ACR</span><span class="sxs-lookup"><span data-stu-id="69d51-2479">ACR</span></span>

* <span data-ttu-id="69d51-2480">Ajout de l’indicateur `--with-secure-properties` à la commande `acr build-task show`</span><span class="sxs-lookup"><span data-stu-id="69d51-2480">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="69d51-2481">Ajout de la commande `acr build-task update-build`</span><span class="sxs-lookup"><span data-stu-id="69d51-2481">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="69d51-2482">ACS</span><span class="sxs-lookup"><span data-stu-id="69d51-2482">ACS</span></span>

* <span data-ttu-id="69d51-2483">Retour au return 0 (réussite) à la fin de `az aks browse` en appuyant sur [Ctrl + C]</span><span class="sxs-lookup"><span data-stu-id="69d51-2483">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="69d51-2484">Batch</span><span class="sxs-lookup"><span data-stu-id="69d51-2484">Batch</span></span>

* <span data-ttu-id="69d51-2485">Correction du bug lors de l’affichage des jetons AAD dans le Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="69d51-2485">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="69d51-2486">Conteneur</span><span class="sxs-lookup"><span data-stu-id="69d51-2486">Container</span></span>

* <span data-ttu-id="69d51-2487">Suppression de l’exigence pour `--log-analytics-workspace-key` pour le nom ou l’identifiant lors de l’abonnement standard</span><span class="sxs-lookup"><span data-stu-id="69d51-2487">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="69d51-2488">Réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-2488">Network</span></span>

* <span data-ttu-id="69d51-2489">Ajout du serveur DNS au profil du 09/03/2017 pour Azure Stack</span><span class="sxs-lookup"><span data-stu-id="69d51-2489">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="69d51-2490">Ressource</span><span class="sxs-lookup"><span data-stu-id="69d51-2490">Resource</span></span>

* <span data-ttu-id="69d51-2491">Ajout de `--rollback-on-error` à `group deployment create` pour exécuter un déploiement correct et connu en cas d’erreur</span><span class="sxs-lookup"><span data-stu-id="69d51-2491">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="69d51-2492">Correction d’un problème où `--parameters {}` avec `group deployment create` entraînait une erreur</span><span class="sxs-lookup"><span data-stu-id="69d51-2492">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="69d51-2493">Role</span><span class="sxs-lookup"><span data-stu-id="69d51-2493">Role</span></span>

* <span data-ttu-id="69d51-2494">Ajout de la prise en charge du profil stack du 09/03/2017</span><span class="sxs-lookup"><span data-stu-id="69d51-2494">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="69d51-2495">Correction d’un problème où les paramètres de mise à jour génériques à `app update` ne fonctionnaient pas correctement</span><span class="sxs-lookup"><span data-stu-id="69d51-2495">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="69d51-2496">Recherche</span><span class="sxs-lookup"><span data-stu-id="69d51-2496">Search</span></span>

* <span data-ttu-id="69d51-2497">Ajout de commandes pour le service de recherches d’Azure</span><span class="sxs-lookup"><span data-stu-id="69d51-2497">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="69d51-2498">Service Bus</span><span class="sxs-lookup"><span data-stu-id="69d51-2498">Service Bus</span></span>

* <span data-ttu-id="69d51-2499">Ajout d’un groupe de commandes de migration pour migrer un espace de noms d’un Service Bus Standard à un Premium</span><span class="sxs-lookup"><span data-stu-id="69d51-2499">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="69d51-2500">Ajout de nouvelles propriétés facultatives à la file d’attente du Service Bus et à l’abonnement</span><span class="sxs-lookup"><span data-stu-id="69d51-2500">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="69d51-2501">`--enable-batched-operations` et `--enable-dead-lettering-on-message-expiration` dans `queue`</span><span class="sxs-lookup"><span data-stu-id="69d51-2501">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="69d51-2502">`--dead-letter-on-filter-exceptions` dans `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="69d51-2502">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="69d51-2503">Stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-2503">Storage</span></span>

* <span data-ttu-id="69d51-2504">Ajout de la prise en charge du téléchargement de fichiers volumineux à l’aide d’une connexion unique</span><span class="sxs-lookup"><span data-stu-id="69d51-2504">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="69d51-2505">Conversion des commandes `show` qui manquaient d’échouer avec le code de sortie 3 sur une ressource manquante</span><span class="sxs-lookup"><span data-stu-id="69d51-2505">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="69d51-2506">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="69d51-2506">VM</span></span>

* <span data-ttu-id="69d51-2507">Ajout d’une prise en charge pour lister les groupes disponibles par abonnement</span><span class="sxs-lookup"><span data-stu-id="69d51-2507">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="69d51-2508">Ajout de la prise en charge de `StandardSSD_LRS`</span><span class="sxs-lookup"><span data-stu-id="69d51-2508">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="69d51-2509">Ajout d’une prise en charge des groupes de sécurité d’application dans la création du groupe identique de machines virtuelles</span><span class="sxs-lookup"><span data-stu-id="69d51-2509">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="69d51-2510">[CHANGEMENT CASSANT] Changement de `[vm|vmss] create`, `[vm|vmss] identity assign`, et `[vm|vmss] identity remove` pour sortir les identités des utilisateurs au format de dictionnaire</span><span class="sxs-lookup"><span data-stu-id="69d51-2510">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="69d51-2511">18 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="69d51-2511">July 18, 2018</span></span>

<span data-ttu-id="69d51-2512">Version 2.0.42</span><span class="sxs-lookup"><span data-stu-id="69d51-2512">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="69d51-2513">Core</span><span class="sxs-lookup"><span data-stu-id="69d51-2513">Core</span></span>

* <span data-ttu-id="69d51-2514">Ajout de la prise en charge de la connexion basée sur le navigateur dans la fenêtre d’interpréteur de commandes Windows pour Linux</span><span class="sxs-lookup"><span data-stu-id="69d51-2514">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="69d51-2515">Ajout de l’indicateur `--force-string` pour toutes les commandes de mise à jour générique</span><span class="sxs-lookup"><span data-stu-id="69d51-2515">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="69d51-2516">[CHANGEMENT CASSANT] Modification des commandes « d’affichage » pour connecter le message d’erreur et échec avec un code de sortie de 3 sur une ressource manquante</span><span class="sxs-lookup"><span data-stu-id="69d51-2516">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="69d51-2517">ACR</span><span class="sxs-lookup"><span data-stu-id="69d51-2517">ACR</span></span>

* <span data-ttu-id="69d51-2518">[CHANGEMENT CASSANT] Mise à jour de « --no-push » vers un indicateur pur dans la commande « ACR Build »</span><span class="sxs-lookup"><span data-stu-id="69d51-2518">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="69d51-2519">Ajout des commandes `show` et `update` sous le groupe `acr repository`</span><span class="sxs-lookup"><span data-stu-id="69d51-2519">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="69d51-2520">Ajout de l’indicateur `--detail` à `show-manifests` et `show-tags` pour afficher des informations plus détaillées</span><span class="sxs-lookup"><span data-stu-id="69d51-2520">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="69d51-2521">Ajout du paramètre `--image` pour prendre en charge l’obtention des détails de build ou des journaux d’activité par une image</span><span class="sxs-lookup"><span data-stu-id="69d51-2521">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="69d51-2522">ACS</span><span class="sxs-lookup"><span data-stu-id="69d51-2522">ACS</span></span>

* <span data-ttu-id="69d51-2523">Modification de `az aks create` en sortie d’erreur si `--max-pods` est inférieur à 5</span><span class="sxs-lookup"><span data-stu-id="69d51-2523">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="69d51-2524">AppService</span><span class="sxs-lookup"><span data-stu-id="69d51-2524">AppService</span></span>

* <span data-ttu-id="69d51-2525">Ajout de la prise en charge pour les références (SKU) PremiumV2</span><span class="sxs-lookup"><span data-stu-id="69d51-2525">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="69d51-2526">Batch</span><span class="sxs-lookup"><span data-stu-id="69d51-2526">Batch</span></span>

* <span data-ttu-id="69d51-2527">Correction d’un bogue relatif à l’utilisation des informations d’identification de jeton dans le mode Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="69d51-2527">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="69d51-2528">Modification de l’entrée JSON pour respecter la casse</span><span class="sxs-lookup"><span data-stu-id="69d51-2528">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="69d51-2529">Batch AI</span><span class="sxs-lookup"><span data-stu-id="69d51-2529">Batch AI</span></span>

* <span data-ttu-id="69d51-2530">Correction de la commande `az batchai job exec`</span><span class="sxs-lookup"><span data-stu-id="69d51-2530">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="69d51-2531">Conteneur</span><span class="sxs-lookup"><span data-stu-id="69d51-2531">Container</span></span>

* <span data-ttu-id="69d51-2532">Suppression des exigences pour le nom d’utilisateur et le mot de passe pour les registres non dockerhub</span><span class="sxs-lookup"><span data-stu-id="69d51-2532">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="69d51-2533">Correction de l’erreur lors de la création de groupes de conteneur à partir du fichier yaml</span><span class="sxs-lookup"><span data-stu-id="69d51-2533">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="69d51-2534">Réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-2534">Network</span></span>

* <span data-ttu-id="69d51-2535">Ajout de la prise en charge de `--no-wait` pour `network nic [create|update|delete]`</span><span class="sxs-lookup"><span data-stu-id="69d51-2535">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="69d51-2536">Ajout de `network nic wait`</span><span class="sxs-lookup"><span data-stu-id="69d51-2536">Added `network nic wait`</span></span>
* <span data-ttu-id="69d51-2537">Argument `--ids` déconseillé pour `network vnet [subnet|peering] list`</span><span class="sxs-lookup"><span data-stu-id="69d51-2537">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="69d51-2538">Ajout de l’indicateur `--include-default` pour inclure les règles de sécurité par défaut dans la sortie de `network nsg rule list`</span><span class="sxs-lookup"><span data-stu-id="69d51-2538">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="69d51-2539">Ressource</span><span class="sxs-lookup"><span data-stu-id="69d51-2539">Resource</span></span>

* <span data-ttu-id="69d51-2540">Ajout de la prise en charge de `--no-wait` pour `group deployment delete`</span><span class="sxs-lookup"><span data-stu-id="69d51-2540">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="69d51-2541">Ajout de la prise en charge de `--no-wait` pour `deployment delete`</span><span class="sxs-lookup"><span data-stu-id="69d51-2541">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="69d51-2542">Ajout de la commande `deployment wait`</span><span class="sxs-lookup"><span data-stu-id="69d51-2542">Added `deployment wait` command</span></span>
* <span data-ttu-id="69d51-2543">Résolution du problème qui causait l’affichage par erreur des commandes `az deployment` du niveau de l’abonnement pour le profil 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="69d51-2543">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="69d51-2544">SQL</span><span class="sxs-lookup"><span data-stu-id="69d51-2544">SQL</span></span>

* <span data-ttu-id="69d51-2545">Résolution de l’erreur « Le nom du groupe de ressources fourni ne correspond pas au nom de l’URL » lors de la spécification du nom du pool élastique pour les commandes `sql db copy` et `sql db replica create`</span><span class="sxs-lookup"><span data-stu-id="69d51-2545">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="69d51-2546">Autoriser la configuration de SQL Server par défaut en exécutant `az configure --defaults sql-server=<name>`</span><span class="sxs-lookup"><span data-stu-id="69d51-2546">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="69d51-2547">Implémentation de formateurs de table pour les commandes `sql server`, `sql server firewall-rule`, `sql list-usages` et `sql show-usage`</span><span class="sxs-lookup"><span data-stu-id="69d51-2547">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="69d51-2548">Stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-2548">Storage</span></span>

* <span data-ttu-id="69d51-2549">Ajout de la propriété `pageRanges` à la sortie `storage blob show` qui sera renseignée pour les objets blob de pages</span><span class="sxs-lookup"><span data-stu-id="69d51-2549">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="69d51-2550">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="69d51-2550">VM</span></span>

* <span data-ttu-id="69d51-2551">[CHANGEMENT CASSANT] Modification de `vmss create` pour utiliser `Standard_DS1_v2` comme taille d’instance par défaut</span><span class="sxs-lookup"><span data-stu-id="69d51-2551">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="69d51-2552">Ajout de la prise en charge de `--no-wait` pour `vm extension [set|delete]` et `vmss extension [set|delete]`</span><span class="sxs-lookup"><span data-stu-id="69d51-2552">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="69d51-2553">Ajout de `vm extension wait`</span><span class="sxs-lookup"><span data-stu-id="69d51-2553">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="69d51-2554">3 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="69d51-2554">July 3, 2018</span></span>

<span data-ttu-id="69d51-2555">Version 2.0.41</span><span class="sxs-lookup"><span data-stu-id="69d51-2555">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="69d51-2556">AKS</span><span class="sxs-lookup"><span data-stu-id="69d51-2556">AKS</span></span>

* <span data-ttu-id="69d51-2557">Modification de la surveillance pour utiliser l’ID d’abonnement</span><span class="sxs-lookup"><span data-stu-id="69d51-2557">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="69d51-2558">3 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="69d51-2558">July 3, 2018</span></span>

<span data-ttu-id="69d51-2559">Version 2.0.40</span><span class="sxs-lookup"><span data-stu-id="69d51-2559">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="69d51-2560">Core</span><span class="sxs-lookup"><span data-stu-id="69d51-2560">Core</span></span>

* <span data-ttu-id="69d51-2561">Ajout d’un nouveau flux de code d’autorisation pour une connexion interactive</span><span class="sxs-lookup"><span data-stu-id="69d51-2561">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="69d51-2562">ACR</span><span class="sxs-lookup"><span data-stu-id="69d51-2562">ACR</span></span>

* <span data-ttu-id="69d51-2563">Ajout de l’interrogation de l’état du build</span><span class="sxs-lookup"><span data-stu-id="69d51-2563">Added polling build status</span></span>
* <span data-ttu-id="69d51-2564">Ajout de la prise en charge des valeurs d’énumération ne respectant pas la casse</span><span class="sxs-lookup"><span data-stu-id="69d51-2564">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="69d51-2565">Ajout des paramètres `--top` et `--orderby` pour `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="69d51-2565">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="69d51-2566">ACS</span><span class="sxs-lookup"><span data-stu-id="69d51-2566">ACS</span></span>

* <span data-ttu-id="69d51-2567">[CHANGEMENT CASSANT] Active le contrôle d’accès en fonction du rôle Kubernetes par défaut</span><span class="sxs-lookup"><span data-stu-id="69d51-2567">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="69d51-2568">Ajout de l’argument `--disable-rbac` et dépréciation de `--enable-rbac` dans la mesure où il s’agit actuellement de la valeur par défaut</span><span class="sxs-lookup"><span data-stu-id="69d51-2568">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="69d51-2569">Mise à jour des options de la commande `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="69d51-2569">Updated options for `aks browse` command.</span></span> <span data-ttu-id="69d51-2570">Ajout de la prise en charge de `--listen-port`</span><span class="sxs-lookup"><span data-stu-id="69d51-2570">Added `--listen-port` support</span></span>
* <span data-ttu-id="69d51-2571">Mise à jour du package de graphique Helm par défaut pour la commande `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="69d51-2571">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="69d51-2572">Use virtual-kubelet-for-aks-latest.tgz</span><span class="sxs-lookup"><span data-stu-id="69d51-2572">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="69d51-2573">Ajout des commandes `aks enable-addons` et `aks disable-addons` pour mettre à jour un cluster existant</span><span class="sxs-lookup"><span data-stu-id="69d51-2573">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="69d51-2574">AppService</span><span class="sxs-lookup"><span data-stu-id="69d51-2574">AppService</span></span>

* <span data-ttu-id="69d51-2575">Ajout de la prise en charge de la désactivation d’identité via `webapp identity remove`</span><span class="sxs-lookup"><span data-stu-id="69d51-2575">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="69d51-2576">Suppression de la balise `preview` pour la fonctionnalité Identité</span><span class="sxs-lookup"><span data-stu-id="69d51-2576">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="69d51-2577">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="69d51-2577">Backup</span></span>

* <span data-ttu-id="69d51-2578">Mise à jour de la définition du module</span><span class="sxs-lookup"><span data-stu-id="69d51-2578">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="69d51-2579">Batch AI</span><span class="sxs-lookup"><span data-stu-id="69d51-2579">BatchAI</span></span>

* <span data-ttu-id="69d51-2580">Correction de la sortie de table pour les commandes `batchai cluster node list` et `batchai job node list`</span><span class="sxs-lookup"><span data-stu-id="69d51-2580">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="69d51-2581">Cloud</span><span class="sxs-lookup"><span data-stu-id="69d51-2581">Cloud</span></span>

* <span data-ttu-id="69d51-2582">Ajout du suffixe de serveur `acr login` à la configuration du cloud</span><span class="sxs-lookup"><span data-stu-id="69d51-2582">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="69d51-2583">Conteneur</span><span class="sxs-lookup"><span data-stu-id="69d51-2583">Container</span></span>

* <span data-ttu-id="69d51-2584">Modification de `container create` sur valeur par défaut en opération à long terme</span><span class="sxs-lookup"><span data-stu-id="69d51-2584">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="69d51-2585">Ajout des paramètres Log Analytics `--log-analytics-workspace` et `--log-analytics-workspace-key`</span><span class="sxs-lookup"><span data-stu-id="69d51-2585">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="69d51-2586">Ajout du paramètre `--protocol` pour spécifier le protocole réseau à utiliser</span><span class="sxs-lookup"><span data-stu-id="69d51-2586">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="69d51-2587">Extension</span><span class="sxs-lookup"><span data-stu-id="69d51-2587">Extension</span></span>

* <span data-ttu-id="69d51-2588">Modification de `extension list-available` pour afficher uniquement les extensions compatibles avec la version CLI</span><span class="sxs-lookup"><span data-stu-id="69d51-2588">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="69d51-2589">Réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-2589">Network</span></span>

* <span data-ttu-id="69d51-2590">Résolution du problème où les types d’enregistrement étaient sensibles à la casse pour ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="69d51-2590">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="69d51-2591">Rdbms</span><span class="sxs-lookup"><span data-stu-id="69d51-2591">Rdbms</span></span>

* <span data-ttu-id="69d51-2592">Ajout des commandes `[postgres|myql] server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="69d51-2592">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="69d51-2593">Ressource</span><span class="sxs-lookup"><span data-stu-id="69d51-2593">Resource</span></span>

* <span data-ttu-id="69d51-2594">Ajout d’un nouveau groupe d’opérations `deployment`</span><span class="sxs-lookup"><span data-stu-id="69d51-2594">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="69d51-2595">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="69d51-2595">VM</span></span>

* <span data-ttu-id="69d51-2596">Ajout de la prise en charge de la suppression de l’identité affectée au système</span><span class="sxs-lookup"><span data-stu-id="69d51-2596">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="69d51-2597">25 juin 2018</span><span class="sxs-lookup"><span data-stu-id="69d51-2597">June 25, 2018</span></span>

<span data-ttu-id="69d51-2598">Version 2.0.39</span><span class="sxs-lookup"><span data-stu-id="69d51-2598">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="69d51-2599">Interface de ligne de commande</span><span class="sxs-lookup"><span data-stu-id="69d51-2599">CLI</span></span>

* <span data-ttu-id="69d51-2600">Mise à jour de la suppression du fichier dans le programme d’installation MSI pour résoudre le problème d’installation de l’extension</span><span class="sxs-lookup"><span data-stu-id="69d51-2600">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="69d51-2601">19 juin 2018</span><span class="sxs-lookup"><span data-stu-id="69d51-2601">June 19, 2018</span></span>

<span data-ttu-id="69d51-2602">Version 2.0.38</span><span class="sxs-lookup"><span data-stu-id="69d51-2602">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="69d51-2603">Core</span><span class="sxs-lookup"><span data-stu-id="69d51-2603">Core</span></span>

* <span data-ttu-id="69d51-2604">Ajout de la prise en charge globale de `--subscription` pour la plupart des commandes</span><span class="sxs-lookup"><span data-stu-id="69d51-2604">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="69d51-2605">ACR</span><span class="sxs-lookup"><span data-stu-id="69d51-2605">ACR</span></span>

* <span data-ttu-id="69d51-2606">Ajout de `azure-storage-blob` comme dépendance</span><span class="sxs-lookup"><span data-stu-id="69d51-2606">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="69d51-2607">Modification de la configuration de l’UC par défaut avec `acr build-task create` pour utiliser 2 cœurs</span><span class="sxs-lookup"><span data-stu-id="69d51-2607">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="69d51-2608">ACS</span><span class="sxs-lookup"><span data-stu-id="69d51-2608">ACS</span></span>

* <span data-ttu-id="69d51-2609">Mise à jour des options de la commande `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="69d51-2609">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="69d51-2610">Ajout de la prise en charge de `--update`</span><span class="sxs-lookup"><span data-stu-id="69d51-2610">Added `--update` support</span></span>
* <span data-ttu-id="69d51-2611">Modification de `aks get-credentials --admin` pour ne pas remplacer le contexte utilisateur dans `$HOME/.kube/config`</span><span class="sxs-lookup"><span data-stu-id="69d51-2611">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="69d51-2612">Exposition de la propriété en lecture seule `nodeResourceGroup` sur les clusters managés</span><span class="sxs-lookup"><span data-stu-id="69d51-2612">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="69d51-2613">Correction de l’erreur de commande `acs browse`</span><span class="sxs-lookup"><span data-stu-id="69d51-2613">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="69d51-2614">`--connector-name` rendu facultatif pour `aks install-connector`, `aks upgrade-connector` et `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="69d51-2614">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="69d51-2615">Ajout de nouvelles régions Azure Container Instance pour `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="69d51-2615">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="69d51-2616">Ajout de l’emplacement normalisé dans le nom de mise en production Helm et le nom du nœud pour `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="69d51-2616">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="69d51-2617">AppService</span><span class="sxs-lookup"><span data-stu-id="69d51-2617">AppService</span></span>

* <span data-ttu-id="69d51-2618">Ajout de la prise en charge des versions urllib plus récentes</span><span class="sxs-lookup"><span data-stu-id="69d51-2618">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="69d51-2619">Ajout de la prise en charge pour `functionapp create` pour utiliser un plan App Service à partir de groupes de ressources externes</span><span class="sxs-lookup"><span data-stu-id="69d51-2619">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="69d51-2620">Batch</span><span class="sxs-lookup"><span data-stu-id="69d51-2620">Batch</span></span>

* <span data-ttu-id="69d51-2621">Suppression de la dépendance `azure-batch-extensions`</span><span class="sxs-lookup"><span data-stu-id="69d51-2621">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="69d51-2622">Batch AI</span><span class="sxs-lookup"><span data-stu-id="69d51-2622">Batch AI</span></span>

* <span data-ttu-id="69d51-2623">Ajout de la prise en charge des espaces de travail.</span><span class="sxs-lookup"><span data-stu-id="69d51-2623">Added support for workspaces.</span></span> <span data-ttu-id="69d51-2624">Les espaces de travail permettent de regrouper les clusters, serveurs de fichiers et expériences, supprimant la limitation du nombre de ressources qui peuvent être créées</span><span class="sxs-lookup"><span data-stu-id="69d51-2624">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="69d51-2625">Ajout de la prise en charge des expériences.</span><span class="sxs-lookup"><span data-stu-id="69d51-2625">Added support for experiments.</span></span> <span data-ttu-id="69d51-2626">Les expériences permettent de regrouper les tâches dans des collections, supprimant la limitation du nombre de tâches créées</span><span class="sxs-lookup"><span data-stu-id="69d51-2626">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="69d51-2627">Ajout de la prise en charge pour configurer `/dev/shm` pour les travaux en cours d’exécution dans un conteneur docker</span><span class="sxs-lookup"><span data-stu-id="69d51-2627">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="69d51-2628">Ajout des commandes `batchai cluster node exec` et `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="69d51-2628">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="69d51-2629">Ces commandes permettent d’exécuter des commandes directement sur les nœuds et fournissent la fonctionnalité de réacheminement de port.</span><span class="sxs-lookup"><span data-stu-id="69d51-2629">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="69d51-2630">Ajout de la prise en charge des commandes `--ids` et `batchai`</span><span class="sxs-lookup"><span data-stu-id="69d51-2630">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="69d51-2631">[CHANGEMENT CASSANT] Tous les clusters et serveurs de fichiers doivent être créés dans des espaces de travail</span><span class="sxs-lookup"><span data-stu-id="69d51-2631">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="69d51-2632">[CHANGEMENT CASSANT] Les travaux doivent être créés dans des expériences</span><span class="sxs-lookup"><span data-stu-id="69d51-2632">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="69d51-2633">[CHANGEMENT CASSANT] Suppression de `--nfs-resource-group` des commandes `cluster create` et `job create`.</span><span class="sxs-lookup"><span data-stu-id="69d51-2633">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="69d51-2634">Pour monter un NFS appartenant à un autre espace de travail/groupe de ressources, indiquez l’ID ARM du serveur de fichiers via l’option `--nfs`</span><span class="sxs-lookup"><span data-stu-id="69d51-2634">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="69d51-2635">[CHANGEMENT CASSANT] Suppression de `--cluster-resource-group` de la commande `job create`.</span><span class="sxs-lookup"><span data-stu-id="69d51-2635">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="69d51-2636">Pour soumettre un travail sur un cluster appartenant à un autre espace de travail/groupe de ressources, indiquez l’ID ARM du cluster via l’option `--cluster`</span><span class="sxs-lookup"><span data-stu-id="69d51-2636">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="69d51-2637">[CHANGEMENT CASSANT] Suppression de l’attribut `location` des travaux, clusters et serveurs de fichiers.</span><span class="sxs-lookup"><span data-stu-id="69d51-2637">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="69d51-2638">L’emplacement est maintenant un attribut d’espace de travail.</span><span class="sxs-lookup"><span data-stu-id="69d51-2638">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="69d51-2639">[CHANGEMENT CASSANT] Suppression de `--location` des commandes `job create`, `cluster create` et `file-server create`</span><span class="sxs-lookup"><span data-stu-id="69d51-2639">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="69d51-2640">[CHANGEMENT CASSANT] Modification des noms des options courtes pour rendre l’interface plus cohérente :</span><span class="sxs-lookup"><span data-stu-id="69d51-2640">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="69d51-2641">[`--config`, `-c`] renommé en [`--config-file`, `-f`]</span><span class="sxs-lookup"><span data-stu-id="69d51-2641">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="69d51-2642">[`--cluster`, `-r`] renommé en [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="69d51-2642">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="69d51-2643">[`--cluster`, `-n`] renommé en [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="69d51-2643">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="69d51-2644">[`--job`, `-n`] renommé en [`--job`, `-j`]</span><span class="sxs-lookup"><span data-stu-id="69d51-2644">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="69d51-2645">Cartes</span><span class="sxs-lookup"><span data-stu-id="69d51-2645">Maps</span></span>

* <span data-ttu-id="69d51-2646">[CHANGEMENT CASSANT] Modification de `maps account create` pour accepter les Conditions d’utilisation, soit par l’invite interactive ou par l’indicateur `--accept-tos`</span><span class="sxs-lookup"><span data-stu-id="69d51-2646">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="69d51-2647">Réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-2647">Network</span></span>

* <span data-ttu-id="69d51-2648">Ajout de la prise en charge de `https` à `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="69d51-2648">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="69d51-2649">Correction d’un problème où `--endpoint-status` était sensible à la casse.</span><span class="sxs-lookup"><span data-stu-id="69d51-2649">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="69d51-2650">#6502</span><span class="sxs-lookup"><span data-stu-id="69d51-2650">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="69d51-2651">Réservations</span><span class="sxs-lookup"><span data-stu-id="69d51-2651">Reservations</span></span>

* <span data-ttu-id="69d51-2652">[CHANGEMENT CASSANT] Ajout du paramètre obligatoire `ReservedResourceType` à `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="69d51-2652">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="69d51-2653">Ajout du paramètre `Location` à `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="69d51-2653">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="69d51-2654">[CHANGEMENT CASSANT] Suppression de `kind` de `ReservationProperties`</span><span class="sxs-lookup"><span data-stu-id="69d51-2654">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="69d51-2655">[CHANGEMENT CASSANT]`capabilities` renommé en `sku_properties` dans `Catalog`</span><span class="sxs-lookup"><span data-stu-id="69d51-2655">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="69d51-2656">[CHANGEMENT CASSANT] Suppression des propriétés `size` et `tier` de `Catalog`</span><span class="sxs-lookup"><span data-stu-id="69d51-2656">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="69d51-2657">Ajout du paramètre `InstanceFlexibility` à `reservations reservation update`</span><span class="sxs-lookup"><span data-stu-id="69d51-2657">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="69d51-2658">Role</span><span class="sxs-lookup"><span data-stu-id="69d51-2658">Role</span></span>

* <span data-ttu-id="69d51-2659">Amélioration de la gestion des erreurs</span><span class="sxs-lookup"><span data-stu-id="69d51-2659">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="69d51-2660">SQL</span><span class="sxs-lookup"><span data-stu-id="69d51-2660">SQL</span></span>

* <span data-ttu-id="69d51-2661">Correction de l’erreur déroutante lors de l’exécution de `az sql db list-editions` pour un emplacement qui n’est pas disponible pour votre abonnement</span><span class="sxs-lookup"><span data-stu-id="69d51-2661">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="69d51-2662">Stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-2662">Storage</span></span>

* <span data-ttu-id="69d51-2663">Modification de la sortie de table pour que `storage blob download` soit plus lisible</span><span class="sxs-lookup"><span data-stu-id="69d51-2663">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="69d51-2664">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="69d51-2664">VM</span></span>

* <span data-ttu-id="69d51-2665">Amélioration de la vérification de la taille de la machine virtuelle pour la prise en charge de la mise en réseau accélérée dans `vm create`</span><span class="sxs-lookup"><span data-stu-id="69d51-2665">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="69d51-2666">Ajout d’un avertissement pour `vmss create` indiquant que la taille de la machine virtuelle par défaut va passer de `Standard_D1_v2` à `Standard_DS1_v2`</span><span class="sxs-lookup"><span data-stu-id="69d51-2666">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="69d51-2667">Ajout de `--force-update` à `[vm|vmss] extension set` pour mettre à jour l’extension, même lorsque la configuration n’a pas changé</span><span class="sxs-lookup"><span data-stu-id="69d51-2667">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="69d51-2668">13 juin 2018</span><span class="sxs-lookup"><span data-stu-id="69d51-2668">June 13, 2018</span></span>

<span data-ttu-id="69d51-2669">Version 2.0.37</span><span class="sxs-lookup"><span data-stu-id="69d51-2669">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="69d51-2670">Core</span><span class="sxs-lookup"><span data-stu-id="69d51-2670">Core</span></span>

* <span data-ttu-id="69d51-2671">Amélioration de la télémétrie interactive</span><span class="sxs-lookup"><span data-stu-id="69d51-2671">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="69d51-2672">13 juin 2018</span><span class="sxs-lookup"><span data-stu-id="69d51-2672">June 13, 2018</span></span>

<span data-ttu-id="69d51-2673">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="69d51-2673">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="69d51-2674">AKS</span><span class="sxs-lookup"><span data-stu-id="69d51-2674">AKS</span></span>

* <span data-ttu-id="69d51-2675">Ajout d’options réseau avancées à `aks create`</span><span class="sxs-lookup"><span data-stu-id="69d51-2675">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="69d51-2676">Ajout d’arguments à `aks create` pour permettre la surveillance et le routage HTTP</span><span class="sxs-lookup"><span data-stu-id="69d51-2676">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="69d51-2677">Ajout de l’argument `--no-ssh-key` à `aks create`</span><span class="sxs-lookup"><span data-stu-id="69d51-2677">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="69d51-2678">Ajout de l’argument `--enable-rbac` à `aks create`</span><span class="sxs-lookup"><span data-stu-id="69d51-2678">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="69d51-2679">[PRÉVERSION] Ajout de la prise en charge pour l’authentification basée sur Azure Active Directory à `aks create`</span><span class="sxs-lookup"><span data-stu-id="69d51-2679">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="69d51-2680">AppService</span><span class="sxs-lookup"><span data-stu-id="69d51-2680">AppService</span></span>

* <span data-ttu-id="69d51-2681">Résolution d’un problème lié à des versions urllib incompatibles</span><span class="sxs-lookup"><span data-stu-id="69d51-2681">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="69d51-2682">5 juin 2018</span><span class="sxs-lookup"><span data-stu-id="69d51-2682">June 5, 2018</span></span>

<span data-ttu-id="69d51-2683">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="69d51-2683">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="69d51-2684">Interactive</span><span class="sxs-lookup"><span data-stu-id="69d51-2684">Interactive</span></span>

* <span data-ttu-id="69d51-2685">Ajout de limites aux dépendances du mode interactif</span><span class="sxs-lookup"><span data-stu-id="69d51-2685">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="69d51-2686">5 juin 2018</span><span class="sxs-lookup"><span data-stu-id="69d51-2686">June 5, 2018</span></span>

<span data-ttu-id="69d51-2687">Version 2.0.34</span><span class="sxs-lookup"><span data-stu-id="69d51-2687">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="69d51-2688">Core</span><span class="sxs-lookup"><span data-stu-id="69d51-2688">Core</span></span>

* <span data-ttu-id="69d51-2689">Prise en charge supplémentaire pour les références de ressources inter-client</span><span class="sxs-lookup"><span data-stu-id="69d51-2689">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="69d51-2690">Amélioration de la fiabilité de téléchargement des données de télémétrie</span><span class="sxs-lookup"><span data-stu-id="69d51-2690">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="69d51-2691">ACR</span><span class="sxs-lookup"><span data-stu-id="69d51-2691">ACR</span></span>

* <span data-ttu-id="69d51-2692">Prise en charge supplémentaire pour VSTS en tant qu’emplacement source distant</span><span class="sxs-lookup"><span data-stu-id="69d51-2692">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="69d51-2693">Ajout de la commande `acr import`</span><span class="sxs-lookup"><span data-stu-id="69d51-2693">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="69d51-2694">AKS</span><span class="sxs-lookup"><span data-stu-id="69d51-2694">AKS</span></span>

* <span data-ttu-id="69d51-2695">`aks get-credentials` a été modifié pour créer le fichier de configuration kube avec des autorisations de système de fichiers plus sécurisées</span><span class="sxs-lookup"><span data-stu-id="69d51-2695">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="69d51-2696">Batch</span><span class="sxs-lookup"><span data-stu-id="69d51-2696">Batch</span></span>

* <span data-ttu-id="69d51-2697">Résolution du bogue concernant la mise en forme dans la table de liste de pool [[problème #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="69d51-2697">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="69d51-2698">IOT</span><span class="sxs-lookup"><span data-stu-id="69d51-2698">IOT</span></span>

* <span data-ttu-id="69d51-2699">Prise en charge ajoutée pour la création de IoT Hubs de niveau de base</span><span class="sxs-lookup"><span data-stu-id="69d51-2699">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="69d51-2700">Réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-2700">Network</span></span>

* <span data-ttu-id="69d51-2701">`network vnet peering` amélioré</span><span class="sxs-lookup"><span data-stu-id="69d51-2701">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="69d51-2702">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="69d51-2702">Policy Insights</span></span>

* <span data-ttu-id="69d51-2703">Version initiale</span><span class="sxs-lookup"><span data-stu-id="69d51-2703">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="69d51-2704">ARM</span><span class="sxs-lookup"><span data-stu-id="69d51-2704">ARM</span></span>

* <span data-ttu-id="69d51-2705">Ajout des commandes `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="69d51-2705">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="69d51-2706">SQL</span><span class="sxs-lookup"><span data-stu-id="69d51-2706">SQL</span></span>

* <span data-ttu-id="69d51-2707">Ajout de nouvelles commandes d’instance gérée :</span><span class="sxs-lookup"><span data-stu-id="69d51-2707">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="69d51-2708">Ajout de nouvelles commandes de base de données gérée :</span><span class="sxs-lookup"><span data-stu-id="69d51-2708">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="69d51-2709">Stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-2709">Storage</span></span>

* <span data-ttu-id="69d51-2710">Ajout de types MimeTypes supplémentaires pour les formats json et javascript pour être déduit à partir des extensions de fichier</span><span class="sxs-lookup"><span data-stu-id="69d51-2710">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="69d51-2711">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="69d51-2711">VM</span></span>

* <span data-ttu-id="69d51-2712">`vm list-skus` a été modifié pour utiliser des colonnes corrigées et ajouter l’avertissement que `Tier` et `Size` seront supprimés</span><span class="sxs-lookup"><span data-stu-id="69d51-2712">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="69d51-2713">Ajout de l’option `--accelerated-networking` à `vm create`</span><span class="sxs-lookup"><span data-stu-id="69d51-2713">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="69d51-2714">Ajout de `--tags` à `identity create`</span><span class="sxs-lookup"><span data-stu-id="69d51-2714">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="69d51-2715">22 mai 2018</span><span class="sxs-lookup"><span data-stu-id="69d51-2715">May 22, 2018</span></span>

<span data-ttu-id="69d51-2716">Version 2.0.33</span><span class="sxs-lookup"><span data-stu-id="69d51-2716">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="69d51-2717">Core</span><span class="sxs-lookup"><span data-stu-id="69d51-2717">Core</span></span>

* <span data-ttu-id="69d51-2718">Ajout de la prise en charge pour le développement de `@` dans les noms de fichiers</span><span class="sxs-lookup"><span data-stu-id="69d51-2718">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="69d51-2719">ACS</span><span class="sxs-lookup"><span data-stu-id="69d51-2719">ACS</span></span>

* <span data-ttu-id="69d51-2720">Ajout de nouvelles commandes Dev Spaces `aks use-dev-spaces` et `aks remove-dev-spaces`</span><span class="sxs-lookup"><span data-stu-id="69d51-2720">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="69d51-2721">Faute de frappe corrigée dans un message d’aide</span><span class="sxs-lookup"><span data-stu-id="69d51-2721">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="69d51-2722">AppService</span><span class="sxs-lookup"><span data-stu-id="69d51-2722">AppService</span></span>

* <span data-ttu-id="69d51-2723">Amélioration des commandes de mise à jour générique</span><span class="sxs-lookup"><span data-stu-id="69d51-2723">Improved generic update commands</span></span>
* <span data-ttu-id="69d51-2724">Ajout de la prise en charge asynchrone pour `webapp deployment source config-zip`</span><span class="sxs-lookup"><span data-stu-id="69d51-2724">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="69d51-2725">Conteneur</span><span class="sxs-lookup"><span data-stu-id="69d51-2725">Container</span></span>

* <span data-ttu-id="69d51-2726">Prise en charge ajoutée pour l’exportation d’un groupe de conteneurs au format yaml</span><span class="sxs-lookup"><span data-stu-id="69d51-2726">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="69d51-2727">Prise en charge ajoutée pour l’utilisation d’un fichier yaml afin de créer/mettre à jour un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="69d51-2727">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="69d51-2728">Extension</span><span class="sxs-lookup"><span data-stu-id="69d51-2728">Extension</span></span>

* <span data-ttu-id="69d51-2729">Amélioration de la suppression des extensions</span><span class="sxs-lookup"><span data-stu-id="69d51-2729">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="69d51-2730">Interactive</span><span class="sxs-lookup"><span data-stu-id="69d51-2730">Interactive</span></span>

* <span data-ttu-id="69d51-2731">La journalisation a été modifiée pour désactiver l’analyseur pour les saisies semi-automatiques</span><span class="sxs-lookup"><span data-stu-id="69d51-2731">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="69d51-2732">Gestion améliorée des caches d’aide incorrects</span><span class="sxs-lookup"><span data-stu-id="69d51-2732">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="69d51-2733">KeyVault</span><span class="sxs-lookup"><span data-stu-id="69d51-2733">KeyVault</span></span>

* <span data-ttu-id="69d51-2734">Commandes keyvault corrigées afin de fonctionner dans Cloud Shell ou dans des machines virtuelles avec l’identité</span><span class="sxs-lookup"><span data-stu-id="69d51-2734">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="69d51-2735">Réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-2735">Network</span></span>

* <span data-ttu-id="69d51-2736">Résolution d’un problème où `network watcher show-topology` ne fonctionnait pas avec le nom de réseau virtuel et/ou de sous-réseau [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="69d51-2736">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="69d51-2737">Correction d’un problème où certaines commandes `network watcher` revendiquaient que Network Watcher n’était pas activé pour certaines régions alors qu’il l’était [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="69d51-2737">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="69d51-2738">SQL</span><span class="sxs-lookup"><span data-stu-id="69d51-2738">SQL</span></span>

* <span data-ttu-id="69d51-2739">[CHANGEMENT CASSANT] Objets de réponse retournés modifiés à partir des commandes `db` et `dw`</span><span class="sxs-lookup"><span data-stu-id="69d51-2739">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="69d51-2740">Propriété `serviceLevelObjective` renommée en `currentServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="69d51-2740">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="69d51-2741">Suppression des propriétés `currentServiceObjectiveId` et `requestedServiceObjectiveId`</span><span class="sxs-lookup"><span data-stu-id="69d51-2741">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="69d51-2742">Propriété `maxSizeBytes` modifiée en valeur entière au lieu d’une chaîne</span><span class="sxs-lookup"><span data-stu-id="69d51-2742">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="69d51-2743">[CHANGEMENT CASSANT] Les propriétés `db` et `dw` suivantes ont été modifiées pour être en lecture seule :</span><span class="sxs-lookup"><span data-stu-id="69d51-2743">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="69d51-2744">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="69d51-2744">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="69d51-2745">Pour mettre à jour, utilisez le paramètre `--service-objective` ou définissez la propriété `sku.name`</span><span class="sxs-lookup"><span data-stu-id="69d51-2745">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="69d51-2746">`edition`.</span><span class="sxs-lookup"><span data-stu-id="69d51-2746">`edition`.</span></span> <span data-ttu-id="69d51-2747">Pour mettre à jour, utilisez le paramètre `--edition` ou définissez la propriété `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="69d51-2747">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="69d51-2748">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="69d51-2748">`elasticPoolName`.</span></span> <span data-ttu-id="69d51-2749">Pour mettre à jour, utilisez le paramètre `--elastic-pool` ou définissez la propriété `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="69d51-2749">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="69d51-2750">[CHANGEMENT CASSANT] Les propriétés `elastic-pool` suivantes ont été modifiées pour être en lecture seule :</span><span class="sxs-lookup"><span data-stu-id="69d51-2750">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="69d51-2751">`edition`.</span><span class="sxs-lookup"><span data-stu-id="69d51-2751">`edition`.</span></span> <span data-ttu-id="69d51-2752">Pour mettre à jour, utilisez le paramètre `--edition`</span><span class="sxs-lookup"><span data-stu-id="69d51-2752">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="69d51-2753">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="69d51-2753">`dtu`.</span></span> <span data-ttu-id="69d51-2754">Pour mettre à jour, utilisez le paramètre `--capacity`</span><span class="sxs-lookup"><span data-stu-id="69d51-2754">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="69d51-2755">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="69d51-2755">`databaseDtuMin`.</span></span> <span data-ttu-id="69d51-2756">Pour mettre à jour, utilisez le paramètre `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="69d51-2756">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="69d51-2757">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="69d51-2757">`databaseDtuMax`.</span></span> <span data-ttu-id="69d51-2758">Pour mettre à jour, utilisez le paramètre `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="69d51-2758">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="69d51-2759">Ajout des paramètres `--family` et `--capacity` aux commandes `db`, `dw` et `elastic-pool`</span><span class="sxs-lookup"><span data-stu-id="69d51-2759">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="69d51-2760">Ajout de formateurs de table aux commandes `db`, `dw` et `elastic-pool`</span><span class="sxs-lookup"><span data-stu-id="69d51-2760">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="69d51-2761">Stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-2761">Storage</span></span>

* <span data-ttu-id="69d51-2762">Ajout d’un compléteur pour l’argument `--account-name`</span><span class="sxs-lookup"><span data-stu-id="69d51-2762">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="69d51-2763">Correction d’un problème avec `storage entity query`</span><span class="sxs-lookup"><span data-stu-id="69d51-2763">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="69d51-2764">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="69d51-2764">VM</span></span>

* <span data-ttu-id="69d51-2765">[CHANGEMENT CASSANT] Suppression de `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="69d51-2765">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="69d51-2766">La même prise en charge est accessible via `vm update` ou `vm disk attach`</span><span class="sxs-lookup"><span data-stu-id="69d51-2766">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="69d51-2767">Correction de l’image de l’extension efficace dans `[vm|vmss] extension`</span><span class="sxs-lookup"><span data-stu-id="69d51-2767">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="69d51-2768">Ajout de`--boot-diagnostics-storage` à `vm create` pour capturer le journal de démarrage</span><span class="sxs-lookup"><span data-stu-id="69d51-2768">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="69d51-2769">Ajout de `--license-type` à `[vm|vmss] update`</span><span class="sxs-lookup"><span data-stu-id="69d51-2769">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="69d51-2770">7 mai 2018</span><span class="sxs-lookup"><span data-stu-id="69d51-2770">May 7, 2018</span></span>

<span data-ttu-id="69d51-2771">Version 2.0.32</span><span class="sxs-lookup"><span data-stu-id="69d51-2771">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="69d51-2772">Core</span><span class="sxs-lookup"><span data-stu-id="69d51-2772">Core</span></span>

* <span data-ttu-id="69d51-2773">Correction d’une exception non gérée lors de la récupération des clés secrètes à partir d’un compte de principal de service avec certificat</span><span class="sxs-lookup"><span data-stu-id="69d51-2773">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="69d51-2774">Nouvelle prise en charge limitée pour les arguments positionnels</span><span class="sxs-lookup"><span data-stu-id="69d51-2774">Added limited support for positional arguments</span></span>
* <span data-ttu-id="69d51-2775">Correction d’un problème où `--query` ne pouvait pas être utilisé avec `--ids`.</span><span class="sxs-lookup"><span data-stu-id="69d51-2775">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="69d51-2776">#5591</span><span class="sxs-lookup"><span data-stu-id="69d51-2776">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="69d51-2777">Amélioration des scénarios de redirection à partir des commandes en utilisant `--ids`.</span><span class="sxs-lookup"><span data-stu-id="69d51-2777">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="69d51-2778">Prend en charge `-o tsv` avec une requête spécifiée ou `-o json` sans spécification de requête</span><span class="sxs-lookup"><span data-stu-id="69d51-2778">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="69d51-2779">Ajout de suggestions de commande en cas d’erreur engendrées par des fautes de frappe des utilisateurs dans les commandes</span><span class="sxs-lookup"><span data-stu-id="69d51-2779">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="69d51-2780">Amélioration de l’erreur lorsque les utilisateurs entrent `az ''`</span><span class="sxs-lookup"><span data-stu-id="69d51-2780">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="69d51-2781">Ajout de la prise en charge des types de ressources personnalisés pour les modules et les extensions de commande</span><span class="sxs-lookup"><span data-stu-id="69d51-2781">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="69d51-2782">ACR</span><span class="sxs-lookup"><span data-stu-id="69d51-2782">ACR</span></span>

* <span data-ttu-id="69d51-2783">Ajout de commandes de build de l’ACR</span><span class="sxs-lookup"><span data-stu-id="69d51-2783">Added ACR Build commands</span></span>
* <span data-ttu-id="69d51-2784">Améliorations des messages d’erreur dus aux ressources introuvables</span><span class="sxs-lookup"><span data-stu-id="69d51-2784">Improved resource not found error messages</span></span>
* <span data-ttu-id="69d51-2785">Amélioration des performances de création de ressources et de la gestion des erreurs</span><span class="sxs-lookup"><span data-stu-id="69d51-2785">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="69d51-2786">Amélioration de la connexion ACR dans des consoles non standards et des WSL</span><span class="sxs-lookup"><span data-stu-id="69d51-2786">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="69d51-2787">Amélioration des messages d’erreur dus aux commandes de dépôt</span><span class="sxs-lookup"><span data-stu-id="69d51-2787">Improved repository commands error messages</span></span>
* <span data-ttu-id="69d51-2788">Mise à jour des colonnes de la table et du classement</span><span class="sxs-lookup"><span data-stu-id="69d51-2788">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="69d51-2789">ACS</span><span class="sxs-lookup"><span data-stu-id="69d51-2789">ACS</span></span>

* <span data-ttu-id="69d51-2790">Ajout d’un avertissement indiquant que `az aks` est un service en préversion</span><span class="sxs-lookup"><span data-stu-id="69d51-2790">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="69d51-2791">Résolution du problème d’autorisation dans `aks install-connector` lorsque `--aci-resource-group` n’est pas spécifié</span><span class="sxs-lookup"><span data-stu-id="69d51-2791">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="69d51-2792">AMS</span><span class="sxs-lookup"><span data-stu-id="69d51-2792">AMS</span></span>

* <span data-ttu-id="69d51-2793">Version initiale - Gérer des ressources Azure Media Services</span><span class="sxs-lookup"><span data-stu-id="69d51-2793">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="69d51-2794">AppService</span><span class="sxs-lookup"><span data-stu-id="69d51-2794">Appservice</span></span>

* <span data-ttu-id="69d51-2795">Correction d’un bogue dans `webapp delete` lorsque `--slot` est fourni</span><span class="sxs-lookup"><span data-stu-id="69d51-2795">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="69d51-2796">`--runtime-version` retiré de `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="69d51-2796">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="69d51-2797">Ajout de la prise en charge de min\_tls\_version & https2.0</span><span class="sxs-lookup"><span data-stu-id="69d51-2797">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="69d51-2798">Ajout de la prise en charge pour les multiconteneurs</span><span class="sxs-lookup"><span data-stu-id="69d51-2798">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="69d51-2799">Batch AI</span><span class="sxs-lookup"><span data-stu-id="69d51-2799">Batch AI</span></span>

* <span data-ttu-id="69d51-2800">`batchai create cluster` modifié pour respecter la priorité de machine virtuelle configurée dans le fichier de configuration du cluster</span><span class="sxs-lookup"><span data-stu-id="69d51-2800">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="69d51-2801">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="69d51-2801">Cognitive Services</span></span>

* <span data-ttu-id="69d51-2802">Faute de frappe corrigée dans l’exemple de `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="69d51-2802">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="69d51-2803">Consommation</span><span class="sxs-lookup"><span data-stu-id="69d51-2803">Consumption</span></span>

* <span data-ttu-id="69d51-2804">Ajout de nouvelles commandes pour l’API Budget</span><span class="sxs-lookup"><span data-stu-id="69d51-2804">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="69d51-2805">Conteneur</span><span class="sxs-lookup"><span data-stu-id="69d51-2805">Container</span></span>

* <span data-ttu-id="69d51-2806">Suppression de l’exigence pour `--registry-server` pour `container create` lorsqu’un serveur de registre est inclus dans le nom de l’image</span><span class="sxs-lookup"><span data-stu-id="69d51-2806">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="69d51-2807">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="69d51-2807">Cosmos DB</span></span>

* <span data-ttu-id="69d51-2808">Présentation de la prise en charge d’un réseau virtuel pour Azure CLI - Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="69d51-2808">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="69d51-2809">DMS</span><span class="sxs-lookup"><span data-stu-id="69d51-2809">DMS</span></span>

* <span data-ttu-id="69d51-2810">Version initiale - Ajoute la prise en charge de l’instruction SQL pour le scénario de migration de SQL Azure</span><span class="sxs-lookup"><span data-stu-id="69d51-2810">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="69d51-2811">Extension</span><span class="sxs-lookup"><span data-stu-id="69d51-2811">Extension</span></span>

* <span data-ttu-id="69d51-2812">Correction d’un bogue où les métadonnées d’extension cessaient d’être affichées</span><span class="sxs-lookup"><span data-stu-id="69d51-2812">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="69d51-2813">Interactive</span><span class="sxs-lookup"><span data-stu-id="69d51-2813">Interactive</span></span>

* <span data-ttu-id="69d51-2814">Autorise le fonctionnement de compléments interactifs avec des arguments positionnel</span><span class="sxs-lookup"><span data-stu-id="69d51-2814">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="69d51-2815">Sortie plus conviviale lorsque les utilisateurs entrent \'</span><span class="sxs-lookup"><span data-stu-id="69d51-2815">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="69d51-2816">Achèvements corrigés pour les paramètres sans aide</span><span class="sxs-lookup"><span data-stu-id="69d51-2816">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="69d51-2817">Descriptions corrigées pour les groupes de commandes</span><span class="sxs-lookup"><span data-stu-id="69d51-2817">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="69d51-2818">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="69d51-2818">Lab</span></span>

* <span data-ttu-id="69d51-2819">Régressions corrigées de conversion Knack</span><span class="sxs-lookup"><span data-stu-id="69d51-2819">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="69d51-2820">Réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-2820">Network</span></span>

* <span data-ttu-id="69d51-2821">[CHANGEMENT CASSANT] Suppression du paramètre `--ids` pour :</span><span class="sxs-lookup"><span data-stu-id="69d51-2821">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="69d51-2822">Profil</span><span class="sxs-lookup"><span data-stu-id="69d51-2822">Profile</span></span>

* <span data-ttu-id="69d51-2823">Correction de la détection de source `disk create`</span><span class="sxs-lookup"><span data-stu-id="69d51-2823">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="69d51-2824">[CHANGEMENT CASSANT] Suppression de `--msi-port` et `--identity-port` car ils ne sont plus utilisés</span><span class="sxs-lookup"><span data-stu-id="69d51-2824">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="69d51-2825">Correction d’une faute de frappe dans le bref résumé de `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="69d51-2825">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="69d51-2826">Redis</span><span class="sxs-lookup"><span data-stu-id="69d51-2826">Redis</span></span>

* <span data-ttu-id="69d51-2827">`redis patch-schedule patch-schedule show` déconseillé en faveur de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="69d51-2827">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="69d51-2828">`redis list-all` déconseillé.</span><span class="sxs-lookup"><span data-stu-id="69d51-2828">Deprecated `redis list-all`.</span></span> <span data-ttu-id="69d51-2829">Cette fonctionnalité a été pliée dans `redis list`</span><span class="sxs-lookup"><span data-stu-id="69d51-2829">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="69d51-2830">`redis import-method` déconseillé en faveur de `redis import`</span><span class="sxs-lookup"><span data-stu-id="69d51-2830">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="69d51-2831">Ajout de la prise en charge de `--ids` pour diverses commandes</span><span class="sxs-lookup"><span data-stu-id="69d51-2831">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="69d51-2832">Role</span><span class="sxs-lookup"><span data-stu-id="69d51-2832">Role</span></span>

* <span data-ttu-id="69d51-2833">[CHANGEMENT CASSANT] Suppression de `ad sp reset-credentials` déconseillé</span><span class="sxs-lookup"><span data-stu-id="69d51-2833">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="69d51-2834">Stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-2834">Storage</span></span>

* <span data-ttu-id="69d51-2835">Autorise l’application du jeton SAS de destination pour une copie d’objets blob si le SAS source et la clé de compte ne sont pas spécifiés</span><span class="sxs-lookup"><span data-stu-id="69d51-2835">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="69d51-2836">Exposé--délai d’expiration de socket pour les chargements et téléchargements d’objets blob</span><span class="sxs-lookup"><span data-stu-id="69d51-2836">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="69d51-2837">Traite les noms d’objets blob commençant par des séparateurs de chemin d’accès comme des chemins d’accès relatifs</span><span class="sxs-lookup"><span data-stu-id="69d51-2837">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="69d51-2838">Autorise `storage blob copy --source-sas` avec le caractère de démarrage de requête, « ? »</span><span class="sxs-lookup"><span data-stu-id="69d51-2838">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="69d51-2839">`storage entity query --marker` corrigé pour accepter une liste de clé =valeurs</span><span class="sxs-lookup"><span data-stu-id="69d51-2839">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="69d51-2840">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="69d51-2840">VM</span></span>

* <span data-ttu-id="69d51-2841">Correction d’une logique de détection invalide sur l’URI de l’objet blob non gérée</span><span class="sxs-lookup"><span data-stu-id="69d51-2841">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="69d51-2842">Ajout de la prise en charge du chiffrement de disque sans principaux de service fournis par l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="69d51-2842">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="69d51-2843">[CHANGEMENT CASSANT] Ne pas utiliser « ManagedIdentityExtension » de machine virtuelle pour la prise en charge de MSI</span><span class="sxs-lookup"><span data-stu-id="69d51-2843">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="69d51-2844">Ajout de la prise en charge pour la stratégie d’éviction vers `vmss`</span><span class="sxs-lookup"><span data-stu-id="69d51-2844">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="69d51-2845">[CHANGEMENT CASSANT] Suppression de `--ids` de :</span><span class="sxs-lookup"><span data-stu-id="69d51-2845">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="69d51-2846">Ajout de la prise en charge des accélérateurs d’écriture</span><span class="sxs-lookup"><span data-stu-id="69d51-2846">Added write accelerator support</span></span>
* <span data-ttu-id="69d51-2847">Ajout de `vmss perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="69d51-2847">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="69d51-2848">Correction de `vm diagnostics set` pour détecter la fiabilité du type de système d’exploitation de la machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="69d51-2848">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="69d51-2849">Modification de `vm resize` pour vérifier si la taille demandée est différente de celle actuellement définie et pour mettre à jour uniquement en cas de modifications</span><span class="sxs-lookup"><span data-stu-id="69d51-2849">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="69d51-2850">10 avril 2018</span><span class="sxs-lookup"><span data-stu-id="69d51-2850">April 10, 2018</span></span>

<span data-ttu-id="69d51-2851">Version 2.0.31</span><span class="sxs-lookup"><span data-stu-id="69d51-2851">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="69d51-2852">ACR</span><span class="sxs-lookup"><span data-stu-id="69d51-2852">ACR</span></span>

* <span data-ttu-id="69d51-2853">Gestion améliorée des erreurs de secours wincred</span><span class="sxs-lookup"><span data-stu-id="69d51-2853">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="69d51-2854">ACS</span><span class="sxs-lookup"><span data-stu-id="69d51-2854">ACS</span></span>

* <span data-ttu-id="69d51-2855">Modification de la durée de validité des SPN créés par AKS à 5 ans</span><span class="sxs-lookup"><span data-stu-id="69d51-2855">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="69d51-2856">AppService</span><span class="sxs-lookup"><span data-stu-id="69d51-2856">Appservice</span></span>

* [CHANGEMENT CASSANT]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="69d51-2858">Correction d’une exception non interceptée pour les plans webapp inexistants</span><span class="sxs-lookup"><span data-stu-id="69d51-2858">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="69d51-2859">Batch AI</span><span class="sxs-lookup"><span data-stu-id="69d51-2859">BatchAI</span></span>

* <span data-ttu-id="69d51-2860">Ajout de la prise en charge de l’API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="69d51-2860">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="69d51-2861">Montage au niveau du travail</span><span class="sxs-lookup"><span data-stu-id="69d51-2861">Job level mounting</span></span>
  - <span data-ttu-id="69d51-2862">Variables d’environnement avec les valeurs des secrets</span><span class="sxs-lookup"><span data-stu-id="69d51-2862">Environment variables with secret values</span></span>
  - <span data-ttu-id="69d51-2863">Paramètres des compteurs de performances</span><span class="sxs-lookup"><span data-stu-id="69d51-2863">Performance counters settings</span></span>
  - <span data-ttu-id="69d51-2864">Création de rapports de segments de ligne spécifiques à un travail</span><span class="sxs-lookup"><span data-stu-id="69d51-2864">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="69d51-2865">Prise en charge des sous-dossiers dans les listes de fichiers de l’API</span><span class="sxs-lookup"><span data-stu-id="69d51-2865">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="69d51-2866">Création de rapports d’utilisation et de limites</span><span class="sxs-lookup"><span data-stu-id="69d51-2866">Usage and limits reporting</span></span>
  - <span data-ttu-id="69d51-2867">Autorisation de la spécification du type de mise en cache pour les serveurs NFS</span><span class="sxs-lookup"><span data-stu-id="69d51-2867">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="69d51-2868">Prise en charge des images personnalisées</span><span class="sxs-lookup"><span data-stu-id="69d51-2868">Support for custom images</span></span>
  - <span data-ttu-id="69d51-2869">Ajout de la prise en charge de la boîte à outils pyTorch</span><span class="sxs-lookup"><span data-stu-id="69d51-2869">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="69d51-2870">Ajout de la commande `job wait` qui permet d’attendre la fin du travail et d’obtenir le code de sortie du travail</span><span class="sxs-lookup"><span data-stu-id="69d51-2870">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="69d51-2871">Ajout de la commande `usage show` pour répertorier l’utilisation actuelle des ressources Batch AI et les limites pour les différentes régions</span><span class="sxs-lookup"><span data-stu-id="69d51-2871">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="69d51-2872">Prise en charge des clouds nationaux</span><span class="sxs-lookup"><span data-stu-id="69d51-2872">National clouds are supported</span></span>
* <span data-ttu-id="69d51-2873">Ajout d’arguments de ligne de commande de travail pour monter des systèmes de fichiers au niveau du travail en plus des fichiers de configuration</span><span class="sxs-lookup"><span data-stu-id="69d51-2873">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="69d51-2874">Ajout de plus d’options pour personnaliser les clusters : priorité des machines virtuelles, sous-réseau, nombre de nœuds initial pour les clusters avec mise à l’échelle automatique, spécification d’une image personnalisée</span><span class="sxs-lookup"><span data-stu-id="69d51-2874">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="69d51-2875">Ajout d’une option de ligne de commande pour spécifier le type de mise en cache pour les NFS gérés par Batch AI</span><span class="sxs-lookup"><span data-stu-id="69d51-2875">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="69d51-2876">Simplification de la spécification du montage du système de fichiers dans les fichiers config.</span><span class="sxs-lookup"><span data-stu-id="69d51-2876">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="69d51-2877">Il est désormais possible d’omettre les informations d’identification pour les partages de fichiers Azure et les conteneurs d’objets blob Azure : CLI remplira les informations d’identification manquantes à l’aide de la clé du compte de stockage fournie par le biais des paramètres de ligne de commande ou spécifiée via la variable d’environnement, ou interrogera la clé à partir du stockage Azure (si le compte de stockage appartient à l’abonnement actuel)</span><span class="sxs-lookup"><span data-stu-id="69d51-2877">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="69d51-2878">La commande de flux de fichiers de travail se remplit désormais automatiquement lorsque le travail est terminé (réussite, échec, terminé ou supprimé)</span><span class="sxs-lookup"><span data-stu-id="69d51-2878">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="69d51-2879">Amélioration de la sortie `table` pour les opérations `show`</span><span class="sxs-lookup"><span data-stu-id="69d51-2879">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="69d51-2880">Ajout de l’option `--use-auto-storage` pour la création du cluster.</span><span class="sxs-lookup"><span data-stu-id="69d51-2880">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="69d51-2881">Cette option simplifie la gestion des comptes de stockage et le montage de partages de fichiers Azure et de conteneurs d’objets blob Azure vers des clusters</span><span class="sxs-lookup"><span data-stu-id="69d51-2881">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="69d51-2882">Ajout de l’option `--generate-ssh-keys` à `cluster create` et `file-server create`</span><span class="sxs-lookup"><span data-stu-id="69d51-2882">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="69d51-2883">Ajout de la possibilité de fournir la tâche de configuration de nœud via la ligne de commande</span><span class="sxs-lookup"><span data-stu-id="69d51-2883">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="69d51-2884">[CHANGEMENT CASSANT] Déplacement des commandes `job stream-file` et `job list-files` sous le groupe `job file`</span><span class="sxs-lookup"><span data-stu-id="69d51-2884">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="69d51-2885">[CHANGEMENT CASSANT] Renommage de `--admin-user-name` en `--user-name` dans la commande `file-server create` pour être cohérent avec la commande `cluster create`</span><span class="sxs-lookup"><span data-stu-id="69d51-2885">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="69d51-2886">Facturation</span><span class="sxs-lookup"><span data-stu-id="69d51-2886">Billing</span></span>

* <span data-ttu-id="69d51-2887">Ajout de commandes d’inscription de compte</span><span class="sxs-lookup"><span data-stu-id="69d51-2887">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="69d51-2888">Consommation</span><span class="sxs-lookup"><span data-stu-id="69d51-2888">Consumption</span></span>

* <span data-ttu-id="69d51-2889">Ajout des commandes `marketplace`</span><span class="sxs-lookup"><span data-stu-id="69d51-2889">Added `marketplace` commands</span></span>
* <span data-ttu-id="69d51-2890">[CHANGEMENT CASSANT] Renommage de `reservations summaries` en `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="69d51-2890">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="69d51-2891">[CHANGEMENT CASSANT] Renommage de `reservations details` en `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="69d51-2891">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="69d51-2892">[CHANGEMENT CASSANT] Suppression des options abrégées de `--reservation-order-id` et `--reservation-id` pour les commandes `reservation`</span><span class="sxs-lookup"><span data-stu-id="69d51-2892">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="69d51-2893">[CHANGEMENT CASSANT] Suppression des options abrégées de `--grain` pour les commandes `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="69d51-2893">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="69d51-2894">[CHANGEMENT CASSANT] Suppression des options abrégées de `--include-meter-details` pour les commandes `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="69d51-2894">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="69d51-2895">Conteneur</span><span class="sxs-lookup"><span data-stu-id="69d51-2895">Container</span></span>

* <span data-ttu-id="69d51-2896">Ajout des paramètres de montage de volume de dépôt Git `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` et `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="69d51-2896">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="69d51-2897">Résolution de [#5926](https://github.com/Azure/azure-cli/issues/5926) : `az container exec` échoue lorsque le nom du conteneur -- est spécifié</span><span class="sxs-lookup"><span data-stu-id="69d51-2897">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="69d51-2898">Extension</span><span class="sxs-lookup"><span data-stu-id="69d51-2898">Extension</span></span>

* <span data-ttu-id="69d51-2899">Modification du message de vérification de distribution pour qu’il soit au niveau du débogage</span><span class="sxs-lookup"><span data-stu-id="69d51-2899">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="69d51-2900">Interactive</span><span class="sxs-lookup"><span data-stu-id="69d51-2900">Interactive</span></span>

* <span data-ttu-id="69d51-2901">Modification pour arrêter la saisie semi-automatique sur les commandes non reconnues</span><span class="sxs-lookup"><span data-stu-id="69d51-2901">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="69d51-2902">Ajout d’événements de raccordement avant et après la création du sous-arbre de commande</span><span class="sxs-lookup"><span data-stu-id="69d51-2902">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="69d51-2903">Ajout de la saisie semi-automatique pour les paramètres `--ids`</span><span class="sxs-lookup"><span data-stu-id="69d51-2903">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="69d51-2904">Réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-2904">Network</span></span>

* <span data-ttu-id="69d51-2905">Résolution de [#5936](https://github.com/Azure/azure-cli/issues/5936) : les balises `application-gateway create` n’ont pas pu déterminer l’ensemble</span><span class="sxs-lookup"><span data-stu-id="69d51-2905">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="69d51-2906">Ajout de l’argument `--auth-certs` pour joindre des certificats d’authentification pour `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="69d51-2906">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="69d51-2907">#4910</span><span class="sxs-lookup"><span data-stu-id="69d51-2907">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="69d51-2908">Ajout de commandes `ddos-protection` pour créer des plans de protection DDoS</span><span class="sxs-lookup"><span data-stu-id="69d51-2908">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="69d51-2909">Prise en charge de `--ddos-protection-plan` pour `vnet [create|update]` pour associer un réseau virtuel à un plan de protection DDoS</span><span class="sxs-lookup"><span data-stu-id="69d51-2909">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="69d51-2910">Résolution du problème avec l’ indicateur `--disable-bgp-route-propagation` dans `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69d51-2910">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="69d51-2911">Suppression des arguments factices `--public-ip-address-type` et `--subnet-type` pour `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69d51-2911">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="69d51-2912">Ajout de la prise en charge des enregistrements TXT avec les séquences d’échappement RFC 1035 à `network dns zone [import|export]` et `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="69d51-2912">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="69d51-2913">Profil</span><span class="sxs-lookup"><span data-stu-id="69d51-2913">Profile</span></span>

* <span data-ttu-id="69d51-2914">Ajout de la prise en charge des comptes Azure Classic dans `account list`</span><span class="sxs-lookup"><span data-stu-id="69d51-2914">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="69d51-2915">[CHANGEMENT CASSANT] Suppression des arguments `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="69d51-2915">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="69d51-2916">SGBDR</span><span class="sxs-lookup"><span data-stu-id="69d51-2916">RDBMS</span></span>

* <span data-ttu-id="69d51-2917">Ajout de la commande `georestore`</span><span class="sxs-lookup"><span data-stu-id="69d51-2917">Added `georestore` command</span></span>
* <span data-ttu-id="69d51-2918">Suppression de la restriction de taille de stockage de la commande `create`</span><span class="sxs-lookup"><span data-stu-id="69d51-2918">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="69d51-2919">Ressource</span><span class="sxs-lookup"><span data-stu-id="69d51-2919">Resource</span></span>

* <span data-ttu-id="69d51-2920">Ajout de la prise en charge de `--metadata` pour `policy definition create`</span><span class="sxs-lookup"><span data-stu-id="69d51-2920">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="69d51-2921">Ajout de la prise en charge de `--metadata`, `--set`, `--add` et `--remove` à `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="69d51-2921">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="69d51-2922">SQL</span><span class="sxs-lookup"><span data-stu-id="69d51-2922">SQL</span></span>

* <span data-ttu-id="69d51-2923">Ajout de `sql elastic-pool op list` et `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="69d51-2923">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="69d51-2924">Stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-2924">Storage</span></span>

* <span data-ttu-id="69d51-2925">Amélioration des messages d’erreur pour les chaînes de connexion incorrectes</span><span class="sxs-lookup"><span data-stu-id="69d51-2925">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="69d51-2926">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="69d51-2926">VM</span></span>

* <span data-ttu-id="69d51-2927">Ajout de la prise en charge pour configurer le nombre de domaines d’erreur de plateforme sur `vmss create`</span><span class="sxs-lookup"><span data-stu-id="69d51-2927">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="69d51-2928">Modification de `vmss create` sur la valeur par défaut de l’équilibreur de charge Standard pour les groupes identiques désactivés zonaux, grands ou avec un seul groupe de placement</span><span class="sxs-lookup"><span data-stu-id="69d51-2928">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [CHANGEMENT CASSANT]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="69d51-2930">Ajout de la prise en charge des références SKU d’IP public à `vm create`</span><span class="sxs-lookup"><span data-stu-id="69d51-2930">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="69d51-2931">Ajout des arguments `--keyvault` et `--resource-group` à `vm secret format` pour prendre en charge des scénarios où la commande ne parvient pas à résoudre l’ID de coffre.</span><span class="sxs-lookup"><span data-stu-id="69d51-2931">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="69d51-2932">#5718</span><span class="sxs-lookup"><span data-stu-id="69d51-2932">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="69d51-2933">Amélioration des erreurs pour `[vm|vmss create]` lorsque l’emplacement d’un groupe de ressources ne possède aucune prise en charge de zone</span><span class="sxs-lookup"><span data-stu-id="69d51-2933">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="69d51-2934">27 mars 2018</span><span class="sxs-lookup"><span data-stu-id="69d51-2934">March 27, 2018</span></span>

<span data-ttu-id="69d51-2935">Version 2.0.30</span><span class="sxs-lookup"><span data-stu-id="69d51-2935">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="69d51-2936">Core</span><span class="sxs-lookup"><span data-stu-id="69d51-2936">Core</span></span>

* <span data-ttu-id="69d51-2937">Afficher le message pour les extensions marquées en tant que préversions dans l’aide</span><span class="sxs-lookup"><span data-stu-id="69d51-2937">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="69d51-2938">ACS</span><span class="sxs-lookup"><span data-stu-id="69d51-2938">ACS</span></span>

* <span data-ttu-id="69d51-2939">Corriger l’erreur de vérification de certificat SSL pour `aks install-cli` dans Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="69d51-2939">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="69d51-2940">AppService</span><span class="sxs-lookup"><span data-stu-id="69d51-2940">Appservice</span></span>

* <span data-ttu-id="69d51-2941">Ajout de la prise en charge HTTPS exclusive à `webapp update`</span><span class="sxs-lookup"><span data-stu-id="69d51-2941">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="69d51-2942">Ajout de la prise en charge des emplacements à `az webapp identity [assign|show]` et `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="69d51-2942">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="69d51-2943">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="69d51-2943">Backup</span></span>

* <span data-ttu-id="69d51-2944">Ajout de la commande `az backup protection isenabled-for-vm`</span><span class="sxs-lookup"><span data-stu-id="69d51-2944">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="69d51-2945">Cette commande peut être utilisée pour vérifier si une machine virtuelle est sauvegardée par un coffre dans l’abonnement</span><span class="sxs-lookup"><span data-stu-id="69d51-2945">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="69d51-2946">Activation des ID d’objet Azure pour les paramètres `--resource-group` et `--vault-name`, pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="69d51-2946">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="69d51-2947">Modification des paramètres `--name` pour accepter le format de sortie des commandes `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="69d51-2947">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="69d51-2948">Conteneur</span><span class="sxs-lookup"><span data-stu-id="69d51-2948">Container</span></span>

* <span data-ttu-id="69d51-2949">Ajout de la commande `container exec`</span><span class="sxs-lookup"><span data-stu-id="69d51-2949">Added `container exec` command.</span></span> <span data-ttu-id="69d51-2950">Exécute les commandes dans un conteneur, pour un groupe de conteneurs en exécution.</span><span class="sxs-lookup"><span data-stu-id="69d51-2950">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="69d51-2951">Autoriser la sortie de table pour la création et la mise à jour d’un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="69d51-2951">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="69d51-2952">Extension</span><span class="sxs-lookup"><span data-stu-id="69d51-2952">Extension</span></span>

* <span data-ttu-id="69d51-2953">Ajout d’un message pour `extension add` si l’extension est en préversion</span><span class="sxs-lookup"><span data-stu-id="69d51-2953">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="69d51-2954">Modification de `extension list-available` afin d’afficher les données complètes d’extension avec `--show-details`</span><span class="sxs-lookup"><span data-stu-id="69d51-2954">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="69d51-2955">[CHANGEMENT CASSANT] Modification de `extension list-available` afin d’afficher les données simplifiées d’extension par défaut</span><span class="sxs-lookup"><span data-stu-id="69d51-2955">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="69d51-2956">Interactive</span><span class="sxs-lookup"><span data-stu-id="69d51-2956">Interactive</span></span>

* <span data-ttu-id="69d51-2957">Modification des saisies semi-automatiques pour procéder à l’activation dès le chargement de la table de commande</span><span class="sxs-lookup"><span data-stu-id="69d51-2957">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="69d51-2958">Correction du bogue par l’exécution du paramètre `--style`</span><span class="sxs-lookup"><span data-stu-id="69d51-2958">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="69d51-2959">Analyseur lexical interactif instancié après le vidage de la table de commande, si manquant</span><span class="sxs-lookup"><span data-stu-id="69d51-2959">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="69d51-2960">Amélioration de la prise en charge de Completer</span><span class="sxs-lookup"><span data-stu-id="69d51-2960">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="69d51-2961">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="69d51-2961">Lab</span></span>

* <span data-ttu-id="69d51-2962">Correction des bogues avec la commande `create environment`</span><span class="sxs-lookup"><span data-stu-id="69d51-2962">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="69d51-2963">Superviser</span><span class="sxs-lookup"><span data-stu-id="69d51-2963">Monitor</span></span>

* <span data-ttu-id="69d51-2964">Ajout de la prise en charge de `--top`, `--orderby` et `--namespace` à `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="69d51-2964">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="69d51-2965">Résolution de [#4529](https://github.com/Azure/azure-cli/issues/5785) : `metrics list` accepte une liste de mesures séparées par des espaces pour la récupération</span><span class="sxs-lookup"><span data-stu-id="69d51-2965">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="69d51-2966">Ajout de la prise en charge de `--namespace` à `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="69d51-2966">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="69d51-2967">Réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-2967">Network</span></span>

* <span data-ttu-id="69d51-2968">Ajout de la prise en charge des zones de DNS privé</span><span class="sxs-lookup"><span data-stu-id="69d51-2968">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="69d51-2969">Profil</span><span class="sxs-lookup"><span data-stu-id="69d51-2969">Profile</span></span>

* <span data-ttu-id="69d51-2970">Ajout d’un avertissement pour `--identity-port` et `--msi-port` à `login`</span><span class="sxs-lookup"><span data-stu-id="69d51-2970">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="69d51-2971">SGBDR</span><span class="sxs-lookup"><span data-stu-id="69d51-2971">RDBMS</span></span>

* <span data-ttu-id="69d51-2972">Ajout de la version d’API mise à la disposition générale du modèle d’entreprise 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="69d51-2972">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="69d51-2973">Ressource</span><span class="sxs-lookup"><span data-stu-id="69d51-2973">Resource</span></span>

* [CHANGEMENT CASSANT]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="69d51-2975">Role</span><span class="sxs-lookup"><span data-stu-id="69d51-2975">Role</span></span>

* <span data-ttu-id="69d51-2976">Ajout de la prise en charge des configurations d’accès et des clients natifs requis à `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="69d51-2976">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="69d51-2977">Modification des commandes `rbac` afin de renvoyer moins de 1 000 ID sur la résolution d’objet</span><span class="sxs-lookup"><span data-stu-id="69d51-2977">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="69d51-2978">Ajout des commandes de gestion des informations d’identification `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="69d51-2978">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="69d51-2979">[CHANGEMENT CASSANT] Suppression des propriétés de la sortie `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="69d51-2979">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="69d51-2980">Ajout de la prise en charge des autorisations `dataActions` et `notDataActions` à `role definition`</span><span class="sxs-lookup"><span data-stu-id="69d51-2980">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="69d51-2981">Stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-2981">Storage</span></span>

* <span data-ttu-id="69d51-2982">Résolution du problème lié au chargement des fichiers présentant une taille comprise entre 195 Go et 200 Go</span><span class="sxs-lookup"><span data-stu-id="69d51-2982">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="69d51-2983">Résolution de [#4049](https://github.com/Azure/azure-cli/issues/4049) : problèmes avec les chargements d’objets blob d’ajout ignorant les paramètres de condition</span><span class="sxs-lookup"><span data-stu-id="69d51-2983">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="69d51-2984">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="69d51-2984">VM</span></span>

* <span data-ttu-id="69d51-2985">Ajout d’un avertissement à `vmss create` concernant les changements cassants à venir pour les ensembles comprenant plus de 100 instances</span><span class="sxs-lookup"><span data-stu-id="69d51-2985">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="69d51-2986">Ajout de la prise en charge de la résilience dans la zone à `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="69d51-2986">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="69d51-2987">Modification de la vue d’instance de disque pour signaler un meilleur état de chiffrement</span><span class="sxs-lookup"><span data-stu-id="69d51-2987">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="69d51-2988">[CHANGEMENT CASSANT] Modification de `vm extension delete` afin d’annuler la capacité de génération de sortie</span><span class="sxs-lookup"><span data-stu-id="69d51-2988">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="69d51-2989">13 mars 2018</span><span class="sxs-lookup"><span data-stu-id="69d51-2989">March 13, 2018</span></span>

<span data-ttu-id="69d51-2990">Version 2.0.29</span><span class="sxs-lookup"><span data-stu-id="69d51-2990">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="69d51-2991">ACR</span><span class="sxs-lookup"><span data-stu-id="69d51-2991">ACR</span></span>

* <span data-ttu-id="69d51-2992">Ajout de la prise en charge du paramètre `--image` pour `repository delete`</span><span class="sxs-lookup"><span data-stu-id="69d51-2992">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="69d51-2993">Paramètres `--manifest` et `--tag` de la commande `repository delete` déconseillés</span><span class="sxs-lookup"><span data-stu-id="69d51-2993">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="69d51-2994">Ajout de la commande `repository untag` pour supprimer une balise sans supprimer les données</span><span class="sxs-lookup"><span data-stu-id="69d51-2994">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="69d51-2995">ACS</span><span class="sxs-lookup"><span data-stu-id="69d51-2995">ACS</span></span>

* <span data-ttu-id="69d51-2996">Ajout de la commande `aks upgrade-connector` pour mettre à niveau un connecteur existant</span><span class="sxs-lookup"><span data-stu-id="69d51-2996">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="69d51-2997">Modification des fichiers de configuration `kubectl` pour utiliser un YAML de style bloc plus lisible</span><span class="sxs-lookup"><span data-stu-id="69d51-2997">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="69d51-2998">Advisor</span><span class="sxs-lookup"><span data-stu-id="69d51-2998">Advisor</span></span>

* <span data-ttu-id="69d51-2999">[CHANGEMENT CASSANT] Renommage de `advisor configuration get` en `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="69d51-2999">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="69d51-3000">[CHANGEMENT CASSANT] Renommage de `advisor configuration set` en `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="69d51-3000">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="69d51-3001">[CHANGEMENT CASSANT] Suppression de `advisor recommendation generate`</span><span class="sxs-lookup"><span data-stu-id="69d51-3001">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="69d51-3002">Ajout du paramètre `--refresh` pour `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="69d51-3002">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="69d51-3003">Ajout de la commande `advisor recommendation show`</span><span class="sxs-lookup"><span data-stu-id="69d51-3003">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="69d51-3004">AppService</span><span class="sxs-lookup"><span data-stu-id="69d51-3004">Appservice</span></span>

* <span data-ttu-id="69d51-3005">`[webapp|functionapp] assign-identity` déconseillé</span><span class="sxs-lookup"><span data-stu-id="69d51-3005">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="69d51-3006">Ajout des commandes d’identité gérée `webapp identity [assign|show]` et `functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="69d51-3006">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="69d51-3007">Eventhubs</span><span class="sxs-lookup"><span data-stu-id="69d51-3007">Eventhubs</span></span>

* <span data-ttu-id="69d51-3008">Version initiale</span><span class="sxs-lookup"><span data-stu-id="69d51-3008">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="69d51-3009">Extension</span><span class="sxs-lookup"><span data-stu-id="69d51-3009">Extension</span></span>

* <span data-ttu-id="69d51-3010">Ajout d’un contrôle supplémentaire pour avertir l’utilisateur si le distributeur utilisé est différent de celui stocké dans le fichier source du package, car cela peut entraîner des erreurs</span><span class="sxs-lookup"><span data-stu-id="69d51-3010">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="69d51-3011">Interactive</span><span class="sxs-lookup"><span data-stu-id="69d51-3011">Interactive</span></span>

* <span data-ttu-id="69d51-3012">Résolution de [#5625](https://github.com/Azure/azure-cli/issues/5625) : conservation de l’historique entre différentes sessions</span><span class="sxs-lookup"><span data-stu-id="69d51-3012">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="69d51-3013">Résolution de [#3016](https://github.com/Azure/azure-cli/issues/3016) : historique non enregistré alors qu’il était dans la portée</span><span class="sxs-lookup"><span data-stu-id="69d51-3013">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="69d51-3014">Résolution de [#5688](https://github.com/Azure/azure-cli/issues/5688) : la saisie automatique n’apparaît pas si le chargement de la table de commande a rencontré une exception</span><span class="sxs-lookup"><span data-stu-id="69d51-3014">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="69d51-3015">Résolu : indicateur de progression pour les opérations à long terme</span><span class="sxs-lookup"><span data-stu-id="69d51-3015">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="69d51-3016">Superviser</span><span class="sxs-lookup"><span data-stu-id="69d51-3016">Monitor</span></span>

* <span data-ttu-id="69d51-3017">Les commandes `monitor autoscale-settings` ont été déconseillées</span><span class="sxs-lookup"><span data-stu-id="69d51-3017">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="69d51-3018">Ajout des commandes `monitor autoscale`</span><span class="sxs-lookup"><span data-stu-id="69d51-3018">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="69d51-3019">Ajout des commandes `monitor autoscale profile`</span><span class="sxs-lookup"><span data-stu-id="69d51-3019">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="69d51-3020">Ajout des commandes `monitor autoscale rule`</span><span class="sxs-lookup"><span data-stu-id="69d51-3020">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="69d51-3021">Réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-3021">Network</span></span>

* <span data-ttu-id="69d51-3022">[CHANGEMENT CASSANT] Suppression du paramètre `--tags` de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="69d51-3022">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="69d51-3023">Suppression de certaines valeurs par défaut erronées pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="69d51-3023">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="69d51-3024">Ajout des commandes `network watcher connection-monitor`</span><span class="sxs-lookup"><span data-stu-id="69d51-3024">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="69d51-3025">Ajout des paramètres `--vnet` et `--subnet` à `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="69d51-3025">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="69d51-3026">Profil</span><span class="sxs-lookup"><span data-stu-id="69d51-3026">Profile</span></span>

* <span data-ttu-id="69d51-3027">Paramètre `--msi` déconseillé pour `az login`</span><span class="sxs-lookup"><span data-stu-id="69d51-3027">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="69d51-3028">Ajout du paramètre `--identity` pour `az login` afin de remplacer `--msi`</span><span class="sxs-lookup"><span data-stu-id="69d51-3028">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="69d51-3029">SGBDR</span><span class="sxs-lookup"><span data-stu-id="69d51-3029">RDBMS</span></span>

* <span data-ttu-id="69d51-3030">[PRÉVERSION] Modifiée pour utiliser l’API 2017-12-01-préversion</span><span class="sxs-lookup"><span data-stu-id="69d51-3030">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="69d51-3031">Service Bus</span><span class="sxs-lookup"><span data-stu-id="69d51-3031">Service Bus</span></span>

* <span data-ttu-id="69d51-3032">Version initiale</span><span class="sxs-lookup"><span data-stu-id="69d51-3032">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="69d51-3033">Stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-3033">Storage</span></span>

* <span data-ttu-id="69d51-3034">Résolution de [#4971](https://github.com/Azure/azure-cli/issues/4971) : `storage blob copy` prend désormais en charge les autres clouds Azure</span><span class="sxs-lookup"><span data-stu-id="69d51-3034">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="69d51-3035">Résolution de [#5286](https://github.com/Azure/azure-cli/issues/5286) : les commandes batch `storage blob [delete-batch|download-batch|upload-batch]` ne génèrent plus d’erreur lors d’échecs de la condition préalable</span><span class="sxs-lookup"><span data-stu-id="69d51-3035">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="69d51-3036">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="69d51-3036">VM</span></span>

* <span data-ttu-id="69d51-3037">Ajout de prise en charge de `[vm|vmss] create` pour attacher des disques de données non gérées et configurer la mise en cache</span><span class="sxs-lookup"><span data-stu-id="69d51-3037">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="69d51-3038">`[vm|vmss] assign-identity` et `[vm|vmss] remove-identity` sont déconseillés</span><span class="sxs-lookup"><span data-stu-id="69d51-3038">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="69d51-3039">Ajout des commandes `vm identity [assign|remove|show]` et `vmss identity [assign|remove|show]` pour remplacer des commandes déconseillées</span><span class="sxs-lookup"><span data-stu-id="69d51-3039">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="69d51-3040">Modification de la priorité par défaut dans `vmss create` à None</span><span class="sxs-lookup"><span data-stu-id="69d51-3040">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="69d51-3041">27 février 2018</span><span class="sxs-lookup"><span data-stu-id="69d51-3041">February 27, 2018</span></span>

<span data-ttu-id="69d51-3042">Version 2.0.28</span><span class="sxs-lookup"><span data-stu-id="69d51-3042">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="69d51-3043">Core</span><span class="sxs-lookup"><span data-stu-id="69d51-3043">Core</span></span>

* <span data-ttu-id="69d51-3044">Résolution de [#5184](https://github.com/Azure/azure-cli/issues/5184) : problème d’installation d’Homebrew</span><span class="sxs-lookup"><span data-stu-id="69d51-3044">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="69d51-3045">Ajout de la prise en charge de télémétrie d’extension avec des clés personnalisées</span><span class="sxs-lookup"><span data-stu-id="69d51-3045">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="69d51-3046">Ajout de la connexion HTTP à `--debug`</span><span class="sxs-lookup"><span data-stu-id="69d51-3046">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="69d51-3047">ACS</span><span class="sxs-lookup"><span data-stu-id="69d51-3047">ACS</span></span>

* <span data-ttu-id="69d51-3048">Modification pour utiliser le graphique Helm `virtual-kubelet-for-aks` pour `aks install-connector` par défaut</span><span class="sxs-lookup"><span data-stu-id="69d51-3048">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="69d51-3049">Résolution de #7161 : autorisation insuffisante des principaux de service pour la création de groupe de conteneurs ACI</span><span class="sxs-lookup"><span data-stu-id="69d51-3049">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="69d51-3050">Ajout des paramètres `--aci-container-group`, `--location` et `--image-tag` à `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="69d51-3050">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="69d51-3051">Suppression de l’avis de désapprobation de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="69d51-3051">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="69d51-3052">AppService</span><span class="sxs-lookup"><span data-stu-id="69d51-3052">Appservice</span></span>

* <span data-ttu-id="69d51-3053">Mises à jour pour la nouvelle version du kit de développement logiciel (SDK) (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="69d51-3053">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="69d51-3054">Résolu [#5538](https://github.com/Azure/azure-cli/issues/5538) : `Free` défini comme une SKU invalide</span><span class="sxs-lookup"><span data-stu-id="69d51-3054">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="69d51-3055">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="69d51-3055">Cognitive Services</span></span>

* <span data-ttu-id="69d51-3056">Mise à jour de l’avis lors de la création d’un compte Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="69d51-3056">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="69d51-3057">Consommation</span><span class="sxs-lookup"><span data-stu-id="69d51-3057">Consumption</span></span>

* <span data-ttu-id="69d51-3058">Ajout de nouvelles commandes pour l’API priceSheet</span><span class="sxs-lookup"><span data-stu-id="69d51-3058">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="69d51-3059">Mise à jour des formats existants Détails d’utilisations et Détails de la réservation</span><span class="sxs-lookup"><span data-stu-id="69d51-3059">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="69d51-3060">Conteneur</span><span class="sxs-lookup"><span data-stu-id="69d51-3060">Container</span></span>

* <span data-ttu-id="69d51-3061">Ajout des arguments `--secrets` et `--secrets-mount-path` à `container create` pour utiliser des secrets dans ACI</span><span class="sxs-lookup"><span data-stu-id="69d51-3061">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="69d51-3062">Réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-3062">Network</span></span>

* <span data-ttu-id="69d51-3063">Résolution de [#5559](https://github.com/Azure/azure-cli/issues/5559) : client manquant dans `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="69d51-3063">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="69d51-3064">Ressource</span><span class="sxs-lookup"><span data-stu-id="69d51-3064">Resource</span></span>

* <span data-ttu-id="69d51-3065">Modification de `group deployment export` pour afficher un modèle et des erreurs partiels sur échec</span><span class="sxs-lookup"><span data-stu-id="69d51-3065">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="69d51-3066">Role</span><span class="sxs-lookup"><span data-stu-id="69d51-3066">Role</span></span>

* <span data-ttu-id="69d51-3067">Ajout de `role assignment list-changelogs` pour permettre l’audit des rôles du principal de service</span><span class="sxs-lookup"><span data-stu-id="69d51-3067">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="69d51-3068">SQL</span><span class="sxs-lookup"><span data-stu-id="69d51-3068">SQL</span></span>

* <span data-ttu-id="69d51-3069">Ajout de la prise en charge de la redondance de zone pour les bases de données et les pools élastiques lors de création et mise à jour</span><span class="sxs-lookup"><span data-stu-id="69d51-3069">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="69d51-3070">Stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-3070">Storage</span></span>

* <span data-ttu-id="69d51-3071">Activation de la spécification de préfixe/destination pour `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="69d51-3071">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="69d51-3072">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="69d51-3072">VM</span></span>

* <span data-ttu-id="69d51-3073">Ajout de prise en charge de jonction / séparation de disques sur une instance de groupe de machines virtuelles identiques uniques</span><span class="sxs-lookup"><span data-stu-id="69d51-3073">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="69d51-3074">13 février 2018</span><span class="sxs-lookup"><span data-stu-id="69d51-3074">February 13, 2018</span></span>

<span data-ttu-id="69d51-3075">Version 2.0.27</span><span class="sxs-lookup"><span data-stu-id="69d51-3075">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="69d51-3076">Core</span><span class="sxs-lookup"><span data-stu-id="69d51-3076">Core</span></span>

* <span data-ttu-id="69d51-3077">Modification de l’authentification pour passer au système de clé sur l’ID d’abonnement et le nom sur la connexion MSI</span><span class="sxs-lookup"><span data-stu-id="69d51-3077">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="69d51-3078">ACS</span><span class="sxs-lookup"><span data-stu-id="69d51-3078">ACS</span></span>

* <span data-ttu-id="69d51-3079">[CHANGEMENT CASSANT] Renommage de `aks get-versions` en `aks get-upgrades` pour des raisons de précision</span><span class="sxs-lookup"><span data-stu-id="69d51-3079">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="69d51-3080">Modification de `aks get-versions` pour afficher les versions Kubernetes disponibles pour `aks create`</span><span class="sxs-lookup"><span data-stu-id="69d51-3080">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="69d51-3081">Modification des valeurs par défaut de `aks create` de manière à laisser le serveur choisir la version de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="69d51-3081">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="69d51-3082">Mise à jour des messages d’aide faisant référence au principal du service généré par AKS</span><span class="sxs-lookup"><span data-stu-id="69d51-3082">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="69d51-3083">Modification des tailles de nœud par défaut pour `aks create` pour passer de « Standard\_D1\_v2 » à « Standard\_DS1\_v2 »</span><span class="sxs-lookup"><span data-stu-id="69d51-3083">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="69d51-3084">Meilleure fiabilité lors de la localisation du pod de tableau de bord pour `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="69d51-3084">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="69d51-3085">Correction de `aks get-credentials` pour gérer les erreurs Unicode lors du chargement des fichiers de configuration Kubernetes</span><span class="sxs-lookup"><span data-stu-id="69d51-3085">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="69d51-3086">Ajout d’un message à `az aks install-cli` pour aider à l’obtention de `kubectl` dans `$PATH`</span><span class="sxs-lookup"><span data-stu-id="69d51-3086">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="69d51-3087">AppService</span><span class="sxs-lookup"><span data-stu-id="69d51-3087">Appservice</span></span>

* <span data-ttu-id="69d51-3088">Résolution du problème dans lequel `webapp [backup|restore]` a échoué en raison d’une référence null</span><span class="sxs-lookup"><span data-stu-id="69d51-3088">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="69d51-3089">Ajout de la prise en charge supplémentaire des plans App Service par défaut via `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="69d51-3089">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="69d51-3090">CDN</span><span class="sxs-lookup"><span data-stu-id="69d51-3090">CDN</span></span>

* <span data-ttu-id="69d51-3091">Ajout des commandes `cdn custom-domain [enable-https|disable-https]`</span><span class="sxs-lookup"><span data-stu-id="69d51-3091">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="69d51-3092">Conteneur</span><span class="sxs-lookup"><span data-stu-id="69d51-3092">Container</span></span>

* <span data-ttu-id="69d51-3093">Ajout de l’option `--follow` à `az container logs` pour les journaux d’activité de diffusion en continu</span><span class="sxs-lookup"><span data-stu-id="69d51-3093">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="69d51-3094">Ajout de la commande `container attach` qui associe les flux d’erreur et de sortie standard locaux à un conteneur d’un groupe de conteneur</span><span class="sxs-lookup"><span data-stu-id="69d51-3094">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="69d51-3095">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="69d51-3095">CosmosDB</span></span>

* <span data-ttu-id="69d51-3096">Ajout de la prise en charge de la définition de fonctionnalités</span><span class="sxs-lookup"><span data-stu-id="69d51-3096">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="69d51-3097">Extension</span><span class="sxs-lookup"><span data-stu-id="69d51-3097">Extension</span></span>

* <span data-ttu-id="69d51-3098">Ajout de la prise en charge du paramètre `--pip-proxy` pour les commandes `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="69d51-3098">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="69d51-3099">Ajout de la prise en charge de l’argument `--pip-extra-index-urls` pour les commandes `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="69d51-3099">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="69d51-3100">Commentaires</span><span class="sxs-lookup"><span data-stu-id="69d51-3100">Feedback</span></span>

* <span data-ttu-id="69d51-3101">Ajout d’informations d’extension aux données de télémétrie</span><span class="sxs-lookup"><span data-stu-id="69d51-3101">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="69d51-3102">Interactive</span><span class="sxs-lookup"><span data-stu-id="69d51-3102">Interactive</span></span>

* <span data-ttu-id="69d51-3103">Résolution du problème dans lequel l’utilisateur est invité à se connecter à l’aide du mode interactif dans Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="69d51-3103">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="69d51-3104">Correction de la régression avec les listes de saisie semi-automatique des paramètres manquants</span><span class="sxs-lookup"><span data-stu-id="69d51-3104">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="69d51-3105">IoT</span><span class="sxs-lookup"><span data-stu-id="69d51-3105">IoT</span></span>

* <span data-ttu-id="69d51-3106">Résolution du problème dans lequel `iot dps access policy [create|update]` renvoie une erreur « introuvable » en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="69d51-3106">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="69d51-3107">Résolution du problème dans lequel `iot dps linked-hub [create|update]` renvoie une erreur « introuvable » en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="69d51-3107">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="69d51-3108">Ajout de la prise en charge de `--no-wait` pour `iot dps access policy [create|update]` et `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69d51-3108">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="69d51-3109">Modification de `iot hub create` pour autoriser la spécification du nombre de partitions</span><span class="sxs-lookup"><span data-stu-id="69d51-3109">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="69d51-3110">Superviser</span><span class="sxs-lookup"><span data-stu-id="69d51-3110">Monitor</span></span>

* <span data-ttu-id="69d51-3111">Correction de la commande `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="69d51-3111">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="69d51-3112">Réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-3112">Network</span></span>

* <span data-ttu-id="69d51-3113">Correction de l’option `--tags` pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="69d51-3113">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="69d51-3114">Profil</span><span class="sxs-lookup"><span data-stu-id="69d51-3114">Profile</span></span>

* <span data-ttu-id="69d51-3115">Activation `az login` à partir du mode interactif</span><span class="sxs-lookup"><span data-stu-id="69d51-3115">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="69d51-3116">Ressource</span><span class="sxs-lookup"><span data-stu-id="69d51-3116">Resource</span></span>

* <span data-ttu-id="69d51-3117">Rajout de `feature show`</span><span class="sxs-lookup"><span data-stu-id="69d51-3117">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="69d51-3118">Role</span><span class="sxs-lookup"><span data-stu-id="69d51-3118">Role</span></span>

* <span data-ttu-id="69d51-3119">Ajout de l’argument `--available-to-other-tenants` à `ad app update`</span><span class="sxs-lookup"><span data-stu-id="69d51-3119">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="69d51-3120">SQL</span><span class="sxs-lookup"><span data-stu-id="69d51-3120">SQL</span></span>

* <span data-ttu-id="69d51-3121">Ajout des commandes `sql server dns-alias`</span><span class="sxs-lookup"><span data-stu-id="69d51-3121">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="69d51-3122">Ajout de `sql db rename`</span><span class="sxs-lookup"><span data-stu-id="69d51-3122">Added `sql db rename`</span></span>
* <span data-ttu-id="69d51-3123">Ajout de la prise en charge de l’argument `--ids` pour toutes les commandes sql</span><span class="sxs-lookup"><span data-stu-id="69d51-3123">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="69d51-3124">Stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-3124">Storage</span></span>

* <span data-ttu-id="69d51-3125">Ajout des commandes `storage blob service-properties delete-policy` et `storage blob undelete` pour permettre une suppression réversible</span><span class="sxs-lookup"><span data-stu-id="69d51-3125">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="69d51-3126">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="69d51-3126">VM</span></span>

* <span data-ttu-id="69d51-3127">Correction d’un incident lorsque le chiffrement de la machine virtuelle ne peut pas être initialisé entièrement</span><span class="sxs-lookup"><span data-stu-id="69d51-3127">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="69d51-3128">Ajout de la sortie d’ID du principal lors de l’activation de MSI</span><span class="sxs-lookup"><span data-stu-id="69d51-3128">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="69d51-3129">`vm boot-diagnostics get-boot-log` fixe</span><span class="sxs-lookup"><span data-stu-id="69d51-3129">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="69d51-3130">31 janvier 2018</span><span class="sxs-lookup"><span data-stu-id="69d51-3130">January 31, 2018</span></span>

<span data-ttu-id="69d51-3131">Version 2.0.26</span><span class="sxs-lookup"><span data-stu-id="69d51-3131">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="69d51-3132">Core</span><span class="sxs-lookup"><span data-stu-id="69d51-3132">Core</span></span>

* <span data-ttu-id="69d51-3133">Ajout de la prise en charge de la récupération du jeton brut dans le contexte MSI</span><span class="sxs-lookup"><span data-stu-id="69d51-3133">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="69d51-3134">Suppression de la chaîne de l’indicateur d’interrogation après la fin de LRO sur le fichier cmd.exe de Windows</span><span class="sxs-lookup"><span data-stu-id="69d51-3134">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="69d51-3135">Ajout d’un avertissement qui s’affiche lorsque l’utilisation d’une valeur par défaut configurée a été remplacée par une entrée de niveau INFO.</span><span class="sxs-lookup"><span data-stu-id="69d51-3135">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="69d51-3136">Utilisation de `--verbose` pour voir</span><span class="sxs-lookup"><span data-stu-id="69d51-3136">Use `--verbose` to see</span></span>
* <span data-ttu-id="69d51-3137">Ajouter un indicateur de progression pour les commandes wait</span><span class="sxs-lookup"><span data-stu-id="69d51-3137">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="69d51-3138">ACS</span><span class="sxs-lookup"><span data-stu-id="69d51-3138">ACS</span></span>

* <span data-ttu-id="69d51-3139">Clarification de l’argument `--disable-browser`</span><span class="sxs-lookup"><span data-stu-id="69d51-3139">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="69d51-3140">Amélioration de la touche TAB pour les arguments `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="69d51-3140">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="69d51-3141">AppService</span><span class="sxs-lookup"><span data-stu-id="69d51-3141">Appservice</span></span>

* <span data-ttu-id="69d51-3142">`webapp log [tail|download]` fixe</span><span class="sxs-lookup"><span data-stu-id="69d51-3142">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="69d51-3143">Suppression de la vérification de `kind` sur les fonctions et les applications web</span><span class="sxs-lookup"><span data-stu-id="69d51-3143">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="69d51-3144">CDN</span><span class="sxs-lookup"><span data-stu-id="69d51-3144">CDN</span></span>

* <span data-ttu-id="69d51-3145">Résolution du problème de client manquant avec `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="69d51-3145">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="69d51-3146">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="69d51-3146">CosmosDB</span></span>

* <span data-ttu-id="69d51-3147">Correction de la description du paramètre pour les stratégies de basculement</span><span class="sxs-lookup"><span data-stu-id="69d51-3147">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="69d51-3148">Interactive</span><span class="sxs-lookup"><span data-stu-id="69d51-3148">Interactive</span></span>

* <span data-ttu-id="69d51-3149">Résolution du problème dans lequel les listes de saisie semi-automatique d’option de commande ne s’affichent plus</span><span class="sxs-lookup"><span data-stu-id="69d51-3149">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="69d51-3150">Réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-3150">Network</span></span>

* <span data-ttu-id="69d51-3151">Ajout de la protection pour `--cert-password` à `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="69d51-3151">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="69d51-3152">Résolution du problème lié à `application-gateway update` où `--sku` a appliqué par erreur une valeur par défaut</span><span class="sxs-lookup"><span data-stu-id="69d51-3152">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="69d51-3153">Ajout de la protection pour `--shared-key` et `--authorization-key` à `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="69d51-3153">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="69d51-3154">Résolution du problème de client manquant avec `asg create`</span><span class="sxs-lookup"><span data-stu-id="69d51-3154">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="69d51-3155">Ajout du paramètre `--file-name / -f` pour les noms exportés à `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="69d51-3155">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="69d51-3156">Les problèmes suivants liés à `dns zone export` ont été résolus :</span><span class="sxs-lookup"><span data-stu-id="69d51-3156">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="69d51-3157">Résolution du problème dans lequel des enregistrements TXT longs ont été mal exportés</span><span class="sxs-lookup"><span data-stu-id="69d51-3157">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="69d51-3158">Résolution du problème dans lequel des enregistrements TXT entre guillemets ont été mal exportés sans guillemets placés dans une séquence d’échappement.</span><span class="sxs-lookup"><span data-stu-id="69d51-3158">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="69d51-3159">Résolution du problème où certains enregistrements ont été importés à deux reprises avec `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="69d51-3159">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="69d51-3160">Restauration des commandes `vnet-gateway root-cert` et `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="69d51-3160">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="69d51-3161">Profil</span><span class="sxs-lookup"><span data-stu-id="69d51-3161">Profile</span></span>

* <span data-ttu-id="69d51-3162">Correction de `get-access-token` pour qu’il fonctionne à l’intérieur d’une machine virtuelle avec l’identité</span><span class="sxs-lookup"><span data-stu-id="69d51-3162">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="69d51-3163">Ressource</span><span class="sxs-lookup"><span data-stu-id="69d51-3163">Resource</span></span>

* <span data-ttu-id="69d51-3164">Correction du bogue lié à `deployment [create|validate]` où un avertissement ne s’est pas affiché correctement quand un champ ’type’ du modèle contient des valeurs en majuscules</span><span class="sxs-lookup"><span data-stu-id="69d51-3164">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="69d51-3165">Stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-3165">Storage</span></span>

* <span data-ttu-id="69d51-3166">Résolution du problème lié à la migration des comptes Storage V1 vers Storage V2</span><span class="sxs-lookup"><span data-stu-id="69d51-3166">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="69d51-3167">Ajout de la création progressive de rapports pour toutes les commandes de chargement/téléchargement</span><span class="sxs-lookup"><span data-stu-id="69d51-3167">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="69d51-3168">Résolution du bogue empêchant l’option d’argument « -n » avec `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="69d51-3168">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="69d51-3169">Ajout de la colonne de « snapshot » ajouté à la sortie de table pour `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="69d51-3169">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="69d51-3170">Résolution des bogues dans lesquels différents paramètres devaient être analysés en tant qu’entiers</span><span class="sxs-lookup"><span data-stu-id="69d51-3170">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="69d51-3171">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="69d51-3171">VM</span></span>

* <span data-ttu-id="69d51-3172">Ajout de la commande `vm image accept-terms` pour autoriser la création de machines virtuelles à partir d’images moyennant des frais supplémentaires</span><span class="sxs-lookup"><span data-stu-id="69d51-3172">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="69d51-3173">Correction de `[vm|vmss create]` pour garantir l’exécution des commandes sous un proxy avec des certificats non signés</span><span class="sxs-lookup"><span data-stu-id="69d51-3173">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="69d51-3174">[APERÇU] Ajout de la prise en charge de la priorité « faible» au groupe de machines virtuelles identiques</span><span class="sxs-lookup"><span data-stu-id="69d51-3174">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="69d51-3175">Ajout de la protection pour `--admin-password` à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="69d51-3175">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="69d51-3176">17 janvier 2018</span><span class="sxs-lookup"><span data-stu-id="69d51-3176">January 17, 2018</span></span>

<span data-ttu-id="69d51-3177">Version 2.0.25</span><span class="sxs-lookup"><span data-stu-id="69d51-3177">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="69d51-3178">ACR</span><span class="sxs-lookup"><span data-stu-id="69d51-3178">ACR</span></span>

* <span data-ttu-id="69d51-3179">Ajout d’une connexion acr de secours en cas d’erreurs d’informations d’identification Windows</span><span class="sxs-lookup"><span data-stu-id="69d51-3179">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="69d51-3180">Activation des journaux d’activité du Registre</span><span class="sxs-lookup"><span data-stu-id="69d51-3180">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="69d51-3181">ACS</span><span class="sxs-lookup"><span data-stu-id="69d51-3181">ACS</span></span>

* <span data-ttu-id="69d51-3182">Correction de la commande `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="69d51-3182">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="69d51-3183">Suppression de l’exigence de rôle SPN</span><span class="sxs-lookup"><span data-stu-id="69d51-3183">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="69d51-3184">AppService</span><span class="sxs-lookup"><span data-stu-id="69d51-3184">Appservice</span></span>

* <span data-ttu-id="69d51-3185">Correction du bogue avec `config ssl upload` où `hosting_environment_profile` avait la valeur null</span><span class="sxs-lookup"><span data-stu-id="69d51-3185">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="69d51-3186">Ajout de la prise en charge des URL personnalisées pour `browse`</span><span class="sxs-lookup"><span data-stu-id="69d51-3186">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="69d51-3187">Prise en charge de l’emplacement fixe pour `log tail`</span><span class="sxs-lookup"><span data-stu-id="69d51-3187">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="69d51-3188">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="69d51-3188">Backup</span></span>

* <span data-ttu-id="69d51-3189">Modification de l’option `--container-name` de `backup item list` désormais facultative</span><span class="sxs-lookup"><span data-stu-id="69d51-3189">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="69d51-3190">Ajout d’options de compte de stockage à `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="69d51-3190">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="69d51-3191">Correction de la vérification de l’emplacement dans `backup protection enable-for-vm`, ne tient désormais plus compte de la casse</span><span class="sxs-lookup"><span data-stu-id="69d51-3191">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="69d51-3192">Correction d’un problème qui causait l’échec des commandes avec un nom de conteneur non valide</span><span class="sxs-lookup"><span data-stu-id="69d51-3192">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="69d51-3193">Modification de `backup item list` pour inclure « État d’intégrité » par défaut</span><span class="sxs-lookup"><span data-stu-id="69d51-3193">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="69d51-3194">Batch</span><span class="sxs-lookup"><span data-stu-id="69d51-3194">Batch</span></span>

* <span data-ttu-id="69d51-3195">Modification de `batch login` pour retourner des détails d’authentification</span><span class="sxs-lookup"><span data-stu-id="69d51-3195">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="69d51-3196">Cloud</span><span class="sxs-lookup"><span data-stu-id="69d51-3196">Cloud</span></span>

* <span data-ttu-id="69d51-3197">Ne requiert plus de points de terminaison lors de la définition de `--profile` sur un cloud</span><span class="sxs-lookup"><span data-stu-id="69d51-3197">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="69d51-3198">Consommation</span><span class="sxs-lookup"><span data-stu-id="69d51-3198">Consumption</span></span>

* <span data-ttu-id="69d51-3199">Ajout de nouvelles commandes pour les réservations : `consumption reservations summaries` et `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="69d51-3199">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="69d51-3200">Event Grid</span><span class="sxs-lookup"><span data-stu-id="69d51-3200">Event Grid</span></span>

* <span data-ttu-id="69d51-3201">[CHANGEMENT CASSANT] Déplacement des commandes `az eventgrid topic event-subscription` vers `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="69d51-3201">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="69d51-3202">[CHANGEMENT CASSANT] Déplacement des commandes `az eventgrid resource event-subscription` vers `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="69d51-3202">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="69d51-3203">[CHANGEMENT CASSANT] Suppression de la commande `eventgrid event-subscription show-endpoint-url`</span><span class="sxs-lookup"><span data-stu-id="69d51-3203">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="69d51-3204">Utilisation de `eventgrid event-subscription show --include-full-endpoint-url` à la place</span><span class="sxs-lookup"><span data-stu-id="69d51-3204">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="69d51-3205">Ajout de la commande `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="69d51-3205">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="69d51-3206">Ajout de la commande `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="69d51-3206">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="69d51-3207">Ajout du paramètre `--ids` pour les commandes `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="69d51-3207">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="69d51-3208">Ajout de la prise en charge de la saisie semi-automatique via la touche TAB pour les noms de rubrique</span><span class="sxs-lookup"><span data-stu-id="69d51-3208">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="69d51-3209">Interactive</span><span class="sxs-lookup"><span data-stu-id="69d51-3209">Interactive</span></span>

* <span data-ttu-id="69d51-3210">Correction d’un problème qui empêchait le fonctionnement du mode interactif avec Python 2.x</span><span class="sxs-lookup"><span data-stu-id="69d51-3210">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="69d51-3211">Corrections d’erreurs au démarrage</span><span class="sxs-lookup"><span data-stu-id="69d51-3211">Fixed errors on startup</span></span>
* <span data-ttu-id="69d51-3212">Correction du problème de commandes ne s’exécutant pas en mode interactif</span><span class="sxs-lookup"><span data-stu-id="69d51-3212">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="69d51-3213">IoT</span><span class="sxs-lookup"><span data-stu-id="69d51-3213">IoT</span></span>

* <span data-ttu-id="69d51-3214">Ajout de la prise en charge du service de provisionnement des appareils</span><span class="sxs-lookup"><span data-stu-id="69d51-3214">Added support for device provisioning service</span></span>
* <span data-ttu-id="69d51-3215">Ajout de messages de désapprobation dans les commandes et l’aide relative aux commandes</span><span class="sxs-lookup"><span data-stu-id="69d51-3215">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="69d51-3216">Ajout de la vérification IoT pour informer les utilisateurs de l’extension IoT</span><span class="sxs-lookup"><span data-stu-id="69d51-3216">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="69d51-3217">Superviser</span><span class="sxs-lookup"><span data-stu-id="69d51-3217">Monitor</span></span>

* <span data-ttu-id="69d51-3218">Ajout de la prise en charge des paramètres multi diagnostic.</span><span class="sxs-lookup"><span data-stu-id="69d51-3218">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="69d51-3219">Le paramètre `--name` est désormais requis pour `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="69d51-3219">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="69d51-3220">Ajout de la commande `monitor diagnostic-settings categories` pour obtenir la catégorie des paramètres de diagnostic</span><span class="sxs-lookup"><span data-stu-id="69d51-3220">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="69d51-3221">Réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-3221">Network</span></span>

* <span data-ttu-id="69d51-3222">Résolution du problème se produisant lors de la tentative de passage au mode actif-passif, ou depuis ce dernier, avec `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="69d51-3222">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="69d51-3223">Ajout de la prise en charge de HTTP2 vers `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69d51-3223">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="69d51-3224">Profil</span><span class="sxs-lookup"><span data-stu-id="69d51-3224">Profile</span></span>

* <span data-ttu-id="69d51-3225">Ajout de la prise en charge pour la connexion à l’aide d’identités affectées aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="69d51-3225">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="69d51-3226">Role</span><span class="sxs-lookup"><span data-stu-id="69d51-3226">Role</span></span>

* <span data-ttu-id="69d51-3227">Ajout de l’argument `--assignee-object-id` à `role assignment create` pour ignorer les requêtes de graphique</span><span class="sxs-lookup"><span data-stu-id="69d51-3227">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="69d51-3228">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="69d51-3228">Service Fabric</span></span>

* <span data-ttu-id="69d51-3229">Ajout d’erreurs détaillées à la réponse de validation lors de la création du cluster</span><span class="sxs-lookup"><span data-stu-id="69d51-3229">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="69d51-3230">Résolution du problème concernant le client manquant avec plusieurs commandes</span><span class="sxs-lookup"><span data-stu-id="69d51-3230">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="69d51-3231">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="69d51-3231">VM</span></span>

* <span data-ttu-id="69d51-3232">[PRÉVERSION] Prise en charge interzone pour `vmss`</span><span class="sxs-lookup"><span data-stu-id="69d51-3232">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="69d51-3233">[CHANGEMENT CASSANT] Modification de la valeur par défaut `vmss` de zone unique en équilibreur de charge « Standard »</span><span class="sxs-lookup"><span data-stu-id="69d51-3233">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="69d51-3234">[CHANGEMENT CASSANT] Modification de `externalIdentities` en `userAssignedIdentities` pour EMSI</span><span class="sxs-lookup"><span data-stu-id="69d51-3234">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="69d51-3235">[PRÉVERSION] Ajout de la prise en charge de l’échange de disque du système d’exploitation</span><span class="sxs-lookup"><span data-stu-id="69d51-3235">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="69d51-3236">Ajout de la prise en charge de l’utilisation des images de machine virtuelle à partir d’autres abonnements</span><span class="sxs-lookup"><span data-stu-id="69d51-3236">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="69d51-3237">Ajout des arguments `--plan-name`, `--plan-product`, `--plan-promotion-code` et `--plan-publisher` à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="69d51-3237">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="69d51-3238">Correction des problèmes d’erreur avec `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="69d51-3238">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="69d51-3239">Correction de l’utilisation excessive des ressources due à `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="69d51-3239">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="69d51-3240">19 décembre 2017</span><span class="sxs-lookup"><span data-stu-id="69d51-3240">December 19, 2017</span></span>

<span data-ttu-id="69d51-3241">Version 2.0.23</span><span class="sxs-lookup"><span data-stu-id="69d51-3241">Version 2.0.23</span></span>

* <span data-ttu-id="69d51-3242">Ajout de la prise en charge pour la connexion à l’aide d’identités affectées aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="69d51-3242">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="69d51-3243">Conteneur</span><span class="sxs-lookup"><span data-stu-id="69d51-3243">Container</span></span>

* <span data-ttu-id="69d51-3244">Correction de l’ordre incorrect des paramètres pour les journaux d’activité du conteneur</span><span class="sxs-lookup"><span data-stu-id="69d51-3244">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="69d51-3245">Réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-3245">Network</span></span>

* <span data-ttu-id="69d51-3246">Ajout de l’argument `--disable-bgp-route-propagation` à `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69d51-3246">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="69d51-3247">Ajout de l’argument `--ip-tags` à `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69d51-3247">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="69d51-3248">Stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-3248">Storage</span></span>

* <span data-ttu-id="69d51-3249">Ajout de la prise en charge du stockage V2</span><span class="sxs-lookup"><span data-stu-id="69d51-3249">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="69d51-3250">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="69d51-3250">VM</span></span>

* <span data-ttu-id="69d51-3251">[APERÇU] Ajout de la prise en charge des identités affectées aux utilisateurs pour les machines virtuelles et les VMSS</span><span class="sxs-lookup"><span data-stu-id="69d51-3251">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="69d51-3252">5 décembre 2017</span><span class="sxs-lookup"><span data-stu-id="69d51-3252">December 5, 2017</span></span>

<span data-ttu-id="69d51-3253">Version 2.0.22</span><span class="sxs-lookup"><span data-stu-id="69d51-3253">Version 2.0.22</span></span>

* <span data-ttu-id="69d51-3254">Suppression des commandes `az component`.</span><span class="sxs-lookup"><span data-stu-id="69d51-3254">Removed `az component` commands.</span></span> <span data-ttu-id="69d51-3255">Utilisation de `az extension` à la place</span><span class="sxs-lookup"><span data-stu-id="69d51-3255">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="69d51-3256">Core</span><span class="sxs-lookup"><span data-stu-id="69d51-3256">Core</span></span>
* <span data-ttu-id="69d51-3257">Modification du point de terminaison de l’autorité AAD `AZURE_US_GOV_CLOUD` pour le faire passer de login.microsoftonline.com à login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="69d51-3257">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="69d51-3258">Résolution du problème au cours duquel les données de télémétrie étaient constamment renvoyées</span><span class="sxs-lookup"><span data-stu-id="69d51-3258">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="69d51-3259">ACS</span><span class="sxs-lookup"><span data-stu-id="69d51-3259">ACS</span></span>

* <span data-ttu-id="69d51-3260">Ajout des commandes `aks install-connector` et `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="69d51-3260">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="69d51-3261">Amélioration des rapports d’erreurs pour `acs create`</span><span class="sxs-lookup"><span data-stu-id="69d51-3261">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="69d51-3262">Correction de l’utilisation de `aks get-credentials -f` sans chemin d’accès complet</span><span class="sxs-lookup"><span data-stu-id="69d51-3262">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="69d51-3263">Advisor</span><span class="sxs-lookup"><span data-stu-id="69d51-3263">Advisor</span></span>

* <span data-ttu-id="69d51-3264">Version initiale</span><span class="sxs-lookup"><span data-stu-id="69d51-3264">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="69d51-3265">AppService</span><span class="sxs-lookup"><span data-stu-id="69d51-3265">Appservice</span></span>

* <span data-ttu-id="69d51-3266">Correction de la génération du nom de certificat avec `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="69d51-3266">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="69d51-3267">Correction de `webapp [list|show]` et `functionapp [list|show]` de manière à afficher les applications correctes</span><span class="sxs-lookup"><span data-stu-id="69d51-3267">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="69d51-3268">Ajout de la valeur par défaut pour `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="69d51-3268">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="69d51-3269">Consommation</span><span class="sxs-lookup"><span data-stu-id="69d51-3269">Consumption</span></span>

* <span data-ttu-id="69d51-3270">Ajout de la prise en charge de l’API version 2017-11-30</span><span class="sxs-lookup"><span data-stu-id="69d51-3270">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="69d51-3271">Conteneur</span><span class="sxs-lookup"><span data-stu-id="69d51-3271">Container</span></span>

* <span data-ttu-id="69d51-3272">Correction de la régression des ports par défaut</span><span class="sxs-lookup"><span data-stu-id="69d51-3272">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="69d51-3273">Superviser</span><span class="sxs-lookup"><span data-stu-id="69d51-3273">Monitor</span></span>

* <span data-ttu-id="69d51-3274">Ajout de la prise en charge de plusieurs dimensions à la commande des mesures</span><span class="sxs-lookup"><span data-stu-id="69d51-3274">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="69d51-3275">Ressource</span><span class="sxs-lookup"><span data-stu-id="69d51-3275">Resource</span></span>

* <span data-ttu-id="69d51-3276">Ajout de l’argument `--include-response-body` à `resource show`</span><span class="sxs-lookup"><span data-stu-id="69d51-3276">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="69d51-3277">Role</span><span class="sxs-lookup"><span data-stu-id="69d51-3277">Role</span></span>

* <span data-ttu-id="69d51-3278">Ajout de l’affichage des affectations par défaut pour les administrateurs « classiques » à `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="69d51-3278">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="69d51-3279">Ajout de la prise en charge à `ad sp reset-credentials` pour l’ajout d’informations d’identification au lieu de leur remplacement</span><span class="sxs-lookup"><span data-stu-id="69d51-3279">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="69d51-3280">Amélioration des rapports d’erreurs pour `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="69d51-3280">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="69d51-3281">SQL</span><span class="sxs-lookup"><span data-stu-id="69d51-3281">SQL</span></span>

* <span data-ttu-id="69d51-3282">Ajout des commandes `sql db list-usages` et `sql db show-usage`</span><span class="sxs-lookup"><span data-stu-id="69d51-3282">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="69d51-3283">Ajout des commandes `sql server conn-policy show` et `sql server conn-policy update`</span><span class="sxs-lookup"><span data-stu-id="69d51-3283">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="69d51-3284">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="69d51-3284">VM</span></span>

* <span data-ttu-id="69d51-3285">Ajout des informations de zone à `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="69d51-3285">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="69d51-3286">14 novembre 2017</span><span class="sxs-lookup"><span data-stu-id="69d51-3286">November 14, 2017</span></span>

<span data-ttu-id="69d51-3287">Version 2.0.21</span><span class="sxs-lookup"><span data-stu-id="69d51-3287">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="69d51-3288">ACR</span><span class="sxs-lookup"><span data-stu-id="69d51-3288">ACR</span></span>

* <span data-ttu-id="69d51-3289">Ajout de la prise en charge pour la création de webhooks dans les régions de réplication</span><span class="sxs-lookup"><span data-stu-id="69d51-3289">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="69d51-3290">ACS</span><span class="sxs-lookup"><span data-stu-id="69d51-3290">ACS</span></span>

* <span data-ttu-id="69d51-3291">Modification de toutes les mentions « agent » en « nœud » dans AKS</span><span class="sxs-lookup"><span data-stu-id="69d51-3291">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="69d51-3292">Option `--orchestrator-release` déconseillée pour `acs create`</span><span class="sxs-lookup"><span data-stu-id="69d51-3292">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="69d51-3293">Changement de la taille de machine virtuelle par défaut pour AKS à `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="69d51-3293">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="69d51-3294">Résolution de `az aks browse` sur Windows</span><span class="sxs-lookup"><span data-stu-id="69d51-3294">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="69d51-3295">Résolution de `az aks get-credentials` sur Windows</span><span class="sxs-lookup"><span data-stu-id="69d51-3295">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="69d51-3296">AppService</span><span class="sxs-lookup"><span data-stu-id="69d51-3296">Appservice</span></span>

* <span data-ttu-id="69d51-3297">Ajout de la source de déploiement `config-zip` pour les applications Web et de fonction</span><span class="sxs-lookup"><span data-stu-id="69d51-3297">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="69d51-3298">Ajout de l’option `--docker-container-logging` à `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="69d51-3298">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="69d51-3299">Suppression de l’option `storage` du paramètre `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="69d51-3299">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="69d51-3300">Amélioration des messages d’erreur pour `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="69d51-3300">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="69d51-3301">Ajout de la prise en charge pour la création d’applications de fonction Linux</span><span class="sxs-lookup"><span data-stu-id="69d51-3301">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="69d51-3302">`list-locations` fixe</span><span class="sxs-lookup"><span data-stu-id="69d51-3302">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="69d51-3303">Batch</span><span class="sxs-lookup"><span data-stu-id="69d51-3303">Batch</span></span>

* <span data-ttu-id="69d51-3304">Correction du bogue dans la commande de création de pool lorsqu’un ID ressource a été utilisé avec l’indicateur `--image`</span><span class="sxs-lookup"><span data-stu-id="69d51-3304">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="69d51-3305">Batchai</span><span class="sxs-lookup"><span data-stu-id="69d51-3305">Batchai</span></span>

* <span data-ttu-id="69d51-3306">Ajout de l’option courte, `-s`, pour `--vm-size` quand la taille de machine virtuelle est fournie dans la commande `file-server create`</span><span class="sxs-lookup"><span data-stu-id="69d51-3306">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="69d51-3307">Ajout du nom de compte de stockage et des arguments de clé dans les paramètres `cluster create`</span><span class="sxs-lookup"><span data-stu-id="69d51-3307">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="69d51-3308">Résolution de la documentation pour `job list-files` et `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="69d51-3308">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="69d51-3309">Ajout de l’option courte, `-r`, pour `--cluster-name` quand le nom du cluster est fourni dans la commande `job create`</span><span class="sxs-lookup"><span data-stu-id="69d51-3309">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="69d51-3310">Cloud</span><span class="sxs-lookup"><span data-stu-id="69d51-3310">Cloud</span></span>

* <span data-ttu-id="69d51-3311">Modification de `cloud [register|update]` pour empêcher l’inscription des clouds qui ne disposent pas de tous les points de terminaison requis</span><span class="sxs-lookup"><span data-stu-id="69d51-3311">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="69d51-3312">Conteneur</span><span class="sxs-lookup"><span data-stu-id="69d51-3312">Container</span></span>

* <span data-ttu-id="69d51-3313">Ajout de la prise en charge pour ouvrir plusieurs ports</span><span class="sxs-lookup"><span data-stu-id="69d51-3313">Added support to open multiple ports</span></span>
* <span data-ttu-id="69d51-3314">Ajout de la stratégie de redémarrage du groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="69d51-3314">Added container group restart policy</span></span>
* <span data-ttu-id="69d51-3315">Ajout de la prise en charge pour monter le partage de fichier Azure en tant que volume</span><span class="sxs-lookup"><span data-stu-id="69d51-3315">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="69d51-3316">Mise à jour des documents d’assistance</span><span class="sxs-lookup"><span data-stu-id="69d51-3316">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="69d51-3317">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="69d51-3317">Data Lake Analytics</span></span>

* <span data-ttu-id="69d51-3318">Modification de `[job|account] list` pour retourner des informations plus concises</span><span class="sxs-lookup"><span data-stu-id="69d51-3318">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="69d51-3319">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="69d51-3319">Data Lake Store</span></span>

* <span data-ttu-id="69d51-3320">Modification de `account list` pour retourner des informations plus concises</span><span class="sxs-lookup"><span data-stu-id="69d51-3320">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="69d51-3321">Extension</span><span class="sxs-lookup"><span data-stu-id="69d51-3321">Extension</span></span>

* <span data-ttu-id="69d51-3322">Ajout de `extension list-available` pour permettre l’affichage de la liste des extensions officielles Microsoft</span><span class="sxs-lookup"><span data-stu-id="69d51-3322">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="69d51-3323">Ajout de `--name` à `extension [add|update]` pour permettre l’installation des extensions par nom</span><span class="sxs-lookup"><span data-stu-id="69d51-3323">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="69d51-3324">IoT</span><span class="sxs-lookup"><span data-stu-id="69d51-3324">IoT</span></span>

* <span data-ttu-id="69d51-3325">Ajout de la prise en charge pour les autorités de certification (CA) et les chaînes d’approbation</span><span class="sxs-lookup"><span data-stu-id="69d51-3325">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="69d51-3326">Superviser</span><span class="sxs-lookup"><span data-stu-id="69d51-3326">Monitor</span></span>

* <span data-ttu-id="69d51-3327">Ajout des commandes `activity-log alert`</span><span class="sxs-lookup"><span data-stu-id="69d51-3327">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="69d51-3328">Réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-3328">Network</span></span>

* <span data-ttu-id="69d51-3329">Ajout de la prise en charge pour les enregistrements DNS CAA</span><span class="sxs-lookup"><span data-stu-id="69d51-3329">Added support for CAA DNS records</span></span>
* <span data-ttu-id="69d51-3330">Résolution d’un problème empêchant la mise à jour des points de terminaison avec `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="69d51-3330">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="69d51-3331">Résolution d’un problème où `vnet update --dns-servers` ne fonctionnait pas, en fonction de la façon dont avait été créé le réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="69d51-3331">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="69d51-3332">Résolution d’un problème où les noms DNS relatifs n’étaient pas importés correctement par `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="69d51-3332">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="69d51-3333">Réservations</span><span class="sxs-lookup"><span data-stu-id="69d51-3333">Reservations</span></span>

* <span data-ttu-id="69d51-3334">Version préliminaire initiale</span><span class="sxs-lookup"><span data-stu-id="69d51-3334">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="69d51-3335">Ressource</span><span class="sxs-lookup"><span data-stu-id="69d51-3335">Resource</span></span>

* <span data-ttu-id="69d51-3336">Ajout de la prise en charge pour les ID de ressource au paramètre `--resource` et pour les verrous au niveau des ressources</span><span class="sxs-lookup"><span data-stu-id="69d51-3336">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="69d51-3337">SQL</span><span class="sxs-lookup"><span data-stu-id="69d51-3337">SQL</span></span>

* <span data-ttu-id="69d51-3338">Ajout du paramètre `--ignore-missing-vnet-service-endpoint` pour `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69d51-3338">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="69d51-3339">Stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-3339">Storage</span></span>

* <span data-ttu-id="69d51-3340">Modification de `storage account create` pour utiliser la référence SKU `Standard_RAGRS` par défaut</span><span class="sxs-lookup"><span data-stu-id="69d51-3340">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="69d51-3341">Correction du bogue lors du traitement des noms d’objets blob/de fichier qui incluent des caractères non-ascii</span><span class="sxs-lookup"><span data-stu-id="69d51-3341">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="69d51-3342">Correction du bogue qui empêchait l’utilisation de `--source-uri` avec `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="69d51-3342">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="69d51-3343">Ajout de commandes pour paramétrer et supprimer plusieurs objets avec `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="69d51-3343">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="69d51-3344">Résolution du problème de l’activation des métriques avec `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="69d51-3344">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="69d51-3345">Résolution du problème des fichiers de plus de 200 Go lors de l’utilisation de `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="69d51-3345">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="69d51-3346">Résolution du problème où `--bypass` et `--default-action` étaient ignorés par `storage account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69d51-3346">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="69d51-3347">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="69d51-3347">VM</span></span>

* <span data-ttu-id="69d51-3348">Correction d’un bogue avec `vmss create` qui empêchait l’utilisation du niveau de taille `Basic`</span><span class="sxs-lookup"><span data-stu-id="69d51-3348">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="69d51-3349">Ajout d’arguments `--plan` à `[vm|vmss] create` pour les images personnalisées avec des informations de facturation</span><span class="sxs-lookup"><span data-stu-id="69d51-3349">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="69d51-3350">Ajout des commandes `vm secret `[add|remove|list]</span><span class="sxs-lookup"><span data-stu-id="69d51-3350">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="69d51-3351">`vm format-secret` renommé en `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="69d51-3351">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="69d51-3352">Ajout de l’argument `--encrypt format` à `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="69d51-3352">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="69d51-3353">24 octobre 2017</span><span class="sxs-lookup"><span data-stu-id="69d51-3353">October 24, 2017</span></span>

<span data-ttu-id="69d51-3354">Version 2.0.20</span><span class="sxs-lookup"><span data-stu-id="69d51-3354">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="69d51-3355">Core</span><span class="sxs-lookup"><span data-stu-id="69d51-3355">Core</span></span>

* <span data-ttu-id="69d51-3356">Mise à jour de `2017-03-09-profile` pour consommer l’API `MGMT_STORAGE` version `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="69d51-3356">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="69d51-3357">ACR</span><span class="sxs-lookup"><span data-stu-id="69d51-3357">ACR</span></span>

* <span data-ttu-id="69d51-3358">Mise à jour de la gestion des ressources pour pointer vers la version d’API `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="69d51-3358">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="69d51-3359">Modification de la référence SKU « Bring Your Own Storage » en Classique</span><span class="sxs-lookup"><span data-stu-id="69d51-3359">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="69d51-3360">Changement des noms des références SKU de registre en De base, Standard, et Premium</span><span class="sxs-lookup"><span data-stu-id="69d51-3360">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="69d51-3361">ACS</span><span class="sxs-lookup"><span data-stu-id="69d51-3361">ACS</span></span>

* <span data-ttu-id="69d51-3362">[PRÉVERSION] Ajout des commandes `az aks`</span><span class="sxs-lookup"><span data-stu-id="69d51-3362">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="69d51-3363">Réparation de Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="69d51-3363">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="69d51-3364">AppService</span><span class="sxs-lookup"><span data-stu-id="69d51-3364">Appservice</span></span>

* <span data-ttu-id="69d51-3365">Résolution d’une erreur où le téléchargement des journaux d’activité `webapp` était incorrect</span><span class="sxs-lookup"><span data-stu-id="69d51-3365">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="69d51-3366">Composant</span><span class="sxs-lookup"><span data-stu-id="69d51-3366">Component</span></span>

* <span data-ttu-id="69d51-3367">Ajout de clarté dans les messages visant à déconseiller de tous les programmes d’installation et des invites de confirmation</span><span class="sxs-lookup"><span data-stu-id="69d51-3367">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="69d51-3368">Superviser</span><span class="sxs-lookup"><span data-stu-id="69d51-3368">Monitor</span></span>

* <span data-ttu-id="69d51-3369">Ajout des commandes `action-group`</span><span class="sxs-lookup"><span data-stu-id="69d51-3369">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="69d51-3370">Ressource</span><span class="sxs-lookup"><span data-stu-id="69d51-3370">Resource</span></span>

* <span data-ttu-id="69d51-3371">Résolution d’une incompatibilité de la dépendance msrest dans `group export` avec les versions les plus récentes</span><span class="sxs-lookup"><span data-stu-id="69d51-3371">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="69d51-3372">Résolution de `policy assignment create` pour qu’il fonctionne avec les définitions de stratégie et les définitions d’ensemble de stratégie intégrées</span><span class="sxs-lookup"><span data-stu-id="69d51-3372">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="69d51-3373">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="69d51-3373">VM</span></span>

* <span data-ttu-id="69d51-3374">Ajout de l’argument `--accelerated-networking` à `vmss create`</span><span class="sxs-lookup"><span data-stu-id="69d51-3374">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="69d51-3375">9 octobre 2017</span><span class="sxs-lookup"><span data-stu-id="69d51-3375">October 9, 2017</span></span>

<span data-ttu-id="69d51-3376">Version 2.0.19</span><span class="sxs-lookup"><span data-stu-id="69d51-3376">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="69d51-3377">Core</span><span class="sxs-lookup"><span data-stu-id="69d51-3377">Core</span></span>

* <span data-ttu-id="69d51-3378">Ajout de la gestion des URL d’autorisation AD FS avec une barre oblique à Azure Stack</span><span class="sxs-lookup"><span data-stu-id="69d51-3378">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="69d51-3379">AppService</span><span class="sxs-lookup"><span data-stu-id="69d51-3379">Appservice</span></span>

* <span data-ttu-id="69d51-3380">Ajout de la mise à jour générique avec la nouvelle commande `webapp update`</span><span class="sxs-lookup"><span data-stu-id="69d51-3380">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="69d51-3381">Batch</span><span class="sxs-lookup"><span data-stu-id="69d51-3381">Batch</span></span>

* <span data-ttu-id="69d51-3382">Mis à jour du kit de développement logiciel (SDK) à la version 4.0.0</span><span class="sxs-lookup"><span data-stu-id="69d51-3382">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="69d51-3383">Mise à jour de l’option `--image` de VirtualMachineConfiguration pour prendre en charge les références d’image ARM en plus de publish:offre:sku:version</span><span class="sxs-lookup"><span data-stu-id="69d51-3383">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="69d51-3384">Ajout de la prise en charge du nouveau modèle d’extension CLI pour les commandes d’extension Batch</span><span class="sxs-lookup"><span data-stu-id="69d51-3384">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="69d51-3385">Suppression de la prise en charge Batch des modèles de composants</span><span class="sxs-lookup"><span data-stu-id="69d51-3385">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="69d51-3386">Batchai</span><span class="sxs-lookup"><span data-stu-id="69d51-3386">Batchai</span></span>

* <span data-ttu-id="69d51-3387">Version initiale du module Batch AI</span><span class="sxs-lookup"><span data-stu-id="69d51-3387">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="69d51-3388">KeyVault</span><span class="sxs-lookup"><span data-stu-id="69d51-3388">Keyvault</span></span>

* <span data-ttu-id="69d51-3389">Résolution du problème d’authentification Key Vault lors de l’utilisation d’AD FS sur Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="69d51-3389">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="69d51-3390">(#4448)</span><span class="sxs-lookup"><span data-stu-id="69d51-3390">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="69d51-3391">Réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-3391">Network</span></span>

* <span data-ttu-id="69d51-3392">La modification de l’argument `--server` de `application-gateway address-pool create` devient facultative, permettant les pools d’adresses vides</span><span class="sxs-lookup"><span data-stu-id="69d51-3392">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="69d51-3393">Mise à jour de `traffic-manager` pour prendre en charge les fonctionnalités les plus récentes</span><span class="sxs-lookup"><span data-stu-id="69d51-3393">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="69d51-3394">Ressource</span><span class="sxs-lookup"><span data-stu-id="69d51-3394">Resource</span></span>

* <span data-ttu-id="69d51-3395">Ajout de la prise en charge des options `--resource-group/-g` pour le nom du groupe de ressources dans `group`</span><span class="sxs-lookup"><span data-stu-id="69d51-3395">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="69d51-3396">Ajout des commandes à `account lock` pour travailler avec des verrous au niveau de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="69d51-3396">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="69d51-3397">Ajout des commandes à `group lock` pour travailler avec des verrous au niveau du groupe</span><span class="sxs-lookup"><span data-stu-id="69d51-3397">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="69d51-3398">Ajout des commandes à `resource lock` pour travailler avec des verrous au niveau des ressources</span><span class="sxs-lookup"><span data-stu-id="69d51-3398">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="69d51-3399">SQL</span><span class="sxs-lookup"><span data-stu-id="69d51-3399">Sql</span></span>

* <span data-ttu-id="69d51-3400">Ajout de la prise en charge pour le Chiffrement transparent des données (TDE) SQL et le chiffrement transparent des données avec Bring Your Own Key</span><span class="sxs-lookup"><span data-stu-id="69d51-3400">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="69d51-3401">Ajout de la commande `db list-deleted` et du paramètre `db restore --deleted-time`, ce qui offre la possibilité de rechercher et de restaurer les bases de données supprimées</span><span class="sxs-lookup"><span data-stu-id="69d51-3401">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="69d51-3402">Ajout de `db op list` et `db op cancel`, ce qui offre la capacité de répertorier et d’annuler des opérations en cours sur la base de données</span><span class="sxs-lookup"><span data-stu-id="69d51-3402">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="69d51-3403">Stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-3403">Storage</span></span>

* <span data-ttu-id="69d51-3404">Ajout de la prise en charge d’instantané de partage de fichiers</span><span class="sxs-lookup"><span data-stu-id="69d51-3404">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="69d51-3405">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="69d51-3405">Vm</span></span>

* <span data-ttu-id="69d51-3406">Correction d’un bogue dans `vm show` où l’utilisation de `-d` a provoqué un incident dans les adresses IP privées manquantes</span><span class="sxs-lookup"><span data-stu-id="69d51-3406">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="69d51-3407">[VERSION PRÉLIMINAIRE] Ajout de la prise en charge de la mise à niveau propagée pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="69d51-3407">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="69d51-3408">Ajout de la prise en charge de la mise à jour des paramètres de chiffrement avec `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="69d51-3408">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="69d51-3409">Ajout du paramètre `--os-disk-size-gb` pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="69d51-3409">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="69d51-3410">Ajout du paramètre `--license-type` de Windows pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="69d51-3410">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="69d51-3411">22 septembre 2017</span><span class="sxs-lookup"><span data-stu-id="69d51-3411">September 22, 2017</span></span>

<span data-ttu-id="69d51-3412">Version 2.0.18</span><span class="sxs-lookup"><span data-stu-id="69d51-3412">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="69d51-3413">Ressource</span><span class="sxs-lookup"><span data-stu-id="69d51-3413">Resource</span></span>

* <span data-ttu-id="69d51-3414">Ajout de la prise en charge de l’affichage des définitions de stratégie intégrée</span><span class="sxs-lookup"><span data-stu-id="69d51-3414">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="69d51-3415">Ajout de la prise en charge du paramètre de mode pour la création de définitions de stratégie</span><span class="sxs-lookup"><span data-stu-id="69d51-3415">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="69d51-3416">Ajout de la prise en charge des définitions d’interface utilisateur et des modèles pour `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="69d51-3416">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="69d51-3417">[CHANGEMENT CASSANT] Modification du type de ressource `managedapp` de `appliances` en `applications` et de `applianceDefinitions` en `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="69d51-3417">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="69d51-3418">Réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-3418">Network</span></span>

* <span data-ttu-id="69d51-3419">Ajout de la prise en charge de la zone de disponibilité aux sous-commandes `network lb` et `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="69d51-3419">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="69d51-3420">Ajout de la prise en charge du peering Microsoft IPv6 pour `express-route`</span><span class="sxs-lookup"><span data-stu-id="69d51-3420">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="69d51-3421">Ajout des commandes du groupe de sécurité d’application `asg`</span><span class="sxs-lookup"><span data-stu-id="69d51-3421">Added `asg` application security group commands</span></span>
* <span data-ttu-id="69d51-3422">Ajout de l’argument `--application-security-groups` à `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="69d51-3422">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="69d51-3423">Ajout des arguments `--source-asgs` et `--destination-asgs` à `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69d51-3423">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="69d51-3424">Ajout des arguments `--ddos-protection` et `--vm-protection` à `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69d51-3424">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="69d51-3425">Ajout des commandes `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="69d51-3425">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="69d51-3426">Stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-3426">Storage</span></span>

* <span data-ttu-id="69d51-3427">Résolution d’un problème qui pouvait causer l’échec des commandes `storage account network-rule` après la mise à jour du Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="69d51-3427">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="69d51-3428">Événement</span><span class="sxs-lookup"><span data-stu-id="69d51-3428">Eventgrid</span></span>

* <span data-ttu-id="69d51-3429">Mise à jour du Kit de développement logiciel (SDK) Python Azure Event Grid afin d’utiliser une version plus récente de l’API « 2017-09-15-preview »</span><span class="sxs-lookup"><span data-stu-id="69d51-3429">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="69d51-3430">SQL</span><span class="sxs-lookup"><span data-stu-id="69d51-3430">SQL</span></span>

* <span data-ttu-id="69d51-3431">La modification de l’`sql server list`argument`--resource-group` devient facultative.</span><span class="sxs-lookup"><span data-stu-id="69d51-3431">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="69d51-3432">En l’absence de précisions, tous les serveurs SQL dans l’abonnement seront retournés</span><span class="sxs-lookup"><span data-stu-id="69d51-3432">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="69d51-3433">Ajout du paramètre `--no-wait` à `db [create|copy|restore|update|replica create|create|update]` et `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69d51-3433">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="69d51-3434">KeyVault</span><span class="sxs-lookup"><span data-stu-id="69d51-3434">Keyvault</span></span>

* <span data-ttu-id="69d51-3435">Ajout de la prise en charge des commandes Keyvault derrière un proxy</span><span class="sxs-lookup"><span data-stu-id="69d51-3435">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="69d51-3436">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="69d51-3436">VM</span></span>

* <span data-ttu-id="69d51-3437">Ajout de la prise en charge de zone de disponibilité pour `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="69d51-3437">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="69d51-3438">Résolution d’un problème à cause duquel l’utilisation de `--app-gateway ID` avec `vmss create` entraînait un échec</span><span class="sxs-lookup"><span data-stu-id="69d51-3438">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="69d51-3439">Ajout de l’argument `--asgs` à `vm create`</span><span class="sxs-lookup"><span data-stu-id="69d51-3439">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="69d51-3440">Ajout de la prise en charge des commandes en cours d’exécution sur des machines virtuelles avec `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="69d51-3440">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="69d51-3441">[PRÉVERSION] Ajout de la prise en charge du chiffrement de disque VMSS avec `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="69d51-3441">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="69d51-3442">Ajout de la prise en charge de la réalisation de la maintenance sur des machines virtuelles avec `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="69d51-3442">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="69d51-3443">ACS</span><span class="sxs-lookup"><span data-stu-id="69d51-3443">ACS</span></span>

* <span data-ttu-id="69d51-3444">[PRÉVERSION] Ajout de l’argument `--orchestrator-release` à `acs create` pour les régions ACS en préversion</span><span class="sxs-lookup"><span data-stu-id="69d51-3444">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="69d51-3445">AppService</span><span class="sxs-lookup"><span data-stu-id="69d51-3445">Appservice</span></span>

* <span data-ttu-id="69d51-3446">Ajout de la capacité à mettre à jour et à afficher les paramètres d’authentification avec `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="69d51-3446">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="69d51-3447">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="69d51-3447">Backup</span></span>

* <span data-ttu-id="69d51-3448">Préversion</span><span class="sxs-lookup"><span data-stu-id="69d51-3448">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="69d51-3449">11 septembre 2017</span><span class="sxs-lookup"><span data-stu-id="69d51-3449">September 11, 2017</span></span>

<span data-ttu-id="69d51-3450">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="69d51-3450">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="69d51-3451">Core</span><span class="sxs-lookup"><span data-stu-id="69d51-3451">Core</span></span>

* <span data-ttu-id="69d51-3452">Module de commande activé pour définir son propre ID de corrélation dans la télémétrie</span><span class="sxs-lookup"><span data-stu-id="69d51-3452">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="69d51-3453">Résolution du problème de vidage JSON lorsque la télémétrie est définie en mode diagnostics</span><span class="sxs-lookup"><span data-stu-id="69d51-3453">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="69d51-3454">Acs</span><span class="sxs-lookup"><span data-stu-id="69d51-3454">Acs</span></span>

* <span data-ttu-id="69d51-3455">Ajout de la commande `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="69d51-3455">Added `acs list-locations` command</span></span>
* <span data-ttu-id="69d51-3456">Faire en sorte que `ssh-key-file` soit fourni avec la valeur par défaut attendu</span><span class="sxs-lookup"><span data-stu-id="69d51-3456">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="69d51-3457">AppService</span><span class="sxs-lookup"><span data-stu-id="69d51-3457">Appservice</span></span>

* <span data-ttu-id="69d51-3458">Ajout de la possibilité de créer une application web dans un groupe de ressources autre que celui du plan de service actif</span><span class="sxs-lookup"><span data-stu-id="69d51-3458">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="69d51-3459">CDN</span><span class="sxs-lookup"><span data-stu-id="69d51-3459">CDN</span></span>

* <span data-ttu-id="69d51-3460">Correction du bogue « CustomDomain n’est pas itérable » pour `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="69d51-3460">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="69d51-3461">Extension</span><span class="sxs-lookup"><span data-stu-id="69d51-3461">Extension</span></span>

* <span data-ttu-id="69d51-3462">Version initiale</span><span class="sxs-lookup"><span data-stu-id="69d51-3462">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="69d51-3463">KeyVault</span><span class="sxs-lookup"><span data-stu-id="69d51-3463">Keyvault</span></span>

* <span data-ttu-id="69d51-3464">Résolution du problème où les autorisations étaient sensibles à la casse pour `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="69d51-3464">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="69d51-3465">Réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-3465">Network</span></span>

* <span data-ttu-id="69d51-3466">`vnet list-private-access-services` renommé en `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="69d51-3466">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="69d51-3467">Argument `--private-access-services` renommé en `--service-endpoints` pour`vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="69d51-3467">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="69d51-3468">Ajout de la prise en charge de plusieurs plages IP et de ports à `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="69d51-3468">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="69d51-3469">Ajout de la prise en charge de la référence (SKU) pour `lb create`</span><span class="sxs-lookup"><span data-stu-id="69d51-3469">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="69d51-3470">Ajout de la prise en charge de la référence (SKU) pour `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="69d51-3470">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="69d51-3471">Ressource</span><span class="sxs-lookup"><span data-stu-id="69d51-3471">Resource</span></span>

* <span data-ttu-id="69d51-3472">Autoriser le passages dans les définitions de paramètres de stratégie de ressource dans `policy definition create`, et`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="69d51-3472">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="69d51-3473">Autoriser le passage dans les valeurs de paramètres pour `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="69d51-3473">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="69d51-3474">Autoriser le passage de JSON ou d’un fichier pour tous les paramètres</span><span class="sxs-lookup"><span data-stu-id="69d51-3474">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="69d51-3475">Incrémentation de la version de l’API</span><span class="sxs-lookup"><span data-stu-id="69d51-3475">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="69d51-3476">SQL</span><span class="sxs-lookup"><span data-stu-id="69d51-3476">SQL</span></span>

* <span data-ttu-id="69d51-3477">Ajout des commandes `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="69d51-3477">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="69d51-3478">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="69d51-3478">VM</span></span>

* <span data-ttu-id="69d51-3479">Résolu : n’affecte aucun accès tant que `--scope` n’est pas indiqué</span><span class="sxs-lookup"><span data-stu-id="69d51-3479">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="69d51-3480">Résolu : utilisation de la même dénomination d’extension que celle du portail</span><span class="sxs-lookup"><span data-stu-id="69d51-3480">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="69d51-3481">Suppression de `subscription` de la sortie `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="69d51-3481">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="69d51-3482">Résolu : la référence SKU de stockage `[vm|vmss] create` n’est pas appliquée sur les disques de données avec une image</span><span class="sxs-lookup"><span data-stu-id="69d51-3482">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="69d51-3483">Résolu : `vm format-secret --secrets` n’accepte pas d’ID séparés par un saut de ligne</span><span class="sxs-lookup"><span data-stu-id="69d51-3483">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="69d51-3484">31 août 2017</span><span class="sxs-lookup"><span data-stu-id="69d51-3484">August 31, 2017</span></span>

<span data-ttu-id="69d51-3485">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="69d51-3485">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="69d51-3486">KeyVault</span><span class="sxs-lookup"><span data-stu-id="69d51-3486">Keyvault</span></span>

* <span data-ttu-id="69d51-3487">Correction d’un bogue à cause duquel vous tentez de résoudre automatiquement l’encodage secret avec `secret download`</span><span class="sxs-lookup"><span data-stu-id="69d51-3487">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="69d51-3488">Sf</span><span class="sxs-lookup"><span data-stu-id="69d51-3488">Sf</span></span>

* <span data-ttu-id="69d51-3489">Déconseiller toutes les commandes en faveur de Service Fabric CLI (sfctl)</span><span class="sxs-lookup"><span data-stu-id="69d51-3489">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="69d51-3490">Stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-3490">Storage</span></span>

* <span data-ttu-id="69d51-3491">Résolution du problème dans lequel la création de comptes de stockage dans les régions ne prenant pas en charge la fonctionnalité NetworkACLs était impossible</span><span class="sxs-lookup"><span data-stu-id="69d51-3491">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="69d51-3492">Déterminer le type de contenu et l’encodage du contenu lors du chargement d’objets blob et de fichiers si aucun type de contenu et d’encodage n’est spécifié.</span><span class="sxs-lookup"><span data-stu-id="69d51-3492">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="69d51-3493">28 août 2017</span><span class="sxs-lookup"><span data-stu-id="69d51-3493">August 28, 2017</span></span>

<span data-ttu-id="69d51-3494">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="69d51-3494">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="69d51-3495">Interface de ligne de commande</span><span class="sxs-lookup"><span data-stu-id="69d51-3495">CLI</span></span>

* <span data-ttu-id="69d51-3496">Ajout d’une remarque juridique pour `--version`</span><span class="sxs-lookup"><span data-stu-id="69d51-3496">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="69d51-3497">ACS</span><span class="sxs-lookup"><span data-stu-id="69d51-3497">ACS</span></span>

* <span data-ttu-id="69d51-3498">Correction des régions d’aperçu</span><span class="sxs-lookup"><span data-stu-id="69d51-3498">Corrected preview regions</span></span>
* <span data-ttu-id="69d51-3499">Mise en forme par défaut `dns_name_prefix` correctement</span><span class="sxs-lookup"><span data-stu-id="69d51-3499">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="69d51-3500">Optimisation de la sortie de commande des services ACS</span><span class="sxs-lookup"><span data-stu-id="69d51-3500">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="69d51-3501">AppService</span><span class="sxs-lookup"><span data-stu-id="69d51-3501">Appservice</span></span>

* <span data-ttu-id="69d51-3502">[CHANGEMENT CASSANT] Fixation des incohérences dans la sortie de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="69d51-3502">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="69d51-3503">Ajout d’un nouvel alias de `-i` pour `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="69d51-3503">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="69d51-3504">Exposé `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="69d51-3504">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="69d51-3505">Exposition de nouveaux arguments à partir de `az webapp delete` pour conserver le plan de service d'application, les métriques ou l’inscription DNS</span><span class="sxs-lookup"><span data-stu-id="69d51-3505">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="69d51-3506">Résolu : détecter les paramètres d’emplacement correctement</span><span class="sxs-lookup"><span data-stu-id="69d51-3506">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="69d51-3507">IoT</span><span class="sxs-lookup"><span data-stu-id="69d51-3507">IoT</span></span>

* <span data-ttu-id="69d51-3508">Résolution de #3934 : la création de la stratégie n’efface plus les stratégies existantes</span><span class="sxs-lookup"><span data-stu-id="69d51-3508">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="69d51-3509">Réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-3509">Network</span></span>

* <span data-ttu-id="69d51-3510">[CHANGEMENT CASSANT] Renommage de `vnet list-private-access-services` en `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="69d51-3510">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="69d51-3511">[CHANGEMENT CASSANT] Renommage de l’option `--private-access-services` en `--service-endpoints` pour `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69d51-3511">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="69d51-3512">Ajout de la prise en charge de plusieurs IP et de plusieurs pages de port pour `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="69d51-3512">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="69d51-3513">Ajout de la prise en charge de la référence (SKU) pour `lb create`</span><span class="sxs-lookup"><span data-stu-id="69d51-3513">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="69d51-3514">Ajout de la prise en charge de la référence (SKU) pour `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="69d51-3514">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="69d51-3515">Profil</span><span class="sxs-lookup"><span data-stu-id="69d51-3515">Profile</span></span>

* <span data-ttu-id="69d51-3516">exposés `--msi` et `--msi-port` pour vous connecter à l’aide d’une identité de machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="69d51-3516">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="69d51-3517">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="69d51-3517">Service Fabric</span></span>

* <span data-ttu-id="69d51-3518">Préversion</span><span class="sxs-lookup"><span data-stu-id="69d51-3518">Preview release</span></span>
* <span data-ttu-id="69d51-3519">Règles d’utilisateur du Registre/de mot de passe simplifiées pour la commande</span><span class="sxs-lookup"><span data-stu-id="69d51-3519">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="69d51-3520">Invite de mot de passe fixe pour l’utilisateur, même après le passage de paramètre</span><span class="sxs-lookup"><span data-stu-id="69d51-3520">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="69d51-3521">Ajout de la prise en charge de vide `registry_cred`</span><span class="sxs-lookup"><span data-stu-id="69d51-3521">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="69d51-3522">Stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-3522">Storage</span></span>

* <span data-ttu-id="69d51-3523">Paramétrage du niveau blob activé</span><span class="sxs-lookup"><span data-stu-id="69d51-3523">Enabled setting blob tier</span></span>
* <span data-ttu-id="69d51-3524">Ajout des arguments `--bypass` et `--default-action` à `storage account [create|update]` pour la prise en charge du tunneling de service</span><span class="sxs-lookup"><span data-stu-id="69d51-3524">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="69d51-3525">Ajout de commandes permettant d’ajouter des règles de réseau virtuel et des règles basées sur IP à `storage account network-rule`</span><span class="sxs-lookup"><span data-stu-id="69d51-3525">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="69d51-3526">Activation du chiffrement du service par la clé gérée du client</span><span class="sxs-lookup"><span data-stu-id="69d51-3526">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="69d51-3527">[CHANGEMENT CASSANT] Renommage de l’option `--encryption` en `--encryption-services` pour la commande `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="69d51-3527">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="69d51-3528">Problème résolu #4220 : `az storage account update encryption` - incompatibilité de syntaxe</span><span class="sxs-lookup"><span data-stu-id="69d51-3528">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="69d51-3529">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="69d51-3529">VM</span></span>

* <span data-ttu-id="69d51-3530">Correction d’un problème qui entraînait l’affichage d’informations supplémentaires erronées pour `vmss get-instance-view` lors de l’utilisation `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="69d51-3530">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="69d51-3531">Ajout de la prise en charge de `--lb-sku` pour `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="69d51-3531">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="69d51-3532">Suppression des noms humains de la liste rouge du nom de l’administrateur pour `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="69d51-3532">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="69d51-3533">Correction d’un problème qui entraînait `[vm|vmss] create` la levée d’une erreur si la commande ne parvenait pas à extraire des informations de plan à partir d’une image</span><span class="sxs-lookup"><span data-stu-id="69d51-3533">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="69d51-3534">Correction d’un incident qui se produisait lors de la création d’un groupe identique VMMD avec un équilibrage de charge (LB) interne</span><span class="sxs-lookup"><span data-stu-id="69d51-3534">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="69d51-3535">Correction d’un problème qui empêchait `--no-wait` le fonctionnement d’un argument avec `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="69d51-3535">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="69d51-3536">15 août 2017</span><span class="sxs-lookup"><span data-stu-id="69d51-3536">August 15, 2017</span></span>

<span data-ttu-id="69d51-3537">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="69d51-3537">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="69d51-3538">ACS</span><span class="sxs-lookup"><span data-stu-id="69d51-3538">ACS</span></span>

* <span data-ttu-id="69d51-3539">Correction du numéro de port sshMaster0 pour kubernetes</span><span class="sxs-lookup"><span data-stu-id="69d51-3539">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="69d51-3540">AppService</span><span class="sxs-lookup"><span data-stu-id="69d51-3540">Appservice</span></span>

* <span data-ttu-id="69d51-3541">Correction d’une exception qui se produisait lors de la création d’une nouvelle application web Linux basée sur git</span><span class="sxs-lookup"><span data-stu-id="69d51-3541">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="69d51-3542">Event Grid</span><span class="sxs-lookup"><span data-stu-id="69d51-3542">Event Grid</span></span>

* <span data-ttu-id="69d51-3543">Ajout de dépendances du kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="69d51-3543">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="69d51-3544">11 août 2017</span><span class="sxs-lookup"><span data-stu-id="69d51-3544">August 11, 2017</span></span>

<span data-ttu-id="69d51-3545">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="69d51-3545">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="69d51-3546">ACS</span><span class="sxs-lookup"><span data-stu-id="69d51-3546">ACS</span></span>

* <span data-ttu-id="69d51-3547">Ajout de nouvelles régions d’aperçu</span><span class="sxs-lookup"><span data-stu-id="69d51-3547">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="69d51-3548">Batch</span><span class="sxs-lookup"><span data-stu-id="69d51-3548">Batch</span></span>

* <span data-ttu-id="69d51-3549">Mise à jour vers Kit de développement logiciel (DSK) de lot 3.1.0 et Kit de développement logiciel (SDK) de gestion de lot 4.1.0</span><span class="sxs-lookup"><span data-stu-id="69d51-3549">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="69d51-3550">Ajout d'une nouvelle commande affichant le nombre de tâches d’un travail</span><span class="sxs-lookup"><span data-stu-id="69d51-3550">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="69d51-3551">Correction du bogue dans le traitement de l’URL de la signature d'accès partagé du fichier de ressources</span><span class="sxs-lookup"><span data-stu-id="69d51-3551">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="69d51-3552">Point de terminaison de compte Batch prend désormais en charge le préfixe « https:// » facultatif</span><span class="sxs-lookup"><span data-stu-id="69d51-3552">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="69d51-3553">Prise en charge de l’ajout des listes de plus de 100 tâches à un travail</span><span class="sxs-lookup"><span data-stu-id="69d51-3553">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="69d51-3554">Ajout de l’enregistrement de débogage pour le chargement du module de commande Extensions</span><span class="sxs-lookup"><span data-stu-id="69d51-3554">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="69d51-3555">Composant</span><span class="sxs-lookup"><span data-stu-id="69d51-3555">Component</span></span>

* <span data-ttu-id="69d51-3556">Ajout d’un avertissement de désapprobation aux commandes « az component »</span><span class="sxs-lookup"><span data-stu-id="69d51-3556">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="69d51-3557">Conteneur</span><span class="sxs-lookup"><span data-stu-id="69d51-3557">Container</span></span>

* <span data-ttu-id="69d51-3558">`create`: correction d’un problème qui empêchait l’utilisation du signe égal à l’intérieur d’une variable d’environnement</span><span class="sxs-lookup"><span data-stu-id="69d51-3558">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="69d51-3559">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="69d51-3559">Data Lake Store</span></span>

* <span data-ttu-id="69d51-3560">Contrôle de progression activé</span><span class="sxs-lookup"><span data-stu-id="69d51-3560">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="69d51-3561">Event Grid</span><span class="sxs-lookup"><span data-stu-id="69d51-3561">Event Grid</span></span>

* <span data-ttu-id="69d51-3562">Version initiale</span><span class="sxs-lookup"><span data-stu-id="69d51-3562">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="69d51-3563">Réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-3563">Network</span></span>

* <span data-ttu-id="69d51-3564">`lb`: correction d’un problème qui empêchait certains noms de ressources enfant d’être résolus correctement lorsqu’ils étaient omis</span><span class="sxs-lookup"><span data-stu-id="69d51-3564">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="69d51-3565">`application-gateway {subresource} delete`: correction d’un problème en raison duquel `--no-wait` n’était pas honorée</span><span class="sxs-lookup"><span data-stu-id="69d51-3565">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="69d51-3566">`application-gateway http-settings update`: correction d’un problème qui empêchait la désactivation de `--connection-draining-timeout`</span><span class="sxs-lookup"><span data-stu-id="69d51-3566">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="69d51-3567">Correction de erreur argument du mot-clé inattendu `sa_data_size_kilobyes` avec`az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="69d51-3567">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="69d51-3568">Profil</span><span class="sxs-lookup"><span data-stu-id="69d51-3568">Profile</span></span>

* <span data-ttu-id="69d51-3569">`account list`: ajout de `--refresh` pour synchroniser les derniers abonnements à partir du serveur</span><span class="sxs-lookup"><span data-stu-id="69d51-3569">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="69d51-3570">Stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-3570">Storage</span></span>

* <span data-ttu-id="69d51-3571">Activer le compte de stockage de mise à jour avec l’identité attribuée par le système</span><span class="sxs-lookup"><span data-stu-id="69d51-3571">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="69d51-3572">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="69d51-3572">VM</span></span>

* <span data-ttu-id="69d51-3573">`availability-set`: nombre de domaines d’erreur exposés lors de la conversion</span><span class="sxs-lookup"><span data-stu-id="69d51-3573">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="69d51-3574">Commande `list-skus` exposée</span><span class="sxs-lookup"><span data-stu-id="69d51-3574">Exposed `list-skus` command</span></span>
* <span data-ttu-id="69d51-3575">Prise en charge pour affecter l’identité avec ou sans création d’attributions de rôle</span><span class="sxs-lookup"><span data-stu-id="69d51-3575">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="69d51-3576">Appliquer la référence (SKU) de stockage lors de l’attachement de disques de données</span><span class="sxs-lookup"><span data-stu-id="69d51-3576">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="69d51-3577">Suppression du nom du disque du système d’exploitation par défaut et de la référence (SKU) de stockage lors de l’utilisation des disques managés</span><span class="sxs-lookup"><span data-stu-id="69d51-3577">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="69d51-3578">28 juillet 2017</span><span class="sxs-lookup"><span data-stu-id="69d51-3578">July 28, 2017</span></span>

<span data-ttu-id="69d51-3579">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="69d51-3579">Version 2.0.12</span></span>

* <span data-ttu-id="69d51-3580">Ajout de commandes de conteneur</span><span class="sxs-lookup"><span data-stu-id="69d51-3580">Added container commands</span></span>
* <span data-ttu-id="69d51-3581">Ajout de modules de facturation et de consommation</span><span class="sxs-lookup"><span data-stu-id="69d51-3581">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="69d51-3582">Core</span><span class="sxs-lookup"><span data-stu-id="69d51-3582">Core</span></span>

* <span data-ttu-id="69d51-3583">Informations d’authentification du Kit de développement logiciel (SDK) de sortie pour les principaux de service avec des certificats</span><span class="sxs-lookup"><span data-stu-id="69d51-3583">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="69d51-3584">Correction des exceptions de progression de déploiement</span><span class="sxs-lookup"><span data-stu-id="69d51-3584">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="69d51-3585">Utiliser le point de terminaison ARM à partir du cloud actuel pour créer le client de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="69d51-3585">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="69d51-3586">Amélioration de la gestion simultanée de fichiers clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="69d51-3586">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="69d51-3587">Actualiser l’ID de la demande client pour chaque exécution de la commande</span><span class="sxs-lookup"><span data-stu-id="69d51-3587">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="69d51-3588">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel ( SDK) (#3635)</span><span class="sxs-lookup"><span data-stu-id="69d51-3588">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="69d51-3589">Rapports de progression pour les déploiements de modèle (#3510)</span><span class="sxs-lookup"><span data-stu-id="69d51-3589">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="69d51-3590">Ajout de la prise en charge des champs de sortie de la table de prélèvement via la requête jmespath (#3581)</span><span class="sxs-lookup"><span data-stu-id="69d51-3590">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="69d51-3591">Amélioration de la désactivation des arguments d’analyse et de l’historique Ajout avec des mouvements (#3434)</span><span class="sxs-lookup"><span data-stu-id="69d51-3591">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="69d51-3592">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="69d51-3592">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="69d51-3593">Déplacer tous les fichiers d’enregistrement existant vers le dernier dossier</span><span class="sxs-lookup"><span data-stu-id="69d51-3593">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="69d51-3594">Correction de l’idempotence pour VM/VMSS create (#3586)</span><span class="sxs-lookup"><span data-stu-id="69d51-3594">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="69d51-3595">Les chemins d’accès de la commande ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="69d51-3595">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="69d51-3596">Certains paramètres de type booléen ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="69d51-3596">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="69d51-3597">Prise en charge de la connexion à ADFS sur le serveur local de manière identique à Azure Stack</span><span class="sxs-lookup"><span data-stu-id="69d51-3597">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="69d51-3598">Correction des écritures simultanées dans clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="69d51-3598">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="69d51-3599">ACR</span><span class="sxs-lookup"><span data-stu-id="69d51-3599">ACR</span></span>

* <span data-ttu-id="69d51-3600">Ajout de la commande `show-usage` pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="69d51-3600">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="69d51-3601">Prise en charge de la mise à jour de la référence (SKU) pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="69d51-3601">Support SKU update for managed registries</span></span>
* <span data-ttu-id="69d51-3602">Ajout de registres gérés avec la référence (SKU) gérée</span><span class="sxs-lookup"><span data-stu-id="69d51-3602">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="69d51-3603">Ajout de webhooks pour les registres gérés avec le module de commande acr webhook</span><span class="sxs-lookup"><span data-stu-id="69d51-3603">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="69d51-3604">Ajout de l’authentification AAD avec la commande de connexion acr</span><span class="sxs-lookup"><span data-stu-id="69d51-3604">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="69d51-3605">Ajout de la commande de suppression pour les référentiels docker, les manifestes et les balises</span><span class="sxs-lookup"><span data-stu-id="69d51-3605">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="69d51-3606">ACS</span><span class="sxs-lookup"><span data-stu-id="69d51-3606">ACS</span></span>

* <span data-ttu-id="69d51-3607">Prise en charge des API version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="69d51-3607">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="69d51-3608">AppService</span><span class="sxs-lookup"><span data-stu-id="69d51-3608">Appservice</span></span>

* <span data-ttu-id="69d51-3609">Correction d’un bogue à cause duquel l’énumération d’une application Linux ne retournait absolument rien</span><span class="sxs-lookup"><span data-stu-id="69d51-3609">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="69d51-3610">Prise en charge de la récupération de références depuis ACR</span><span class="sxs-lookup"><span data-stu-id="69d51-3610">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="69d51-3611">Supprimer toutes les commandes sous `appservice web`</span><span class="sxs-lookup"><span data-stu-id="69d51-3611">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="69d51-3612">Masquer les mots de passe du registre docker de la commande de sortie (#3656)</span><span class="sxs-lookup"><span data-stu-id="69d51-3612">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="69d51-3613">Vérifier que le navigateur par défaut est utilisé sur macOs sans erreurs (#3623)</span><span class="sxs-lookup"><span data-stu-id="69d51-3613">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="69d51-3614">Améliorer l’aide de `webapp log tail` et `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="69d51-3614">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="69d51-3615">Commandes `traffic-routing` exposées pour configurer le routage statique (#3566)</span><span class="sxs-lookup"><span data-stu-id="69d51-3615">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="69d51-3616">Ajout de correctifs de fiabilité pour la configuration du contrôle de code source (#3245)</span><span class="sxs-lookup"><span data-stu-id="69d51-3616">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="69d51-3617">Suppression d’un argument non pris en charge `--node-version` de `webapp config update` pour les applications Web de Windows.</span><span class="sxs-lookup"><span data-stu-id="69d51-3617">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="69d51-3618">Utilisez à la place `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="69d51-3618">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="69d51-3619">Batch</span><span class="sxs-lookup"><span data-stu-id="69d51-3619">Batch</span></span>

* <span data-ttu-id="69d51-3620">Mise à jour vers kit de développement logiciel (SDK) de lot 3.0.0 avec prise en charge pour les machines virtuelles de faible priorité dans des pools</span><span class="sxs-lookup"><span data-stu-id="69d51-3620">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="69d51-3621">Renommage `pool create` option `--target-dedicated` en `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="69d51-3621">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="69d51-3622">Ajout des options `pool create`, `--target-low-priority-nodes` et `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="69d51-3622">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="69d51-3623">CDN</span><span class="sxs-lookup"><span data-stu-id="69d51-3623">CDN</span></span>

* <span data-ttu-id="69d51-3624">Fourniture d’un meilleur message d’erreur pour `cdn endpoint list` quand le profil spécifié par `--profile-name` n’existe pas</span><span class="sxs-lookup"><span data-stu-id="69d51-3624">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="69d51-3625">Cloud</span><span class="sxs-lookup"><span data-stu-id="69d51-3625">Cloud</span></span>

* <span data-ttu-id="69d51-3626">Modification de la version de l’API du point de terminaison de métadonnées du cloud au format AAAA-MM-JJ</span><span class="sxs-lookup"><span data-stu-id="69d51-3626">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="69d51-3627">Le point de terminaison de la galerie n’est pas nécessaire</span><span class="sxs-lookup"><span data-stu-id="69d51-3627">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="69d51-3628">Prise en charge de l’inscription du cloud, avec le point de terminaison ARM resource manager</span><span class="sxs-lookup"><span data-stu-id="69d51-3628">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="69d51-3629">Ajout d’une option pour `cloud set` permettant de choisir le profil lors de la sélection du cloud actuel</span><span class="sxs-lookup"><span data-stu-id="69d51-3629">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="69d51-3630">Exposé `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="69d51-3630">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="69d51-3631">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="69d51-3631">CosmosDB</span></span>

* <span data-ttu-id="69d51-3632">Correction relative à la permission de la création de collection avec une clé de partition personnalisée</span><span class="sxs-lookup"><span data-stu-id="69d51-3632">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="69d51-3633">Ajout de la prise en charge de la durée de vie par défaut de la collection</span><span class="sxs-lookup"><span data-stu-id="69d51-3633">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="69d51-3634">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="69d51-3634">Data Lake Analytics</span></span>

* <span data-ttu-id="69d51-3635">Ajout de commandes pour la gestion de la stratégie de calcul sous le titre `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="69d51-3635">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="69d51-3636">Ajout de `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="69d51-3636">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="69d51-3637">Ajout de `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="69d51-3637">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="69d51-3638">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="69d51-3638">Data Lake Store</span></span>

* <span data-ttu-id="69d51-3639">Ajout de la prise en charge pour la rotation de coffre de clés gérés par l’utilisateur dans `dls account update`</span><span class="sxs-lookup"><span data-stu-id="69d51-3639">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="69d51-3640">Mise à jour de la version du kit de développement logiciel (SDK) du système de fichiers Data Lake Store sous-jacente, réglant un problème de performance</span><span class="sxs-lookup"><span data-stu-id="69d51-3640">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="69d51-3641">Ajout de la commande `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="69d51-3641">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="69d51-3642">Cette commande tente d’activer un utilisateur de coffre de clés fourni par l’utilisateur pour utiliser le chiffrement des données dans un compte Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="69d51-3642">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="69d51-3643">Interactive</span><span class="sxs-lookup"><span data-stu-id="69d51-3643">Interactive</span></span>

* <span data-ttu-id="69d51-3644">Amélioration du temps de démarrage à l’aide des commandes en cache</span><span class="sxs-lookup"><span data-stu-id="69d51-3644">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="69d51-3645">Couverture de test accrue</span><span class="sxs-lookup"><span data-stu-id="69d51-3645">Increased test coverage</span></span>
* <span data-ttu-id="69d51-3646">Amélioration du mouvement « ? » pour injecter également dans la commande suivante</span><span class="sxs-lookup"><span data-stu-id="69d51-3646">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="69d51-3647">Correction d’erreurs interactives avec le profil 2017-03-09-profil-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="69d51-3647">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="69d51-3648">Autorisé `--version` en tant que paramètre pour le mode interactif (#3645)</span><span class="sxs-lookup"><span data-stu-id="69d51-3648">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="69d51-3649">Empêche le mode interactif de lever des erreurs à partir des listes de saisie semi-automatique de validation (#3570)</span><span class="sxs-lookup"><span data-stu-id="69d51-3649">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="69d51-3650">Rapports de progression pour les déploiements de modèles (#3510)</span><span class="sxs-lookup"><span data-stu-id="69d51-3650">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="69d51-3651">Ajout de l’indicateur `--progress`</span><span class="sxs-lookup"><span data-stu-id="69d51-3651">Added `--progress` flag</span></span>
* <span data-ttu-id="69d51-3652">Suppression `--debug` et `--verbose` des listes de saisie semi-automatique</span><span class="sxs-lookup"><span data-stu-id="69d51-3652">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="69d51-3653">Suppression `interactive` des listes de saisie semi-automatique (#3324)</span><span class="sxs-lookup"><span data-stu-id="69d51-3653">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="69d51-3654">IoT</span><span class="sxs-lookup"><span data-stu-id="69d51-3654">IoT</span></span>

* <span data-ttu-id="69d51-3655">La création de la stratégie n’efface plus les stratégies existantes.</span><span class="sxs-lookup"><span data-stu-id="69d51-3655">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="69d51-3656">(#3934)</span><span class="sxs-lookup"><span data-stu-id="69d51-3656">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="69d51-3657">Coffre de clés</span><span class="sxs-lookup"><span data-stu-id="69d51-3657">Key vault</span></span>

* <span data-ttu-id="69d51-3658">Ajout de commandes pour les fonctionnalités de récupération de coffre de clés :</span><span class="sxs-lookup"><span data-stu-id="69d51-3658">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="69d51-3659">`keyvault`sous-commandes `purge`, `recover`,`keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="69d51-3659">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="69d51-3660">`keyvault secret`sous-commandes `backup`, `restore`, `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="69d51-3660">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="69d51-3661">`keyvault certificate`sous-commandes `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="69d51-3661">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="69d51-3662">`keyvault key`sous-commandes `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="69d51-3662">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="69d51-3663">Ajout de l’intégration du coffre de clés du principal du service (#3133)</span><span class="sxs-lookup"><span data-stu-id="69d51-3663">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="69d51-3664">Mise à jour du plan de données du coffre de clés vers 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="69d51-3664">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="69d51-3665">(#3307)</span><span class="sxs-lookup"><span data-stu-id="69d51-3665">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="69d51-3666">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="69d51-3666">Lab</span></span>

* <span data-ttu-id="69d51-3667">Ajout de la prise en charge de la revendication de toutes les machines virtuelles dans le laboratoire via `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="69d51-3667">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="69d51-3668">Ajout du formateur de sortie de tableau pour `az lab vm list` et `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="69d51-3668">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="69d51-3669">Superviser</span><span class="sxs-lookup"><span data-stu-id="69d51-3669">Monitor</span></span>

* <span data-ttu-id="69d51-3670">Correctif pour le fichier de modèle avec `monitor autoscale-settings get-parameters-template` commande (#3349)</span><span class="sxs-lookup"><span data-stu-id="69d51-3670">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="69d51-3671">`monitor alert-rule-incidents list` renommé en `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="69d51-3671">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="69d51-3672">`monitor alert-rule-incidents show` renommé en `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="69d51-3672">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="69d51-3673">`monitor metric-defintions list` renommé en `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="69d51-3673">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="69d51-3674">`monitor alert-rules` renommé en `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="69d51-3674">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="69d51-3675">Modifié `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="69d51-3675">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="69d51-3676">sous-commandes`condition` et `action` n’acceptent plus JSON</span><span class="sxs-lookup"><span data-stu-id="69d51-3676">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="69d51-3677">Ajout de nombreux paramètres simplifiant le processus de création de règle</span><span class="sxs-lookup"><span data-stu-id="69d51-3677">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="69d51-3678">`location` n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="69d51-3678">`location` no longer required</span></span>
  * <span data-ttu-id="69d51-3679">Ajout d’un nom et de la prise en charge de l’ID de la cible</span><span class="sxs-lookup"><span data-stu-id="69d51-3679">Add name and ID support for target</span></span>
  * <span data-ttu-id="69d51-3680">Suppression de `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="69d51-3680">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="69d51-3681">Le renommage de `is-enabled` en `enabled`n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="69d51-3681">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="69d51-3682">`description` par défaut sont désormais basées sur la condition fournie</span><span class="sxs-lookup"><span data-stu-id="69d51-3682">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="69d51-3683">Ajout d’exemples aidant à clarifier le nouveau format</span><span class="sxs-lookup"><span data-stu-id="69d51-3683">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="69d51-3684">Prise en charge des noms ou des ID pour les commandes `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="69d51-3684">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="69d51-3685">Ajout d’arguments d’usage et d’exemples pour `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="69d51-3685">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="69d51-3686">Réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-3686">Network</span></span>

* <span data-ttu-id="69d51-3687">Ajout de la commande `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="69d51-3687">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="69d51-3688">Ajout de l’argument `--private-access-services` à `vnet subnet create` et `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="69d51-3688">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="69d51-3689">Correction d’un problème `application-gateway redirect-config create` qui causait l’échec de</span><span class="sxs-lookup"><span data-stu-id="69d51-3689">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="69d51-3690">Correction d’un problème `application-gateway redirect-config update` qui `--no-wait` empêchait le fonctionnement de</span><span class="sxs-lookup"><span data-stu-id="69d51-3690">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="69d51-3691">Correction d’un bogue lié à l’utilisation d’un `--servers` argument avec `application-gateway address-pool create` et `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="69d51-3691">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="69d51-3692">Ajout des commandes `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="69d51-3692">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="69d51-3693">Ajout de commandes à `application-gateway ssl-policy` : `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="69d51-3693">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="69d51-3694">Ajout d’arguments à `application-gateway ssl-policy set` : `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="69d51-3694">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="69d51-3695">Ajout d’arguments à `application-gateway http-settings create` et `application-gateway http-settings update` : `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="69d51-3695">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="69d51-3696">Ajout d’arguments à `application-gateway url-path-map create` et `application-gateway url-path-map update`, `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="69d51-3696">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="69d51-3697">Ajout d’un argument `--redirect-config` à `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="69d51-3697">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="69d51-3698">Ajout de la prise en charge de `--no-wait` pour `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="69d51-3698">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="69d51-3699">Ajout d’arguments à `application-gateway probe create` et `application-gateway probe update` : `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="69d51-3699">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="69d51-3700">Ajout d’un argument `--redirect-config` à `application-gateway rule create` et `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="69d51-3700">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="69d51-3701">Ajout de la prise en charge de `--accelerated-networking` pour `nic create` et `nic update`</span><span class="sxs-lookup"><span data-stu-id="69d51-3701">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="69d51-3702">Suppression de l’ `--internal-dns-name-suffix` argument à partir de `nic create`</span><span class="sxs-lookup"><span data-stu-id="69d51-3702">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="69d51-3703">Ajout de la prise en charge de `--dns-servers` pour `nic update` et `nic create` : ajout de la prise en charge de --dns-servers</span><span class="sxs-lookup"><span data-stu-id="69d51-3703">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="69d51-3704">Correction d’un bogue qui faisait `local-gateway create` ignorer `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="69d51-3704">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="69d51-3705">Ajout de la prise en charge de `--dns-servers` pour `vnet update`</span><span class="sxs-lookup"><span data-stu-id="69d51-3705">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="69d51-3706">Correction d’un bogue lors de la création d’un peering sans filtrage de l’itinéraire avec `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="69d51-3706">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="69d51-3707">Correction d’un bogue qui empêchait le fonctionnement des arguments `--provider` et `--bandwidth` avec `express-route update`</span><span class="sxs-lookup"><span data-stu-id="69d51-3707">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="69d51-3708">Correction d’un bogue avec `network watcher show-topology` une logique de valeurs par défaut</span><span class="sxs-lookup"><span data-stu-id="69d51-3708">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="69d51-3709">Amélioration de la mise en forme de sortie pour `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="69d51-3709">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="69d51-3710">Utilisation de l’IP frontale par défaut pour `application-gateway http-listener create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="69d51-3710">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="69d51-3711">Utilisation d’un pool d’adresses par défaut, des paramètres HTTP et de l’écouteur HTTP pour `application-gateway rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="69d51-3711">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="69d51-3712">Utilisation de l’IP frontale par défaut et du pool principal `lb rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="69d51-3712">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="69d51-3713">Utilisation de l’IP frontale par défaut pour `lb inbound-nat-rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="69d51-3713">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="69d51-3714">Profil</span><span class="sxs-lookup"><span data-stu-id="69d51-3714">Profile</span></span>

* <span data-ttu-id="69d51-3715">Prise en charge de la connexion à l’intérieur d’une machine virtuelle avec une identité gérée</span><span class="sxs-lookup"><span data-stu-id="69d51-3715">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="69d51-3716">Prise en charge de la sortie pour `account show` au format de fichier d’authentification du Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="69d51-3716">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="69d51-3717">Affichage des avertissements de désapprobation lors de l’utilisation de '--expanded-view'</span><span class="sxs-lookup"><span data-stu-id="69d51-3717">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="69d51-3718">Ajout de la commande `get-access-token` permettant de fournir un jeton AAD brut</span><span class="sxs-lookup"><span data-stu-id="69d51-3718">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="69d51-3719">Prise en charge de la connexion avec un compte d’utilisateur sans abonnements associés</span><span class="sxs-lookup"><span data-stu-id="69d51-3719">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="69d51-3720">SGBDR</span><span class="sxs-lookup"><span data-stu-id="69d51-3720">RDBMS</span></span>

* <span data-ttu-id="69d51-3721">Prise en charge de l’énumération de serveurs à travers un abonnement (#3417)</span><span class="sxs-lookup"><span data-stu-id="69d51-3721">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="69d51-3722">Correction de `%s` non traité car il manque `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="69d51-3722">Fixed `%s` not processed because of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="69d51-3723">Correction du mappage de la source du document et ajout de la tâche CI permettant la vérification de (#3361)</span><span class="sxs-lookup"><span data-stu-id="69d51-3723">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="69d51-3724">Correction concernant l’aide relative à MySQL et PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="69d51-3724">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="69d51-3725">Ressource</span><span class="sxs-lookup"><span data-stu-id="69d51-3725">Resource</span></span>

* <span data-ttu-id="69d51-3726">Amélioration des invites pour les paramètres manquants de `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="69d51-3726">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="69d51-3727">Amélioration de l’analyse de `--parameters KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="69d51-3727">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="69d51-3728">Correction des problèmes à cause desquels `group deployment create` les fichiers de paramètres n’étaient plus reconnus à l’aide de la `@<file>` syntaxe</span><span class="sxs-lookup"><span data-stu-id="69d51-3728">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="69d51-3729">Prise en charge de l’ `--ids` argument pour `resource` et `managedapp` les commandes</span><span class="sxs-lookup"><span data-stu-id="69d51-3729">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="69d51-3730">Correction de certains messages d’analyse et d’erreur (#3584)</span><span class="sxs-lookup"><span data-stu-id="69d51-3730">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="69d51-3731">Correction de l’analyse `--resource-type` permettant à la `lock` commande d’accepter `<resource-namespace>` et `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="69d51-3731">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="69d51-3732">Ajout de la vérification de paramètre des modèles de liaison de modèle (#3629)</span><span class="sxs-lookup"><span data-stu-id="69d51-3732">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="69d51-3733">Ajout de la prise en charge de la spécification des paramètres de déploiement à l’aide de la `KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="69d51-3733">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="69d51-3734">Role</span><span class="sxs-lookup"><span data-stu-id="69d51-3734">Role</span></span>

* <span data-ttu-id="69d51-3735">Prise en charge de la sortie au format de fichier d’authentification du Kit de développement logiciel (SDK) pour `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="69d51-3735">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="69d51-3736">Nettoyage des attributions de rôles et de l’application AAD liée lors de la suppression d’un principal de service (#3610)</span><span class="sxs-lookup"><span data-stu-id="69d51-3736">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="69d51-3737">Inclusion du format d’heure dans `app create` args `--start-date` et `--end-date` descriptions</span><span class="sxs-lookup"><span data-stu-id="69d51-3737">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="69d51-3738">Affichage des avertissements de désapprobation lors de l’utilisation de `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="69d51-3738">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="69d51-3739">Ajout de l’intégration du coffre de clés pour les commandes `create-for-rbac` et `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="69d51-3739">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="69d51-3740">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="69d51-3740">Service Fabric</span></span>
* <span data-ttu-id="69d51-3741">Correction d’un problème avec les fichiers volumineux dans les applications tronquées sur le chargement (#3666)</span><span class="sxs-lookup"><span data-stu-id="69d51-3741">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="69d51-3742">Ajout de tests pour les commandes Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="69d51-3742">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="69d51-3743">Correction de nombreuses commandes Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="69d51-3743">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="69d51-3744">SQL</span><span class="sxs-lookup"><span data-stu-id="69d51-3744">SQL</span></span>

* <span data-ttu-id="69d51-3745">Suppression du paramètre `sql server create` `--identity` rompu</span><span class="sxs-lookup"><span data-stu-id="69d51-3745">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="69d51-3746">Suppression des valeurs de mot de passe à partir de la sortie de commande `sql server create` et `sql server update`</span><span class="sxs-lookup"><span data-stu-id="69d51-3746">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="69d51-3747">Ajout des commandes `sql db list-editions` et `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="69d51-3747">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="69d51-3748">Stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-3748">Storage</span></span>

* <span data-ttu-id="69d51-3749">Suppression d’une `--marker` option à partir des commandes `storage blob list`, `storage container list`et `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="69d51-3749">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="69d51-3750">Activation de la création d’un compte de stockage https-only</span><span class="sxs-lookup"><span data-stu-id="69d51-3750">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="69d51-3751">Mise à jour des métriques de stockage, de la journalisation et des commandes cors (#3495)</span><span class="sxs-lookup"><span data-stu-id="69d51-3751">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="69d51-3752">Reformulation d’un message d’exception de l’ajout CORS (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="69d51-3752">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="69d51-3753">Conversion du générateur à une liste en mode exécution d’essai de la commande de téléchargement de lot (#3592)</span><span class="sxs-lookup"><span data-stu-id="69d51-3753">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="69d51-3754">Correction du problème d’essai associé au lot de téléchargement du blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="69d51-3754">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="69d51-3755">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="69d51-3755">VM</span></span>

* <span data-ttu-id="69d51-3756">Prise en charge de la configuration du groupe de sécurité réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-3756">Support configuring nsg</span></span>
* <span data-ttu-id="69d51-3757">Correction d’un bogue qui entraînait une configuration incorrecte du serveur DNS</span><span class="sxs-lookup"><span data-stu-id="69d51-3757">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="69d51-3758">Prise en charge des identités de service géré</span><span class="sxs-lookup"><span data-stu-id="69d51-3758">Support managed service identities</span></span>
* <span data-ttu-id="69d51-3759">Correction d’un problème à cause duquel `cmss create` avec un équilibreur de charge existant exigeait `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="69d51-3759">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="69d51-3760">Les disques de données créés avec le numéro d’unité logique `vm image create` commencent à 0</span><span class="sxs-lookup"><span data-stu-id="69d51-3760">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="69d51-3761">10 mai 2017</span><span class="sxs-lookup"><span data-stu-id="69d51-3761">May 10, 2017</span></span>

<span data-ttu-id="69d51-3762">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="69d51-3762">Version 2.0.6</span></span>

* <span data-ttu-id="69d51-3763">documentdb renommé en cosmosdb</span><span class="sxs-lookup"><span data-stu-id="69d51-3763">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="69d51-3764">Ajouter rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="69d51-3764">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="69d51-3765">Inclure les modules Data Lake Analytics et Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="69d51-3765">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="69d51-3766">Inclure le module Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="69d51-3766">Include Cognitive Services module</span></span>
* <span data-ttu-id="69d51-3767">Inclure le module Service Fabric</span><span class="sxs-lookup"><span data-stu-id="69d51-3767">Include Service Fabric module</span></span>
* <span data-ttu-id="69d51-3768">Inclure le module Interactive (az-shell renommé)</span><span class="sxs-lookup"><span data-stu-id="69d51-3768">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="69d51-3769">Ajouter la prise en charge des commandes CDN</span><span class="sxs-lookup"><span data-stu-id="69d51-3769">Add support for CDN commands</span></span>
* <span data-ttu-id="69d51-3770">Supprimer le module Container</span><span class="sxs-lookup"><span data-stu-id="69d51-3770">Remove Container module</span></span>
* <span data-ttu-id="69d51-3771">Ajouter « az -v » comme raccourci pour « az --version » ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="69d51-3771">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="69d51-3772">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="69d51-3772">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="69d51-3773">Core</span><span class="sxs-lookup"><span data-stu-id="69d51-3773">Core</span></span>

* <span data-ttu-id="69d51-3774">principal : capturer les exceptions provoquées par un fournisseur non enregistré et l’enregistrer automatiquement</span><span class="sxs-lookup"><span data-stu-id="69d51-3774">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="69d51-3775">performance : conserver le cache de jeton adal en mémoire jusqu’à la fin du processus ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="69d51-3775">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="69d51-3776">Corriger les octets retournés par l’empreinte digitale hex -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="69d51-3776">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="69d51-3777">Téléchargement du certificat Key Vault et intégration AAD SP améliorés ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="69d51-3777">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="69d51-3778">Ajouter l’emplacement de Python à « az —version » ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="69d51-3778">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="69d51-3779">connexion : prise en charge de la connexion lorsqu’il n’y a aucun abonnement ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="69d51-3779">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="69d51-3780">principal : corriger une erreur lors de la connexion à l’aide d’un principal de service deux fois ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="69d51-3780">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="69d51-3781">principal : autoriser la configuration du chemin d’accès d’accessTokens.json via une variable d’environnement ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="69d51-3781">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="69d51-3782">principal : autoriser l’application des valeurs par défaut configurées sur les arguments facultatifs ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="69d51-3782">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="69d51-3783">principal : performances améliorées</span><span class="sxs-lookup"><span data-stu-id="69d51-3783">core: Improved performance</span></span>
* <span data-ttu-id="69d51-3784">principal : certificats d’autorité de certification personnalisés, prise en charge de la définition de la variable d’environnement REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="69d51-3784">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="69d51-3785">principal : configuration du cloud, utiliser le point de terminaison « resource manager » si le point de terminaison « management » n’est pas défini</span><span class="sxs-lookup"><span data-stu-id="69d51-3785">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="69d51-3786">ACS</span><span class="sxs-lookup"><span data-stu-id="69d51-3786">ACS</span></span>

* <span data-ttu-id="69d51-3787">corriger le nombre de maîtres et d’agents sur un nombre entier au lieu d’une chaîne</span><span class="sxs-lookup"><span data-stu-id="69d51-3787">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="69d51-3788">exposer « az acs create --no-wait » et « az acs wait » pour la création asynchrone</span><span class="sxs-lookup"><span data-stu-id="69d51-3788">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="69d51-3789">exposer « az acs create --validate » pour les validations de test</span><span class="sxs-lookup"><span data-stu-id="69d51-3789">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="69d51-3790">supprimer le profil Windows avant l’appel PUT pour la commande de mise à l’échelle ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="69d51-3790">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="69d51-3791">AppService</span><span class="sxs-lookup"><span data-stu-id="69d51-3791">AppService</span></span>

* <span data-ttu-id="69d51-3792">functionapp : ajouter la prise en charge complète de functionapp, notamment créer, afficher, liste, supprimer, nom d’hôte, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="69d51-3792">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="69d51-3793">Ajout de Team Services (vsts) comme option de livraison continue à « config contrôle source web appservice »</span><span class="sxs-lookup"><span data-stu-id="69d51-3793">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="69d51-3794">Créer « az webapp » pour remplacer « az appservice web » (pour la rétrocompatibilité, « az appservice web » sera conservé dans les 2 prochaines versions)</span><span class="sxs-lookup"><span data-stu-id="69d51-3794">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="69d51-3795">Exposer des arguments pour configurer le déploiement et des « piles d’exécution » sur webapp create</span><span class="sxs-lookup"><span data-stu-id="69d51-3795">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="69d51-3796">Exposer « webapp list-runtimes »</span><span class="sxs-lookup"><span data-stu-id="69d51-3796">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="69d51-3797">prendre en charge la configuration des chaînes de connexion ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="69d51-3797">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="69d51-3798">prendre en charge le basculement d’emplacement avec aperçu</span><span class="sxs-lookup"><span data-stu-id="69d51-3798">support slot swap with preview</span></span>
* <span data-ttu-id="69d51-3799">Supprimer les erreurs des commandes appservice ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="69d51-3799">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="69d51-3800">Utiliser le groupe de ressources du plan app service pour les opérations de certificat ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="69d51-3800">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="69d51-3801">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="69d51-3801">CosmosDB</span></span>

* <span data-ttu-id="69d51-3802">Renommer le module documentdb en cosmosdb</span><span class="sxs-lookup"><span data-stu-id="69d51-3802">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="69d51-3803">Prise en charge ajoutée pour les API de plan de données documentdb : gestion de base de données et de collecte</span><span class="sxs-lookup"><span data-stu-id="69d51-3803">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="69d51-3804">Prise en charge ajoutée pour activer le basculement automatique sur les comptes de base de données</span><span class="sxs-lookup"><span data-stu-id="69d51-3804">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="69d51-3805">Prise en charge ajoutée pour la nouvelle stratégie de cohérence ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="69d51-3805">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="69d51-3806">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="69d51-3806">Data Lake Analytics</span></span>

* <span data-ttu-id="69d51-3807">Corriger un bogue dans lequel le filtrage sur le résultat et l’état des listes de travaux lève une erreur</span><span class="sxs-lookup"><span data-stu-id="69d51-3807">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="69d51-3808">Ajouter la prise en charge d’un nouveau type d’élément de catalogue : paquet.</span><span class="sxs-lookup"><span data-stu-id="69d51-3808">Add support for new catalog item type: package.</span></span> <span data-ttu-id="69d51-3809">accessible via : `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="69d51-3809">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="69d51-3810">A rendu possible le fait de répertorier les éléments de catalogue suivants à partir d’une base de données (aucune spécification de schéma requise) :</span><span class="sxs-lookup"><span data-stu-id="69d51-3810">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="69d51-3811">Table de charge de travail</span><span class="sxs-lookup"><span data-stu-id="69d51-3811">Table</span></span>
  * <span data-ttu-id="69d51-3812">Fonction table</span><span class="sxs-lookup"><span data-stu-id="69d51-3812">Table valued function</span></span>
  * <span data-ttu-id="69d51-3813">Affichage</span><span class="sxs-lookup"><span data-stu-id="69d51-3813">View</span></span>
  * <span data-ttu-id="69d51-3814">Statistiques de table.</span><span class="sxs-lookup"><span data-stu-id="69d51-3814">Table Statistics.</span></span> <span data-ttu-id="69d51-3815">Cela peut également être répertorié avec un schéma, mais sans spécifier un nom de table</span><span class="sxs-lookup"><span data-stu-id="69d51-3815">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="69d51-3816">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="69d51-3816">Data Lake Store</span></span>

* <span data-ttu-id="69d51-3817">Mettre à jour la version du Kit de développement logiciel (SDK) du système de fichiers sous-jacent, qui offre une meilleure prise en charge pour gérer les scénarios de limitation côté serveur</span><span class="sxs-lookup"><span data-stu-id="69d51-3817">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="69d51-3818">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="69d51-3818">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="69d51-3819">aide manquante pour afficher l’accès.</span><span class="sxs-lookup"><span data-stu-id="69d51-3819">missed help for access show.</span></span> <span data-ttu-id="69d51-3820">ajout en cours.</span><span class="sxs-lookup"><span data-stu-id="69d51-3820">adding it.</span></span> <span data-ttu-id="69d51-3821">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="69d51-3821">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="69d51-3822">Rechercher</span><span class="sxs-lookup"><span data-stu-id="69d51-3822">Find</span></span>

* <span data-ttu-id="69d51-3823">résultats de la recherche améliorés et autorisation du contrôle de version de l’index de recherche</span><span class="sxs-lookup"><span data-stu-id="69d51-3823">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="69d51-3824">KeyVault</span><span class="sxs-lookup"><span data-stu-id="69d51-3824">KeyVault</span></span>

* <span data-ttu-id="69d51-3825">BC : `az keyvault certificate download` remplacer -e dans chaîne ou élément binaire par PEM ou DER afin de mieux représenter les options</span><span class="sxs-lookup"><span data-stu-id="69d51-3825">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="69d51-3826">BC : supprimer --expires et --not-before dans `keyvault certificate create`, car ces paramètres ne sont pas pris en charge par le service</span><span class="sxs-lookup"><span data-stu-id="69d51-3826">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="69d51-3827">Ajoute le paramètre --validity à `keyvault certificate create` pour substituer de manière sélective la valeur dans --policy</span><span class="sxs-lookup"><span data-stu-id="69d51-3827">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="69d51-3828">Résout le problème dans `keyvault certificate get-default-policy` où « expires » et « not_before » étaient exposés mais « validity_in_months » ne l’était pas</span><span class="sxs-lookup"><span data-stu-id="69d51-3828">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="69d51-3829">correction de keyvault pour l’importation de pem et pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="69d51-3829">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="69d51-3830">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="69d51-3830">Lab</span></span>

* <span data-ttu-id="69d51-3831">Ajout des commandes créer, afficher, supprimer et liste pour l’environnement dans le laboratoire</span><span class="sxs-lookup"><span data-stu-id="69d51-3831">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="69d51-3832">Ajout des commandes afficher et liste pour afficher les modèles ARM dans le laboratoire</span><span class="sxs-lookup"><span data-stu-id="69d51-3832">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="69d51-3833">Ajout de l’indicateur --environment dans `az lab vm list` pour filtrer les machines virtuelles selon l’environnement du laboratoire</span><span class="sxs-lookup"><span data-stu-id="69d51-3833">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="69d51-3834">Ajout de la commande pratique `az lab formula export-artifacts` pour exporter une structure d’artefact dans une formule de laboratoire</span><span class="sxs-lookup"><span data-stu-id="69d51-3834">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="69d51-3835">Ajout de commandes pour gérer les secrets dans un laboratoire</span><span class="sxs-lookup"><span data-stu-id="69d51-3835">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="69d51-3836">Superviser</span><span class="sxs-lookup"><span data-stu-id="69d51-3836">Monitor</span></span>

* <span data-ttu-id="69d51-3837">Résolution de bogue : modélisation de `--actions` de `az alert-rules create` pour consommer la chaîne JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="69d51-3837">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="69d51-3838">Correction de bogue : la création de paramètres de diagnostic n’accepte pas les métriques/journaux à partir des commandes d’affichage ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="69d51-3838">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="69d51-3839">Réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-3839">Network</span></span>

* <span data-ttu-id="69d51-3840">Ajouter la commande `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="69d51-3840">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="69d51-3841">Ajouter la prise en charge du paramètre `--filters` pour `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="69d51-3841">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="69d51-3842">Ajouter la prise en charge pour le drainage de connexion Application Gateway</span><span class="sxs-lookup"><span data-stu-id="69d51-3842">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="69d51-3843">Ajouter la prise en charge pour la configuration du jeu de règles WAF d’Application Gateway</span><span class="sxs-lookup"><span data-stu-id="69d51-3843">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="69d51-3844">Ajouter la prise en charge des règles et des filtres de routage ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="69d51-3844">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="69d51-3845">Ajouter la prise en charge pour le routage géographique TrafficManager</span><span class="sxs-lookup"><span data-stu-id="69d51-3845">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="69d51-3846">Ajouter la prise en charge des sélecteurs de trafic basés sur la stratégie de connexion VPN</span><span class="sxs-lookup"><span data-stu-id="69d51-3846">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="69d51-3847">Ajouter la prise en charge pour les stratégies IPSec de la connexion VPN</span><span class="sxs-lookup"><span data-stu-id="69d51-3847">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="69d51-3848">Corriger le bogue avec `vpn-connection create` lors de l’utilisation des paramètres `--no-wait` ou `--validate`</span><span class="sxs-lookup"><span data-stu-id="69d51-3848">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="69d51-3849">Ajouter la prise en charge des passerelles de réseau virtuel actif-actif</span><span class="sxs-lookup"><span data-stu-id="69d51-3849">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="69d51-3850">Supprimer les valeurs NULL de la sortie des commandes `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="69d51-3850">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="69d51-3851">BC : résoudre un bogue dans la sortie de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="69d51-3851">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="69d51-3852">Corriger le bogue où l’argument « --key-length » de « vpn-connection create » n’était pas analysé correctement</span><span class="sxs-lookup"><span data-stu-id="69d51-3852">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="69d51-3853">Corriger le bogue dans `dns zone import` où les enregistrements n’étaient pas été importés correctement</span><span class="sxs-lookup"><span data-stu-id="69d51-3853">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="69d51-3854">Corriger le bogue où `traffic-manager endpoint update` ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="69d51-3854">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="69d51-3855">Ajouter des commandes d’aperçu « network watcher »</span><span class="sxs-lookup"><span data-stu-id="69d51-3855">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="69d51-3856">Profil</span><span class="sxs-lookup"><span data-stu-id="69d51-3856">Profile</span></span>

* <span data-ttu-id="69d51-3857">Prendre en charge la connexion lorsqu’il n’y a aucun abonnement trouvé ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="69d51-3857">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="69d51-3858">Prendre en charge un nom de paramètre court dans le jeu de comptes az --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="69d51-3858">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="69d51-3859">Redis</span><span class="sxs-lookup"><span data-stu-id="69d51-3859">Redis</span></span>

* <span data-ttu-id="69d51-3860">Ajout d’une commande de mise à jour qui ajoute également la possibilité de mettre à l’échelle pour le cache redis</span><span class="sxs-lookup"><span data-stu-id="69d51-3860">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="69d51-3861">Commande « update-settings » déconseillée</span><span class="sxs-lookup"><span data-stu-id="69d51-3861">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="69d51-3862">Ressource</span><span class="sxs-lookup"><span data-stu-id="69d51-3862">Resource</span></span>

* <span data-ttu-id="69d51-3863">Ajouter managedapp et les commandes de définition managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="69d51-3863">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="69d51-3864">Prendre en charge les commandes « provider operation » ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="69d51-3864">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="69d51-3865">Prendre en charge la création de ressource générique ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="69d51-3865">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="69d51-3866">Corriger l’analyse de ressource et la recherche de version d’API.</span><span class="sxs-lookup"><span data-stu-id="69d51-3866">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="69d51-3867">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="69d51-3867">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="69d51-3868">Ajouter des documents pour mise à jour du verrou az.</span><span class="sxs-lookup"><span data-stu-id="69d51-3868">Add docs for az lock update.</span></span> <span data-ttu-id="69d51-3869">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="69d51-3869">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="69d51-3870">Sortie d’erreur si vous essayez de lister des ressources pour un groupe qui n’existe pas.</span><span class="sxs-lookup"><span data-stu-id="69d51-3870">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="69d51-3871">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="69d51-3871">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="69d51-3872">[Compute] Résoudre les problèmes de mise à jour de VMSS et du groupe à haute disponibilité de machines virtuelles.</span><span class="sxs-lookup"><span data-stu-id="69d51-3872">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="69d51-3873">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="69d51-3873">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="69d51-3874">Corriger le verrouillage des commandes créer et supprimer si parent-resource-path est None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="69d51-3874">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="69d51-3875">Role</span><span class="sxs-lookup"><span data-stu-id="69d51-3875">Role</span></span>

* <span data-ttu-id="69d51-3876">create-for-rbac : vérifier que la date de fin du SP ne dépassera pas la date d’expiration du certificat ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="69d51-3876">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="69d51-3877">RBAC : ajouter la prise en charge complète de « ad group » ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="69d51-3877">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="69d51-3878">rôle : résoudre les problèmes de mise à jour de définition de rôle ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="69d51-3878">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="69d51-3879">create-for-rbac : vérifier que le mot de passe fourni par l’utilisateur est accepté</span><span class="sxs-lookup"><span data-stu-id="69d51-3879">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="69d51-3880">SQL</span><span class="sxs-lookup"><span data-stu-id="69d51-3880">SQL</span></span>

* <span data-ttu-id="69d51-3881">Ajout des commandes az sql server list-usages et az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="69d51-3881">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="69d51-3882">SQL : possibilité de se connecter directement au fournisseur de ressources ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="69d51-3882">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="69d51-3883">Stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-3883">Storage</span></span>

* <span data-ttu-id="69d51-3884">Définir l’emplacement par défaut sur l’emplacement du groupe de ressources pour `storage account create`</span><span class="sxs-lookup"><span data-stu-id="69d51-3884">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="69d51-3885">Ajouter la prise en charge de la copie incrémentielle d’objet blob</span><span class="sxs-lookup"><span data-stu-id="69d51-3885">Add support for incremental blob copy</span></span>
* <span data-ttu-id="69d51-3886">Ajouter la prise en charge du chargement d’objet blob de blocs volumineux</span><span class="sxs-lookup"><span data-stu-id="69d51-3886">Add support for large block blob upload</span></span>
* <span data-ttu-id="69d51-3887">Modifier la taille de bloc à 100 Mo lorsque le fichier à charger est supérieur à 200 Go</span><span class="sxs-lookup"><span data-stu-id="69d51-3887">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="69d51-3888">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="69d51-3888">VM</span></span>

* <span data-ttu-id="69d51-3889">avail-set : rendre le compte de domaine UD&FD facultatif</span><span class="sxs-lookup"><span data-stu-id="69d51-3889">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="69d51-3890">Remarque : commandes de machine virtuelle dans clouds souverains. Veuillez éviter les fonctionnalités liées au disque managé, notamment :</span><span class="sxs-lookup"><span data-stu-id="69d51-3890">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="69d51-3891">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="69d51-3891">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="69d51-3892">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="69d51-3892">az vm/vmss disk</span></span>
  3. <span data-ttu-id="69d51-3893">Dans « az vm/vmss create », utiliser « —use-unmanaged-disk » pour éviter le disque managé Les autres commandes devraient fonctionner</span><span class="sxs-lookup"><span data-stu-id="69d51-3893">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="69d51-3894">vm/vmss : améliorer le texte d’avertissement lors de la génération de paires de clés ssh</span><span class="sxs-lookup"><span data-stu-id="69d51-3894">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="69d51-3895">vm/vmss : prendre en charge la création à partir d’une image de la Place de marché qui requiert des informations sur le plan ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="69d51-3895">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="69d51-3896">3 avril 2017</span><span class="sxs-lookup"><span data-stu-id="69d51-3896">April 3, 2017</span></span>

<span data-ttu-id="69d51-3897">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="69d51-3897">Version 2.0.2</span></span>

<span data-ttu-id="69d51-3898">Nous avons publié les composants ACR, Batch, KeyVault et SQL dans cette version</span><span class="sxs-lookup"><span data-stu-id="69d51-3898">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="69d51-3899">Core</span><span class="sxs-lookup"><span data-stu-id="69d51-3899">Core</span></span>

* <span data-ttu-id="69d51-3900">Ajout des modules acr, lab, monitor et find à la liste par défaut</span><span class="sxs-lookup"><span data-stu-id="69d51-3900">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="69d51-3901">Connexion : ignorer les locataires erronés ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="69d51-3901">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="69d51-3902">login : définition de l’abonnement par défaut à la valeur « un » avec l’état « Activé » ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="69d51-3902">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="69d51-3903">Ajout de la prise en charge des commandes wait et de --no-wait à davantage de commandes ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="69d51-3903">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="69d51-3904">core : prise en charge de la connexion à l’aide du principal du service avec un certificat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="69d51-3904">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="69d51-3905">Ajout d’une invite pour les paramètres de modèle manquants.</span><span class="sxs-lookup"><span data-stu-id="69d51-3905">Add prompting for missing template parameters.</span></span> <span data-ttu-id="69d51-3906">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="69d51-3906">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="69d51-3907">Prise en charge de la définition de valeurs par défaut pour des arguments courants tels que le groupe de ressources par défaut, le site web par défaut et la machine virtuelle par défaut</span><span class="sxs-lookup"><span data-stu-id="69d51-3907">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="69d51-3908">Prise en charge de la connexion à un locataire spécifique</span><span class="sxs-lookup"><span data-stu-id="69d51-3908">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="69d51-3909">ACS</span><span class="sxs-lookup"><span data-stu-id="69d51-3909">ACS</span></span>

* <span data-ttu-id="69d51-3910">[ACS] Ajout de la prise en charge de la configuration d’un cluster ACS par défaut ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="69d51-3910">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="69d51-3911">Ajout de la prise en charge de l’invite de mot de passe de clé ssh.</span><span class="sxs-lookup"><span data-stu-id="69d51-3911">Add support for ssh key password prompting.</span></span> <span data-ttu-id="69d51-3912">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="69d51-3912">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="69d51-3913">Ajout de la prise en charge des clusters Windows.</span><span class="sxs-lookup"><span data-stu-id="69d51-3913">Add support for windows clusters.</span></span> <span data-ttu-id="69d51-3914">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="69d51-3914">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="69d51-3915">Basculement du rôle Propriétaire au rôle Contributeur.</span><span class="sxs-lookup"><span data-stu-id="69d51-3915">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="69d51-3916">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="69d51-3916">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="69d51-3917">AppService</span><span class="sxs-lookup"><span data-stu-id="69d51-3917">AppService</span></span>

* <span data-ttu-id="69d51-3918">appservice : prise en charge de l’obtention de l’adresse IP externe utilisée pour les enregistrements A DNS ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="69d51-3918">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="69d51-3919">appservice : prise en charge de la liaison des certificats avec caractères génériques ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="69d51-3919">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="69d51-3920">appservice : prise en charge des profils de publication de liste ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="69d51-3920">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="69d51-3921">AppService : déclenchement de la synchronisation de contrôle de code source après la configuration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="69d51-3921">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="69d51-3922">DataLake</span><span class="sxs-lookup"><span data-stu-id="69d51-3922">DataLake</span></span>

* <span data-ttu-id="69d51-3923">Version initiale du module Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="69d51-3923">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="69d51-3924">Version initiale du module Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="69d51-3924">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="69d51-3925">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="69d51-3925">DocuemntDB</span></span>

* <span data-ttu-id="69d51-3926">DocumentDB : ajout de la prise en charge de l’énumération des chaînes de connexion ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="69d51-3926">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="69d51-3927">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="69d51-3927">VM</span></span>

* <span data-ttu-id="69d51-3928">[Compute] Ajout de la prise en charge d’AppGateway à la création de groupe de machines virtuelles identiques ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="69d51-3928">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="69d51-3929">[VM/VMSS] Amélioration de la prise en charge de la mise en cache de disque ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="69d51-3929">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="69d51-3930">VM/VMSS : intégration de la logique de validation des informations d’identification utilisée par le portail ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="69d51-3930">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="69d51-3931">Ajout de la prise en charge des commandes wait et de --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="69d51-3931">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="69d51-3932">Groupe de machines virtuelles identiques : prise en charge de \* pour énumérer les vues d’instance parmi les machines virtuelles ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="69d51-3932">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="69d51-3933">Ajout --secrets pour machine virtuelle et groupe de machines virtuelles identiques ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="69d51-3933">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="69d51-3934">Autorisation de la création de machines virtuelles avec un disque dur virtuel spécialisé ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="69d51-3934">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="69d51-3935">27 février 2017</span><span class="sxs-lookup"><span data-stu-id="69d51-3935">February 27, 2017</span></span>

<span data-ttu-id="69d51-3936">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="69d51-3936">Version 2.0.0</span></span>

<span data-ttu-id="69d51-3937">Cette version d’Azure CLI 2.0 est la première instance mise à la disposition générale. La disponibilité générale s’applique à ces modules de commande :</span><span class="sxs-lookup"><span data-stu-id="69d51-3937">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="69d51-3938">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="69d51-3938">Container Service (acs)</span></span>
- <span data-ttu-id="69d51-3939">Compute (notamment Resource Manager, machine virtuelle, groupes de machines virtuelles identiques, Disques managés)</span><span class="sxs-lookup"><span data-stu-id="69d51-3939">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="69d51-3940">Mise en réseau</span><span class="sxs-lookup"><span data-stu-id="69d51-3940">Networking</span></span>
- <span data-ttu-id="69d51-3941">Stockage</span><span class="sxs-lookup"><span data-stu-id="69d51-3941">Storage</span></span>

<span data-ttu-id="69d51-3942">Ces modules de commande, pouvant être utilisés en production, sont pris en charge par le contrat de niveau de service (SLA) Microsoft standard. Vous pouvez ouvrir des incidents directement auprès du support technique Microsoft ou dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/). Vous pouvez poser des questions sur [StackOverflow à l’aide du mot-clé azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), ou contacter l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Vous pouvez fournir des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="69d51-3942">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="69d51-3943">Les commandes de ces modules sont stables et il n’est pas prévu que la syntaxe change dans les mises à jour ultérieures de cette version d’Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="69d51-3943">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="69d51-3944">Pour vérifier la version de l’interface CLI, utilisez `az --version`. La sortie indique la version de l’interface CLI proprement dite (2.0.0 dans cette version), les différents modules de commande et les versions de Python et de GCC que vous utilisez.</span><span class="sxs-lookup"><span data-stu-id="69d51-3944">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="69d51-3945">Certains de ces modules de commande présentent un suffixe « b*n* » ou « rc*n* ». Ces modules de commande, encore en préversion, seront mis à la disposition générale à l’avenir.</span><span class="sxs-lookup"><span data-stu-id="69d51-3945">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="69d51-3946">Nous avons également des versions d’évaluation nocturnes de l’interface CLI. Pour plus d’informations, consultez ces instructions sur l’[obtention des builds nocturnes](https://github.com/Azure/azure-cli#nightly-builds), ainsi que ces instructions sur [la contribution au code et la configuration d’un environnement de développement](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="69d51-3946">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="69d51-3947">Vous pouvez signaler des problèmes liés aux versions d’évaluation nocturnes comme suit :</span><span class="sxs-lookup"><span data-stu-id="69d51-3947">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="69d51-3948">Signalez des problèmes dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="69d51-3948">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="69d51-3949">Contactez l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="69d51-3949">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="69d51-3950">Fournissez des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="69d51-3950">Provide feedback from the command line with the `az feedback` command</span></span>

# <a name="beta-release-notes"></a>[<span data-ttu-id="69d51-3951">Notes de publication de la version bêta</span><span class="sxs-lookup"><span data-stu-id="69d51-3951">Beta release notes</span></span>](#tab/azure-cli-beta)

<span data-ttu-id="69d51-3952">La version bêta d’Azure CLI est une migration qui fait suite au changement de la méthode d’authentification, de la plateforme AAD (v1.0) à la [Plateforme d’identité Microsoft (v2.0)](/azure/active-directory/develop/v2-overview).</span><span class="sxs-lookup"><span data-stu-id="69d51-3952">The Azure CLI beta release is a migration from the authentican method of AAD platform (v1.0) to [Microsoft Identity platform (v2.0)](/azure/active-directory/develop/v2-overview).</span></span>

## <a name="june-23-2020"></a><span data-ttu-id="69d51-3953">23 juin 2020</span><span class="sxs-lookup"><span data-stu-id="69d51-3953">June 23, 2020</span></span>

### <a name="things-to-know-about-the-new-azure-cli-beta-release"></a><span data-ttu-id="69d51-3954">Choses à savoir sur la nouvelle version bêta d’Azure CLI</span><span class="sxs-lookup"><span data-stu-id="69d51-3954">Things to know about the new Azure CLI beta release</span></span>

-   <span data-ttu-id="69d51-3955">La version bêta d’Azure CLI prend en charge toutes les commandes CLI disponibles dans la version finale actuelle.</span><span class="sxs-lookup"><span data-stu-id="69d51-3955">The beta version of the Azure CLI supports all CLI commands that you will find in the current released version.</span></span>
-   <span data-ttu-id="69d51-3956">Notez que vous devrez vous reconnecter une fois la version bêta installée.</span><span class="sxs-lookup"><span data-stu-id="69d51-3956">Relogin is required after install the beta version.</span></span>
-   <span data-ttu-id="69d51-3957">La version bêta prend uniquement en charge la plateforme Windows.</span><span class="sxs-lookup"><span data-stu-id="69d51-3957">The beta release only supports the Windows platform.</span></span>
-   <span data-ttu-id="69d51-3958">Azure Stack n’est pas pris en charge.</span><span class="sxs-lookup"><span data-stu-id="69d51-3958">The Azure Stack is not supported.</span></span>
-   <span data-ttu-id="69d51-3959">Le paramètre `--use-cert-sn-issuer` n’est pas pris en charge lors de l’utilisation de la clé du principal de service pour l’authentification.</span><span class="sxs-lookup"><span data-stu-id="69d51-3959">`--use-cert-sn-issuer` parameter is not supported when using service principal key to authenticate.</span></span>
-   <span data-ttu-id="69d51-3960">Ignorer la vérification SSL par le biais de l’environnement `ADAL_PYTHON_SSL_NO_VERIFY` n’est pas pris en charge.</span><span class="sxs-lookup"><span data-stu-id="69d51-3960">Skip SSL verification via environment `ADAL_PYTHON_SSL_NO_VERIFY` is not supported.</span></span>

<span data-ttu-id="69d51-3961">Si vous rencontrez des problèmes dans la version bêta, envoyez vos commentaires à l’équipe d’ingénieurs d’Azure CLI sur [GitHub](https://github.com/Azure/azure-cli/issues/new/choose).</span><span class="sxs-lookup"><span data-stu-id="69d51-3961">If you find any issues in the beta release, the Azure CLI engineering team welcomes your comments on [GitHub](https://github.com/Azure/azure-cli/issues/new/choose).</span></span>

---
