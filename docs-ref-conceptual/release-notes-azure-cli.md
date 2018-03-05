---
title: "Notes de publication d’Azure CLI 2.0"
description: "En savoir plus sur les dernières mises à jour d’Azure CLI 2.0"
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 02/27/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 01078b7a3665f563f0a6b1d809c9a41f18d136d6
ms.sourcegitcommit: f3ab5da6019083ef2482b62c7355817e6170dcfb
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/28/2018
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="14a9b-103">Notes de publication d’Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="14a9b-103">Azure CLI 2.0 release notes</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="14a9b-104">27 février 2018</span><span class="sxs-lookup"><span data-stu-id="14a9b-104">February 27, 2018</span></span>

<span data-ttu-id="14a9b-105">Version 2.0.28</span><span class="sxs-lookup"><span data-stu-id="14a9b-105">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="14a9b-106">Principal</span><span class="sxs-lookup"><span data-stu-id="14a9b-106">Core</span></span>

* <span data-ttu-id="14a9b-107">Résolu [#5184](https://github.com/Azure/azure-cli/issues/5184) : Problème d’installation d’Homebrew</span><span class="sxs-lookup"><span data-stu-id="14a9b-107">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="14a9b-108">Ajout de la prise en charge de télémétrie d’extension avec des clés personnalisées</span><span class="sxs-lookup"><span data-stu-id="14a9b-108">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="14a9b-109">Ajout de la connexion HTTP à `--debug`</span><span class="sxs-lookup"><span data-stu-id="14a9b-109">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="14a9b-110">ACS</span><span class="sxs-lookup"><span data-stu-id="14a9b-110">ACS</span></span>

* <span data-ttu-id="14a9b-111">Modification pour utiliser le graphique Helm `virtual-kubelet-for-aks` pour `aks install-connector` par défaut</span><span class="sxs-lookup"><span data-stu-id="14a9b-111">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="14a9b-112">Problème résolu : autorisation insuffisante des principaux de service à créer des groupes de conteneur ACI</span><span class="sxs-lookup"><span data-stu-id="14a9b-112">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="14a9b-113">Ajout des paramètres `--aci-container-group`, `--location` et `--image-tag` à `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="14a9b-113">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="14a9b-114">Suppression de l’avis de désapprobation de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="14a9b-114">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="14a9b-115">AppService</span><span class="sxs-lookup"><span data-stu-id="14a9b-115">Appservice</span></span>

* <span data-ttu-id="14a9b-116">Mises à jour pour la nouvelle version du kit de développement logiciel (SDK) (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="14a9b-116">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="14a9b-117">Résolu [#5538](https://github.com/Azure/azure-cli/issues/5538) : `Free` défini comme une SKU invalide</span><span class="sxs-lookup"><span data-stu-id="14a9b-117">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="14a9b-118">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="14a9b-118">Cognitive Services</span></span>

* <span data-ttu-id="14a9b-119">Mise à jour de l’avis lors de la création d’un compte Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="14a9b-119">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="14a9b-120">Consommation</span><span class="sxs-lookup"><span data-stu-id="14a9b-120">Consumption</span></span>

* <span data-ttu-id="14a9b-121">Ajout de nouvelles commandes pour l’API priceSheet</span><span class="sxs-lookup"><span data-stu-id="14a9b-121">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="14a9b-122">Mise à jour des formats existants Détails d’utilisations et Détails de la réservation</span><span class="sxs-lookup"><span data-stu-id="14a9b-122">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="14a9b-123">Conteneur</span><span class="sxs-lookup"><span data-stu-id="14a9b-123">Container</span></span>

* <span data-ttu-id="14a9b-124">Ajout des arguments `--secrets` et `--secrets-mount-path` à `container create` pour utiliser des secrets dans ACI</span><span class="sxs-lookup"><span data-stu-id="14a9b-124">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="14a9b-125">Réseau</span><span class="sxs-lookup"><span data-stu-id="14a9b-125">Network</span></span>

* <span data-ttu-id="14a9b-126">Résolu [#5559](https://github.com/Azure/azure-cli/issues/5559) : client manquant dans `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="14a9b-126">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="14a9b-127">Ressource</span><span class="sxs-lookup"><span data-stu-id="14a9b-127">Resource</span></span>

* <span data-ttu-id="14a9b-128">Modification de `group deployment export` pour afficher un modèle et des erreurs partiels sur échec</span><span class="sxs-lookup"><span data-stu-id="14a9b-128">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="14a9b-129">Rôle</span><span class="sxs-lookup"><span data-stu-id="14a9b-129">Role</span></span>

* <span data-ttu-id="14a9b-130">Ajout de `role assignment list-changelogs` pour permettre l’audit des rôles du principal de service</span><span class="sxs-lookup"><span data-stu-id="14a9b-130">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="14a9b-131">SQL</span><span class="sxs-lookup"><span data-stu-id="14a9b-131">SQL</span></span>

* <span data-ttu-id="14a9b-132">Ajout de la prise en charge de la redondance de zone pour les bases de données et les pools élastiques lors de création et mise à jour</span><span class="sxs-lookup"><span data-stu-id="14a9b-132">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="14a9b-133">Stockage</span><span class="sxs-lookup"><span data-stu-id="14a9b-133">Storage</span></span>

* <span data-ttu-id="14a9b-134">Activation de la spécification de préfixe/destination pour `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="14a9b-134">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="14a9b-135">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14a9b-135">VM</span></span>

* <span data-ttu-id="14a9b-136">Ajout de prise en charge de jonction / séparation de disques sur une instance de groupe de machines virtuelles identiques uniques</span><span class="sxs-lookup"><span data-stu-id="14a9b-136">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="14a9b-137">13 février 2018</span><span class="sxs-lookup"><span data-stu-id="14a9b-137">February 13, 2018</span></span>

<span data-ttu-id="14a9b-138">Version 2.0.27</span><span class="sxs-lookup"><span data-stu-id="14a9b-138">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="14a9b-139">Principal</span><span class="sxs-lookup"><span data-stu-id="14a9b-139">Core</span></span>

* <span data-ttu-id="14a9b-140">Modification de l’authentification pour passer au système de clé sur l’ID d’abonnement et le nom sur la connexion MSI</span><span class="sxs-lookup"><span data-stu-id="14a9b-140">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="14a9b-141">ACS</span><span class="sxs-lookup"><span data-stu-id="14a9b-141">ACS</span></span>

* <span data-ttu-id="14a9b-142">[CHANGEMENT] `aks get-versions` renommé en `aks get-upgrades` pour des raisons de précision</span><span class="sxs-lookup"><span data-stu-id="14a9b-142">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="14a9b-143">Modification de `aks get-versions` pour afficher les versions Kubernetes disponibles pour `aks create`</span><span class="sxs-lookup"><span data-stu-id="14a9b-143">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="14a9b-144">Modification des valeurs par défaut de `aks create` de manière à laisser le serveur choisir la version de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="14a9b-144">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="14a9b-145">Mise à jour des messages d’aide faisant référence au principal du service généré par AKS</span><span class="sxs-lookup"><span data-stu-id="14a9b-145">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="14a9b-146">Modification des tailles de nœud par défaut pour `aks create` pour passer de « Standard\_D1\_v2 » à « Standard\_DS1\_v2 »</span><span class="sxs-lookup"><span data-stu-id="14a9b-146">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="14a9b-147">Meilleure fiabilité lors de la localisation du pod de tableau de bord pour `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="14a9b-147">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="14a9b-148">Correction de `aks get-credentials` pour gérer les erreurs Unicode lors du chargement des fichiers de configuration Kubernetes</span><span class="sxs-lookup"><span data-stu-id="14a9b-148">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="14a9b-149">Ajout d’un message à `az aks install-cli` pour aider à l’obtention de `kubectl` dans `$PATH`</span><span class="sxs-lookup"><span data-stu-id="14a9b-149">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="14a9b-150">AppService</span><span class="sxs-lookup"><span data-stu-id="14a9b-150">Appservice</span></span>

* <span data-ttu-id="14a9b-151">Résolution du problème dans lequel `webapp [backup|restore]` a échoué en raison d’une référence null</span><span class="sxs-lookup"><span data-stu-id="14a9b-151">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="14a9b-152">Ajout de la prise en charge supplémentaire des plans App Service par défaut via `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="14a9b-152">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="14a9b-153">CDN</span><span class="sxs-lookup"><span data-stu-id="14a9b-153">CDN</span></span>

* <span data-ttu-id="14a9b-154">Ajout des commandes `cdn custom-domain [enable-https|disable-https]`</span><span class="sxs-lookup"><span data-stu-id="14a9b-154">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="14a9b-155">Conteneur</span><span class="sxs-lookup"><span data-stu-id="14a9b-155">Container</span></span>

* <span data-ttu-id="14a9b-156">Ajout de l’option `--follow` à `az container logs` pour les journaux de diffusion en continu</span><span class="sxs-lookup"><span data-stu-id="14a9b-156">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="14a9b-157">Ajout de la commande `container attach` qui associe les flux d’erreur et de sortie standard locaux à un conteneur d’un groupe de conteneur</span><span class="sxs-lookup"><span data-stu-id="14a9b-157">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="14a9b-158">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="14a9b-158">CosmosDB</span></span>

* <span data-ttu-id="14a9b-159">Ajout de la prise en charge de la définition de fonctionnalités</span><span class="sxs-lookup"><span data-stu-id="14a9b-159">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="14a9b-160">Extension</span><span class="sxs-lookup"><span data-stu-id="14a9b-160">Extension</span></span>

* <span data-ttu-id="14a9b-161">Ajout de la prise en charge du paramètre `--pip-proxy` pour les commandes `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="14a9b-161">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="14a9b-162">Ajout de la prise en charge de l’argument `--pip-extra-index-urls` pour les commandes `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="14a9b-162">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="14a9b-163">Commentaires</span><span class="sxs-lookup"><span data-stu-id="14a9b-163">Feedback</span></span>

* <span data-ttu-id="14a9b-164">Ajout d’informations d’extension aux données de télémétrie</span><span class="sxs-lookup"><span data-stu-id="14a9b-164">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="14a9b-165">Interactive</span><span class="sxs-lookup"><span data-stu-id="14a9b-165">Interactive</span></span>

* <span data-ttu-id="14a9b-166">Résolution du problème dans lequel l’utilisateur est invité à se connecter à l’aide du mode interactif dans Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="14a9b-166">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="14a9b-167">Correction de la régression avec les listes de saisie semi-automatique des paramètres manquants</span><span class="sxs-lookup"><span data-stu-id="14a9b-167">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="14a9b-168">IoT</span><span class="sxs-lookup"><span data-stu-id="14a9b-168">IoT</span></span>

* <span data-ttu-id="14a9b-169">Résolution du problème dans lequel `iot dps access policy [create|update]` renvoie une erreur « introuvable » en cas de réussite.</span><span class="sxs-lookup"><span data-stu-id="14a9b-169">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success.</span></span>
* <span data-ttu-id="14a9b-170">Résolution du problème dans lequel `iot dps linked-hub [create|update]` renvoie une erreur « introuvable » en cas de réussite.</span><span class="sxs-lookup"><span data-stu-id="14a9b-170">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success.</span></span>
* <span data-ttu-id="14a9b-171">Ajout de la prise en charge de `--no-wait` pour `iot dps access policy [create|update]` et `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="14a9b-171">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="14a9b-172">Modification de `iot hub create` pour autoriser la spécification du nombre de partitions</span><span class="sxs-lookup"><span data-stu-id="14a9b-172">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="14a9b-173">Surveiller</span><span class="sxs-lookup"><span data-stu-id="14a9b-173">Monitor</span></span>

* <span data-ttu-id="14a9b-174">Correction de la commande `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="14a9b-174">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="14a9b-175">Réseau</span><span class="sxs-lookup"><span data-stu-id="14a9b-175">Network</span></span>

* <span data-ttu-id="14a9b-176">Correction de l’option `--tags` pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="14a9b-176">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="14a9b-177">Profil</span><span class="sxs-lookup"><span data-stu-id="14a9b-177">Profile</span></span>

* <span data-ttu-id="14a9b-178">Activation `az login` à partir du mode interactif</span><span class="sxs-lookup"><span data-stu-id="14a9b-178">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="14a9b-179">Ressource</span><span class="sxs-lookup"><span data-stu-id="14a9b-179">Resource</span></span>

* <span data-ttu-id="14a9b-180">Rajout de `feature show`</span><span class="sxs-lookup"><span data-stu-id="14a9b-180">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="14a9b-181">Rôle</span><span class="sxs-lookup"><span data-stu-id="14a9b-181">Role</span></span>

* <span data-ttu-id="14a9b-182">Ajout de l’argument `--available-to-other-tenants` à `ad app update`</span><span class="sxs-lookup"><span data-stu-id="14a9b-182">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="14a9b-183">SQL</span><span class="sxs-lookup"><span data-stu-id="14a9b-183">SQL</span></span>

* <span data-ttu-id="14a9b-184">Ajout des commandes `sql server dns-alias`</span><span class="sxs-lookup"><span data-stu-id="14a9b-184">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="14a9b-185">Ajout de `sql db rename`</span><span class="sxs-lookup"><span data-stu-id="14a9b-185">Added `sql db rename`</span></span>
* <span data-ttu-id="14a9b-186">Ajout de la prise en charge de l’argument `--ids` pour toutes les commandes sql</span><span class="sxs-lookup"><span data-stu-id="14a9b-186">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="14a9b-187">Stockage</span><span class="sxs-lookup"><span data-stu-id="14a9b-187">Storage</span></span>

* <span data-ttu-id="14a9b-188">Ajout des commandes `storage blob service-properties delete-policy` et `storage blob undelete` pour permettre une suppression réversible</span><span class="sxs-lookup"><span data-stu-id="14a9b-188">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="14a9b-189">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14a9b-189">VM</span></span>

* <span data-ttu-id="14a9b-190">Correction d’un incident lorsque le chiffrement de la machine virtuelle ne peut pas être initialisé entièrement</span><span class="sxs-lookup"><span data-stu-id="14a9b-190">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="14a9b-191">Ajout de la sortie d’ID du principal lors de l’activation de MSI</span><span class="sxs-lookup"><span data-stu-id="14a9b-191">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="14a9b-192">`vm boot-diagnostics get-boot-log` fixe</span><span class="sxs-lookup"><span data-stu-id="14a9b-192">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="14a9b-193">31 janvier 2018</span><span class="sxs-lookup"><span data-stu-id="14a9b-193">January 31, 2018</span></span>

<span data-ttu-id="14a9b-194">Version 2.0.26</span><span class="sxs-lookup"><span data-stu-id="14a9b-194">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="14a9b-195">Principal</span><span class="sxs-lookup"><span data-stu-id="14a9b-195">Core</span></span>

* <span data-ttu-id="14a9b-196">Ajout de la prise en charge de la récupération du jeton brut dans le contexte MSI</span><span class="sxs-lookup"><span data-stu-id="14a9b-196">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="14a9b-197">Suppression de la chaîne de l’indicateur d’interrogation après la fin de LRO sur le fichier cmd.exe de Windows</span><span class="sxs-lookup"><span data-stu-id="14a9b-197">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="14a9b-198">Ajout d’un avertissement qui s’affiche lorsque l’utilisation d’une valeur par défaut configurée a été remplacée par une entrée de niveau INFO.</span><span class="sxs-lookup"><span data-stu-id="14a9b-198">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="14a9b-199">Utilisation de `--verbose` pour voir</span><span class="sxs-lookup"><span data-stu-id="14a9b-199">Use `--verbose` to see</span></span>
* <span data-ttu-id="14a9b-200">Ajouter un indicateur de progression pour les commandes wait</span><span class="sxs-lookup"><span data-stu-id="14a9b-200">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="14a9b-201">ACS</span><span class="sxs-lookup"><span data-stu-id="14a9b-201">ACS</span></span>

* <span data-ttu-id="14a9b-202">Clarification de l’argument `--disable-browser`</span><span class="sxs-lookup"><span data-stu-id="14a9b-202">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="14a9b-203">Amélioration de la touche TAB pour les arguments `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="14a9b-203">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="14a9b-204">AppService</span><span class="sxs-lookup"><span data-stu-id="14a9b-204">Appservice</span></span>

* <span data-ttu-id="14a9b-205">`webapp log [tail|download]` fixe</span><span class="sxs-lookup"><span data-stu-id="14a9b-205">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="14a9b-206">Suppression de la vérification de `kind` sur les fonctions et les applications web</span><span class="sxs-lookup"><span data-stu-id="14a9b-206">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="14a9b-207">CDN</span><span class="sxs-lookup"><span data-stu-id="14a9b-207">CDN</span></span>

* <span data-ttu-id="14a9b-208">Résolution du problème de client manquant avec `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="14a9b-208">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="14a9b-209">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="14a9b-209">CosmosDB</span></span>

* <span data-ttu-id="14a9b-210">Correction de la description du paramètre pour les stratégies de basculement</span><span class="sxs-lookup"><span data-stu-id="14a9b-210">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="14a9b-211">Interactive</span><span class="sxs-lookup"><span data-stu-id="14a9b-211">Interactive</span></span>

* <span data-ttu-id="14a9b-212">Résolution du problème dans lequel les listes de saisie semi-automatique d’option de commande ne s’affichent plus</span><span class="sxs-lookup"><span data-stu-id="14a9b-212">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="14a9b-213">Réseau</span><span class="sxs-lookup"><span data-stu-id="14a9b-213">Network</span></span>

* <span data-ttu-id="14a9b-214">Ajout de la protection pour `--cert-password` à `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="14a9b-214">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="14a9b-215">Résolution du problème lié à `application-gateway update` où `--sku` a appliqué par erreur une valeur par défaut</span><span class="sxs-lookup"><span data-stu-id="14a9b-215">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="14a9b-216">Ajout de la protection pour `--shared-key` et `--authorization-key` à `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="14a9b-216">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="14a9b-217">Résolution du problème de client manquant avec `asg create`</span><span class="sxs-lookup"><span data-stu-id="14a9b-217">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="14a9b-218">Ajout du paramètre `--file-name / -f` pour les noms exportés à `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="14a9b-218">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="14a9b-219">Les problèmes suivants liés à `dns zone export` ont été résolus :</span><span class="sxs-lookup"><span data-stu-id="14a9b-219">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="14a9b-220">Résolution du problème dans lequel des enregistrements TXT longs ont été mal exportés</span><span class="sxs-lookup"><span data-stu-id="14a9b-220">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="14a9b-221">Résolution du problème dans lequel des enregistrements TXT entre guillemets ont été mal exportés sans guillemets placés dans une séquence d’échappement.</span><span class="sxs-lookup"><span data-stu-id="14a9b-221">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="14a9b-222">Résolution du problème où certains enregistrements ont été importés à deux reprises avec `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="14a9b-222">Fixed issue where certain records were imported twice with `dns zone import`</span></span> 
* <span data-ttu-id="14a9b-223">Restauration des commandes `vnet-gateway root-cert` et `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="14a9b-223">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="14a9b-224">Profil</span><span class="sxs-lookup"><span data-stu-id="14a9b-224">Profile</span></span>

* <span data-ttu-id="14a9b-225">Correction de `get-access-token` pour qu’il fonctionne à l’intérieur d’une machine virtuelle avec l’identité</span><span class="sxs-lookup"><span data-stu-id="14a9b-225">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="14a9b-226">Ressource</span><span class="sxs-lookup"><span data-stu-id="14a9b-226">Resource</span></span>

* <span data-ttu-id="14a9b-227">Correction du bogue lié à `deployment [create|validate]` où un avertissement ne s’est pas affiché correctement quand un champ ’type’ du modèle contient des valeurs en majuscules</span><span class="sxs-lookup"><span data-stu-id="14a9b-227">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="14a9b-228">Stockage</span><span class="sxs-lookup"><span data-stu-id="14a9b-228">Storage</span></span>

* <span data-ttu-id="14a9b-229">Résolution du problème lié à la migration des comptes Storage V1 vers Storage V2</span><span class="sxs-lookup"><span data-stu-id="14a9b-229">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="14a9b-230">Ajout de la création progressive de rapports pour toutes les commandes de chargement/téléchargement</span><span class="sxs-lookup"><span data-stu-id="14a9b-230">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="14a9b-231">Résolution du bogue empêchant l’option d’argument « -n » avec `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="14a9b-231">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>  
* <span data-ttu-id="14a9b-232">Ajout de la colonne de « snapshot » ajouté à la sortie de table pour `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="14a9b-232">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="14a9b-233">Résolution des bogues dans lesquels différents paramètres devaient être analysés en tant qu’entiers</span><span class="sxs-lookup"><span data-stu-id="14a9b-233">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="14a9b-234">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14a9b-234">VM</span></span>

* <span data-ttu-id="14a9b-235">Ajout de la commande `vm image accept-terms` pour autoriser la création de machines virtuelles à partir d’images moyennant des frais supplémentaires</span><span class="sxs-lookup"><span data-stu-id="14a9b-235">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="14a9b-236">Correction de `[vm|vmss create]` pour garantir l’exécution des commandes sous un proxy avec des certificats non signés</span><span class="sxs-lookup"><span data-stu-id="14a9b-236">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="14a9b-237">[APERÇU] Ajout de la prise en charge de la priorité « faible» au groupe de machines virtuelles identiques</span><span class="sxs-lookup"><span data-stu-id="14a9b-237">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="14a9b-238">Ajout de la protection pour `--admin-password` à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="14a9b-238">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="14a9b-239">17 janvier 2018</span><span class="sxs-lookup"><span data-stu-id="14a9b-239">January 17, 2018</span></span>

<span data-ttu-id="14a9b-240">Version 2.0.25</span><span class="sxs-lookup"><span data-stu-id="14a9b-240">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="14a9b-241">ACR</span><span class="sxs-lookup"><span data-stu-id="14a9b-241">ACR</span></span>

* <span data-ttu-id="14a9b-242">Ajout d’une connexion acr de secours en cas d’erreurs d’informations d’identification Windows</span><span class="sxs-lookup"><span data-stu-id="14a9b-242">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="14a9b-243">Activation des journaux du Registre</span><span class="sxs-lookup"><span data-stu-id="14a9b-243">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="14a9b-244">ACS</span><span class="sxs-lookup"><span data-stu-id="14a9b-244">ACS</span></span>

* <span data-ttu-id="14a9b-245">Correction de la commande `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="14a9b-245">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="14a9b-246">Suppression de l’exigence de rôle SPN</span><span class="sxs-lookup"><span data-stu-id="14a9b-246">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="14a9b-247">AppService</span><span class="sxs-lookup"><span data-stu-id="14a9b-247">Appservice</span></span>

* <span data-ttu-id="14a9b-248">Correction du bogue avec `config ssl upload` où `hosting_environment_profile` avait la valeur null</span><span class="sxs-lookup"><span data-stu-id="14a9b-248">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="14a9b-249">Ajout de la prise en charge des URL personnalisées pour `browse`</span><span class="sxs-lookup"><span data-stu-id="14a9b-249">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="14a9b-250">Prise en charge de l’emplacement fixe pour `log tail`</span><span class="sxs-lookup"><span data-stu-id="14a9b-250">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="14a9b-251">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="14a9b-251">Backup</span></span>

* <span data-ttu-id="14a9b-252">Modification de l’option `--container-name` de `backup item list` désormais facultative</span><span class="sxs-lookup"><span data-stu-id="14a9b-252">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="14a9b-253">Ajout d’options de compte de stockage à `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="14a9b-253">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="14a9b-254">Correction de la vérification de l’emplacement dans `backup protection enable-for-vm`, ne tient désormais plus compte de la casse</span><span class="sxs-lookup"><span data-stu-id="14a9b-254">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="14a9b-255">Correction d’un problème qui causait l’échec des commandes avec un nom de conteneur non valide</span><span class="sxs-lookup"><span data-stu-id="14a9b-255">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="14a9b-256">Modification de `backup item list` pour inclure « État d’intégrité » par défaut</span><span class="sxs-lookup"><span data-stu-id="14a9b-256">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="14a9b-257">Batch</span><span class="sxs-lookup"><span data-stu-id="14a9b-257">Batch</span></span>

* <span data-ttu-id="14a9b-258">Modification de `batch login` pour retourner des détails d’authentification</span><span class="sxs-lookup"><span data-stu-id="14a9b-258">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="14a9b-259">Cloud</span><span class="sxs-lookup"><span data-stu-id="14a9b-259">Cloud</span></span>

* <span data-ttu-id="14a9b-260">Ne requiert plus de points de terminaison lors de la définition de `--profile` sur un cloud</span><span class="sxs-lookup"><span data-stu-id="14a9b-260">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="14a9b-261">Consommation</span><span class="sxs-lookup"><span data-stu-id="14a9b-261">Consumption</span></span>

* <span data-ttu-id="14a9b-262">Ajout de nouvelles commandes pour les réservations : `consumption reservations summaries` et `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="14a9b-262">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="14a9b-263">Event Grid</span><span class="sxs-lookup"><span data-stu-id="14a9b-263">Event Grid</span></span>

* <span data-ttu-id="14a9b-264">[MODIFICATION CRITIQUE] Déplacement des commandes `az eventgrid topic event-subscription` vers `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="14a9b-264">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="14a9b-265">[MODIFICATION CRITIQUE] Déplacement des commandes `az eventgrid resource event-subscription` vers `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="14a9b-265">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="14a9b-266">[MODIFICATION CRITIQUE] Suppression de la commande `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="14a9b-266">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="14a9b-267">Utilisation de `eventgrid event-subscription show --include-full-endpoint-url` à la place</span><span class="sxs-lookup"><span data-stu-id="14a9b-267">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="14a9b-268">Ajout de la commande `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="14a9b-268">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="14a9b-269">Ajout de la commande `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="14a9b-269">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="14a9b-270">Ajout du paramètre `--ids` pour les commandes `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="14a9b-270">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="14a9b-271">Ajout de la prise en charge de la saisie semi-automatique via la touche TAB pour les noms de rubrique</span><span class="sxs-lookup"><span data-stu-id="14a9b-271">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="14a9b-272">Interactive</span><span class="sxs-lookup"><span data-stu-id="14a9b-272">Interactive</span></span>

* <span data-ttu-id="14a9b-273">Correction d’un problème qui empêchait le fonctionnement du mode interactif avec Python 2.x</span><span class="sxs-lookup"><span data-stu-id="14a9b-273">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="14a9b-274">Corrections d’erreurs au démarrage</span><span class="sxs-lookup"><span data-stu-id="14a9b-274">Fixed errors on startup</span></span>
* <span data-ttu-id="14a9b-275">Correction du problème de commandes ne s’exécutant pas en mode interactif</span><span class="sxs-lookup"><span data-stu-id="14a9b-275">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="14a9b-276">IoT</span><span class="sxs-lookup"><span data-stu-id="14a9b-276">IoT</span></span>

* <span data-ttu-id="14a9b-277">Ajout de la prise en charge du service de provisionnement des appareils</span><span class="sxs-lookup"><span data-stu-id="14a9b-277">Added support for device provisioning service</span></span>
* <span data-ttu-id="14a9b-278">Ajout de messages de désapprobation dans les commandes et l’aide relative aux commandes</span><span class="sxs-lookup"><span data-stu-id="14a9b-278">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="14a9b-279">Ajout de la vérification IoT pour informer les utilisateurs de l’extension IoT</span><span class="sxs-lookup"><span data-stu-id="14a9b-279">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="14a9b-280">Surveiller</span><span class="sxs-lookup"><span data-stu-id="14a9b-280">Monitor</span></span>

* <span data-ttu-id="14a9b-281">Ajout de la prise en charge des paramètres multi diagnostic.</span><span class="sxs-lookup"><span data-stu-id="14a9b-281">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="14a9b-282">Le paramètre `--name` est désormais requis pour `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="14a9b-282">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="14a9b-283">Ajout de la commande `monitor diagnostic-settings categories` pour obtenir la catégorie des paramètres de diagnostic</span><span class="sxs-lookup"><span data-stu-id="14a9b-283">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="14a9b-284">Réseau</span><span class="sxs-lookup"><span data-stu-id="14a9b-284">Network</span></span>

* <span data-ttu-id="14a9b-285">Résolution du problème se produisant lors de la tentative de passage au mode actif-passif, ou depuis ce dernier, avec `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="14a9b-285">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="14a9b-286">Ajout de la prise en charge de HTTP2 vers `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="14a9b-286">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="14a9b-287">Profil</span><span class="sxs-lookup"><span data-stu-id="14a9b-287">Profile</span></span>

* <span data-ttu-id="14a9b-288">Ajout de la prise en charge pour la connexion à l’aide d’identités affectées aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="14a9b-288">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="14a9b-289">Rôle</span><span class="sxs-lookup"><span data-stu-id="14a9b-289">Role</span></span>

* <span data-ttu-id="14a9b-290">Ajout de l’argument `--assignee-object-id` à `role assignment create` pour ignorer les requêtes de graphique</span><span class="sxs-lookup"><span data-stu-id="14a9b-290">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="14a9b-291">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="14a9b-291">Service Fabric</span></span>

* <span data-ttu-id="14a9b-292">Ajout d’erreurs détaillées à la réponse de validation lors de la création du cluster</span><span class="sxs-lookup"><span data-stu-id="14a9b-292">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="14a9b-293">Résolution du problème concernant le client manquant avec plusieurs commandes</span><span class="sxs-lookup"><span data-stu-id="14a9b-293">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="14a9b-294">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14a9b-294">VM</span></span>

* <span data-ttu-id="14a9b-295">[PRÉVERSION] Prise en charge interzone pour `vmss`</span><span class="sxs-lookup"><span data-stu-id="14a9b-295">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="14a9b-296">[MODIFICATION CRITIQUE] Modification de zone unique `vmss` par défaut en équilibreur de charge « Standard »</span><span class="sxs-lookup"><span data-stu-id="14a9b-296">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="14a9b-297">[MODIFICATION CRITIQUE] Modification de `externalIdentities` en `userAssignedIdentities` pour EMSI</span><span class="sxs-lookup"><span data-stu-id="14a9b-297">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="14a9b-298">[PRÉVERSION] Ajout de la prise en charge de l’échange de disque du système d’exploitation</span><span class="sxs-lookup"><span data-stu-id="14a9b-298">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="14a9b-299">Ajout de la prise en charge de l’utilisation des images de machine virtuelle à partir d’autres abonnements</span><span class="sxs-lookup"><span data-stu-id="14a9b-299">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="14a9b-300">Ajout des arguments `--plan-name`, `--plan-product`, `--plan-promotion-code` et `--plan-publisher` à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="14a9b-300">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="14a9b-301">Correction des problèmes d’erreur avec `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="14a9b-301">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="14a9b-302">Correction de l’utilisation excessive des ressources due à `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="14a9b-302">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="14a9b-303">19 décembre 2017</span><span class="sxs-lookup"><span data-stu-id="14a9b-303">December 19, 2017</span></span>

<span data-ttu-id="14a9b-304">Version 2.0.23</span><span class="sxs-lookup"><span data-stu-id="14a9b-304">Version 2.0.23</span></span>

* <span data-ttu-id="14a9b-305">Ajout de la prise en charge pour la connexion à l’aide d’identités affectées aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="14a9b-305">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="14a9b-306">Conteneur</span><span class="sxs-lookup"><span data-stu-id="14a9b-306">Container</span></span>

* <span data-ttu-id="14a9b-307">Correction de l’ordre incorrect des paramètres pour les journaux du conteneur</span><span class="sxs-lookup"><span data-stu-id="14a9b-307">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="14a9b-308">Réseau</span><span class="sxs-lookup"><span data-stu-id="14a9b-308">Network</span></span>

* <span data-ttu-id="14a9b-309">Ajout de l’argument `--disable-bgp-route-propagation` à `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="14a9b-309">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="14a9b-310">Ajout de l’argument `--ip-tags` à `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="14a9b-310">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="14a9b-311">Stockage</span><span class="sxs-lookup"><span data-stu-id="14a9b-311">Storage</span></span>

* <span data-ttu-id="14a9b-312">Ajout de la prise en charge du stockage V2</span><span class="sxs-lookup"><span data-stu-id="14a9b-312">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="14a9b-313">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14a9b-313">VM</span></span>

* <span data-ttu-id="14a9b-314">[APERÇU] Ajout de la prise en charge des identités affectées aux utilisateurs pour les machines virtuelles et les VMSS</span><span class="sxs-lookup"><span data-stu-id="14a9b-314">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="14a9b-315">5 décembre 2017</span><span class="sxs-lookup"><span data-stu-id="14a9b-315">December 5, 2017</span></span>

<span data-ttu-id="14a9b-316">Version 2.0.22</span><span class="sxs-lookup"><span data-stu-id="14a9b-316">Version 2.0.22</span></span>

* <span data-ttu-id="14a9b-317">Suppression des commandes `az component`.</span><span class="sxs-lookup"><span data-stu-id="14a9b-317">Removed `az component` commands.</span></span> <span data-ttu-id="14a9b-318">Utilisation de `az extension` à la place</span><span class="sxs-lookup"><span data-stu-id="14a9b-318">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="14a9b-319">Principal</span><span class="sxs-lookup"><span data-stu-id="14a9b-319">Core</span></span>
* <span data-ttu-id="14a9b-320">Modification du point de terminaison de l’autorité AAD `AZURE_US_GOV_CLOUD` pour le faire passer de login.microsoftonline.com à login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="14a9b-320">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="14a9b-321">Résolution du problème au cours duquel les données de télémétrie étaient constamment renvoyées</span><span class="sxs-lookup"><span data-stu-id="14a9b-321">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="14a9b-322">ACS</span><span class="sxs-lookup"><span data-stu-id="14a9b-322">ACS</span></span>

* <span data-ttu-id="14a9b-323">Ajout des commandes `aks install-connector` et `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="14a9b-323">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="14a9b-324">Amélioration des rapports d’erreurs pour `acs create`</span><span class="sxs-lookup"><span data-stu-id="14a9b-324">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="14a9b-325">Correction de l’utilisation de `aks get-credentials -f` sans chemin d’accès complet</span><span class="sxs-lookup"><span data-stu-id="14a9b-325">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="14a9b-326">Advisor</span><span class="sxs-lookup"><span data-stu-id="14a9b-326">Advisor</span></span>

* <span data-ttu-id="14a9b-327">Version initiale</span><span class="sxs-lookup"><span data-stu-id="14a9b-327">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="14a9b-328">AppService</span><span class="sxs-lookup"><span data-stu-id="14a9b-328">Appservice</span></span>

* <span data-ttu-id="14a9b-329">Correction de la génération du nom de certificat avec `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="14a9b-329">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="14a9b-330">Correction de `webapp [list|show]` et `functionapp [list|show]` de manière à afficher les applications correctes</span><span class="sxs-lookup"><span data-stu-id="14a9b-330">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="14a9b-331">Ajout de la valeur par défaut pour `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="14a9b-331">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="14a9b-332">Consommation</span><span class="sxs-lookup"><span data-stu-id="14a9b-332">Consumption</span></span>

* <span data-ttu-id="14a9b-333">Ajout de la prise en charge de l’API version 2017-11-30</span><span class="sxs-lookup"><span data-stu-id="14a9b-333">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="14a9b-334">Conteneur</span><span class="sxs-lookup"><span data-stu-id="14a9b-334">Container</span></span>

* <span data-ttu-id="14a9b-335">Correction de la régression des ports par défaut</span><span class="sxs-lookup"><span data-stu-id="14a9b-335">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="14a9b-336">Surveiller</span><span class="sxs-lookup"><span data-stu-id="14a9b-336">Monitor</span></span>

* <span data-ttu-id="14a9b-337">Ajout de la prise en charge de plusieurs dimensions à la commande des mesures</span><span class="sxs-lookup"><span data-stu-id="14a9b-337">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="14a9b-338">Ressource</span><span class="sxs-lookup"><span data-stu-id="14a9b-338">Resource</span></span>

* <span data-ttu-id="14a9b-339">Ajout de l’argument `--include-response-body` à `resource show`</span><span class="sxs-lookup"><span data-stu-id="14a9b-339">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="14a9b-340">Rôle</span><span class="sxs-lookup"><span data-stu-id="14a9b-340">Role</span></span>

* <span data-ttu-id="14a9b-341">Ajout de l’affichage des affectations par défaut pour les administrateurs « classiques » à `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="14a9b-341">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="14a9b-342">Ajout de la prise en charge à `ad sp reset-credentials` pour l’ajout d’informations d’identification au lieu de leur remplacement</span><span class="sxs-lookup"><span data-stu-id="14a9b-342">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="14a9b-343">Amélioration des rapports d’erreurs pour `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="14a9b-343">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="14a9b-344">SQL</span><span class="sxs-lookup"><span data-stu-id="14a9b-344">SQL</span></span>

* <span data-ttu-id="14a9b-345">Ajout des commandes `sql db list-usages` et `sql db show-usage`</span><span class="sxs-lookup"><span data-stu-id="14a9b-345">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="14a9b-346">Ajout des commandes `sql server conn-policy show` et `sql server conn-policy update`</span><span class="sxs-lookup"><span data-stu-id="14a9b-346">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="14a9b-347">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14a9b-347">VM</span></span>

* <span data-ttu-id="14a9b-348">Ajout des informations de zone à `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="14a9b-348">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="14a9b-349">14 novembre 2017</span><span class="sxs-lookup"><span data-stu-id="14a9b-349">November 14, 2017</span></span>

<span data-ttu-id="14a9b-350">Version 2.0.21</span><span class="sxs-lookup"><span data-stu-id="14a9b-350">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="14a9b-351">ACR</span><span class="sxs-lookup"><span data-stu-id="14a9b-351">ACR</span></span>

* <span data-ttu-id="14a9b-352">Ajout de la prise en charge pour la création de webhooks dans les régions de réplication</span><span class="sxs-lookup"><span data-stu-id="14a9b-352">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="14a9b-353">ACS</span><span class="sxs-lookup"><span data-stu-id="14a9b-353">ACS</span></span>

* <span data-ttu-id="14a9b-354">Modification de toutes les mentions « agent » en « nœud » dans AKS</span><span class="sxs-lookup"><span data-stu-id="14a9b-354">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="14a9b-355">Option `--orchestrator-release` déconseillée pour `acs create`</span><span class="sxs-lookup"><span data-stu-id="14a9b-355">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="14a9b-356">Changement de la taille de machine virtuelle par défaut pour AKS à `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="14a9b-356">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="14a9b-357">Résolution de `az aks browse` sur Windows</span><span class="sxs-lookup"><span data-stu-id="14a9b-357">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="14a9b-358">Résolution de `az aks get-credentials` sur Windows</span><span class="sxs-lookup"><span data-stu-id="14a9b-358">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="14a9b-359">AppService</span><span class="sxs-lookup"><span data-stu-id="14a9b-359">Appservice</span></span>

* <span data-ttu-id="14a9b-360">Ajout de la source de déploiement `config-zip` pour les applications Web et de fonction</span><span class="sxs-lookup"><span data-stu-id="14a9b-360">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="14a9b-361">Ajout de l’option `--docker-container-logging` à `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="14a9b-361">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="14a9b-362">Suppression de l’option `storage` du paramètre `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="14a9b-362">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="14a9b-363">Amélioration des messages d’erreur pour `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="14a9b-363">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="14a9b-364">Ajout de la prise en charge pour la création d’applications de fonction Linux</span><span class="sxs-lookup"><span data-stu-id="14a9b-364">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="14a9b-365">`list-locations` fixe</span><span class="sxs-lookup"><span data-stu-id="14a9b-365">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="14a9b-366">Batch</span><span class="sxs-lookup"><span data-stu-id="14a9b-366">Batch</span></span>

* <span data-ttu-id="14a9b-367">Correction du bogue dans la commande de création de pool lorsqu’un ID ressource a été utilisé avec l’indicateur `--image`</span><span class="sxs-lookup"><span data-stu-id="14a9b-367">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="14a9b-368">Batchai</span><span class="sxs-lookup"><span data-stu-id="14a9b-368">Batchai</span></span>

* <span data-ttu-id="14a9b-369">Ajout de l’option courte, `-s`, pour `--vm-size` quand la taille de machine virtuelle est fournie dans la commande `file-server create`</span><span class="sxs-lookup"><span data-stu-id="14a9b-369">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="14a9b-370">Ajout du nom de compte de stockage et des arguments de clé dans les paramètres `cluster create`</span><span class="sxs-lookup"><span data-stu-id="14a9b-370">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="14a9b-371">Résolution de la documentation pour `job list-files` et `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="14a9b-371">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="14a9b-372">Ajout de l’option courte, `-r`, pour `--cluster-name` quand le nom du cluster est fourni dans la commande `job create`</span><span class="sxs-lookup"><span data-stu-id="14a9b-372">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="14a9b-373">Cloud</span><span class="sxs-lookup"><span data-stu-id="14a9b-373">Cloud</span></span>

* <span data-ttu-id="14a9b-374">Modification de `cloud [register|update]` pour empêcher l’inscription des clouds qui ne disposent pas de tous les points de terminaison requis</span><span class="sxs-lookup"><span data-stu-id="14a9b-374">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="14a9b-375">Conteneur</span><span class="sxs-lookup"><span data-stu-id="14a9b-375">Container</span></span>

* <span data-ttu-id="14a9b-376">Ajout de la prise en charge pour ouvrir plusieurs ports</span><span class="sxs-lookup"><span data-stu-id="14a9b-376">Added support to open multiple ports</span></span>
* <span data-ttu-id="14a9b-377">Ajout de la stratégie de redémarrage du groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="14a9b-377">Added container group restart policy</span></span>
* <span data-ttu-id="14a9b-378">Ajout de la prise en charge pour monter le partage de fichier Azure en tant que volume</span><span class="sxs-lookup"><span data-stu-id="14a9b-378">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="14a9b-379">Mise à jour des documents d’assistance</span><span class="sxs-lookup"><span data-stu-id="14a9b-379">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="14a9b-380">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="14a9b-380">Data Lake Analytics</span></span>

* <span data-ttu-id="14a9b-381">Modification de `[job|account] list` pour retourner des informations plus concises</span><span class="sxs-lookup"><span data-stu-id="14a9b-381">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="14a9b-382">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="14a9b-382">Data Lake Store</span></span>

* <span data-ttu-id="14a9b-383">Modification de `account list` pour retourner des informations plus concises</span><span class="sxs-lookup"><span data-stu-id="14a9b-383">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="14a9b-384">Extension</span><span class="sxs-lookup"><span data-stu-id="14a9b-384">Extension</span></span>

* <span data-ttu-id="14a9b-385">Ajout de `extension list-available` pour permettre l’affichage de la liste des extensions officielles Microsoft</span><span class="sxs-lookup"><span data-stu-id="14a9b-385">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="14a9b-386">Ajout de `--name` à `extension [add|update]` pour permettre l’installation des extensions par nom</span><span class="sxs-lookup"><span data-stu-id="14a9b-386">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="14a9b-387">IoT</span><span class="sxs-lookup"><span data-stu-id="14a9b-387">IoT</span></span>

* <span data-ttu-id="14a9b-388">Ajout de la prise en charge pour les autorités de certification (CA) et les chaînes d’approbation</span><span class="sxs-lookup"><span data-stu-id="14a9b-388">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="14a9b-389">Surveiller</span><span class="sxs-lookup"><span data-stu-id="14a9b-389">Monitor</span></span>

* <span data-ttu-id="14a9b-390">Ajout des commandes `activity-log alert`</span><span class="sxs-lookup"><span data-stu-id="14a9b-390">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="14a9b-391">Réseau</span><span class="sxs-lookup"><span data-stu-id="14a9b-391">Network</span></span>

* <span data-ttu-id="14a9b-392">Ajout de la prise en charge pour les enregistrements DNS CAA</span><span class="sxs-lookup"><span data-stu-id="14a9b-392">Added support for CAA DNS records</span></span>
* <span data-ttu-id="14a9b-393">Résolution d’un problème empêchant la mise à jour des points de terminaison avec `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="14a9b-393">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="14a9b-394">Résolution d’un problème où `vnet update --dns-servers` ne fonctionnait pas, en fonction de la façon dont avait été créé le réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="14a9b-394">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="14a9b-395">Résolution d’un problème où les noms DNS relatifs n’étaient pas importés correctement par `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="14a9b-395">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="14a9b-396">Réservations</span><span class="sxs-lookup"><span data-stu-id="14a9b-396">Reservations</span></span>

* <span data-ttu-id="14a9b-397">Version préliminaire initiale</span><span class="sxs-lookup"><span data-stu-id="14a9b-397">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="14a9b-398">Ressource</span><span class="sxs-lookup"><span data-stu-id="14a9b-398">Resource</span></span>

* <span data-ttu-id="14a9b-399">Ajout de la prise en charge pour les ID de ressource au paramètre `--resource` et pour les verrous au niveau des ressources</span><span class="sxs-lookup"><span data-stu-id="14a9b-399">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="14a9b-400">SQL</span><span class="sxs-lookup"><span data-stu-id="14a9b-400">SQL</span></span>

* <span data-ttu-id="14a9b-401">Ajout du paramètre `--ignore-missing-vnet-service-endpoint` pour `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="14a9b-401">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="14a9b-402">Stockage</span><span class="sxs-lookup"><span data-stu-id="14a9b-402">Storage</span></span>

* <span data-ttu-id="14a9b-403">Modification de `storage account create` pour utiliser la référence SKU `Standard_RAGRS` par défaut</span><span class="sxs-lookup"><span data-stu-id="14a9b-403">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="14a9b-404">Correction du bogue lors du traitement des noms d’objets blob/de fichier qui incluent des caractères non-ascii</span><span class="sxs-lookup"><span data-stu-id="14a9b-404">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="14a9b-405">Correction du bogue qui empêchait l’utilisation de `--source-uri` avec `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="14a9b-405">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="14a9b-406">Ajout de commandes pour paramétrer et supprimer plusieurs objets avec `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="14a9b-406">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="14a9b-407">Résolution du problème de l’activation des métriques avec `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="14a9b-407">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="14a9b-408">Résolution du problème des fichiers de plus de 200 Go lors de l’utilisation de `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="14a9b-408">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="14a9b-409">Résolution du problème où `--bypass` et `--default-action` étaient ignorés par `storage account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="14a9b-409">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="14a9b-410">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14a9b-410">VM</span></span>

* <span data-ttu-id="14a9b-411">Correction d’un bogue avec `vmss create` qui empêchait l’utilisation du niveau de taille `Basic`</span><span class="sxs-lookup"><span data-stu-id="14a9b-411">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="14a9b-412">Ajout d’arguments `--plan` à `[vm|vmss] create` pour les images personnalisées avec des informations de facturation</span><span class="sxs-lookup"><span data-stu-id="14a9b-412">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="14a9b-413">Ajout des commandes `vm secret `[add|remove|list]</span><span class="sxs-lookup"><span data-stu-id="14a9b-413">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="14a9b-414">Renommage de `vm format-secret` en `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="14a9b-414">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="14a9b-415">Ajout de l’argument `--encrypt format` à `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="14a9b-415">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="14a9b-416">24 octobre 2017</span><span class="sxs-lookup"><span data-stu-id="14a9b-416">October 24, 2017</span></span>

<span data-ttu-id="14a9b-417">Version 2.0.20</span><span class="sxs-lookup"><span data-stu-id="14a9b-417">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="14a9b-418">Principal</span><span class="sxs-lookup"><span data-stu-id="14a9b-418">Core</span></span>

* <span data-ttu-id="14a9b-419">Mise à jour de `2017-03-09-profile` pour consommer l’API `MGMT_STORAGE` version `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="14a9b-419">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="14a9b-420">ACR</span><span class="sxs-lookup"><span data-stu-id="14a9b-420">ACR</span></span>

* <span data-ttu-id="14a9b-421">Mise à jour de la gestion des ressources pour pointer vers la version d’API `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="14a9b-421">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="14a9b-422">Modification de la référence SKU « Bring Your Own Storage » en Classique</span><span class="sxs-lookup"><span data-stu-id="14a9b-422">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="14a9b-423">Changement des noms des références SKU de registre en De base, Standard, et Premium</span><span class="sxs-lookup"><span data-stu-id="14a9b-423">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="14a9b-424">ACS</span><span class="sxs-lookup"><span data-stu-id="14a9b-424">ACS</span></span>

* <span data-ttu-id="14a9b-425">[PRÉVERSION] Ajout des commandes `az aks`</span><span class="sxs-lookup"><span data-stu-id="14a9b-425">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="14a9b-426">Réparation de Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="14a9b-426">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="14a9b-427">AppService</span><span class="sxs-lookup"><span data-stu-id="14a9b-427">Appservice</span></span>

* <span data-ttu-id="14a9b-428">Résolution d’une erreur où le téléchargement des journaux `webapp` était incorrect</span><span class="sxs-lookup"><span data-stu-id="14a9b-428">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="14a9b-429">Composant</span><span class="sxs-lookup"><span data-stu-id="14a9b-429">Component</span></span>

* <span data-ttu-id="14a9b-430">Ajout de clarté dans les messages visant à déconseiller de tous les programmes d’installation et des invites de confirmation</span><span class="sxs-lookup"><span data-stu-id="14a9b-430">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="14a9b-431">Surveiller</span><span class="sxs-lookup"><span data-stu-id="14a9b-431">Monitor</span></span>

* <span data-ttu-id="14a9b-432">Ajout des commandes `action-group`</span><span class="sxs-lookup"><span data-stu-id="14a9b-432">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="14a9b-433">Ressource</span><span class="sxs-lookup"><span data-stu-id="14a9b-433">Resource</span></span>

* <span data-ttu-id="14a9b-434">Résolution d’une incompatibilité de la dépendance msrest dans `group export` avec les versions les plus récentes</span><span class="sxs-lookup"><span data-stu-id="14a9b-434">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="14a9b-435">Résolution de `policy assignment create` pour qu’il fonctionne avec les définitions de stratégie et les définitions d’ensemble de stratégie intégrées</span><span class="sxs-lookup"><span data-stu-id="14a9b-435">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="14a9b-436">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14a9b-436">VM</span></span>

* <span data-ttu-id="14a9b-437">Ajout de l’argument `--accelerated-networking` à `vmss create`</span><span class="sxs-lookup"><span data-stu-id="14a9b-437">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="14a9b-438">9 octobre 2017</span><span class="sxs-lookup"><span data-stu-id="14a9b-438">October 9, 2017</span></span>

<span data-ttu-id="14a9b-439">Version 2.0.19</span><span class="sxs-lookup"><span data-stu-id="14a9b-439">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="14a9b-440">Principal</span><span class="sxs-lookup"><span data-stu-id="14a9b-440">Core</span></span>

* <span data-ttu-id="14a9b-441">Ajout de la gestion des URL d’autorisation AD FS avec une barre oblique à Azure Stack</span><span class="sxs-lookup"><span data-stu-id="14a9b-441">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="14a9b-442">AppService</span><span class="sxs-lookup"><span data-stu-id="14a9b-442">Appservice</span></span>

* <span data-ttu-id="14a9b-443">Ajout de la mise à jour générique avec la nouvelle commande `webapp update`</span><span class="sxs-lookup"><span data-stu-id="14a9b-443">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="14a9b-444">Batch</span><span class="sxs-lookup"><span data-stu-id="14a9b-444">Batch</span></span>

* <span data-ttu-id="14a9b-445">Mis à jour du kit de développement logiciel (SDK) à la version 4.0.0</span><span class="sxs-lookup"><span data-stu-id="14a9b-445">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="14a9b-446">Mise à jour de l’option `--image` de VirtualMachineConfiguration pour prendre en charge les références d’image ARM en plus de publish:offre:sku:version</span><span class="sxs-lookup"><span data-stu-id="14a9b-446">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="14a9b-447">Ajout de la prise en charge du nouveau modèle d’extension CLI pour les commandes d’extension Batch</span><span class="sxs-lookup"><span data-stu-id="14a9b-447">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="14a9b-448">Suppression de la prise en charge Batch des modèles de composants</span><span class="sxs-lookup"><span data-stu-id="14a9b-448">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="14a9b-449">Batchai</span><span class="sxs-lookup"><span data-stu-id="14a9b-449">Batchai</span></span>

* <span data-ttu-id="14a9b-450">Version initiale du module Batch AI</span><span class="sxs-lookup"><span data-stu-id="14a9b-450">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="14a9b-451">KeyVault</span><span class="sxs-lookup"><span data-stu-id="14a9b-451">Keyvault</span></span>

* <span data-ttu-id="14a9b-452">Résolution du problème d’authentification Key Vault lors de l’utilisation d’AD FS sur Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="14a9b-452">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="14a9b-453">(#4448)</span><span class="sxs-lookup"><span data-stu-id="14a9b-453">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="14a9b-454">Réseau</span><span class="sxs-lookup"><span data-stu-id="14a9b-454">Network</span></span>

* <span data-ttu-id="14a9b-455">La modification de l’argument `--server` de `application-gateway address-pool create` devient facultative, permettant les pools d’adresses vides</span><span class="sxs-lookup"><span data-stu-id="14a9b-455">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="14a9b-456">Mise à jour de `traffic-manager` pour prendre en charge les fonctionnalités les plus récentes</span><span class="sxs-lookup"><span data-stu-id="14a9b-456">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="14a9b-457">Ressource</span><span class="sxs-lookup"><span data-stu-id="14a9b-457">Resource</span></span>

* <span data-ttu-id="14a9b-458">Ajout de la prise en charge des options `--resource-group/-g` pour le nom du groupe de ressources dans `group`</span><span class="sxs-lookup"><span data-stu-id="14a9b-458">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="14a9b-459">Ajout des commandes à `account lock` pour travailler avec des verrous au niveau de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="14a9b-459">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="14a9b-460">Ajout des commandes à `group lock` pour travailler avec des verrous au niveau du groupe</span><span class="sxs-lookup"><span data-stu-id="14a9b-460">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="14a9b-461">Ajout des commandes à `resource lock` pour travailler avec des verrous au niveau des ressources</span><span class="sxs-lookup"><span data-stu-id="14a9b-461">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="14a9b-462">SQL</span><span class="sxs-lookup"><span data-stu-id="14a9b-462">Sql</span></span>

* <span data-ttu-id="14a9b-463">Ajout de la prise en charge pour le Chiffrement transparent des données (TDE) SQL et le chiffrement transparent des données avec Bring Your Own Key</span><span class="sxs-lookup"><span data-stu-id="14a9b-463">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="14a9b-464">Ajout de la commande `db list-deleted` et du paramètre `db restore --deleted-time`, ce qui offre la possibilité de rechercher et de restaurer les bases de données supprimées</span><span class="sxs-lookup"><span data-stu-id="14a9b-464">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="14a9b-465">Ajout de `db op list` et `db op cancel`, ce qui offre la capacité de répertorier et d’annuler des opérations en cours sur la base de données</span><span class="sxs-lookup"><span data-stu-id="14a9b-465">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="14a9b-466">Stockage</span><span class="sxs-lookup"><span data-stu-id="14a9b-466">Storage</span></span>

* <span data-ttu-id="14a9b-467">Ajout de la prise en charge d’instantané de partage de fichiers</span><span class="sxs-lookup"><span data-stu-id="14a9b-467">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="14a9b-468">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14a9b-468">Vm</span></span>

* <span data-ttu-id="14a9b-469">Correction d’un bogue dans `vm show` où l’utilisation de `-d` a provoqué un incident dans les adresses IP privées manquantes</span><span class="sxs-lookup"><span data-stu-id="14a9b-469">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="14a9b-470">[VERSION PRÉLIMINAIRE] Ajout de la prise en charge de la mise à niveau propagée pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="14a9b-470">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="14a9b-471">Ajout de la prise en charge de la mise à jour des paramètres de chiffrement avec `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="14a9b-471">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="14a9b-472">Ajout du paramètre `--os-disk-size-gb` pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="14a9b-472">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="14a9b-473">Ajout du paramètre `--license-type` de Windows pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="14a9b-473">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="14a9b-474">22 septembre 2017</span><span class="sxs-lookup"><span data-stu-id="14a9b-474">September 22, 2017</span></span>

<span data-ttu-id="14a9b-475">Version 2.0.18</span><span class="sxs-lookup"><span data-stu-id="14a9b-475">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="14a9b-476">Ressource</span><span class="sxs-lookup"><span data-stu-id="14a9b-476">Resource</span></span>

* <span data-ttu-id="14a9b-477">Ajout de la prise en charge de l’affichage des définitions de stratégie intégrée</span><span class="sxs-lookup"><span data-stu-id="14a9b-477">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="14a9b-478">Ajout de la prise en charge du paramètre de mode pour la création de définitions de stratégie</span><span class="sxs-lookup"><span data-stu-id="14a9b-478">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="14a9b-479">Ajout de la prise en charge des définitions d’interface utilisateur et des modèles pour `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="14a9b-479">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="14a9b-480">[CHANGEMENT RÉCENT] Modification du type de ressource `managedapp` de `appliances` en `applications` et de `applianceDefinitions` en `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="14a9b-480">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="14a9b-481">Réseau</span><span class="sxs-lookup"><span data-stu-id="14a9b-481">Network</span></span>

* <span data-ttu-id="14a9b-482">Ajout de la prise en charge de la zone de disponibilité aux sous-commandes `network lb` et `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="14a9b-482">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="14a9b-483">Ajout de la prise en charge de l’homologation Microsoft IPv6 pour `express-route`</span><span class="sxs-lookup"><span data-stu-id="14a9b-483">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="14a9b-484">Ajout des commandes du groupe de sécurité d’application `asg`</span><span class="sxs-lookup"><span data-stu-id="14a9b-484">Added `asg` application security group commands</span></span>
* <span data-ttu-id="14a9b-485">Ajout de l’argument `--application-security-groups` à `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="14a9b-485">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="14a9b-486">Ajout des arguments `--source-asgs` et `--destination-asgs` à `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="14a9b-486">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="14a9b-487">Ajout des arguments `--ddos-protection` et `--vm-protection` à `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="14a9b-487">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="14a9b-488">Ajout des commandes `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="14a9b-488">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="14a9b-489">Stockage</span><span class="sxs-lookup"><span data-stu-id="14a9b-489">Storage</span></span>

* <span data-ttu-id="14a9b-490">Résolution d’un problème qui pouvait causer l’échec des commandes `storage account network-rule` après la mise à jour du Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="14a9b-490">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="14a9b-491">Événement</span><span class="sxs-lookup"><span data-stu-id="14a9b-491">Eventgrid</span></span>

* <span data-ttu-id="14a9b-492">Mise à jour du Kit de développement logiciel (SDK) Python Azure Event Grid afin d’utiliser une version plus récente de l’API « 2017-09-15-preview »</span><span class="sxs-lookup"><span data-stu-id="14a9b-492">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="14a9b-493">SQL</span><span class="sxs-lookup"><span data-stu-id="14a9b-493">SQL</span></span>

* <span data-ttu-id="14a9b-494">La modification de l’`sql server list`argument`--resource-group` devient facultative.</span><span class="sxs-lookup"><span data-stu-id="14a9b-494">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="14a9b-495">En l’absence de précisions, tous les serveurs SQL dans l’abonnement seront retournés</span><span class="sxs-lookup"><span data-stu-id="14a9b-495">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="14a9b-496">Ajout du paramètre `--no-wait` à `db [create|copy|restore|update|replica create|create|update]` et `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="14a9b-496">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="14a9b-497">KeyVault</span><span class="sxs-lookup"><span data-stu-id="14a9b-497">Keyvault</span></span>

* <span data-ttu-id="14a9b-498">Ajout de la prise en charge des commandes Keyvault derrière un proxy</span><span class="sxs-lookup"><span data-stu-id="14a9b-498">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="14a9b-499">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14a9b-499">VM</span></span>

* <span data-ttu-id="14a9b-500">Ajout de la prise en charge de zone de disponibilité pour `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="14a9b-500">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="14a9b-501">Résolution d’un problème à cause duquel l’utilisation de `--app-gateway ID` avec `vmss create` entraînait un échec</span><span class="sxs-lookup"><span data-stu-id="14a9b-501">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="14a9b-502">Ajout de l’argument `--asgs` à `vm create`</span><span class="sxs-lookup"><span data-stu-id="14a9b-502">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="14a9b-503">Ajout de la prise en charge des commandes en cours d’exécution sur des machines virtuelles avec `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="14a9b-503">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="14a9b-504">[PRÉVERSION] Ajout de la prise en charge du chiffrement de disque VMSS avec `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="14a9b-504">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="14a9b-505">Ajout de la prise en charge de la réalisation de la maintenance sur des machines virtuelles avec `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="14a9b-505">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="14a9b-506">ACS</span><span class="sxs-lookup"><span data-stu-id="14a9b-506">ACS</span></span>

* <span data-ttu-id="14a9b-507">[PRÉVERSION] Ajout de l’argument `--orchestrator-release` à `acs create` pour les régions ACS en préversion</span><span class="sxs-lookup"><span data-stu-id="14a9b-507">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="14a9b-508">AppService</span><span class="sxs-lookup"><span data-stu-id="14a9b-508">Appservice</span></span>

* <span data-ttu-id="14a9b-509">Ajout de la capacité à mettre à jour et à afficher les paramètres d’authentification avec `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="14a9b-509">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="14a9b-510">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="14a9b-510">Backup</span></span>

* <span data-ttu-id="14a9b-511">Version préliminaire</span><span class="sxs-lookup"><span data-stu-id="14a9b-511">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="14a9b-512">11 septembre 2017</span><span class="sxs-lookup"><span data-stu-id="14a9b-512">September 11, 2017</span></span>

<span data-ttu-id="14a9b-513">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="14a9b-513">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="14a9b-514">Principal</span><span class="sxs-lookup"><span data-stu-id="14a9b-514">Core</span></span>

* <span data-ttu-id="14a9b-515">Module de commande activé pour définir son propre ID de corrélation dans la télémétrie</span><span class="sxs-lookup"><span data-stu-id="14a9b-515">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="14a9b-516">Résolution du problème de vidage JSON lorsque la télémétrie est définie en mode diagnostics</span><span class="sxs-lookup"><span data-stu-id="14a9b-516">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="14a9b-517">Acs</span><span class="sxs-lookup"><span data-stu-id="14a9b-517">Acs</span></span>

* <span data-ttu-id="14a9b-518">Ajout de la commande `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="14a9b-518">Added `acs list-locations` command</span></span>
* <span data-ttu-id="14a9b-519">Faire en sorte que `ssh-key-file` soit fourni avec la valeur par défaut attendu</span><span class="sxs-lookup"><span data-stu-id="14a9b-519">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="14a9b-520">AppService</span><span class="sxs-lookup"><span data-stu-id="14a9b-520">Appservice</span></span>

* <span data-ttu-id="14a9b-521">Ajout de la possibilité de créer une application web dans un groupe de ressources autre que celui du plan de service actif</span><span class="sxs-lookup"><span data-stu-id="14a9b-521">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="14a9b-522">CDN</span><span class="sxs-lookup"><span data-stu-id="14a9b-522">CDN</span></span>

* <span data-ttu-id="14a9b-523">Correction du bogue « CustomDomain n’est pas itérable » pour `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="14a9b-523">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`.</span></span>

### <a name="extension"></a><span data-ttu-id="14a9b-524">Extension</span><span class="sxs-lookup"><span data-stu-id="14a9b-524">Extension</span></span>

* <span data-ttu-id="14a9b-525">Version initiale.</span><span class="sxs-lookup"><span data-stu-id="14a9b-525">Initial Release.</span></span>

### <a name="keyvault"></a><span data-ttu-id="14a9b-526">KeyVault</span><span class="sxs-lookup"><span data-stu-id="14a9b-526">Keyvault</span></span>

* <span data-ttu-id="14a9b-527">Résolution du problème, où les autorisations étaient sensibles à la casse pour `keyvault set-policy`.</span><span class="sxs-lookup"><span data-stu-id="14a9b-527">Fixed issue where permissions were case sensitive for `keyvault set-policy`.</span></span>

### <a name="network"></a><span data-ttu-id="14a9b-528">Réseau</span><span class="sxs-lookup"><span data-stu-id="14a9b-528">Network</span></span>

* <span data-ttu-id="14a9b-529">Renommage de `vnet list-private-access-services` en `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="14a9b-529">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="14a9b-530">Argument `--private-access-services` renommé en `--service-endpoints` pour`vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="14a9b-530">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="14a9b-531">Ajout de la prise en charge de plusieurs plages IP et de ports à `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="14a9b-531">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="14a9b-532">Ajout de la prise en charge de la référence (SKU) pour `lb create`</span><span class="sxs-lookup"><span data-stu-id="14a9b-532">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="14a9b-533">Ajout de la prise en charge de la référence (SKU) pour `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="14a9b-533">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="14a9b-534">Ressource</span><span class="sxs-lookup"><span data-stu-id="14a9b-534">Resource</span></span>

* <span data-ttu-id="14a9b-535">Autoriser le passages dans les définitions de paramètres de stratégie de ressource dans `policy definition create`, et`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="14a9b-535">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="14a9b-536">Autoriser le passage dans les valeurs de paramètres pour `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="14a9b-536">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="14a9b-537">Autoriser le passage de JSON ou d’un fichier pour tous les paramètres</span><span class="sxs-lookup"><span data-stu-id="14a9b-537">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="14a9b-538">Incrémentation de la version de l’API</span><span class="sxs-lookup"><span data-stu-id="14a9b-538">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="14a9b-539">SQL</span><span class="sxs-lookup"><span data-stu-id="14a9b-539">SQL</span></span>

* <span data-ttu-id="14a9b-540">Ajout des commandes `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="14a9b-540">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="14a9b-541">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14a9b-541">VM</span></span>

* <span data-ttu-id="14a9b-542">Résolu : n’affecte aucun accès tant que `--scope` n’est pas indiqué</span><span class="sxs-lookup"><span data-stu-id="14a9b-542">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="14a9b-543">Résolu : utilisation de la même dénomination d’extension que celle du portail</span><span class="sxs-lookup"><span data-stu-id="14a9b-543">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="14a9b-544">Suppression de `subscription` de la sortie `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="14a9b-544">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="14a9b-545">Résolu : la référence SKU de stockage `[vm|vmss] create` n’est pas appliquée sur les disques de données avec une image</span><span class="sxs-lookup"><span data-stu-id="14a9b-545">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="14a9b-546">Résolu : `vm format-secret --secrets` n’accepte pas d’ID séparés par un saut de ligne</span><span class="sxs-lookup"><span data-stu-id="14a9b-546">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="14a9b-547">31 août 2017</span><span class="sxs-lookup"><span data-stu-id="14a9b-547">August 31, 2017</span></span>

<span data-ttu-id="14a9b-548">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="14a9b-548">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="14a9b-549">KeyVault</span><span class="sxs-lookup"><span data-stu-id="14a9b-549">Keyvault</span></span>

* <span data-ttu-id="14a9b-550">Correction d’un bogue à cause duquel vous tentez de résoudre automatiquement l’encodage secret avec `secret download`</span><span class="sxs-lookup"><span data-stu-id="14a9b-550">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="14a9b-551">Sf</span><span class="sxs-lookup"><span data-stu-id="14a9b-551">Sf</span></span>

* <span data-ttu-id="14a9b-552">Déconseiller toutes les commandes en faveur de Service Fabric CLI (sfctl)</span><span class="sxs-lookup"><span data-stu-id="14a9b-552">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="14a9b-553">Stockage</span><span class="sxs-lookup"><span data-stu-id="14a9b-553">Storage</span></span>

* <span data-ttu-id="14a9b-554">Résolution du problème dans lequel la création de comptes de stockage dans les régions ne prenant pas en charge la fonctionnalité NetworkACLs était impossible</span><span class="sxs-lookup"><span data-stu-id="14a9b-554">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="14a9b-555">Déterminer le type de contenu et l’encodage du contenu lors du chargement d’objets blob et de fichiers si aucun type de contenu et d’encodage n’est spécifié.</span><span class="sxs-lookup"><span data-stu-id="14a9b-555">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="14a9b-556">28 août 2017</span><span class="sxs-lookup"><span data-stu-id="14a9b-556">August 28, 2017</span></span>

<span data-ttu-id="14a9b-557">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="14a9b-557">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="14a9b-558">Interface de ligne de commande</span><span class="sxs-lookup"><span data-stu-id="14a9b-558">CLI</span></span>

* <span data-ttu-id="14a9b-559">Ajout d’une remarque juridique pour `--version`.</span><span class="sxs-lookup"><span data-stu-id="14a9b-559">Added legal note to `--version`.</span></span>

### <a name="acs"></a><span data-ttu-id="14a9b-560">ACS</span><span class="sxs-lookup"><span data-stu-id="14a9b-560">ACS</span></span>

* <span data-ttu-id="14a9b-561">Correction des régions d’aperçu.</span><span class="sxs-lookup"><span data-stu-id="14a9b-561">Corrected preview regions.</span></span>
* <span data-ttu-id="14a9b-562">Mise en forme par défaut `dns_name_prefix` correctement.</span><span class="sxs-lookup"><span data-stu-id="14a9b-562">Formatted default `dns_name_prefix` properly.</span></span>
* <span data-ttu-id="14a9b-563">Sortie de commande des services ACS optimisée.</span><span class="sxs-lookup"><span data-stu-id="14a9b-563">Optimized acs command output.</span></span>

### <a name="appservice"></a><span data-ttu-id="14a9b-564">AppService</span><span class="sxs-lookup"><span data-stu-id="14a9b-564">Appservice</span></span>

* <span data-ttu-id="14a9b-565">[MODIFICATION CRITIQUE] Fixation des incohérences dans la sortie de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="14a9b-565">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="14a9b-566">Ajout d’un nouvel alias de `-i` pour `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="14a9b-566">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="14a9b-567">Exposé `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="14a9b-567">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="14a9b-568">Exposition de nouveaux arguments à partir de `az webapp delete` pour conserver le plan de service d'application, les métriques ou l’inscription DNS</span><span class="sxs-lookup"><span data-stu-id="14a9b-568">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="14a9b-569">Problème résolu : Détecter les paramètres d’emplacement correctement</span><span class="sxs-lookup"><span data-stu-id="14a9b-569">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="14a9b-570">IoT</span><span class="sxs-lookup"><span data-stu-id="14a9b-570">IoT</span></span>

* <span data-ttu-id="14a9b-571">Résolu #3934 : La création de la stratégie n’efface plus les stratégies existantes</span><span class="sxs-lookup"><span data-stu-id="14a9b-571">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="14a9b-572">Réseau</span><span class="sxs-lookup"><span data-stu-id="14a9b-572">Network</span></span>

* <span data-ttu-id="14a9b-573">[MODIFICATION CRITIQUE] Renommage `vnet list-private-access-services` à `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="14a9b-573">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="14a9b-574">[MODIFICATION CRITIQUE] Renommage de l’option `--private-access-services` en `--service-endpoints` pour `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="14a9b-574">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="14a9b-575">Ajout de la prise en charge de plusieurs IP et de plusieurs pages de port pour `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="14a9b-575">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="14a9b-576">Ajout de la prise en charge de la référence (SKU) pour `lb create`</span><span class="sxs-lookup"><span data-stu-id="14a9b-576">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="14a9b-577">Ajout de la prise en charge de la référence (SKU) pour `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="14a9b-577">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="14a9b-578">Profil</span><span class="sxs-lookup"><span data-stu-id="14a9b-578">Profile</span></span>

* <span data-ttu-id="14a9b-579">exposés `--msi` et `--msi-port` pour vous connecter à l’aide d’une identité de machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14a9b-579">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="14a9b-580">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="14a9b-580">Service Fabric</span></span>

* <span data-ttu-id="14a9b-581">Version préliminaire</span><span class="sxs-lookup"><span data-stu-id="14a9b-581">Preview release</span></span>
* <span data-ttu-id="14a9b-582">Règles d’utilisateur du Registre/de mot de passe simplifiées pour la commande</span><span class="sxs-lookup"><span data-stu-id="14a9b-582">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="14a9b-583">Invite de mot de passe fixe pour l’utilisateur, même après le passage de paramètre</span><span class="sxs-lookup"><span data-stu-id="14a9b-583">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="14a9b-584">Ajout de la prise en charge de vide `registry_cred`</span><span class="sxs-lookup"><span data-stu-id="14a9b-584">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="14a9b-585">Stockage</span><span class="sxs-lookup"><span data-stu-id="14a9b-585">Storage</span></span>

* <span data-ttu-id="14a9b-586">Paramétrage du niveau blob activé</span><span class="sxs-lookup"><span data-stu-id="14a9b-586">Enabled setting blob tier</span></span>
* <span data-ttu-id="14a9b-587">Ajout des arguments `--bypass` et `--default-action` à `storage account [create|update]` pour la prise en charge du tunneling de service</span><span class="sxs-lookup"><span data-stu-id="14a9b-587">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="14a9b-588">Ajout de commandes permettant d’ajouter des règles de réseau virtuel et des règles basées sur IP à `storage account network-rule`</span><span class="sxs-lookup"><span data-stu-id="14a9b-588">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="14a9b-589">Activation du chiffrement du service par la clé gérée du client</span><span class="sxs-lookup"><span data-stu-id="14a9b-589">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="14a9b-590">[MODIFICATION CRITIQUE] Renommage de l’option `--encryption` en `--encryption-services` pour `az storage account create and az storage account update` la commande</span><span class="sxs-lookup"><span data-stu-id="14a9b-590">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="14a9b-591">Problème résolu #4220 : `az storage account update encryption` - incompatibilité de syntaxe</span><span class="sxs-lookup"><span data-stu-id="14a9b-591">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="14a9b-592">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14a9b-592">VM</span></span>

* <span data-ttu-id="14a9b-593">Correction d’un problème qui entraînait l’affichage d’informations supplémentaires erronées pour `vmss get-instance-view` lors de l’utilisation `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="14a9b-593">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="14a9b-594">Ajout de la prise en charge de `--lb-sku` pour `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="14a9b-594">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="14a9b-595">Suppression des noms humains de la liste rouge du nom de l’administrateur pour `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="14a9b-595">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="14a9b-596">Correction d’un problème qui entraînait `[vm|vmss] create` la levée d’une erreur si la commande ne parvenait pas à extraire des informations de plan à partir d’une image</span><span class="sxs-lookup"><span data-stu-id="14a9b-596">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="14a9b-597">Correction d’un incident qui se produisait lors de la création d’un groupe identique VMMD avec un équilibrage de charge (LB) interne</span><span class="sxs-lookup"><span data-stu-id="14a9b-597">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="14a9b-598">Correction d’un problème qui empêchait `--no-wait` le fonctionnement d’un argument avec `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="14a9b-598">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="14a9b-599">15 août 2017</span><span class="sxs-lookup"><span data-stu-id="14a9b-599">August 15, 2017</span></span>

<span data-ttu-id="14a9b-600">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="14a9b-600">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="14a9b-601">ACS</span><span class="sxs-lookup"><span data-stu-id="14a9b-601">ACS</span></span>

* <span data-ttu-id="14a9b-602">Correction du numéro de port sshMaster0 pour kubernetes</span><span class="sxs-lookup"><span data-stu-id="14a9b-602">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="14a9b-603">AppService</span><span class="sxs-lookup"><span data-stu-id="14a9b-603">Appservice</span></span>

* <span data-ttu-id="14a9b-604">Correction d’une exception qui se produisait lors de la création d’une nouvelle application web Linux basée sur git</span><span class="sxs-lookup"><span data-stu-id="14a9b-604">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="14a9b-605">Event Grid</span><span class="sxs-lookup"><span data-stu-id="14a9b-605">Event Grid</span></span>

* <span data-ttu-id="14a9b-606">Ajout de dépendances du kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="14a9b-606">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="14a9b-607">11 août 2017</span><span class="sxs-lookup"><span data-stu-id="14a9b-607">August 11, 2017</span></span>

<span data-ttu-id="14a9b-608">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="14a9b-608">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="14a9b-609">ACS</span><span class="sxs-lookup"><span data-stu-id="14a9b-609">ACS</span></span>

* <span data-ttu-id="14a9b-610">Ajout de nouvelles régions d’aperçu</span><span class="sxs-lookup"><span data-stu-id="14a9b-610">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="14a9b-611">Batch</span><span class="sxs-lookup"><span data-stu-id="14a9b-611">Batch</span></span>

* <span data-ttu-id="14a9b-612">Mise à jour vers Kit de développement logiciel (DSK) de lot 3.1.0 et Kit de développement logiciel (SDK) de gestion de lot 4.1.0</span><span class="sxs-lookup"><span data-stu-id="14a9b-612">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="14a9b-613">Ajout d'une nouvelle commande affichant le nombre de tâches d’un travail</span><span class="sxs-lookup"><span data-stu-id="14a9b-613">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="14a9b-614">Correction du bogue dans le traitement de l’URL de la signature d'accès partagé du fichier de ressources</span><span class="sxs-lookup"><span data-stu-id="14a9b-614">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="14a9b-615">Point de terminaison de compte Batch prend désormais en charge le préfixe « https:// » facultatif</span><span class="sxs-lookup"><span data-stu-id="14a9b-615">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="14a9b-616">Prise en charge de l’ajout des listes de plus de 100 tâches à un travail</span><span class="sxs-lookup"><span data-stu-id="14a9b-616">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="14a9b-617">Ajout de l’enregistrement de débogage pour le chargement du module de commande Extensions</span><span class="sxs-lookup"><span data-stu-id="14a9b-617">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="14a9b-618">Composant</span><span class="sxs-lookup"><span data-stu-id="14a9b-618">Component</span></span>

* <span data-ttu-id="14a9b-619">Ajout d’un avertissement de désapprobation aux commandes « az component »</span><span class="sxs-lookup"><span data-stu-id="14a9b-619">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="14a9b-620">Conteneur</span><span class="sxs-lookup"><span data-stu-id="14a9b-620">Container</span></span>

* <span data-ttu-id="14a9b-621">`create` : correction d’un problème qui empêchait l’autorisation de signe égal à l’intérieur d’une variable d’environnement</span><span class="sxs-lookup"><span data-stu-id="14a9b-621">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="14a9b-622">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="14a9b-622">Data Lake Store</span></span>

* <span data-ttu-id="14a9b-623">Contrôle de progression activé</span><span class="sxs-lookup"><span data-stu-id="14a9b-623">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="14a9b-624">Event Grid</span><span class="sxs-lookup"><span data-stu-id="14a9b-624">Event Grid</span></span>

* <span data-ttu-id="14a9b-625">Version initiale</span><span class="sxs-lookup"><span data-stu-id="14a9b-625">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="14a9b-626">Réseau</span><span class="sxs-lookup"><span data-stu-id="14a9b-626">Network</span></span>

* <span data-ttu-id="14a9b-627">`lb` : correction d’un problème qui empêchait certains noms de ressources enfant d’être résolus correctement lorsqu’ils étaient omis</span><span class="sxs-lookup"><span data-stu-id="14a9b-627">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="14a9b-628">`application-gateway {subresource} delete` : correction d’un problème en raison duquel `--no-wait` n’était pas honorée</span><span class="sxs-lookup"><span data-stu-id="14a9b-628">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="14a9b-629">`application-gateway http-settings update` : correction d’un problème `--connection-draining-timeout` qui empêchait la désactivation de</span><span class="sxs-lookup"><span data-stu-id="14a9b-629">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="14a9b-630">Correction de erreur argument du mot-clé inattendu `sa_data_size_kilobyes` avec`az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="14a9b-630">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="14a9b-631">Profil</span><span class="sxs-lookup"><span data-stu-id="14a9b-631">Profile</span></span>

* <span data-ttu-id="14a9b-632">`account list` : ajout de `--refresh` pour synchroniser les derniers abonnements à partir du serveur</span><span class="sxs-lookup"><span data-stu-id="14a9b-632">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="14a9b-633">Stockage</span><span class="sxs-lookup"><span data-stu-id="14a9b-633">Storage</span></span>

* <span data-ttu-id="14a9b-634">Activer le compte de stockage de mise à jour avec l’identité attribuée par le système</span><span class="sxs-lookup"><span data-stu-id="14a9b-634">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="14a9b-635">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14a9b-635">VM</span></span>

* <span data-ttu-id="14a9b-636">`availability-set` : nombre de domaines d’erreur exposé sur convert</span><span class="sxs-lookup"><span data-stu-id="14a9b-636">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="14a9b-637">Commande `list-skus` exposée</span><span class="sxs-lookup"><span data-stu-id="14a9b-637">Exposed `list-skus` command</span></span>
* <span data-ttu-id="14a9b-638">Prise en charge pour affecter l’identité avec ou sans création d’attributions de rôle</span><span class="sxs-lookup"><span data-stu-id="14a9b-638">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="14a9b-639">Appliquer la référence (SKU) de stockage lors de l’attachement de disques de données</span><span class="sxs-lookup"><span data-stu-id="14a9b-639">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="14a9b-640">Suppression du nom du disque du système d’exploitation par défaut et de la référence (SKU) de stockage lors de l’utilisation des disques gérés</span><span class="sxs-lookup"><span data-stu-id="14a9b-640">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="14a9b-641">28 juillet 2017</span><span class="sxs-lookup"><span data-stu-id="14a9b-641">July 28, 2017</span></span>

<span data-ttu-id="14a9b-642">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="14a9b-642">Version 2.0.12</span></span>

* <span data-ttu-id="14a9b-643">Ajout de commandes de conteneur</span><span class="sxs-lookup"><span data-stu-id="14a9b-643">Added container commands</span></span>
* <span data-ttu-id="14a9b-644">Ajout de modules de facturation et de consommation</span><span class="sxs-lookup"><span data-stu-id="14a9b-644">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="14a9b-645">Principal</span><span class="sxs-lookup"><span data-stu-id="14a9b-645">Core</span></span>

* <span data-ttu-id="14a9b-646">Informations d’authentification du Kit de développement logiciel (SDK) de sortie pour les principaux de service avec des certificats</span><span class="sxs-lookup"><span data-stu-id="14a9b-646">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="14a9b-647">Correction des exceptions de progression de déploiement</span><span class="sxs-lookup"><span data-stu-id="14a9b-647">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="14a9b-648">Utiliser le point de terminaison ARM à partir du cloud actuel pour créer le client de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="14a9b-648">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="14a9b-649">Amélioration de la gestion simultanée de fichiers clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="14a9b-649">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="14a9b-650">Actualiser l’ID de la demande client pour chaque exécution de la commande</span><span class="sxs-lookup"><span data-stu-id="14a9b-650">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="14a9b-651">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel ( SDK) (#3635)</span><span class="sxs-lookup"><span data-stu-id="14a9b-651">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="14a9b-652">Rapports de progression pour les déploiements de modèle (#3510)</span><span class="sxs-lookup"><span data-stu-id="14a9b-652">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="14a9b-653">Ajout de la prise en charge des champs de sortie de la table de prélèvement via la requête jmespath (#3581)</span><span class="sxs-lookup"><span data-stu-id="14a9b-653">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="14a9b-654">Amélioration de la désactivation des arguments d’analyse et de l’historique Ajout avec des mouvements (#3434)</span><span class="sxs-lookup"><span data-stu-id="14a9b-654">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="14a9b-655">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="14a9b-655">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="14a9b-656">Déplacer tous les fichiers d’enregistrement existant vers le dernier dossier</span><span class="sxs-lookup"><span data-stu-id="14a9b-656">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="14a9b-657">Correction de l’idempotence pour VM/VMSS create (#3586)</span><span class="sxs-lookup"><span data-stu-id="14a9b-657">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="14a9b-658">Les chemins d’accès de la commande ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="14a9b-658">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="14a9b-659">Certains paramètres de type booléen ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="14a9b-659">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="14a9b-660">Prise en charge de la connexion à ADFS sur le serveur local de manière identique à Azure Stack</span><span class="sxs-lookup"><span data-stu-id="14a9b-660">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="14a9b-661">Correction des écritures simultanées dans clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="14a9b-661">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="14a9b-662">ACR</span><span class="sxs-lookup"><span data-stu-id="14a9b-662">ACR</span></span>

* <span data-ttu-id="14a9b-663">Ajout de la commande `show-usage` pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="14a9b-663">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="14a9b-664">Prise en charge de la mise à jour de la référence (SKU) pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="14a9b-664">Support SKU update for managed registries</span></span>
* <span data-ttu-id="14a9b-665">Ajout de registres gérés avec la référence (SKU) gérée</span><span class="sxs-lookup"><span data-stu-id="14a9b-665">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="14a9b-666">Ajout de webhooks pour les registres gérés avec le module de commande acr webhook</span><span class="sxs-lookup"><span data-stu-id="14a9b-666">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="14a9b-667">Ajout de l’authentification AAD avec la commande de connexion acr</span><span class="sxs-lookup"><span data-stu-id="14a9b-667">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="14a9b-668">Ajout de la commande de suppression pour les référentiels docker, les manifestes et les balises</span><span class="sxs-lookup"><span data-stu-id="14a9b-668">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="14a9b-669">ACS</span><span class="sxs-lookup"><span data-stu-id="14a9b-669">ACS</span></span>

* <span data-ttu-id="14a9b-670">Prise en charge des API version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="14a9b-670">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="14a9b-671">AppService</span><span class="sxs-lookup"><span data-stu-id="14a9b-671">Appservice</span></span>

* <span data-ttu-id="14a9b-672">Correction d’un bogue à cause duquel l’énumération d’une application Linux ne retournait absolument rien</span><span class="sxs-lookup"><span data-stu-id="14a9b-672">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="14a9b-673">Prise en charge de la récupération de références depuis ACR</span><span class="sxs-lookup"><span data-stu-id="14a9b-673">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="14a9b-674">Supprimer toutes les commandes sous `appservice web`</span><span class="sxs-lookup"><span data-stu-id="14a9b-674">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="14a9b-675">Masquer les mots de passe du registre docker de la commande de sortie (#3656)</span><span class="sxs-lookup"><span data-stu-id="14a9b-675">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="14a9b-676">Vérifier que le navigateur par défaut est utilisé sur macOs sans erreurs (#3623)</span><span class="sxs-lookup"><span data-stu-id="14a9b-676">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="14a9b-677">Améliorer l’aide de `webapp log tail` et `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="14a9b-677">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="14a9b-678">Commandes `traffic-routing` exposées pour configurer le routage statique (#3566)</span><span class="sxs-lookup"><span data-stu-id="14a9b-678">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="14a9b-679">Ajout de correctifs de fiabilité pour la configuration du contrôle de code source (#3245)</span><span class="sxs-lookup"><span data-stu-id="14a9b-679">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="14a9b-680">Suppression d’un argument non pris en charge `--node-version` de `webapp config update` pour les applications Web de Windows.</span><span class="sxs-lookup"><span data-stu-id="14a9b-680">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="14a9b-681">Utilisez à la place `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="14a9b-681">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="14a9b-682">Batch</span><span class="sxs-lookup"><span data-stu-id="14a9b-682">Batch</span></span>

* <span data-ttu-id="14a9b-683">Mise à jour vers kit de développement logiciel (SDK) de lot 3.0.0 avec prise en charge pour les machines virtuelles de faible priorité dans des pools</span><span class="sxs-lookup"><span data-stu-id="14a9b-683">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="14a9b-684">Renommage `pool create` option `--target-dedicated` en `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="14a9b-684">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="14a9b-685">Ajout des options `pool create`, `--target-low-priority-nodes` et `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="14a9b-685">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="14a9b-686">CDN</span><span class="sxs-lookup"><span data-stu-id="14a9b-686">CDN</span></span>

* <span data-ttu-id="14a9b-687">Fourni un meilleur message d’erreur pour `cdn endpoint list` quand le profil spécifié par `--profile-name` n’existe pas.</span><span class="sxs-lookup"><span data-stu-id="14a9b-687">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist.</span></span>

### <a name="cloud"></a><span data-ttu-id="14a9b-688">Cloud</span><span class="sxs-lookup"><span data-stu-id="14a9b-688">Cloud</span></span>

* <span data-ttu-id="14a9b-689">Modification de la version de l’API du point de terminaison de métadonnées du cloud au format AAAA-MM-JJ</span><span class="sxs-lookup"><span data-stu-id="14a9b-689">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="14a9b-690">Le point de terminaison de la galerie n’est pas nécessaire</span><span class="sxs-lookup"><span data-stu-id="14a9b-690">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="14a9b-691">Prise en charge de l’inscription du cloud, avec le point de terminaison ARM resource manager</span><span class="sxs-lookup"><span data-stu-id="14a9b-691">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="14a9b-692">Ajout d’une option pour `cloud set` permettant de choisir le profil lors de la sélection du cloud actuel</span><span class="sxs-lookup"><span data-stu-id="14a9b-692">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="14a9b-693">Exposé `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="14a9b-693">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="14a9b-694">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="14a9b-694">CosmosDB</span></span>

* <span data-ttu-id="14a9b-695">Correction relative à la permission de la création de collection avec une clé de partition personnalisée</span><span class="sxs-lookup"><span data-stu-id="14a9b-695">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="14a9b-696">Ajout de la prise en charge de la durée de vie par défaut de la collection.</span><span class="sxs-lookup"><span data-stu-id="14a9b-696">Added support for collection default TTL.</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="14a9b-697">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="14a9b-697">Data Lake Analytics</span></span>

* <span data-ttu-id="14a9b-698">Ajout de commandes pour la gestion de la stratégie de calcul sous le titre `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="14a9b-698">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="14a9b-699">Ajout de `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="14a9b-699">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="14a9b-700">Ajout de `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="14a9b-700">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="14a9b-701">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="14a9b-701">Data Lake Store</span></span>

* <span data-ttu-id="14a9b-702">Ajout de la prise en charge pour la rotation de coffre de clés gérés par l’utilisateur dans `dls account update`</span><span class="sxs-lookup"><span data-stu-id="14a9b-702">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="14a9b-703">Mise à jour de la version du kit de développement logiciel (SDK) du système de fichiers Data Lake Store sous-jacente, réglant un problème de performance</span><span class="sxs-lookup"><span data-stu-id="14a9b-703">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="14a9b-704">Ajout de la commande `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="14a9b-704">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="14a9b-705">Cette commande tente d’activer un utilisateur de coffre de clés fourni par l’utilisateur pour utiliser le chiffrement des données dans un compte Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="14a9b-705">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="14a9b-706">Interactive</span><span class="sxs-lookup"><span data-stu-id="14a9b-706">Interactive</span></span>

* <span data-ttu-id="14a9b-707">Amélioration du temps de démarrage à l’aide des commandes en cache</span><span class="sxs-lookup"><span data-stu-id="14a9b-707">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="14a9b-708">Couverture de test accrue</span><span class="sxs-lookup"><span data-stu-id="14a9b-708">Increased test coverage</span></span>
* <span data-ttu-id="14a9b-709">Amélioration du mouvement « ? » pour injecter également dans la commande suivante</span><span class="sxs-lookup"><span data-stu-id="14a9b-709">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="14a9b-710">Correction d’erreurs interactives avec le profil 2017-03-09-profil-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="14a9b-710">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="14a9b-711">Autorisé `--version` en tant que paramètre pour le mode interactif (#3645)</span><span class="sxs-lookup"><span data-stu-id="14a9b-711">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="14a9b-712">Empêche le mode interactif de lever des erreurs à partir des listes de saisie semi-automatique de validation (#3570)</span><span class="sxs-lookup"><span data-stu-id="14a9b-712">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="14a9b-713">Rapports de progression pour les déploiements de modèles (#3510)</span><span class="sxs-lookup"><span data-stu-id="14a9b-713">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="14a9b-714">Ajout de l’indicateur `--progress`</span><span class="sxs-lookup"><span data-stu-id="14a9b-714">Added `--progress` flag</span></span>
* <span data-ttu-id="14a9b-715">Suppression `--debug` et `--verbose` des listes de saisie semi-automatique</span><span class="sxs-lookup"><span data-stu-id="14a9b-715">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="14a9b-716">Suppression `interactive` des listes de saisie semi-automatique (#3324)</span><span class="sxs-lookup"><span data-stu-id="14a9b-716">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="14a9b-717">IoT</span><span class="sxs-lookup"><span data-stu-id="14a9b-717">IoT</span></span>

* <span data-ttu-id="14a9b-718">La création de la stratégie n’efface plus les stratégies existantes.</span><span class="sxs-lookup"><span data-stu-id="14a9b-718">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="14a9b-719">(#3934)</span><span class="sxs-lookup"><span data-stu-id="14a9b-719">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="14a9b-720">Coffre de clés</span><span class="sxs-lookup"><span data-stu-id="14a9b-720">Key vault</span></span>

* <span data-ttu-id="14a9b-721">Ajout de commandes pour les fonctionnalités de récupération de coffre de clés :</span><span class="sxs-lookup"><span data-stu-id="14a9b-721">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="14a9b-722">`keyvault`sous-commandes `purge`, `recover`,`keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="14a9b-722">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="14a9b-723">`keyvault secret`sous-commandes `backup`, `restore`, `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="14a9b-723">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="14a9b-724">`keyvault certificate`sous-commandes `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="14a9b-724">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="14a9b-725">`keyvault key`sous-commandes `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="14a9b-725">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="14a9b-726">Ajout de l’intégration du coffre de clés du principal du service (#3133)</span><span class="sxs-lookup"><span data-stu-id="14a9b-726">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="14a9b-727">Mise à jour du plan de données du coffre de clés vers 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="14a9b-727">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="14a9b-728">(#3307)</span><span class="sxs-lookup"><span data-stu-id="14a9b-728">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="14a9b-729">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="14a9b-729">Lab</span></span>

* <span data-ttu-id="14a9b-730">Ajout de la prise en charge de la revendication de toutes les machines virtuelles dans le laboratoire via `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="14a9b-730">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="14a9b-731">Ajout du formateur de sortie de tableau pour `az lab vm list` et `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="14a9b-731">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="14a9b-732">Surveiller</span><span class="sxs-lookup"><span data-stu-id="14a9b-732">Monitor</span></span>

* <span data-ttu-id="14a9b-733">Correctif pour le fichier de modèle avec `monitor autoscale-settings get-parameters-template` commande (#3349)</span><span class="sxs-lookup"><span data-stu-id="14a9b-733">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="14a9b-734">Renommage de `monitor alert-rule-incidents list` en `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="14a9b-734">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="14a9b-735">Renommage de `monitor alert-rule-incidents show` en `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="14a9b-735">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="14a9b-736">Renommage de `monitor metric-defintions list` en `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="14a9b-736">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="14a9b-737">Renommage de `monitor alert-rules` en `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="14a9b-737">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="14a9b-738">Modifié `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="14a9b-738">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="14a9b-739">sous-commandes`condition` et `action` n’acceptent plus JSON</span><span class="sxs-lookup"><span data-stu-id="14a9b-739">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="14a9b-740">Ajout de nombreux paramètres simplifiant le processus de création de règle</span><span class="sxs-lookup"><span data-stu-id="14a9b-740">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="14a9b-741">`location` n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="14a9b-741">`location` no longer required</span></span>
  * <span data-ttu-id="14a9b-742">Ajout d’un nom et de la prise en charge de l’ID de la cible</span><span class="sxs-lookup"><span data-stu-id="14a9b-742">Add name and ID support for target</span></span>
  * <span data-ttu-id="14a9b-743">Suppression de `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="14a9b-743">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="14a9b-744">Le renommage de `is-enabled` en `enabled`n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="14a9b-744">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="14a9b-745">`description` par défaut sont désormais basées sur la condition fournie</span><span class="sxs-lookup"><span data-stu-id="14a9b-745">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="14a9b-746">Ajout d’exemples aidant à clarifier le nouveau format</span><span class="sxs-lookup"><span data-stu-id="14a9b-746">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="14a9b-747">Prise en charge des noms ou des ID pour les commandes `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="14a9b-747">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="14a9b-748">Ajout d’arguments d’usage et d’exemples pour `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="14a9b-748">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="14a9b-749">Réseau</span><span class="sxs-lookup"><span data-stu-id="14a9b-749">Network</span></span>

* <span data-ttu-id="14a9b-750">Ajout de la commande `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="14a9b-750">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="14a9b-751">Ajout de l’argument `--private-access-services` à `vnet subnet create` et `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="14a9b-751">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="14a9b-752">Correction d’un problème `application-gateway redirect-config create` qui causait l’échec de</span><span class="sxs-lookup"><span data-stu-id="14a9b-752">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="14a9b-753">Correction d’un problème `application-gateway redirect-config update` qui `--no-wait` empêchait le fonctionnement de</span><span class="sxs-lookup"><span data-stu-id="14a9b-753">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="14a9b-754">Correction d’un bogue lié à l’utilisation d’un `--servers` argument avec `application-gateway address-pool create` et `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="14a9b-754">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="14a9b-755">Ajout des commandes `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="14a9b-755">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="14a9b-756">Ajout de commandes à `application-gateway ssl-policy` : `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="14a9b-756">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="14a9b-757">Ajout d’arguments à `application-gateway ssl-policy set` : `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="14a9b-757">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="14a9b-758">Ajout d’arguments à `application-gateway http-settings create` et `application-gateway http-settings update` : `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="14a9b-758">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="14a9b-759">Ajout d’arguments à `application-gateway url-path-map create` et `application-gateway url-path-map update`, `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="14a9b-759">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="14a9b-760">Ajout d’un argument `--redirect-config` à `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="14a9b-760">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="14a9b-761">Ajout de la prise en charge de `--no-wait` pour `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="14a9b-761">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="14a9b-762">Ajout d’arguments à `application-gateway probe create` et `application-gateway probe update` : `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="14a9b-762">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="14a9b-763">Ajout d’un argument `--redirect-config` à `application-gateway rule create` et `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="14a9b-763">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="14a9b-764">Ajout de la prise en charge de `--accelerated-networking` pour `nic create` et `nic update`</span><span class="sxs-lookup"><span data-stu-id="14a9b-764">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="14a9b-765">Suppression de l’ `--internal-dns-name-suffix` argument à partir de `nic create`</span><span class="sxs-lookup"><span data-stu-id="14a9b-765">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="14a9b-766">Ajout de la prise en charge de `--dns-servers` pour `nic update` et `nic create` : ajout de la prise en charge pour les serveurs DNS :</span><span class="sxs-lookup"><span data-stu-id="14a9b-766">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="14a9b-767">Correction d’un bogue qui faisait `local-gateway create` ignorer `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="14a9b-767">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="14a9b-768">Ajout de la prise en charge de `--dns-servers` pour `vnet update`</span><span class="sxs-lookup"><span data-stu-id="14a9b-768">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="14a9b-769">Correction d’un bogue lors de la création d’une homologation sans filtrage de l’itinéraire avec `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="14a9b-769">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="14a9b-770">Correction d’un bogue qui empêchait le fonctionnement des arguments `--provider` et `--bandwidth` avec `express-route update`</span><span class="sxs-lookup"><span data-stu-id="14a9b-770">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="14a9b-771">Correction d’un bogue avec `network watcher show-topology` une logique de valeurs par défaut</span><span class="sxs-lookup"><span data-stu-id="14a9b-771">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="14a9b-772">Amélioration de la mise en forme de sortie pour `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="14a9b-772">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="14a9b-773">Utilisation de l’IP frontale par défaut pour `application-gateway http-listener create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="14a9b-773">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="14a9b-774">Utilisation d’un pool d’adresses par défaut, des paramètres HTTP et de l’écouteur HTTP pour `application-gateway rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="14a9b-774">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="14a9b-775">Utilisation de l’IP frontale par défaut et du pool principal `lb rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="14a9b-775">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="14a9b-776">Utilisation de l’IP frontale par défaut pour `lb inbound-nat-rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="14a9b-776">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="14a9b-777">Profil</span><span class="sxs-lookup"><span data-stu-id="14a9b-777">Profile</span></span>

* <span data-ttu-id="14a9b-778">Prise en charge de la connexion à l’intérieur d’une machine virtuelle avec une identité gérée</span><span class="sxs-lookup"><span data-stu-id="14a9b-778">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="14a9b-779">Prise en charge de la sortie pour `account show` au format de fichier d’authentification du Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="14a9b-779">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="14a9b-780">Affichage des avertissements de désapprobation lors de l’utilisation de '--expanded-view'</span><span class="sxs-lookup"><span data-stu-id="14a9b-780">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="14a9b-781">Ajout de la commande `get-access-token` permettant de fournir un jeton AAD brut</span><span class="sxs-lookup"><span data-stu-id="14a9b-781">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="14a9b-782">Prise en charge de la connexion avec un compte d’utilisateur sans abonnements associés</span><span class="sxs-lookup"><span data-stu-id="14a9b-782">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="14a9b-783">SGBDR</span><span class="sxs-lookup"><span data-stu-id="14a9b-783">RDBMS</span></span>

* <span data-ttu-id="14a9b-784">Prise en charge de l’énumération de serveurs à travers un abonnement (#3417)</span><span class="sxs-lookup"><span data-stu-id="14a9b-784">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="14a9b-785">Correction de `%s` non traité car il manque `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="14a9b-785">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="14a9b-786">Correction du mappage de la source du document et ajout de la tâche CI permettant la vérification de (#3361)</span><span class="sxs-lookup"><span data-stu-id="14a9b-786">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="14a9b-787">Correction concernant l’aide relative à MySQL et PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="14a9b-787">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="14a9b-788">Ressource</span><span class="sxs-lookup"><span data-stu-id="14a9b-788">Resource</span></span>

* <span data-ttu-id="14a9b-789">Amélioration des invites pour les paramètres manquants de `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="14a9b-789">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="14a9b-790">Amélioration de l’analyse de `--parameters KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="14a9b-790">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="14a9b-791">Correction des problèmes à cause desquels `group deployment create` les fichiers de paramètres n’étaient plus reconnus à l’aide de la `@<file>` syntaxe</span><span class="sxs-lookup"><span data-stu-id="14a9b-791">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="14a9b-792">Prise en charge de l’ `--ids` argument pour `resource` et `managedapp` les commandes</span><span class="sxs-lookup"><span data-stu-id="14a9b-792">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="14a9b-793">Correction de certains messages d’analyse et d’erreur (#3584)</span><span class="sxs-lookup"><span data-stu-id="14a9b-793">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="14a9b-794">Correction de l’analyse `--resource-type` permettant à la `lock` commande d’accepter `<resource-namespace>` et `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="14a9b-794">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="14a9b-795">Ajout de la vérification de paramètre des modèles de liaison de modèle (#3629)</span><span class="sxs-lookup"><span data-stu-id="14a9b-795">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="14a9b-796">Ajout de la prise en charge de la spécification des paramètres de déploiement à l’aide de la `KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="14a9b-796">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="14a9b-797">Rôle</span><span class="sxs-lookup"><span data-stu-id="14a9b-797">Role</span></span>

* <span data-ttu-id="14a9b-798">Prise en charge de la sortie au format de fichier d’authentification du Kit de développement logiciel (SDK) pour `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="14a9b-798">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="14a9b-799">Nettoyage des attributions de rôles et de l’application AAD liée lors de la suppression d’un principal de service (#3610)</span><span class="sxs-lookup"><span data-stu-id="14a9b-799">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="14a9b-800">Inclusion du format d’heure dans `app create` args `--start-date` et `--end-date` descriptions</span><span class="sxs-lookup"><span data-stu-id="14a9b-800">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="14a9b-801">Affichage des avertissements de désapprobation lors de l’utilisation de `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="14a9b-801">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="14a9b-802">Ajout de l’intégration du coffre de clés pour les commandes `create-for-rbac` et `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="14a9b-802">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="14a9b-803">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="14a9b-803">Service Fabric</span></span>
* <span data-ttu-id="14a9b-804">Correction d’un problème avec les fichiers volumineux dans les applications tronquées sur le chargement (#3666)</span><span class="sxs-lookup"><span data-stu-id="14a9b-804">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="14a9b-805">Ajout de tests pour les commandes Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="14a9b-805">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="14a9b-806">Correction de nombreuses commandes Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="14a9b-806">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="14a9b-807">SQL</span><span class="sxs-lookup"><span data-stu-id="14a9b-807">SQL</span></span>

* <span data-ttu-id="14a9b-808">Suppression du paramètre rompu `sql server create` `--identity`</span><span class="sxs-lookup"><span data-stu-id="14a9b-808">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="14a9b-809">Suppression des valeurs de mot de passe à partir de la sortie de commande `sql server create` et `sql server update`</span><span class="sxs-lookup"><span data-stu-id="14a9b-809">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="14a9b-810">Ajout des commandes `sql db list-editions` et `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="14a9b-810">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="14a9b-811">Stockage</span><span class="sxs-lookup"><span data-stu-id="14a9b-811">Storage</span></span>

* <span data-ttu-id="14a9b-812">Suppression d’une `--marker` option à partir des commandes `storage blob list`, `storage container list`et `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="14a9b-812">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="14a9b-813">Activation de la création d’un compte de stockage https-only</span><span class="sxs-lookup"><span data-stu-id="14a9b-813">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="14a9b-814">Mise à jour des métriques de stockage, de la journalisation et des commandes cors (#3495)</span><span class="sxs-lookup"><span data-stu-id="14a9b-814">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="14a9b-815">Reformulation d’un message d’exception de l’ajout CORS (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="14a9b-815">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="14a9b-816">Conversion du générateur à une liste en mode exécution d’essai de la commande de téléchargement de lot (#3592)</span><span class="sxs-lookup"><span data-stu-id="14a9b-816">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="14a9b-817">Correction du problème d’essai associé au lot de téléchargement du blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="14a9b-817">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="14a9b-818">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14a9b-818">VM</span></span>

* <span data-ttu-id="14a9b-819">Prise en charge de la configuration du groupe de sécurité réseau</span><span class="sxs-lookup"><span data-stu-id="14a9b-819">Support configuring nsg</span></span>
* <span data-ttu-id="14a9b-820">Correction d’un bogue qui entraînait une configuration incorrecte du serveur DNS</span><span class="sxs-lookup"><span data-stu-id="14a9b-820">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="14a9b-821">Prise en charge des identités de service géré</span><span class="sxs-lookup"><span data-stu-id="14a9b-821">Support managed service identities</span></span>
* <span data-ttu-id="14a9b-822">Correction d’un problème à cause duquel `cmss create` avec un équilibreur de charge existant exigeait `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="14a9b-822">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`.</span></span>
* <span data-ttu-id="14a9b-823">Les disques de données créés avec le numéro d’unité logique `vm image create` commencent à 0</span><span class="sxs-lookup"><span data-stu-id="14a9b-823">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="14a9b-824">10 mai 2017</span><span class="sxs-lookup"><span data-stu-id="14a9b-824">May 10, 2017</span></span>

<span data-ttu-id="14a9b-825">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="14a9b-825">Version 2.0.6</span></span>

* <span data-ttu-id="14a9b-826">documentdb renommé en cosmosdb</span><span class="sxs-lookup"><span data-stu-id="14a9b-826">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="14a9b-827">Ajouter rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="14a9b-827">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="14a9b-828">Inclure les modules Data Lake Analytics et Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="14a9b-828">Include Data Lake Analytics and Data Lake Store modules.</span></span>
* <span data-ttu-id="14a9b-829">Inclure le module Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="14a9b-829">Include Cognitive Services module.</span></span>
* <span data-ttu-id="14a9b-830">Inclure le module Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="14a9b-830">Include Service Fabric module.</span></span>
* <span data-ttu-id="14a9b-831">Inclure le module Interactive (az-shell renommé).</span><span class="sxs-lookup"><span data-stu-id="14a9b-831">Include Interactive module (rename of az-shell).</span></span>
* <span data-ttu-id="14a9b-832">Ajouter la prise en charge des commandes CDN.</span><span class="sxs-lookup"><span data-stu-id="14a9b-832">Add support for CDN commands.</span></span>
* <span data-ttu-id="14a9b-833">Supprimer le module Container.</span><span class="sxs-lookup"><span data-stu-id="14a9b-833">Remove Container module.</span></span>
* <span data-ttu-id="14a9b-834">Ajouter « az -v » comme raccourci pour « az --version » ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="14a9b-834">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="14a9b-835">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="14a9b-835">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="14a9b-836">Principal</span><span class="sxs-lookup"><span data-stu-id="14a9b-836">Core</span></span>

* <span data-ttu-id="14a9b-837">principal : capturer les exceptions provoquées par un fournisseur non enregistré et l’enregistrer automatiquement</span><span class="sxs-lookup"><span data-stu-id="14a9b-837">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="14a9b-838">performance : conserver le cache de jeton adal en mémoire jusqu’à la fin du processus ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="14a9b-838">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="14a9b-839">Corriger les octets retournés par l’empreinte digitale hex -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="14a9b-839">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="14a9b-840">Téléchargement du certificat Key Vault et intégration AAD SP améliorés ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="14a9b-840">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="14a9b-841">Ajouter l’emplacement de Python à « az —version » ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="14a9b-841">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="14a9b-842">connexion : prise en charge de la connexion lorsqu’il n’y a aucun abonnement ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="14a9b-842">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="14a9b-843">principal : corriger une erreur lors de la connexion à l’aide d’un principal de service deux fois ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="14a9b-843">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="14a9b-844">principal : autoriser la configuration du chemin d’accès de accessTokens.json via une variable d’environnement ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="14a9b-844">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="14a9b-845">principal : autoriser l’application des valeurs par défaut configurées sur les arguments facultatifs ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="14a9b-845">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="14a9b-846">principal : performances améliorées</span><span class="sxs-lookup"><span data-stu-id="14a9b-846">core: Improved performance</span></span>
* <span data-ttu-id="14a9b-847">principal : certificats d’autorité de certification personnalisés - prise en charge de la définition de la variable d’environnement REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="14a9b-847">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="14a9b-848">principal : configuration du cloud - utiliser le point de terminaison « resource manager » si le point de terminaison « management » n’est pas défini</span><span class="sxs-lookup"><span data-stu-id="14a9b-848">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="14a9b-849">ACS</span><span class="sxs-lookup"><span data-stu-id="14a9b-849">ACS</span></span>

* <span data-ttu-id="14a9b-850">corriger le nombre de maîtres et d’agents sur un nombre entier au lieu d’une chaîne</span><span class="sxs-lookup"><span data-stu-id="14a9b-850">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="14a9b-851">exposer « az acs create --no-wait » et « az acs wait » pour la création asynchrone</span><span class="sxs-lookup"><span data-stu-id="14a9b-851">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="14a9b-852">exposer « az acs create --validate » pour les validations de test</span><span class="sxs-lookup"><span data-stu-id="14a9b-852">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="14a9b-853">supprimer le profil Windows avant l’appel PUT pour la commande de mise à l’échelle ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="14a9b-853">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="14a9b-854">AppService</span><span class="sxs-lookup"><span data-stu-id="14a9b-854">AppService</span></span>

* <span data-ttu-id="14a9b-855">functionapp : ajouter la prise en charge complète de functionapp, notamment créer, afficher, liste, supprimer, nom d’hôte, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="14a9b-855">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="14a9b-856">Ajout de Team Services (vsts) comme option de livraison continue à « config contrôle source web appservice »</span><span class="sxs-lookup"><span data-stu-id="14a9b-856">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="14a9b-857">Créer « az webapp » pour remplacer « az appservice web » (pour la rétrocompatibilité, « az appservice web » sera conservé dans les 2 prochaines versions)</span><span class="sxs-lookup"><span data-stu-id="14a9b-857">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="14a9b-858">Exposer des arguments pour configurer le déploiement et des « piles d’exécution » sur webapp create</span><span class="sxs-lookup"><span data-stu-id="14a9b-858">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="14a9b-859">Exposer « webapp list-runtimes »</span><span class="sxs-lookup"><span data-stu-id="14a9b-859">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="14a9b-860">prendre en charge la configuration des chaînes de connexion ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="14a9b-860">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="14a9b-861">prendre en charge le basculement d’emplacement avec aperçu</span><span class="sxs-lookup"><span data-stu-id="14a9b-861">support slot swap with preview</span></span>
* <span data-ttu-id="14a9b-862">Supprimer les erreurs des commandes appservice ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="14a9b-862">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="14a9b-863">Utiliser le groupe de ressources du plan app service pour les opérations de certificat ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="14a9b-863">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="14a9b-864">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="14a9b-864">CosmosDB</span></span>

* <span data-ttu-id="14a9b-865">Renommer le module documentdb en cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="14a9b-865">Rename documentdb module to cosmosdb.</span></span>
* <span data-ttu-id="14a9b-866">Prise en charge ajoutée pour les API de plan de données documentdb : gestion de base de données et de collecte</span><span class="sxs-lookup"><span data-stu-id="14a9b-866">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="14a9b-867">Prise en charge ajoutée pour activer le basculement automatique sur les comptes de base de données</span><span class="sxs-lookup"><span data-stu-id="14a9b-867">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="14a9b-868">Prise en charge ajoutée pour la nouvelle stratégie de cohérence ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="14a9b-868">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="14a9b-869">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="14a9b-869">Data Lake Analytics</span></span>

* <span data-ttu-id="14a9b-870">Corriger un bogue dans lequel le filtrage sur le résultat et l’état des listes de travaux lève une erreur.</span><span class="sxs-lookup"><span data-stu-id="14a9b-870">Fix a bug where filtering on result and state for job lists would throw an error.</span></span>
* <span data-ttu-id="14a9b-871">Ajouter la prise en charge d’un nouveau type d’élément de catalogue : paquet.</span><span class="sxs-lookup"><span data-stu-id="14a9b-871">Add support for new catalog item type: package.</span></span> <span data-ttu-id="14a9b-872">accessible via : `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="14a9b-872">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="14a9b-873">A rendu possible le fait de répertorier les éléments de catalogue suivants à partir d’une base de données (aucune spécification de schéma requise) :</span><span class="sxs-lookup"><span data-stu-id="14a9b-873">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="14a9b-874">Table</span><span class="sxs-lookup"><span data-stu-id="14a9b-874">Table</span></span>
  * <span data-ttu-id="14a9b-875">Fonction table</span><span class="sxs-lookup"><span data-stu-id="14a9b-875">Table valued function</span></span>
  * <span data-ttu-id="14a9b-876">Affichage</span><span class="sxs-lookup"><span data-stu-id="14a9b-876">View</span></span>
  * <span data-ttu-id="14a9b-877">Statistiques de table.</span><span class="sxs-lookup"><span data-stu-id="14a9b-877">Table Statistics.</span></span> <span data-ttu-id="14a9b-878">Cela peut également être répertorié avec un schéma, mais sans spécifier un nom de table.</span><span class="sxs-lookup"><span data-stu-id="14a9b-878">This can also be listed with a schema, but without specifying a table name.</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="14a9b-879">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="14a9b-879">Data Lake Store</span></span>

* <span data-ttu-id="14a9b-880">Mettre à jour la version du Kit de développement logiciel (SDK) du système de fichiers sous-jacent, qui offre une meilleure prise en charge pour gérer les scénarios de limitation côté serveur.</span><span class="sxs-lookup"><span data-stu-id="14a9b-880">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios.</span></span>
* <span data-ttu-id="14a9b-881">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="14a9b-881">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="14a9b-882">aide manquante pour afficher l’accès.</span><span class="sxs-lookup"><span data-stu-id="14a9b-882">missed help for access show.</span></span> <span data-ttu-id="14a9b-883">ajout en cours.</span><span class="sxs-lookup"><span data-stu-id="14a9b-883">adding it.</span></span> <span data-ttu-id="14a9b-884">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="14a9b-884">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="14a9b-885">Rechercher</span><span class="sxs-lookup"><span data-stu-id="14a9b-885">Find</span></span>

* <span data-ttu-id="14a9b-886">résultats de la recherche améliorés et autorisation du contrôle de version de l’index de recherche</span><span class="sxs-lookup"><span data-stu-id="14a9b-886">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="14a9b-887">KeyVault</span><span class="sxs-lookup"><span data-stu-id="14a9b-887">KeyVault</span></span>

* <span data-ttu-id="14a9b-888">BC : `az keyvault certificate download` remplacer -e dans chaîne ou élément binaire par PEM ou DER afin de mieux représenter les options</span><span class="sxs-lookup"><span data-stu-id="14a9b-888">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="14a9b-889">BC : Supprimer --expires et --not-before dans `keyvault certificate create` car ces paramètres ne sont pas pris en charge par le service.</span><span class="sxs-lookup"><span data-stu-id="14a9b-889">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service.</span></span>
* <span data-ttu-id="14a9b-890">Ajoute le paramètre --validity à `keyvault certificate create` pour substituer de manière sélective la valeur dans --policy</span><span class="sxs-lookup"><span data-stu-id="14a9b-890">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="14a9b-891">Résout le problème dans `keyvault certificate get-default-policy` où « expires » et « not_before » étaient exposés mais « validity_in_months » ne l’était pas.</span><span class="sxs-lookup"><span data-stu-id="14a9b-891">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not.</span></span>
* <span data-ttu-id="14a9b-892">correction de keyvault pour l’importation de pem et pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="14a9b-892">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="14a9b-893">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="14a9b-893">Lab</span></span>

* <span data-ttu-id="14a9b-894">Ajout des commandes créer, afficher, supprimer et liste pour l’environnement dans le laboratoire.</span><span class="sxs-lookup"><span data-stu-id="14a9b-894">Adding create, show, delete & list commands for environment in the lab.</span></span>
* <span data-ttu-id="14a9b-895">Ajout des commandes afficher et liste pour afficher les modèles ARM dans le laboratoire.</span><span class="sxs-lookup"><span data-stu-id="14a9b-895">Adding show & list commands to view ARM templates in the lab.</span></span>
* <span data-ttu-id="14a9b-896">Ajout de l’indicateur --environment dans `az lab vm list` pour filtrer les machines virtuelles selon l’environnement du laboratoire.</span><span class="sxs-lookup"><span data-stu-id="14a9b-896">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab.</span></span>
* <span data-ttu-id="14a9b-897">Ajout de la commande pratique `az lab formula export-artifacts` pour exporter une structure d’artefact dans une formule de laboratoire.</span><span class="sxs-lookup"><span data-stu-id="14a9b-897">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula.</span></span>
* <span data-ttu-id="14a9b-898">Ajout de commandes pour gérer les secrets dans un laboratoire.</span><span class="sxs-lookup"><span data-stu-id="14a9b-898">Add commands to manage secrets within a Lab.</span></span>

### <a name="monitor"></a><span data-ttu-id="14a9b-899">Surveiller</span><span class="sxs-lookup"><span data-stu-id="14a9b-899">Monitor</span></span>

* <span data-ttu-id="14a9b-900">Correction de bogue : modélisation `--actions` de `az alert-rules create` pour consommer la chaîne JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="14a9b-900">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="14a9b-901">Correction de bogue : la création de paramètres de diagnostic n’accepte pas les métriques/journaux à partir des commandes d’affichage ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="14a9b-901">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="14a9b-902">Réseau</span><span class="sxs-lookup"><span data-stu-id="14a9b-902">Network</span></span>

* <span data-ttu-id="14a9b-903">Ajouter la commande `network watcher test-connectivity`.</span><span class="sxs-lookup"><span data-stu-id="14a9b-903">Add `network watcher test-connectivity` command.</span></span>
* <span data-ttu-id="14a9b-904">Ajouter la prise en charge du paramètre `--filters` pour `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="14a9b-904">Add support for `--filters` parameter for `network watcher packet-capture create`.</span></span>
* <span data-ttu-id="14a9b-905">Ajouter la prise en charge pour le drainage de connexion Application Gateway.</span><span class="sxs-lookup"><span data-stu-id="14a9b-905">Add support for Application Gateway connection draining.</span></span>
* <span data-ttu-id="14a9b-906">Ajouter la prise en charge pour la configuration du jeu de règles WAF d’Application Gateway.</span><span class="sxs-lookup"><span data-stu-id="14a9b-906">Add support for Application Gateway WAF rule set configuration.</span></span>
* <span data-ttu-id="14a9b-907">Ajouter la prise en charge des règles et des filtres de routage ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="14a9b-907">Add support for ExpressRoute route filters and rules.</span></span>
* <span data-ttu-id="14a9b-908">Ajouter la prise en charge pour le routage géographique TrafficManager.</span><span class="sxs-lookup"><span data-stu-id="14a9b-908">Add support for TrafficManager geographic routing.</span></span>
* <span data-ttu-id="14a9b-909">Ajouter la prise en charge des sélecteurs de trafic basés sur la stratégie de connexion VPN.</span><span class="sxs-lookup"><span data-stu-id="14a9b-909">Add support for VPN connection policy-based traffic selectors.</span></span>
* <span data-ttu-id="14a9b-910">Ajouter la prise en charge pour les stratégies IPSec de la connexion VPN.</span><span class="sxs-lookup"><span data-stu-id="14a9b-910">Add support for VPN connection IPSec policies.</span></span>
* <span data-ttu-id="14a9b-911">Corriger le bogue avec `vpn-connection create` lors de l’utilisation des paramètres `--no-wait` ou `--validate`.</span><span class="sxs-lookup"><span data-stu-id="14a9b-911">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters.</span></span>
* <span data-ttu-id="14a9b-912">Ajouter la prise en charge des passerelles de réseau virtuel actif-actif</span><span class="sxs-lookup"><span data-stu-id="14a9b-912">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="14a9b-913">Supprimer les valeurs NULL de la sortie des commandes `network vpn-connection list/show`.</span><span class="sxs-lookup"><span data-stu-id="14a9b-913">Remove nulls values from output of `network vpn-connection list/show` commands.</span></span>
* <span data-ttu-id="14a9b-914">BC : résoudre un bogue dans la sortie de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="14a9b-914">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="14a9b-915">Corriger le bogue où l’argument « --key-length » de « vpn-connection create » n’était pas analysé correctement.</span><span class="sxs-lookup"><span data-stu-id="14a9b-915">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly.</span></span>
* <span data-ttu-id="14a9b-916">Corriger le bogue dans `dns zone import` où les enregistrements n’étaient pas été importés correctement.</span><span class="sxs-lookup"><span data-stu-id="14a9b-916">Fix bug in `dns zone import` where records were not imported correctly.</span></span>
* <span data-ttu-id="14a9b-917">Corriger le bogue où `traffic-manager endpoint update` ne fonctionnait pas.</span><span class="sxs-lookup"><span data-stu-id="14a9b-917">Fix bug where `traffic-manager endpoint update` did not work.</span></span>
* <span data-ttu-id="14a9b-918">Ajouter des commandes d’aperçu « network watcher ».</span><span class="sxs-lookup"><span data-stu-id="14a9b-918">Add 'network watcher' preview commands.</span></span>

### <a name="profile"></a><span data-ttu-id="14a9b-919">Profil</span><span class="sxs-lookup"><span data-stu-id="14a9b-919">Profile</span></span>

* <span data-ttu-id="14a9b-920">Prendre en charge la connexion lorsqu’il n’y a aucun abonnement trouvé ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="14a9b-920">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="14a9b-921">Prendre en charge un nom de paramètre court dans le jeu de comptes az --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="14a9b-921">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="14a9b-922">Redis</span><span class="sxs-lookup"><span data-stu-id="14a9b-922">Redis</span></span>

* <span data-ttu-id="14a9b-923">Ajout d’une commande de mise à jour qui ajoute également la possibilité de mettre à l’échelle pour le cache redis</span><span class="sxs-lookup"><span data-stu-id="14a9b-923">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="14a9b-924">Commande « update-settings » déconseillée.</span><span class="sxs-lookup"><span data-stu-id="14a9b-924">Deprecates the 'update-settings' command.</span></span>

### <a name="resource"></a><span data-ttu-id="14a9b-925">Ressource</span><span class="sxs-lookup"><span data-stu-id="14a9b-925">Resource</span></span>

* <span data-ttu-id="14a9b-926">Ajouter managedapp et les commandes de définition managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="14a9b-926">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="14a9b-927">Prendre en charge les commandes « provider operation » ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="14a9b-927">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="14a9b-928">Prendre en charge la création de ressource générique ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="14a9b-928">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="14a9b-929">Corriger l’analyse de ressource et la recherche de version d’API.</span><span class="sxs-lookup"><span data-stu-id="14a9b-929">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="14a9b-930">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="14a9b-930">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="14a9b-931">Ajouter des documents pour mise à jour du verrou az.</span><span class="sxs-lookup"><span data-stu-id="14a9b-931">Add docs for az lock update.</span></span> <span data-ttu-id="14a9b-932">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="14a9b-932">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="14a9b-933">Sortie d’erreur si vous essayez de lister des ressources pour un groupe qui n’existe pas.</span><span class="sxs-lookup"><span data-stu-id="14a9b-933">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="14a9b-934">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="14a9b-934">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="14a9b-935">[Compute] Résoudre les problèmes de mise à jour de VMSS et du groupe à haute disponibilité de machines virtuelles.</span><span class="sxs-lookup"><span data-stu-id="14a9b-935">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="14a9b-936">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="14a9b-936">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="14a9b-937">Corriger le verrouillage des commandes créer et supprimer si parent-resource-path est None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="14a9b-937">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="14a9b-938">Rôle</span><span class="sxs-lookup"><span data-stu-id="14a9b-938">Role</span></span>

* <span data-ttu-id="14a9b-939">create-for-rbac : vérifier que la date de fin du SP ne dépassera pas la date d’expiration du certificat ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="14a9b-939">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="14a9b-940">RBAC : ajouter la prise en charge complète de « ad group » ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="14a9b-940">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="14a9b-941">rôle : résoudre les problèmes de mise à jour de définition de rôle ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="14a9b-941">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="14a9b-942">create-for-rbac : vérifier que le mot de passe fourni par l’utilisateur est accepté</span><span class="sxs-lookup"><span data-stu-id="14a9b-942">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="14a9b-943">SQL</span><span class="sxs-lookup"><span data-stu-id="14a9b-943">SQL</span></span>

* <span data-ttu-id="14a9b-944">Commandes az sql server list-usages et az sql db list-usages ajoutées.</span><span class="sxs-lookup"><span data-stu-id="14a9b-944">Added az sql server list-usages and az sql db list-usages commands.</span></span>
* <span data-ttu-id="14a9b-945">SQL : possibilité de se connecter directement au fournisseur de ressources ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="14a9b-945">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="14a9b-946">Stockage</span><span class="sxs-lookup"><span data-stu-id="14a9b-946">Storage</span></span>

* <span data-ttu-id="14a9b-947">Définir l’emplacement par défaut sur l’emplacement du groupe de ressources pour `storage account create`.</span><span class="sxs-lookup"><span data-stu-id="14a9b-947">Default location to resource group location for `storage account create`.</span></span>
* <span data-ttu-id="14a9b-948">Ajouter la prise en charge de la copie incrémentielle d’objet blob</span><span class="sxs-lookup"><span data-stu-id="14a9b-948">Add support for incremental blob copy</span></span>
* <span data-ttu-id="14a9b-949">Ajouter la prise en charge du chargement d’objet blob de blocs volumineux</span><span class="sxs-lookup"><span data-stu-id="14a9b-949">Add support for large block blob upload</span></span>
* <span data-ttu-id="14a9b-950">Modifier la taille de bloc à 100 Mo lorsque le fichier à charger est supérieur à 200 Go</span><span class="sxs-lookup"><span data-stu-id="14a9b-950">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="14a9b-951">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14a9b-951">VM</span></span>

* <span data-ttu-id="14a9b-952">avail-set : rendre le compte de domaine UD&FD facultatif</span><span class="sxs-lookup"><span data-stu-id="14a9b-952">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="14a9b-953">remarque : commandes de machine virtuelle dans clouds souverains Veuillez éviter les fonctionnalités liées au disque managé, notamment :</span><span class="sxs-lookup"><span data-stu-id="14a9b-953">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="14a9b-954">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="14a9b-954">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="14a9b-955">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="14a9b-955">az vm/vmss disk</span></span>
  3. <span data-ttu-id="14a9b-956">Dans « az vm/vmss create », utiliser « —use-unmanaged-disk » pour éviter le disque managé Les autres commandes devraient fonctionner</span><span class="sxs-lookup"><span data-stu-id="14a9b-956">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="14a9b-957">vm/vmss : améliorer le texte d’avertissement lors de la génération de paires de clés ssh</span><span class="sxs-lookup"><span data-stu-id="14a9b-957">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="14a9b-958">vm/vmss : prendre en charge la création à partir d’une image de la Place de marché qui requiert des informations sur le plan ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="14a9b-958">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="14a9b-959">3 avril 2017</span><span class="sxs-lookup"><span data-stu-id="14a9b-959">April 3, 2017</span></span>

<span data-ttu-id="14a9b-960">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="14a9b-960">Version 2.0.2</span></span>

<span data-ttu-id="14a9b-961">Nous avons publié les composants ACR, Batch, KeyVault et SQL dans cette version.</span><span class="sxs-lookup"><span data-stu-id="14a9b-961">We released the ACR, Batch, KeyVault, and SQL components in this release.</span></span>

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

### <a name="core"></a><span data-ttu-id="14a9b-962">Principal</span><span class="sxs-lookup"><span data-stu-id="14a9b-962">Core</span></span>

* <span data-ttu-id="14a9b-963">Ajout des modules acr, lab, monitor et find à la liste par défaut.</span><span class="sxs-lookup"><span data-stu-id="14a9b-963">Add acr, lab, monitor, and find modules to default list.</span></span>
* <span data-ttu-id="14a9b-964">Connexion : ignorer les locataires erronés ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="14a9b-964">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="14a9b-965">login : définition de l’abonnement par défaut à la valeur « un » avec l’état « Activé » ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="14a9b-965">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="14a9b-966">Ajout de la prise en charge des commandes wait et de --no-wait à davantage de commandes ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="14a9b-966">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="14a9b-967">core : prise en charge de la connexion à l’aide du principal du service avec un certificat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="14a9b-967">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="14a9b-968">Ajout d’une invite pour les paramètres de modèle manquants.</span><span class="sxs-lookup"><span data-stu-id="14a9b-968">Add prompting for missing template parameters.</span></span> <span data-ttu-id="14a9b-969">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="14a9b-969">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="14a9b-970">Prise en charge de la définition de valeurs par défaut pour des arguments courants tels que le groupe de ressources par défaut, le site web par défaut et la machine virtuelle par défaut</span><span class="sxs-lookup"><span data-stu-id="14a9b-970">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="14a9b-971">Prise en charge de la connexion à un locataire spécifique</span><span class="sxs-lookup"><span data-stu-id="14a9b-971">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="14a9b-972">ACS</span><span class="sxs-lookup"><span data-stu-id="14a9b-972">ACS</span></span>

* <span data-ttu-id="14a9b-973">[ACS] Ajout de la prise en charge de la configuration d’un cluster ACS par défaut ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="14a9b-973">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="14a9b-974">Ajout de la prise en charge de l’invite de mot de passe de clé ssh.</span><span class="sxs-lookup"><span data-stu-id="14a9b-974">Add support for ssh key password prompting.</span></span> <span data-ttu-id="14a9b-975">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="14a9b-975">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="14a9b-976">Ajout de la prise en charge des clusters Windows.</span><span class="sxs-lookup"><span data-stu-id="14a9b-976">Add support for windows clusters.</span></span> <span data-ttu-id="14a9b-977">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="14a9b-977">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="14a9b-978">Basculement du rôle Propriétaire au rôle Contributeur.</span><span class="sxs-lookup"><span data-stu-id="14a9b-978">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="14a9b-979">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="14a9b-979">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="14a9b-980">AppService</span><span class="sxs-lookup"><span data-stu-id="14a9b-980">AppService</span></span>

* <span data-ttu-id="14a9b-981">appservice : prise en charge de l’obtention de l’adresse IP externe utilisée pour les enregistrements A DNS ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="14a9b-981">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="14a9b-982">appservice : prise en charge de la liaison des certificats avec caractères génériques ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="14a9b-982">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="14a9b-983">appservice : prise en charge des profils de publication de liste ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="14a9b-983">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="14a9b-984">AppService : déclenchement de la synchronisation de contrôle de code source après la configuration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="14a9b-984">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="14a9b-985">DataLake</span><span class="sxs-lookup"><span data-stu-id="14a9b-985">DataLake</span></span>

* <span data-ttu-id="14a9b-986">Version initiale du module Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="14a9b-986">Initial release of Data Lake Analytics module.</span></span>
* <span data-ttu-id="14a9b-987">Version initiale du module Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="14a9b-987">Initial release of Data Lake Store module.</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="14a9b-988">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="14a9b-988">DocuemntDB</span></span>

* <span data-ttu-id="14a9b-989">DocumentDB : ajout de la prise en charge de l’énumération des chaînes de connexion ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="14a9b-989">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="14a9b-990">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="14a9b-990">VM</span></span>

* <span data-ttu-id="14a9b-991">[Compute] Ajout de la prise en charge d’AppGateway à la création de groupe de machines virtuelles identiques ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="14a9b-991">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="14a9b-992">[VM/VMSS] Amélioration de la prise en charge de la mise en cache de disque ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="14a9b-992">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="14a9b-993">VM/VMSS : intégration de la logique de validation des informations d’identification utilisée par le portail ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="14a9b-993">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="14a9b-994">Ajout de la prise en charge des commandes wait et de --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="14a9b-994">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="14a9b-995">Groupe de machines virtuelles identiques : prise en charge de \* pour énumérer les vues d’instance parmi les machines virtuelles ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="14a9b-995">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="14a9b-996">Ajout de --secrets pour les machines virtuelles et les groupes de machines virtuelles identiques ([#2212} (https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="14a9b-996">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="14a9b-997">Autorisation de la création de machines virtuelles avec un disque dur virtuel spécialisé ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="14a9b-997">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="14a9b-998">27 février 2017</span><span class="sxs-lookup"><span data-stu-id="14a9b-998">February 27, 2017</span></span>

<span data-ttu-id="14a9b-999">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="14a9b-999">Version 2.0.0</span></span>

<span data-ttu-id="14a9b-1000">Cette version d’Azure CLI 2.0 est la première version en « Disponibilité générale ».</span><span class="sxs-lookup"><span data-stu-id="14a9b-1000">This release of Azure CLI 2.0 is the first "Generally Available" release.</span></span>
<span data-ttu-id="14a9b-1001">La disponibilité générale s’applique à ces modules de commande :</span><span class="sxs-lookup"><span data-stu-id="14a9b-1001">General availability applies to these command modules:</span></span>
- <span data-ttu-id="14a9b-1002">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="14a9b-1002">Container Service (acs)</span></span>
- <span data-ttu-id="14a9b-1003">Compute (notamment Resource Manager, machine virtuelle, groupes de machines virtuelles identiques, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="14a9b-1003">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="14a9b-1004">Réseau</span><span class="sxs-lookup"><span data-stu-id="14a9b-1004">Networking</span></span>
- <span data-ttu-id="14a9b-1005">Stockage</span><span class="sxs-lookup"><span data-stu-id="14a9b-1005">Storage</span></span>

<span data-ttu-id="14a9b-1006">Ces modules de commande peuvent être utilisés en production et sont pris en charge par le contrat SLA Microsoft standard.</span><span class="sxs-lookup"><span data-stu-id="14a9b-1006">These command modules can be used in production and are supported by standard Microsoft SLA.</span></span>
<span data-ttu-id="14a9b-1007">Vous pouvez ouvrir des incidents directement auprès du support technique de Microsoft ou dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/).</span><span class="sxs-lookup"><span data-stu-id="14a9b-1007">You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/).</span></span>
<span data-ttu-id="14a9b-1008">Vous pouvez poser des questions sur [StackOverflow à l’aide du mot clé azure-cli](http://stackoverflow.com/questions/tagged/azure-cli) ou contacter l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Vous pouvez fournir des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="14a9b-1008">You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). You can provide feedback from the command line with the `az feedback` command.</span></span>

<span data-ttu-id="14a9b-1009">Les commandes de ces modules sont stables et il n’est pas prévu que la syntaxe change dans les mises à jour ultérieures de cette version d’Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="14a9b-1009">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI.</span></span>

<span data-ttu-id="14a9b-1010">Pour vérifier la version de l’interface CLI, utilisez `az --version`.</span><span class="sxs-lookup"><span data-stu-id="14a9b-1010">To verify the version of the CLI, use `az --version`.</span></span>
<span data-ttu-id="14a9b-1011">La sortie indique la version de l’interface CLI proprement dite (2.0.0 dans cette version), les différents modules de commande et les versions de Python et de GCC que vous utilisez.</span><span class="sxs-lookup"><span data-stu-id="14a9b-1011">The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using.</span></span>

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
> <span data-ttu-id="14a9b-1012">Certains des modules de commande ont un suffixe « b*n* » ou « rc*n* ».</span><span class="sxs-lookup"><span data-stu-id="14a9b-1012">Some of the command modules have a "b*n*" or "rc*n*" postfix.</span></span>
> <span data-ttu-id="14a9b-1013">Ces modules de commande sont toujours en préversion et seront à la disposition générale ultérieurement.</span><span class="sxs-lookup"><span data-stu-id="14a9b-1013">These command modules are still in preview and will become generally available in the future.</span></span>

<span data-ttu-id="14a9b-1014">Nous avons également des versions d’évaluation nocturnes de l’interface CLI.</span><span class="sxs-lookup"><span data-stu-id="14a9b-1014">We also have nightly preview builds of the CLI.</span></span>
<span data-ttu-id="14a9b-1015">Pour plus d’informations, consultez ces instructions sur [l’obtention des builds nocturnes](https://github.com/Azure/azure-cli#nightly-builds) et ces instructions sur [la contribution au code et la configuration d’un environnement de développement](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="14a9b-1015">For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup).</span></span>

<span data-ttu-id="14a9b-1016">Vous pouvez signaler des problèmes liés aux versions d’évaluation nocturnes comme suit :</span><span class="sxs-lookup"><span data-stu-id="14a9b-1016">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="14a9b-1017">Signalez des problèmes dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="14a9b-1017">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="14a9b-1018">Contactez l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="14a9b-1018">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span></span>
- <span data-ttu-id="14a9b-1019">Fournissez des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="14a9b-1019">Provide feedback from the command line with the `az feedback` command.</span></span>

