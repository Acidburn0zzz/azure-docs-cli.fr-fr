---
title: Notes de publication d’Azure CLI 2.0
description: En savoir plus sur les dernières mises à jour d’Azure CLI 2.0
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 08/28/2018
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 5d179a49ad64201270be7848a72535b871081125
ms.sourcegitcommit: c90bc90c9a2b3adf2836d7cfb84951cd3ab51317
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/06/2018
ms.locfileid: "43828743"
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="93d0e-103">Notes de publication d’Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="93d0e-103">Azure CLI 2.0 release notes</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="93d0e-104">28 Août 2018</span><span class="sxs-lookup"><span data-stu-id="93d0e-104">August 28, 2018</span></span>

<span data-ttu-id="93d0e-105">Version 2.0.45</span><span class="sxs-lookup"><span data-stu-id="93d0e-105">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="93d0e-106">Principal</span><span class="sxs-lookup"><span data-stu-id="93d0e-106">Core</span></span>

* <span data-ttu-id="93d0e-107">Résolution du problème de chargement de fichier de configuration vide</span><span class="sxs-lookup"><span data-stu-id="93d0e-107">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="93d0e-108">Ajout de la prise en charge du profil `2018-03-01-hybrid` pour Azure Stack</span><span class="sxs-lookup"><span data-stu-id="93d0e-108">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="93d0e-109">ACR</span><span class="sxs-lookup"><span data-stu-id="93d0e-109">ACR</span></span>

* <span data-ttu-id="93d0e-110">Ajout d’une solution pour les opérations d’exécution sans les requêtes ARM</span><span class="sxs-lookup"><span data-stu-id="93d0e-110">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="93d0e-111">Exclusion des fichiers de contrôle de version (par exemple, .git, .gitignore) chargés par défaut dans les fichiers tar dans la commande `build`</span><span class="sxs-lookup"><span data-stu-id="93d0e-111">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="93d0e-112">ACS</span><span class="sxs-lookup"><span data-stu-id="93d0e-112">ACS</span></span>

* <span data-ttu-id="93d0e-113">Modification de `aks create` à la valeur par défaut sur les machines virtuelles `Standard_DS2_v2`</span><span class="sxs-lookup"><span data-stu-id="93d0e-113">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="93d0e-114">Modification de `aks get-credentials` afin d’appeler de nouvelles API pour l’obtention des informations d’identification des clusters</span><span class="sxs-lookup"><span data-stu-id="93d0e-114">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="93d0e-115">AppService</span><span class="sxs-lookup"><span data-stu-id="93d0e-115">AppService</span></span>

* <span data-ttu-id="93d0e-116">Prise en charge de CORS sur functionapp et webapp</span><span class="sxs-lookup"><span data-stu-id="93d0e-116">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="93d0e-117">Ajout de la prise en charge de la balise ARM sur les commandes de création</span><span class="sxs-lookup"><span data-stu-id="93d0e-117">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="93d0e-118">Modification de `[webapp|functionapp] identity show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="93d0e-118">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="93d0e-119">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="93d0e-119">Backup</span></span>

* <span data-ttu-id="93d0e-120">Modification de `backup vault backup-properties show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="93d0e-120">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="93d0e-121">Service de robot</span><span class="sxs-lookup"><span data-stu-id="93d0e-121">Bot Service</span></span>

* <span data-ttu-id="93d0e-122">Version initiale de l’interface CLI de Bot Service</span><span class="sxs-lookup"><span data-stu-id="93d0e-122">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="93d0e-123">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="93d0e-123">Cognitive Services</span></span>

* <span data-ttu-id="93d0e-124">Ajout du nouveau paramètre `--api-properties,` requis pour la création de certains services</span><span class="sxs-lookup"><span data-stu-id="93d0e-124">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="93d0e-125">IoT</span><span class="sxs-lookup"><span data-stu-id="93d0e-125">IoT</span></span>

* <span data-ttu-id="93d0e-126">Résolution du problème relatif à l’association de hubs liés</span><span class="sxs-lookup"><span data-stu-id="93d0e-126">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="93d0e-127">Surveiller</span><span class="sxs-lookup"><span data-stu-id="93d0e-127">Monitor</span></span>

* <span data-ttu-id="93d0e-128">Ajout des commandes `monitor metrics alert` permettant de recevoir des alertes sur les métriques quasiment en temps réel</span><span class="sxs-lookup"><span data-stu-id="93d0e-128">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="93d0e-129">Commandes `monitor alert` déconseillées</span><span class="sxs-lookup"><span data-stu-id="93d0e-129">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="93d0e-130">Réseau</span><span class="sxs-lookup"><span data-stu-id="93d0e-130">Network</span></span>

* <span data-ttu-id="93d0e-131">Modification de `network application-gateway ssl-policy predefined show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="93d0e-131">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="93d0e-132">Ressource</span><span class="sxs-lookup"><span data-stu-id="93d0e-132">Resource</span></span>

* <span data-ttu-id="93d0e-133">Modification de `provider operation show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="93d0e-133">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="93d0e-134">Stockage</span><span class="sxs-lookup"><span data-stu-id="93d0e-134">Storage</span></span>

* <span data-ttu-id="93d0e-135">Modification de `storage share policy show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="93d0e-135">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="93d0e-136">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="93d0e-136">VM</span></span>

* <span data-ttu-id="93d0e-137">Modification de `vm/vmss identity show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="93d0e-137">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="93d0e-138">Remplacement de `--storage-caching` pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="93d0e-138">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="93d0e-139">14 août 2018</span><span class="sxs-lookup"><span data-stu-id="93d0e-139">Auguest 14, 2018</span></span>

<span data-ttu-id="93d0e-140">Version 2.0.44</span><span class="sxs-lookup"><span data-stu-id="93d0e-140">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="93d0e-141">Principal</span><span class="sxs-lookup"><span data-stu-id="93d0e-141">Core</span></span>

* <span data-ttu-id="93d0e-142">Correction de l’affichage numérique dans la sortie `table`</span><span class="sxs-lookup"><span data-stu-id="93d0e-142">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="93d0e-143">Ajout du format de sortie YAML</span><span class="sxs-lookup"><span data-stu-id="93d0e-143">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="93d0e-144">Télémétrie</span><span class="sxs-lookup"><span data-stu-id="93d0e-144">Telemetry</span></span>

* <span data-ttu-id="93d0e-145">Amélioration des rapports de télémétrie</span><span class="sxs-lookup"><span data-stu-id="93d0e-145">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="93d0e-146">ACR</span><span class="sxs-lookup"><span data-stu-id="93d0e-146">ACR</span></span>

* <span data-ttu-id="93d0e-147">Ajout des commandes `content-trust policy`</span><span class="sxs-lookup"><span data-stu-id="93d0e-147">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="93d0e-148">Résolution du problème où `.dockerignore` n’était pas honorée</span><span class="sxs-lookup"><span data-stu-id="93d0e-148">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="93d0e-149">ACS</span><span class="sxs-lookup"><span data-stu-id="93d0e-149">ACS</span></span>

* <span data-ttu-id="93d0e-150">Modification de `az acs/aks install-cli` afin d’effectuer l’installation sous `%USERPROFILE%\.azure-kubectl` sur Windows</span><span class="sxs-lookup"><span data-stu-id="93d0e-150">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="93d0e-151">Modification de `az aks install-connector` afin de détecter si le cluster dispose du contrôle RBAC et de configurer le connecteur ACI correctement</span><span class="sxs-lookup"><span data-stu-id="93d0e-151">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="93d0e-152">Remplacement par l’attribution de rôle au sous-réseau lorsque l’attribution est fournie</span><span class="sxs-lookup"><span data-stu-id="93d0e-152">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="93d0e-153">Ajout de l’option nouveau « ignorer attribution de rôle » pour le sous-réseau lorsque l’attribution est fournie</span><span class="sxs-lookup"><span data-stu-id="93d0e-153">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="93d0e-154">Modification ignorant l’attribution de rôle au sous-réseau lorsque l’attribution existe déjà</span><span class="sxs-lookup"><span data-stu-id="93d0e-154">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="93d0e-155">AppService</span><span class="sxs-lookup"><span data-stu-id="93d0e-155">AppService</span></span>

* <span data-ttu-id="93d0e-156">Correction d’un bogue empêchant de créer une application de fonction à l’aide de comptes de stockage dans les groupes de ressources externes</span><span class="sxs-lookup"><span data-stu-id="93d0e-156">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="93d0e-157">Correction d’un incident lors du déploiement de dossier zip</span><span class="sxs-lookup"><span data-stu-id="93d0e-157">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="93d0e-158">Batch AI</span><span class="sxs-lookup"><span data-stu-id="93d0e-158">BatchAI</span></span>

* <span data-ttu-id="93d0e-159">Modification de la sortie de l’enregistreur d’événements pour la création du compte de stockage automatique afin de spécifier l’information « ressource *groupe*».</span><span class="sxs-lookup"><span data-stu-id="93d0e-159">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="93d0e-160">Conteneur</span><span class="sxs-lookup"><span data-stu-id="93d0e-160">Container</span></span>

* <span data-ttu-id="93d0e-161">Ajout de `--secure-environment-variables` pour transmettre des variables d’environnement sécurisées vers un conteneur</span><span class="sxs-lookup"><span data-stu-id="93d0e-161">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="93d0e-162">IoT</span><span class="sxs-lookup"><span data-stu-id="93d0e-162">IoT</span></span>

* <span data-ttu-id="93d0e-163">[CHANGEMENT CASSANT] Suppression des commandes obsolètes déplacées vers l’extension iot</span><span class="sxs-lookup"><span data-stu-id="93d0e-163">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="93d0e-164">Mise à jour des éléments afin de ne pas prendre en compte le domaine `azure-devices.net`</span><span class="sxs-lookup"><span data-stu-id="93d0e-164">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="93d0e-165">Iot Central</span><span class="sxs-lookup"><span data-stu-id="93d0e-165">Iot Central</span></span>

* <span data-ttu-id="93d0e-166">Version initiale du module IoT Central</span><span class="sxs-lookup"><span data-stu-id="93d0e-166">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="93d0e-167">KeyVault</span><span class="sxs-lookup"><span data-stu-id="93d0e-167">KeyVault</span></span>


* <span data-ttu-id="93d0e-168">Ajout des commandes pour la gestion des comptes de stockage et les définitions SAS</span><span class="sxs-lookup"><span data-stu-id="93d0e-168">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="93d0e-169">Ajout de commandes pour les règles réseau</span><span class="sxs-lookup"><span data-stu-id="93d0e-169">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="93d0e-170">Ajout du paramètre `--id` aux opérations relatives au mots de passe confidentiels, clés et certificats</span><span class="sxs-lookup"><span data-stu-id="93d0e-170">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="93d0e-171">Ajout de la prise en charge pour la version multi-api avec gestion des coffres de clés</span><span class="sxs-lookup"><span data-stu-id="93d0e-171">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="93d0e-172">Ajout de la prise en charge pour la version multi-api avec plan de données des coffres de clés</span><span class="sxs-lookup"><span data-stu-id="93d0e-172">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="93d0e-173">Relais</span><span class="sxs-lookup"><span data-stu-id="93d0e-173">Relay</span></span>

* <span data-ttu-id="93d0e-174">Version initiale</span><span class="sxs-lookup"><span data-stu-id="93d0e-174">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="93d0e-175">SQL</span><span class="sxs-lookup"><span data-stu-id="93d0e-175">Sql</span></span>

* <span data-ttu-id="93d0e-176">Ajout des commandes `sql failover-group`</span><span class="sxs-lookup"><span data-stu-id="93d0e-176">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="93d0e-177">Stockage</span><span class="sxs-lookup"><span data-stu-id="93d0e-177">Storage</span></span>

* <span data-ttu-id="93d0e-178">[CHANGEMENT CASSANT] Modification de `storage account show-usage` afin d’exiger le paramètre `--location` et de répertorier par région</span><span class="sxs-lookup"><span data-stu-id="93d0e-178">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="93d0e-179">Modification du paramètre `--resource-group` afin de le rendre facultatif pour les commandes `storage account`</span><span class="sxs-lookup"><span data-stu-id="93d0e-179">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="93d0e-180">Suppression des avertissements concernant l’échec de la condition préalable pour les défaillances isolées dans les commandes batch pour les messages agrégés uniques</span><span class="sxs-lookup"><span data-stu-id="93d0e-180">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="93d0e-181">Modification des commandes `[blob|file] delete-batch` afin de ne plus produire des tableaux ayant la valeur null</span><span class="sxs-lookup"><span data-stu-id="93d0e-181">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="93d0e-182">Modification des commandes `blob [download|upload|delete-batch]` afin de lire le jeton de SAS à partir de l’url du conteneur</span><span class="sxs-lookup"><span data-stu-id="93d0e-182">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="93d0e-183">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="93d0e-183">VM</span></span>

* <span data-ttu-id="93d0e-184">Ajout des filtres courants à `vm list-skus` pour une plus grande simplicité d’utilisation</span><span class="sxs-lookup"><span data-stu-id="93d0e-184">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="93d0e-185">31 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="93d0e-185">July 31, 2018</span></span>

<span data-ttu-id="93d0e-186">Version 2.0.43</span><span class="sxs-lookup"><span data-stu-id="93d0e-186">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="93d0e-187">ACR</span><span class="sxs-lookup"><span data-stu-id="93d0e-187">ACR</span></span>

* <span data-ttu-id="93d0e-188">Ajout de l’indicateur `--with-secure-properties` à la commande `acr build-task show`</span><span class="sxs-lookup"><span data-stu-id="93d0e-188">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="93d0e-189">Ajout de la commande `acr build-task update-build`</span><span class="sxs-lookup"><span data-stu-id="93d0e-189">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="93d0e-190">ACS</span><span class="sxs-lookup"><span data-stu-id="93d0e-190">ACS</span></span>

* <span data-ttu-id="93d0e-191">Retour au return 0 (réussite) à la fin de `az aks browse` en appuyant sur [Ctrl + C]</span><span class="sxs-lookup"><span data-stu-id="93d0e-191">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="93d0e-192">Batch</span><span class="sxs-lookup"><span data-stu-id="93d0e-192">Batch</span></span>

* <span data-ttu-id="93d0e-193">Correction du bug lors de l’affichage des jetons AAD dans le Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="93d0e-193">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="93d0e-194">Conteneur</span><span class="sxs-lookup"><span data-stu-id="93d0e-194">Container</span></span>

* <span data-ttu-id="93d0e-195">Suppression de l’exigence pour `--log-analytics-workspace-key` pour le nom ou l’identifiant lors de l’abonnement standard</span><span class="sxs-lookup"><span data-stu-id="93d0e-195">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="93d0e-196">Réseau</span><span class="sxs-lookup"><span data-stu-id="93d0e-196">Network</span></span>

* <span data-ttu-id="93d0e-197">Ajout du serveur DNS au profil du 09/03/2017 pour Azure Stack</span><span class="sxs-lookup"><span data-stu-id="93d0e-197">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="93d0e-198">Ressource</span><span class="sxs-lookup"><span data-stu-id="93d0e-198">Resource</span></span>

* <span data-ttu-id="93d0e-199">Ajout de `--rollback-on-error` à `group deployment create` pour exécuter un déploiement correct et connu en cas d’erreur</span><span class="sxs-lookup"><span data-stu-id="93d0e-199">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="93d0e-200">Correction d’un problème où `--parameters {}` avec `group deployment create` entraînait une erreur</span><span class="sxs-lookup"><span data-stu-id="93d0e-200">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="93d0e-201">Rôle</span><span class="sxs-lookup"><span data-stu-id="93d0e-201">Role</span></span>

* <span data-ttu-id="93d0e-202">Ajout de la prise en charge du profil stack du 09/03/2017</span><span class="sxs-lookup"><span data-stu-id="93d0e-202">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="93d0e-203">Correction d’un problème où les paramètres de mise à jour génériques à `app update` ne fonctionnaient pas correctement</span><span class="sxs-lookup"><span data-stu-id="93d0e-203">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="93d0e-204">Recherche</span><span class="sxs-lookup"><span data-stu-id="93d0e-204">Search</span></span>

* <span data-ttu-id="93d0e-205">Ajout de commandes pour le service de recherches d’Azure</span><span class="sxs-lookup"><span data-stu-id="93d0e-205">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="93d0e-206">Service Bus</span><span class="sxs-lookup"><span data-stu-id="93d0e-206">Service Bus</span></span>

* <span data-ttu-id="93d0e-207">Ajout d’un groupe de commandes de migration pour migrer un espace de noms d’un Service Bus Standard à un Premium</span><span class="sxs-lookup"><span data-stu-id="93d0e-207">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="93d0e-208">Ajout de nouvelles propriétés facultatives à la file d’attente du Service Bus et à l’abonnement</span><span class="sxs-lookup"><span data-stu-id="93d0e-208">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="93d0e-209">`--enable-batched-operations` et `--enable-dead-lettering-on-message-expiration` dans `queue`</span><span class="sxs-lookup"><span data-stu-id="93d0e-209">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="93d0e-210">`--dead-letter-on-filter-exceptions` dans `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="93d0e-210">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="93d0e-211">Stockage</span><span class="sxs-lookup"><span data-stu-id="93d0e-211">Storage</span></span>

* <span data-ttu-id="93d0e-212">Ajout de la prise en charge du téléchargement de fichiers volumineux à l’aide d’une connexion unique</span><span class="sxs-lookup"><span data-stu-id="93d0e-212">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="93d0e-213">Conversion des commandes `show` qui manquaient d’échouer avec le code de sortie 3 sur une ressource manquante</span><span class="sxs-lookup"><span data-stu-id="93d0e-213">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="93d0e-214">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="93d0e-214">VM</span></span>

* <span data-ttu-id="93d0e-215">Ajout d’une prise en charge pour lister les groupes disponibles par abonnement</span><span class="sxs-lookup"><span data-stu-id="93d0e-215">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="93d0e-216">Ajout de la prise en charge de `StandardSSD_LRS`</span><span class="sxs-lookup"><span data-stu-id="93d0e-216">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="93d0e-217">Ajout d’une prise en charge des groupes de sécurité d’application dans la création du groupe identique de machines virtuelles</span><span class="sxs-lookup"><span data-stu-id="93d0e-217">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="93d0e-218">[CHANGEMENT CASSANT] Changement de `[vm|vmss] create`, `[vm|vmss] identity assign`, et `[vm|vmss] identity remove` pour sortir les identités des utilisateurs au format de dictionnaire</span><span class="sxs-lookup"><span data-stu-id="93d0e-218">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="93d0e-219">18 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="93d0e-219">July 18, 2018</span></span>

<span data-ttu-id="93d0e-220">Version 2.0.42</span><span class="sxs-lookup"><span data-stu-id="93d0e-220">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="93d0e-221">Principal</span><span class="sxs-lookup"><span data-stu-id="93d0e-221">Core</span></span>

* <span data-ttu-id="93d0e-222">Ajout de la prise en charge de la connexion basée sur le navigateur dans la fenêtre d’interpréteur de commandes Windows pour Linux</span><span class="sxs-lookup"><span data-stu-id="93d0e-222">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="93d0e-223">Ajout de l’indicateur `--force-string` pour toutes les commandes de mise à jour générique</span><span class="sxs-lookup"><span data-stu-id="93d0e-223">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="93d0e-224">[CHANGEMENT CASSANT] Modification des commandes « d’affichage » pour connecter le message d’erreur et échec avec un code de sortie de 3 sur une ressource manquante</span><span class="sxs-lookup"><span data-stu-id="93d0e-224">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="93d0e-225">ACR</span><span class="sxs-lookup"><span data-stu-id="93d0e-225">ACR</span></span>

* <span data-ttu-id="93d0e-226">[CHANGEMENT CASSANT] Mise à jour de « --no-push » vers un indicateur pur dans la commande « ACR Build »</span><span class="sxs-lookup"><span data-stu-id="93d0e-226">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="93d0e-227">Ajout des commandes `show` et `update` sous le groupe `acr repository`</span><span class="sxs-lookup"><span data-stu-id="93d0e-227">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="93d0e-228">Ajout de l’indicateur `--detail` à `show-manifests` et `show-tags` pour afficher des informations plus détaillées</span><span class="sxs-lookup"><span data-stu-id="93d0e-228">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="93d0e-229">Ajout du paramètre `--image` pour prendre en charge l’obtention des détails de build ou des journaux par une image</span><span class="sxs-lookup"><span data-stu-id="93d0e-229">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="93d0e-230">ACS</span><span class="sxs-lookup"><span data-stu-id="93d0e-230">ACS</span></span>

* <span data-ttu-id="93d0e-231">Modification de `az aks create` en sortie d’erreur si `--max-pods` est inférieur à 5</span><span class="sxs-lookup"><span data-stu-id="93d0e-231">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="93d0e-232">AppService</span><span class="sxs-lookup"><span data-stu-id="93d0e-232">AppService</span></span>

* <span data-ttu-id="93d0e-233">Ajout de la prise en charge pour les références (SKU) PremiumV2</span><span class="sxs-lookup"><span data-stu-id="93d0e-233">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="93d0e-234">Batch</span><span class="sxs-lookup"><span data-stu-id="93d0e-234">Batch</span></span>

* <span data-ttu-id="93d0e-235">Correction d’un bogue relatif à l’utilisation des informations d’identification de jeton dans le mode Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="93d0e-235">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="93d0e-236">Modification de l’entrée JSON pour respecter la casse</span><span class="sxs-lookup"><span data-stu-id="93d0e-236">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="93d0e-237">Batch AI</span><span class="sxs-lookup"><span data-stu-id="93d0e-237">Batch AI</span></span>

* <span data-ttu-id="93d0e-238">Correction de la commande `az batchai job exec`</span><span class="sxs-lookup"><span data-stu-id="93d0e-238">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="93d0e-239">Conteneur</span><span class="sxs-lookup"><span data-stu-id="93d0e-239">Container</span></span>

* <span data-ttu-id="93d0e-240">Suppression des exigences pour le nom d’utilisateur et le mot de passe pour les registres non dockerhub</span><span class="sxs-lookup"><span data-stu-id="93d0e-240">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="93d0e-241">Correction de l’erreur lors de la création de groupes de conteneur à partir du fichier yaml</span><span class="sxs-lookup"><span data-stu-id="93d0e-241">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="93d0e-242">Réseau</span><span class="sxs-lookup"><span data-stu-id="93d0e-242">Network</span></span>

* <span data-ttu-id="93d0e-243">Ajout de la prise en charge de `--no-wait` pour `network nic [create|update|delete]`</span><span class="sxs-lookup"><span data-stu-id="93d0e-243">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="93d0e-244">Ajout de `network nic wait`</span><span class="sxs-lookup"><span data-stu-id="93d0e-244">Added `network nic wait`</span></span>
* <span data-ttu-id="93d0e-245">Argument `--ids` déconseillé pour `network vnet [subnet|peering] list`</span><span class="sxs-lookup"><span data-stu-id="93d0e-245">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="93d0e-246">Ajout de l’indicateur `--include-default` pour inclure les règles de sécurité par défaut dans la sortie de `network nsg rule list`</span><span class="sxs-lookup"><span data-stu-id="93d0e-246">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="93d0e-247">Ressource</span><span class="sxs-lookup"><span data-stu-id="93d0e-247">Resource</span></span>

* <span data-ttu-id="93d0e-248">Ajout de la prise en charge de `--no-wait` pour `group deployment delete`</span><span class="sxs-lookup"><span data-stu-id="93d0e-248">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="93d0e-249">Ajout de la prise en charge de `--no-wait` pour `deployment delete`</span><span class="sxs-lookup"><span data-stu-id="93d0e-249">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="93d0e-250">Ajout de la commande `deployment wait`</span><span class="sxs-lookup"><span data-stu-id="93d0e-250">Added `deployment wait` command</span></span>
* <span data-ttu-id="93d0e-251">Résolution du problème qui causait l’affichage par erreur des commandes `az deployment` du niveau de l’abonnement pour le profil 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="93d0e-251">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="93d0e-252">SQL</span><span class="sxs-lookup"><span data-stu-id="93d0e-252">SQL</span></span>

* <span data-ttu-id="93d0e-253">Résolution de l’erreur « Le nom du groupe de ressources fourni ne correspond pas au nom de l’URL » lors de la spécification du nom du pool élastique pour les commandes `sql db copy` et `sql db replica create`</span><span class="sxs-lookup"><span data-stu-id="93d0e-253">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="93d0e-254">Autoriser la configuration de SQL Server par défaut en exécutant `az configure --defaults sql-server=<name>`</span><span class="sxs-lookup"><span data-stu-id="93d0e-254">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="93d0e-255">Implémentation de formateurs de table pour les commandes `sql server`, `sql server firewall-rule`, `sql list-usages` et `sql show-usage`</span><span class="sxs-lookup"><span data-stu-id="93d0e-255">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="93d0e-256">Stockage</span><span class="sxs-lookup"><span data-stu-id="93d0e-256">Storage</span></span>

* <span data-ttu-id="93d0e-257">Ajout de la propriété `pageRanges` à la sortie `storage blob show` qui sera renseignée pour les objets blob de pages</span><span class="sxs-lookup"><span data-stu-id="93d0e-257">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="93d0e-258">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="93d0e-258">VM</span></span>

* <span data-ttu-id="93d0e-259">[CHANGEMENT CASSANT] Modification de `vmss create` pour utiliser `Standard_DS1_v2` comme taille d’instance par défaut</span><span class="sxs-lookup"><span data-stu-id="93d0e-259">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="93d0e-260">Ajout de la prise en charge de `--no-wait` pour `vm extension [set|delete]` et `vmss extension [set|delete]`</span><span class="sxs-lookup"><span data-stu-id="93d0e-260">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="93d0e-261">Ajout de `vm extension wait`</span><span class="sxs-lookup"><span data-stu-id="93d0e-261">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="93d0e-262">3 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="93d0e-262">July 3, 2018</span></span>

<span data-ttu-id="93d0e-263">Version 2.0.41</span><span class="sxs-lookup"><span data-stu-id="93d0e-263">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="93d0e-264">AKS</span><span class="sxs-lookup"><span data-stu-id="93d0e-264">AKS</span></span>

* <span data-ttu-id="93d0e-265">Modification de la surveillance pour utiliser l’ID d’abonnement</span><span class="sxs-lookup"><span data-stu-id="93d0e-265">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="93d0e-266">3 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="93d0e-266">July 3, 2018</span></span>

<span data-ttu-id="93d0e-267">Version 2.0.40</span><span class="sxs-lookup"><span data-stu-id="93d0e-267">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="93d0e-268">Principal</span><span class="sxs-lookup"><span data-stu-id="93d0e-268">Core</span></span>

* <span data-ttu-id="93d0e-269">Ajout d’un nouveau flux de code d’autorisation pour une connexion interactive</span><span class="sxs-lookup"><span data-stu-id="93d0e-269">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="93d0e-270">ACR</span><span class="sxs-lookup"><span data-stu-id="93d0e-270">ACR</span></span>

* <span data-ttu-id="93d0e-271">Ajout de l’interrogation de l’état du build</span><span class="sxs-lookup"><span data-stu-id="93d0e-271">Added polling build status</span></span>
* <span data-ttu-id="93d0e-272">Ajout de la prise en charge des valeurs d’énumération ne respectant pas la casse</span><span class="sxs-lookup"><span data-stu-id="93d0e-272">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="93d0e-273">Ajout des paramètres `--top` et `--orderby` pour `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="93d0e-273">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="93d0e-274">ACS</span><span class="sxs-lookup"><span data-stu-id="93d0e-274">ACS</span></span>

* <span data-ttu-id="93d0e-275">[CHANGEMENT CASSANT] Active le contrôle d’accès en fonction du rôle Kubernetes par défaut</span><span class="sxs-lookup"><span data-stu-id="93d0e-275">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="93d0e-276">Ajout de l’argument `--disable-rbac` et dépréciation de `--enable-rbac` dans la mesure où il s’agit actuellement de la valeur par défaut</span><span class="sxs-lookup"><span data-stu-id="93d0e-276">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="93d0e-277">Mise à jour des options de la commande `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="93d0e-277">Updated options for `aks browse` command.</span></span> <span data-ttu-id="93d0e-278">Ajout de la prise en charge de `--listen-port`</span><span class="sxs-lookup"><span data-stu-id="93d0e-278">Added `--listen-port` support</span></span>
* <span data-ttu-id="93d0e-279">Mise à jour du package de graphique Helm par défaut pour la commande `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="93d0e-279">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="93d0e-280">Use virtual-kubelet-for-aks-latest.tgz</span><span class="sxs-lookup"><span data-stu-id="93d0e-280">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="93d0e-281">Ajout des commandes `aks enable-addons` et `aks disable-addons` pour mettre à jour un cluster existant</span><span class="sxs-lookup"><span data-stu-id="93d0e-281">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="93d0e-282">AppService</span><span class="sxs-lookup"><span data-stu-id="93d0e-282">AppService</span></span>

* <span data-ttu-id="93d0e-283">Ajout de la prise en charge de la désactivation d’identité via `webapp identity remove`</span><span class="sxs-lookup"><span data-stu-id="93d0e-283">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="93d0e-284">Suppression de la balise `preview` pour la fonctionnalité Identité</span><span class="sxs-lookup"><span data-stu-id="93d0e-284">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="93d0e-285">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="93d0e-285">Backup</span></span>

* <span data-ttu-id="93d0e-286">Mise à jour de la définition du module</span><span class="sxs-lookup"><span data-stu-id="93d0e-286">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="93d0e-287">Batch AI</span><span class="sxs-lookup"><span data-stu-id="93d0e-287">BatchAI</span></span>

* <span data-ttu-id="93d0e-288">Correction de la sortie de table pour les commandes `batchai cluster node list` et `batchai job node list`</span><span class="sxs-lookup"><span data-stu-id="93d0e-288">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="93d0e-289">Cloud</span><span class="sxs-lookup"><span data-stu-id="93d0e-289">Cloud</span></span>

* <span data-ttu-id="93d0e-290">Ajout du suffixe de serveur `acr login` à la configuration du cloud</span><span class="sxs-lookup"><span data-stu-id="93d0e-290">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="93d0e-291">Conteneur</span><span class="sxs-lookup"><span data-stu-id="93d0e-291">Container</span></span>

* <span data-ttu-id="93d0e-292">Modification de `container create` sur valeur par défaut en opération à long terme</span><span class="sxs-lookup"><span data-stu-id="93d0e-292">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="93d0e-293">Ajout des paramètres Log Analytics `--log-analytics-workspace` et `--log-analytics-workspace-key`</span><span class="sxs-lookup"><span data-stu-id="93d0e-293">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="93d0e-294">Ajout du paramètre `--protocol` pour spécifier le protocole réseau à utiliser</span><span class="sxs-lookup"><span data-stu-id="93d0e-294">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="93d0e-295">Extension</span><span class="sxs-lookup"><span data-stu-id="93d0e-295">Extension</span></span>

* <span data-ttu-id="93d0e-296">Modification de `extension list-available` pour afficher uniquement les extensions compatibles avec la version CLI</span><span class="sxs-lookup"><span data-stu-id="93d0e-296">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="93d0e-297">Réseau</span><span class="sxs-lookup"><span data-stu-id="93d0e-297">Network</span></span>

* <span data-ttu-id="93d0e-298">Résolution du problème où les types d’enregistrement étaient sensibles à la casse pour ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="93d0e-298">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="93d0e-299">Rdbms</span><span class="sxs-lookup"><span data-stu-id="93d0e-299">Rdbms</span></span>

* <span data-ttu-id="93d0e-300">Ajout des commandes `[postgres|myql] server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="93d0e-300">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="93d0e-301">Ressource</span><span class="sxs-lookup"><span data-stu-id="93d0e-301">Resource</span></span>

* <span data-ttu-id="93d0e-302">Ajout d’un nouveau groupe d’opérations `deployment`</span><span class="sxs-lookup"><span data-stu-id="93d0e-302">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="93d0e-303">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="93d0e-303">VM</span></span>

* <span data-ttu-id="93d0e-304">Ajout de la prise en charge de la suppression de l’identité affectée au système</span><span class="sxs-lookup"><span data-stu-id="93d0e-304">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="93d0e-305">25 juin 2018</span><span class="sxs-lookup"><span data-stu-id="93d0e-305">June 25, 2018</span></span>

<span data-ttu-id="93d0e-306">Version 2.0.39</span><span class="sxs-lookup"><span data-stu-id="93d0e-306">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="93d0e-307">Interface de ligne de commande</span><span class="sxs-lookup"><span data-stu-id="93d0e-307">CLI</span></span>

* <span data-ttu-id="93d0e-308">Mise à jour de la suppression du fichier dans le programme d’installation MSI pour résoudre le problème d’installation de l’extension</span><span class="sxs-lookup"><span data-stu-id="93d0e-308">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="93d0e-309">19 juin 2018</span><span class="sxs-lookup"><span data-stu-id="93d0e-309">June 19, 2018</span></span>

<span data-ttu-id="93d0e-310">Version 2.0.38</span><span class="sxs-lookup"><span data-stu-id="93d0e-310">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="93d0e-311">Principal</span><span class="sxs-lookup"><span data-stu-id="93d0e-311">Core</span></span>

* <span data-ttu-id="93d0e-312">Ajout de la prise en charge globale de `--subscription` pour la plupart des commandes</span><span class="sxs-lookup"><span data-stu-id="93d0e-312">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="93d0e-313">ACR</span><span class="sxs-lookup"><span data-stu-id="93d0e-313">ACR</span></span>

* <span data-ttu-id="93d0e-314">Ajout de `azure-storage-blob` comme dépendance</span><span class="sxs-lookup"><span data-stu-id="93d0e-314">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="93d0e-315">Modification de la configuration de l’UC par défaut avec `acr build-task create` pour utiliser 2 cœurs</span><span class="sxs-lookup"><span data-stu-id="93d0e-315">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="93d0e-316">ACS</span><span class="sxs-lookup"><span data-stu-id="93d0e-316">ACS</span></span>

* <span data-ttu-id="93d0e-317">Mise à jour des options de la commande `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="93d0e-317">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="93d0e-318">Ajout de la prise en charge de `--update`</span><span class="sxs-lookup"><span data-stu-id="93d0e-318">Added `--update` support</span></span>
* <span data-ttu-id="93d0e-319">Modification de `aks get-credentials --admin` pour ne pas remplacer le contexte utilisateur dans `$HOME/.kube/config`</span><span class="sxs-lookup"><span data-stu-id="93d0e-319">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="93d0e-320">Exposition de la propriété en lecture seule `nodeResourceGroup` sur les clusters managés</span><span class="sxs-lookup"><span data-stu-id="93d0e-320">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="93d0e-321">Correction de l’erreur de commande `acs browse`</span><span class="sxs-lookup"><span data-stu-id="93d0e-321">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="93d0e-322">`--connector-name` rendu facultatif pour `aks install-connector`, `aks upgrade-connector` et `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="93d0e-322">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="93d0e-323">Ajout de nouvelles régions Azure Container Instance pour `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="93d0e-323">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="93d0e-324">Ajout de l’emplacement normalisé dans le nom de mise en production Helm et le nom du nœud pour `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="93d0e-324">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="93d0e-325">AppService</span><span class="sxs-lookup"><span data-stu-id="93d0e-325">AppService</span></span>

* <span data-ttu-id="93d0e-326">Ajout de la prise en charge des versions urllib plus récentes</span><span class="sxs-lookup"><span data-stu-id="93d0e-326">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="93d0e-327">Ajout de la prise en charge pour `functionapp create` pour utiliser un plan App Service à partir de groupes de ressources externes</span><span class="sxs-lookup"><span data-stu-id="93d0e-327">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="93d0e-328">Batch</span><span class="sxs-lookup"><span data-stu-id="93d0e-328">Batch</span></span>

* <span data-ttu-id="93d0e-329">Suppression de la dépendance `azure-batch-extensions`</span><span class="sxs-lookup"><span data-stu-id="93d0e-329">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="93d0e-330">Batch AI</span><span class="sxs-lookup"><span data-stu-id="93d0e-330">Batch AI</span></span>

* <span data-ttu-id="93d0e-331">Ajout de la prise en charge des espaces de travail.</span><span class="sxs-lookup"><span data-stu-id="93d0e-331">Added support for workspaces.</span></span> <span data-ttu-id="93d0e-332">Les espaces de travail permettent de regrouper les clusters, serveurs de fichiers et expériences, supprimant la limitation du nombre de ressources qui peuvent être créées</span><span class="sxs-lookup"><span data-stu-id="93d0e-332">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="93d0e-333">Ajout de la prise en charge des expériences.</span><span class="sxs-lookup"><span data-stu-id="93d0e-333">Added support for experiments.</span></span> <span data-ttu-id="93d0e-334">Les expériences permettent de regrouper les tâches dans des collections, supprimant la limitation du nombre de tâches créées</span><span class="sxs-lookup"><span data-stu-id="93d0e-334">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="93d0e-335">Ajout de la prise en charge pour configurer `/dev/shm` pour les travaux en cours d’exécution dans un conteneur docker</span><span class="sxs-lookup"><span data-stu-id="93d0e-335">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="93d0e-336">Ajout des commandes `batchai cluster node exec` et `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="93d0e-336">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="93d0e-337">Ces commandes permettent d’exécuter des commandes directement sur les nœuds et fournissent la fonctionnalité de réacheminement de port.</span><span class="sxs-lookup"><span data-stu-id="93d0e-337">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="93d0e-338">Ajout de la prise en charge des commandes `--ids` et `batchai`</span><span class="sxs-lookup"><span data-stu-id="93d0e-338">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="93d0e-339">[CHANGEMENT CASSANT] Tous les clusters et serveurs de fichiers doivent être créés dans des espaces de travail</span><span class="sxs-lookup"><span data-stu-id="93d0e-339">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="93d0e-340">[CHANGEMENT CASSANT] Les travaux doivent être créés dans des expériences</span><span class="sxs-lookup"><span data-stu-id="93d0e-340">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="93d0e-341">[CHANGEMENT CASSANT] Suppression de `--nfs-resource-group` des commandes `cluster create` et `job create`.</span><span class="sxs-lookup"><span data-stu-id="93d0e-341">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="93d0e-342">Pour monter un NFS appartenant à un autre espace de travail/groupe de ressources, indiquez l’ID ARM du serveur de fichiers via l’option `--nfs`</span><span class="sxs-lookup"><span data-stu-id="93d0e-342">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="93d0e-343">[CHANGEMENT CASSANT] Suppression de `--cluster-resource-group` de la commande `job create`.</span><span class="sxs-lookup"><span data-stu-id="93d0e-343">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="93d0e-344">Pour soumettre un travail sur un cluster appartenant à un autre espace de travail/groupe de ressources, indiquez l’ID ARM du cluster via l’option `--cluster`</span><span class="sxs-lookup"><span data-stu-id="93d0e-344">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="93d0e-345">[CHANGEMENT CASSANT] Suppression de l’attribut `location` des travaux, clusters et serveurs de fichiers.</span><span class="sxs-lookup"><span data-stu-id="93d0e-345">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="93d0e-346">L’emplacement est maintenant un attribut d’espace de travail.</span><span class="sxs-lookup"><span data-stu-id="93d0e-346">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="93d0e-347">[CHANGEMENT CASSANT] Suppression de `--location` des commandes `job create`, `cluster create` et `file-server create`</span><span class="sxs-lookup"><span data-stu-id="93d0e-347">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="93d0e-348">[CHANGEMENT CASSANT] Modification des noms des options courtes pour rendre l’interface plus cohérente :</span><span class="sxs-lookup"><span data-stu-id="93d0e-348">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
 - <span data-ttu-id="93d0e-349">[`--config`, `-c`] renommé en [`--config-file`, `-f`]</span><span class="sxs-lookup"><span data-stu-id="93d0e-349">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
 - <span data-ttu-id="93d0e-350">[`--cluster`, `-r`] renommé en [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="93d0e-350">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
 - <span data-ttu-id="93d0e-351">[`--cluster`, `-n`] renommé en [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="93d0e-351">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
 - <span data-ttu-id="93d0e-352">[`--job`, `-n`] renommé en [`--job`, `-j`]</span><span class="sxs-lookup"><span data-stu-id="93d0e-352">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="93d0e-353">Cartes</span><span class="sxs-lookup"><span data-stu-id="93d0e-353">Maps</span></span>

* <span data-ttu-id="93d0e-354">[CHANGEMENT CASSANT] Modification de `maps account create` pour accepter les Conditions d’utilisation, soit par l’invite interactive ou par l’indicateur `--accept-tos`</span><span class="sxs-lookup"><span data-stu-id="93d0e-354">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="93d0e-355">Réseau</span><span class="sxs-lookup"><span data-stu-id="93d0e-355">Network</span></span>

* <span data-ttu-id="93d0e-356">Ajout de la prise en charge de `https` à `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="93d0e-356">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="93d0e-357">Correction d’un problème où `--endpoint-status` était sensible à la casse.</span><span class="sxs-lookup"><span data-stu-id="93d0e-357">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="93d0e-358">#6502</span><span class="sxs-lookup"><span data-stu-id="93d0e-358">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="93d0e-359">Réservations</span><span class="sxs-lookup"><span data-stu-id="93d0e-359">Reservations</span></span>

* <span data-ttu-id="93d0e-360">[CHANGEMENT CASSANT] Ajout du paramètre obligatoire `ReservedResourceType` à `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="93d0e-360">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="93d0e-361">Ajout du paramètre `Location` à `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="93d0e-361">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="93d0e-362">[CHANGEMENT CASSANT] Suppression de `kind` de `ReservationProperties`</span><span class="sxs-lookup"><span data-stu-id="93d0e-362">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="93d0e-363">[CHANGEMENT CASSANT] `capabilities` renommé en `sku_properties` dans `Catalog`</span><span class="sxs-lookup"><span data-stu-id="93d0e-363">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="93d0e-364">[CHANGEMENT CASSANT] Suppression des propriétés `size` et `tier` de `Catalog`</span><span class="sxs-lookup"><span data-stu-id="93d0e-364">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="93d0e-365">Ajout du paramètre `InstanceFlexibility` à `reservations reservation update`</span><span class="sxs-lookup"><span data-stu-id="93d0e-365">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="93d0e-366">Rôle</span><span class="sxs-lookup"><span data-stu-id="93d0e-366">Role</span></span>

* <span data-ttu-id="93d0e-367">Amélioration de la gestion des erreurs</span><span class="sxs-lookup"><span data-stu-id="93d0e-367">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="93d0e-368">SQL</span><span class="sxs-lookup"><span data-stu-id="93d0e-368">SQL</span></span>

* <span data-ttu-id="93d0e-369">Correction de l’erreur déroutante lors de l’exécution de `az sql db list-editions` pour un emplacement qui n’est pas disponible pour votre abonnement</span><span class="sxs-lookup"><span data-stu-id="93d0e-369">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="93d0e-370">Stockage</span><span class="sxs-lookup"><span data-stu-id="93d0e-370">Storage</span></span>

* <span data-ttu-id="93d0e-371">Modification de la sortie de table pour que `storage blob download` soit plus lisible</span><span class="sxs-lookup"><span data-stu-id="93d0e-371">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="93d0e-372">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="93d0e-372">VM</span></span>

* <span data-ttu-id="93d0e-373">Amélioration de la vérification de la taille de la machine virtuelle pour la prise en charge de la mise en réseau accélérée dans `vm create`</span><span class="sxs-lookup"><span data-stu-id="93d0e-373">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="93d0e-374">Ajout d’un avertissement pour `vmss create` indiquant que la taille de la machine virtuelle par défaut va passer de `Standard_D1_v2` à `Standard_DS1_v2`</span><span class="sxs-lookup"><span data-stu-id="93d0e-374">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="93d0e-375">Ajout de `--force-update` à `[vm|vmss] extension set` pour mettre à jour l’extension, même lorsque la configuration n’a pas changé</span><span class="sxs-lookup"><span data-stu-id="93d0e-375">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="93d0e-376">13 juin 2018</span><span class="sxs-lookup"><span data-stu-id="93d0e-376">June 13, 2018</span></span>

<span data-ttu-id="93d0e-377">Version 2.0.37</span><span class="sxs-lookup"><span data-stu-id="93d0e-377">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="93d0e-378">Principal</span><span class="sxs-lookup"><span data-stu-id="93d0e-378">Core</span></span>

* <span data-ttu-id="93d0e-379">Amélioration de la télémétrie interactive</span><span class="sxs-lookup"><span data-stu-id="93d0e-379">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="93d0e-380">13 juin 2018</span><span class="sxs-lookup"><span data-stu-id="93d0e-380">June 13, 2018</span></span>

<span data-ttu-id="93d0e-381">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="93d0e-381">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="93d0e-382">AKS</span><span class="sxs-lookup"><span data-stu-id="93d0e-382">AKS</span></span>

* <span data-ttu-id="93d0e-383">Ajout d’options réseau avancées à `aks create`</span><span class="sxs-lookup"><span data-stu-id="93d0e-383">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="93d0e-384">Ajout d’arguments à `aks create` pour permettre la surveillance et le routage HTTP</span><span class="sxs-lookup"><span data-stu-id="93d0e-384">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="93d0e-385">Ajout de l’argument `--no-ssh-key` à `aks create`</span><span class="sxs-lookup"><span data-stu-id="93d0e-385">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="93d0e-386">Ajout de l’argument `--enable-rbac` à `aks create`</span><span class="sxs-lookup"><span data-stu-id="93d0e-386">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="93d0e-387">[PRÉVERSION] Ajout de la prise en charge pour l’authentification basée sur Azure Active Directory à `aks create`</span><span class="sxs-lookup"><span data-stu-id="93d0e-387">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="93d0e-388">AppService</span><span class="sxs-lookup"><span data-stu-id="93d0e-388">AppService</span></span>

* <span data-ttu-id="93d0e-389">Résolution d’un problème lié à des versions urllib incompatibles</span><span class="sxs-lookup"><span data-stu-id="93d0e-389">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="93d0e-390">5 juin 2018</span><span class="sxs-lookup"><span data-stu-id="93d0e-390">June 5, 2018</span></span>

<span data-ttu-id="93d0e-391">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="93d0e-391">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="93d0e-392">Interactive</span><span class="sxs-lookup"><span data-stu-id="93d0e-392">Interactive</span></span>

* <span data-ttu-id="93d0e-393">Ajout de limites aux dépendances du mode interactif</span><span class="sxs-lookup"><span data-stu-id="93d0e-393">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="93d0e-394">5 juin 2018</span><span class="sxs-lookup"><span data-stu-id="93d0e-394">June 5, 2018</span></span>

<span data-ttu-id="93d0e-395">Version 2.0.34</span><span class="sxs-lookup"><span data-stu-id="93d0e-395">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="93d0e-396">Principal</span><span class="sxs-lookup"><span data-stu-id="93d0e-396">Core</span></span>

* <span data-ttu-id="93d0e-397">Prise en charge supplémentaire pour les références de ressources inter-client</span><span class="sxs-lookup"><span data-stu-id="93d0e-397">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="93d0e-398">Amélioration de la fiabilité de téléchargement des données de télémétrie</span><span class="sxs-lookup"><span data-stu-id="93d0e-398">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="93d0e-399">ACR</span><span class="sxs-lookup"><span data-stu-id="93d0e-399">ACR</span></span>

* <span data-ttu-id="93d0e-400">Prise en charge supplémentaire pour VSTS en tant qu’emplacement source distant</span><span class="sxs-lookup"><span data-stu-id="93d0e-400">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="93d0e-401">Ajout de la commande `acr import`</span><span class="sxs-lookup"><span data-stu-id="93d0e-401">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="93d0e-402">AKS</span><span class="sxs-lookup"><span data-stu-id="93d0e-402">AKS</span></span>

* <span data-ttu-id="93d0e-403">`aks get-credentials` a été modifié pour créer le fichier de configuration kube avec des autorisations de système de fichiers plus sécurisées</span><span class="sxs-lookup"><span data-stu-id="93d0e-403">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="93d0e-404">Batch</span><span class="sxs-lookup"><span data-stu-id="93d0e-404">Batch</span></span>

* <span data-ttu-id="93d0e-405">Résolution du bogue concernant la mise en forme dans la table de liste de pool [[problème #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="93d0e-405">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="93d0e-406">IOT</span><span class="sxs-lookup"><span data-stu-id="93d0e-406">IOT</span></span>

* <span data-ttu-id="93d0e-407">Prise en charge ajoutée pour la création de IoT Hubs de niveau de base</span><span class="sxs-lookup"><span data-stu-id="93d0e-407">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="93d0e-408">Réseau</span><span class="sxs-lookup"><span data-stu-id="93d0e-408">Network</span></span>

* <span data-ttu-id="93d0e-409">`network vnet peering` amélioré</span><span class="sxs-lookup"><span data-stu-id="93d0e-409">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="93d0e-410">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="93d0e-410">Policy Insights</span></span>

* <span data-ttu-id="93d0e-411">Version initiale</span><span class="sxs-lookup"><span data-stu-id="93d0e-411">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="93d0e-412">ARM</span><span class="sxs-lookup"><span data-stu-id="93d0e-412">ARM</span></span>

* <span data-ttu-id="93d0e-413">Ajout des commandes `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="93d0e-413">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="93d0e-414">SQL</span><span class="sxs-lookup"><span data-stu-id="93d0e-414">SQL</span></span>

* <span data-ttu-id="93d0e-415">Ajout de nouvelles commandes d’instance gérée :</span><span class="sxs-lookup"><span data-stu-id="93d0e-415">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="93d0e-416">Ajout de nouvelles commandes de base de données gérée :</span><span class="sxs-lookup"><span data-stu-id="93d0e-416">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="93d0e-417">Stockage</span><span class="sxs-lookup"><span data-stu-id="93d0e-417">Storage</span></span>

* <span data-ttu-id="93d0e-418">Ajout de types MimeTypes supplémentaires pour les formats json et javascript pour être déduit à partir des extensions de fichier</span><span class="sxs-lookup"><span data-stu-id="93d0e-418">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="93d0e-419">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="93d0e-419">VM</span></span>

* <span data-ttu-id="93d0e-420">`vm list-skus` a été modifié pour utiliser des colonnes corrigées et ajouter l’avertissement que `Tier` et `Size` seront supprimés</span><span class="sxs-lookup"><span data-stu-id="93d0e-420">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="93d0e-421">Ajout de l’option `--accelerated-networking` à `vm create`</span><span class="sxs-lookup"><span data-stu-id="93d0e-421">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="93d0e-422">Ajout de `--tags` à `identity create`</span><span class="sxs-lookup"><span data-stu-id="93d0e-422">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="93d0e-423">22 mai 2018</span><span class="sxs-lookup"><span data-stu-id="93d0e-423">May 22, 2018</span></span>

<span data-ttu-id="93d0e-424">Version 2.0.33</span><span class="sxs-lookup"><span data-stu-id="93d0e-424">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="93d0e-425">Principal</span><span class="sxs-lookup"><span data-stu-id="93d0e-425">Core</span></span>

* <span data-ttu-id="93d0e-426">Ajout de la prise en charge pour le développement de `@` dans les noms de fichiers</span><span class="sxs-lookup"><span data-stu-id="93d0e-426">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="93d0e-427">ACS</span><span class="sxs-lookup"><span data-stu-id="93d0e-427">ACS</span></span>

* <span data-ttu-id="93d0e-428">Ajout de nouvelles commandes Dev Spaces `aks use-dev-spaces` et `aks remove-dev-spaces`</span><span class="sxs-lookup"><span data-stu-id="93d0e-428">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="93d0e-429">Faute de frappe corrigée dans un message d’aide</span><span class="sxs-lookup"><span data-stu-id="93d0e-429">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="93d0e-430">AppService</span><span class="sxs-lookup"><span data-stu-id="93d0e-430">AppService</span></span>

* <span data-ttu-id="93d0e-431">Amélioration des commandes de mise à jour générique</span><span class="sxs-lookup"><span data-stu-id="93d0e-431">Improved generic update commands</span></span>
* <span data-ttu-id="93d0e-432">Ajout de la prise en charge asynchrone pour `webapp deployment source config-zip`</span><span class="sxs-lookup"><span data-stu-id="93d0e-432">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="93d0e-433">Conteneur</span><span class="sxs-lookup"><span data-stu-id="93d0e-433">Container</span></span>

* <span data-ttu-id="93d0e-434">Prise en charge ajoutée pour l’exportation d’un groupe de conteneurs au format yaml</span><span class="sxs-lookup"><span data-stu-id="93d0e-434">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="93d0e-435">Prise en charge ajoutée pour l’utilisation d’un fichier yaml afin de créer/mettre à jour un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="93d0e-435">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="93d0e-436">Extension</span><span class="sxs-lookup"><span data-stu-id="93d0e-436">Extension</span></span>

* <span data-ttu-id="93d0e-437">Amélioration de la suppression des extensions</span><span class="sxs-lookup"><span data-stu-id="93d0e-437">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="93d0e-438">Interactive</span><span class="sxs-lookup"><span data-stu-id="93d0e-438">Interactive</span></span>

* <span data-ttu-id="93d0e-439">La journalisation a été modifiée pour désactiver l’analyseur pour les saisies semi-automatiques</span><span class="sxs-lookup"><span data-stu-id="93d0e-439">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="93d0e-440">Gestion améliorée des caches d’aide incorrects</span><span class="sxs-lookup"><span data-stu-id="93d0e-440">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="93d0e-441">KeyVault</span><span class="sxs-lookup"><span data-stu-id="93d0e-441">KeyVault</span></span>

* <span data-ttu-id="93d0e-442">Commandes keyvault corrigées afin de fonctionner dans Cloud Shell ou dans des machines virtuelles avec l’identité</span><span class="sxs-lookup"><span data-stu-id="93d0e-442">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="93d0e-443">Réseau</span><span class="sxs-lookup"><span data-stu-id="93d0e-443">Network</span></span>

* <span data-ttu-id="93d0e-444">Résolution d’un problème où `network watcher show-topology` ne fonctionnait pas avec le nom de réseau virtuel et/ou de sous-réseau [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="93d0e-444">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="93d0e-445">Correction d’un problème où certaines commandes `network watcher` revendiquaient que Network Watcher n’était pas activé pour certaines régions alors qu’il l’était [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="93d0e-445">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="93d0e-446">SQL</span><span class="sxs-lookup"><span data-stu-id="93d0e-446">SQL</span></span>

* <span data-ttu-id="93d0e-447">[CHANGEMENT CASSANT] Objets de réponse retournés modifiés à partir des commandes `db` et `dw`</span><span class="sxs-lookup"><span data-stu-id="93d0e-447">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="93d0e-448">Propriété `serviceLevelObjective` renommée en `currentServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="93d0e-448">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="93d0e-449">Suppression des propriétés `currentServiceObjectiveId` et `requestedServiceObjectiveId`</span><span class="sxs-lookup"><span data-stu-id="93d0e-449">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="93d0e-450">Propriété `maxSizeBytes` modifiée en valeur entière au lieu d’une chaîne</span><span class="sxs-lookup"><span data-stu-id="93d0e-450">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="93d0e-451">[CHANGEMENT CASSANT] Les propriétés `db` et `dw` suivantes ont été modifiées pour être en lecture seule :</span><span class="sxs-lookup"><span data-stu-id="93d0e-451">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="93d0e-452">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="93d0e-452">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="93d0e-453">Pour mettre à jour, utilisez le paramètre `--service-objective` ou définissez la propriété `sku.name`</span><span class="sxs-lookup"><span data-stu-id="93d0e-453">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="93d0e-454">`edition`.</span><span class="sxs-lookup"><span data-stu-id="93d0e-454">`edition`.</span></span> <span data-ttu-id="93d0e-455">Pour mettre à jour, utilisez le paramètre `--edition` ou définissez la propriété `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="93d0e-455">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="93d0e-456">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="93d0e-456">`elasticPoolName`.</span></span> <span data-ttu-id="93d0e-457">Pour mettre à jour, utilisez le paramètre `--elastic-pool` ou définissez la propriété `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="93d0e-457">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="93d0e-458">[CHANGEMENT CASSANT] Les propriétés `elastic-pool` suivantes ont été modifiées pour être en lecture seule :</span><span class="sxs-lookup"><span data-stu-id="93d0e-458">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="93d0e-459">`edition`.</span><span class="sxs-lookup"><span data-stu-id="93d0e-459">`edition`.</span></span> <span data-ttu-id="93d0e-460">Pour mettre à jour, utilisez le paramètre `--edition`</span><span class="sxs-lookup"><span data-stu-id="93d0e-460">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="93d0e-461">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="93d0e-461">`dtu`.</span></span> <span data-ttu-id="93d0e-462">Pour mettre à jour, utilisez le paramètre `--capacity`</span><span class="sxs-lookup"><span data-stu-id="93d0e-462">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="93d0e-463">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="93d0e-463">`databaseDtuMin`.</span></span> <span data-ttu-id="93d0e-464">Pour mettre à jour, utilisez le paramètre `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="93d0e-464">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="93d0e-465">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="93d0e-465">`databaseDtuMax`.</span></span> <span data-ttu-id="93d0e-466">Pour mettre à jour, utilisez le paramètre `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="93d0e-466">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="93d0e-467">Ajout des paramètres `--family` et `--capacity` aux commandes `db`, `dw` et `elastic-pool`</span><span class="sxs-lookup"><span data-stu-id="93d0e-467">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="93d0e-468">Ajout de formateurs de table aux commandes `db`, `dw` et `elastic-pool`</span><span class="sxs-lookup"><span data-stu-id="93d0e-468">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="93d0e-469">Stockage</span><span class="sxs-lookup"><span data-stu-id="93d0e-469">Storage</span></span>

* <span data-ttu-id="93d0e-470">Ajout d’un compléteur pour l’argument `--account-name`</span><span class="sxs-lookup"><span data-stu-id="93d0e-470">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="93d0e-471">Correction d’un problème avec `storage entity query`</span><span class="sxs-lookup"><span data-stu-id="93d0e-471">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="93d0e-472">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="93d0e-472">VM</span></span>

* <span data-ttu-id="93d0e-473">[CHANGEMENT CASSANT] Suppression de `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="93d0e-473">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="93d0e-474">La même prise en charge est accessible via `vm update` ou `vm disk attach`</span><span class="sxs-lookup"><span data-stu-id="93d0e-474">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="93d0e-475">Correction de l’image de l’extension efficace dans `[vm|vmss] extension`</span><span class="sxs-lookup"><span data-stu-id="93d0e-475">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="93d0e-476">Ajout de`--boot-diagnostics-storage` à `vm create` pour capturer le journal de démarrage</span><span class="sxs-lookup"><span data-stu-id="93d0e-476">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="93d0e-477">Ajout de `--license-type` à `[vm|vmss] update`</span><span class="sxs-lookup"><span data-stu-id="93d0e-477">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="93d0e-478">7 mai 2018</span><span class="sxs-lookup"><span data-stu-id="93d0e-478">May 7, 2018</span></span>

<span data-ttu-id="93d0e-479">Version 2.0.32</span><span class="sxs-lookup"><span data-stu-id="93d0e-479">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="93d0e-480">Principal</span><span class="sxs-lookup"><span data-stu-id="93d0e-480">Core</span></span>

* <span data-ttu-id="93d0e-481">Correction d’une exception non gérée lors de la récupération des clés secrètes à partir d’un compte de principal de service avec certificat</span><span class="sxs-lookup"><span data-stu-id="93d0e-481">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="93d0e-482">Nouvelle prise en charge limitée pour les arguments positionnels</span><span class="sxs-lookup"><span data-stu-id="93d0e-482">Added limited support for positional arguments</span></span>
* <span data-ttu-id="93d0e-483">Correction d’un problème où `--query` ne pouvait pas être utilisé avec `--ids`.</span><span class="sxs-lookup"><span data-stu-id="93d0e-483">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="93d0e-484">#5591</span><span class="sxs-lookup"><span data-stu-id="93d0e-484">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="93d0e-485">Amélioration des scénarios de redirection à partir des commandes en utilisant `--ids`.</span><span class="sxs-lookup"><span data-stu-id="93d0e-485">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="93d0e-486">Prend en charge `-o tsv` avec une requête spécifiée ou `-o json` sans spécification de requête</span><span class="sxs-lookup"><span data-stu-id="93d0e-486">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="93d0e-487">Ajout de suggestions de commande en cas d’erreur engendrées par des fautes de frappe des utilisateurs dans les commandes</span><span class="sxs-lookup"><span data-stu-id="93d0e-487">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="93d0e-488">Amélioration de l’erreur lorsque les utilisateurs entrent `az ''`</span><span class="sxs-lookup"><span data-stu-id="93d0e-488">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="93d0e-489">Ajout de la prise en charge des types de ressources personnalisés pour les modules et les extensions de commande</span><span class="sxs-lookup"><span data-stu-id="93d0e-489">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="93d0e-490">ACR</span><span class="sxs-lookup"><span data-stu-id="93d0e-490">ACR</span></span>

* <span data-ttu-id="93d0e-491">Ajout de commandes de build de l’ACR</span><span class="sxs-lookup"><span data-stu-id="93d0e-491">Added ACR Build commands</span></span>
* <span data-ttu-id="93d0e-492">Améliorations des messages d’erreur dus aux ressources introuvables</span><span class="sxs-lookup"><span data-stu-id="93d0e-492">Improved resource not found error messages</span></span>
* <span data-ttu-id="93d0e-493">Amélioration des performances de création de ressources et de la gestion des erreurs</span><span class="sxs-lookup"><span data-stu-id="93d0e-493">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="93d0e-494">Amélioration de la connexion ACR dans des consoles non standards et des WSL</span><span class="sxs-lookup"><span data-stu-id="93d0e-494">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="93d0e-495">Amélioration des messages d’erreur dus aux commandes de dépôt</span><span class="sxs-lookup"><span data-stu-id="93d0e-495">Improved repository commands error messages</span></span>
* <span data-ttu-id="93d0e-496">Mise à jour des colonnes de la table et du classement</span><span class="sxs-lookup"><span data-stu-id="93d0e-496">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="93d0e-497">ACS</span><span class="sxs-lookup"><span data-stu-id="93d0e-497">ACS</span></span>

* <span data-ttu-id="93d0e-498">Ajout d’un avertissement indiquant que `az aks` est un service en préversion</span><span class="sxs-lookup"><span data-stu-id="93d0e-498">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="93d0e-499">Résolution du problème d’autorisation dans `aks install-connector` lorsque `--aci-resource-group` n’est pas spécifié</span><span class="sxs-lookup"><span data-stu-id="93d0e-499">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="93d0e-500">AMS</span><span class="sxs-lookup"><span data-stu-id="93d0e-500">AMS</span></span>

* <span data-ttu-id="93d0e-501">Version initiale - Gérer des ressources Azure Media Services</span><span class="sxs-lookup"><span data-stu-id="93d0e-501">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="93d0e-502">AppService</span><span class="sxs-lookup"><span data-stu-id="93d0e-502">Appservice</span></span>

* <span data-ttu-id="93d0e-503">Correction d’un bogue dans `webapp delete` lorsque `--slot` est fourni</span><span class="sxs-lookup"><span data-stu-id="93d0e-503">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="93d0e-504">`--runtime-version` retiré de `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="93d0e-504">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="93d0e-505">Ajout de la prise en charge de min\_tls\_version & https2.0</span><span class="sxs-lookup"><span data-stu-id="93d0e-505">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="93d0e-506">Ajout de la prise en charge pour les multiconteneurs</span><span class="sxs-lookup"><span data-stu-id="93d0e-506">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="93d0e-507">Batch AI</span><span class="sxs-lookup"><span data-stu-id="93d0e-507">Batch AI</span></span>

* <span data-ttu-id="93d0e-508">`batchai create cluster` modifié pour respecter la priorité de machine virtuelle configurée dans le fichier de configuration du cluster</span><span class="sxs-lookup"><span data-stu-id="93d0e-508">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="93d0e-509">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="93d0e-509">Cognitive Services</span></span>

* <span data-ttu-id="93d0e-510">Faute de frappe corrigée dans l’exemple de `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="93d0e-510">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="93d0e-511">Consommation</span><span class="sxs-lookup"><span data-stu-id="93d0e-511">Consumption</span></span>

* <span data-ttu-id="93d0e-512">Ajout de nouvelles commandes pour l’API Budget</span><span class="sxs-lookup"><span data-stu-id="93d0e-512">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="93d0e-513">Conteneur</span><span class="sxs-lookup"><span data-stu-id="93d0e-513">Container</span></span>

* <span data-ttu-id="93d0e-514">Suppression de l’exigence pour `--registry-server` pour `container create` lorsqu’un serveur de registre est inclus dans le nom de l’image</span><span class="sxs-lookup"><span data-stu-id="93d0e-514">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="93d0e-515">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="93d0e-515">Cosmos DB</span></span>

* <span data-ttu-id="93d0e-516">Présentation de la prise en charge d’un réseau virtuel pour Azure CLI - Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="93d0e-516">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="93d0e-517">DMS</span><span class="sxs-lookup"><span data-stu-id="93d0e-517">DMS</span></span>

* <span data-ttu-id="93d0e-518">Version initiale - Ajoute la prise en charge de l’instruction SQL pour le scénario de migration de SQL Azure</span><span class="sxs-lookup"><span data-stu-id="93d0e-518">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="93d0e-519">Extension</span><span class="sxs-lookup"><span data-stu-id="93d0e-519">Extension</span></span>

* <span data-ttu-id="93d0e-520">Correction d’un bogue où les métadonnées d’extension cessaient d’être affichées</span><span class="sxs-lookup"><span data-stu-id="93d0e-520">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="93d0e-521">Interactive</span><span class="sxs-lookup"><span data-stu-id="93d0e-521">Interactive</span></span>

* <span data-ttu-id="93d0e-522">Autorise le fonctionnement de compléments interactifs avec des arguments positionnel</span><span class="sxs-lookup"><span data-stu-id="93d0e-522">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="93d0e-523">Sortie plus conviviale lorsque les utilisateurs entrent \'</span><span class="sxs-lookup"><span data-stu-id="93d0e-523">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="93d0e-524">Achèvements corrigés pour les paramètres sans aide</span><span class="sxs-lookup"><span data-stu-id="93d0e-524">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="93d0e-525">Descriptions corrigées pour les groupes de commandes</span><span class="sxs-lookup"><span data-stu-id="93d0e-525">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="93d0e-526">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="93d0e-526">Lab</span></span>

* <span data-ttu-id="93d0e-527">Régressions corrigées de conversion Knack</span><span class="sxs-lookup"><span data-stu-id="93d0e-527">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="93d0e-528">Réseau</span><span class="sxs-lookup"><span data-stu-id="93d0e-528">Network</span></span>

* <span data-ttu-id="93d0e-529">[CHANGEMENT CASSANT] Suppression du paramètre `--ids` pour :</span><span class="sxs-lookup"><span data-stu-id="93d0e-529">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="93d0e-530">Profil</span><span class="sxs-lookup"><span data-stu-id="93d0e-530">Profile</span></span>

* <span data-ttu-id="93d0e-531">Correction de la détection de source `disk create`</span><span class="sxs-lookup"><span data-stu-id="93d0e-531">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="93d0e-532">[CHANGEMENT CASSANT] Suppression de `--msi-port` et `--identity-port` car ils ne sont plus utilisés</span><span class="sxs-lookup"><span data-stu-id="93d0e-532">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="93d0e-533">Correction d’une faute de frappe dans le bref résumé de `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="93d0e-533">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="93d0e-534">Redis</span><span class="sxs-lookup"><span data-stu-id="93d0e-534">Redis</span></span>

* <span data-ttu-id="93d0e-535">`redis patch-schedule patch-schedule show` déconseillé en faveur de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="93d0e-535">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="93d0e-536">`redis list-all` déconseillé.</span><span class="sxs-lookup"><span data-stu-id="93d0e-536">Deprecated `redis list-all`.</span></span> <span data-ttu-id="93d0e-537">Cette fonctionnalité a été pliée dans `redis list`</span><span class="sxs-lookup"><span data-stu-id="93d0e-537">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="93d0e-538">`redis import-method` déconseillé en faveur de `redis import`</span><span class="sxs-lookup"><span data-stu-id="93d0e-538">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="93d0e-539">Ajout de la prise en charge de `--ids` pour diverses commandes</span><span class="sxs-lookup"><span data-stu-id="93d0e-539">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="93d0e-540">Rôle</span><span class="sxs-lookup"><span data-stu-id="93d0e-540">Role</span></span>

* <span data-ttu-id="93d0e-541">[CHANGEMENT CASSANT] Suppression de `ad sp reset-credentials` déconseillé</span><span class="sxs-lookup"><span data-stu-id="93d0e-541">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="93d0e-542">Stockage</span><span class="sxs-lookup"><span data-stu-id="93d0e-542">Storage</span></span>

* <span data-ttu-id="93d0e-543">Autorise l’application du jeton SAS de destination pour une copie d’objets blob si le SAS source et la clé de compte ne sont pas spécifiés</span><span class="sxs-lookup"><span data-stu-id="93d0e-543">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="93d0e-544">Exposé--délai d’expiration de socket pour les chargements et téléchargements d’objets blob</span><span class="sxs-lookup"><span data-stu-id="93d0e-544">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="93d0e-545">Traite les noms d’objets blob commençant par des séparateurs de chemin d’accès comme des chemins d’accès relatifs</span><span class="sxs-lookup"><span data-stu-id="93d0e-545">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="93d0e-546">Autorise `storage blob copy --source-sas` avec le caractère de démarrage de requête, « ? »</span><span class="sxs-lookup"><span data-stu-id="93d0e-546">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="93d0e-547">`storage entity query --marker` corrigé pour accepter une liste de clé =valeurs</span><span class="sxs-lookup"><span data-stu-id="93d0e-547">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="93d0e-548">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="93d0e-548">VM</span></span>

* <span data-ttu-id="93d0e-549">Correction d’une logique de détection invalide sur l’URI de l’objet blob non gérée</span><span class="sxs-lookup"><span data-stu-id="93d0e-549">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="93d0e-550">Ajout de la prise en charge du chiffrement de disque sans principaux de service fournis par l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="93d0e-550">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="93d0e-551">[CHANGEMENT CASSANT] Ne pas utiliser « ManagedIdentityExtension » de machine virtuelle pour la prise en charge de MSI</span><span class="sxs-lookup"><span data-stu-id="93d0e-551">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="93d0e-552">Ajout de la prise en charge pour la stratégie d’éviction vers `vmss`</span><span class="sxs-lookup"><span data-stu-id="93d0e-552">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="93d0e-553">[CHANGEMENT CASSANT] Suppression de `--ids` de :</span><span class="sxs-lookup"><span data-stu-id="93d0e-553">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="93d0e-554">Ajout de la prise en charge des accélérateurs d’écriture</span><span class="sxs-lookup"><span data-stu-id="93d0e-554">Added write accelerator support</span></span>
* <span data-ttu-id="93d0e-555">Ajout de `vmss perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="93d0e-555">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="93d0e-556">Correction de `vm diagnostics set` pour détecter la fiabilité du type de système d’exploitation de la machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="93d0e-556">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="93d0e-557">Modification de `vm resize` pour vérifier si la taille demandée est différente de celle actuellement définie et pour mettre à jour uniquement en cas de modifications</span><span class="sxs-lookup"><span data-stu-id="93d0e-557">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="93d0e-558">10 avril 2018</span><span class="sxs-lookup"><span data-stu-id="93d0e-558">April 10, 2018</span></span>

<span data-ttu-id="93d0e-559">Version 2.0.31</span><span class="sxs-lookup"><span data-stu-id="93d0e-559">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="93d0e-560">ACR</span><span class="sxs-lookup"><span data-stu-id="93d0e-560">ACR</span></span>

* <span data-ttu-id="93d0e-561">Gestion améliorée des erreurs de secours wincred</span><span class="sxs-lookup"><span data-stu-id="93d0e-561">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="93d0e-562">ACS</span><span class="sxs-lookup"><span data-stu-id="93d0e-562">ACS</span></span>

* <span data-ttu-id="93d0e-563">Modification de la durée de validité des SPN créés par AKS à 5 ans</span><span class="sxs-lookup"><span data-stu-id="93d0e-563">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="93d0e-564">AppService</span><span class="sxs-lookup"><span data-stu-id="93d0e-564">Appservice</span></span>

* [CHANGEMENT CASSANT]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="93d0e-566">Correction d’une exception non interceptée pour les plans webapp inexistants</span><span class="sxs-lookup"><span data-stu-id="93d0e-566">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="93d0e-567">Batch AI</span><span class="sxs-lookup"><span data-stu-id="93d0e-567">BatchAI</span></span>

* <span data-ttu-id="93d0e-568">Ajout de la prise en charge de l’API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="93d0e-568">Added support for 2018-03-01 API</span></span>

 - <span data-ttu-id="93d0e-569">Montage au niveau du travail</span><span class="sxs-lookup"><span data-stu-id="93d0e-569">Job level mounting</span></span>
 - <span data-ttu-id="93d0e-570">Variables d’environnement avec les valeurs des secrets</span><span class="sxs-lookup"><span data-stu-id="93d0e-570">Environment variables with secret values</span></span>
 - <span data-ttu-id="93d0e-571">Paramètres des compteurs de performances</span><span class="sxs-lookup"><span data-stu-id="93d0e-571">Performance counters settings</span></span>
 - <span data-ttu-id="93d0e-572">Création de rapports de segments de ligne spécifiques à un travail</span><span class="sxs-lookup"><span data-stu-id="93d0e-572">Reporting of job specific path segment</span></span>
 - <span data-ttu-id="93d0e-573">Prise en charge des sous-dossiers dans les listes de fichiers de l’API</span><span class="sxs-lookup"><span data-stu-id="93d0e-573">Support for subfolders in list files api</span></span>
 - <span data-ttu-id="93d0e-574">Création de rapports d’utilisation et de limites</span><span class="sxs-lookup"><span data-stu-id="93d0e-574">Usage and limits reporting</span></span>
 - <span data-ttu-id="93d0e-575">Autorisation de la spécification du type de mise en cache pour les serveurs NFS</span><span class="sxs-lookup"><span data-stu-id="93d0e-575">Allow to specify caching type for NFS servers</span></span>
 - <span data-ttu-id="93d0e-576">Prise en charge des images personnalisées</span><span class="sxs-lookup"><span data-stu-id="93d0e-576">Support for custom images</span></span>
 - <span data-ttu-id="93d0e-577">Ajout de la prise en charge de la boîte à outils pyTorch</span><span class="sxs-lookup"><span data-stu-id="93d0e-577">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="93d0e-578">Ajout de la commande `job wait` qui permet d’attendre la fin du travail et d’obtenir le code de sortie du travail</span><span class="sxs-lookup"><span data-stu-id="93d0e-578">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="93d0e-579">Ajout de la commande `usage show` pour répertorier l’utilisation actuelle des ressources Batch AI et les limites pour les différentes régions</span><span class="sxs-lookup"><span data-stu-id="93d0e-579">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="93d0e-580">Prise en charge des clouds nationaux</span><span class="sxs-lookup"><span data-stu-id="93d0e-580">National clouds are supported</span></span>
* <span data-ttu-id="93d0e-581">Ajout d’arguments de ligne de commande de travail pour monter des systèmes de fichiers au niveau du travail en plus des fichiers de configuration</span><span class="sxs-lookup"><span data-stu-id="93d0e-581">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="93d0e-582">Ajout de plus d’options pour personnaliser les clusters : priorité des machines virtuelles, sous-réseau, nombre de nœuds initial pour les clusters avec mise à l’échelle automatique, spécification d’une image personnalisée</span><span class="sxs-lookup"><span data-stu-id="93d0e-582">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="93d0e-583">Ajout d’une option de ligne de commande pour spécifier le type de mise en cache pour les NFS gérés par Batch AI</span><span class="sxs-lookup"><span data-stu-id="93d0e-583">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="93d0e-584">Simplification de la spécification du montage du système de fichiers dans les fichiers config.</span><span class="sxs-lookup"><span data-stu-id="93d0e-584">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="93d0e-585">Il est désormais possible d’omettre les informations d’identification pour les partages de fichiers Azure et les conteneurs d’objets blob Azure : CLI remplira les informations d’identification manquantes à l’aide de la clé du compte de stockage fournie par le biais des paramètres de ligne de commande ou spécifiée via la variable d’environnement, ou interrogera la clé à partir du stockage Azure (si le compte de stockage appartient à l’abonnement actuel)</span><span class="sxs-lookup"><span data-stu-id="93d0e-585">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="93d0e-586">La commande de flux de fichiers de travail se remplit désormais automatiquement lorsque le travail est terminé (réussite, échec, terminé ou supprimé)</span><span class="sxs-lookup"><span data-stu-id="93d0e-586">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="93d0e-587">Amélioration de la sortie `table` pour les opérations `show`</span><span class="sxs-lookup"><span data-stu-id="93d0e-587">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="93d0e-588">Ajout de l’option `--use-auto-storage` pour la création du cluster.</span><span class="sxs-lookup"><span data-stu-id="93d0e-588">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="93d0e-589">Cette option simplifie la gestion des comptes de stockage et le montage de partages de fichiers Azure et de conteneurs d’objets blob Azure vers des clusters</span><span class="sxs-lookup"><span data-stu-id="93d0e-589">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="93d0e-590">Ajout de l’option `--generate-ssh-keys` à `cluster create` et `file-server create`</span><span class="sxs-lookup"><span data-stu-id="93d0e-590">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="93d0e-591">Ajout de la possibilité de fournir la tâche de configuration de nœud via la ligne de commande</span><span class="sxs-lookup"><span data-stu-id="93d0e-591">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="93d0e-592">[CHANGEMENT CASSANT] Déplacement des commandes `job stream-file` et `job list-files` sous le groupe `job file`</span><span class="sxs-lookup"><span data-stu-id="93d0e-592">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="93d0e-593">[CHANGEMENT CASSANT] Renommage de `--admin-user-name` en `--user-name` dans la commande `file-server create` pour être cohérent avec la commande `cluster create`</span><span class="sxs-lookup"><span data-stu-id="93d0e-593">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="93d0e-594">Facturation</span><span class="sxs-lookup"><span data-stu-id="93d0e-594">Billing</span></span>

* <span data-ttu-id="93d0e-595">Ajout de commandes d’inscription de compte</span><span class="sxs-lookup"><span data-stu-id="93d0e-595">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="93d0e-596">Consommation</span><span class="sxs-lookup"><span data-stu-id="93d0e-596">Consumption</span></span>

* <span data-ttu-id="93d0e-597">Ajout des commandes `marketplace`</span><span class="sxs-lookup"><span data-stu-id="93d0e-597">Added `marketplace` commands</span></span>
* <span data-ttu-id="93d0e-598">[CHANGEMENT CASSANT] Renommage de `reservations summaries` en `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="93d0e-598">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="93d0e-599">[CHANGEMENT CASSANT] Renommage de `reservations details` en `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="93d0e-599">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="93d0e-600">[CHANGEMENT CASSANT] Suppression des options abrégées de `--reservation-order-id` et `--reservation-id` pour les commandes `reservation`</span><span class="sxs-lookup"><span data-stu-id="93d0e-600">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="93d0e-601">[CHANGEMENT CASSANT] Suppression des options abrégées de `--grain` pour les commandes `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="93d0e-601">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="93d0e-602">[CHANGEMENT CASSANT] Suppression des options abrégées de `--include-meter-details` pour les commandes `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="93d0e-602">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="93d0e-603">Conteneur</span><span class="sxs-lookup"><span data-stu-id="93d0e-603">Container</span></span>

* <span data-ttu-id="93d0e-604">Ajout des paramètres de montage de volume de référentiel Git `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` et `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="93d0e-604">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="93d0e-605">Résolution de [#5926](https://github.com/Azure/azure-cli/issues/5926) : `az container exec` échoue lorsque le nom du conteneur -- est spécifié</span><span class="sxs-lookup"><span data-stu-id="93d0e-605">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="93d0e-606">Extension</span><span class="sxs-lookup"><span data-stu-id="93d0e-606">Extension</span></span>

* <span data-ttu-id="93d0e-607">Modification du message de vérification de distribution pour qu’il soit au niveau du débogage</span><span class="sxs-lookup"><span data-stu-id="93d0e-607">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="93d0e-608">Interactive</span><span class="sxs-lookup"><span data-stu-id="93d0e-608">Interactive</span></span>

* <span data-ttu-id="93d0e-609">Modification pour arrêter la saisie semi-automatique sur les commandes non reconnues</span><span class="sxs-lookup"><span data-stu-id="93d0e-609">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="93d0e-610">Ajout d’événements de raccordement avant et après la création du sous-arbre de commande</span><span class="sxs-lookup"><span data-stu-id="93d0e-610">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="93d0e-611">Ajout de la saisie semi-automatique pour les paramètres `--ids`</span><span class="sxs-lookup"><span data-stu-id="93d0e-611">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="93d0e-612">Réseau</span><span class="sxs-lookup"><span data-stu-id="93d0e-612">Network</span></span>

* <span data-ttu-id="93d0e-613">Résolution de [#5936](https://github.com/Azure/azure-cli/issues/5936) : les balises `application-gateway create` n’ont pas pu déterminer l’ensemble</span><span class="sxs-lookup"><span data-stu-id="93d0e-613">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="93d0e-614">Ajout de l’argument `--auth-certs` pour joindre des certificats d’authentification pour `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="93d0e-614">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="93d0e-615">#4910</span><span class="sxs-lookup"><span data-stu-id="93d0e-615">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="93d0e-616">Ajout de commandes `ddos-protection` pour créer des plans de protection DDoS</span><span class="sxs-lookup"><span data-stu-id="93d0e-616">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="93d0e-617">Prise en charge de `--ddos-protection-plan` pour `vnet [create|update]` pour associer un réseau virtuel à un plan de protection DDoS</span><span class="sxs-lookup"><span data-stu-id="93d0e-617">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="93d0e-618">Résolution du problème avec l’ indicateur `--disable-bgp-route-propagation` dans `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="93d0e-618">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="93d0e-619">Suppression des arguments factices `--public-ip-address-type` et `--subnet-type` pour `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="93d0e-619">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="93d0e-620">Ajout de la prise en charge des enregistrements TXT avec les séquences d’échappement RFC 1035 à `network dns zone [import|export]` et `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="93d0e-620">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="93d0e-621">Profil</span><span class="sxs-lookup"><span data-stu-id="93d0e-621">Profile</span></span>

* <span data-ttu-id="93d0e-622">Ajout de la prise en charge des comptes Azure Classic dans `account list`</span><span class="sxs-lookup"><span data-stu-id="93d0e-622">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="93d0e-623">[CHANGEMENT CASSANT] Suppression des arguments `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="93d0e-623">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="93d0e-624">SGBDR</span><span class="sxs-lookup"><span data-stu-id="93d0e-624">RDBMS</span></span>

* <span data-ttu-id="93d0e-625">Ajout de la commande `georestore`</span><span class="sxs-lookup"><span data-stu-id="93d0e-625">Added `georestore` command</span></span>
* <span data-ttu-id="93d0e-626">Suppression de la restriction de taille de stockage de la commande `create`</span><span class="sxs-lookup"><span data-stu-id="93d0e-626">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="93d0e-627">Ressource</span><span class="sxs-lookup"><span data-stu-id="93d0e-627">Resource</span></span>

* <span data-ttu-id="93d0e-628">Ajout de la prise en charge de `--metadata` pour `policy definition create`</span><span class="sxs-lookup"><span data-stu-id="93d0e-628">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="93d0e-629">Ajout de la prise en charge de `--metadata`, `--set`, `--add` et `--remove` à `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="93d0e-629">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="93d0e-630">SQL</span><span class="sxs-lookup"><span data-stu-id="93d0e-630">SQL</span></span>

* <span data-ttu-id="93d0e-631">Ajout de `sql elastic-pool op list` et `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="93d0e-631">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="93d0e-632">Stockage</span><span class="sxs-lookup"><span data-stu-id="93d0e-632">Storage</span></span>

* <span data-ttu-id="93d0e-633">Amélioration des messages d’erreur pour les chaînes de connexion incorrectes</span><span class="sxs-lookup"><span data-stu-id="93d0e-633">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="93d0e-634">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="93d0e-634">VM</span></span>

* <span data-ttu-id="93d0e-635">Ajout de la prise en charge pour configurer le nombre de domaines d’erreur de plateforme sur `vmss create`</span><span class="sxs-lookup"><span data-stu-id="93d0e-635">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="93d0e-636">Modification de `vmss create` sur la valeur par défaut de l’équilibreur de charge Standard pour les groupes identiques désactivés zonaux, grands ou avec un seul groupe de placement</span><span class="sxs-lookup"><span data-stu-id="93d0e-636">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [CHANGEMENT CASSANT]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="93d0e-638">Ajout de la prise en charge des références SKU d’IP public à `vm create`</span><span class="sxs-lookup"><span data-stu-id="93d0e-638">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="93d0e-639">Ajout des arguments `--keyvault` et `--resource-group` à `vm secret format` pour prendre en charge des scénarios où la commande ne parvient pas à résoudre l’ID de coffre.</span><span class="sxs-lookup"><span data-stu-id="93d0e-639">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="93d0e-640">#5718</span><span class="sxs-lookup"><span data-stu-id="93d0e-640">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="93d0e-641">Amélioration des erreurs pour `[vm|vmss create]` lorsque l’emplacement d’un groupe de ressources ne possède aucune prise en charge de zone</span><span class="sxs-lookup"><span data-stu-id="93d0e-641">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="93d0e-642">27 mars 2018</span><span class="sxs-lookup"><span data-stu-id="93d0e-642">March 27, 2018</span></span>

<span data-ttu-id="93d0e-643">Version 2.0.30</span><span class="sxs-lookup"><span data-stu-id="93d0e-643">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="93d0e-644">Principal</span><span class="sxs-lookup"><span data-stu-id="93d0e-644">Core</span></span>

* <span data-ttu-id="93d0e-645">Afficher le message pour les extensions marquées en tant que préversions dans l’aide</span><span class="sxs-lookup"><span data-stu-id="93d0e-645">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="93d0e-646">ACS</span><span class="sxs-lookup"><span data-stu-id="93d0e-646">ACS</span></span>

* <span data-ttu-id="93d0e-647">Corriger l’erreur de vérification de certificat SSL pour `aks install-cli` dans Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="93d0e-647">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="93d0e-648">AppService</span><span class="sxs-lookup"><span data-stu-id="93d0e-648">Appservice</span></span>

* <span data-ttu-id="93d0e-649">Ajout de la prise en charge HTTPS exclusive à `webapp update`</span><span class="sxs-lookup"><span data-stu-id="93d0e-649">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="93d0e-650">Ajout de la prise en charge des emplacements à `az webapp identity [assign|show]` et `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="93d0e-650">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="93d0e-651">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="93d0e-651">Backup</span></span>

* <span data-ttu-id="93d0e-652">Ajout de la commande `az backup protection isenabled-for-vm`</span><span class="sxs-lookup"><span data-stu-id="93d0e-652">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="93d0e-653">Cette commande peut être utilisée pour vérifier si une machine virtuelle est sauvegardée par un coffre dans l’abonnement</span><span class="sxs-lookup"><span data-stu-id="93d0e-653">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="93d0e-654">Activation des ID d’objet Azure pour les paramètres `--resource-group` et `--vault-name`, pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="93d0e-654">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="93d0e-655">Modification des paramètres `--name` pour accepter le format de sortie des commandes `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="93d0e-655">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="93d0e-656">Conteneur</span><span class="sxs-lookup"><span data-stu-id="93d0e-656">Container</span></span>

* <span data-ttu-id="93d0e-657">Ajout de la commande `container exec`</span><span class="sxs-lookup"><span data-stu-id="93d0e-657">Added `container exec` command.</span></span> <span data-ttu-id="93d0e-658">Exécute les commandes dans un conteneur, pour un groupe de conteneurs en exécution.</span><span class="sxs-lookup"><span data-stu-id="93d0e-658">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="93d0e-659">Autoriser la sortie de table pour la création et la mise à jour d’un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="93d0e-659">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="93d0e-660">Extension</span><span class="sxs-lookup"><span data-stu-id="93d0e-660">Extension</span></span>

* <span data-ttu-id="93d0e-661">Ajout d’un message pour `extension add` si l’extension est en préversion</span><span class="sxs-lookup"><span data-stu-id="93d0e-661">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="93d0e-662">Modification de `extension list-available` afin d’afficher les données complètes d’extension avec `--show-details`</span><span class="sxs-lookup"><span data-stu-id="93d0e-662">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="93d0e-663">[CHANGEMENT CASSANT] Modification de `extension list-available` afin d’afficher les données simplifiées d’extension par défaut</span><span class="sxs-lookup"><span data-stu-id="93d0e-663">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="93d0e-664">Interactive</span><span class="sxs-lookup"><span data-stu-id="93d0e-664">Interactive</span></span>

* <span data-ttu-id="93d0e-665">Modification des saisies semi-automatiques pour procéder à l’activation dès le chargement de la table de commande</span><span class="sxs-lookup"><span data-stu-id="93d0e-665">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="93d0e-666">Correction du bogue par l’exécution du paramètre `--style`</span><span class="sxs-lookup"><span data-stu-id="93d0e-666">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="93d0e-667">Analyseur lexical interactif instancié après le vidage de la table de commande, si manquant</span><span class="sxs-lookup"><span data-stu-id="93d0e-667">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="93d0e-668">Amélioration de la prise en charge de Completer</span><span class="sxs-lookup"><span data-stu-id="93d0e-668">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="93d0e-669">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="93d0e-669">Lab</span></span>

* <span data-ttu-id="93d0e-670">Correction des bogues avec la commande `create environment`</span><span class="sxs-lookup"><span data-stu-id="93d0e-670">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="93d0e-671">Surveiller</span><span class="sxs-lookup"><span data-stu-id="93d0e-671">Monitor</span></span>

* <span data-ttu-id="93d0e-672">Ajout de la prise en charge de `--top`, `--orderby` et `--namespace` à `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="93d0e-672">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="93d0e-673">Résolution de [#4529](https://github.com/Azure/azure-cli/issues/5785) : `metrics list` Accepte une liste de mesures séparées par des espaces à récupérer</span><span class="sxs-lookup"><span data-stu-id="93d0e-673">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="93d0e-674">Ajout de la prise en charge de `--namespace` à `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="93d0e-674">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="93d0e-675">Réseau</span><span class="sxs-lookup"><span data-stu-id="93d0e-675">Network</span></span>

* <span data-ttu-id="93d0e-676">Ajout de la prise en charge des zones de DNS privé</span><span class="sxs-lookup"><span data-stu-id="93d0e-676">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="93d0e-677">Profil</span><span class="sxs-lookup"><span data-stu-id="93d0e-677">Profile</span></span>

* <span data-ttu-id="93d0e-678">Ajout d’un avertissement pour `--identity-port` et `--msi-port` à `login`</span><span class="sxs-lookup"><span data-stu-id="93d0e-678">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="93d0e-679">SGBDR</span><span class="sxs-lookup"><span data-stu-id="93d0e-679">RDBMS</span></span>

* <span data-ttu-id="93d0e-680">Ajout de la version d’API mise à la disposition générale du modèle d’entreprise 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="93d0e-680">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="93d0e-681">Ressource</span><span class="sxs-lookup"><span data-stu-id="93d0e-681">Resource</span></span>

* [CHANGEMENT CASSANT]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="93d0e-683">Rôle</span><span class="sxs-lookup"><span data-stu-id="93d0e-683">Role</span></span>

* <span data-ttu-id="93d0e-684">Ajout de la prise en charge des configurations d’accès et des clients natifs requis à `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="93d0e-684">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="93d0e-685">Modification des commandes `rbac` afin de renvoyer moins de 1 000 ID sur la résolution d’objet</span><span class="sxs-lookup"><span data-stu-id="93d0e-685">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="93d0e-686">Ajout des commandes de gestion des informations d’identification `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="93d0e-686">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="93d0e-687">[CHANGEMENT CASSANT] Suppression des propriétés de la sortie `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="93d0e-687">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="93d0e-688">Ajout de la prise en charge des autorisations `dataActions` et `notDataActions` à `role definition`</span><span class="sxs-lookup"><span data-stu-id="93d0e-688">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="93d0e-689">Stockage</span><span class="sxs-lookup"><span data-stu-id="93d0e-689">Storage</span></span>

* <span data-ttu-id="93d0e-690">Résolution du problème lié au chargement des fichiers présentant une taille comprise entre 195 Go et 200 Go</span><span class="sxs-lookup"><span data-stu-id="93d0e-690">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="93d0e-691">Résolution de [#4049](https://github.com/Azure/azure-cli/issues/4049) : Problèmes avec les chargements d’objets blob d’ajout ignorant les paramètres de condition</span><span class="sxs-lookup"><span data-stu-id="93d0e-691">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="93d0e-692">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="93d0e-692">VM</span></span>

* <span data-ttu-id="93d0e-693">Ajout d’un avertissement à `vmss create` concernant les changements cassants à venir pour les ensembles comprenant plus de 100 instances</span><span class="sxs-lookup"><span data-stu-id="93d0e-693">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="93d0e-694">Ajout de la prise en charge de la résilience dans la zone à `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="93d0e-694">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="93d0e-695">Modification de la vue d’instance de disque pour signaler un meilleur état de chiffrement</span><span class="sxs-lookup"><span data-stu-id="93d0e-695">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="93d0e-696">[CHANGEMENT CASSANT] Modification de `vm extension delete` afin d’annuler la capacité de génération de sortie</span><span class="sxs-lookup"><span data-stu-id="93d0e-696">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="93d0e-697">13 mars 2018</span><span class="sxs-lookup"><span data-stu-id="93d0e-697">March 13, 2018</span></span>

<span data-ttu-id="93d0e-698">Version 2.0.29</span><span class="sxs-lookup"><span data-stu-id="93d0e-698">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="93d0e-699">ACR</span><span class="sxs-lookup"><span data-stu-id="93d0e-699">ACR</span></span>

* <span data-ttu-id="93d0e-700">Ajout de la prise en charge du paramètre `--image` pour `repository delete`</span><span class="sxs-lookup"><span data-stu-id="93d0e-700">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="93d0e-701">Paramètres `--manifest` et `--tag` de la commande `repository delete` déconseillés</span><span class="sxs-lookup"><span data-stu-id="93d0e-701">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="93d0e-702">Ajout de la commande `repository untag` pour supprimer une balise sans supprimer les données</span><span class="sxs-lookup"><span data-stu-id="93d0e-702">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="93d0e-703">ACS</span><span class="sxs-lookup"><span data-stu-id="93d0e-703">ACS</span></span>

* <span data-ttu-id="93d0e-704">Ajout de la commande `aks upgrade-connector` pour mettre à niveau un connecteur existant</span><span class="sxs-lookup"><span data-stu-id="93d0e-704">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="93d0e-705">Modification des fichiers de configuration `kubectl` pour utiliser un YAML de style bloc plus lisible</span><span class="sxs-lookup"><span data-stu-id="93d0e-705">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="93d0e-706">Advisor</span><span class="sxs-lookup"><span data-stu-id="93d0e-706">Advisor</span></span>

* <span data-ttu-id="93d0e-707">[CHANGEMENT CASSANT] Renommage de `advisor configuration get` en `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="93d0e-707">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="93d0e-708">[CHANGEMENT CASSANT] Renommage de `advisor configuration set` en `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="93d0e-708">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="93d0e-709">[CHANGEMENT CASSANT] Suppression de `advisor recommendation generate`</span><span class="sxs-lookup"><span data-stu-id="93d0e-709">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="93d0e-710">Ajout du paramètre `--refresh` pour `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="93d0e-710">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="93d0e-711">Ajout de la commande `advisor recommendation show`</span><span class="sxs-lookup"><span data-stu-id="93d0e-711">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="93d0e-712">AppService</span><span class="sxs-lookup"><span data-stu-id="93d0e-712">Appservice</span></span>

* <span data-ttu-id="93d0e-713">`[webapp|functionapp] assign-identity` déconseillé</span><span class="sxs-lookup"><span data-stu-id="93d0e-713">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="93d0e-714">Ajout des commandes d’identité gérée `webapp identity [assign|show]` et `functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="93d0e-714">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="93d0e-715">Eventhubs</span><span class="sxs-lookup"><span data-stu-id="93d0e-715">Eventhubs</span></span>

* <span data-ttu-id="93d0e-716">Version initiale</span><span class="sxs-lookup"><span data-stu-id="93d0e-716">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="93d0e-717">Extension</span><span class="sxs-lookup"><span data-stu-id="93d0e-717">Extension</span></span>

* <span data-ttu-id="93d0e-718">Ajout d’un contrôle supplémentaire pour avertir l’utilisateur si le distributeur utilisé est différent de celui stocké dans le fichier source du package, car cela peut entraîner des erreurs</span><span class="sxs-lookup"><span data-stu-id="93d0e-718">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="93d0e-719">Interactive</span><span class="sxs-lookup"><span data-stu-id="93d0e-719">Interactive</span></span>

* <span data-ttu-id="93d0e-720">Résolu [#5625](https://github.com/Azure/azure-cli/issues/5625) : conservation de l’historique entre différentes sessions</span><span class="sxs-lookup"><span data-stu-id="93d0e-720">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="93d0e-721">Résolu [#3016](https://github.com/Azure/azure-cli/issues/3016) : historique non enregistré alors qu’il était dans la portée</span><span class="sxs-lookup"><span data-stu-id="93d0e-721">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="93d0e-722">Résolu [#5688](https://github.com/Azure/azure-cli/issues/5688) : la saisie automatique n’apparaît pas si le chargement de la table de commande a rencontré une exception</span><span class="sxs-lookup"><span data-stu-id="93d0e-722">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="93d0e-723">Résolu : indicateur de progression pour les opérations à long terme</span><span class="sxs-lookup"><span data-stu-id="93d0e-723">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="93d0e-724">Surveiller</span><span class="sxs-lookup"><span data-stu-id="93d0e-724">Monitor</span></span>

* <span data-ttu-id="93d0e-725">Les commandes `monitor autoscale-settings` ont été déconseillées</span><span class="sxs-lookup"><span data-stu-id="93d0e-725">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="93d0e-726">Ajout des commandes `monitor autoscale`</span><span class="sxs-lookup"><span data-stu-id="93d0e-726">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="93d0e-727">Ajout des commandes `monitor autoscale profile`</span><span class="sxs-lookup"><span data-stu-id="93d0e-727">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="93d0e-728">Ajout des commandes `monitor autoscale rule`</span><span class="sxs-lookup"><span data-stu-id="93d0e-728">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="93d0e-729">Réseau</span><span class="sxs-lookup"><span data-stu-id="93d0e-729">Network</span></span>

* <span data-ttu-id="93d0e-730">[CHANGEMENT CASSANT] Suppression du paramètre `--tags` de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="93d0e-730">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="93d0e-731">Suppression de certaines valeurs par défaut erronées pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="93d0e-731">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="93d0e-732">Ajout des commandes `network watcher connection-monitor`</span><span class="sxs-lookup"><span data-stu-id="93d0e-732">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="93d0e-733">Ajout des paramètres `--vnet` et `--subnet` à `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="93d0e-733">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="93d0e-734">Profil</span><span class="sxs-lookup"><span data-stu-id="93d0e-734">Profile</span></span>

* <span data-ttu-id="93d0e-735">Paramètre `--msi` déconseillé pour `az login`</span><span class="sxs-lookup"><span data-stu-id="93d0e-735">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="93d0e-736">Ajout du paramètre `--identity` pour `az login` afin de remplacer `--msi`</span><span class="sxs-lookup"><span data-stu-id="93d0e-736">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="93d0e-737">SGBDR</span><span class="sxs-lookup"><span data-stu-id="93d0e-737">RDBMS</span></span>

* <span data-ttu-id="93d0e-738">[PRÉVERSION] Modifiée pour utiliser l’API 2017-12-01-préversion</span><span class="sxs-lookup"><span data-stu-id="93d0e-738">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="93d0e-739">Service Bus</span><span class="sxs-lookup"><span data-stu-id="93d0e-739">Service Bus</span></span>

* <span data-ttu-id="93d0e-740">Version initiale</span><span class="sxs-lookup"><span data-stu-id="93d0e-740">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="93d0e-741">Stockage</span><span class="sxs-lookup"><span data-stu-id="93d0e-741">Storage</span></span>

* <span data-ttu-id="93d0e-742">Résolution de [#4971](https://github.com/Azure/azure-cli/issues/4971) : `storage blob copy` prend désormais en charge les autres clouds Azure</span><span class="sxs-lookup"><span data-stu-id="93d0e-742">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="93d0e-743">Résolu [#5286](https://github.com/Azure/azure-cli/issues/5286) : Les lots de commandes `storage blob [delete-batch|download-batch|upload-batch]` ne génèrent plus une erreur lors d’échecs de la condition préalable</span><span class="sxs-lookup"><span data-stu-id="93d0e-743">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="93d0e-744">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="93d0e-744">VM</span></span>

* <span data-ttu-id="93d0e-745">Ajout de prise en charge de `[vm|vmss] create` pour attacher des disques de données non gérées et configurer la mise en cache</span><span class="sxs-lookup"><span data-stu-id="93d0e-745">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="93d0e-746">`[vm|vmss] assign-identity` et `[vm|vmss] remove-identity` sont déconseillés</span><span class="sxs-lookup"><span data-stu-id="93d0e-746">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="93d0e-747">Ajout des commandes `vm identity [assign|remove|show]` et `vmss identity [assign|remove|show]` pour remplacer des commandes déconseillées</span><span class="sxs-lookup"><span data-stu-id="93d0e-747">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="93d0e-748">Modification de la priorité par défaut dans `vmss create` à None</span><span class="sxs-lookup"><span data-stu-id="93d0e-748">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="93d0e-749">27 février 2018</span><span class="sxs-lookup"><span data-stu-id="93d0e-749">February 27, 2018</span></span>

<span data-ttu-id="93d0e-750">Version 2.0.28</span><span class="sxs-lookup"><span data-stu-id="93d0e-750">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="93d0e-751">Principal</span><span class="sxs-lookup"><span data-stu-id="93d0e-751">Core</span></span>

* <span data-ttu-id="93d0e-752">Résolu [#5184](https://github.com/Azure/azure-cli/issues/5184) : Problème d’installation d’Homebrew</span><span class="sxs-lookup"><span data-stu-id="93d0e-752">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="93d0e-753">Ajout de la prise en charge de télémétrie d’extension avec des clés personnalisées</span><span class="sxs-lookup"><span data-stu-id="93d0e-753">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="93d0e-754">Ajout de la connexion HTTP à `--debug`</span><span class="sxs-lookup"><span data-stu-id="93d0e-754">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="93d0e-755">ACS</span><span class="sxs-lookup"><span data-stu-id="93d0e-755">ACS</span></span>

* <span data-ttu-id="93d0e-756">Modification pour utiliser le graphique Helm `virtual-kubelet-for-aks` pour `aks install-connector` par défaut</span><span class="sxs-lookup"><span data-stu-id="93d0e-756">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="93d0e-757">Problème résolu : autorisation insuffisante des principaux de service à créer des groupes de conteneur ACI</span><span class="sxs-lookup"><span data-stu-id="93d0e-757">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="93d0e-758">Ajout des paramètres `--aci-container-group`, `--location` et `--image-tag` à `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="93d0e-758">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="93d0e-759">Suppression de l’avis de désapprobation de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="93d0e-759">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="93d0e-760">AppService</span><span class="sxs-lookup"><span data-stu-id="93d0e-760">Appservice</span></span>

* <span data-ttu-id="93d0e-761">Mises à jour pour la nouvelle version du kit de développement logiciel (SDK) (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="93d0e-761">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="93d0e-762">Résolu [#5538](https://github.com/Azure/azure-cli/issues/5538) : `Free` défini comme une SKU invalide</span><span class="sxs-lookup"><span data-stu-id="93d0e-762">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="93d0e-763">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="93d0e-763">Cognitive Services</span></span>

* <span data-ttu-id="93d0e-764">Mise à jour de l’avis lors de la création d’un compte Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="93d0e-764">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="93d0e-765">Consommation</span><span class="sxs-lookup"><span data-stu-id="93d0e-765">Consumption</span></span>

* <span data-ttu-id="93d0e-766">Ajout de nouvelles commandes pour l’API priceSheet</span><span class="sxs-lookup"><span data-stu-id="93d0e-766">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="93d0e-767">Mise à jour des formats existants Détails d’utilisations et Détails de la réservation</span><span class="sxs-lookup"><span data-stu-id="93d0e-767">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="93d0e-768">Conteneur</span><span class="sxs-lookup"><span data-stu-id="93d0e-768">Container</span></span>

* <span data-ttu-id="93d0e-769">Ajout des arguments `--secrets` et `--secrets-mount-path` à `container create` pour utiliser des secrets dans ACI</span><span class="sxs-lookup"><span data-stu-id="93d0e-769">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="93d0e-770">Réseau</span><span class="sxs-lookup"><span data-stu-id="93d0e-770">Network</span></span>

* <span data-ttu-id="93d0e-771">Résolu [#5559](https://github.com/Azure/azure-cli/issues/5559) : client manquant dans `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="93d0e-771">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="93d0e-772">Ressource</span><span class="sxs-lookup"><span data-stu-id="93d0e-772">Resource</span></span>

* <span data-ttu-id="93d0e-773">Modification de `group deployment export` pour afficher un modèle et des erreurs partiels sur échec</span><span class="sxs-lookup"><span data-stu-id="93d0e-773">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="93d0e-774">Rôle</span><span class="sxs-lookup"><span data-stu-id="93d0e-774">Role</span></span>

* <span data-ttu-id="93d0e-775">Ajout de `role assignment list-changelogs` pour permettre l’audit des rôles du principal de service</span><span class="sxs-lookup"><span data-stu-id="93d0e-775">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="93d0e-776">SQL</span><span class="sxs-lookup"><span data-stu-id="93d0e-776">SQL</span></span>

* <span data-ttu-id="93d0e-777">Ajout de la prise en charge de la redondance de zone pour les bases de données et les pools élastiques lors de création et mise à jour</span><span class="sxs-lookup"><span data-stu-id="93d0e-777">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="93d0e-778">Stockage</span><span class="sxs-lookup"><span data-stu-id="93d0e-778">Storage</span></span>

* <span data-ttu-id="93d0e-779">Activation de la spécification de préfixe/destination pour `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="93d0e-779">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="93d0e-780">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="93d0e-780">VM</span></span>

* <span data-ttu-id="93d0e-781">Ajout de prise en charge de jonction / séparation de disques sur une instance de groupe de machines virtuelles identiques uniques</span><span class="sxs-lookup"><span data-stu-id="93d0e-781">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="93d0e-782">13 février 2018</span><span class="sxs-lookup"><span data-stu-id="93d0e-782">February 13, 2018</span></span>

<span data-ttu-id="93d0e-783">Version 2.0.27</span><span class="sxs-lookup"><span data-stu-id="93d0e-783">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="93d0e-784">Principal</span><span class="sxs-lookup"><span data-stu-id="93d0e-784">Core</span></span>

* <span data-ttu-id="93d0e-785">Modification de l’authentification pour passer au système de clé sur l’ID d’abonnement et le nom sur la connexion MSI</span><span class="sxs-lookup"><span data-stu-id="93d0e-785">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="93d0e-786">ACS</span><span class="sxs-lookup"><span data-stu-id="93d0e-786">ACS</span></span>

* <span data-ttu-id="93d0e-787">[CHANGEMENT CASSANT] Renommage de `aks get-versions` en `aks get-upgrades` pour des raisons de précision</span><span class="sxs-lookup"><span data-stu-id="93d0e-787">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="93d0e-788">Modification de `aks get-versions` pour afficher les versions Kubernetes disponibles pour `aks create`</span><span class="sxs-lookup"><span data-stu-id="93d0e-788">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="93d0e-789">Modification des valeurs par défaut de `aks create` de manière à laisser le serveur choisir la version de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="93d0e-789">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="93d0e-790">Mise à jour des messages d’aide faisant référence au principal du service généré par AKS</span><span class="sxs-lookup"><span data-stu-id="93d0e-790">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="93d0e-791">Modification des tailles de nœud par défaut pour `aks create` pour passer de « Standard\_D1\_v2 » à « Standard\_DS1\_v2 »</span><span class="sxs-lookup"><span data-stu-id="93d0e-791">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="93d0e-792">Meilleure fiabilité lors de la localisation du pod de tableau de bord pour `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="93d0e-792">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="93d0e-793">Correction de `aks get-credentials` pour gérer les erreurs Unicode lors du chargement des fichiers de configuration Kubernetes</span><span class="sxs-lookup"><span data-stu-id="93d0e-793">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="93d0e-794">Ajout d’un message à `az aks install-cli` pour aider à l’obtention de `kubectl` dans `$PATH`</span><span class="sxs-lookup"><span data-stu-id="93d0e-794">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="93d0e-795">AppService</span><span class="sxs-lookup"><span data-stu-id="93d0e-795">Appservice</span></span>

* <span data-ttu-id="93d0e-796">Résolution du problème dans lequel `webapp [backup|restore]` a échoué en raison d’une référence null</span><span class="sxs-lookup"><span data-stu-id="93d0e-796">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="93d0e-797">Ajout de la prise en charge supplémentaire des plans App Service par défaut via `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="93d0e-797">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="93d0e-798">CDN</span><span class="sxs-lookup"><span data-stu-id="93d0e-798">CDN</span></span>

* <span data-ttu-id="93d0e-799">Ajout des commandes `cdn custom-domain [enable-https|disable-https]`</span><span class="sxs-lookup"><span data-stu-id="93d0e-799">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="93d0e-800">Conteneur</span><span class="sxs-lookup"><span data-stu-id="93d0e-800">Container</span></span>

* <span data-ttu-id="93d0e-801">Ajout de l’option `--follow` à `az container logs` pour les journaux de diffusion en continu</span><span class="sxs-lookup"><span data-stu-id="93d0e-801">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="93d0e-802">Ajout de la commande `container attach` qui associe les flux d’erreur et de sortie standard locaux à un conteneur d’un groupe de conteneur</span><span class="sxs-lookup"><span data-stu-id="93d0e-802">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="93d0e-803">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="93d0e-803">CosmosDB</span></span>

* <span data-ttu-id="93d0e-804">Ajout de la prise en charge de la définition de fonctionnalités</span><span class="sxs-lookup"><span data-stu-id="93d0e-804">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="93d0e-805">Extension</span><span class="sxs-lookup"><span data-stu-id="93d0e-805">Extension</span></span>

* <span data-ttu-id="93d0e-806">Ajout de la prise en charge du paramètre `--pip-proxy` pour les commandes `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="93d0e-806">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="93d0e-807">Ajout de la prise en charge de l’argument `--pip-extra-index-urls` pour les commandes `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="93d0e-807">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="93d0e-808">Commentaires</span><span class="sxs-lookup"><span data-stu-id="93d0e-808">Feedback</span></span>

* <span data-ttu-id="93d0e-809">Ajout d’informations d’extension aux données de télémétrie</span><span class="sxs-lookup"><span data-stu-id="93d0e-809">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="93d0e-810">Interactive</span><span class="sxs-lookup"><span data-stu-id="93d0e-810">Interactive</span></span>

* <span data-ttu-id="93d0e-811">Résolution du problème dans lequel l’utilisateur est invité à se connecter à l’aide du mode interactif dans Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="93d0e-811">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="93d0e-812">Correction de la régression avec les listes de saisie semi-automatique des paramètres manquants</span><span class="sxs-lookup"><span data-stu-id="93d0e-812">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="93d0e-813">IoT</span><span class="sxs-lookup"><span data-stu-id="93d0e-813">IoT</span></span>

* <span data-ttu-id="93d0e-814">Résolution du problème dans lequel `iot dps access policy [create|update]` renvoie une erreur « introuvable » en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="93d0e-814">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="93d0e-815">Résolution du problème dans lequel `iot dps linked-hub [create|update]` renvoie une erreur « introuvable » en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="93d0e-815">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="93d0e-816">Ajout de la prise en charge de `--no-wait` pour `iot dps access policy [create|update]` et `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="93d0e-816">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="93d0e-817">Modification de `iot hub create` pour autoriser la spécification du nombre de partitions</span><span class="sxs-lookup"><span data-stu-id="93d0e-817">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="93d0e-818">Surveiller</span><span class="sxs-lookup"><span data-stu-id="93d0e-818">Monitor</span></span>

* <span data-ttu-id="93d0e-819">Correction de la commande `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="93d0e-819">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="93d0e-820">Réseau</span><span class="sxs-lookup"><span data-stu-id="93d0e-820">Network</span></span>

* <span data-ttu-id="93d0e-821">Correction de l’option `--tags` pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="93d0e-821">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="93d0e-822">Profil</span><span class="sxs-lookup"><span data-stu-id="93d0e-822">Profile</span></span>

* <span data-ttu-id="93d0e-823">Activation `az login` à partir du mode interactif</span><span class="sxs-lookup"><span data-stu-id="93d0e-823">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="93d0e-824">Ressource</span><span class="sxs-lookup"><span data-stu-id="93d0e-824">Resource</span></span>

* <span data-ttu-id="93d0e-825">Rajout de `feature show`</span><span class="sxs-lookup"><span data-stu-id="93d0e-825">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="93d0e-826">Rôle</span><span class="sxs-lookup"><span data-stu-id="93d0e-826">Role</span></span>

* <span data-ttu-id="93d0e-827">Ajout de l’argument `--available-to-other-tenants` à `ad app update`</span><span class="sxs-lookup"><span data-stu-id="93d0e-827">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="93d0e-828">SQL</span><span class="sxs-lookup"><span data-stu-id="93d0e-828">SQL</span></span>

* <span data-ttu-id="93d0e-829">Ajout des commandes `sql server dns-alias`</span><span class="sxs-lookup"><span data-stu-id="93d0e-829">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="93d0e-830">Ajout de `sql db rename`</span><span class="sxs-lookup"><span data-stu-id="93d0e-830">Added `sql db rename`</span></span>
* <span data-ttu-id="93d0e-831">Ajout de la prise en charge de l’argument `--ids` pour toutes les commandes sql</span><span class="sxs-lookup"><span data-stu-id="93d0e-831">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="93d0e-832">Stockage</span><span class="sxs-lookup"><span data-stu-id="93d0e-832">Storage</span></span>

* <span data-ttu-id="93d0e-833">Ajout des commandes `storage blob service-properties delete-policy` et `storage blob undelete` pour permettre une suppression réversible</span><span class="sxs-lookup"><span data-stu-id="93d0e-833">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="93d0e-834">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="93d0e-834">VM</span></span>

* <span data-ttu-id="93d0e-835">Correction d’un incident lorsque le chiffrement de la machine virtuelle ne peut pas être initialisé entièrement</span><span class="sxs-lookup"><span data-stu-id="93d0e-835">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="93d0e-836">Ajout de la sortie d’ID du principal lors de l’activation de MSI</span><span class="sxs-lookup"><span data-stu-id="93d0e-836">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="93d0e-837">`vm boot-diagnostics get-boot-log` fixe</span><span class="sxs-lookup"><span data-stu-id="93d0e-837">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="93d0e-838">31 janvier 2018</span><span class="sxs-lookup"><span data-stu-id="93d0e-838">January 31, 2018</span></span>

<span data-ttu-id="93d0e-839">Version 2.0.26</span><span class="sxs-lookup"><span data-stu-id="93d0e-839">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="93d0e-840">Principal</span><span class="sxs-lookup"><span data-stu-id="93d0e-840">Core</span></span>

* <span data-ttu-id="93d0e-841">Ajout de la prise en charge de la récupération du jeton brut dans le contexte MSI</span><span class="sxs-lookup"><span data-stu-id="93d0e-841">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="93d0e-842">Suppression de la chaîne de l’indicateur d’interrogation après la fin de LRO sur le fichier cmd.exe de Windows</span><span class="sxs-lookup"><span data-stu-id="93d0e-842">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="93d0e-843">Ajout d’un avertissement qui s’affiche lorsque l’utilisation d’une valeur par défaut configurée a été remplacée par une entrée de niveau INFO.</span><span class="sxs-lookup"><span data-stu-id="93d0e-843">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="93d0e-844">Utilisation de `--verbose` pour voir</span><span class="sxs-lookup"><span data-stu-id="93d0e-844">Use `--verbose` to see</span></span>
* <span data-ttu-id="93d0e-845">Ajouter un indicateur de progression pour les commandes wait</span><span class="sxs-lookup"><span data-stu-id="93d0e-845">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="93d0e-846">ACS</span><span class="sxs-lookup"><span data-stu-id="93d0e-846">ACS</span></span>

* <span data-ttu-id="93d0e-847">Clarification de l’argument `--disable-browser`</span><span class="sxs-lookup"><span data-stu-id="93d0e-847">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="93d0e-848">Amélioration de la touche TAB pour les arguments `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="93d0e-848">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="93d0e-849">AppService</span><span class="sxs-lookup"><span data-stu-id="93d0e-849">Appservice</span></span>

* <span data-ttu-id="93d0e-850">`webapp log [tail|download]` fixe</span><span class="sxs-lookup"><span data-stu-id="93d0e-850">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="93d0e-851">Suppression de la vérification de `kind` sur les fonctions et les applications web</span><span class="sxs-lookup"><span data-stu-id="93d0e-851">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="93d0e-852">CDN</span><span class="sxs-lookup"><span data-stu-id="93d0e-852">CDN</span></span>

* <span data-ttu-id="93d0e-853">Résolution du problème de client manquant avec `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="93d0e-853">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="93d0e-854">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="93d0e-854">CosmosDB</span></span>

* <span data-ttu-id="93d0e-855">Correction de la description du paramètre pour les stratégies de basculement</span><span class="sxs-lookup"><span data-stu-id="93d0e-855">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="93d0e-856">Interactive</span><span class="sxs-lookup"><span data-stu-id="93d0e-856">Interactive</span></span>

* <span data-ttu-id="93d0e-857">Résolution du problème dans lequel les listes de saisie semi-automatique d’option de commande ne s’affichent plus</span><span class="sxs-lookup"><span data-stu-id="93d0e-857">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="93d0e-858">Réseau</span><span class="sxs-lookup"><span data-stu-id="93d0e-858">Network</span></span>

* <span data-ttu-id="93d0e-859">Ajout de la protection pour `--cert-password` à `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="93d0e-859">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="93d0e-860">Résolution du problème lié à `application-gateway update` où `--sku` a appliqué par erreur une valeur par défaut</span><span class="sxs-lookup"><span data-stu-id="93d0e-860">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="93d0e-861">Ajout de la protection pour `--shared-key` et `--authorization-key` à `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="93d0e-861">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="93d0e-862">Résolution du problème de client manquant avec `asg create`</span><span class="sxs-lookup"><span data-stu-id="93d0e-862">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="93d0e-863">Ajout du paramètre `--file-name / -f` pour les noms exportés à `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="93d0e-863">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="93d0e-864">Les problèmes suivants liés à `dns zone export` ont été résolus :</span><span class="sxs-lookup"><span data-stu-id="93d0e-864">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="93d0e-865">Résolution du problème dans lequel des enregistrements TXT longs ont été mal exportés</span><span class="sxs-lookup"><span data-stu-id="93d0e-865">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="93d0e-866">Résolution du problème dans lequel des enregistrements TXT entre guillemets ont été mal exportés sans guillemets placés dans une séquence d’échappement.</span><span class="sxs-lookup"><span data-stu-id="93d0e-866">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="93d0e-867">Résolution du problème où certains enregistrements ont été importés à deux reprises avec `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="93d0e-867">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="93d0e-868">Restauration des commandes `vnet-gateway root-cert` et `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="93d0e-868">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="93d0e-869">Profil</span><span class="sxs-lookup"><span data-stu-id="93d0e-869">Profile</span></span>

* <span data-ttu-id="93d0e-870">Correction de `get-access-token` pour qu’il fonctionne à l’intérieur d’une machine virtuelle avec l’identité</span><span class="sxs-lookup"><span data-stu-id="93d0e-870">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="93d0e-871">Ressource</span><span class="sxs-lookup"><span data-stu-id="93d0e-871">Resource</span></span>

* <span data-ttu-id="93d0e-872">Correction du bogue lié à `deployment [create|validate]` où un avertissement ne s’est pas affiché correctement quand un champ ’type’ du modèle contient des valeurs en majuscules</span><span class="sxs-lookup"><span data-stu-id="93d0e-872">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="93d0e-873">Stockage</span><span class="sxs-lookup"><span data-stu-id="93d0e-873">Storage</span></span>

* <span data-ttu-id="93d0e-874">Résolution du problème lié à la migration des comptes Storage V1 vers Storage V2</span><span class="sxs-lookup"><span data-stu-id="93d0e-874">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="93d0e-875">Ajout de la création progressive de rapports pour toutes les commandes de chargement/téléchargement</span><span class="sxs-lookup"><span data-stu-id="93d0e-875">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="93d0e-876">Résolution du bogue empêchant l’option d’argument « -n » avec `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="93d0e-876">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="93d0e-877">Ajout de la colonne de « snapshot » ajouté à la sortie de table pour `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="93d0e-877">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="93d0e-878">Résolution des bogues dans lesquels différents paramètres devaient être analysés en tant qu’entiers</span><span class="sxs-lookup"><span data-stu-id="93d0e-878">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="93d0e-879">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="93d0e-879">VM</span></span>

* <span data-ttu-id="93d0e-880">Ajout de la commande `vm image accept-terms` pour autoriser la création de machines virtuelles à partir d’images moyennant des frais supplémentaires</span><span class="sxs-lookup"><span data-stu-id="93d0e-880">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="93d0e-881">Correction de `[vm|vmss create]` pour garantir l’exécution des commandes sous un proxy avec des certificats non signés</span><span class="sxs-lookup"><span data-stu-id="93d0e-881">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="93d0e-882">[APERÇU] Ajout de la prise en charge de la priorité « faible» au groupe de machines virtuelles identiques</span><span class="sxs-lookup"><span data-stu-id="93d0e-882">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="93d0e-883">Ajout de la protection pour `--admin-password` à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="93d0e-883">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="93d0e-884">17 janvier 2018</span><span class="sxs-lookup"><span data-stu-id="93d0e-884">January 17, 2018</span></span>

<span data-ttu-id="93d0e-885">Version 2.0.25</span><span class="sxs-lookup"><span data-stu-id="93d0e-885">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="93d0e-886">ACR</span><span class="sxs-lookup"><span data-stu-id="93d0e-886">ACR</span></span>

* <span data-ttu-id="93d0e-887">Ajout d’une connexion acr de secours en cas d’erreurs d’informations d’identification Windows</span><span class="sxs-lookup"><span data-stu-id="93d0e-887">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="93d0e-888">Activation des journaux du Registre</span><span class="sxs-lookup"><span data-stu-id="93d0e-888">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="93d0e-889">ACS</span><span class="sxs-lookup"><span data-stu-id="93d0e-889">ACS</span></span>

* <span data-ttu-id="93d0e-890">Correction de la commande `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="93d0e-890">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="93d0e-891">Suppression de l’exigence de rôle SPN</span><span class="sxs-lookup"><span data-stu-id="93d0e-891">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="93d0e-892">AppService</span><span class="sxs-lookup"><span data-stu-id="93d0e-892">Appservice</span></span>

* <span data-ttu-id="93d0e-893">Correction du bogue avec `config ssl upload` où `hosting_environment_profile` avait la valeur null</span><span class="sxs-lookup"><span data-stu-id="93d0e-893">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="93d0e-894">Ajout de la prise en charge des URL personnalisées pour `browse`</span><span class="sxs-lookup"><span data-stu-id="93d0e-894">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="93d0e-895">Prise en charge de l’emplacement fixe pour `log tail`</span><span class="sxs-lookup"><span data-stu-id="93d0e-895">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="93d0e-896">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="93d0e-896">Backup</span></span>

* <span data-ttu-id="93d0e-897">Modification de l’option `--container-name` de `backup item list` désormais facultative</span><span class="sxs-lookup"><span data-stu-id="93d0e-897">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="93d0e-898">Ajout d’options de compte de stockage à `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="93d0e-898">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="93d0e-899">Correction de la vérification de l’emplacement dans `backup protection enable-for-vm`, ne tient désormais plus compte de la casse</span><span class="sxs-lookup"><span data-stu-id="93d0e-899">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="93d0e-900">Correction d’un problème qui causait l’échec des commandes avec un nom de conteneur non valide</span><span class="sxs-lookup"><span data-stu-id="93d0e-900">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="93d0e-901">Modification de `backup item list` pour inclure « État d’intégrité » par défaut</span><span class="sxs-lookup"><span data-stu-id="93d0e-901">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="93d0e-902">Batch</span><span class="sxs-lookup"><span data-stu-id="93d0e-902">Batch</span></span>

* <span data-ttu-id="93d0e-903">Modification de `batch login` pour retourner des détails d’authentification</span><span class="sxs-lookup"><span data-stu-id="93d0e-903">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="93d0e-904">Cloud</span><span class="sxs-lookup"><span data-stu-id="93d0e-904">Cloud</span></span>

* <span data-ttu-id="93d0e-905">Ne requiert plus de points de terminaison lors de la définition de `--profile` sur un cloud</span><span class="sxs-lookup"><span data-stu-id="93d0e-905">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="93d0e-906">Consommation</span><span class="sxs-lookup"><span data-stu-id="93d0e-906">Consumption</span></span>

* <span data-ttu-id="93d0e-907">Ajout de nouvelles commandes pour les réservations : `consumption reservations summaries` et `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="93d0e-907">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="93d0e-908">Event Grid</span><span class="sxs-lookup"><span data-stu-id="93d0e-908">Event Grid</span></span>

* <span data-ttu-id="93d0e-909">[CHANGEMENT CASSANT] Déplacement des commandes `az eventgrid topic event-subscription` vers `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="93d0e-909">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="93d0e-910">[CHANGEMENT CASSANT] Déplacement des commandes `az eventgrid resource event-subscription` vers `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="93d0e-910">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="93d0e-911">[CHANGEMENT CASSANT] Suppression de la commande `eventgrid event-subscription show-endpoint-url`</span><span class="sxs-lookup"><span data-stu-id="93d0e-911">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="93d0e-912">Utilisation de `eventgrid event-subscription show --include-full-endpoint-url` à la place</span><span class="sxs-lookup"><span data-stu-id="93d0e-912">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="93d0e-913">Ajout de la commande `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="93d0e-913">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="93d0e-914">Ajout de la commande `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="93d0e-914">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="93d0e-915">Ajout du paramètre `--ids` pour les commandes `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="93d0e-915">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="93d0e-916">Ajout de la prise en charge de la saisie semi-automatique via la touche TAB pour les noms de rubrique</span><span class="sxs-lookup"><span data-stu-id="93d0e-916">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="93d0e-917">Interactive</span><span class="sxs-lookup"><span data-stu-id="93d0e-917">Interactive</span></span>

* <span data-ttu-id="93d0e-918">Correction d’un problème qui empêchait le fonctionnement du mode interactif avec Python 2.x</span><span class="sxs-lookup"><span data-stu-id="93d0e-918">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="93d0e-919">Corrections d’erreurs au démarrage</span><span class="sxs-lookup"><span data-stu-id="93d0e-919">Fixed errors on startup</span></span>
* <span data-ttu-id="93d0e-920">Correction du problème de commandes ne s’exécutant pas en mode interactif</span><span class="sxs-lookup"><span data-stu-id="93d0e-920">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="93d0e-921">IoT</span><span class="sxs-lookup"><span data-stu-id="93d0e-921">IoT</span></span>

* <span data-ttu-id="93d0e-922">Ajout de la prise en charge du service de provisionnement des appareils</span><span class="sxs-lookup"><span data-stu-id="93d0e-922">Added support for device provisioning service</span></span>
* <span data-ttu-id="93d0e-923">Ajout de messages de désapprobation dans les commandes et l’aide relative aux commandes</span><span class="sxs-lookup"><span data-stu-id="93d0e-923">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="93d0e-924">Ajout de la vérification IoT pour informer les utilisateurs de l’extension IoT</span><span class="sxs-lookup"><span data-stu-id="93d0e-924">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="93d0e-925">Surveiller</span><span class="sxs-lookup"><span data-stu-id="93d0e-925">Monitor</span></span>

* <span data-ttu-id="93d0e-926">Ajout de la prise en charge des paramètres multi diagnostic.</span><span class="sxs-lookup"><span data-stu-id="93d0e-926">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="93d0e-927">Le paramètre `--name` est désormais requis pour `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="93d0e-927">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="93d0e-928">Ajout de la commande `monitor diagnostic-settings categories` pour obtenir la catégorie des paramètres de diagnostic</span><span class="sxs-lookup"><span data-stu-id="93d0e-928">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="93d0e-929">Réseau</span><span class="sxs-lookup"><span data-stu-id="93d0e-929">Network</span></span>

* <span data-ttu-id="93d0e-930">Résolution du problème se produisant lors de la tentative de passage au mode actif-passif, ou depuis ce dernier, avec `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="93d0e-930">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="93d0e-931">Ajout de la prise en charge de HTTP2 vers `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="93d0e-931">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="93d0e-932">Profil</span><span class="sxs-lookup"><span data-stu-id="93d0e-932">Profile</span></span>

* <span data-ttu-id="93d0e-933">Ajout de la prise en charge pour la connexion à l’aide d’identités affectées aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="93d0e-933">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="93d0e-934">Rôle</span><span class="sxs-lookup"><span data-stu-id="93d0e-934">Role</span></span>

* <span data-ttu-id="93d0e-935">Ajout de l’argument `--assignee-object-id` à `role assignment create` pour ignorer les requêtes de graphique</span><span class="sxs-lookup"><span data-stu-id="93d0e-935">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="93d0e-936">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="93d0e-936">Service Fabric</span></span>

* <span data-ttu-id="93d0e-937">Ajout d’erreurs détaillées à la réponse de validation lors de la création du cluster</span><span class="sxs-lookup"><span data-stu-id="93d0e-937">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="93d0e-938">Résolution du problème concernant le client manquant avec plusieurs commandes</span><span class="sxs-lookup"><span data-stu-id="93d0e-938">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="93d0e-939">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="93d0e-939">VM</span></span>

* <span data-ttu-id="93d0e-940">[PRÉVERSION] Prise en charge interzone pour `vmss`</span><span class="sxs-lookup"><span data-stu-id="93d0e-940">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="93d0e-941">[CHANGEMENT CASSANT] Modification de la valeur par défaut `vmss` de zone unique en équilibreur de charge « Standard »</span><span class="sxs-lookup"><span data-stu-id="93d0e-941">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="93d0e-942">[CHANGEMENT CASSANT] Modification de `externalIdentities` en `userAssignedIdentities` pour EMSI</span><span class="sxs-lookup"><span data-stu-id="93d0e-942">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="93d0e-943">[PRÉVERSION] Ajout de la prise en charge de l’échange de disque du système d’exploitation</span><span class="sxs-lookup"><span data-stu-id="93d0e-943">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="93d0e-944">Ajout de la prise en charge de l’utilisation des images de machine virtuelle à partir d’autres abonnements</span><span class="sxs-lookup"><span data-stu-id="93d0e-944">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="93d0e-945">Ajout des arguments `--plan-name`, `--plan-product`, `--plan-promotion-code` et `--plan-publisher` à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="93d0e-945">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="93d0e-946">Correction des problèmes d’erreur avec `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="93d0e-946">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="93d0e-947">Correction de l’utilisation excessive des ressources due à `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="93d0e-947">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="93d0e-948">19 décembre 2017</span><span class="sxs-lookup"><span data-stu-id="93d0e-948">December 19, 2017</span></span>

<span data-ttu-id="93d0e-949">Version 2.0.23</span><span class="sxs-lookup"><span data-stu-id="93d0e-949">Version 2.0.23</span></span>

* <span data-ttu-id="93d0e-950">Ajout de la prise en charge pour la connexion à l’aide d’identités affectées aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="93d0e-950">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="93d0e-951">Conteneur</span><span class="sxs-lookup"><span data-stu-id="93d0e-951">Container</span></span>

* <span data-ttu-id="93d0e-952">Correction de l’ordre incorrect des paramètres pour les journaux du conteneur</span><span class="sxs-lookup"><span data-stu-id="93d0e-952">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="93d0e-953">Réseau</span><span class="sxs-lookup"><span data-stu-id="93d0e-953">Network</span></span>

* <span data-ttu-id="93d0e-954">Ajout de l’argument `--disable-bgp-route-propagation` à `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="93d0e-954">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="93d0e-955">Ajout de l’argument `--ip-tags` à `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="93d0e-955">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="93d0e-956">Stockage</span><span class="sxs-lookup"><span data-stu-id="93d0e-956">Storage</span></span>

* <span data-ttu-id="93d0e-957">Ajout de la prise en charge du stockage V2</span><span class="sxs-lookup"><span data-stu-id="93d0e-957">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="93d0e-958">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="93d0e-958">VM</span></span>

* <span data-ttu-id="93d0e-959">[APERÇU] Ajout de la prise en charge des identités affectées aux utilisateurs pour les machines virtuelles et les VMSS</span><span class="sxs-lookup"><span data-stu-id="93d0e-959">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="93d0e-960">5 décembre 2017</span><span class="sxs-lookup"><span data-stu-id="93d0e-960">December 5, 2017</span></span>

<span data-ttu-id="93d0e-961">Version 2.0.22</span><span class="sxs-lookup"><span data-stu-id="93d0e-961">Version 2.0.22</span></span>

* <span data-ttu-id="93d0e-962">Suppression des commandes `az component`.</span><span class="sxs-lookup"><span data-stu-id="93d0e-962">Removed `az component` commands.</span></span> <span data-ttu-id="93d0e-963">Utilisation de `az extension` à la place</span><span class="sxs-lookup"><span data-stu-id="93d0e-963">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="93d0e-964">Principal</span><span class="sxs-lookup"><span data-stu-id="93d0e-964">Core</span></span>
* <span data-ttu-id="93d0e-965">Modification du point de terminaison de l’autorité AAD `AZURE_US_GOV_CLOUD` pour le faire passer de login.microsoftonline.com à login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="93d0e-965">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="93d0e-966">Résolution du problème au cours duquel les données de télémétrie étaient constamment renvoyées</span><span class="sxs-lookup"><span data-stu-id="93d0e-966">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="93d0e-967">ACS</span><span class="sxs-lookup"><span data-stu-id="93d0e-967">ACS</span></span>

* <span data-ttu-id="93d0e-968">Ajout des commandes `aks install-connector` et `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="93d0e-968">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="93d0e-969">Amélioration des rapports d’erreurs pour `acs create`</span><span class="sxs-lookup"><span data-stu-id="93d0e-969">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="93d0e-970">Correction de l’utilisation de `aks get-credentials -f` sans chemin d’accès complet</span><span class="sxs-lookup"><span data-stu-id="93d0e-970">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="93d0e-971">Advisor</span><span class="sxs-lookup"><span data-stu-id="93d0e-971">Advisor</span></span>

* <span data-ttu-id="93d0e-972">Version initiale</span><span class="sxs-lookup"><span data-stu-id="93d0e-972">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="93d0e-973">AppService</span><span class="sxs-lookup"><span data-stu-id="93d0e-973">Appservice</span></span>

* <span data-ttu-id="93d0e-974">Correction de la génération du nom de certificat avec `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="93d0e-974">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="93d0e-975">Correction de `webapp [list|show]` et `functionapp [list|show]` de manière à afficher les applications correctes</span><span class="sxs-lookup"><span data-stu-id="93d0e-975">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="93d0e-976">Ajout de la valeur par défaut pour `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="93d0e-976">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="93d0e-977">Consommation</span><span class="sxs-lookup"><span data-stu-id="93d0e-977">Consumption</span></span>

* <span data-ttu-id="93d0e-978">Ajout de la prise en charge de l’API version 2017-11-30</span><span class="sxs-lookup"><span data-stu-id="93d0e-978">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="93d0e-979">Conteneur</span><span class="sxs-lookup"><span data-stu-id="93d0e-979">Container</span></span>

* <span data-ttu-id="93d0e-980">Correction de la régression des ports par défaut</span><span class="sxs-lookup"><span data-stu-id="93d0e-980">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="93d0e-981">Surveiller</span><span class="sxs-lookup"><span data-stu-id="93d0e-981">Monitor</span></span>

* <span data-ttu-id="93d0e-982">Ajout de la prise en charge de plusieurs dimensions à la commande des mesures</span><span class="sxs-lookup"><span data-stu-id="93d0e-982">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="93d0e-983">Ressource</span><span class="sxs-lookup"><span data-stu-id="93d0e-983">Resource</span></span>

* <span data-ttu-id="93d0e-984">Ajout de l’argument `--include-response-body` à `resource show`</span><span class="sxs-lookup"><span data-stu-id="93d0e-984">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="93d0e-985">Rôle</span><span class="sxs-lookup"><span data-stu-id="93d0e-985">Role</span></span>

* <span data-ttu-id="93d0e-986">Ajout de l’affichage des affectations par défaut pour les administrateurs « classiques » à `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="93d0e-986">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="93d0e-987">Ajout de la prise en charge à `ad sp reset-credentials` pour l’ajout d’informations d’identification au lieu de leur remplacement</span><span class="sxs-lookup"><span data-stu-id="93d0e-987">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="93d0e-988">Amélioration des rapports d’erreurs pour `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="93d0e-988">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="93d0e-989">SQL</span><span class="sxs-lookup"><span data-stu-id="93d0e-989">SQL</span></span>

* <span data-ttu-id="93d0e-990">Ajout des commandes `sql db list-usages` et `sql db show-usage`</span><span class="sxs-lookup"><span data-stu-id="93d0e-990">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="93d0e-991">Ajout des commandes `sql server conn-policy show` et `sql server conn-policy update`</span><span class="sxs-lookup"><span data-stu-id="93d0e-991">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="93d0e-992">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="93d0e-992">VM</span></span>

* <span data-ttu-id="93d0e-993">Ajout des informations de zone à `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="93d0e-993">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="93d0e-994">14 novembre 2017</span><span class="sxs-lookup"><span data-stu-id="93d0e-994">November 14, 2017</span></span>

<span data-ttu-id="93d0e-995">Version 2.0.21</span><span class="sxs-lookup"><span data-stu-id="93d0e-995">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="93d0e-996">ACR</span><span class="sxs-lookup"><span data-stu-id="93d0e-996">ACR</span></span>

* <span data-ttu-id="93d0e-997">Ajout de la prise en charge pour la création de webhooks dans les régions de réplication</span><span class="sxs-lookup"><span data-stu-id="93d0e-997">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="93d0e-998">ACS</span><span class="sxs-lookup"><span data-stu-id="93d0e-998">ACS</span></span>

* <span data-ttu-id="93d0e-999">Modification de toutes les mentions « agent » en « nœud » dans AKS</span><span class="sxs-lookup"><span data-stu-id="93d0e-999">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="93d0e-1000">Option `--orchestrator-release` déconseillée pour `acs create`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1000">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="93d0e-1001">Changement de la taille de machine virtuelle par défaut pour AKS à `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1001">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="93d0e-1002">Résolution de `az aks browse` sur Windows</span><span class="sxs-lookup"><span data-stu-id="93d0e-1002">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="93d0e-1003">Résolution de `az aks get-credentials` sur Windows</span><span class="sxs-lookup"><span data-stu-id="93d0e-1003">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="93d0e-1004">AppService</span><span class="sxs-lookup"><span data-stu-id="93d0e-1004">Appservice</span></span>

* <span data-ttu-id="93d0e-1005">Ajout de la source de déploiement `config-zip` pour les applications Web et de fonction</span><span class="sxs-lookup"><span data-stu-id="93d0e-1005">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="93d0e-1006">Ajout de l’option `--docker-container-logging` à `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1006">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="93d0e-1007">Suppression de l’option `storage` du paramètre `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1007">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="93d0e-1008">Amélioration des messages d’erreur pour `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1008">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="93d0e-1009">Ajout de la prise en charge pour la création d’applications de fonction Linux</span><span class="sxs-lookup"><span data-stu-id="93d0e-1009">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="93d0e-1010">`list-locations` fixe</span><span class="sxs-lookup"><span data-stu-id="93d0e-1010">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="93d0e-1011">Batch</span><span class="sxs-lookup"><span data-stu-id="93d0e-1011">Batch</span></span>

* <span data-ttu-id="93d0e-1012">Correction du bogue dans la commande de création de pool lorsqu’un ID ressource a été utilisé avec l’indicateur `--image`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1012">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="93d0e-1013">Batchai</span><span class="sxs-lookup"><span data-stu-id="93d0e-1013">Batchai</span></span>

* <span data-ttu-id="93d0e-1014">Ajout de l’option courte, `-s`, pour `--vm-size` quand la taille de machine virtuelle est fournie dans la commande `file-server create`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1014">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="93d0e-1015">Ajout du nom de compte de stockage et des arguments de clé dans les paramètres `cluster create`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1015">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="93d0e-1016">Résolution de la documentation pour `job list-files` et `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1016">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="93d0e-1017">Ajout de l’option courte, `-r`, pour `--cluster-name` quand le nom du cluster est fourni dans la commande `job create`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1017">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="93d0e-1018">Cloud</span><span class="sxs-lookup"><span data-stu-id="93d0e-1018">Cloud</span></span>

* <span data-ttu-id="93d0e-1019">Modification de `cloud [register|update]` pour empêcher l’inscription des clouds qui ne disposent pas de tous les points de terminaison requis</span><span class="sxs-lookup"><span data-stu-id="93d0e-1019">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="93d0e-1020">Conteneur</span><span class="sxs-lookup"><span data-stu-id="93d0e-1020">Container</span></span>

* <span data-ttu-id="93d0e-1021">Ajout de la prise en charge pour ouvrir plusieurs ports</span><span class="sxs-lookup"><span data-stu-id="93d0e-1021">Added support to open multiple ports</span></span>
* <span data-ttu-id="93d0e-1022">Ajout de la stratégie de redémarrage du groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="93d0e-1022">Added container group restart policy</span></span>
* <span data-ttu-id="93d0e-1023">Ajout de la prise en charge pour monter le partage de fichier Azure en tant que volume</span><span class="sxs-lookup"><span data-stu-id="93d0e-1023">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="93d0e-1024">Mise à jour des documents d’assistance</span><span class="sxs-lookup"><span data-stu-id="93d0e-1024">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="93d0e-1025">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="93d0e-1025">Data Lake Analytics</span></span>

* <span data-ttu-id="93d0e-1026">Modification de `[job|account] list` pour retourner des informations plus concises</span><span class="sxs-lookup"><span data-stu-id="93d0e-1026">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="93d0e-1027">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="93d0e-1027">Data Lake Store</span></span>

* <span data-ttu-id="93d0e-1028">Modification de `account list` pour retourner des informations plus concises</span><span class="sxs-lookup"><span data-stu-id="93d0e-1028">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="93d0e-1029">Extension</span><span class="sxs-lookup"><span data-stu-id="93d0e-1029">Extension</span></span>

* <span data-ttu-id="93d0e-1030">Ajout de `extension list-available` pour permettre l’affichage de la liste des extensions officielles Microsoft</span><span class="sxs-lookup"><span data-stu-id="93d0e-1030">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="93d0e-1031">Ajout de `--name` à `extension [add|update]` pour permettre l’installation des extensions par nom</span><span class="sxs-lookup"><span data-stu-id="93d0e-1031">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="93d0e-1032">IoT</span><span class="sxs-lookup"><span data-stu-id="93d0e-1032">IoT</span></span>

* <span data-ttu-id="93d0e-1033">Ajout de la prise en charge pour les autorités de certification (CA) et les chaînes d’approbation</span><span class="sxs-lookup"><span data-stu-id="93d0e-1033">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="93d0e-1034">Surveiller</span><span class="sxs-lookup"><span data-stu-id="93d0e-1034">Monitor</span></span>

* <span data-ttu-id="93d0e-1035">Ajout des commandes `activity-log alert`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1035">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="93d0e-1036">Réseau</span><span class="sxs-lookup"><span data-stu-id="93d0e-1036">Network</span></span>

* <span data-ttu-id="93d0e-1037">Ajout de la prise en charge pour les enregistrements DNS CAA</span><span class="sxs-lookup"><span data-stu-id="93d0e-1037">Added support for CAA DNS records</span></span>
* <span data-ttu-id="93d0e-1038">Résolution d’un problème empêchant la mise à jour des points de terminaison avec `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1038">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="93d0e-1039">Résolution d’un problème où `vnet update --dns-servers` ne fonctionnait pas, en fonction de la façon dont avait été créé le réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="93d0e-1039">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="93d0e-1040">Résolution d’un problème où les noms DNS relatifs n’étaient pas importés correctement par `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1040">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="93d0e-1041">Réservations</span><span class="sxs-lookup"><span data-stu-id="93d0e-1041">Reservations</span></span>

* <span data-ttu-id="93d0e-1042">Version préliminaire initiale</span><span class="sxs-lookup"><span data-stu-id="93d0e-1042">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="93d0e-1043">Ressource</span><span class="sxs-lookup"><span data-stu-id="93d0e-1043">Resource</span></span>

* <span data-ttu-id="93d0e-1044">Ajout de la prise en charge pour les ID de ressource au paramètre `--resource` et pour les verrous au niveau des ressources</span><span class="sxs-lookup"><span data-stu-id="93d0e-1044">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="93d0e-1045">SQL</span><span class="sxs-lookup"><span data-stu-id="93d0e-1045">SQL</span></span>

* <span data-ttu-id="93d0e-1046">Ajout du paramètre `--ignore-missing-vnet-service-endpoint` pour `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1046">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="93d0e-1047">Stockage</span><span class="sxs-lookup"><span data-stu-id="93d0e-1047">Storage</span></span>

* <span data-ttu-id="93d0e-1048">Modification de `storage account create` pour utiliser la référence SKU `Standard_RAGRS` par défaut</span><span class="sxs-lookup"><span data-stu-id="93d0e-1048">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="93d0e-1049">Correction du bogue lors du traitement des noms d’objets blob/de fichier qui incluent des caractères non-ascii</span><span class="sxs-lookup"><span data-stu-id="93d0e-1049">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="93d0e-1050">Correction du bogue qui empêchait l’utilisation de `--source-uri` avec `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1050">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="93d0e-1051">Ajout de commandes pour paramétrer et supprimer plusieurs objets avec `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1051">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="93d0e-1052">Résolution du problème de l’activation des métriques avec `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1052">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="93d0e-1053">Résolution du problème des fichiers de plus de 200 Go lors de l’utilisation de `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1053">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="93d0e-1054">Résolution du problème où `--bypass` et `--default-action` étaient ignorés par `storage account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1054">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="93d0e-1055">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="93d0e-1055">VM</span></span>

* <span data-ttu-id="93d0e-1056">Correction d’un bogue avec `vmss create` qui empêchait l’utilisation du niveau de taille `Basic`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1056">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="93d0e-1057">Ajout d’arguments `--plan` à `[vm|vmss] create` pour les images personnalisées avec des informations de facturation</span><span class="sxs-lookup"><span data-stu-id="93d0e-1057">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="93d0e-1058">Ajout des commandes `vm secret `[add|remove|list]</span><span class="sxs-lookup"><span data-stu-id="93d0e-1058">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="93d0e-1059">Renommage de `vm format-secret` en `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1059">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="93d0e-1060">Ajout de l’argument `--encrypt format` à `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1060">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="93d0e-1061">24 octobre 2017</span><span class="sxs-lookup"><span data-stu-id="93d0e-1061">October 24, 2017</span></span>

<span data-ttu-id="93d0e-1062">Version 2.0.20</span><span class="sxs-lookup"><span data-stu-id="93d0e-1062">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="93d0e-1063">Principal</span><span class="sxs-lookup"><span data-stu-id="93d0e-1063">Core</span></span>

* <span data-ttu-id="93d0e-1064">Mise à jour de `2017-03-09-profile` pour consommer l’API `MGMT_STORAGE` version `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1064">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="93d0e-1065">ACR</span><span class="sxs-lookup"><span data-stu-id="93d0e-1065">ACR</span></span>

* <span data-ttu-id="93d0e-1066">Mise à jour de la gestion des ressources pour pointer vers la version d’API `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1066">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="93d0e-1067">Modification de la référence SKU « Bring Your Own Storage » en Classique</span><span class="sxs-lookup"><span data-stu-id="93d0e-1067">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="93d0e-1068">Changement des noms des références SKU de registre en De base, Standard, et Premium</span><span class="sxs-lookup"><span data-stu-id="93d0e-1068">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="93d0e-1069">ACS</span><span class="sxs-lookup"><span data-stu-id="93d0e-1069">ACS</span></span>

* <span data-ttu-id="93d0e-1070">[PRÉVERSION] Ajout des commandes `az aks`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1070">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="93d0e-1071">Réparation de Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1071">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="93d0e-1072">AppService</span><span class="sxs-lookup"><span data-stu-id="93d0e-1072">Appservice</span></span>

* <span data-ttu-id="93d0e-1073">Résolution d’une erreur où le téléchargement des journaux `webapp` était incorrect</span><span class="sxs-lookup"><span data-stu-id="93d0e-1073">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="93d0e-1074">Composant</span><span class="sxs-lookup"><span data-stu-id="93d0e-1074">Component</span></span>

* <span data-ttu-id="93d0e-1075">Ajout de clarté dans les messages visant à déconseiller de tous les programmes d’installation et des invites de confirmation</span><span class="sxs-lookup"><span data-stu-id="93d0e-1075">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="93d0e-1076">Surveiller</span><span class="sxs-lookup"><span data-stu-id="93d0e-1076">Monitor</span></span>

* <span data-ttu-id="93d0e-1077">Ajout des commandes `action-group`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1077">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="93d0e-1078">Ressource</span><span class="sxs-lookup"><span data-stu-id="93d0e-1078">Resource</span></span>

* <span data-ttu-id="93d0e-1079">Résolution d’une incompatibilité de la dépendance msrest dans `group export` avec les versions les plus récentes</span><span class="sxs-lookup"><span data-stu-id="93d0e-1079">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="93d0e-1080">Résolution de `policy assignment create` pour qu’il fonctionne avec les définitions de stratégie et les définitions d’ensemble de stratégie intégrées</span><span class="sxs-lookup"><span data-stu-id="93d0e-1080">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="93d0e-1081">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="93d0e-1081">VM</span></span>

* <span data-ttu-id="93d0e-1082">Ajout de l’argument `--accelerated-networking` à `vmss create`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1082">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="93d0e-1083">9 octobre 2017</span><span class="sxs-lookup"><span data-stu-id="93d0e-1083">October 9, 2017</span></span>

<span data-ttu-id="93d0e-1084">Version 2.0.19</span><span class="sxs-lookup"><span data-stu-id="93d0e-1084">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="93d0e-1085">Principal</span><span class="sxs-lookup"><span data-stu-id="93d0e-1085">Core</span></span>

* <span data-ttu-id="93d0e-1086">Ajout de la gestion des URL d’autorisation AD FS avec une barre oblique à Azure Stack</span><span class="sxs-lookup"><span data-stu-id="93d0e-1086">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="93d0e-1087">AppService</span><span class="sxs-lookup"><span data-stu-id="93d0e-1087">Appservice</span></span>

* <span data-ttu-id="93d0e-1088">Ajout de la mise à jour générique avec la nouvelle commande `webapp update`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1088">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="93d0e-1089">Batch</span><span class="sxs-lookup"><span data-stu-id="93d0e-1089">Batch</span></span>

* <span data-ttu-id="93d0e-1090">Mis à jour du kit de développement logiciel (SDK) à la version 4.0.0</span><span class="sxs-lookup"><span data-stu-id="93d0e-1090">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="93d0e-1091">Mise à jour de l’option `--image` de VirtualMachineConfiguration pour prendre en charge les références d’image ARM en plus de publish:offre:sku:version</span><span class="sxs-lookup"><span data-stu-id="93d0e-1091">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="93d0e-1092">Ajout de la prise en charge du nouveau modèle d’extension CLI pour les commandes d’extension Batch</span><span class="sxs-lookup"><span data-stu-id="93d0e-1092">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="93d0e-1093">Suppression de la prise en charge Batch des modèles de composants</span><span class="sxs-lookup"><span data-stu-id="93d0e-1093">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="93d0e-1094">Batchai</span><span class="sxs-lookup"><span data-stu-id="93d0e-1094">Batchai</span></span>

* <span data-ttu-id="93d0e-1095">Version initiale du module Batch AI</span><span class="sxs-lookup"><span data-stu-id="93d0e-1095">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="93d0e-1096">KeyVault</span><span class="sxs-lookup"><span data-stu-id="93d0e-1096">Keyvault</span></span>

* <span data-ttu-id="93d0e-1097">Résolution du problème d’authentification Key Vault lors de l’utilisation d’AD FS sur Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="93d0e-1097">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="93d0e-1098">(#4448)</span><span class="sxs-lookup"><span data-stu-id="93d0e-1098">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="93d0e-1099">Réseau</span><span class="sxs-lookup"><span data-stu-id="93d0e-1099">Network</span></span>

* <span data-ttu-id="93d0e-1100">La modification de l’argument `--server` de `application-gateway address-pool create` devient facultative, permettant les pools d’adresses vides</span><span class="sxs-lookup"><span data-stu-id="93d0e-1100">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="93d0e-1101">Mise à jour de `traffic-manager` pour prendre en charge les fonctionnalités les plus récentes</span><span class="sxs-lookup"><span data-stu-id="93d0e-1101">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="93d0e-1102">Ressource</span><span class="sxs-lookup"><span data-stu-id="93d0e-1102">Resource</span></span>

* <span data-ttu-id="93d0e-1103">Ajout de la prise en charge des options `--resource-group/-g` pour le nom du groupe de ressources dans `group`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1103">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="93d0e-1104">Ajout des commandes à `account lock` pour travailler avec des verrous au niveau de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="93d0e-1104">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="93d0e-1105">Ajout des commandes à `group lock` pour travailler avec des verrous au niveau du groupe</span><span class="sxs-lookup"><span data-stu-id="93d0e-1105">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="93d0e-1106">Ajout des commandes à `resource lock` pour travailler avec des verrous au niveau des ressources</span><span class="sxs-lookup"><span data-stu-id="93d0e-1106">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="93d0e-1107">SQL</span><span class="sxs-lookup"><span data-stu-id="93d0e-1107">Sql</span></span>

* <span data-ttu-id="93d0e-1108">Ajout de la prise en charge pour le Chiffrement transparent des données (TDE) SQL et le chiffrement transparent des données avec Bring Your Own Key</span><span class="sxs-lookup"><span data-stu-id="93d0e-1108">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="93d0e-1109">Ajout de la commande `db list-deleted` et du paramètre `db restore --deleted-time`, ce qui offre la possibilité de rechercher et de restaurer les bases de données supprimées</span><span class="sxs-lookup"><span data-stu-id="93d0e-1109">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="93d0e-1110">Ajout de `db op list` et `db op cancel`, ce qui offre la capacité de répertorier et d’annuler des opérations en cours sur la base de données</span><span class="sxs-lookup"><span data-stu-id="93d0e-1110">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="93d0e-1111">Stockage</span><span class="sxs-lookup"><span data-stu-id="93d0e-1111">Storage</span></span>

* <span data-ttu-id="93d0e-1112">Ajout de la prise en charge d’instantané de partage de fichiers</span><span class="sxs-lookup"><span data-stu-id="93d0e-1112">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="93d0e-1113">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="93d0e-1113">Vm</span></span>

* <span data-ttu-id="93d0e-1114">Correction d’un bogue dans `vm show` où l’utilisation de `-d` a provoqué un incident dans les adresses IP privées manquantes</span><span class="sxs-lookup"><span data-stu-id="93d0e-1114">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="93d0e-1115">[VERSION PRÉLIMINAIRE] Ajout de la prise en charge de la mise à niveau propagée pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1115">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="93d0e-1116">Ajout de la prise en charge de la mise à jour des paramètres de chiffrement avec `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1116">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="93d0e-1117">Ajout du paramètre `--os-disk-size-gb` pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1117">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="93d0e-1118">Ajout du paramètre `--license-type` de Windows pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1118">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="93d0e-1119">22 septembre 2017</span><span class="sxs-lookup"><span data-stu-id="93d0e-1119">September 22, 2017</span></span>

<span data-ttu-id="93d0e-1120">Version 2.0.18</span><span class="sxs-lookup"><span data-stu-id="93d0e-1120">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="93d0e-1121">Ressource</span><span class="sxs-lookup"><span data-stu-id="93d0e-1121">Resource</span></span>

* <span data-ttu-id="93d0e-1122">Ajout de la prise en charge de l’affichage des définitions de stratégie intégrée</span><span class="sxs-lookup"><span data-stu-id="93d0e-1122">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="93d0e-1123">Ajout de la prise en charge du paramètre de mode pour la création de définitions de stratégie</span><span class="sxs-lookup"><span data-stu-id="93d0e-1123">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="93d0e-1124">Ajout de la prise en charge des définitions d’interface utilisateur et des modèles pour `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1124">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="93d0e-1125">[CHANGEMENT CASSANT] Modification du type de ressource `managedapp` de `appliances` en `applications` et de `applianceDefinitions` en `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1125">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="93d0e-1126">Réseau</span><span class="sxs-lookup"><span data-stu-id="93d0e-1126">Network</span></span>

* <span data-ttu-id="93d0e-1127">Ajout de la prise en charge de la zone de disponibilité aux sous-commandes `network lb` et `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1127">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="93d0e-1128">Ajout de la prise en charge de l’homologation Microsoft IPv6 pour `express-route`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1128">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="93d0e-1129">Ajout des commandes du groupe de sécurité d’application `asg`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1129">Added `asg` application security group commands</span></span>
* <span data-ttu-id="93d0e-1130">Ajout de l’argument `--application-security-groups` à `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1130">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="93d0e-1131">Ajout des arguments `--source-asgs` et `--destination-asgs` à `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1131">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="93d0e-1132">Ajout des arguments `--ddos-protection` et `--vm-protection` à `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1132">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="93d0e-1133">Ajout des commandes `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1133">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="93d0e-1134">Stockage</span><span class="sxs-lookup"><span data-stu-id="93d0e-1134">Storage</span></span>

* <span data-ttu-id="93d0e-1135">Résolution d’un problème qui pouvait causer l’échec des commandes `storage account network-rule` après la mise à jour du Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="93d0e-1135">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="93d0e-1136">Événement</span><span class="sxs-lookup"><span data-stu-id="93d0e-1136">Eventgrid</span></span>

* <span data-ttu-id="93d0e-1137">Mise à jour du Kit de développement logiciel (SDK) Python Azure Event Grid afin d’utiliser une version plus récente de l’API « 2017-09-15-preview »</span><span class="sxs-lookup"><span data-stu-id="93d0e-1137">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="93d0e-1138">SQL</span><span class="sxs-lookup"><span data-stu-id="93d0e-1138">SQL</span></span>

* <span data-ttu-id="93d0e-1139">La modification de l’`sql server list`argument`--resource-group` devient facultative.</span><span class="sxs-lookup"><span data-stu-id="93d0e-1139">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="93d0e-1140">En l’absence de précisions, tous les serveurs SQL dans l’abonnement seront retournés</span><span class="sxs-lookup"><span data-stu-id="93d0e-1140">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="93d0e-1141">Ajout du paramètre `--no-wait` à `db [create|copy|restore|update|replica create|create|update]` et `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1141">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="93d0e-1142">KeyVault</span><span class="sxs-lookup"><span data-stu-id="93d0e-1142">Keyvault</span></span>

* <span data-ttu-id="93d0e-1143">Ajout de la prise en charge des commandes Keyvault derrière un proxy</span><span class="sxs-lookup"><span data-stu-id="93d0e-1143">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="93d0e-1144">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="93d0e-1144">VM</span></span>

* <span data-ttu-id="93d0e-1145">Ajout de la prise en charge de zone de disponibilité pour `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1145">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="93d0e-1146">Résolution d’un problème à cause duquel l’utilisation de `--app-gateway ID` avec `vmss create` entraînait un échec</span><span class="sxs-lookup"><span data-stu-id="93d0e-1146">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="93d0e-1147">Ajout de l’argument `--asgs` à `vm create`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1147">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="93d0e-1148">Ajout de la prise en charge des commandes en cours d’exécution sur des machines virtuelles avec `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1148">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="93d0e-1149">[PRÉVERSION] Ajout de la prise en charge du chiffrement de disque VMSS avec `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1149">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="93d0e-1150">Ajout de la prise en charge de la réalisation de la maintenance sur des machines virtuelles avec `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1150">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="93d0e-1151">ACS</span><span class="sxs-lookup"><span data-stu-id="93d0e-1151">ACS</span></span>

* <span data-ttu-id="93d0e-1152">[PRÉVERSION] Ajout de l’argument `--orchestrator-release` à `acs create` pour les régions ACS en préversion</span><span class="sxs-lookup"><span data-stu-id="93d0e-1152">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="93d0e-1153">AppService</span><span class="sxs-lookup"><span data-stu-id="93d0e-1153">Appservice</span></span>

* <span data-ttu-id="93d0e-1154">Ajout de la capacité à mettre à jour et à afficher les paramètres d’authentification avec `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1154">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="93d0e-1155">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="93d0e-1155">Backup</span></span>

* <span data-ttu-id="93d0e-1156">Version préliminaire</span><span class="sxs-lookup"><span data-stu-id="93d0e-1156">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="93d0e-1157">11 septembre 2017</span><span class="sxs-lookup"><span data-stu-id="93d0e-1157">September 11, 2017</span></span>

<span data-ttu-id="93d0e-1158">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="93d0e-1158">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="93d0e-1159">Principal</span><span class="sxs-lookup"><span data-stu-id="93d0e-1159">Core</span></span>

* <span data-ttu-id="93d0e-1160">Module de commande activé pour définir son propre ID de corrélation dans la télémétrie</span><span class="sxs-lookup"><span data-stu-id="93d0e-1160">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="93d0e-1161">Résolution du problème de vidage JSON lorsque la télémétrie est définie en mode diagnostics</span><span class="sxs-lookup"><span data-stu-id="93d0e-1161">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="93d0e-1162">Acs</span><span class="sxs-lookup"><span data-stu-id="93d0e-1162">Acs</span></span>

* <span data-ttu-id="93d0e-1163">Ajout de la commande `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1163">Added `acs list-locations` command</span></span>
* <span data-ttu-id="93d0e-1164">Faire en sorte que `ssh-key-file` soit fourni avec la valeur par défaut attendu</span><span class="sxs-lookup"><span data-stu-id="93d0e-1164">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="93d0e-1165">AppService</span><span class="sxs-lookup"><span data-stu-id="93d0e-1165">Appservice</span></span>

* <span data-ttu-id="93d0e-1166">Ajout de la possibilité de créer une application web dans un groupe de ressources autre que celui du plan de service actif</span><span class="sxs-lookup"><span data-stu-id="93d0e-1166">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="93d0e-1167">CDN</span><span class="sxs-lookup"><span data-stu-id="93d0e-1167">CDN</span></span>

* <span data-ttu-id="93d0e-1168">Correction du bogue « CustomDomain n’est pas itérable » pour `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1168">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="93d0e-1169">Extension</span><span class="sxs-lookup"><span data-stu-id="93d0e-1169">Extension</span></span>

* <span data-ttu-id="93d0e-1170">Version initiale</span><span class="sxs-lookup"><span data-stu-id="93d0e-1170">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="93d0e-1171">KeyVault</span><span class="sxs-lookup"><span data-stu-id="93d0e-1171">Keyvault</span></span>

* <span data-ttu-id="93d0e-1172">Résolution du problème où les autorisations étaient sensibles à la casse pour `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1172">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="93d0e-1173">Réseau</span><span class="sxs-lookup"><span data-stu-id="93d0e-1173">Network</span></span>

* <span data-ttu-id="93d0e-1174">Renommage de `vnet list-private-access-services` en `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1174">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="93d0e-1175">Argument `--private-access-services` renommé en `--service-endpoints` pour`vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1175">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="93d0e-1176">Ajout de la prise en charge de plusieurs plages IP et de ports à `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1176">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="93d0e-1177">Ajout de la prise en charge de la référence (SKU) pour `lb create`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1177">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="93d0e-1178">Ajout de la prise en charge de la référence (SKU) pour `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1178">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="93d0e-1179">Ressource</span><span class="sxs-lookup"><span data-stu-id="93d0e-1179">Resource</span></span>

* <span data-ttu-id="93d0e-1180">Autoriser le passages dans les définitions de paramètres de stratégie de ressource dans `policy definition create`, et`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1180">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="93d0e-1181">Autoriser le passage dans les valeurs de paramètres pour `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1181">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="93d0e-1182">Autoriser le passage de JSON ou d’un fichier pour tous les paramètres</span><span class="sxs-lookup"><span data-stu-id="93d0e-1182">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="93d0e-1183">Incrémentation de la version de l’API</span><span class="sxs-lookup"><span data-stu-id="93d0e-1183">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="93d0e-1184">SQL</span><span class="sxs-lookup"><span data-stu-id="93d0e-1184">SQL</span></span>

* <span data-ttu-id="93d0e-1185">Ajout des commandes `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1185">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="93d0e-1186">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="93d0e-1186">VM</span></span>

* <span data-ttu-id="93d0e-1187">Résolu : n’affecte aucun accès tant que `--scope` n’est pas indiqué</span><span class="sxs-lookup"><span data-stu-id="93d0e-1187">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="93d0e-1188">Résolu : utilisation de la même dénomination d’extension que celle du portail</span><span class="sxs-lookup"><span data-stu-id="93d0e-1188">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="93d0e-1189">Suppression de `subscription` de la sortie `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1189">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="93d0e-1190">Résolu : la référence SKU de stockage `[vm|vmss] create` n’est pas appliquée sur les disques de données avec une image</span><span class="sxs-lookup"><span data-stu-id="93d0e-1190">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="93d0e-1191">Résolu : `vm format-secret --secrets` n’accepte pas d’ID séparés par un saut de ligne</span><span class="sxs-lookup"><span data-stu-id="93d0e-1191">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="93d0e-1192">31 août 2017</span><span class="sxs-lookup"><span data-stu-id="93d0e-1192">August 31, 2017</span></span>

<span data-ttu-id="93d0e-1193">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="93d0e-1193">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="93d0e-1194">KeyVault</span><span class="sxs-lookup"><span data-stu-id="93d0e-1194">Keyvault</span></span>

* <span data-ttu-id="93d0e-1195">Correction d’un bogue à cause duquel vous tentez de résoudre automatiquement l’encodage secret avec `secret download`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1195">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="93d0e-1196">Sf</span><span class="sxs-lookup"><span data-stu-id="93d0e-1196">Sf</span></span>

* <span data-ttu-id="93d0e-1197">Déconseiller toutes les commandes en faveur de Service Fabric CLI (sfctl)</span><span class="sxs-lookup"><span data-stu-id="93d0e-1197">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="93d0e-1198">Stockage</span><span class="sxs-lookup"><span data-stu-id="93d0e-1198">Storage</span></span>

* <span data-ttu-id="93d0e-1199">Résolution du problème dans lequel la création de comptes de stockage dans les régions ne prenant pas en charge la fonctionnalité NetworkACLs était impossible</span><span class="sxs-lookup"><span data-stu-id="93d0e-1199">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="93d0e-1200">Déterminer le type de contenu et l’encodage du contenu lors du chargement d’objets blob et de fichiers si aucun type de contenu et d’encodage n’est spécifié.</span><span class="sxs-lookup"><span data-stu-id="93d0e-1200">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="93d0e-1201">28 août 2017</span><span class="sxs-lookup"><span data-stu-id="93d0e-1201">August 28, 2017</span></span>

<span data-ttu-id="93d0e-1202">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="93d0e-1202">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="93d0e-1203">Interface de ligne de commande</span><span class="sxs-lookup"><span data-stu-id="93d0e-1203">CLI</span></span>

* <span data-ttu-id="93d0e-1204">Ajout d’une remarque juridique pour `--version`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1204">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="93d0e-1205">ACS</span><span class="sxs-lookup"><span data-stu-id="93d0e-1205">ACS</span></span>

* <span data-ttu-id="93d0e-1206">Correction des régions d’aperçu</span><span class="sxs-lookup"><span data-stu-id="93d0e-1206">Corrected preview regions</span></span>
* <span data-ttu-id="93d0e-1207">Mise en forme par défaut `dns_name_prefix` correctement</span><span class="sxs-lookup"><span data-stu-id="93d0e-1207">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="93d0e-1208">Optimisation de la sortie de commande des services ACS</span><span class="sxs-lookup"><span data-stu-id="93d0e-1208">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="93d0e-1209">AppService</span><span class="sxs-lookup"><span data-stu-id="93d0e-1209">Appservice</span></span>

* <span data-ttu-id="93d0e-1210">[CHANGEMENT CASSANT] Fixation des incohérences dans la sortie de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1210">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="93d0e-1211">Ajout d’un nouvel alias de `-i` pour `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1211">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="93d0e-1212">Exposé `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1212">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="93d0e-1213">Exposition de nouveaux arguments à partir de `az webapp delete` pour conserver le plan de service d'application, les métriques ou l’inscription DNS</span><span class="sxs-lookup"><span data-stu-id="93d0e-1213">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="93d0e-1214">Problème résolu : Détecter les paramètres d’emplacement correctement</span><span class="sxs-lookup"><span data-stu-id="93d0e-1214">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="93d0e-1215">IoT</span><span class="sxs-lookup"><span data-stu-id="93d0e-1215">IoT</span></span>

* <span data-ttu-id="93d0e-1216">Résolu #3934 : La création de la stratégie n’efface plus les stratégies existantes</span><span class="sxs-lookup"><span data-stu-id="93d0e-1216">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="93d0e-1217">Réseau</span><span class="sxs-lookup"><span data-stu-id="93d0e-1217">Network</span></span>

* <span data-ttu-id="93d0e-1218">[CHANGEMENT CASSANT] Renommage de `vnet list-private-access-services` en `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1218">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="93d0e-1219">[CHANGEMENT CASSANT] Renommage de l’option `--private-access-services` en `--service-endpoints` pour `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1219">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="93d0e-1220">Ajout de la prise en charge de plusieurs IP et de plusieurs pages de port pour `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1220">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="93d0e-1221">Ajout de la prise en charge de la référence (SKU) pour `lb create`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1221">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="93d0e-1222">Ajout de la prise en charge de la référence (SKU) pour `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1222">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="93d0e-1223">Profil</span><span class="sxs-lookup"><span data-stu-id="93d0e-1223">Profile</span></span>

* <span data-ttu-id="93d0e-1224">exposés `--msi` et `--msi-port` pour vous connecter à l’aide d’une identité de machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="93d0e-1224">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="93d0e-1225">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="93d0e-1225">Service Fabric</span></span>

* <span data-ttu-id="93d0e-1226">Version préliminaire</span><span class="sxs-lookup"><span data-stu-id="93d0e-1226">Preview release</span></span>
* <span data-ttu-id="93d0e-1227">Règles d’utilisateur du Registre/de mot de passe simplifiées pour la commande</span><span class="sxs-lookup"><span data-stu-id="93d0e-1227">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="93d0e-1228">Invite de mot de passe fixe pour l’utilisateur, même après le passage de paramètre</span><span class="sxs-lookup"><span data-stu-id="93d0e-1228">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="93d0e-1229">Ajout de la prise en charge de vide `registry_cred`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1229">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="93d0e-1230">Stockage</span><span class="sxs-lookup"><span data-stu-id="93d0e-1230">Storage</span></span>

* <span data-ttu-id="93d0e-1231">Paramétrage du niveau blob activé</span><span class="sxs-lookup"><span data-stu-id="93d0e-1231">Enabled setting blob tier</span></span>
* <span data-ttu-id="93d0e-1232">Ajout des arguments `--bypass` et `--default-action` à `storage account [create|update]` pour la prise en charge du tunneling de service</span><span class="sxs-lookup"><span data-stu-id="93d0e-1232">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="93d0e-1233">Ajout de commandes permettant d’ajouter des règles de réseau virtuel et des règles basées sur IP à `storage account network-rule`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1233">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="93d0e-1234">Activation du chiffrement du service par la clé gérée du client</span><span class="sxs-lookup"><span data-stu-id="93d0e-1234">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="93d0e-1235">[CHANGEMENT CASSANT] Renommage de l’option `--encryption` en `--encryption-services` pour la commande `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1235">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="93d0e-1236">Problème résolu #4220 : `az storage account update encryption` - incompatibilité de syntaxe</span><span class="sxs-lookup"><span data-stu-id="93d0e-1236">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="93d0e-1237">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="93d0e-1237">VM</span></span>

* <span data-ttu-id="93d0e-1238">Correction d’un problème qui entraînait l’affichage d’informations supplémentaires erronées pour `vmss get-instance-view` lors de l’utilisation `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1238">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="93d0e-1239">Ajout de la prise en charge de `--lb-sku` pour `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="93d0e-1239">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="93d0e-1240">Suppression des noms humains de la liste rouge du nom de l’administrateur pour `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1240">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="93d0e-1241">Correction d’un problème qui entraînait `[vm|vmss] create` la levée d’une erreur si la commande ne parvenait pas à extraire des informations de plan à partir d’une image</span><span class="sxs-lookup"><span data-stu-id="93d0e-1241">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="93d0e-1242">Correction d’un incident qui se produisait lors de la création d’un groupe identique VMMD avec un équilibrage de charge (LB) interne</span><span class="sxs-lookup"><span data-stu-id="93d0e-1242">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="93d0e-1243">Correction d’un problème qui empêchait `--no-wait` le fonctionnement d’un argument avec `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1243">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="93d0e-1244">15 août 2017</span><span class="sxs-lookup"><span data-stu-id="93d0e-1244">August 15, 2017</span></span>

<span data-ttu-id="93d0e-1245">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="93d0e-1245">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="93d0e-1246">ACS</span><span class="sxs-lookup"><span data-stu-id="93d0e-1246">ACS</span></span>

* <span data-ttu-id="93d0e-1247">Correction du numéro de port sshMaster0 pour kubernetes</span><span class="sxs-lookup"><span data-stu-id="93d0e-1247">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="93d0e-1248">AppService</span><span class="sxs-lookup"><span data-stu-id="93d0e-1248">Appservice</span></span>

* <span data-ttu-id="93d0e-1249">Correction d’une exception qui se produisait lors de la création d’une nouvelle application web Linux basée sur git</span><span class="sxs-lookup"><span data-stu-id="93d0e-1249">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="93d0e-1250">Event Grid</span><span class="sxs-lookup"><span data-stu-id="93d0e-1250">Event Grid</span></span>

* <span data-ttu-id="93d0e-1251">Ajout de dépendances du kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="93d0e-1251">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="93d0e-1252">11 août 2017</span><span class="sxs-lookup"><span data-stu-id="93d0e-1252">August 11, 2017</span></span>

<span data-ttu-id="93d0e-1253">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="93d0e-1253">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="93d0e-1254">ACS</span><span class="sxs-lookup"><span data-stu-id="93d0e-1254">ACS</span></span>

* <span data-ttu-id="93d0e-1255">Ajout de nouvelles régions d’aperçu</span><span class="sxs-lookup"><span data-stu-id="93d0e-1255">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="93d0e-1256">Batch</span><span class="sxs-lookup"><span data-stu-id="93d0e-1256">Batch</span></span>

* <span data-ttu-id="93d0e-1257">Mise à jour vers Kit de développement logiciel (DSK) de lot 3.1.0 et Kit de développement logiciel (SDK) de gestion de lot 4.1.0</span><span class="sxs-lookup"><span data-stu-id="93d0e-1257">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="93d0e-1258">Ajout d'une nouvelle commande affichant le nombre de tâches d’un travail</span><span class="sxs-lookup"><span data-stu-id="93d0e-1258">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="93d0e-1259">Correction du bogue dans le traitement de l’URL de la signature d'accès partagé du fichier de ressources</span><span class="sxs-lookup"><span data-stu-id="93d0e-1259">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="93d0e-1260">Point de terminaison de compte Batch prend désormais en charge le préfixe « https:// » facultatif</span><span class="sxs-lookup"><span data-stu-id="93d0e-1260">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="93d0e-1261">Prise en charge de l’ajout des listes de plus de 100 tâches à un travail</span><span class="sxs-lookup"><span data-stu-id="93d0e-1261">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="93d0e-1262">Ajout de l’enregistrement de débogage pour le chargement du module de commande Extensions</span><span class="sxs-lookup"><span data-stu-id="93d0e-1262">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="93d0e-1263">Composant</span><span class="sxs-lookup"><span data-stu-id="93d0e-1263">Component</span></span>

* <span data-ttu-id="93d0e-1264">Ajout d’un avertissement de désapprobation aux commandes « az component »</span><span class="sxs-lookup"><span data-stu-id="93d0e-1264">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="93d0e-1265">Conteneur</span><span class="sxs-lookup"><span data-stu-id="93d0e-1265">Container</span></span>

* <span data-ttu-id="93d0e-1266">`create` : correction d’un problème qui empêchait l’autorisation de signe égal à l’intérieur d’une variable d’environnement</span><span class="sxs-lookup"><span data-stu-id="93d0e-1266">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="93d0e-1267">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="93d0e-1267">Data Lake Store</span></span>

* <span data-ttu-id="93d0e-1268">Contrôle de progression activé</span><span class="sxs-lookup"><span data-stu-id="93d0e-1268">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="93d0e-1269">Event Grid</span><span class="sxs-lookup"><span data-stu-id="93d0e-1269">Event Grid</span></span>

* <span data-ttu-id="93d0e-1270">Version initiale</span><span class="sxs-lookup"><span data-stu-id="93d0e-1270">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="93d0e-1271">Réseau</span><span class="sxs-lookup"><span data-stu-id="93d0e-1271">Network</span></span>

* <span data-ttu-id="93d0e-1272">`lb` : correction d’un problème qui empêchait certains noms de ressources enfant d’être résolus correctement lorsqu’ils étaient omis</span><span class="sxs-lookup"><span data-stu-id="93d0e-1272">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="93d0e-1273">`application-gateway {subresource} delete` : correction d’un problème en raison duquel `--no-wait` n’était pas honorée</span><span class="sxs-lookup"><span data-stu-id="93d0e-1273">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="93d0e-1274">`application-gateway http-settings update` : correction d’un problème `--connection-draining-timeout` qui empêchait la désactivation de</span><span class="sxs-lookup"><span data-stu-id="93d0e-1274">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="93d0e-1275">Correction de erreur argument du mot-clé inattendu `sa_data_size_kilobyes` avec`az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1275">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="93d0e-1276">Profil</span><span class="sxs-lookup"><span data-stu-id="93d0e-1276">Profile</span></span>

* <span data-ttu-id="93d0e-1277">`account list` : ajout de `--refresh` pour synchroniser les derniers abonnements à partir du serveur</span><span class="sxs-lookup"><span data-stu-id="93d0e-1277">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="93d0e-1278">Stockage</span><span class="sxs-lookup"><span data-stu-id="93d0e-1278">Storage</span></span>

* <span data-ttu-id="93d0e-1279">Activer le compte de stockage de mise à jour avec l’identité attribuée par le système</span><span class="sxs-lookup"><span data-stu-id="93d0e-1279">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="93d0e-1280">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="93d0e-1280">VM</span></span>

* <span data-ttu-id="93d0e-1281">`availability-set` : nombre de domaines d’erreur exposé sur convert</span><span class="sxs-lookup"><span data-stu-id="93d0e-1281">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="93d0e-1282">Commande `list-skus` exposée</span><span class="sxs-lookup"><span data-stu-id="93d0e-1282">Exposed `list-skus` command</span></span>
* <span data-ttu-id="93d0e-1283">Prise en charge pour affecter l’identité avec ou sans création d’attributions de rôle</span><span class="sxs-lookup"><span data-stu-id="93d0e-1283">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="93d0e-1284">Appliquer la référence (SKU) de stockage lors de l’attachement de disques de données</span><span class="sxs-lookup"><span data-stu-id="93d0e-1284">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="93d0e-1285">Suppression du nom du disque du système d’exploitation par défaut et de la référence (SKU) de stockage lors de l’utilisation des disques gérés</span><span class="sxs-lookup"><span data-stu-id="93d0e-1285">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="93d0e-1286">28 juillet 2017</span><span class="sxs-lookup"><span data-stu-id="93d0e-1286">July 28, 2017</span></span>

<span data-ttu-id="93d0e-1287">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="93d0e-1287">Version 2.0.12</span></span>

* <span data-ttu-id="93d0e-1288">Ajout de commandes de conteneur</span><span class="sxs-lookup"><span data-stu-id="93d0e-1288">Added container commands</span></span>
* <span data-ttu-id="93d0e-1289">Ajout de modules de facturation et de consommation</span><span class="sxs-lookup"><span data-stu-id="93d0e-1289">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="93d0e-1290">Principal</span><span class="sxs-lookup"><span data-stu-id="93d0e-1290">Core</span></span>

* <span data-ttu-id="93d0e-1291">Informations d’authentification du Kit de développement logiciel (SDK) de sortie pour les principaux de service avec des certificats</span><span class="sxs-lookup"><span data-stu-id="93d0e-1291">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="93d0e-1292">Correction des exceptions de progression de déploiement</span><span class="sxs-lookup"><span data-stu-id="93d0e-1292">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="93d0e-1293">Utiliser le point de terminaison ARM à partir du cloud actuel pour créer le client de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="93d0e-1293">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="93d0e-1294">Amélioration de la gestion simultanée de fichiers clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="93d0e-1294">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="93d0e-1295">Actualiser l’ID de la demande client pour chaque exécution de la commande</span><span class="sxs-lookup"><span data-stu-id="93d0e-1295">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="93d0e-1296">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel ( SDK) (#3635)</span><span class="sxs-lookup"><span data-stu-id="93d0e-1296">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="93d0e-1297">Rapports de progression pour les déploiements de modèle (#3510)</span><span class="sxs-lookup"><span data-stu-id="93d0e-1297">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="93d0e-1298">Ajout de la prise en charge des champs de sortie de la table de prélèvement via la requête jmespath (#3581)</span><span class="sxs-lookup"><span data-stu-id="93d0e-1298">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="93d0e-1299">Amélioration de la désactivation des arguments d’analyse et de l’historique Ajout avec des mouvements (#3434)</span><span class="sxs-lookup"><span data-stu-id="93d0e-1299">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="93d0e-1300">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="93d0e-1300">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="93d0e-1301">Déplacer tous les fichiers d’enregistrement existant vers le dernier dossier</span><span class="sxs-lookup"><span data-stu-id="93d0e-1301">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="93d0e-1302">Correction de l’idempotence pour VM/VMSS create (#3586)</span><span class="sxs-lookup"><span data-stu-id="93d0e-1302">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="93d0e-1303">Les chemins d’accès de la commande ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="93d0e-1303">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="93d0e-1304">Certains paramètres de type booléen ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="93d0e-1304">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="93d0e-1305">Prise en charge de la connexion à ADFS sur le serveur local de manière identique à Azure Stack</span><span class="sxs-lookup"><span data-stu-id="93d0e-1305">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="93d0e-1306">Correction des écritures simultanées dans clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="93d0e-1306">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="93d0e-1307">ACR</span><span class="sxs-lookup"><span data-stu-id="93d0e-1307">ACR</span></span>

* <span data-ttu-id="93d0e-1308">Ajout de la commande `show-usage` pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="93d0e-1308">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="93d0e-1309">Prise en charge de la mise à jour de la référence (SKU) pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="93d0e-1309">Support SKU update for managed registries</span></span>
* <span data-ttu-id="93d0e-1310">Ajout de registres gérés avec la référence (SKU) gérée</span><span class="sxs-lookup"><span data-stu-id="93d0e-1310">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="93d0e-1311">Ajout de webhooks pour les registres gérés avec le module de commande acr webhook</span><span class="sxs-lookup"><span data-stu-id="93d0e-1311">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="93d0e-1312">Ajout de l’authentification AAD avec la commande de connexion acr</span><span class="sxs-lookup"><span data-stu-id="93d0e-1312">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="93d0e-1313">Ajout de la commande de suppression pour les référentiels docker, les manifestes et les balises</span><span class="sxs-lookup"><span data-stu-id="93d0e-1313">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="93d0e-1314">ACS</span><span class="sxs-lookup"><span data-stu-id="93d0e-1314">ACS</span></span>

* <span data-ttu-id="93d0e-1315">Prise en charge des API version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="93d0e-1315">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="93d0e-1316">AppService</span><span class="sxs-lookup"><span data-stu-id="93d0e-1316">Appservice</span></span>

* <span data-ttu-id="93d0e-1317">Correction d’un bogue à cause duquel l’énumération d’une application Linux ne retournait absolument rien</span><span class="sxs-lookup"><span data-stu-id="93d0e-1317">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="93d0e-1318">Prise en charge de la récupération de références depuis ACR</span><span class="sxs-lookup"><span data-stu-id="93d0e-1318">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="93d0e-1319">Supprimer toutes les commandes sous `appservice web`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1319">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="93d0e-1320">Masquer les mots de passe du registre docker de la commande de sortie (#3656)</span><span class="sxs-lookup"><span data-stu-id="93d0e-1320">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="93d0e-1321">Vérifier que le navigateur par défaut est utilisé sur macOs sans erreurs (#3623)</span><span class="sxs-lookup"><span data-stu-id="93d0e-1321">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="93d0e-1322">Améliorer l’aide de `webapp log tail` et `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="93d0e-1322">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="93d0e-1323">Commandes `traffic-routing` exposées pour configurer le routage statique (#3566)</span><span class="sxs-lookup"><span data-stu-id="93d0e-1323">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="93d0e-1324">Ajout de correctifs de fiabilité pour la configuration du contrôle de code source (#3245)</span><span class="sxs-lookup"><span data-stu-id="93d0e-1324">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="93d0e-1325">Suppression d’un argument non pris en charge `--node-version` de `webapp config update` pour les applications Web de Windows.</span><span class="sxs-lookup"><span data-stu-id="93d0e-1325">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="93d0e-1326">Utilisez à la place `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1326">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="93d0e-1327">Batch</span><span class="sxs-lookup"><span data-stu-id="93d0e-1327">Batch</span></span>

* <span data-ttu-id="93d0e-1328">Mise à jour vers kit de développement logiciel (SDK) de lot 3.0.0 avec prise en charge pour les machines virtuelles de faible priorité dans des pools</span><span class="sxs-lookup"><span data-stu-id="93d0e-1328">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="93d0e-1329">Renommage `pool create` option `--target-dedicated` en `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1329">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="93d0e-1330">Ajout des options `pool create`, `--target-low-priority-nodes` et `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1330">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="93d0e-1331">CDN</span><span class="sxs-lookup"><span data-stu-id="93d0e-1331">CDN</span></span>

* <span data-ttu-id="93d0e-1332">Fourniture d’un meilleur message d’erreur pour `cdn endpoint list` quand le profil spécifié par `--profile-name` n’existe pas</span><span class="sxs-lookup"><span data-stu-id="93d0e-1332">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="93d0e-1333">Cloud</span><span class="sxs-lookup"><span data-stu-id="93d0e-1333">Cloud</span></span>

* <span data-ttu-id="93d0e-1334">Modification de la version de l’API du point de terminaison de métadonnées du cloud au format AAAA-MM-JJ</span><span class="sxs-lookup"><span data-stu-id="93d0e-1334">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="93d0e-1335">Le point de terminaison de la galerie n’est pas nécessaire</span><span class="sxs-lookup"><span data-stu-id="93d0e-1335">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="93d0e-1336">Prise en charge de l’inscription du cloud, avec le point de terminaison ARM resource manager</span><span class="sxs-lookup"><span data-stu-id="93d0e-1336">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="93d0e-1337">Ajout d’une option pour `cloud set` permettant de choisir le profil lors de la sélection du cloud actuel</span><span class="sxs-lookup"><span data-stu-id="93d0e-1337">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="93d0e-1338">Exposé `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1338">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="93d0e-1339">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="93d0e-1339">CosmosDB</span></span>

* <span data-ttu-id="93d0e-1340">Correction relative à la permission de la création de collection avec une clé de partition personnalisée</span><span class="sxs-lookup"><span data-stu-id="93d0e-1340">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="93d0e-1341">Ajout de la prise en charge de la durée de vie par défaut de la collection</span><span class="sxs-lookup"><span data-stu-id="93d0e-1341">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="93d0e-1342">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="93d0e-1342">Data Lake Analytics</span></span>

* <span data-ttu-id="93d0e-1343">Ajout de commandes pour la gestion de la stratégie de calcul sous le titre `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1343">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="93d0e-1344">Ajout de `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1344">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="93d0e-1345">Ajout de `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1345">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="93d0e-1346">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="93d0e-1346">Data Lake Store</span></span>

* <span data-ttu-id="93d0e-1347">Ajout de la prise en charge pour la rotation de coffre de clés gérés par l’utilisateur dans `dls account update`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1347">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="93d0e-1348">Mise à jour de la version du kit de développement logiciel (SDK) du système de fichiers Data Lake Store sous-jacente, réglant un problème de performance</span><span class="sxs-lookup"><span data-stu-id="93d0e-1348">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="93d0e-1349">Ajout de la commande `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="93d0e-1349">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="93d0e-1350">Cette commande tente d’activer un utilisateur de coffre de clés fourni par l’utilisateur pour utiliser le chiffrement des données dans un compte Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="93d0e-1350">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="93d0e-1351">Interactive</span><span class="sxs-lookup"><span data-stu-id="93d0e-1351">Interactive</span></span>

* <span data-ttu-id="93d0e-1352">Amélioration du temps de démarrage à l’aide des commandes en cache</span><span class="sxs-lookup"><span data-stu-id="93d0e-1352">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="93d0e-1353">Couverture de test accrue</span><span class="sxs-lookup"><span data-stu-id="93d0e-1353">Increased test coverage</span></span>
* <span data-ttu-id="93d0e-1354">Amélioration du mouvement « ? » pour injecter également dans la commande suivante</span><span class="sxs-lookup"><span data-stu-id="93d0e-1354">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="93d0e-1355">Correction d’erreurs interactives avec le profil 2017-03-09-profil-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="93d0e-1355">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="93d0e-1356">Autorisé `--version` en tant que paramètre pour le mode interactif (#3645)</span><span class="sxs-lookup"><span data-stu-id="93d0e-1356">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="93d0e-1357">Empêche le mode interactif de lever des erreurs à partir des listes de saisie semi-automatique de validation (#3570)</span><span class="sxs-lookup"><span data-stu-id="93d0e-1357">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="93d0e-1358">Rapports de progression pour les déploiements de modèles (#3510)</span><span class="sxs-lookup"><span data-stu-id="93d0e-1358">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="93d0e-1359">Ajout de l’indicateur `--progress`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1359">Added `--progress` flag</span></span>
* <span data-ttu-id="93d0e-1360">Suppression `--debug` et `--verbose` des listes de saisie semi-automatique</span><span class="sxs-lookup"><span data-stu-id="93d0e-1360">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="93d0e-1361">Suppression `interactive` des listes de saisie semi-automatique (#3324)</span><span class="sxs-lookup"><span data-stu-id="93d0e-1361">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="93d0e-1362">IoT</span><span class="sxs-lookup"><span data-stu-id="93d0e-1362">IoT</span></span>

* <span data-ttu-id="93d0e-1363">La création de la stratégie n’efface plus les stratégies existantes.</span><span class="sxs-lookup"><span data-stu-id="93d0e-1363">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="93d0e-1364">(#3934)</span><span class="sxs-lookup"><span data-stu-id="93d0e-1364">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="93d0e-1365">Coffre de clés</span><span class="sxs-lookup"><span data-stu-id="93d0e-1365">Key vault</span></span>

* <span data-ttu-id="93d0e-1366">Ajout de commandes pour les fonctionnalités de récupération de coffre de clés :</span><span class="sxs-lookup"><span data-stu-id="93d0e-1366">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="93d0e-1367">`keyvault`sous-commandes `purge`, `recover`,`keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1367">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="93d0e-1368">`keyvault secret`sous-commandes `backup`, `restore`, `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1368">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="93d0e-1369">`keyvault certificate`sous-commandes `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1369">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="93d0e-1370">`keyvault key`sous-commandes `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1370">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="93d0e-1371">Ajout de l’intégration du coffre de clés du principal du service (#3133)</span><span class="sxs-lookup"><span data-stu-id="93d0e-1371">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="93d0e-1372">Mise à jour du plan de données du coffre de clés vers 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="93d0e-1372">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="93d0e-1373">(#3307)</span><span class="sxs-lookup"><span data-stu-id="93d0e-1373">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="93d0e-1374">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="93d0e-1374">Lab</span></span>

* <span data-ttu-id="93d0e-1375">Ajout de la prise en charge de la revendication de toutes les machines virtuelles dans le laboratoire via `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1375">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="93d0e-1376">Ajout du formateur de sortie de tableau pour `az lab vm list` et `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1376">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="93d0e-1377">Surveiller</span><span class="sxs-lookup"><span data-stu-id="93d0e-1377">Monitor</span></span>

* <span data-ttu-id="93d0e-1378">Correctif pour le fichier de modèle avec `monitor autoscale-settings get-parameters-template` commande (#3349)</span><span class="sxs-lookup"><span data-stu-id="93d0e-1378">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="93d0e-1379">Renommage de `monitor alert-rule-incidents list` en `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1379">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="93d0e-1380">Renommage de `monitor alert-rule-incidents show` en `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1380">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="93d0e-1381">Renommage de `monitor metric-defintions list` en `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1381">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="93d0e-1382">Renommage de `monitor alert-rules` en `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1382">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="93d0e-1383">Modifié `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="93d0e-1383">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="93d0e-1384">sous-commandes`condition` et `action` n’acceptent plus JSON</span><span class="sxs-lookup"><span data-stu-id="93d0e-1384">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="93d0e-1385">Ajout de nombreux paramètres simplifiant le processus de création de règle</span><span class="sxs-lookup"><span data-stu-id="93d0e-1385">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="93d0e-1386">`location` n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="93d0e-1386">`location` no longer required</span></span>
  * <span data-ttu-id="93d0e-1387">Ajout d’un nom et de la prise en charge de l’ID de la cible</span><span class="sxs-lookup"><span data-stu-id="93d0e-1387">Add name and ID support for target</span></span>
  * <span data-ttu-id="93d0e-1388">Suppression de `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1388">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="93d0e-1389">Le renommage de `is-enabled` en `enabled`n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="93d0e-1389">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="93d0e-1390">`description` par défaut sont désormais basées sur la condition fournie</span><span class="sxs-lookup"><span data-stu-id="93d0e-1390">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="93d0e-1391">Ajout d’exemples aidant à clarifier le nouveau format</span><span class="sxs-lookup"><span data-stu-id="93d0e-1391">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="93d0e-1392">Prise en charge des noms ou des ID pour les commandes `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1392">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="93d0e-1393">Ajout d’arguments d’usage et d’exemples pour `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1393">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="93d0e-1394">Réseau</span><span class="sxs-lookup"><span data-stu-id="93d0e-1394">Network</span></span>

* <span data-ttu-id="93d0e-1395">Ajout de la commande `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1395">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="93d0e-1396">Ajout de l’argument `--private-access-services` à `vnet subnet create` et `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1396">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="93d0e-1397">Correction d’un problème `application-gateway redirect-config create` qui causait l’échec de</span><span class="sxs-lookup"><span data-stu-id="93d0e-1397">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="93d0e-1398">Correction d’un problème `application-gateway redirect-config update` qui `--no-wait` empêchait le fonctionnement de</span><span class="sxs-lookup"><span data-stu-id="93d0e-1398">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="93d0e-1399">Correction d’un bogue lié à l’utilisation d’un `--servers` argument avec `application-gateway address-pool create` et `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1399">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="93d0e-1400">Ajout des commandes `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1400">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="93d0e-1401">Ajout de commandes à `application-gateway ssl-policy` : `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1401">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="93d0e-1402">Ajout d’arguments à `application-gateway ssl-policy set` : `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1402">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="93d0e-1403">Ajout d’arguments à `application-gateway http-settings create` et `application-gateway http-settings update` : `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1403">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="93d0e-1404">Ajout d’arguments à `application-gateway url-path-map create` et `application-gateway url-path-map update`, `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1404">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="93d0e-1405">Ajout d’un argument `--redirect-config` à `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1405">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="93d0e-1406">Ajout de la prise en charge de `--no-wait` pour `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1406">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="93d0e-1407">Ajout d’arguments à `application-gateway probe create` et `application-gateway probe update` : `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1407">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="93d0e-1408">Ajout d’un argument `--redirect-config` à `application-gateway rule create` et `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1408">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="93d0e-1409">Ajout de la prise en charge de `--accelerated-networking` pour `nic create` et `nic update`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1409">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="93d0e-1410">Suppression de l’ `--internal-dns-name-suffix` argument à partir de `nic create`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1410">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="93d0e-1411">Ajout de la prise en charge de `--dns-servers` pour `nic update` et `nic create` : ajout de la prise en charge pour les serveurs DNS :</span><span class="sxs-lookup"><span data-stu-id="93d0e-1411">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="93d0e-1412">Correction d’un bogue qui faisait `local-gateway create` ignorer `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1412">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="93d0e-1413">Ajout de la prise en charge de `--dns-servers` pour `vnet update`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1413">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="93d0e-1414">Correction d’un bogue lors de la création d’une homologation sans filtrage de l’itinéraire avec `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1414">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="93d0e-1415">Correction d’un bogue qui empêchait le fonctionnement des arguments `--provider` et `--bandwidth` avec `express-route update`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1415">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="93d0e-1416">Correction d’un bogue avec `network watcher show-topology` une logique de valeurs par défaut</span><span class="sxs-lookup"><span data-stu-id="93d0e-1416">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="93d0e-1417">Amélioration de la mise en forme de sortie pour `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1417">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="93d0e-1418">Utilisation de l’IP frontale par défaut pour `application-gateway http-listener create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="93d0e-1418">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="93d0e-1419">Utilisation d’un pool d’adresses par défaut, des paramètres HTTP et de l’écouteur HTTP pour `application-gateway rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="93d0e-1419">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="93d0e-1420">Utilisation de l’IP frontale par défaut et du pool principal `lb rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="93d0e-1420">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="93d0e-1421">Utilisation de l’IP frontale par défaut pour `lb inbound-nat-rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="93d0e-1421">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="93d0e-1422">Profil</span><span class="sxs-lookup"><span data-stu-id="93d0e-1422">Profile</span></span>

* <span data-ttu-id="93d0e-1423">Prise en charge de la connexion à l’intérieur d’une machine virtuelle avec une identité gérée</span><span class="sxs-lookup"><span data-stu-id="93d0e-1423">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="93d0e-1424">Prise en charge de la sortie pour `account show` au format de fichier d’authentification du Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="93d0e-1424">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="93d0e-1425">Affichage des avertissements de désapprobation lors de l’utilisation de '--expanded-view'</span><span class="sxs-lookup"><span data-stu-id="93d0e-1425">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="93d0e-1426">Ajout de la commande `get-access-token` permettant de fournir un jeton AAD brut</span><span class="sxs-lookup"><span data-stu-id="93d0e-1426">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="93d0e-1427">Prise en charge de la connexion avec un compte d’utilisateur sans abonnements associés</span><span class="sxs-lookup"><span data-stu-id="93d0e-1427">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="93d0e-1428">SGBDR</span><span class="sxs-lookup"><span data-stu-id="93d0e-1428">RDBMS</span></span>

* <span data-ttu-id="93d0e-1429">Prise en charge de l’énumération de serveurs à travers un abonnement (#3417)</span><span class="sxs-lookup"><span data-stu-id="93d0e-1429">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="93d0e-1430">Correction de `%s` non traité car il manque `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="93d0e-1430">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="93d0e-1431">Correction du mappage de la source du document et ajout de la tâche CI permettant la vérification de (#3361)</span><span class="sxs-lookup"><span data-stu-id="93d0e-1431">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="93d0e-1432">Correction concernant l’aide relative à MySQL et PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="93d0e-1432">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="93d0e-1433">Ressource</span><span class="sxs-lookup"><span data-stu-id="93d0e-1433">Resource</span></span>

* <span data-ttu-id="93d0e-1434">Amélioration des invites pour les paramètres manquants de `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1434">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="93d0e-1435">Amélioration de l’analyse de `--parameters KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="93d0e-1435">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="93d0e-1436">Correction des problèmes à cause desquels `group deployment create` les fichiers de paramètres n’étaient plus reconnus à l’aide de la `@<file>` syntaxe</span><span class="sxs-lookup"><span data-stu-id="93d0e-1436">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="93d0e-1437">Prise en charge de l’ `--ids` argument pour `resource` et `managedapp` les commandes</span><span class="sxs-lookup"><span data-stu-id="93d0e-1437">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="93d0e-1438">Correction de certains messages d’analyse et d’erreur (#3584)</span><span class="sxs-lookup"><span data-stu-id="93d0e-1438">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="93d0e-1439">Correction de l’analyse `--resource-type` permettant à la `lock` commande d’accepter `<resource-namespace>` et `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1439">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="93d0e-1440">Ajout de la vérification de paramètre des modèles de liaison de modèle (#3629)</span><span class="sxs-lookup"><span data-stu-id="93d0e-1440">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="93d0e-1441">Ajout de la prise en charge de la spécification des paramètres de déploiement à l’aide de la `KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="93d0e-1441">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="93d0e-1442">Rôle</span><span class="sxs-lookup"><span data-stu-id="93d0e-1442">Role</span></span>

* <span data-ttu-id="93d0e-1443">Prise en charge de la sortie au format de fichier d’authentification du Kit de développement logiciel (SDK) pour `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1443">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="93d0e-1444">Nettoyage des attributions de rôles et de l’application AAD liée lors de la suppression d’un principal de service (#3610)</span><span class="sxs-lookup"><span data-stu-id="93d0e-1444">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="93d0e-1445">Inclusion du format d’heure dans `app create` args `--start-date` et `--end-date` descriptions</span><span class="sxs-lookup"><span data-stu-id="93d0e-1445">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="93d0e-1446">Affichage des avertissements de désapprobation lors de l’utilisation de `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1446">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="93d0e-1447">Ajout de l’intégration du coffre de clés pour les commandes `create-for-rbac` et `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1447">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="93d0e-1448">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="93d0e-1448">Service Fabric</span></span>
* <span data-ttu-id="93d0e-1449">Correction d’un problème avec les fichiers volumineux dans les applications tronquées sur le chargement (#3666)</span><span class="sxs-lookup"><span data-stu-id="93d0e-1449">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="93d0e-1450">Ajout de tests pour les commandes Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="93d0e-1450">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="93d0e-1451">Correction de nombreuses commandes Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="93d0e-1451">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="93d0e-1452">SQL</span><span class="sxs-lookup"><span data-stu-id="93d0e-1452">SQL</span></span>

* <span data-ttu-id="93d0e-1453">Suppression du paramètre rompu `sql server create` `--identity`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1453">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="93d0e-1454">Suppression des valeurs de mot de passe à partir de la sortie de commande `sql server create` et `sql server update`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1454">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="93d0e-1455">Ajout des commandes `sql db list-editions` et `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1455">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="93d0e-1456">Stockage</span><span class="sxs-lookup"><span data-stu-id="93d0e-1456">Storage</span></span>

* <span data-ttu-id="93d0e-1457">Suppression d’une `--marker` option à partir des commandes `storage blob list`, `storage container list`et `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="93d0e-1457">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="93d0e-1458">Activation de la création d’un compte de stockage https-only</span><span class="sxs-lookup"><span data-stu-id="93d0e-1458">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="93d0e-1459">Mise à jour des métriques de stockage, de la journalisation et des commandes cors (#3495)</span><span class="sxs-lookup"><span data-stu-id="93d0e-1459">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="93d0e-1460">Reformulation d’un message d’exception de l’ajout CORS (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="93d0e-1460">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="93d0e-1461">Conversion du générateur à une liste en mode exécution d’essai de la commande de téléchargement de lot (#3592)</span><span class="sxs-lookup"><span data-stu-id="93d0e-1461">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="93d0e-1462">Correction du problème d’essai associé au lot de téléchargement du blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="93d0e-1462">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="93d0e-1463">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="93d0e-1463">VM</span></span>

* <span data-ttu-id="93d0e-1464">Prise en charge de la configuration du groupe de sécurité réseau</span><span class="sxs-lookup"><span data-stu-id="93d0e-1464">Support configuring nsg</span></span>
* <span data-ttu-id="93d0e-1465">Correction d’un bogue qui entraînait une configuration incorrecte du serveur DNS</span><span class="sxs-lookup"><span data-stu-id="93d0e-1465">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="93d0e-1466">Prise en charge des identités de service géré</span><span class="sxs-lookup"><span data-stu-id="93d0e-1466">Support managed service identities</span></span>
* <span data-ttu-id="93d0e-1467">Correction d’un problème à cause duquel `cmss create` avec un équilibreur de charge existant exigeait `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1467">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="93d0e-1468">Les disques de données créés avec le numéro d’unité logique `vm image create` commencent à 0</span><span class="sxs-lookup"><span data-stu-id="93d0e-1468">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="93d0e-1469">10 mai 2017</span><span class="sxs-lookup"><span data-stu-id="93d0e-1469">May 10, 2017</span></span>

<span data-ttu-id="93d0e-1470">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="93d0e-1470">Version 2.0.6</span></span>

* <span data-ttu-id="93d0e-1471">documentdb renommé en cosmosdb</span><span class="sxs-lookup"><span data-stu-id="93d0e-1471">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="93d0e-1472">Ajouter rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="93d0e-1472">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="93d0e-1473">Inclure les modules Data Lake Analytics et Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="93d0e-1473">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="93d0e-1474">Inclure le module Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="93d0e-1474">Include Cognitive Services module</span></span>
* <span data-ttu-id="93d0e-1475">Inclure le module Service Fabric</span><span class="sxs-lookup"><span data-stu-id="93d0e-1475">Include Service Fabric module</span></span>
* <span data-ttu-id="93d0e-1476">Inclure le module Interactive (az-shell renommé)</span><span class="sxs-lookup"><span data-stu-id="93d0e-1476">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="93d0e-1477">Ajouter la prise en charge des commandes CDN</span><span class="sxs-lookup"><span data-stu-id="93d0e-1477">Add support for CDN commands</span></span>
* <span data-ttu-id="93d0e-1478">Supprimer le module Container</span><span class="sxs-lookup"><span data-stu-id="93d0e-1478">Remove Container module</span></span>
* <span data-ttu-id="93d0e-1479">Ajouter « az -v » comme raccourci pour « az --version » ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="93d0e-1479">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="93d0e-1480">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="93d0e-1480">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="93d0e-1481">Principal</span><span class="sxs-lookup"><span data-stu-id="93d0e-1481">Core</span></span>

* <span data-ttu-id="93d0e-1482">principal : capturer les exceptions provoquées par un fournisseur non enregistré et l’enregistrer automatiquement</span><span class="sxs-lookup"><span data-stu-id="93d0e-1482">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="93d0e-1483">performance : conserver le cache de jeton adal en mémoire jusqu’à la fin du processus ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="93d0e-1483">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="93d0e-1484">Corriger les octets retournés par l’empreinte digitale hex -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="93d0e-1484">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="93d0e-1485">Téléchargement du certificat Key Vault et intégration AAD SP améliorés ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="93d0e-1485">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="93d0e-1486">Ajouter l’emplacement de Python à « az —version » ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="93d0e-1486">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="93d0e-1487">connexion : prise en charge de la connexion lorsqu’il n’y a aucun abonnement ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="93d0e-1487">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="93d0e-1488">principal : corriger une erreur lors de la connexion à l’aide d’un principal de service deux fois ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="93d0e-1488">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="93d0e-1489">principal : autoriser la configuration du chemin d’accès de accessTokens.json via une variable d’environnement ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="93d0e-1489">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="93d0e-1490">principal : autoriser l’application des valeurs par défaut configurées sur les arguments facultatifs ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="93d0e-1490">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="93d0e-1491">principal : performances améliorées</span><span class="sxs-lookup"><span data-stu-id="93d0e-1491">core: Improved performance</span></span>
* <span data-ttu-id="93d0e-1492">principal : certificats d’autorité de certification personnalisés - prise en charge de la définition de la variable d’environnement REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="93d0e-1492">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="93d0e-1493">principal : configuration du cloud - utiliser le point de terminaison « resource manager » si le point de terminaison « management » n’est pas défini</span><span class="sxs-lookup"><span data-stu-id="93d0e-1493">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="93d0e-1494">ACS</span><span class="sxs-lookup"><span data-stu-id="93d0e-1494">ACS</span></span>

* <span data-ttu-id="93d0e-1495">corriger le nombre de maîtres et d’agents sur un nombre entier au lieu d’une chaîne</span><span class="sxs-lookup"><span data-stu-id="93d0e-1495">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="93d0e-1496">exposer « az acs create --no-wait » et « az acs wait » pour la création asynchrone</span><span class="sxs-lookup"><span data-stu-id="93d0e-1496">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="93d0e-1497">exposer « az acs create --validate » pour les validations de test</span><span class="sxs-lookup"><span data-stu-id="93d0e-1497">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="93d0e-1498">supprimer le profil Windows avant l’appel PUT pour la commande de mise à l’échelle ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="93d0e-1498">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="93d0e-1499">AppService</span><span class="sxs-lookup"><span data-stu-id="93d0e-1499">AppService</span></span>

* <span data-ttu-id="93d0e-1500">functionapp : ajouter la prise en charge complète de functionapp, notamment créer, afficher, liste, supprimer, nom d’hôte, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="93d0e-1500">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="93d0e-1501">Ajout de Team Services (vsts) comme option de livraison continue à « config contrôle source web appservice »</span><span class="sxs-lookup"><span data-stu-id="93d0e-1501">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="93d0e-1502">Créer « az webapp » pour remplacer « az appservice web » (pour la rétrocompatibilité, « az appservice web » sera conservé dans les 2 prochaines versions)</span><span class="sxs-lookup"><span data-stu-id="93d0e-1502">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="93d0e-1503">Exposer des arguments pour configurer le déploiement et des « piles d’exécution » sur webapp create</span><span class="sxs-lookup"><span data-stu-id="93d0e-1503">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="93d0e-1504">Exposer « webapp list-runtimes »</span><span class="sxs-lookup"><span data-stu-id="93d0e-1504">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="93d0e-1505">prendre en charge la configuration des chaînes de connexion ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="93d0e-1505">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="93d0e-1506">prendre en charge le basculement d’emplacement avec aperçu</span><span class="sxs-lookup"><span data-stu-id="93d0e-1506">support slot swap with preview</span></span>
* <span data-ttu-id="93d0e-1507">Supprimer les erreurs des commandes appservice ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="93d0e-1507">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="93d0e-1508">Utiliser le groupe de ressources du plan app service pour les opérations de certificat ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="93d0e-1508">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="93d0e-1509">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="93d0e-1509">CosmosDB</span></span>

* <span data-ttu-id="93d0e-1510">Renommer le module documentdb en cosmosdb</span><span class="sxs-lookup"><span data-stu-id="93d0e-1510">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="93d0e-1511">Prise en charge ajoutée pour les API de plan de données documentdb : gestion de base de données et de collecte</span><span class="sxs-lookup"><span data-stu-id="93d0e-1511">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="93d0e-1512">Prise en charge ajoutée pour activer le basculement automatique sur les comptes de base de données</span><span class="sxs-lookup"><span data-stu-id="93d0e-1512">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="93d0e-1513">Prise en charge ajoutée pour la nouvelle stratégie de cohérence ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="93d0e-1513">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="93d0e-1514">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="93d0e-1514">Data Lake Analytics</span></span>

* <span data-ttu-id="93d0e-1515">Corriger un bogue dans lequel le filtrage sur le résultat et l’état des listes de travaux lève une erreur</span><span class="sxs-lookup"><span data-stu-id="93d0e-1515">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="93d0e-1516">Ajouter la prise en charge d’un nouveau type d’élément de catalogue : paquet.</span><span class="sxs-lookup"><span data-stu-id="93d0e-1516">Add support for new catalog item type: package.</span></span> <span data-ttu-id="93d0e-1517">accessible via : `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1517">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="93d0e-1518">A rendu possible le fait de répertorier les éléments de catalogue suivants à partir d’une base de données (aucune spécification de schéma requise) :</span><span class="sxs-lookup"><span data-stu-id="93d0e-1518">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="93d0e-1519">Table</span><span class="sxs-lookup"><span data-stu-id="93d0e-1519">Table</span></span>
  * <span data-ttu-id="93d0e-1520">Fonction table</span><span class="sxs-lookup"><span data-stu-id="93d0e-1520">Table valued function</span></span>
  * <span data-ttu-id="93d0e-1521">Affichage</span><span class="sxs-lookup"><span data-stu-id="93d0e-1521">View</span></span>
  * <span data-ttu-id="93d0e-1522">Statistiques de table.</span><span class="sxs-lookup"><span data-stu-id="93d0e-1522">Table Statistics.</span></span> <span data-ttu-id="93d0e-1523">Cela peut également être répertorié avec un schéma, mais sans spécifier un nom de table</span><span class="sxs-lookup"><span data-stu-id="93d0e-1523">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="93d0e-1524">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="93d0e-1524">Data Lake Store</span></span>

* <span data-ttu-id="93d0e-1525">Mettre à jour la version du Kit de développement logiciel (SDK) du système de fichiers sous-jacent, qui offre une meilleure prise en charge pour gérer les scénarios de limitation côté serveur</span><span class="sxs-lookup"><span data-stu-id="93d0e-1525">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="93d0e-1526">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="93d0e-1526">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="93d0e-1527">aide manquante pour afficher l’accès.</span><span class="sxs-lookup"><span data-stu-id="93d0e-1527">missed help for access show.</span></span> <span data-ttu-id="93d0e-1528">ajout en cours.</span><span class="sxs-lookup"><span data-stu-id="93d0e-1528">adding it.</span></span> <span data-ttu-id="93d0e-1529">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="93d0e-1529">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="93d0e-1530">Rechercher</span><span class="sxs-lookup"><span data-stu-id="93d0e-1530">Find</span></span>

* <span data-ttu-id="93d0e-1531">résultats de la recherche améliorés et autorisation du contrôle de version de l’index de recherche</span><span class="sxs-lookup"><span data-stu-id="93d0e-1531">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="93d0e-1532">KeyVault</span><span class="sxs-lookup"><span data-stu-id="93d0e-1532">KeyVault</span></span>

* <span data-ttu-id="93d0e-1533">BC : `az keyvault certificate download` remplacer -e dans chaîne ou élément binaire par PEM ou DER afin de mieux représenter les options</span><span class="sxs-lookup"><span data-stu-id="93d0e-1533">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="93d0e-1534">BC : Supprimer --expires et --not-before dans `keyvault certificate create` car ces paramètres ne sont pas pris en charge par le service</span><span class="sxs-lookup"><span data-stu-id="93d0e-1534">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="93d0e-1535">Ajoute le paramètre --validity à `keyvault certificate create` pour substituer de manière sélective la valeur dans --policy</span><span class="sxs-lookup"><span data-stu-id="93d0e-1535">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="93d0e-1536">Résout le problème dans `keyvault certificate get-default-policy` où « expires » et « not_before » étaient exposés mais « validity_in_months » ne l’était pas</span><span class="sxs-lookup"><span data-stu-id="93d0e-1536">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="93d0e-1537">correction de keyvault pour l’importation de pem et pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="93d0e-1537">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="93d0e-1538">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="93d0e-1538">Lab</span></span>

* <span data-ttu-id="93d0e-1539">Ajout des commandes créer, afficher, supprimer et liste pour l’environnement dans le laboratoire</span><span class="sxs-lookup"><span data-stu-id="93d0e-1539">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="93d0e-1540">Ajout des commandes afficher et liste pour afficher les modèles ARM dans le laboratoire</span><span class="sxs-lookup"><span data-stu-id="93d0e-1540">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="93d0e-1541">Ajout de l’indicateur --environment dans `az lab vm list` pour filtrer les machines virtuelles selon l’environnement du laboratoire</span><span class="sxs-lookup"><span data-stu-id="93d0e-1541">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="93d0e-1542">Ajout de la commande pratique `az lab formula export-artifacts` pour exporter une structure d’artefact dans une formule de laboratoire</span><span class="sxs-lookup"><span data-stu-id="93d0e-1542">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="93d0e-1543">Ajout de commandes pour gérer les secrets dans un laboratoire</span><span class="sxs-lookup"><span data-stu-id="93d0e-1543">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="93d0e-1544">Surveiller</span><span class="sxs-lookup"><span data-stu-id="93d0e-1544">Monitor</span></span>

* <span data-ttu-id="93d0e-1545">Correction de bogue : modélisation `--actions` de `az alert-rules create` pour consommer la chaîne JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="93d0e-1545">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="93d0e-1546">Correction de bogue : la création de paramètres de diagnostic n’accepte pas les métriques/journaux à partir des commandes d’affichage ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="93d0e-1546">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="93d0e-1547">Réseau</span><span class="sxs-lookup"><span data-stu-id="93d0e-1547">Network</span></span>

* <span data-ttu-id="93d0e-1548">Ajouter la commande `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1548">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="93d0e-1549">Ajouter la prise en charge du paramètre `--filters` pour `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1549">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="93d0e-1550">Ajouter la prise en charge pour le drainage de connexion Application Gateway</span><span class="sxs-lookup"><span data-stu-id="93d0e-1550">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="93d0e-1551">Ajouter la prise en charge pour la configuration du jeu de règles WAF d’Application Gateway</span><span class="sxs-lookup"><span data-stu-id="93d0e-1551">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="93d0e-1552">Ajouter la prise en charge des règles et des filtres de routage ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="93d0e-1552">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="93d0e-1553">Ajouter la prise en charge pour le routage géographique TrafficManager</span><span class="sxs-lookup"><span data-stu-id="93d0e-1553">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="93d0e-1554">Ajouter la prise en charge des sélecteurs de trafic basés sur la stratégie de connexion VPN</span><span class="sxs-lookup"><span data-stu-id="93d0e-1554">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="93d0e-1555">Ajouter la prise en charge pour les stratégies IPSec de la connexion VPN</span><span class="sxs-lookup"><span data-stu-id="93d0e-1555">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="93d0e-1556">Corriger le bogue avec `vpn-connection create` lors de l’utilisation des paramètres `--no-wait` ou `--validate`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1556">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="93d0e-1557">Ajouter la prise en charge des passerelles de réseau virtuel actif-actif</span><span class="sxs-lookup"><span data-stu-id="93d0e-1557">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="93d0e-1558">Supprimer les valeurs NULL de la sortie des commandes `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1558">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="93d0e-1559">BC : résoudre un bogue dans la sortie de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1559">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="93d0e-1560">Corriger le bogue où l’argument « --key-length » de « vpn-connection create » n’était pas analysé correctement</span><span class="sxs-lookup"><span data-stu-id="93d0e-1560">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="93d0e-1561">Corriger le bogue dans `dns zone import` où les enregistrements n’étaient pas été importés correctement</span><span class="sxs-lookup"><span data-stu-id="93d0e-1561">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="93d0e-1562">Corriger le bogue où `traffic-manager endpoint update` ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="93d0e-1562">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="93d0e-1563">Ajouter des commandes d’aperçu « network watcher »</span><span class="sxs-lookup"><span data-stu-id="93d0e-1563">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="93d0e-1564">Profil</span><span class="sxs-lookup"><span data-stu-id="93d0e-1564">Profile</span></span>

* <span data-ttu-id="93d0e-1565">Prendre en charge la connexion lorsqu’il n’y a aucun abonnement trouvé ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="93d0e-1565">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="93d0e-1566">Prendre en charge un nom de paramètre court dans le jeu de comptes az --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="93d0e-1566">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="93d0e-1567">Redis</span><span class="sxs-lookup"><span data-stu-id="93d0e-1567">Redis</span></span>

* <span data-ttu-id="93d0e-1568">Ajout d’une commande de mise à jour qui ajoute également la possibilité de mettre à l’échelle pour le cache redis</span><span class="sxs-lookup"><span data-stu-id="93d0e-1568">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="93d0e-1569">Commande « update-settings » déconseillée</span><span class="sxs-lookup"><span data-stu-id="93d0e-1569">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="93d0e-1570">Ressource</span><span class="sxs-lookup"><span data-stu-id="93d0e-1570">Resource</span></span>

* <span data-ttu-id="93d0e-1571">Ajouter managedapp et les commandes de définition managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="93d0e-1571">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="93d0e-1572">Prendre en charge les commandes « provider operation » ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="93d0e-1572">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="93d0e-1573">Prendre en charge la création de ressource générique ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="93d0e-1573">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="93d0e-1574">Corriger l’analyse de ressource et la recherche de version d’API.</span><span class="sxs-lookup"><span data-stu-id="93d0e-1574">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="93d0e-1575">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="93d0e-1575">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="93d0e-1576">Ajouter des documents pour mise à jour du verrou az.</span><span class="sxs-lookup"><span data-stu-id="93d0e-1576">Add docs for az lock update.</span></span> <span data-ttu-id="93d0e-1577">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="93d0e-1577">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="93d0e-1578">Sortie d’erreur si vous essayez de lister des ressources pour un groupe qui n’existe pas.</span><span class="sxs-lookup"><span data-stu-id="93d0e-1578">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="93d0e-1579">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="93d0e-1579">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="93d0e-1580">[Compute] Résoudre les problèmes de mise à jour de VMSS et du groupe à haute disponibilité de machines virtuelles.</span><span class="sxs-lookup"><span data-stu-id="93d0e-1580">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="93d0e-1581">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="93d0e-1581">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="93d0e-1582">Corriger le verrouillage des commandes créer et supprimer si parent-resource-path est None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="93d0e-1582">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="93d0e-1583">Rôle</span><span class="sxs-lookup"><span data-stu-id="93d0e-1583">Role</span></span>

* <span data-ttu-id="93d0e-1584">create-for-rbac : vérifier que la date de fin du SP ne dépassera pas la date d’expiration du certificat ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="93d0e-1584">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="93d0e-1585">RBAC : ajouter la prise en charge complète de « ad group » ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="93d0e-1585">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="93d0e-1586">rôle : résoudre les problèmes de mise à jour de définition de rôle ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="93d0e-1586">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="93d0e-1587">create-for-rbac : vérifier que le mot de passe fourni par l’utilisateur est accepté</span><span class="sxs-lookup"><span data-stu-id="93d0e-1587">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="93d0e-1588">SQL</span><span class="sxs-lookup"><span data-stu-id="93d0e-1588">SQL</span></span>

* <span data-ttu-id="93d0e-1589">Ajout des commandes az sql server list-usages et az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="93d0e-1589">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="93d0e-1590">SQL : possibilité de se connecter directement au fournisseur de ressources ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="93d0e-1590">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="93d0e-1591">Stockage</span><span class="sxs-lookup"><span data-stu-id="93d0e-1591">Storage</span></span>

* <span data-ttu-id="93d0e-1592">Définir l’emplacement par défaut sur l’emplacement du groupe de ressources pour `storage account create`</span><span class="sxs-lookup"><span data-stu-id="93d0e-1592">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="93d0e-1593">Ajouter la prise en charge de la copie incrémentielle d’objet blob</span><span class="sxs-lookup"><span data-stu-id="93d0e-1593">Add support for incremental blob copy</span></span>
* <span data-ttu-id="93d0e-1594">Ajouter la prise en charge du chargement d’objet blob de blocs volumineux</span><span class="sxs-lookup"><span data-stu-id="93d0e-1594">Add support for large block blob upload</span></span>
* <span data-ttu-id="93d0e-1595">Modifier la taille de bloc à 100 Mo lorsque le fichier à charger est supérieur à 200 Go</span><span class="sxs-lookup"><span data-stu-id="93d0e-1595">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="93d0e-1596">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="93d0e-1596">VM</span></span>

* <span data-ttu-id="93d0e-1597">avail-set : rendre le compte de domaine UD&FD facultatif</span><span class="sxs-lookup"><span data-stu-id="93d0e-1597">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="93d0e-1598">remarque : commandes de machine virtuelle dans clouds souverains Veuillez éviter les fonctionnalités liées au disque managé, notamment :</span><span class="sxs-lookup"><span data-stu-id="93d0e-1598">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="93d0e-1599">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="93d0e-1599">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="93d0e-1600">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="93d0e-1600">az vm/vmss disk</span></span>
  3. <span data-ttu-id="93d0e-1601">Dans « az vm/vmss create », utiliser « —use-unmanaged-disk » pour éviter le disque managé Les autres commandes devraient fonctionner</span><span class="sxs-lookup"><span data-stu-id="93d0e-1601">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="93d0e-1602">vm/vmss : améliorer le texte d’avertissement lors de la génération de paires de clés ssh</span><span class="sxs-lookup"><span data-stu-id="93d0e-1602">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="93d0e-1603">vm/vmss : prendre en charge la création à partir d’une image de la Place de marché qui requiert des informations sur le plan ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="93d0e-1603">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="93d0e-1604">3 avril 2017</span><span class="sxs-lookup"><span data-stu-id="93d0e-1604">April 3, 2017</span></span>

<span data-ttu-id="93d0e-1605">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="93d0e-1605">Version 2.0.2</span></span>

<span data-ttu-id="93d0e-1606">Nous avons publié les composants ACR, Batch, KeyVault et SQL dans cette version</span><span class="sxs-lookup"><span data-stu-id="93d0e-1606">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="93d0e-1607">Principal</span><span class="sxs-lookup"><span data-stu-id="93d0e-1607">Core</span></span>

* <span data-ttu-id="93d0e-1608">Ajout des modules acr, lab, monitor et find à la liste par défaut</span><span class="sxs-lookup"><span data-stu-id="93d0e-1608">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="93d0e-1609">Connexion : ignorer les locataires erronés ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="93d0e-1609">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="93d0e-1610">login : définition de l’abonnement par défaut à la valeur « un » avec l’état « Activé » ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="93d0e-1610">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="93d0e-1611">Ajout de la prise en charge des commandes wait et de --no-wait à davantage de commandes ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="93d0e-1611">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="93d0e-1612">core : prise en charge de la connexion à l’aide du principal du service avec un certificat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="93d0e-1612">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="93d0e-1613">Ajout d’une invite pour les paramètres de modèle manquants.</span><span class="sxs-lookup"><span data-stu-id="93d0e-1613">Add prompting for missing template parameters.</span></span> <span data-ttu-id="93d0e-1614">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="93d0e-1614">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="93d0e-1615">Prise en charge de la définition de valeurs par défaut pour des arguments courants tels que le groupe de ressources par défaut, le site web par défaut et la machine virtuelle par défaut</span><span class="sxs-lookup"><span data-stu-id="93d0e-1615">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="93d0e-1616">Prise en charge de la connexion à un locataire spécifique</span><span class="sxs-lookup"><span data-stu-id="93d0e-1616">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="93d0e-1617">ACS</span><span class="sxs-lookup"><span data-stu-id="93d0e-1617">ACS</span></span>

* <span data-ttu-id="93d0e-1618">[ACS] Ajout de la prise en charge de la configuration d’un cluster ACS par défaut ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="93d0e-1618">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="93d0e-1619">Ajout de la prise en charge de l’invite de mot de passe de clé ssh.</span><span class="sxs-lookup"><span data-stu-id="93d0e-1619">Add support for ssh key password prompting.</span></span> <span data-ttu-id="93d0e-1620">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="93d0e-1620">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="93d0e-1621">Ajout de la prise en charge des clusters Windows.</span><span class="sxs-lookup"><span data-stu-id="93d0e-1621">Add support for windows clusters.</span></span> <span data-ttu-id="93d0e-1622">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="93d0e-1622">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="93d0e-1623">Basculement du rôle Propriétaire au rôle Contributeur.</span><span class="sxs-lookup"><span data-stu-id="93d0e-1623">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="93d0e-1624">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="93d0e-1624">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="93d0e-1625">AppService</span><span class="sxs-lookup"><span data-stu-id="93d0e-1625">AppService</span></span>

* <span data-ttu-id="93d0e-1626">appservice : prise en charge de l’obtention de l’adresse IP externe utilisée pour les enregistrements A DNS ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="93d0e-1626">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="93d0e-1627">appservice : prise en charge de la liaison des certificats avec caractères génériques ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="93d0e-1627">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="93d0e-1628">appservice : prise en charge des profils de publication de liste ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="93d0e-1628">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="93d0e-1629">AppService : déclenchement de la synchronisation de contrôle de code source après la configuration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="93d0e-1629">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="93d0e-1630">DataLake</span><span class="sxs-lookup"><span data-stu-id="93d0e-1630">DataLake</span></span>

* <span data-ttu-id="93d0e-1631">Version initiale du module Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="93d0e-1631">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="93d0e-1632">Version initiale du module Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="93d0e-1632">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="93d0e-1633">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="93d0e-1633">DocuemntDB</span></span>

* <span data-ttu-id="93d0e-1634">DocumentDB : ajout de la prise en charge de l’énumération des chaînes de connexion ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="93d0e-1634">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="93d0e-1635">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="93d0e-1635">VM</span></span>

* <span data-ttu-id="93d0e-1636">[Compute] Ajout de la prise en charge d’AppGateway à la création de groupe de machines virtuelles identiques ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="93d0e-1636">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="93d0e-1637">[VM/VMSS] Amélioration de la prise en charge de la mise en cache de disque ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="93d0e-1637">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="93d0e-1638">VM/VMSS : intégration de la logique de validation des informations d’identification utilisée par le portail ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="93d0e-1638">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="93d0e-1639">Ajout de la prise en charge des commandes wait et de --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="93d0e-1639">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="93d0e-1640">Groupe de machines virtuelles identiques : prise en charge de \* pour énumérer les vues d’instance parmi les machines virtuelles ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="93d0e-1640">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="93d0e-1641">Ajout --secrets pour machine virtuelle et groupe de machines virtuelles identiques ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="93d0e-1641">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="93d0e-1642">Autorisation de la création de machines virtuelles avec un disque dur virtuel spécialisé ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="93d0e-1642">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="93d0e-1643">27 février 2017</span><span class="sxs-lookup"><span data-stu-id="93d0e-1643">February 27, 2017</span></span>

<span data-ttu-id="93d0e-1644">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="93d0e-1644">Version 2.0.0</span></span>

<span data-ttu-id="93d0e-1645">Cette version d’Azure CLI 2.0 est la première instance mise à la disposition générale. La disponibilité générale s’applique à ces modules de commande :</span><span class="sxs-lookup"><span data-stu-id="93d0e-1645">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="93d0e-1646">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="93d0e-1646">Container Service (acs)</span></span>
- <span data-ttu-id="93d0e-1647">Compute (notamment Resource Manager, machine virtuelle, groupes de machines virtuelles identiques, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="93d0e-1647">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="93d0e-1648">Réseau</span><span class="sxs-lookup"><span data-stu-id="93d0e-1648">Networking</span></span>
- <span data-ttu-id="93d0e-1649">Stockage</span><span class="sxs-lookup"><span data-stu-id="93d0e-1649">Storage</span></span>

<span data-ttu-id="93d0e-1650">Ces modules de commande, pouvant être utilisés en production, sont pris en charge par le contrat de niveau de service (SLA) Microsoft standard. Vous pouvez ouvrir des incidents directement auprès du support technique Microsoft ou dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/). Vous pouvez poser des questions sur [StackOverflow à l’aide du mot-clé azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), ou contacter l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Vous pouvez fournir des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="93d0e-1650">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="93d0e-1651">Les commandes de ces modules sont stables et il n’est pas prévu que la syntaxe change dans les mises à jour ultérieures de cette version d’Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="93d0e-1651">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="93d0e-1652">Pour vérifier la version de l’interface CLI, utilisez `az --version`. La sortie indique la version de l’interface CLI proprement dite (2.0.0 dans cette version), les différents modules de commande et les versions de Python et de GCC que vous utilisez.</span><span class="sxs-lookup"><span data-stu-id="93d0e-1652">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="93d0e-1653">Certains de ces modules de commande présentent un suffixe « b*n* » ou « rc*n* ». Ces modules de commande, encore en préversion, seront mis à la disposition générale à l’avenir.</span><span class="sxs-lookup"><span data-stu-id="93d0e-1653">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="93d0e-1654">Nous avons également des versions d’évaluation nocturnes de l’interface CLI. Pour plus d’informations, consultez ces instructions sur l’[obtention des builds nocturnes](https://github.com/Azure/azure-cli#nightly-builds), ainsi que ces instructions sur [la contribution au code et la configuration d’un environnement de développement](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="93d0e-1654">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="93d0e-1655">Vous pouvez signaler des problèmes liés aux versions d’évaluation nocturnes comme suit :</span><span class="sxs-lookup"><span data-stu-id="93d0e-1655">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="93d0e-1656">Signalez des problèmes dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="93d0e-1656">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="93d0e-1657">Contactez l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="93d0e-1657">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="93d0e-1658">Fournissez des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="93d0e-1658">Provide feedback from the command line with the `az feedback` command</span></span>

