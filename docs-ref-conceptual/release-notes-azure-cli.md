---
title: Notes de publication d’Azure CLI
description: En savoir plus sur les dernières mises à jour d’Azure CLI
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 10/23/2018
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 65e34ab6014c47ae92a6d4bae8cdc30d4a1413dc
ms.sourcegitcommit: aec89531c938781b4724f43b5bb4b878e106a26a
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/23/2018
ms.locfileid: "49952483"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="217ac-103">Notes de publication d’Azure CLI</span><span class="sxs-lookup"><span data-stu-id="217ac-103">Azure CLI release notes</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="217ac-104">23 octobre 2018</span><span class="sxs-lookup"><span data-stu-id="217ac-104">October 23, 2018</span></span>

<span data-ttu-id="217ac-105">Version 2.0.49</span><span class="sxs-lookup"><span data-stu-id="217ac-105">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="217ac-106">Principal</span><span class="sxs-lookup"><span data-stu-id="217ac-106">Core</span></span>
* <span data-ttu-id="217ac-107">Correction du problème avec `--ids` où `--subscription` serait prioritaire sur l’abonnement dans `--ids`</span><span class="sxs-lookup"><span data-stu-id="217ac-107">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="217ac-108">Ajout d’avertissements explicites lorsque les paramètres sont ignorés par `--ids`</span><span class="sxs-lookup"><span data-stu-id="217ac-108">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="217ac-109">ACR</span><span class="sxs-lookup"><span data-stu-id="217ac-109">ACR</span></span>
* <span data-ttu-id="217ac-110">Correction d’un problème de codage ACR Build dans Python2</span><span class="sxs-lookup"><span data-stu-id="217ac-110">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="217ac-111">CDN</span><span class="sxs-lookup"><span data-stu-id="217ac-111">CDN</span></span>
* <span data-ttu-id="217ac-112">[CHANGEMENT CASSANT] Modification du comportement de mise en cache de chaîne de requête par défaut de `cdn endpoint create` afin que ce ne soit plus « IgnoreQueryString » par défaut.</span><span class="sxs-lookup"><span data-stu-id="217ac-112">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="217ac-113">Il est maintenant défini par le service</span><span class="sxs-lookup"><span data-stu-id="217ac-113">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="217ac-114">Conteneur</span><span class="sxs-lookup"><span data-stu-id="217ac-114">Container</span></span>
* <span data-ttu-id="217ac-115">Ajout de `Private` comme un type valide pour passer à «--ip-address»</span><span class="sxs-lookup"><span data-stu-id="217ac-115">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="217ac-116">Modification pour permettre l’utilisation d’un seul ID de sous-réseau pour configurer un réseau virtuel pour le groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="217ac-116">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="217ac-117">Modification pour permettre l’utilisation d’un nom de réseau virtuel ou d’un ID de ressource pour permettre l’utilisation de réseaux virtuels à partir de groupes de ressources différents</span><span class="sxs-lookup"><span data-stu-id="217ac-117">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="217ac-118">Ajout de `--assign-identity` pour ajouter une identité MSI à un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="217ac-118">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="217ac-119">Ajout de `--scope` pour créer une attribution de rôle pour l’identité MSI attribuée par le système</span><span class="sxs-lookup"><span data-stu-id="217ac-119">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="217ac-120">Ajout d’un avertissement lors de la création d’un groupe de conteneurs avec une image sans processus à long terme</span><span class="sxs-lookup"><span data-stu-id="217ac-120">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="217ac-121">Correction de problèmes de sortie de table pour les commandes `list` et `show`</span><span class="sxs-lookup"><span data-stu-id="217ac-121">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="217ac-122">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="217ac-122">CosmosDB</span></span>
* <span data-ttu-id="217ac-123">Ajout de la prise en charge de `--enable-multiple-write-locations` pour `cosmosdb create`</span><span class="sxs-lookup"><span data-stu-id="217ac-123">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="217ac-124">Interactive</span><span class="sxs-lookup"><span data-stu-id="217ac-124">Interactive</span></span>
* <span data-ttu-id="217ac-125">Modifié pour assurer l’apparition du paramètre d’abonnement global dans les paramètres</span><span class="sxs-lookup"><span data-stu-id="217ac-125">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="217ac-126">IoT Central</span><span class="sxs-lookup"><span data-stu-id="217ac-126">IoT Central</span></span>
* <span data-ttu-id="217ac-127">Ajout d’options de modèle et de nom d’affichage pour la création de l’application IoT central</span><span class="sxs-lookup"><span data-stu-id="217ac-127">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="217ac-128">[CHANGEMENT CASSANT] Suppression de la prise en charge de la référence SKU F1, utilisez la référence SKU S1 à la place</span><span class="sxs-lookup"><span data-stu-id="217ac-128">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="217ac-129">Surveiller</span><span class="sxs-lookup"><span data-stu-id="217ac-129">Monitor</span></span>
* <span data-ttu-id="217ac-130">Change en `monitor activity-log list` :</span><span class="sxs-lookup"><span data-stu-id="217ac-130">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="217ac-131">Prise en charge ajoutée pour répertorier tous les événements au niveau de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="217ac-131">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="217ac-132">Ajout du paramètre `--offset` pour créer plus facilement des requêtes de temps</span><span class="sxs-lookup"><span data-stu-id="217ac-132">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="217ac-133">Amélioration de la validation pour `--start-time` et `--end-time` pour utiliser des plages de formats ISO8601 plus larges et des formats dateHeure plus conviviaux</span><span class="sxs-lookup"><span data-stu-id="217ac-133">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="217ac-134">Ajout de `--namespace` comme alias pour l’option déconseillée `--resource-provider`</span><span class="sxs-lookup"><span data-stu-id="217ac-134">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="217ac-135">`--filters` déconseillé, car aucune valeur autre que celles avec des options fortement typées ne sont prises en charge par le service</span><span class="sxs-lookup"><span data-stu-id="217ac-135">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="217ac-136">Change en `monitor metrics list` :</span><span class="sxs-lookup"><span data-stu-id="217ac-136">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="217ac-137">Ajout du paramètre `--offset` pour créer plus facilement des requêtes de temps</span><span class="sxs-lookup"><span data-stu-id="217ac-137">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="217ac-138">Amélioration de la validation pour `--start-time` et `--end-time` pour utiliser des plages de formats ISO8601 plus larges et des formats dateHeure plus conviviaux</span><span class="sxs-lookup"><span data-stu-id="217ac-138">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="217ac-139">Amélioration de la validation pour les arguments `--event-hub` et `--event-hub-rule` à `monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="217ac-139">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="217ac-140">Réseau</span><span class="sxs-lookup"><span data-stu-id="217ac-140">Network</span></span>
* <span data-ttu-id="217ac-141">Ajout des arguments `--app-gateway-address-pools` et `--gateway-name` à `nic create`, pour prendre en charge l’ajout de pools d’adresses principaux Application Gateway à une carte réseau</span><span class="sxs-lookup"><span data-stu-id="217ac-141">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="217ac-142">Ajout des arguments `--app-gateway-address-pools` et `--gateway-name` à `nic ip-config create/update`, pour prendre en charge l’ajout de pools d’adresses principaux Application Gateway à une carte réseau</span><span class="sxs-lookup"><span data-stu-id="217ac-142">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="217ac-143">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="217ac-143">ServiceBus</span></span>
* <span data-ttu-id="217ac-144">Ajout de `migration_state` en lecture seule à MigrationConfigProperties pour afficher l’état actuel de migration d’espace de noms Standard à Premium de Service Bus</span><span class="sxs-lookup"><span data-stu-id="217ac-144">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="217ac-145">SQL</span><span class="sxs-lookup"><span data-stu-id="217ac-145">SQL</span></span>
* <span data-ttu-id="217ac-146">`sql failover-group create` et `sql failover-group update` corrigés pour fonctionner avec la stratégie de basculement manuel</span><span class="sxs-lookup"><span data-stu-id="217ac-146">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="217ac-147">Stockage</span><span class="sxs-lookup"><span data-stu-id="217ac-147">Storage</span></span>
* <span data-ttu-id="217ac-148">Formatage de sortie de `az storage cors list` corrigé, tous les éléments affichent une clé de « Service » correcte</span><span class="sxs-lookup"><span data-stu-id="217ac-148">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="217ac-149">Ajout du paramètre `--bypass-immutability-policy` pour la suppression du conteneur de stratégie d’immuabilité bloquée</span><span class="sxs-lookup"><span data-stu-id="217ac-149">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="217ac-150">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="217ac-150">VM</span></span>
* <span data-ttu-id="217ac-151">Mode de mise en cache configuré sur `None` pour la série de machines Lv/Lv2 dans `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="217ac-151">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="217ac-152">Mise à jour de la liste des tailles prises en charge, prenant en charge l’accélérateur de mise en réseau pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="217ac-152">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="217ac-153">Ajout des arguments fortement typés pour les configurations d’E/S et Mbits/s Ultrassd pour `disk create`</span><span class="sxs-lookup"><span data-stu-id="217ac-153">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="217ac-154">16 octobre 2018</span><span class="sxs-lookup"><span data-stu-id="217ac-154">October 16, 2018</span></span>

<span data-ttu-id="217ac-155">Version 2.0.48</span><span class="sxs-lookup"><span data-stu-id="217ac-155">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="217ac-156">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="217ac-156">VM</span></span>
* <span data-ttu-id="217ac-157">Résolution du problème de kit de développement logiciel qui a provoqué l’échec d’installation de Homebrew</span><span class="sxs-lookup"><span data-stu-id="217ac-157">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="217ac-158">9 octobre 2018</span><span class="sxs-lookup"><span data-stu-id="217ac-158">October 9, 2018</span></span>

<span data-ttu-id="217ac-159">Version 2.0.47</span><span class="sxs-lookup"><span data-stu-id="217ac-159">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="217ac-160">Principal</span><span class="sxs-lookup"><span data-stu-id="217ac-160">Core</span></span>
* <span data-ttu-id="217ac-161">Gestion améliorée des erreurs « Demande incorrecte »</span><span class="sxs-lookup"><span data-stu-id="217ac-161">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="217ac-162">ACR</span><span class="sxs-lookup"><span data-stu-id="217ac-162">ACR</span></span>
* <span data-ttu-id="217ac-163">Prise en charge de format de tableau similaire, comme le client helm</span><span class="sxs-lookup"><span data-stu-id="217ac-163">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="217ac-164">ACS</span><span class="sxs-lookup"><span data-stu-id="217ac-164">ACS</span></span>
* <span data-ttu-id="217ac-165">Ajout de `aks [create|scale] --nodepool-name` pour configurer le nom du pool de nœuds, tronqué à 12 caractères, par défaut : nodepool1</span><span class="sxs-lookup"><span data-stu-id="217ac-165">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="217ac-166">Correction d’une erreur pour revenir à « scp » lorsque Parimiko échoue</span><span class="sxs-lookup"><span data-stu-id="217ac-166">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="217ac-167">Modification de `aks create` pour ne plus nécessiter `--aad-tenant-id`</span><span class="sxs-lookup"><span data-stu-id="217ac-167">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="217ac-168">Fusion améliorée des informations d'identification Kubernetes lorsque des entrées dupliquées sont présentes</span><span class="sxs-lookup"><span data-stu-id="217ac-168">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="217ac-169">Conteneur</span><span class="sxs-lookup"><span data-stu-id="217ac-169">Container</span></span>
* <span data-ttu-id="217ac-170">Modification de `functionapp create` pour prendre en charge la création d’un type de plan de consommation Linux avec un runtime spécifique</span><span class="sxs-lookup"><span data-stu-id="217ac-170">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="217ac-171">[PRÉVERSION] Prise en charge de l’hébergement d’applications web sur les conteneurs Windows</span><span class="sxs-lookup"><span data-stu-id="217ac-171">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="217ac-172">Event Hub</span><span class="sxs-lookup"><span data-stu-id="217ac-172">Event Hub</span></span>
* <span data-ttu-id="217ac-173">Correction de la commande `eventhub update`</span><span class="sxs-lookup"><span data-stu-id="217ac-173">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="217ac-174">[CHANGEMENT CASSANT] Modification des commandes `list` pour gérer des erreurs resource(s) NotFound(404) d’une manière habituelle au lieu d’afficher une liste vide</span><span class="sxs-lookup"><span data-stu-id="217ac-174">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="217ac-175">Extensions</span><span class="sxs-lookup"><span data-stu-id="217ac-175">Extensions</span></span>
* <span data-ttu-id="217ac-176">Correction d’une erreur de tentative d’ajout d’une extension déjà installée</span><span class="sxs-lookup"><span data-stu-id="217ac-176">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="217ac-177">HDInsight</span><span class="sxs-lookup"><span data-stu-id="217ac-177">HDInsight</span></span>
* <span data-ttu-id="217ac-178">Version initiale</span><span class="sxs-lookup"><span data-stu-id="217ac-178">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="217ac-179">IoT</span><span class="sxs-lookup"><span data-stu-id="217ac-179">IoT</span></span>
* <span data-ttu-id="217ac-180">Ajout de la commande d’installation de l’extension à une bannière pour la première exécution</span><span class="sxs-lookup"><span data-stu-id="217ac-180">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="217ac-181">KeyVault</span><span class="sxs-lookup"><span data-stu-id="217ac-181">KeyVault</span></span>
* <span data-ttu-id="217ac-182">Modification pour restreindre les commandes de stockage keyvault au dernier profil API</span><span class="sxs-lookup"><span data-stu-id="217ac-182">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="217ac-183">Réseau</span><span class="sxs-lookup"><span data-stu-id="217ac-183">Network</span></span>
* <span data-ttu-id="217ac-184">Correction de `network dns zone create` : la commande réussit même si l’utilisateur a configuré un emplacement par défaut.</span><span class="sxs-lookup"><span data-stu-id="217ac-184">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="217ac-185">Voir #6052</span><span class="sxs-lookup"><span data-stu-id="217ac-185">See #6052</span></span>
* <span data-ttu-id="217ac-186">Remplacement de `--remote-vnet-id` pour `network vnet peering create`</span><span class="sxs-lookup"><span data-stu-id="217ac-186">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="217ac-187">Ajout de `--remote-vnet` à `network vnet peering create`, qui accepte un nom ou ID</span><span class="sxs-lookup"><span data-stu-id="217ac-187">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="217ac-188">Prise en charge de multiples préfixes de sous-réseau pour `network vnet create` avec `--subnet-prefixes`</span><span class="sxs-lookup"><span data-stu-id="217ac-188">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="217ac-189">Prise en charge de multiple préfixes de sous-réseau pour `network vnet subnet [create|update]` avec `--address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="217ac-189">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="217ac-190">Correction d’une erreur relative à `network application-gateway create` qui empêchait la création de passerelles avec les références SKU `WAF_v2` ou `Standard_v2`</span><span class="sxs-lookup"><span data-stu-id="217ac-190">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="217ac-191">Ajout de l’argument d’usage `--service-endpoint-policy` à `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="217ac-191">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="217ac-192">Rôle</span><span class="sxs-lookup"><span data-stu-id="217ac-192">Role</span></span>
* <span data-ttu-id="217ac-193">Prise en charge du listing des propriétaires d’applications Azure AD à `ad app owner`</span><span class="sxs-lookup"><span data-stu-id="217ac-193">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="217ac-194">Prise en charge du listing des propriétaires de principaux de service Azure AD à `ad sp owner`</span><span class="sxs-lookup"><span data-stu-id="217ac-194">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="217ac-195">Modification pour garantir que les commandes de mise à jour et de création de définition de rôle acceptent les configurations à autorisations multiples</span><span class="sxs-lookup"><span data-stu-id="217ac-195">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="217ac-196">Modification de `ad sp create-for-rbac` pour garantir que l’URI de la page d’accueil est toujours « https »</span><span class="sxs-lookup"><span data-stu-id="217ac-196">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="217ac-197">Service Bus</span><span class="sxs-lookup"><span data-stu-id="217ac-197">Service Bus</span></span>
* <span data-ttu-id="217ac-198">[CHANGEMENT CASSANT] Modification des commandes `list` pour gérer des erreurs resource(s) NotFound(404) d’une manière habituelle au lieu d’afficher une liste vide</span><span class="sxs-lookup"><span data-stu-id="217ac-198">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="217ac-199">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="217ac-199">VM</span></span>
* <span data-ttu-id="217ac-200">Correction du champ vide `accessSas` dans `disk grant-access`</span><span class="sxs-lookup"><span data-stu-id="217ac-200">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="217ac-201">Modification de `vmss create` pour réserver une plage de port de frontend assez large pour gérer le surprovisionnement</span><span class="sxs-lookup"><span data-stu-id="217ac-201">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="217ac-202">Correction des commandes de mise à jour pour `sig`</span><span class="sxs-lookup"><span data-stu-id="217ac-202">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="217ac-203">Prise en charge `--no-wait` de la gestion de versions d’images dans `sig`</span><span class="sxs-lookup"><span data-stu-id="217ac-203">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="217ac-204">Modification de `vm list-ip-addresses` pour afficher la zone de disponibilité des adresses IP publiques</span><span class="sxs-lookup"><span data-stu-id="217ac-204">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="217ac-205">Modification de `[vm|vmss] disk attach` pour définir le numéro d’identité logique (LUN) par défaut du disque sur le premier emplacement disponible</span><span class="sxs-lookup"><span data-stu-id="217ac-205">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="217ac-206">21 septembre 2018</span><span class="sxs-lookup"><span data-stu-id="217ac-206">September 21, 2018</span></span>

<span data-ttu-id="217ac-207">Version 2.0.46</span><span class="sxs-lookup"><span data-stu-id="217ac-207">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="217ac-208">ACR</span><span class="sxs-lookup"><span data-stu-id="217ac-208">ACR</span></span>
* <span data-ttu-id="217ac-209">Ajout de commandes de tâche ACR</span><span class="sxs-lookup"><span data-stu-id="217ac-209">Added ACR Task commands</span></span>
* <span data-ttu-id="217ac-210">Ajout de la commande d’exécution rapide</span><span class="sxs-lookup"><span data-stu-id="217ac-210">Added quick run command</span></span>
* <span data-ttu-id="217ac-211">Groupe de commandes `build-task` déconseillé</span><span class="sxs-lookup"><span data-stu-id="217ac-211">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="217ac-212">Ajout du groupe de commandes `helm` pour prendre en charge la gestion des graphiques Helm avec ACR</span><span class="sxs-lookup"><span data-stu-id="217ac-212">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="217ac-213">Ajout de la prise en charge de la création idempotent pour les registres managés</span><span class="sxs-lookup"><span data-stu-id="217ac-213">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="217ac-214">Ajout d’un indicateur de non-format pour l’affichage des journaux de génération</span><span class="sxs-lookup"><span data-stu-id="217ac-214">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="217ac-215">ACS</span><span class="sxs-lookup"><span data-stu-id="217ac-215">ACS</span></span>
* <span data-ttu-id="217ac-216">Modification de la commande `install-connector` pour configurer le nom de domaine complet maître AKS</span><span class="sxs-lookup"><span data-stu-id="217ac-216">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="217ac-217">Correction de la création d’attribution de rôle pour vnet-subnet-id lorsque le principal de service n’est pas spécifié, et pour skip-role-assignemnt</span><span class="sxs-lookup"><span data-stu-id="217ac-217">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="217ac-218">AppService</span><span class="sxs-lookup"><span data-stu-id="217ac-218">AppService</span></span>

* <span data-ttu-id="217ac-219">Ajout de la prise en charge de la gestion des opérations (continues et déclenchées) des Webjobs</span><span class="sxs-lookup"><span data-stu-id="217ac-219">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="217ac-220">az webapp config set prend en charge la propriété FTS-state. Aussi ajout de la prise en charge de az functionapp config set & show</span><span class="sxs-lookup"><span data-stu-id="217ac-220">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="217ac-221">Ajout de la prise en charge de Bring Your Own Storage pour les applications web</span><span class="sxs-lookup"><span data-stu-id="217ac-221">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="217ac-222">Ajout de la prise en charge du référencement et de la restauration des applications web supprimées</span><span class="sxs-lookup"><span data-stu-id="217ac-222">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="217ac-223">Batch</span><span class="sxs-lookup"><span data-stu-id="217ac-223">Batch</span></span>
* <span data-ttu-id="217ac-224">Modification de l’ajout des tâches via `--json-file` pour prendre en charge la syntaxe AddTaskCollectionParameter</span><span class="sxs-lookup"><span data-stu-id="217ac-224">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="217ac-225">Mise à jour de la documentation des formats `--json-file` acceptés</span><span class="sxs-lookup"><span data-stu-id="217ac-225">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="217ac-226">Ajout de `--max-tasks-per-node-option` à `batch pool create`</span><span class="sxs-lookup"><span data-stu-id="217ac-226">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="217ac-227">Modification du comportement de `batch account` pour afficher la connexion au compte si aucune option n’est spécifiée</span><span class="sxs-lookup"><span data-stu-id="217ac-227">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="217ac-228">Batch AI</span><span class="sxs-lookup"><span data-stu-id="217ac-228">Batch AI</span></span> 
* <span data-ttu-id="217ac-229">Correction de l’échec de création de compte de stockage automatique dans la commande `batchai cluster create`</span><span class="sxs-lookup"><span data-stu-id="217ac-229">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="217ac-230">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="217ac-230">Cognitive Services</span></span>
* <span data-ttu-id="217ac-231">Ajout de Completer pour les arguments `--sku`, `--kind` et `--location`</span><span class="sxs-lookup"><span data-stu-id="217ac-231">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="217ac-232">Ajout de la commande `cognitiveservices account list-usage`</span><span class="sxs-lookup"><span data-stu-id="217ac-232">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="217ac-233">Ajout de la commande `cognitiveservices account list-kinds`</span><span class="sxs-lookup"><span data-stu-id="217ac-233">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="217ac-234">Ajout de la commande `cognitiveservices account list`</span><span class="sxs-lookup"><span data-stu-id="217ac-234">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="217ac-235">`cognitiveservices list` déconseillé</span><span class="sxs-lookup"><span data-stu-id="217ac-235">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="217ac-236">Modification de `--name` afin de le rendre facultatif pour `cognitiveservices account list-skus`</span><span class="sxs-lookup"><span data-stu-id="217ac-236">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="217ac-237">Conteneur</span><span class="sxs-lookup"><span data-stu-id="217ac-237">Container</span></span>
* <span data-ttu-id="217ac-238">Ajout de la possibilité de redémarrer et d’arrêter un groupe de conteneurs en cours d’exécution</span><span class="sxs-lookup"><span data-stu-id="217ac-238">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="217ac-239">Ajout de `--network-profile` pour autoriser le passage dans un profil réseau</span><span class="sxs-lookup"><span data-stu-id="217ac-239">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="217ac-240">Ajout de `--subnet` et `--vnet_name` pour autoriser la création de groupes de conteneurs dans un réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="217ac-240">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="217ac-241">Modification de la sortie de table pour afficher l’état du groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="217ac-241">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="217ac-242">DataLake</span><span class="sxs-lookup"><span data-stu-id="217ac-242">Datalake</span></span>
* <span data-ttu-id="217ac-243">Ajout de commandes pour les règles de réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="217ac-243">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="217ac-244">Shell interactif</span><span class="sxs-lookup"><span data-stu-id="217ac-244">Interactive Shell</span></span>
* <span data-ttu-id="217ac-245">Correction des erreurs sur Windows où les commandes ne s’exécutent pas correctement</span><span class="sxs-lookup"><span data-stu-id="217ac-245">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="217ac-246">Correction du problème de chargement de commande dans le Shell interactif provoqué par les objets déconseillés</span><span class="sxs-lookup"><span data-stu-id="217ac-246">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="217ac-247">IoT</span><span class="sxs-lookup"><span data-stu-id="217ac-247">IoT</span></span>
* <span data-ttu-id="217ac-248">Ajout de la prise en charge du routage des hubs IoT</span><span class="sxs-lookup"><span data-stu-id="217ac-248">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="217ac-249">Key Vault</span><span class="sxs-lookup"><span data-stu-id="217ac-249">Key Vault</span></span>
* <span data-ttu-id="217ac-250">Correction de l’importation de la clé Key Vault pour les clés RSA</span><span class="sxs-lookup"><span data-stu-id="217ac-250">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="217ac-251">Réseau</span><span class="sxs-lookup"><span data-stu-id="217ac-251">Network</span></span>
* <span data-ttu-id="217ac-252">Ajout des commandes `network public-ip prefix` pour prendre en charge les fonctionnalités de préfixes d’adresses IP publiques</span><span class="sxs-lookup"><span data-stu-id="217ac-252">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="217ac-253">Ajout des commandes `network service-endpoint` pour prendre en charge les fonctionnalités de stratégie de point de terminaison de service</span><span class="sxs-lookup"><span data-stu-id="217ac-253">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="217ac-254">Ajout des commandes `network lb outbound-rule` pour prendre en charge la création de règles de trafic sortant d’un équilibreur de charge standard</span><span class="sxs-lookup"><span data-stu-id="217ac-254">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="217ac-255">Ajout de `--public-ip-prefix` à `network lb frontend-ip create/update` pour prendre en charge les configurations IP frontales à l’aide de préfixes d’adresses IP publiques</span><span class="sxs-lookup"><span data-stu-id="217ac-255">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="217ac-256">Ajout de `--enable-tcp-reset` à `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span><span class="sxs-lookup"><span data-stu-id="217ac-256">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="217ac-257">Ajout de `--disable-outbound-snat` à `network lb rule create/update`</span><span class="sxs-lookup"><span data-stu-id="217ac-257">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="217ac-258">Autoriser `network watcher flow-log show/configure` à être utilisé avec des groupes de sécurité réseau classiques</span><span class="sxs-lookup"><span data-stu-id="217ac-258">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="217ac-259">Ajouter la commande `network watcher run-configuration-diagnostic`</span><span class="sxs-lookup"><span data-stu-id="217ac-259">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="217ac-260">Correction de la commande `network watcher test-connectivity` et ajout des propriétés `--method`, `--valid-status-codes` et `--headers`</span><span class="sxs-lookup"><span data-stu-id="217ac-260">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="217ac-261">`network express-route create/update` : ajout de l’indicateur `--allow-global-reach`</span><span class="sxs-lookup"><span data-stu-id="217ac-261">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="217ac-262">`network vnet subnet create/update` : ajout de la prise en charge de `--delegation`</span><span class="sxs-lookup"><span data-stu-id="217ac-262">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="217ac-263">Ajout de la commande `network vnet subnet list-available-delegations`</span><span class="sxs-lookup"><span data-stu-id="217ac-263">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="217ac-264">`network traffic-manager profile create/update` : ajout de la prise en charge de `--interval`, `--timeout` et `--max-failures` pour les options Deprecated de configuration du moniteur `--monitor-path`, `--monitor-port` et `--monitor-protocol` en faveur de `--path`, `--port`, `--protocol`</span><span class="sxs-lookup"><span data-stu-id="217ac-264">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="217ac-265">`network lb frontend-ip create/update` : correction de la logique de réglage de la méthode d’allocation d’adresses IP privées. Si une adresse IP privée est fournie, l’allocation sera statique. Si aucune adresse IP privée n’est fournie, ou qu’une chaîne vide est fournie pour l’adresse IP privée, l’allocation est dynamique.</span><span class="sxs-lookup"><span data-stu-id="217ac-265">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="217ac-266">`dns record-set * create/update` : ajout de la prise en charge de `--target-resource`</span><span class="sxs-lookup"><span data-stu-id="217ac-266">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="217ac-267">Ajout des commandes `network interface-endpoint` pour interroger les objets de point de terminaison de l’interface</span><span class="sxs-lookup"><span data-stu-id="217ac-267">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="217ac-268">Ajout de `network profile show/list/delete` pour la gestion partielle des profils de réseau</span><span class="sxs-lookup"><span data-stu-id="217ac-268">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="217ac-269">Ajout des commandes `network express-route peering connection` pour gérer les connexions d’appairage entre les routes ExpressRoutes</span><span class="sxs-lookup"><span data-stu-id="217ac-269">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="217ac-270">SGBDR</span><span class="sxs-lookup"><span data-stu-id="217ac-270">RDBMS</span></span>
* <span data-ttu-id="217ac-271">Ajout de la prise en charge du service MariaDB</span><span class="sxs-lookup"><span data-stu-id="217ac-271">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="217ac-272">Réservation</span><span class="sxs-lookup"><span data-stu-id="217ac-272">Reservation</span></span>
* <span data-ttu-id="217ac-273">Ajout de CosmosDb dans le type d’énumération des ressources réservées</span><span class="sxs-lookup"><span data-stu-id="217ac-273">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="217ac-274">Ajout de la propriété de nom dans un modèle Patch</span><span class="sxs-lookup"><span data-stu-id="217ac-274">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="217ac-275">Gérer l’application</span><span class="sxs-lookup"><span data-stu-id="217ac-275">Manage App</span></span>
* <span data-ttu-id="217ac-276">Correction du bogue dans `managedapp create --kind MarketPlace` à l’origine du blocage de la création d’instance d’une application Marketplace gérée</span><span class="sxs-lookup"><span data-stu-id="217ac-276">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="217ac-277">Modification des commandes `feature` afin qu’elles soient limitées aux profils pris en charge</span><span class="sxs-lookup"><span data-stu-id="217ac-277">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="217ac-278">Rôle</span><span class="sxs-lookup"><span data-stu-id="217ac-278">Role</span></span>
* <span data-ttu-id="217ac-279">Ajout de la prise en charge pour répertorier les appartenances de l’utilisateur à des groupes</span><span class="sxs-lookup"><span data-stu-id="217ac-279">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="217ac-280">SignalR</span><span class="sxs-lookup"><span data-stu-id="217ac-280">SignalR</span></span>
* <span data-ttu-id="217ac-281">Première version</span><span class="sxs-lookup"><span data-stu-id="217ac-281">First release</span></span>

### <a name="storage"></a><span data-ttu-id="217ac-282">Stockage</span><span class="sxs-lookup"><span data-stu-id="217ac-282">Storage</span></span>
* <span data-ttu-id="217ac-283">Ajout du paramètre `--auth-mode login` pour l’utilisation des informations d’identification de l’utilisateur pour autoriser les objets blob et les files d’attente</span><span class="sxs-lookup"><span data-stu-id="217ac-283">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="217ac-284">Ajout de `storage container immutability-policy/legal-hold` pour gérer le stockage immuable</span><span class="sxs-lookup"><span data-stu-id="217ac-284">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="217ac-285">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="217ac-285">VM</span></span>
* <span data-ttu-id="217ac-286">Correction d’un problème `vm create --generate-ssh-keys` qui remplace le fichier de clé privée si le fichier de clé publique est manquant (#4725, #6780)</span><span class="sxs-lookup"><span data-stu-id="217ac-286">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="217ac-287">Ajout de la prise en charge pour la galerie d’images partagée via `az sig`</span><span class="sxs-lookup"><span data-stu-id="217ac-287">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="217ac-288">28 Août 2018</span><span class="sxs-lookup"><span data-stu-id="217ac-288">August 28, 2018</span></span>

<span data-ttu-id="217ac-289">Version 2.0.45</span><span class="sxs-lookup"><span data-stu-id="217ac-289">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="217ac-290">Principal</span><span class="sxs-lookup"><span data-stu-id="217ac-290">Core</span></span>

* <span data-ttu-id="217ac-291">Résolution du problème de chargement de fichier de configuration vide</span><span class="sxs-lookup"><span data-stu-id="217ac-291">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="217ac-292">Ajout de la prise en charge du profil `2018-03-01-hybrid` pour Azure Stack</span><span class="sxs-lookup"><span data-stu-id="217ac-292">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="217ac-293">ACR</span><span class="sxs-lookup"><span data-stu-id="217ac-293">ACR</span></span>

* <span data-ttu-id="217ac-294">Ajout d’une solution pour les opérations d’exécution sans les requêtes ARM</span><span class="sxs-lookup"><span data-stu-id="217ac-294">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="217ac-295">Exclusion des fichiers de contrôle de version (par exemple, .git, .gitignore) chargés par défaut dans les fichiers tar dans la commande `build`</span><span class="sxs-lookup"><span data-stu-id="217ac-295">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="217ac-296">ACS</span><span class="sxs-lookup"><span data-stu-id="217ac-296">ACS</span></span>

* <span data-ttu-id="217ac-297">Modification de `aks create` à la valeur par défaut sur les machines virtuelles `Standard_DS2_v2`</span><span class="sxs-lookup"><span data-stu-id="217ac-297">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="217ac-298">Modification de `aks get-credentials` afin d’appeler de nouvelles API pour l’obtention des informations d’identification des clusters</span><span class="sxs-lookup"><span data-stu-id="217ac-298">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="217ac-299">AppService</span><span class="sxs-lookup"><span data-stu-id="217ac-299">AppService</span></span>

* <span data-ttu-id="217ac-300">Prise en charge de CORS sur functionapp et webapp</span><span class="sxs-lookup"><span data-stu-id="217ac-300">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="217ac-301">Ajout de la prise en charge de la balise ARM sur les commandes de création</span><span class="sxs-lookup"><span data-stu-id="217ac-301">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="217ac-302">Modification de `[webapp|functionapp] identity show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="217ac-302">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="217ac-303">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="217ac-303">Backup</span></span>

* <span data-ttu-id="217ac-304">Modification de `backup vault backup-properties show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="217ac-304">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="217ac-305">Service de robot</span><span class="sxs-lookup"><span data-stu-id="217ac-305">Bot Service</span></span>

* <span data-ttu-id="217ac-306">Version initiale de l’interface CLI de Bot Service</span><span class="sxs-lookup"><span data-stu-id="217ac-306">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="217ac-307">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="217ac-307">Cognitive Services</span></span>

* <span data-ttu-id="217ac-308">Ajout du nouveau paramètre `--api-properties,` requis pour la création de certains services</span><span class="sxs-lookup"><span data-stu-id="217ac-308">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="217ac-309">IoT</span><span class="sxs-lookup"><span data-stu-id="217ac-309">IoT</span></span>

* <span data-ttu-id="217ac-310">Résolution du problème relatif à l’association de hubs liés</span><span class="sxs-lookup"><span data-stu-id="217ac-310">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="217ac-311">Surveiller</span><span class="sxs-lookup"><span data-stu-id="217ac-311">Monitor</span></span>

* <span data-ttu-id="217ac-312">Ajout des commandes `monitor metrics alert` permettant de recevoir des alertes sur les métriques quasiment en temps réel</span><span class="sxs-lookup"><span data-stu-id="217ac-312">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="217ac-313">Commandes `monitor alert` déconseillées</span><span class="sxs-lookup"><span data-stu-id="217ac-313">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="217ac-314">Réseau</span><span class="sxs-lookup"><span data-stu-id="217ac-314">Network</span></span>

* <span data-ttu-id="217ac-315">Modification de `network application-gateway ssl-policy predefined show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="217ac-315">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="217ac-316">Ressource</span><span class="sxs-lookup"><span data-stu-id="217ac-316">Resource</span></span>

* <span data-ttu-id="217ac-317">Modification de `provider operation show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="217ac-317">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="217ac-318">Stockage</span><span class="sxs-lookup"><span data-stu-id="217ac-318">Storage</span></span>

* <span data-ttu-id="217ac-319">Modification de `storage share policy show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="217ac-319">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="217ac-320">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="217ac-320">VM</span></span>

* <span data-ttu-id="217ac-321">Modification de `vm/vmss identity show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="217ac-321">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="217ac-322">Remplacement de `--storage-caching` pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="217ac-322">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="217ac-323">14 août 2018</span><span class="sxs-lookup"><span data-stu-id="217ac-323">Auguest 14, 2018</span></span>

<span data-ttu-id="217ac-324">Version 2.0.44</span><span class="sxs-lookup"><span data-stu-id="217ac-324">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="217ac-325">Principal</span><span class="sxs-lookup"><span data-stu-id="217ac-325">Core</span></span>

* <span data-ttu-id="217ac-326">Correction de l’affichage numérique dans la sortie `table`</span><span class="sxs-lookup"><span data-stu-id="217ac-326">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="217ac-327">Ajout du format de sortie YAML</span><span class="sxs-lookup"><span data-stu-id="217ac-327">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="217ac-328">Télémétrie</span><span class="sxs-lookup"><span data-stu-id="217ac-328">Telemetry</span></span>

* <span data-ttu-id="217ac-329">Amélioration des rapports de télémétrie</span><span class="sxs-lookup"><span data-stu-id="217ac-329">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="217ac-330">ACR</span><span class="sxs-lookup"><span data-stu-id="217ac-330">ACR</span></span>

* <span data-ttu-id="217ac-331">Ajout des commandes `content-trust policy`</span><span class="sxs-lookup"><span data-stu-id="217ac-331">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="217ac-332">Résolution du problème où `.dockerignore` n’était pas honorée</span><span class="sxs-lookup"><span data-stu-id="217ac-332">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="217ac-333">ACS</span><span class="sxs-lookup"><span data-stu-id="217ac-333">ACS</span></span>

* <span data-ttu-id="217ac-334">Modification de `az acs/aks install-cli` afin d’effectuer l’installation sous `%USERPROFILE%\.azure-kubectl` sur Windows</span><span class="sxs-lookup"><span data-stu-id="217ac-334">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="217ac-335">Modification de `az aks install-connector` afin de détecter si le cluster dispose du contrôle RBAC et de configurer le connecteur ACI correctement</span><span class="sxs-lookup"><span data-stu-id="217ac-335">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="217ac-336">Remplacement par l’attribution de rôle au sous-réseau lorsque l’attribution est fournie</span><span class="sxs-lookup"><span data-stu-id="217ac-336">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="217ac-337">Ajout de l’option nouveau « ignorer attribution de rôle » pour le sous-réseau lorsque l’attribution est fournie</span><span class="sxs-lookup"><span data-stu-id="217ac-337">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="217ac-338">Modification ignorant l’attribution de rôle au sous-réseau lorsque l’attribution existe déjà</span><span class="sxs-lookup"><span data-stu-id="217ac-338">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="217ac-339">AppService</span><span class="sxs-lookup"><span data-stu-id="217ac-339">AppService</span></span>

* <span data-ttu-id="217ac-340">Correction d’un bogue empêchant de créer une application de fonction à l’aide de comptes de stockage dans les groupes de ressources externes</span><span class="sxs-lookup"><span data-stu-id="217ac-340">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="217ac-341">Correction d’un incident lors du déploiement de dossier zip</span><span class="sxs-lookup"><span data-stu-id="217ac-341">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="217ac-342">Batch AI</span><span class="sxs-lookup"><span data-stu-id="217ac-342">BatchAI</span></span>

* <span data-ttu-id="217ac-343">Modification de la sortie de l’enregistreur d’événements pour la création du compte de stockage automatique afin de spécifier l’information « ressource *groupe*».</span><span class="sxs-lookup"><span data-stu-id="217ac-343">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="217ac-344">Conteneur</span><span class="sxs-lookup"><span data-stu-id="217ac-344">Container</span></span>

* <span data-ttu-id="217ac-345">Ajout de `--secure-environment-variables` pour transmettre des variables d’environnement sécurisées vers un conteneur</span><span class="sxs-lookup"><span data-stu-id="217ac-345">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="217ac-346">IoT</span><span class="sxs-lookup"><span data-stu-id="217ac-346">IoT</span></span>

* <span data-ttu-id="217ac-347">[CHANGEMENT CASSANT] Suppression des commandes obsolètes déplacées vers l’extension iot</span><span class="sxs-lookup"><span data-stu-id="217ac-347">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="217ac-348">Mise à jour des éléments afin de ne pas prendre en compte le domaine `azure-devices.net`</span><span class="sxs-lookup"><span data-stu-id="217ac-348">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="217ac-349">Iot Central</span><span class="sxs-lookup"><span data-stu-id="217ac-349">Iot Central</span></span>

* <span data-ttu-id="217ac-350">Version initiale du module IoT Central</span><span class="sxs-lookup"><span data-stu-id="217ac-350">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="217ac-351">KeyVault</span><span class="sxs-lookup"><span data-stu-id="217ac-351">KeyVault</span></span>


* <span data-ttu-id="217ac-352">Ajout des commandes pour la gestion des comptes de stockage et les définitions SAS</span><span class="sxs-lookup"><span data-stu-id="217ac-352">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="217ac-353">Ajout de commandes pour les règles réseau</span><span class="sxs-lookup"><span data-stu-id="217ac-353">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="217ac-354">Ajout du paramètre `--id` aux opérations relatives aux mots de passe confidentiels, clés et certificats</span><span class="sxs-lookup"><span data-stu-id="217ac-354">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="217ac-355">Ajout de la prise en charge pour la version multi-api avec gestion des coffres de clés</span><span class="sxs-lookup"><span data-stu-id="217ac-355">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="217ac-356">Ajout de la prise en charge pour la version multi-api avec plan de données des coffres de clés</span><span class="sxs-lookup"><span data-stu-id="217ac-356">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="217ac-357">Relais</span><span class="sxs-lookup"><span data-stu-id="217ac-357">Relay</span></span>

* <span data-ttu-id="217ac-358">Version initiale</span><span class="sxs-lookup"><span data-stu-id="217ac-358">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="217ac-359">SQL</span><span class="sxs-lookup"><span data-stu-id="217ac-359">Sql</span></span>

* <span data-ttu-id="217ac-360">Ajout des commandes `sql failover-group`</span><span class="sxs-lookup"><span data-stu-id="217ac-360">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="217ac-361">Stockage</span><span class="sxs-lookup"><span data-stu-id="217ac-361">Storage</span></span>

* <span data-ttu-id="217ac-362">[CHANGEMENT CASSANT] Modification de `storage account show-usage` afin d’exiger le paramètre `--location` et de répertorier par région</span><span class="sxs-lookup"><span data-stu-id="217ac-362">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="217ac-363">Modification du paramètre `--resource-group` afin de le rendre facultatif pour les commandes `storage account`</span><span class="sxs-lookup"><span data-stu-id="217ac-363">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="217ac-364">Suppression des avertissements concernant l’échec de la condition préalable pour les défaillances isolées dans les commandes batch pour les messages agrégés uniques</span><span class="sxs-lookup"><span data-stu-id="217ac-364">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="217ac-365">Modification des commandes `[blob|file] delete-batch` afin de ne plus produire des tableaux ayant la valeur null</span><span class="sxs-lookup"><span data-stu-id="217ac-365">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="217ac-366">Modification des commandes `blob [download|upload|delete-batch]` afin de lire le jeton de SAS à partir de l’url du conteneur</span><span class="sxs-lookup"><span data-stu-id="217ac-366">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="217ac-367">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="217ac-367">VM</span></span>

* <span data-ttu-id="217ac-368">Ajout des filtres courants à `vm list-skus` pour une plus grande simplicité d’utilisation</span><span class="sxs-lookup"><span data-stu-id="217ac-368">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="217ac-369">31 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="217ac-369">July 31, 2018</span></span>

<span data-ttu-id="217ac-370">Version 2.0.43</span><span class="sxs-lookup"><span data-stu-id="217ac-370">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="217ac-371">ACR</span><span class="sxs-lookup"><span data-stu-id="217ac-371">ACR</span></span>

* <span data-ttu-id="217ac-372">Ajout de l’indicateur `--with-secure-properties` à la commande `acr build-task show`</span><span class="sxs-lookup"><span data-stu-id="217ac-372">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="217ac-373">Ajout de la commande `acr build-task update-build`</span><span class="sxs-lookup"><span data-stu-id="217ac-373">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="217ac-374">ACS</span><span class="sxs-lookup"><span data-stu-id="217ac-374">ACS</span></span>

* <span data-ttu-id="217ac-375">Retour au return 0 (réussite) à la fin de `az aks browse` en appuyant sur [Ctrl + C]</span><span class="sxs-lookup"><span data-stu-id="217ac-375">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="217ac-376">Batch</span><span class="sxs-lookup"><span data-stu-id="217ac-376">Batch</span></span>

* <span data-ttu-id="217ac-377">Correction du bug lors de l’affichage des jetons AAD dans le Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="217ac-377">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="217ac-378">Conteneur</span><span class="sxs-lookup"><span data-stu-id="217ac-378">Container</span></span>

* <span data-ttu-id="217ac-379">Suppression de l’exigence pour `--log-analytics-workspace-key` pour le nom ou l’identifiant lors de l’abonnement standard</span><span class="sxs-lookup"><span data-stu-id="217ac-379">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="217ac-380">Réseau</span><span class="sxs-lookup"><span data-stu-id="217ac-380">Network</span></span>

* <span data-ttu-id="217ac-381">Ajout du serveur DNS au profil du 09/03/2017 pour Azure Stack</span><span class="sxs-lookup"><span data-stu-id="217ac-381">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="217ac-382">Ressource</span><span class="sxs-lookup"><span data-stu-id="217ac-382">Resource</span></span>

* <span data-ttu-id="217ac-383">Ajout de `--rollback-on-error` à `group deployment create` pour exécuter un déploiement correct et connu en cas d’erreur</span><span class="sxs-lookup"><span data-stu-id="217ac-383">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="217ac-384">Correction d’un problème où `--parameters {}` avec `group deployment create` entraînait une erreur</span><span class="sxs-lookup"><span data-stu-id="217ac-384">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="217ac-385">Rôle</span><span class="sxs-lookup"><span data-stu-id="217ac-385">Role</span></span>

* <span data-ttu-id="217ac-386">Ajout de la prise en charge du profil stack du 09/03/2017</span><span class="sxs-lookup"><span data-stu-id="217ac-386">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="217ac-387">Correction d’un problème où les paramètres de mise à jour génériques à `app update` ne fonctionnaient pas correctement</span><span class="sxs-lookup"><span data-stu-id="217ac-387">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="217ac-388">Recherche</span><span class="sxs-lookup"><span data-stu-id="217ac-388">Search</span></span>

* <span data-ttu-id="217ac-389">Ajout de commandes pour le service de recherches d’Azure</span><span class="sxs-lookup"><span data-stu-id="217ac-389">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="217ac-390">Service Bus</span><span class="sxs-lookup"><span data-stu-id="217ac-390">Service Bus</span></span>

* <span data-ttu-id="217ac-391">Ajout d’un groupe de commandes de migration pour migrer un espace de noms d’un Service Bus Standard à un Premium</span><span class="sxs-lookup"><span data-stu-id="217ac-391">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="217ac-392">Ajout de nouvelles propriétés facultatives à la file d’attente du Service Bus et à l’abonnement</span><span class="sxs-lookup"><span data-stu-id="217ac-392">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="217ac-393">`--enable-batched-operations` et `--enable-dead-lettering-on-message-expiration` dans `queue`</span><span class="sxs-lookup"><span data-stu-id="217ac-393">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="217ac-394">`--dead-letter-on-filter-exceptions` dans `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="217ac-394">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="217ac-395">Stockage</span><span class="sxs-lookup"><span data-stu-id="217ac-395">Storage</span></span>

* <span data-ttu-id="217ac-396">Ajout de la prise en charge du téléchargement de fichiers volumineux à l’aide d’une connexion unique</span><span class="sxs-lookup"><span data-stu-id="217ac-396">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="217ac-397">Conversion des commandes `show` qui manquaient d’échouer avec le code de sortie 3 sur une ressource manquante</span><span class="sxs-lookup"><span data-stu-id="217ac-397">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="217ac-398">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="217ac-398">VM</span></span>

* <span data-ttu-id="217ac-399">Ajout d’une prise en charge pour lister les groupes disponibles par abonnement</span><span class="sxs-lookup"><span data-stu-id="217ac-399">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="217ac-400">Ajout de la prise en charge de `StandardSSD_LRS`</span><span class="sxs-lookup"><span data-stu-id="217ac-400">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="217ac-401">Ajout d’une prise en charge des groupes de sécurité d’application dans la création du groupe identique de machines virtuelles</span><span class="sxs-lookup"><span data-stu-id="217ac-401">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="217ac-402">[CHANGEMENT CASSANT] Changement de `[vm|vmss] create`, `[vm|vmss] identity assign`, et `[vm|vmss] identity remove` pour sortir les identités des utilisateurs au format de dictionnaire</span><span class="sxs-lookup"><span data-stu-id="217ac-402">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="217ac-403">18 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="217ac-403">July 18, 2018</span></span>

<span data-ttu-id="217ac-404">Version 2.0.42</span><span class="sxs-lookup"><span data-stu-id="217ac-404">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="217ac-405">Principal</span><span class="sxs-lookup"><span data-stu-id="217ac-405">Core</span></span>

* <span data-ttu-id="217ac-406">Ajout de la prise en charge de la connexion basée sur le navigateur dans la fenêtre d’interpréteur de commandes Windows pour Linux</span><span class="sxs-lookup"><span data-stu-id="217ac-406">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="217ac-407">Ajout de l’indicateur `--force-string` pour toutes les commandes de mise à jour générique</span><span class="sxs-lookup"><span data-stu-id="217ac-407">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="217ac-408">[CHANGEMENT CASSANT] Modification des commandes « d’affichage » pour connecter le message d’erreur et échec avec un code de sortie de 3 sur une ressource manquante</span><span class="sxs-lookup"><span data-stu-id="217ac-408">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="217ac-409">ACR</span><span class="sxs-lookup"><span data-stu-id="217ac-409">ACR</span></span>

* <span data-ttu-id="217ac-410">[CHANGEMENT CASSANT] Mise à jour de « --no-push » vers un indicateur pur dans la commande « ACR Build »</span><span class="sxs-lookup"><span data-stu-id="217ac-410">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="217ac-411">Ajout des commandes `show` et `update` sous le groupe `acr repository`</span><span class="sxs-lookup"><span data-stu-id="217ac-411">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="217ac-412">Ajout de l’indicateur `--detail` à `show-manifests` et `show-tags` pour afficher des informations plus détaillées</span><span class="sxs-lookup"><span data-stu-id="217ac-412">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="217ac-413">Ajout du paramètre `--image` pour prendre en charge l’obtention des détails de build ou des journaux par une image</span><span class="sxs-lookup"><span data-stu-id="217ac-413">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="217ac-414">ACS</span><span class="sxs-lookup"><span data-stu-id="217ac-414">ACS</span></span>

* <span data-ttu-id="217ac-415">Modification de `az aks create` en sortie d’erreur si `--max-pods` est inférieur à 5</span><span class="sxs-lookup"><span data-stu-id="217ac-415">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="217ac-416">AppService</span><span class="sxs-lookup"><span data-stu-id="217ac-416">AppService</span></span>

* <span data-ttu-id="217ac-417">Ajout de la prise en charge pour les références (SKU) PremiumV2</span><span class="sxs-lookup"><span data-stu-id="217ac-417">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="217ac-418">Batch</span><span class="sxs-lookup"><span data-stu-id="217ac-418">Batch</span></span>

* <span data-ttu-id="217ac-419">Correction d’un bogue relatif à l’utilisation des informations d’identification de jeton dans le mode Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="217ac-419">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="217ac-420">Modification de l’entrée JSON pour respecter la casse</span><span class="sxs-lookup"><span data-stu-id="217ac-420">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="217ac-421">Batch AI</span><span class="sxs-lookup"><span data-stu-id="217ac-421">Batch AI</span></span>

* <span data-ttu-id="217ac-422">Correction de la commande `az batchai job exec`</span><span class="sxs-lookup"><span data-stu-id="217ac-422">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="217ac-423">Conteneur</span><span class="sxs-lookup"><span data-stu-id="217ac-423">Container</span></span>

* <span data-ttu-id="217ac-424">Suppression des exigences pour le nom d’utilisateur et le mot de passe pour les registres non dockerhub</span><span class="sxs-lookup"><span data-stu-id="217ac-424">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="217ac-425">Correction de l’erreur lors de la création de groupes de conteneur à partir du fichier yaml</span><span class="sxs-lookup"><span data-stu-id="217ac-425">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="217ac-426">Réseau</span><span class="sxs-lookup"><span data-stu-id="217ac-426">Network</span></span>

* <span data-ttu-id="217ac-427">Ajout de la prise en charge de `--no-wait` pour `network nic [create|update|delete]`</span><span class="sxs-lookup"><span data-stu-id="217ac-427">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="217ac-428">Ajout de `network nic wait`</span><span class="sxs-lookup"><span data-stu-id="217ac-428">Added `network nic wait`</span></span>
* <span data-ttu-id="217ac-429">Argument `--ids` déconseillé pour `network vnet [subnet|peering] list`</span><span class="sxs-lookup"><span data-stu-id="217ac-429">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="217ac-430">Ajout de l’indicateur `--include-default` pour inclure les règles de sécurité par défaut dans la sortie de `network nsg rule list`</span><span class="sxs-lookup"><span data-stu-id="217ac-430">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="217ac-431">Ressource</span><span class="sxs-lookup"><span data-stu-id="217ac-431">Resource</span></span>

* <span data-ttu-id="217ac-432">Ajout de la prise en charge de `--no-wait` pour `group deployment delete`</span><span class="sxs-lookup"><span data-stu-id="217ac-432">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="217ac-433">Ajout de la prise en charge de `--no-wait` pour `deployment delete`</span><span class="sxs-lookup"><span data-stu-id="217ac-433">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="217ac-434">Ajout de la commande `deployment wait`</span><span class="sxs-lookup"><span data-stu-id="217ac-434">Added `deployment wait` command</span></span>
* <span data-ttu-id="217ac-435">Résolution du problème qui causait l’affichage par erreur des commandes `az deployment` du niveau de l’abonnement pour le profil 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="217ac-435">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="217ac-436">SQL</span><span class="sxs-lookup"><span data-stu-id="217ac-436">SQL</span></span>

* <span data-ttu-id="217ac-437">Résolution de l’erreur « Le nom du groupe de ressources fourni ne correspond pas au nom de l’URL » lors de la spécification du nom du pool élastique pour les commandes `sql db copy` et `sql db replica create`</span><span class="sxs-lookup"><span data-stu-id="217ac-437">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="217ac-438">Autoriser la configuration de SQL Server par défaut en exécutant `az configure --defaults sql-server=<name>`</span><span class="sxs-lookup"><span data-stu-id="217ac-438">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="217ac-439">Implémentation de formateurs de table pour les commandes `sql server`, `sql server firewall-rule`, `sql list-usages` et `sql show-usage`</span><span class="sxs-lookup"><span data-stu-id="217ac-439">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="217ac-440">Stockage</span><span class="sxs-lookup"><span data-stu-id="217ac-440">Storage</span></span>

* <span data-ttu-id="217ac-441">Ajout de la propriété `pageRanges` à la sortie `storage blob show` qui sera renseignée pour les objets blob de pages</span><span class="sxs-lookup"><span data-stu-id="217ac-441">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="217ac-442">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="217ac-442">VM</span></span>

* <span data-ttu-id="217ac-443">[CHANGEMENT CASSANT] Modification de `vmss create` pour utiliser `Standard_DS1_v2` comme taille d’instance par défaut</span><span class="sxs-lookup"><span data-stu-id="217ac-443">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="217ac-444">Ajout de la prise en charge de `--no-wait` pour `vm extension [set|delete]` et `vmss extension [set|delete]`</span><span class="sxs-lookup"><span data-stu-id="217ac-444">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="217ac-445">Ajout de `vm extension wait`</span><span class="sxs-lookup"><span data-stu-id="217ac-445">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="217ac-446">3 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="217ac-446">July 3, 2018</span></span>

<span data-ttu-id="217ac-447">Version 2.0.41</span><span class="sxs-lookup"><span data-stu-id="217ac-447">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="217ac-448">AKS</span><span class="sxs-lookup"><span data-stu-id="217ac-448">AKS</span></span>

* <span data-ttu-id="217ac-449">Modification de la surveillance pour utiliser l’ID d’abonnement</span><span class="sxs-lookup"><span data-stu-id="217ac-449">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="217ac-450">3 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="217ac-450">July 3, 2018</span></span>

<span data-ttu-id="217ac-451">Version 2.0.40</span><span class="sxs-lookup"><span data-stu-id="217ac-451">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="217ac-452">Principal</span><span class="sxs-lookup"><span data-stu-id="217ac-452">Core</span></span>

* <span data-ttu-id="217ac-453">Ajout d’un nouveau flux de code d’autorisation pour une connexion interactive</span><span class="sxs-lookup"><span data-stu-id="217ac-453">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="217ac-454">ACR</span><span class="sxs-lookup"><span data-stu-id="217ac-454">ACR</span></span>

* <span data-ttu-id="217ac-455">Ajout de l’interrogation de l’état du build</span><span class="sxs-lookup"><span data-stu-id="217ac-455">Added polling build status</span></span>
* <span data-ttu-id="217ac-456">Ajout de la prise en charge des valeurs d’énumération ne respectant pas la casse</span><span class="sxs-lookup"><span data-stu-id="217ac-456">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="217ac-457">Ajout des paramètres `--top` et `--orderby` pour `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="217ac-457">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="217ac-458">ACS</span><span class="sxs-lookup"><span data-stu-id="217ac-458">ACS</span></span>

* <span data-ttu-id="217ac-459">[CHANGEMENT CASSANT] Active le contrôle d’accès en fonction du rôle Kubernetes par défaut</span><span class="sxs-lookup"><span data-stu-id="217ac-459">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="217ac-460">Ajout de l’argument `--disable-rbac` et dépréciation de `--enable-rbac` dans la mesure où il s’agit actuellement de la valeur par défaut</span><span class="sxs-lookup"><span data-stu-id="217ac-460">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="217ac-461">Mise à jour des options de la commande `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="217ac-461">Updated options for `aks browse` command.</span></span> <span data-ttu-id="217ac-462">Ajout de la prise en charge de `--listen-port`</span><span class="sxs-lookup"><span data-stu-id="217ac-462">Added `--listen-port` support</span></span>
* <span data-ttu-id="217ac-463">Mise à jour du package de graphique Helm par défaut pour la commande `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="217ac-463">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="217ac-464">Use virtual-kubelet-for-aks-latest.tgz</span><span class="sxs-lookup"><span data-stu-id="217ac-464">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="217ac-465">Ajout des commandes `aks enable-addons` et `aks disable-addons` pour mettre à jour un cluster existant</span><span class="sxs-lookup"><span data-stu-id="217ac-465">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="217ac-466">AppService</span><span class="sxs-lookup"><span data-stu-id="217ac-466">AppService</span></span>

* <span data-ttu-id="217ac-467">Ajout de la prise en charge de la désactivation d’identité via `webapp identity remove`</span><span class="sxs-lookup"><span data-stu-id="217ac-467">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="217ac-468">Suppression de la balise `preview` pour la fonctionnalité Identité</span><span class="sxs-lookup"><span data-stu-id="217ac-468">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="217ac-469">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="217ac-469">Backup</span></span>

* <span data-ttu-id="217ac-470">Mise à jour de la définition du module</span><span class="sxs-lookup"><span data-stu-id="217ac-470">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="217ac-471">Batch AI</span><span class="sxs-lookup"><span data-stu-id="217ac-471">BatchAI</span></span>

* <span data-ttu-id="217ac-472">Correction de la sortie de table pour les commandes `batchai cluster node list` et `batchai job node list`</span><span class="sxs-lookup"><span data-stu-id="217ac-472">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="217ac-473">Cloud</span><span class="sxs-lookup"><span data-stu-id="217ac-473">Cloud</span></span>

* <span data-ttu-id="217ac-474">Ajout du suffixe de serveur `acr login` à la configuration du cloud</span><span class="sxs-lookup"><span data-stu-id="217ac-474">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="217ac-475">Conteneur</span><span class="sxs-lookup"><span data-stu-id="217ac-475">Container</span></span>

* <span data-ttu-id="217ac-476">Modification de `container create` sur valeur par défaut en opération à long terme</span><span class="sxs-lookup"><span data-stu-id="217ac-476">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="217ac-477">Ajout des paramètres Log Analytics `--log-analytics-workspace` et `--log-analytics-workspace-key`</span><span class="sxs-lookup"><span data-stu-id="217ac-477">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="217ac-478">Ajout du paramètre `--protocol` pour spécifier le protocole réseau à utiliser</span><span class="sxs-lookup"><span data-stu-id="217ac-478">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="217ac-479">Extension</span><span class="sxs-lookup"><span data-stu-id="217ac-479">Extension</span></span>

* <span data-ttu-id="217ac-480">Modification de `extension list-available` pour afficher uniquement les extensions compatibles avec la version CLI</span><span class="sxs-lookup"><span data-stu-id="217ac-480">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="217ac-481">Réseau</span><span class="sxs-lookup"><span data-stu-id="217ac-481">Network</span></span>

* <span data-ttu-id="217ac-482">Résolution du problème où les types d’enregistrement étaient sensibles à la casse pour ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="217ac-482">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="217ac-483">Rdbms</span><span class="sxs-lookup"><span data-stu-id="217ac-483">Rdbms</span></span>

* <span data-ttu-id="217ac-484">Ajout des commandes `[postgres|myql] server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="217ac-484">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="217ac-485">Ressource</span><span class="sxs-lookup"><span data-stu-id="217ac-485">Resource</span></span>

* <span data-ttu-id="217ac-486">Ajout d’un nouveau groupe d’opérations `deployment`</span><span class="sxs-lookup"><span data-stu-id="217ac-486">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="217ac-487">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="217ac-487">VM</span></span>

* <span data-ttu-id="217ac-488">Ajout de la prise en charge de la suppression de l’identité affectée au système</span><span class="sxs-lookup"><span data-stu-id="217ac-488">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="217ac-489">25 juin 2018</span><span class="sxs-lookup"><span data-stu-id="217ac-489">June 25, 2018</span></span>

<span data-ttu-id="217ac-490">Version 2.0.39</span><span class="sxs-lookup"><span data-stu-id="217ac-490">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="217ac-491">Interface de ligne de commande</span><span class="sxs-lookup"><span data-stu-id="217ac-491">CLI</span></span>

* <span data-ttu-id="217ac-492">Mise à jour de la suppression du fichier dans le programme d’installation MSI pour résoudre le problème d’installation de l’extension</span><span class="sxs-lookup"><span data-stu-id="217ac-492">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="217ac-493">19 juin 2018</span><span class="sxs-lookup"><span data-stu-id="217ac-493">June 19, 2018</span></span>

<span data-ttu-id="217ac-494">Version 2.0.38</span><span class="sxs-lookup"><span data-stu-id="217ac-494">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="217ac-495">Principal</span><span class="sxs-lookup"><span data-stu-id="217ac-495">Core</span></span>

* <span data-ttu-id="217ac-496">Ajout de la prise en charge globale de `--subscription` pour la plupart des commandes</span><span class="sxs-lookup"><span data-stu-id="217ac-496">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="217ac-497">ACR</span><span class="sxs-lookup"><span data-stu-id="217ac-497">ACR</span></span>

* <span data-ttu-id="217ac-498">Ajout de `azure-storage-blob` comme dépendance</span><span class="sxs-lookup"><span data-stu-id="217ac-498">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="217ac-499">Modification de la configuration de l’UC par défaut avec `acr build-task create` pour utiliser 2 cœurs</span><span class="sxs-lookup"><span data-stu-id="217ac-499">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="217ac-500">ACS</span><span class="sxs-lookup"><span data-stu-id="217ac-500">ACS</span></span>

* <span data-ttu-id="217ac-501">Mise à jour des options de la commande `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="217ac-501">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="217ac-502">Ajout de la prise en charge de `--update`</span><span class="sxs-lookup"><span data-stu-id="217ac-502">Added `--update` support</span></span>
* <span data-ttu-id="217ac-503">Modification de `aks get-credentials --admin` pour ne pas remplacer le contexte utilisateur dans `$HOME/.kube/config`</span><span class="sxs-lookup"><span data-stu-id="217ac-503">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="217ac-504">Exposition de la propriété en lecture seule `nodeResourceGroup` sur les clusters managés</span><span class="sxs-lookup"><span data-stu-id="217ac-504">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="217ac-505">Correction de l’erreur de commande `acs browse`</span><span class="sxs-lookup"><span data-stu-id="217ac-505">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="217ac-506">`--connector-name` rendu facultatif pour `aks install-connector`, `aks upgrade-connector` et `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="217ac-506">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="217ac-507">Ajout de nouvelles régions Azure Container Instance pour `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="217ac-507">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="217ac-508">Ajout de l’emplacement normalisé dans le nom de mise en production Helm et le nom du nœud pour `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="217ac-508">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="217ac-509">AppService</span><span class="sxs-lookup"><span data-stu-id="217ac-509">AppService</span></span>

* <span data-ttu-id="217ac-510">Ajout de la prise en charge des versions urllib plus récentes</span><span class="sxs-lookup"><span data-stu-id="217ac-510">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="217ac-511">Ajout de la prise en charge pour `functionapp create` pour utiliser un plan App Service à partir de groupes de ressources externes</span><span class="sxs-lookup"><span data-stu-id="217ac-511">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="217ac-512">Batch</span><span class="sxs-lookup"><span data-stu-id="217ac-512">Batch</span></span>

* <span data-ttu-id="217ac-513">Suppression de la dépendance `azure-batch-extensions`</span><span class="sxs-lookup"><span data-stu-id="217ac-513">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="217ac-514">Batch AI</span><span class="sxs-lookup"><span data-stu-id="217ac-514">Batch AI</span></span>

* <span data-ttu-id="217ac-515">Ajout de la prise en charge des espaces de travail.</span><span class="sxs-lookup"><span data-stu-id="217ac-515">Added support for workspaces.</span></span> <span data-ttu-id="217ac-516">Les espaces de travail permettent de regrouper les clusters, serveurs de fichiers et expériences, supprimant la limitation du nombre de ressources qui peuvent être créées</span><span class="sxs-lookup"><span data-stu-id="217ac-516">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="217ac-517">Ajout de la prise en charge des expériences.</span><span class="sxs-lookup"><span data-stu-id="217ac-517">Added support for experiments.</span></span> <span data-ttu-id="217ac-518">Les expériences permettent de regrouper les tâches dans des collections, supprimant la limitation du nombre de tâches créées</span><span class="sxs-lookup"><span data-stu-id="217ac-518">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="217ac-519">Ajout de la prise en charge pour configurer `/dev/shm` pour les travaux en cours d’exécution dans un conteneur docker</span><span class="sxs-lookup"><span data-stu-id="217ac-519">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="217ac-520">Ajout des commandes `batchai cluster node exec` et `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="217ac-520">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="217ac-521">Ces commandes permettent d’exécuter des commandes directement sur les nœuds et fournissent la fonctionnalité de réacheminement de port.</span><span class="sxs-lookup"><span data-stu-id="217ac-521">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="217ac-522">Ajout de la prise en charge des commandes `--ids` et `batchai`</span><span class="sxs-lookup"><span data-stu-id="217ac-522">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="217ac-523">[CHANGEMENT CASSANT] Tous les clusters et serveurs de fichiers doivent être créés dans des espaces de travail</span><span class="sxs-lookup"><span data-stu-id="217ac-523">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="217ac-524">[CHANGEMENT CASSANT] Les travaux doivent être créés dans des expériences</span><span class="sxs-lookup"><span data-stu-id="217ac-524">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="217ac-525">[CHANGEMENT CASSANT] Suppression de `--nfs-resource-group` des commandes `cluster create` et `job create`.</span><span class="sxs-lookup"><span data-stu-id="217ac-525">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="217ac-526">Pour monter un NFS appartenant à un autre espace de travail/groupe de ressources, indiquez l’ID ARM du serveur de fichiers via l’option `--nfs`</span><span class="sxs-lookup"><span data-stu-id="217ac-526">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="217ac-527">[CHANGEMENT CASSANT] Suppression de `--cluster-resource-group` de la commande `job create`.</span><span class="sxs-lookup"><span data-stu-id="217ac-527">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="217ac-528">Pour soumettre un travail sur un cluster appartenant à un autre espace de travail/groupe de ressources, indiquez l’ID ARM du cluster via l’option `--cluster`</span><span class="sxs-lookup"><span data-stu-id="217ac-528">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="217ac-529">[CHANGEMENT CASSANT] Suppression de l’attribut `location` des travaux, clusters et serveurs de fichiers.</span><span class="sxs-lookup"><span data-stu-id="217ac-529">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="217ac-530">L’emplacement est maintenant un attribut d’espace de travail.</span><span class="sxs-lookup"><span data-stu-id="217ac-530">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="217ac-531">[CHANGEMENT CASSANT] Suppression de `--location` des commandes `job create`, `cluster create` et `file-server create`</span><span class="sxs-lookup"><span data-stu-id="217ac-531">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="217ac-532">[CHANGEMENT CASSANT] Modification des noms des options courtes pour rendre l’interface plus cohérente :</span><span class="sxs-lookup"><span data-stu-id="217ac-532">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="217ac-533">[`--config`, `-c`] renommé en [`--config-file`, `-f`]</span><span class="sxs-lookup"><span data-stu-id="217ac-533">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="217ac-534">[`--cluster`, `-r`] renommé en [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="217ac-534">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="217ac-535">[`--cluster`, `-n`] renommé en [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="217ac-535">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="217ac-536">[`--job`, `-n`] renommé en [`--job`, `-j`]</span><span class="sxs-lookup"><span data-stu-id="217ac-536">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="217ac-537">Cartes</span><span class="sxs-lookup"><span data-stu-id="217ac-537">Maps</span></span>

* <span data-ttu-id="217ac-538">[CHANGEMENT CASSANT] Modification de `maps account create` pour accepter les Conditions d’utilisation, soit par l’invite interactive ou par l’indicateur `--accept-tos`</span><span class="sxs-lookup"><span data-stu-id="217ac-538">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="217ac-539">Réseau</span><span class="sxs-lookup"><span data-stu-id="217ac-539">Network</span></span>

* <span data-ttu-id="217ac-540">Ajout de la prise en charge de `https` à `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="217ac-540">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="217ac-541">Correction d’un problème où `--endpoint-status` était sensible à la casse.</span><span class="sxs-lookup"><span data-stu-id="217ac-541">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="217ac-542">#6502</span><span class="sxs-lookup"><span data-stu-id="217ac-542">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="217ac-543">Réservations</span><span class="sxs-lookup"><span data-stu-id="217ac-543">Reservations</span></span>

* <span data-ttu-id="217ac-544">[CHANGEMENT CASSANT] Ajout du paramètre obligatoire `ReservedResourceType` à `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="217ac-544">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="217ac-545">Ajout du paramètre `Location` à `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="217ac-545">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="217ac-546">[CHANGEMENT CASSANT] Suppression de `kind` de `ReservationProperties`</span><span class="sxs-lookup"><span data-stu-id="217ac-546">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="217ac-547">[CHANGEMENT CASSANT] `capabilities` renommé en `sku_properties` dans `Catalog`</span><span class="sxs-lookup"><span data-stu-id="217ac-547">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="217ac-548">[CHANGEMENT CASSANT] Suppression des propriétés `size` et `tier` de `Catalog`</span><span class="sxs-lookup"><span data-stu-id="217ac-548">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="217ac-549">Ajout du paramètre `InstanceFlexibility` à `reservations reservation update`</span><span class="sxs-lookup"><span data-stu-id="217ac-549">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="217ac-550">Rôle</span><span class="sxs-lookup"><span data-stu-id="217ac-550">Role</span></span>

* <span data-ttu-id="217ac-551">Amélioration de la gestion des erreurs</span><span class="sxs-lookup"><span data-stu-id="217ac-551">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="217ac-552">SQL</span><span class="sxs-lookup"><span data-stu-id="217ac-552">SQL</span></span>

* <span data-ttu-id="217ac-553">Correction de l’erreur déroutante lors de l’exécution de `az sql db list-editions` pour un emplacement qui n’est pas disponible pour votre abonnement</span><span class="sxs-lookup"><span data-stu-id="217ac-553">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="217ac-554">Stockage</span><span class="sxs-lookup"><span data-stu-id="217ac-554">Storage</span></span>

* <span data-ttu-id="217ac-555">Modification de la sortie de table pour que `storage blob download` soit plus lisible</span><span class="sxs-lookup"><span data-stu-id="217ac-555">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="217ac-556">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="217ac-556">VM</span></span>

* <span data-ttu-id="217ac-557">Amélioration de la vérification de la taille de la machine virtuelle pour la prise en charge de la mise en réseau accélérée dans `vm create`</span><span class="sxs-lookup"><span data-stu-id="217ac-557">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="217ac-558">Ajout d’un avertissement pour `vmss create` indiquant que la taille de la machine virtuelle par défaut va passer de `Standard_D1_v2` à `Standard_DS1_v2`</span><span class="sxs-lookup"><span data-stu-id="217ac-558">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="217ac-559">Ajout de `--force-update` à `[vm|vmss] extension set` pour mettre à jour l’extension, même lorsque la configuration n’a pas changé</span><span class="sxs-lookup"><span data-stu-id="217ac-559">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="217ac-560">13 juin 2018</span><span class="sxs-lookup"><span data-stu-id="217ac-560">June 13, 2018</span></span>

<span data-ttu-id="217ac-561">Version 2.0.37</span><span class="sxs-lookup"><span data-stu-id="217ac-561">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="217ac-562">Principal</span><span class="sxs-lookup"><span data-stu-id="217ac-562">Core</span></span>

* <span data-ttu-id="217ac-563">Amélioration de la télémétrie interactive</span><span class="sxs-lookup"><span data-stu-id="217ac-563">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="217ac-564">13 juin 2018</span><span class="sxs-lookup"><span data-stu-id="217ac-564">June 13, 2018</span></span>

<span data-ttu-id="217ac-565">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="217ac-565">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="217ac-566">AKS</span><span class="sxs-lookup"><span data-stu-id="217ac-566">AKS</span></span>

* <span data-ttu-id="217ac-567">Ajout d’options réseau avancées à `aks create`</span><span class="sxs-lookup"><span data-stu-id="217ac-567">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="217ac-568">Ajout d’arguments à `aks create` pour permettre la surveillance et le routage HTTP</span><span class="sxs-lookup"><span data-stu-id="217ac-568">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="217ac-569">Ajout de l’argument `--no-ssh-key` à `aks create`</span><span class="sxs-lookup"><span data-stu-id="217ac-569">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="217ac-570">Ajout de l’argument `--enable-rbac` à `aks create`</span><span class="sxs-lookup"><span data-stu-id="217ac-570">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="217ac-571">[PRÉVERSION] Ajout de la prise en charge pour l’authentification basée sur Azure Active Directory à `aks create`</span><span class="sxs-lookup"><span data-stu-id="217ac-571">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="217ac-572">AppService</span><span class="sxs-lookup"><span data-stu-id="217ac-572">AppService</span></span>

* <span data-ttu-id="217ac-573">Résolution d’un problème lié à des versions urllib incompatibles</span><span class="sxs-lookup"><span data-stu-id="217ac-573">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="217ac-574">5 juin 2018</span><span class="sxs-lookup"><span data-stu-id="217ac-574">June 5, 2018</span></span>

<span data-ttu-id="217ac-575">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="217ac-575">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="217ac-576">Interactive</span><span class="sxs-lookup"><span data-stu-id="217ac-576">Interactive</span></span>

* <span data-ttu-id="217ac-577">Ajout de limites aux dépendances du mode interactif</span><span class="sxs-lookup"><span data-stu-id="217ac-577">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="217ac-578">5 juin 2018</span><span class="sxs-lookup"><span data-stu-id="217ac-578">June 5, 2018</span></span>

<span data-ttu-id="217ac-579">Version 2.0.34</span><span class="sxs-lookup"><span data-stu-id="217ac-579">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="217ac-580">Principal</span><span class="sxs-lookup"><span data-stu-id="217ac-580">Core</span></span>

* <span data-ttu-id="217ac-581">Prise en charge supplémentaire pour les références de ressources inter-client</span><span class="sxs-lookup"><span data-stu-id="217ac-581">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="217ac-582">Amélioration de la fiabilité de téléchargement des données de télémétrie</span><span class="sxs-lookup"><span data-stu-id="217ac-582">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="217ac-583">ACR</span><span class="sxs-lookup"><span data-stu-id="217ac-583">ACR</span></span>

* <span data-ttu-id="217ac-584">Prise en charge supplémentaire pour VSTS en tant qu’emplacement source distant</span><span class="sxs-lookup"><span data-stu-id="217ac-584">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="217ac-585">Ajout de la commande `acr import`</span><span class="sxs-lookup"><span data-stu-id="217ac-585">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="217ac-586">AKS</span><span class="sxs-lookup"><span data-stu-id="217ac-586">AKS</span></span>

* <span data-ttu-id="217ac-587">`aks get-credentials` a été modifié pour créer le fichier de configuration kube avec des autorisations de système de fichiers plus sécurisées</span><span class="sxs-lookup"><span data-stu-id="217ac-587">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="217ac-588">Batch</span><span class="sxs-lookup"><span data-stu-id="217ac-588">Batch</span></span>

* <span data-ttu-id="217ac-589">Résolution du bogue concernant la mise en forme dans la table de liste de pool [[problème #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="217ac-589">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="217ac-590">IOT</span><span class="sxs-lookup"><span data-stu-id="217ac-590">IOT</span></span>

* <span data-ttu-id="217ac-591">Prise en charge ajoutée pour la création de IoT Hubs de niveau de base</span><span class="sxs-lookup"><span data-stu-id="217ac-591">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="217ac-592">Réseau</span><span class="sxs-lookup"><span data-stu-id="217ac-592">Network</span></span>

* <span data-ttu-id="217ac-593">`network vnet peering` amélioré</span><span class="sxs-lookup"><span data-stu-id="217ac-593">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="217ac-594">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="217ac-594">Policy Insights</span></span>

* <span data-ttu-id="217ac-595">Version initiale</span><span class="sxs-lookup"><span data-stu-id="217ac-595">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="217ac-596">ARM</span><span class="sxs-lookup"><span data-stu-id="217ac-596">ARM</span></span>

* <span data-ttu-id="217ac-597">Ajout des commandes `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="217ac-597">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="217ac-598">SQL</span><span class="sxs-lookup"><span data-stu-id="217ac-598">SQL</span></span>

* <span data-ttu-id="217ac-599">Ajout de nouvelles commandes d’instance gérée :</span><span class="sxs-lookup"><span data-stu-id="217ac-599">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="217ac-600">Ajout de nouvelles commandes de base de données gérée :</span><span class="sxs-lookup"><span data-stu-id="217ac-600">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="217ac-601">Stockage</span><span class="sxs-lookup"><span data-stu-id="217ac-601">Storage</span></span>

* <span data-ttu-id="217ac-602">Ajout de types MimeTypes supplémentaires pour les formats json et javascript pour être déduit à partir des extensions de fichier</span><span class="sxs-lookup"><span data-stu-id="217ac-602">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="217ac-603">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="217ac-603">VM</span></span>

* <span data-ttu-id="217ac-604">`vm list-skus` a été modifié pour utiliser des colonnes corrigées et ajouter l’avertissement que `Tier` et `Size` seront supprimés</span><span class="sxs-lookup"><span data-stu-id="217ac-604">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="217ac-605">Ajout de l’option `--accelerated-networking` à `vm create`</span><span class="sxs-lookup"><span data-stu-id="217ac-605">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="217ac-606">Ajout de `--tags` à `identity create`</span><span class="sxs-lookup"><span data-stu-id="217ac-606">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="217ac-607">22 mai 2018</span><span class="sxs-lookup"><span data-stu-id="217ac-607">May 22, 2018</span></span>

<span data-ttu-id="217ac-608">Version 2.0.33</span><span class="sxs-lookup"><span data-stu-id="217ac-608">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="217ac-609">Principal</span><span class="sxs-lookup"><span data-stu-id="217ac-609">Core</span></span>

* <span data-ttu-id="217ac-610">Ajout de la prise en charge pour le développement de `@` dans les noms de fichiers</span><span class="sxs-lookup"><span data-stu-id="217ac-610">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="217ac-611">ACS</span><span class="sxs-lookup"><span data-stu-id="217ac-611">ACS</span></span>

* <span data-ttu-id="217ac-612">Ajout de nouvelles commandes Dev Spaces `aks use-dev-spaces` et `aks remove-dev-spaces`</span><span class="sxs-lookup"><span data-stu-id="217ac-612">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="217ac-613">Faute de frappe corrigée dans un message d’aide</span><span class="sxs-lookup"><span data-stu-id="217ac-613">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="217ac-614">AppService</span><span class="sxs-lookup"><span data-stu-id="217ac-614">AppService</span></span>

* <span data-ttu-id="217ac-615">Amélioration des commandes de mise à jour générique</span><span class="sxs-lookup"><span data-stu-id="217ac-615">Improved generic update commands</span></span>
* <span data-ttu-id="217ac-616">Ajout de la prise en charge asynchrone pour `webapp deployment source config-zip`</span><span class="sxs-lookup"><span data-stu-id="217ac-616">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="217ac-617">Conteneur</span><span class="sxs-lookup"><span data-stu-id="217ac-617">Container</span></span>

* <span data-ttu-id="217ac-618">Prise en charge ajoutée pour l’exportation d’un groupe de conteneurs au format yaml</span><span class="sxs-lookup"><span data-stu-id="217ac-618">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="217ac-619">Prise en charge ajoutée pour l’utilisation d’un fichier yaml afin de créer/mettre à jour un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="217ac-619">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="217ac-620">Extension</span><span class="sxs-lookup"><span data-stu-id="217ac-620">Extension</span></span>

* <span data-ttu-id="217ac-621">Amélioration de la suppression des extensions</span><span class="sxs-lookup"><span data-stu-id="217ac-621">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="217ac-622">Interactive</span><span class="sxs-lookup"><span data-stu-id="217ac-622">Interactive</span></span>

* <span data-ttu-id="217ac-623">La journalisation a été modifiée pour désactiver l’analyseur pour les saisies semi-automatiques</span><span class="sxs-lookup"><span data-stu-id="217ac-623">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="217ac-624">Gestion améliorée des caches d’aide incorrects</span><span class="sxs-lookup"><span data-stu-id="217ac-624">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="217ac-625">KeyVault</span><span class="sxs-lookup"><span data-stu-id="217ac-625">KeyVault</span></span>

* <span data-ttu-id="217ac-626">Commandes keyvault corrigées afin de fonctionner dans Cloud Shell ou dans des machines virtuelles avec l’identité</span><span class="sxs-lookup"><span data-stu-id="217ac-626">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="217ac-627">Réseau</span><span class="sxs-lookup"><span data-stu-id="217ac-627">Network</span></span>

* <span data-ttu-id="217ac-628">Résolution d’un problème où `network watcher show-topology` ne fonctionnait pas avec le nom de réseau virtuel et/ou de sous-réseau [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="217ac-628">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="217ac-629">Correction d’un problème où certaines commandes `network watcher` revendiquaient que Network Watcher n’était pas activé pour certaines régions alors qu’il l’était [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="217ac-629">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="217ac-630">SQL</span><span class="sxs-lookup"><span data-stu-id="217ac-630">SQL</span></span>

* <span data-ttu-id="217ac-631">[CHANGEMENT CASSANT] Objets de réponse retournés modifiés à partir des commandes `db` et `dw`</span><span class="sxs-lookup"><span data-stu-id="217ac-631">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="217ac-632">Propriété `serviceLevelObjective` renommée en `currentServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="217ac-632">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="217ac-633">Suppression des propriétés `currentServiceObjectiveId` et `requestedServiceObjectiveId`</span><span class="sxs-lookup"><span data-stu-id="217ac-633">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="217ac-634">Propriété `maxSizeBytes` modifiée en valeur entière au lieu d’une chaîne</span><span class="sxs-lookup"><span data-stu-id="217ac-634">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="217ac-635">[CHANGEMENT CASSANT] Les propriétés `db` et `dw` suivantes ont été modifiées pour être en lecture seule :</span><span class="sxs-lookup"><span data-stu-id="217ac-635">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="217ac-636">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="217ac-636">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="217ac-637">Pour mettre à jour, utilisez le paramètre `--service-objective` ou définissez la propriété `sku.name`</span><span class="sxs-lookup"><span data-stu-id="217ac-637">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="217ac-638">`edition`.</span><span class="sxs-lookup"><span data-stu-id="217ac-638">`edition`.</span></span> <span data-ttu-id="217ac-639">Pour mettre à jour, utilisez le paramètre `--edition` ou définissez la propriété `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="217ac-639">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="217ac-640">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="217ac-640">`elasticPoolName`.</span></span> <span data-ttu-id="217ac-641">Pour mettre à jour, utilisez le paramètre `--elastic-pool` ou définissez la propriété `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="217ac-641">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="217ac-642">[CHANGEMENT CASSANT] Les propriétés `elastic-pool` suivantes ont été modifiées pour être en lecture seule :</span><span class="sxs-lookup"><span data-stu-id="217ac-642">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="217ac-643">`edition`.</span><span class="sxs-lookup"><span data-stu-id="217ac-643">`edition`.</span></span> <span data-ttu-id="217ac-644">Pour mettre à jour, utilisez le paramètre `--edition`</span><span class="sxs-lookup"><span data-stu-id="217ac-644">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="217ac-645">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="217ac-645">`dtu`.</span></span> <span data-ttu-id="217ac-646">Pour mettre à jour, utilisez le paramètre `--capacity`</span><span class="sxs-lookup"><span data-stu-id="217ac-646">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="217ac-647">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="217ac-647">`databaseDtuMin`.</span></span> <span data-ttu-id="217ac-648">Pour mettre à jour, utilisez le paramètre `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="217ac-648">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="217ac-649">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="217ac-649">`databaseDtuMax`.</span></span> <span data-ttu-id="217ac-650">Pour mettre à jour, utilisez le paramètre `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="217ac-650">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="217ac-651">Ajout des paramètres `--family` et `--capacity` aux commandes `db`, `dw` et `elastic-pool`</span><span class="sxs-lookup"><span data-stu-id="217ac-651">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="217ac-652">Ajout de formateurs de table aux commandes `db`, `dw` et `elastic-pool`</span><span class="sxs-lookup"><span data-stu-id="217ac-652">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="217ac-653">Stockage</span><span class="sxs-lookup"><span data-stu-id="217ac-653">Storage</span></span>

* <span data-ttu-id="217ac-654">Ajout d’un compléteur pour l’argument `--account-name`</span><span class="sxs-lookup"><span data-stu-id="217ac-654">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="217ac-655">Correction d’un problème avec `storage entity query`</span><span class="sxs-lookup"><span data-stu-id="217ac-655">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="217ac-656">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="217ac-656">VM</span></span>

* <span data-ttu-id="217ac-657">[CHANGEMENT CASSANT] Suppression de `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="217ac-657">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="217ac-658">La même prise en charge est accessible via `vm update` ou `vm disk attach`</span><span class="sxs-lookup"><span data-stu-id="217ac-658">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="217ac-659">Correction de l’image de l’extension efficace dans `[vm|vmss] extension`</span><span class="sxs-lookup"><span data-stu-id="217ac-659">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="217ac-660">Ajout de`--boot-diagnostics-storage` à `vm create` pour capturer le journal de démarrage</span><span class="sxs-lookup"><span data-stu-id="217ac-660">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="217ac-661">Ajout de `--license-type` à `[vm|vmss] update`</span><span class="sxs-lookup"><span data-stu-id="217ac-661">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="217ac-662">7 mai 2018</span><span class="sxs-lookup"><span data-stu-id="217ac-662">May 7, 2018</span></span>

<span data-ttu-id="217ac-663">Version 2.0.32</span><span class="sxs-lookup"><span data-stu-id="217ac-663">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="217ac-664">Principal</span><span class="sxs-lookup"><span data-stu-id="217ac-664">Core</span></span>

* <span data-ttu-id="217ac-665">Correction d’une exception non gérée lors de la récupération des clés secrètes à partir d’un compte de principal de service avec certificat</span><span class="sxs-lookup"><span data-stu-id="217ac-665">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="217ac-666">Nouvelle prise en charge limitée pour les arguments positionnels</span><span class="sxs-lookup"><span data-stu-id="217ac-666">Added limited support for positional arguments</span></span>
* <span data-ttu-id="217ac-667">Correction d’un problème où `--query` ne pouvait pas être utilisé avec `--ids`.</span><span class="sxs-lookup"><span data-stu-id="217ac-667">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="217ac-668">#5591</span><span class="sxs-lookup"><span data-stu-id="217ac-668">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="217ac-669">Amélioration des scénarios de redirection à partir des commandes en utilisant `--ids`.</span><span class="sxs-lookup"><span data-stu-id="217ac-669">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="217ac-670">Prend en charge `-o tsv` avec une requête spécifiée ou `-o json` sans spécification de requête</span><span class="sxs-lookup"><span data-stu-id="217ac-670">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="217ac-671">Ajout de suggestions de commande en cas d’erreur engendrées par des fautes de frappe des utilisateurs dans les commandes</span><span class="sxs-lookup"><span data-stu-id="217ac-671">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="217ac-672">Amélioration de l’erreur lorsque les utilisateurs entrent `az ''`</span><span class="sxs-lookup"><span data-stu-id="217ac-672">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="217ac-673">Ajout de la prise en charge des types de ressources personnalisés pour les modules et les extensions de commande</span><span class="sxs-lookup"><span data-stu-id="217ac-673">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="217ac-674">ACR</span><span class="sxs-lookup"><span data-stu-id="217ac-674">ACR</span></span>

* <span data-ttu-id="217ac-675">Ajout de commandes de build de l’ACR</span><span class="sxs-lookup"><span data-stu-id="217ac-675">Added ACR Build commands</span></span>
* <span data-ttu-id="217ac-676">Améliorations des messages d’erreur dus aux ressources introuvables</span><span class="sxs-lookup"><span data-stu-id="217ac-676">Improved resource not found error messages</span></span>
* <span data-ttu-id="217ac-677">Amélioration des performances de création de ressources et de la gestion des erreurs</span><span class="sxs-lookup"><span data-stu-id="217ac-677">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="217ac-678">Amélioration de la connexion ACR dans des consoles non standards et des WSL</span><span class="sxs-lookup"><span data-stu-id="217ac-678">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="217ac-679">Amélioration des messages d’erreur dus aux commandes de dépôt</span><span class="sxs-lookup"><span data-stu-id="217ac-679">Improved repository commands error messages</span></span>
* <span data-ttu-id="217ac-680">Mise à jour des colonnes de la table et du classement</span><span class="sxs-lookup"><span data-stu-id="217ac-680">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="217ac-681">ACS</span><span class="sxs-lookup"><span data-stu-id="217ac-681">ACS</span></span>

* <span data-ttu-id="217ac-682">Ajout d’un avertissement indiquant que `az aks` est un service en préversion</span><span class="sxs-lookup"><span data-stu-id="217ac-682">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="217ac-683">Résolution du problème d’autorisation dans `aks install-connector` lorsque `--aci-resource-group` n’est pas spécifié</span><span class="sxs-lookup"><span data-stu-id="217ac-683">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="217ac-684">AMS</span><span class="sxs-lookup"><span data-stu-id="217ac-684">AMS</span></span>

* <span data-ttu-id="217ac-685">Version initiale - Gérer des ressources Azure Media Services</span><span class="sxs-lookup"><span data-stu-id="217ac-685">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="217ac-686">AppService</span><span class="sxs-lookup"><span data-stu-id="217ac-686">Appservice</span></span>

* <span data-ttu-id="217ac-687">Correction d’un bogue dans `webapp delete` lorsque `--slot` est fourni</span><span class="sxs-lookup"><span data-stu-id="217ac-687">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="217ac-688">`--runtime-version` retiré de `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="217ac-688">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="217ac-689">Ajout de la prise en charge de min\_tls\_version & https2.0</span><span class="sxs-lookup"><span data-stu-id="217ac-689">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="217ac-690">Ajout de la prise en charge pour les multiconteneurs</span><span class="sxs-lookup"><span data-stu-id="217ac-690">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="217ac-691">Batch AI</span><span class="sxs-lookup"><span data-stu-id="217ac-691">Batch AI</span></span>

* <span data-ttu-id="217ac-692">`batchai create cluster` modifié pour respecter la priorité de machine virtuelle configurée dans le fichier de configuration du cluster</span><span class="sxs-lookup"><span data-stu-id="217ac-692">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="217ac-693">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="217ac-693">Cognitive Services</span></span>

* <span data-ttu-id="217ac-694">Faute de frappe corrigée dans l’exemple de `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="217ac-694">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="217ac-695">Consommation</span><span class="sxs-lookup"><span data-stu-id="217ac-695">Consumption</span></span>

* <span data-ttu-id="217ac-696">Ajout de nouvelles commandes pour l’API Budget</span><span class="sxs-lookup"><span data-stu-id="217ac-696">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="217ac-697">Conteneur</span><span class="sxs-lookup"><span data-stu-id="217ac-697">Container</span></span>

* <span data-ttu-id="217ac-698">Suppression de l’exigence pour `--registry-server` pour `container create` lorsqu’un serveur de registre est inclus dans le nom de l’image</span><span class="sxs-lookup"><span data-stu-id="217ac-698">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="217ac-699">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="217ac-699">Cosmos DB</span></span>

* <span data-ttu-id="217ac-700">Présentation de la prise en charge d’un réseau virtuel pour Azure CLI - Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="217ac-700">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="217ac-701">DMS</span><span class="sxs-lookup"><span data-stu-id="217ac-701">DMS</span></span>

* <span data-ttu-id="217ac-702">Version initiale - Ajoute la prise en charge de l’instruction SQL pour le scénario de migration de SQL Azure</span><span class="sxs-lookup"><span data-stu-id="217ac-702">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="217ac-703">Extension</span><span class="sxs-lookup"><span data-stu-id="217ac-703">Extension</span></span>

* <span data-ttu-id="217ac-704">Correction d’un bogue où les métadonnées d’extension cessaient d’être affichées</span><span class="sxs-lookup"><span data-stu-id="217ac-704">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="217ac-705">Interactive</span><span class="sxs-lookup"><span data-stu-id="217ac-705">Interactive</span></span>

* <span data-ttu-id="217ac-706">Autorise le fonctionnement de compléments interactifs avec des arguments positionnel</span><span class="sxs-lookup"><span data-stu-id="217ac-706">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="217ac-707">Sortie plus conviviale lorsque les utilisateurs entrent \'</span><span class="sxs-lookup"><span data-stu-id="217ac-707">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="217ac-708">Achèvements corrigés pour les paramètres sans aide</span><span class="sxs-lookup"><span data-stu-id="217ac-708">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="217ac-709">Descriptions corrigées pour les groupes de commandes</span><span class="sxs-lookup"><span data-stu-id="217ac-709">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="217ac-710">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="217ac-710">Lab</span></span>

* <span data-ttu-id="217ac-711">Régressions corrigées de conversion Knack</span><span class="sxs-lookup"><span data-stu-id="217ac-711">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="217ac-712">Réseau</span><span class="sxs-lookup"><span data-stu-id="217ac-712">Network</span></span>

* <span data-ttu-id="217ac-713">[CHANGEMENT CASSANT] Suppression du paramètre `--ids` pour :</span><span class="sxs-lookup"><span data-stu-id="217ac-713">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="217ac-714">Profil</span><span class="sxs-lookup"><span data-stu-id="217ac-714">Profile</span></span>

* <span data-ttu-id="217ac-715">Correction de la détection de source `disk create`</span><span class="sxs-lookup"><span data-stu-id="217ac-715">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="217ac-716">[CHANGEMENT CASSANT] Suppression de `--msi-port` et `--identity-port` car ils ne sont plus utilisés</span><span class="sxs-lookup"><span data-stu-id="217ac-716">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="217ac-717">Correction d’une faute de frappe dans le bref résumé de `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="217ac-717">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="217ac-718">Redis</span><span class="sxs-lookup"><span data-stu-id="217ac-718">Redis</span></span>

* <span data-ttu-id="217ac-719">`redis patch-schedule patch-schedule show` déconseillé en faveur de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="217ac-719">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="217ac-720">`redis list-all` déconseillé.</span><span class="sxs-lookup"><span data-stu-id="217ac-720">Deprecated `redis list-all`.</span></span> <span data-ttu-id="217ac-721">Cette fonctionnalité a été pliée dans `redis list`</span><span class="sxs-lookup"><span data-stu-id="217ac-721">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="217ac-722">`redis import-method` déconseillé en faveur de `redis import`</span><span class="sxs-lookup"><span data-stu-id="217ac-722">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="217ac-723">Ajout de la prise en charge de `--ids` pour diverses commandes</span><span class="sxs-lookup"><span data-stu-id="217ac-723">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="217ac-724">Rôle</span><span class="sxs-lookup"><span data-stu-id="217ac-724">Role</span></span>

* <span data-ttu-id="217ac-725">[CHANGEMENT CASSANT] Suppression de `ad sp reset-credentials` déconseillé</span><span class="sxs-lookup"><span data-stu-id="217ac-725">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="217ac-726">Stockage</span><span class="sxs-lookup"><span data-stu-id="217ac-726">Storage</span></span>

* <span data-ttu-id="217ac-727">Autorise l’application du jeton SAS de destination pour une copie d’objets blob si le SAS source et la clé de compte ne sont pas spécifiés</span><span class="sxs-lookup"><span data-stu-id="217ac-727">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="217ac-728">Exposé--délai d’expiration de socket pour les chargements et téléchargements d’objets blob</span><span class="sxs-lookup"><span data-stu-id="217ac-728">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="217ac-729">Traite les noms d’objets blob commençant par des séparateurs de chemin d’accès comme des chemins d’accès relatifs</span><span class="sxs-lookup"><span data-stu-id="217ac-729">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="217ac-730">Autorise `storage blob copy --source-sas` avec le caractère de démarrage de requête, « ? »</span><span class="sxs-lookup"><span data-stu-id="217ac-730">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="217ac-731">`storage entity query --marker` corrigé pour accepter une liste de clé =valeurs</span><span class="sxs-lookup"><span data-stu-id="217ac-731">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="217ac-732">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="217ac-732">VM</span></span>

* <span data-ttu-id="217ac-733">Correction d’une logique de détection invalide sur l’URI de l’objet blob non gérée</span><span class="sxs-lookup"><span data-stu-id="217ac-733">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="217ac-734">Ajout de la prise en charge du chiffrement de disque sans principaux de service fournis par l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="217ac-734">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="217ac-735">[CHANGEMENT CASSANT] Ne pas utiliser « ManagedIdentityExtension » de machine virtuelle pour la prise en charge de MSI</span><span class="sxs-lookup"><span data-stu-id="217ac-735">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="217ac-736">Ajout de la prise en charge pour la stratégie d’éviction vers `vmss`</span><span class="sxs-lookup"><span data-stu-id="217ac-736">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="217ac-737">[CHANGEMENT CASSANT] Suppression de `--ids` de :</span><span class="sxs-lookup"><span data-stu-id="217ac-737">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="217ac-738">Ajout de la prise en charge des accélérateurs d’écriture</span><span class="sxs-lookup"><span data-stu-id="217ac-738">Added write accelerator support</span></span>
* <span data-ttu-id="217ac-739">Ajout de `vmss perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="217ac-739">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="217ac-740">Correction de `vm diagnostics set` pour détecter la fiabilité du type de système d’exploitation de la machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="217ac-740">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="217ac-741">Modification de `vm resize` pour vérifier si la taille demandée est différente de celle actuellement définie et pour mettre à jour uniquement en cas de modifications</span><span class="sxs-lookup"><span data-stu-id="217ac-741">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="217ac-742">10 avril 2018</span><span class="sxs-lookup"><span data-stu-id="217ac-742">April 10, 2018</span></span>

<span data-ttu-id="217ac-743">Version 2.0.31</span><span class="sxs-lookup"><span data-stu-id="217ac-743">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="217ac-744">ACR</span><span class="sxs-lookup"><span data-stu-id="217ac-744">ACR</span></span>

* <span data-ttu-id="217ac-745">Gestion améliorée des erreurs de secours wincred</span><span class="sxs-lookup"><span data-stu-id="217ac-745">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="217ac-746">ACS</span><span class="sxs-lookup"><span data-stu-id="217ac-746">ACS</span></span>

* <span data-ttu-id="217ac-747">Modification de la durée de validité des SPN créés par AKS à 5 ans</span><span class="sxs-lookup"><span data-stu-id="217ac-747">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="217ac-748">AppService</span><span class="sxs-lookup"><span data-stu-id="217ac-748">Appservice</span></span>

* [CHANGEMENT CASSANT]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="217ac-750">Correction d’une exception non interceptée pour les plans webapp inexistants</span><span class="sxs-lookup"><span data-stu-id="217ac-750">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="217ac-751">Batch AI</span><span class="sxs-lookup"><span data-stu-id="217ac-751">BatchAI</span></span>

* <span data-ttu-id="217ac-752">Ajout de la prise en charge de l’API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="217ac-752">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="217ac-753">Montage au niveau du travail</span><span class="sxs-lookup"><span data-stu-id="217ac-753">Job level mounting</span></span>
  - <span data-ttu-id="217ac-754">Variables d’environnement avec les valeurs des secrets</span><span class="sxs-lookup"><span data-stu-id="217ac-754">Environment variables with secret values</span></span>
  - <span data-ttu-id="217ac-755">Paramètres des compteurs de performances</span><span class="sxs-lookup"><span data-stu-id="217ac-755">Performance counters settings</span></span>
  - <span data-ttu-id="217ac-756">Création de rapports de segments de ligne spécifiques à un travail</span><span class="sxs-lookup"><span data-stu-id="217ac-756">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="217ac-757">Prise en charge des sous-dossiers dans les listes de fichiers de l’API</span><span class="sxs-lookup"><span data-stu-id="217ac-757">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="217ac-758">Création de rapports d’utilisation et de limites</span><span class="sxs-lookup"><span data-stu-id="217ac-758">Usage and limits reporting</span></span>
  - <span data-ttu-id="217ac-759">Autorisation de la spécification du type de mise en cache pour les serveurs NFS</span><span class="sxs-lookup"><span data-stu-id="217ac-759">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="217ac-760">Prise en charge des images personnalisées</span><span class="sxs-lookup"><span data-stu-id="217ac-760">Support for custom images</span></span>
  - <span data-ttu-id="217ac-761">Ajout de la prise en charge de la boîte à outils pyTorch</span><span class="sxs-lookup"><span data-stu-id="217ac-761">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="217ac-762">Ajout de la commande `job wait` qui permet d’attendre la fin du travail et d’obtenir le code de sortie du travail</span><span class="sxs-lookup"><span data-stu-id="217ac-762">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="217ac-763">Ajout de la commande `usage show` pour répertorier l’utilisation actuelle des ressources Batch AI et les limites pour les différentes régions</span><span class="sxs-lookup"><span data-stu-id="217ac-763">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="217ac-764">Prise en charge des clouds nationaux</span><span class="sxs-lookup"><span data-stu-id="217ac-764">National clouds are supported</span></span>
* <span data-ttu-id="217ac-765">Ajout d’arguments de ligne de commande de travail pour monter des systèmes de fichiers au niveau du travail en plus des fichiers de configuration</span><span class="sxs-lookup"><span data-stu-id="217ac-765">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="217ac-766">Ajout de plus d’options pour personnaliser les clusters : priorité des machines virtuelles, sous-réseau, nombre de nœuds initial pour les clusters avec mise à l’échelle automatique, spécification d’une image personnalisée</span><span class="sxs-lookup"><span data-stu-id="217ac-766">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="217ac-767">Ajout d’une option de ligne de commande pour spécifier le type de mise en cache pour les NFS gérés par Batch AI</span><span class="sxs-lookup"><span data-stu-id="217ac-767">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="217ac-768">Simplification de la spécification du montage du système de fichiers dans les fichiers config.</span><span class="sxs-lookup"><span data-stu-id="217ac-768">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="217ac-769">Il est désormais possible d’omettre les informations d’identification pour les partages de fichiers Azure et les conteneurs d’objets blob Azure : CLI remplira les informations d’identification manquantes à l’aide de la clé du compte de stockage fournie par le biais des paramètres de ligne de commande ou spécifiée via la variable d’environnement, ou interrogera la clé à partir du stockage Azure (si le compte de stockage appartient à l’abonnement actuel)</span><span class="sxs-lookup"><span data-stu-id="217ac-769">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="217ac-770">La commande de flux de fichiers de travail se remplit désormais automatiquement lorsque le travail est terminé (réussite, échec, terminé ou supprimé)</span><span class="sxs-lookup"><span data-stu-id="217ac-770">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="217ac-771">Amélioration de la sortie `table` pour les opérations `show`</span><span class="sxs-lookup"><span data-stu-id="217ac-771">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="217ac-772">Ajout de l’option `--use-auto-storage` pour la création du cluster.</span><span class="sxs-lookup"><span data-stu-id="217ac-772">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="217ac-773">Cette option simplifie la gestion des comptes de stockage et le montage de partages de fichiers Azure et de conteneurs d’objets blob Azure vers des clusters</span><span class="sxs-lookup"><span data-stu-id="217ac-773">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="217ac-774">Ajout de l’option `--generate-ssh-keys` à `cluster create` et `file-server create`</span><span class="sxs-lookup"><span data-stu-id="217ac-774">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="217ac-775">Ajout de la possibilité de fournir la tâche de configuration de nœud via la ligne de commande</span><span class="sxs-lookup"><span data-stu-id="217ac-775">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="217ac-776">[CHANGEMENT CASSANT] Déplacement des commandes `job stream-file` et `job list-files` sous le groupe `job file`</span><span class="sxs-lookup"><span data-stu-id="217ac-776">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="217ac-777">[CHANGEMENT CASSANT] Renommage de `--admin-user-name` en `--user-name` dans la commande `file-server create` pour être cohérent avec la commande `cluster create`</span><span class="sxs-lookup"><span data-stu-id="217ac-777">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="217ac-778">Facturation</span><span class="sxs-lookup"><span data-stu-id="217ac-778">Billing</span></span>

* <span data-ttu-id="217ac-779">Ajout de commandes d’inscription de compte</span><span class="sxs-lookup"><span data-stu-id="217ac-779">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="217ac-780">Consommation</span><span class="sxs-lookup"><span data-stu-id="217ac-780">Consumption</span></span>

* <span data-ttu-id="217ac-781">Ajout des commandes `marketplace`</span><span class="sxs-lookup"><span data-stu-id="217ac-781">Added `marketplace` commands</span></span>
* <span data-ttu-id="217ac-782">[CHANGEMENT CASSANT] Renommage de `reservations summaries` en `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="217ac-782">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="217ac-783">[CHANGEMENT CASSANT] Renommage de `reservations details` en `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="217ac-783">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="217ac-784">[CHANGEMENT CASSANT] Suppression des options abrégées de `--reservation-order-id` et `--reservation-id` pour les commandes `reservation`</span><span class="sxs-lookup"><span data-stu-id="217ac-784">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="217ac-785">[CHANGEMENT CASSANT] Suppression des options abrégées de `--grain` pour les commandes `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="217ac-785">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="217ac-786">[CHANGEMENT CASSANT] Suppression des options abrégées de `--include-meter-details` pour les commandes `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="217ac-786">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="217ac-787">Conteneur</span><span class="sxs-lookup"><span data-stu-id="217ac-787">Container</span></span>

* <span data-ttu-id="217ac-788">Ajout des paramètres de montage de volume de référentiel Git `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` et `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="217ac-788">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="217ac-789">Résolution de [#5926](https://github.com/Azure/azure-cli/issues/5926) : `az container exec` échoue lorsque le nom du conteneur -- est spécifié</span><span class="sxs-lookup"><span data-stu-id="217ac-789">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="217ac-790">Extension</span><span class="sxs-lookup"><span data-stu-id="217ac-790">Extension</span></span>

* <span data-ttu-id="217ac-791">Modification du message de vérification de distribution pour qu’il soit au niveau du débogage</span><span class="sxs-lookup"><span data-stu-id="217ac-791">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="217ac-792">Interactive</span><span class="sxs-lookup"><span data-stu-id="217ac-792">Interactive</span></span>

* <span data-ttu-id="217ac-793">Modification pour arrêter la saisie semi-automatique sur les commandes non reconnues</span><span class="sxs-lookup"><span data-stu-id="217ac-793">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="217ac-794">Ajout d’événements de raccordement avant et après la création du sous-arbre de commande</span><span class="sxs-lookup"><span data-stu-id="217ac-794">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="217ac-795">Ajout de la saisie semi-automatique pour les paramètres `--ids`</span><span class="sxs-lookup"><span data-stu-id="217ac-795">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="217ac-796">Réseau</span><span class="sxs-lookup"><span data-stu-id="217ac-796">Network</span></span>

* <span data-ttu-id="217ac-797">Résolution de [#5936](https://github.com/Azure/azure-cli/issues/5936) : les balises `application-gateway create` n’ont pas pu déterminer l’ensemble</span><span class="sxs-lookup"><span data-stu-id="217ac-797">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="217ac-798">Ajout de l’argument `--auth-certs` pour joindre des certificats d’authentification pour `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="217ac-798">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="217ac-799">#4910</span><span class="sxs-lookup"><span data-stu-id="217ac-799">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="217ac-800">Ajout de commandes `ddos-protection` pour créer des plans de protection DDoS</span><span class="sxs-lookup"><span data-stu-id="217ac-800">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="217ac-801">Prise en charge de `--ddos-protection-plan` pour `vnet [create|update]` pour associer un réseau virtuel à un plan de protection DDoS</span><span class="sxs-lookup"><span data-stu-id="217ac-801">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="217ac-802">Résolution du problème avec l’indicateur `--disable-bgp-route-propagation` dans `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="217ac-802">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="217ac-803">Suppression des arguments factices `--public-ip-address-type` et `--subnet-type` pour `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="217ac-803">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="217ac-804">Ajout de la prise en charge des enregistrements TXT avec les séquences d’échappement RFC 1035 à `network dns zone [import|export]` et `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="217ac-804">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="217ac-805">Profil</span><span class="sxs-lookup"><span data-stu-id="217ac-805">Profile</span></span>

* <span data-ttu-id="217ac-806">Ajout de la prise en charge des comptes Azure Classic dans `account list`</span><span class="sxs-lookup"><span data-stu-id="217ac-806">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="217ac-807">[CHANGEMENT CASSANT] Suppression des arguments `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="217ac-807">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="217ac-808">SGBDR</span><span class="sxs-lookup"><span data-stu-id="217ac-808">RDBMS</span></span>

* <span data-ttu-id="217ac-809">Ajout de la commande `georestore`</span><span class="sxs-lookup"><span data-stu-id="217ac-809">Added `georestore` command</span></span>
* <span data-ttu-id="217ac-810">Suppression de la restriction de taille de stockage de la commande `create`</span><span class="sxs-lookup"><span data-stu-id="217ac-810">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="217ac-811">Ressource</span><span class="sxs-lookup"><span data-stu-id="217ac-811">Resource</span></span>

* <span data-ttu-id="217ac-812">Ajout de la prise en charge de `--metadata` pour `policy definition create`</span><span class="sxs-lookup"><span data-stu-id="217ac-812">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="217ac-813">Ajout de la prise en charge de `--metadata`, `--set`, `--add` et `--remove` à `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="217ac-813">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="217ac-814">SQL</span><span class="sxs-lookup"><span data-stu-id="217ac-814">SQL</span></span>

* <span data-ttu-id="217ac-815">Ajout de `sql elastic-pool op list` et `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="217ac-815">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="217ac-816">Stockage</span><span class="sxs-lookup"><span data-stu-id="217ac-816">Storage</span></span>

* <span data-ttu-id="217ac-817">Amélioration des messages d’erreur pour les chaînes de connexion incorrectes</span><span class="sxs-lookup"><span data-stu-id="217ac-817">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="217ac-818">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="217ac-818">VM</span></span>

* <span data-ttu-id="217ac-819">Ajout de la prise en charge pour configurer le nombre de domaines d’erreur de plateforme sur `vmss create`</span><span class="sxs-lookup"><span data-stu-id="217ac-819">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="217ac-820">Modification de `vmss create` sur la valeur par défaut de l’équilibreur de charge Standard pour les groupes identiques désactivés zonaux, grands ou avec un seul groupe de placement</span><span class="sxs-lookup"><span data-stu-id="217ac-820">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [CHANGEMENT CASSANT]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="217ac-822">Ajout de la prise en charge des références SKU d’IP public à `vm create`</span><span class="sxs-lookup"><span data-stu-id="217ac-822">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="217ac-823">Ajout des arguments `--keyvault` et `--resource-group` à `vm secret format` pour prendre en charge des scénarios où la commande ne parvient pas à résoudre l’ID de coffre.</span><span class="sxs-lookup"><span data-stu-id="217ac-823">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="217ac-824">#5718</span><span class="sxs-lookup"><span data-stu-id="217ac-824">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="217ac-825">Amélioration des erreurs pour `[vm|vmss create]` lorsque l’emplacement d’un groupe de ressources ne possède aucune prise en charge de zone</span><span class="sxs-lookup"><span data-stu-id="217ac-825">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="217ac-826">27 mars 2018</span><span class="sxs-lookup"><span data-stu-id="217ac-826">March 27, 2018</span></span>

<span data-ttu-id="217ac-827">Version 2.0.30</span><span class="sxs-lookup"><span data-stu-id="217ac-827">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="217ac-828">Principal</span><span class="sxs-lookup"><span data-stu-id="217ac-828">Core</span></span>

* <span data-ttu-id="217ac-829">Afficher le message pour les extensions marquées en tant que préversions dans l’aide</span><span class="sxs-lookup"><span data-stu-id="217ac-829">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="217ac-830">ACS</span><span class="sxs-lookup"><span data-stu-id="217ac-830">ACS</span></span>

* <span data-ttu-id="217ac-831">Corriger l’erreur de vérification de certificat SSL pour `aks install-cli` dans Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="217ac-831">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="217ac-832">AppService</span><span class="sxs-lookup"><span data-stu-id="217ac-832">Appservice</span></span>

* <span data-ttu-id="217ac-833">Ajout de la prise en charge HTTPS exclusive à `webapp update`</span><span class="sxs-lookup"><span data-stu-id="217ac-833">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="217ac-834">Ajout de la prise en charge des emplacements à `az webapp identity [assign|show]` et `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="217ac-834">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="217ac-835">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="217ac-835">Backup</span></span>

* <span data-ttu-id="217ac-836">Ajout de la commande `az backup protection isenabled-for-vm`</span><span class="sxs-lookup"><span data-stu-id="217ac-836">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="217ac-837">Cette commande peut être utilisée pour vérifier si une machine virtuelle est sauvegardée par un coffre dans l’abonnement</span><span class="sxs-lookup"><span data-stu-id="217ac-837">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="217ac-838">Activation des ID d’objet Azure pour les paramètres `--resource-group` et `--vault-name`, pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="217ac-838">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="217ac-839">Modification des paramètres `--name` pour accepter le format de sortie des commandes `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="217ac-839">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="217ac-840">Conteneur</span><span class="sxs-lookup"><span data-stu-id="217ac-840">Container</span></span>

* <span data-ttu-id="217ac-841">Ajout de la commande `container exec`</span><span class="sxs-lookup"><span data-stu-id="217ac-841">Added `container exec` command.</span></span> <span data-ttu-id="217ac-842">Exécute les commandes dans un conteneur, pour un groupe de conteneurs en exécution.</span><span class="sxs-lookup"><span data-stu-id="217ac-842">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="217ac-843">Autoriser la sortie de table pour la création et la mise à jour d’un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="217ac-843">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="217ac-844">Extension</span><span class="sxs-lookup"><span data-stu-id="217ac-844">Extension</span></span>

* <span data-ttu-id="217ac-845">Ajout d’un message pour `extension add` si l’extension est en préversion</span><span class="sxs-lookup"><span data-stu-id="217ac-845">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="217ac-846">Modification de `extension list-available` afin d’afficher les données complètes d’extension avec `--show-details`</span><span class="sxs-lookup"><span data-stu-id="217ac-846">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="217ac-847">[CHANGEMENT CASSANT] Modification de `extension list-available` afin d’afficher les données simplifiées d’extension par défaut</span><span class="sxs-lookup"><span data-stu-id="217ac-847">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="217ac-848">Interactive</span><span class="sxs-lookup"><span data-stu-id="217ac-848">Interactive</span></span>

* <span data-ttu-id="217ac-849">Modification des saisies semi-automatiques pour procéder à l’activation dès le chargement de la table de commande</span><span class="sxs-lookup"><span data-stu-id="217ac-849">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="217ac-850">Correction du bogue par l’exécution du paramètre `--style`</span><span class="sxs-lookup"><span data-stu-id="217ac-850">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="217ac-851">Analyseur lexical interactif instancié après le vidage de la table de commande, si manquant</span><span class="sxs-lookup"><span data-stu-id="217ac-851">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="217ac-852">Amélioration de la prise en charge de Completer</span><span class="sxs-lookup"><span data-stu-id="217ac-852">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="217ac-853">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="217ac-853">Lab</span></span>

* <span data-ttu-id="217ac-854">Correction des bogues avec la commande `create environment`</span><span class="sxs-lookup"><span data-stu-id="217ac-854">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="217ac-855">Surveiller</span><span class="sxs-lookup"><span data-stu-id="217ac-855">Monitor</span></span>

* <span data-ttu-id="217ac-856">Ajout de la prise en charge de `--top`, `--orderby` et `--namespace` à `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="217ac-856">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="217ac-857">Résolution de [#4529](https://github.com/Azure/azure-cli/issues/5785) : `metrics list` Accepte une liste de mesures séparées par des espaces à récupérer</span><span class="sxs-lookup"><span data-stu-id="217ac-857">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="217ac-858">Ajout de la prise en charge de `--namespace` à `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="217ac-858">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="217ac-859">Réseau</span><span class="sxs-lookup"><span data-stu-id="217ac-859">Network</span></span>

* <span data-ttu-id="217ac-860">Ajout de la prise en charge des zones de DNS privé</span><span class="sxs-lookup"><span data-stu-id="217ac-860">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="217ac-861">Profil</span><span class="sxs-lookup"><span data-stu-id="217ac-861">Profile</span></span>

* <span data-ttu-id="217ac-862">Ajout d’un avertissement pour `--identity-port` et `--msi-port` à `login`</span><span class="sxs-lookup"><span data-stu-id="217ac-862">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="217ac-863">SGBDR</span><span class="sxs-lookup"><span data-stu-id="217ac-863">RDBMS</span></span>

* <span data-ttu-id="217ac-864">Ajout de la version d’API mise à la disposition générale du modèle d’entreprise 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="217ac-864">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="217ac-865">Ressource</span><span class="sxs-lookup"><span data-stu-id="217ac-865">Resource</span></span>

* [CHANGEMENT CASSANT]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="217ac-867">Rôle</span><span class="sxs-lookup"><span data-stu-id="217ac-867">Role</span></span>

* <span data-ttu-id="217ac-868">Ajout de la prise en charge des configurations d’accès et des clients natifs requis à `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="217ac-868">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="217ac-869">Modification des commandes `rbac` afin de renvoyer moins de 1 000 ID sur la résolution d’objet</span><span class="sxs-lookup"><span data-stu-id="217ac-869">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="217ac-870">Ajout des commandes de gestion des informations d’identification `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="217ac-870">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="217ac-871">[CHANGEMENT CASSANT] Suppression des propriétés de la sortie `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="217ac-871">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="217ac-872">Ajout de la prise en charge des autorisations `dataActions` et `notDataActions` à `role definition`</span><span class="sxs-lookup"><span data-stu-id="217ac-872">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="217ac-873">Stockage</span><span class="sxs-lookup"><span data-stu-id="217ac-873">Storage</span></span>

* <span data-ttu-id="217ac-874">Résolution du problème lié au chargement des fichiers présentant une taille comprise entre 195 Go et 200 Go</span><span class="sxs-lookup"><span data-stu-id="217ac-874">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="217ac-875">Résolution de [#4049](https://github.com/Azure/azure-cli/issues/4049) : Problèmes avec les chargements d’objets blob d’ajout ignorant les paramètres de condition</span><span class="sxs-lookup"><span data-stu-id="217ac-875">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="217ac-876">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="217ac-876">VM</span></span>

* <span data-ttu-id="217ac-877">Ajout d’un avertissement à `vmss create` concernant les changements cassants à venir pour les ensembles comprenant plus de 100 instances</span><span class="sxs-lookup"><span data-stu-id="217ac-877">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="217ac-878">Ajout de la prise en charge de la résilience dans la zone à `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="217ac-878">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="217ac-879">Modification de la vue d’instance de disque pour signaler un meilleur état de chiffrement</span><span class="sxs-lookup"><span data-stu-id="217ac-879">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="217ac-880">[CHANGEMENT CASSANT] Modification de `vm extension delete` afin d’annuler la capacité de génération de sortie</span><span class="sxs-lookup"><span data-stu-id="217ac-880">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="217ac-881">13 mars 2018</span><span class="sxs-lookup"><span data-stu-id="217ac-881">March 13, 2018</span></span>

<span data-ttu-id="217ac-882">Version 2.0.29</span><span class="sxs-lookup"><span data-stu-id="217ac-882">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="217ac-883">ACR</span><span class="sxs-lookup"><span data-stu-id="217ac-883">ACR</span></span>

* <span data-ttu-id="217ac-884">Ajout de la prise en charge du paramètre `--image` pour `repository delete`</span><span class="sxs-lookup"><span data-stu-id="217ac-884">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="217ac-885">Paramètres `--manifest` et `--tag` de la commande `repository delete` déconseillés</span><span class="sxs-lookup"><span data-stu-id="217ac-885">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="217ac-886">Ajout de la commande `repository untag` pour supprimer une balise sans supprimer les données</span><span class="sxs-lookup"><span data-stu-id="217ac-886">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="217ac-887">ACS</span><span class="sxs-lookup"><span data-stu-id="217ac-887">ACS</span></span>

* <span data-ttu-id="217ac-888">Ajout de la commande `aks upgrade-connector` pour mettre à niveau un connecteur existant</span><span class="sxs-lookup"><span data-stu-id="217ac-888">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="217ac-889">Modification des fichiers de configuration `kubectl` pour utiliser un YAML de style bloc plus lisible</span><span class="sxs-lookup"><span data-stu-id="217ac-889">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="217ac-890">Advisor</span><span class="sxs-lookup"><span data-stu-id="217ac-890">Advisor</span></span>

* <span data-ttu-id="217ac-891">[CHANGEMENT CASSANT] Renommage de `advisor configuration get` en `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="217ac-891">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="217ac-892">[CHANGEMENT CASSANT] Renommage de `advisor configuration set` en `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="217ac-892">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="217ac-893">[CHANGEMENT CASSANT] Suppression de `advisor recommendation generate`</span><span class="sxs-lookup"><span data-stu-id="217ac-893">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="217ac-894">Ajout du paramètre `--refresh` pour `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="217ac-894">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="217ac-895">Ajout de la commande `advisor recommendation show`</span><span class="sxs-lookup"><span data-stu-id="217ac-895">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="217ac-896">AppService</span><span class="sxs-lookup"><span data-stu-id="217ac-896">Appservice</span></span>

* <span data-ttu-id="217ac-897">`[webapp|functionapp] assign-identity` déconseillé</span><span class="sxs-lookup"><span data-stu-id="217ac-897">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="217ac-898">Ajout des commandes d’identité gérée `webapp identity [assign|show]` et `functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="217ac-898">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="217ac-899">Eventhubs</span><span class="sxs-lookup"><span data-stu-id="217ac-899">Eventhubs</span></span>

* <span data-ttu-id="217ac-900">Version initiale</span><span class="sxs-lookup"><span data-stu-id="217ac-900">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="217ac-901">Extension</span><span class="sxs-lookup"><span data-stu-id="217ac-901">Extension</span></span>

* <span data-ttu-id="217ac-902">Ajout d’un contrôle supplémentaire pour avertir l’utilisateur si le distributeur utilisé est différent de celui stocké dans le fichier source du package, car cela peut entraîner des erreurs</span><span class="sxs-lookup"><span data-stu-id="217ac-902">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="217ac-903">Interactive</span><span class="sxs-lookup"><span data-stu-id="217ac-903">Interactive</span></span>

* <span data-ttu-id="217ac-904">Résolu [#5625](https://github.com/Azure/azure-cli/issues/5625) : conservation de l’historique entre différentes sessions</span><span class="sxs-lookup"><span data-stu-id="217ac-904">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="217ac-905">Résolu [#3016](https://github.com/Azure/azure-cli/issues/3016) : historique non enregistré alors qu’il était dans la portée</span><span class="sxs-lookup"><span data-stu-id="217ac-905">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="217ac-906">Résolu [#5688](https://github.com/Azure/azure-cli/issues/5688) : la saisie automatique n’apparaît pas si le chargement de la table de commande a rencontré une exception</span><span class="sxs-lookup"><span data-stu-id="217ac-906">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="217ac-907">Résolu : indicateur de progression pour les opérations à long terme</span><span class="sxs-lookup"><span data-stu-id="217ac-907">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="217ac-908">Surveiller</span><span class="sxs-lookup"><span data-stu-id="217ac-908">Monitor</span></span>

* <span data-ttu-id="217ac-909">Les commandes `monitor autoscale-settings` ont été déconseillées</span><span class="sxs-lookup"><span data-stu-id="217ac-909">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="217ac-910">Ajout des commandes `monitor autoscale`</span><span class="sxs-lookup"><span data-stu-id="217ac-910">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="217ac-911">Ajout des commandes `monitor autoscale profile`</span><span class="sxs-lookup"><span data-stu-id="217ac-911">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="217ac-912">Ajout des commandes `monitor autoscale rule`</span><span class="sxs-lookup"><span data-stu-id="217ac-912">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="217ac-913">Réseau</span><span class="sxs-lookup"><span data-stu-id="217ac-913">Network</span></span>

* <span data-ttu-id="217ac-914">[CHANGEMENT CASSANT] Suppression du paramètre `--tags` de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="217ac-914">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="217ac-915">Suppression de certaines valeurs par défaut erronées pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="217ac-915">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="217ac-916">Ajout des commandes `network watcher connection-monitor`</span><span class="sxs-lookup"><span data-stu-id="217ac-916">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="217ac-917">Ajout des paramètres `--vnet` et `--subnet` à `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="217ac-917">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="217ac-918">Profil</span><span class="sxs-lookup"><span data-stu-id="217ac-918">Profile</span></span>

* <span data-ttu-id="217ac-919">Paramètre `--msi` déconseillé pour `az login`</span><span class="sxs-lookup"><span data-stu-id="217ac-919">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="217ac-920">Ajout du paramètre `--identity` pour `az login` afin de remplacer `--msi`</span><span class="sxs-lookup"><span data-stu-id="217ac-920">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="217ac-921">SGBDR</span><span class="sxs-lookup"><span data-stu-id="217ac-921">RDBMS</span></span>

* <span data-ttu-id="217ac-922">[PRÉVERSION] Modifiée pour utiliser l’API 2017-12-01-préversion</span><span class="sxs-lookup"><span data-stu-id="217ac-922">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="217ac-923">Service Bus</span><span class="sxs-lookup"><span data-stu-id="217ac-923">Service Bus</span></span>

* <span data-ttu-id="217ac-924">Version initiale</span><span class="sxs-lookup"><span data-stu-id="217ac-924">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="217ac-925">Stockage</span><span class="sxs-lookup"><span data-stu-id="217ac-925">Storage</span></span>

* <span data-ttu-id="217ac-926">Résolution de [#4971](https://github.com/Azure/azure-cli/issues/4971) : `storage blob copy` prend désormais en charge les autres clouds Azure</span><span class="sxs-lookup"><span data-stu-id="217ac-926">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="217ac-927">Résolu [#5286](https://github.com/Azure/azure-cli/issues/5286) : Les lots de commandes `storage blob [delete-batch|download-batch|upload-batch]` ne génèrent plus une erreur lors d’échecs de la condition préalable</span><span class="sxs-lookup"><span data-stu-id="217ac-927">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="217ac-928">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="217ac-928">VM</span></span>

* <span data-ttu-id="217ac-929">Ajout de prise en charge de `[vm|vmss] create` pour attacher des disques de données non gérées et configurer la mise en cache</span><span class="sxs-lookup"><span data-stu-id="217ac-929">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="217ac-930">`[vm|vmss] assign-identity` et `[vm|vmss] remove-identity` sont déconseillés</span><span class="sxs-lookup"><span data-stu-id="217ac-930">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="217ac-931">Ajout des commandes `vm identity [assign|remove|show]` et `vmss identity [assign|remove|show]` pour remplacer des commandes déconseillées</span><span class="sxs-lookup"><span data-stu-id="217ac-931">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="217ac-932">Modification de la priorité par défaut dans `vmss create` à None</span><span class="sxs-lookup"><span data-stu-id="217ac-932">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="217ac-933">27 février 2018</span><span class="sxs-lookup"><span data-stu-id="217ac-933">February 27, 2018</span></span>

<span data-ttu-id="217ac-934">Version 2.0.28</span><span class="sxs-lookup"><span data-stu-id="217ac-934">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="217ac-935">Principal</span><span class="sxs-lookup"><span data-stu-id="217ac-935">Core</span></span>

* <span data-ttu-id="217ac-936">Résolu [#5184](https://github.com/Azure/azure-cli/issues/5184) : Problème d’installation d’Homebrew</span><span class="sxs-lookup"><span data-stu-id="217ac-936">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="217ac-937">Ajout de la prise en charge de télémétrie d’extension avec des clés personnalisées</span><span class="sxs-lookup"><span data-stu-id="217ac-937">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="217ac-938">Ajout de la connexion HTTP à `--debug`</span><span class="sxs-lookup"><span data-stu-id="217ac-938">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="217ac-939">ACS</span><span class="sxs-lookup"><span data-stu-id="217ac-939">ACS</span></span>

* <span data-ttu-id="217ac-940">Modification pour utiliser le graphique Helm `virtual-kubelet-for-aks` pour `aks install-connector` par défaut</span><span class="sxs-lookup"><span data-stu-id="217ac-940">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="217ac-941">Problème résolu : autorisation insuffisante des principaux de service à créer des groupes de conteneur ACI</span><span class="sxs-lookup"><span data-stu-id="217ac-941">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="217ac-942">Ajout des paramètres `--aci-container-group`, `--location` et `--image-tag` à `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="217ac-942">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="217ac-943">Suppression de l’avis de désapprobation de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="217ac-943">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="217ac-944">AppService</span><span class="sxs-lookup"><span data-stu-id="217ac-944">Appservice</span></span>

* <span data-ttu-id="217ac-945">Mises à jour pour la nouvelle version du kit de développement logiciel (SDK) (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="217ac-945">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="217ac-946">Résolu [#5538](https://github.com/Azure/azure-cli/issues/5538) : `Free` défini comme une SKU invalide</span><span class="sxs-lookup"><span data-stu-id="217ac-946">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="217ac-947">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="217ac-947">Cognitive Services</span></span>

* <span data-ttu-id="217ac-948">Mise à jour de l’avis lors de la création d’un compte Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="217ac-948">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="217ac-949">Consommation</span><span class="sxs-lookup"><span data-stu-id="217ac-949">Consumption</span></span>

* <span data-ttu-id="217ac-950">Ajout de nouvelles commandes pour l’API priceSheet</span><span class="sxs-lookup"><span data-stu-id="217ac-950">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="217ac-951">Mise à jour des formats existants Détails d’utilisations et Détails de la réservation</span><span class="sxs-lookup"><span data-stu-id="217ac-951">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="217ac-952">Conteneur</span><span class="sxs-lookup"><span data-stu-id="217ac-952">Container</span></span>

* <span data-ttu-id="217ac-953">Ajout des arguments `--secrets` et `--secrets-mount-path` à `container create` pour utiliser des secrets dans ACI</span><span class="sxs-lookup"><span data-stu-id="217ac-953">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="217ac-954">Réseau</span><span class="sxs-lookup"><span data-stu-id="217ac-954">Network</span></span>

* <span data-ttu-id="217ac-955">Résolu [#5559](https://github.com/Azure/azure-cli/issues/5559) : client manquant dans `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="217ac-955">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="217ac-956">Ressource</span><span class="sxs-lookup"><span data-stu-id="217ac-956">Resource</span></span>

* <span data-ttu-id="217ac-957">Modification de `group deployment export` pour afficher un modèle et des erreurs partiels sur échec</span><span class="sxs-lookup"><span data-stu-id="217ac-957">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="217ac-958">Rôle</span><span class="sxs-lookup"><span data-stu-id="217ac-958">Role</span></span>

* <span data-ttu-id="217ac-959">Ajout de `role assignment list-changelogs` pour permettre l’audit des rôles du principal de service</span><span class="sxs-lookup"><span data-stu-id="217ac-959">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="217ac-960">SQL</span><span class="sxs-lookup"><span data-stu-id="217ac-960">SQL</span></span>

* <span data-ttu-id="217ac-961">Ajout de la prise en charge de la redondance de zone pour les bases de données et les pools élastiques lors de création et mise à jour</span><span class="sxs-lookup"><span data-stu-id="217ac-961">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="217ac-962">Stockage</span><span class="sxs-lookup"><span data-stu-id="217ac-962">Storage</span></span>

* <span data-ttu-id="217ac-963">Activation de la spécification de préfixe/destination pour `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="217ac-963">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="217ac-964">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="217ac-964">VM</span></span>

* <span data-ttu-id="217ac-965">Ajout de prise en charge de jonction / séparation de disques sur une instance de groupe de machines virtuelles identiques uniques</span><span class="sxs-lookup"><span data-stu-id="217ac-965">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="217ac-966">13 février 2018</span><span class="sxs-lookup"><span data-stu-id="217ac-966">February 13, 2018</span></span>

<span data-ttu-id="217ac-967">Version 2.0.27</span><span class="sxs-lookup"><span data-stu-id="217ac-967">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="217ac-968">Principal</span><span class="sxs-lookup"><span data-stu-id="217ac-968">Core</span></span>

* <span data-ttu-id="217ac-969">Modification de l’authentification pour passer au système de clé sur l’ID d’abonnement et le nom sur la connexion MSI</span><span class="sxs-lookup"><span data-stu-id="217ac-969">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="217ac-970">ACS</span><span class="sxs-lookup"><span data-stu-id="217ac-970">ACS</span></span>

* <span data-ttu-id="217ac-971">[CHANGEMENT CASSANT] Renommage de `aks get-versions` en `aks get-upgrades` pour des raisons de précision</span><span class="sxs-lookup"><span data-stu-id="217ac-971">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="217ac-972">Modification de `aks get-versions` pour afficher les versions Kubernetes disponibles pour `aks create`</span><span class="sxs-lookup"><span data-stu-id="217ac-972">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="217ac-973">Modification des valeurs par défaut de `aks create` de manière à laisser le serveur choisir la version de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="217ac-973">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="217ac-974">Mise à jour des messages d’aide faisant référence au principal du service généré par AKS</span><span class="sxs-lookup"><span data-stu-id="217ac-974">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="217ac-975">Modification des tailles de nœud par défaut pour `aks create` pour passer de « Standard\_D1\_v2 » à « Standard\_DS1\_v2 »</span><span class="sxs-lookup"><span data-stu-id="217ac-975">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="217ac-976">Meilleure fiabilité lors de la localisation du pod de tableau de bord pour `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="217ac-976">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="217ac-977">Correction de `aks get-credentials` pour gérer les erreurs Unicode lors du chargement des fichiers de configuration Kubernetes</span><span class="sxs-lookup"><span data-stu-id="217ac-977">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="217ac-978">Ajout d’un message à `az aks install-cli` pour aider à l’obtention de `kubectl` dans `$PATH`</span><span class="sxs-lookup"><span data-stu-id="217ac-978">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="217ac-979">AppService</span><span class="sxs-lookup"><span data-stu-id="217ac-979">Appservice</span></span>

* <span data-ttu-id="217ac-980">Résolution du problème dans lequel `webapp [backup|restore]` a échoué en raison d’une référence null</span><span class="sxs-lookup"><span data-stu-id="217ac-980">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="217ac-981">Ajout de la prise en charge supplémentaire des plans App Service par défaut via `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="217ac-981">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="217ac-982">CDN</span><span class="sxs-lookup"><span data-stu-id="217ac-982">CDN</span></span>

* <span data-ttu-id="217ac-983">Ajout des commandes `cdn custom-domain [enable-https|disable-https]`</span><span class="sxs-lookup"><span data-stu-id="217ac-983">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="217ac-984">Conteneur</span><span class="sxs-lookup"><span data-stu-id="217ac-984">Container</span></span>

* <span data-ttu-id="217ac-985">Ajout de l’option `--follow` à `az container logs` pour les journaux de diffusion en continu</span><span class="sxs-lookup"><span data-stu-id="217ac-985">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="217ac-986">Ajout de la commande `container attach` qui associe les flux d’erreur et de sortie standard locaux à un conteneur d’un groupe de conteneur</span><span class="sxs-lookup"><span data-stu-id="217ac-986">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="217ac-987">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="217ac-987">CosmosDB</span></span>

* <span data-ttu-id="217ac-988">Ajout de la prise en charge de la définition de fonctionnalités</span><span class="sxs-lookup"><span data-stu-id="217ac-988">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="217ac-989">Extension</span><span class="sxs-lookup"><span data-stu-id="217ac-989">Extension</span></span>

* <span data-ttu-id="217ac-990">Ajout de la prise en charge du paramètre `--pip-proxy` pour les commandes `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="217ac-990">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="217ac-991">Ajout de la prise en charge de l’argument `--pip-extra-index-urls` pour les commandes `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="217ac-991">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="217ac-992">Commentaires</span><span class="sxs-lookup"><span data-stu-id="217ac-992">Feedback</span></span>

* <span data-ttu-id="217ac-993">Ajout d’informations d’extension aux données de télémétrie</span><span class="sxs-lookup"><span data-stu-id="217ac-993">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="217ac-994">Interactive</span><span class="sxs-lookup"><span data-stu-id="217ac-994">Interactive</span></span>

* <span data-ttu-id="217ac-995">Résolution du problème dans lequel l’utilisateur est invité à se connecter à l’aide du mode interactif dans Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="217ac-995">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="217ac-996">Correction de la régression avec les listes de saisie semi-automatique des paramètres manquants</span><span class="sxs-lookup"><span data-stu-id="217ac-996">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="217ac-997">IoT</span><span class="sxs-lookup"><span data-stu-id="217ac-997">IoT</span></span>

* <span data-ttu-id="217ac-998">Résolution du problème dans lequel `iot dps access policy [create|update]` renvoie une erreur « introuvable » en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="217ac-998">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="217ac-999">Résolution du problème dans lequel `iot dps linked-hub [create|update]` renvoie une erreur « introuvable » en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="217ac-999">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="217ac-1000">Ajout de la prise en charge de `--no-wait` pour `iot dps access policy [create|update]` et `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="217ac-1000">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="217ac-1001">Modification de `iot hub create` pour autoriser la spécification du nombre de partitions</span><span class="sxs-lookup"><span data-stu-id="217ac-1001">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="217ac-1002">Surveiller</span><span class="sxs-lookup"><span data-stu-id="217ac-1002">Monitor</span></span>

* <span data-ttu-id="217ac-1003">Correction de la commande `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="217ac-1003">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="217ac-1004">Réseau</span><span class="sxs-lookup"><span data-stu-id="217ac-1004">Network</span></span>

* <span data-ttu-id="217ac-1005">Correction de l’option `--tags` pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="217ac-1005">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="217ac-1006">Profil</span><span class="sxs-lookup"><span data-stu-id="217ac-1006">Profile</span></span>

* <span data-ttu-id="217ac-1007">Activation `az login` à partir du mode interactif</span><span class="sxs-lookup"><span data-stu-id="217ac-1007">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="217ac-1008">Ressource</span><span class="sxs-lookup"><span data-stu-id="217ac-1008">Resource</span></span>

* <span data-ttu-id="217ac-1009">Rajout de `feature show`</span><span class="sxs-lookup"><span data-stu-id="217ac-1009">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="217ac-1010">Rôle</span><span class="sxs-lookup"><span data-stu-id="217ac-1010">Role</span></span>

* <span data-ttu-id="217ac-1011">Ajout de l’argument `--available-to-other-tenants` à `ad app update`</span><span class="sxs-lookup"><span data-stu-id="217ac-1011">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="217ac-1012">SQL</span><span class="sxs-lookup"><span data-stu-id="217ac-1012">SQL</span></span>

* <span data-ttu-id="217ac-1013">Ajout des commandes `sql server dns-alias`</span><span class="sxs-lookup"><span data-stu-id="217ac-1013">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="217ac-1014">Ajout de `sql db rename`</span><span class="sxs-lookup"><span data-stu-id="217ac-1014">Added `sql db rename`</span></span>
* <span data-ttu-id="217ac-1015">Ajout de la prise en charge de l’argument `--ids` pour toutes les commandes sql</span><span class="sxs-lookup"><span data-stu-id="217ac-1015">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="217ac-1016">Stockage</span><span class="sxs-lookup"><span data-stu-id="217ac-1016">Storage</span></span>

* <span data-ttu-id="217ac-1017">Ajout des commandes `storage blob service-properties delete-policy` et `storage blob undelete` pour permettre une suppression réversible</span><span class="sxs-lookup"><span data-stu-id="217ac-1017">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="217ac-1018">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="217ac-1018">VM</span></span>

* <span data-ttu-id="217ac-1019">Correction d’un incident lorsque le chiffrement de la machine virtuelle ne peut pas être initialisé entièrement</span><span class="sxs-lookup"><span data-stu-id="217ac-1019">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="217ac-1020">Ajout de la sortie d’ID du principal lors de l’activation de MSI</span><span class="sxs-lookup"><span data-stu-id="217ac-1020">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="217ac-1021">`vm boot-diagnostics get-boot-log` fixe</span><span class="sxs-lookup"><span data-stu-id="217ac-1021">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="217ac-1022">31 janvier 2018</span><span class="sxs-lookup"><span data-stu-id="217ac-1022">January 31, 2018</span></span>

<span data-ttu-id="217ac-1023">Version 2.0.26</span><span class="sxs-lookup"><span data-stu-id="217ac-1023">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="217ac-1024">Principal</span><span class="sxs-lookup"><span data-stu-id="217ac-1024">Core</span></span>

* <span data-ttu-id="217ac-1025">Ajout de la prise en charge de la récupération du jeton brut dans le contexte MSI</span><span class="sxs-lookup"><span data-stu-id="217ac-1025">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="217ac-1026">Suppression de la chaîne de l’indicateur d’interrogation après la fin de LRO sur le fichier cmd.exe de Windows</span><span class="sxs-lookup"><span data-stu-id="217ac-1026">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="217ac-1027">Ajout d’un avertissement qui s’affiche lorsque l’utilisation d’une valeur par défaut configurée a été remplacée par une entrée de niveau INFO.</span><span class="sxs-lookup"><span data-stu-id="217ac-1027">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="217ac-1028">Utilisation de `--verbose` pour voir</span><span class="sxs-lookup"><span data-stu-id="217ac-1028">Use `--verbose` to see</span></span>
* <span data-ttu-id="217ac-1029">Ajouter un indicateur de progression pour les commandes wait</span><span class="sxs-lookup"><span data-stu-id="217ac-1029">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="217ac-1030">ACS</span><span class="sxs-lookup"><span data-stu-id="217ac-1030">ACS</span></span>

* <span data-ttu-id="217ac-1031">Clarification de l’argument `--disable-browser`</span><span class="sxs-lookup"><span data-stu-id="217ac-1031">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="217ac-1032">Amélioration de la touche TAB pour les arguments `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="217ac-1032">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="217ac-1033">AppService</span><span class="sxs-lookup"><span data-stu-id="217ac-1033">Appservice</span></span>

* <span data-ttu-id="217ac-1034">`webapp log [tail|download]` fixe</span><span class="sxs-lookup"><span data-stu-id="217ac-1034">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="217ac-1035">Suppression de la vérification de `kind` sur les fonctions et les applications web</span><span class="sxs-lookup"><span data-stu-id="217ac-1035">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="217ac-1036">CDN</span><span class="sxs-lookup"><span data-stu-id="217ac-1036">CDN</span></span>

* <span data-ttu-id="217ac-1037">Résolution du problème de client manquant avec `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="217ac-1037">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="217ac-1038">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="217ac-1038">CosmosDB</span></span>

* <span data-ttu-id="217ac-1039">Correction de la description du paramètre pour les stratégies de basculement</span><span class="sxs-lookup"><span data-stu-id="217ac-1039">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="217ac-1040">Interactive</span><span class="sxs-lookup"><span data-stu-id="217ac-1040">Interactive</span></span>

* <span data-ttu-id="217ac-1041">Résolution du problème dans lequel les listes de saisie semi-automatique d’option de commande ne s’affichent plus</span><span class="sxs-lookup"><span data-stu-id="217ac-1041">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="217ac-1042">Réseau</span><span class="sxs-lookup"><span data-stu-id="217ac-1042">Network</span></span>

* <span data-ttu-id="217ac-1043">Ajout de la protection pour `--cert-password` à `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="217ac-1043">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="217ac-1044">Résolution du problème lié à `application-gateway update` où `--sku` a appliqué par erreur une valeur par défaut</span><span class="sxs-lookup"><span data-stu-id="217ac-1044">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="217ac-1045">Ajout de la protection pour `--shared-key` et `--authorization-key` à `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="217ac-1045">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="217ac-1046">Résolution du problème de client manquant avec `asg create`</span><span class="sxs-lookup"><span data-stu-id="217ac-1046">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="217ac-1047">Ajout du paramètre `--file-name / -f` pour les noms exportés à `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="217ac-1047">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="217ac-1048">Les problèmes suivants liés à `dns zone export` ont été résolus :</span><span class="sxs-lookup"><span data-stu-id="217ac-1048">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="217ac-1049">Résolution du problème dans lequel des enregistrements TXT longs ont été mal exportés</span><span class="sxs-lookup"><span data-stu-id="217ac-1049">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="217ac-1050">Résolution du problème dans lequel des enregistrements TXT entre guillemets ont été mal exportés sans guillemets placés dans une séquence d’échappement.</span><span class="sxs-lookup"><span data-stu-id="217ac-1050">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="217ac-1051">Résolution du problème où certains enregistrements ont été importés à deux reprises avec `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="217ac-1051">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="217ac-1052">Restauration des commandes `vnet-gateway root-cert` et `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="217ac-1052">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="217ac-1053">Profil</span><span class="sxs-lookup"><span data-stu-id="217ac-1053">Profile</span></span>

* <span data-ttu-id="217ac-1054">Correction de `get-access-token` pour qu’il fonctionne à l’intérieur d’une machine virtuelle avec l’identité</span><span class="sxs-lookup"><span data-stu-id="217ac-1054">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="217ac-1055">Ressource</span><span class="sxs-lookup"><span data-stu-id="217ac-1055">Resource</span></span>

* <span data-ttu-id="217ac-1056">Correction du bogue lié à `deployment [create|validate]` où un avertissement ne s’est pas affiché correctement quand un champ ’type’ du modèle contient des valeurs en majuscules</span><span class="sxs-lookup"><span data-stu-id="217ac-1056">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="217ac-1057">Stockage</span><span class="sxs-lookup"><span data-stu-id="217ac-1057">Storage</span></span>

* <span data-ttu-id="217ac-1058">Résolution du problème lié à la migration des comptes Storage V1 vers Storage V2</span><span class="sxs-lookup"><span data-stu-id="217ac-1058">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="217ac-1059">Ajout de la création progressive de rapports pour toutes les commandes de chargement/téléchargement</span><span class="sxs-lookup"><span data-stu-id="217ac-1059">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="217ac-1060">Résolution du bogue empêchant l’option d’argument « -n » avec `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="217ac-1060">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="217ac-1061">Ajout de la colonne de « snapshot » ajouté à la sortie de table pour `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="217ac-1061">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="217ac-1062">Résolution des bogues dans lesquels différents paramètres devaient être analysés en tant qu’entiers</span><span class="sxs-lookup"><span data-stu-id="217ac-1062">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="217ac-1063">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="217ac-1063">VM</span></span>

* <span data-ttu-id="217ac-1064">Ajout de la commande `vm image accept-terms` pour autoriser la création de machines virtuelles à partir d’images moyennant des frais supplémentaires</span><span class="sxs-lookup"><span data-stu-id="217ac-1064">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="217ac-1065">Correction de `[vm|vmss create]` pour garantir l’exécution des commandes sous un proxy avec des certificats non signés</span><span class="sxs-lookup"><span data-stu-id="217ac-1065">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="217ac-1066">[APERÇU] Ajout de la prise en charge de la priorité « faible» au groupe de machines virtuelles identiques</span><span class="sxs-lookup"><span data-stu-id="217ac-1066">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="217ac-1067">Ajout de la protection pour `--admin-password` à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="217ac-1067">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="217ac-1068">17 janvier 2018</span><span class="sxs-lookup"><span data-stu-id="217ac-1068">January 17, 2018</span></span>

<span data-ttu-id="217ac-1069">Version 2.0.25</span><span class="sxs-lookup"><span data-stu-id="217ac-1069">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="217ac-1070">ACR</span><span class="sxs-lookup"><span data-stu-id="217ac-1070">ACR</span></span>

* <span data-ttu-id="217ac-1071">Ajout d’une connexion acr de secours en cas d’erreurs d’informations d’identification Windows</span><span class="sxs-lookup"><span data-stu-id="217ac-1071">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="217ac-1072">Activation des journaux du Registre</span><span class="sxs-lookup"><span data-stu-id="217ac-1072">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="217ac-1073">ACS</span><span class="sxs-lookup"><span data-stu-id="217ac-1073">ACS</span></span>

* <span data-ttu-id="217ac-1074">Correction de la commande `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="217ac-1074">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="217ac-1075">Suppression de l’exigence de rôle SPN</span><span class="sxs-lookup"><span data-stu-id="217ac-1075">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="217ac-1076">AppService</span><span class="sxs-lookup"><span data-stu-id="217ac-1076">Appservice</span></span>

* <span data-ttu-id="217ac-1077">Correction du bogue avec `config ssl upload` où `hosting_environment_profile` avait la valeur null</span><span class="sxs-lookup"><span data-stu-id="217ac-1077">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="217ac-1078">Ajout de la prise en charge des URL personnalisées pour `browse`</span><span class="sxs-lookup"><span data-stu-id="217ac-1078">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="217ac-1079">Prise en charge de l’emplacement fixe pour `log tail`</span><span class="sxs-lookup"><span data-stu-id="217ac-1079">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="217ac-1080">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="217ac-1080">Backup</span></span>

* <span data-ttu-id="217ac-1081">Modification de l’option `--container-name` de `backup item list` désormais facultative</span><span class="sxs-lookup"><span data-stu-id="217ac-1081">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="217ac-1082">Ajout d’options de compte de stockage à `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="217ac-1082">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="217ac-1083">Correction de la vérification de l’emplacement dans `backup protection enable-for-vm`, ne tient désormais plus compte de la casse</span><span class="sxs-lookup"><span data-stu-id="217ac-1083">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="217ac-1084">Correction d’un problème qui causait l’échec des commandes avec un nom de conteneur non valide</span><span class="sxs-lookup"><span data-stu-id="217ac-1084">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="217ac-1085">Modification de `backup item list` pour inclure « État d’intégrité » par défaut</span><span class="sxs-lookup"><span data-stu-id="217ac-1085">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="217ac-1086">Batch</span><span class="sxs-lookup"><span data-stu-id="217ac-1086">Batch</span></span>

* <span data-ttu-id="217ac-1087">Modification de `batch login` pour retourner des détails d’authentification</span><span class="sxs-lookup"><span data-stu-id="217ac-1087">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="217ac-1088">Cloud</span><span class="sxs-lookup"><span data-stu-id="217ac-1088">Cloud</span></span>

* <span data-ttu-id="217ac-1089">Ne requiert plus de points de terminaison lors de la définition de `--profile` sur un cloud</span><span class="sxs-lookup"><span data-stu-id="217ac-1089">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="217ac-1090">Consommation</span><span class="sxs-lookup"><span data-stu-id="217ac-1090">Consumption</span></span>

* <span data-ttu-id="217ac-1091">Ajout de nouvelles commandes pour les réservations : `consumption reservations summaries` et `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="217ac-1091">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="217ac-1092">Event Grid</span><span class="sxs-lookup"><span data-stu-id="217ac-1092">Event Grid</span></span>

* <span data-ttu-id="217ac-1093">[CHANGEMENT CASSANT] Déplacement des commandes `az eventgrid topic event-subscription` vers `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="217ac-1093">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="217ac-1094">[CHANGEMENT CASSANT] Déplacement des commandes `az eventgrid resource event-subscription` vers `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="217ac-1094">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="217ac-1095">[CHANGEMENT CASSANT] Suppression de la commande `eventgrid event-subscription show-endpoint-url`</span><span class="sxs-lookup"><span data-stu-id="217ac-1095">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="217ac-1096">Utilisation de `eventgrid event-subscription show --include-full-endpoint-url` à la place</span><span class="sxs-lookup"><span data-stu-id="217ac-1096">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="217ac-1097">Ajout de la commande `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="217ac-1097">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="217ac-1098">Ajout de la commande `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="217ac-1098">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="217ac-1099">Ajout du paramètre `--ids` pour les commandes `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="217ac-1099">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="217ac-1100">Ajout de la prise en charge de la saisie semi-automatique via la touche TAB pour les noms de rubrique</span><span class="sxs-lookup"><span data-stu-id="217ac-1100">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="217ac-1101">Interactive</span><span class="sxs-lookup"><span data-stu-id="217ac-1101">Interactive</span></span>

* <span data-ttu-id="217ac-1102">Correction d’un problème qui empêchait le fonctionnement du mode interactif avec Python 2.x</span><span class="sxs-lookup"><span data-stu-id="217ac-1102">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="217ac-1103">Corrections d’erreurs au démarrage</span><span class="sxs-lookup"><span data-stu-id="217ac-1103">Fixed errors on startup</span></span>
* <span data-ttu-id="217ac-1104">Correction du problème de commandes ne s’exécutant pas en mode interactif</span><span class="sxs-lookup"><span data-stu-id="217ac-1104">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="217ac-1105">IoT</span><span class="sxs-lookup"><span data-stu-id="217ac-1105">IoT</span></span>

* <span data-ttu-id="217ac-1106">Ajout de la prise en charge du service de provisionnement des appareils</span><span class="sxs-lookup"><span data-stu-id="217ac-1106">Added support for device provisioning service</span></span>
* <span data-ttu-id="217ac-1107">Ajout de messages de désapprobation dans les commandes et l’aide relative aux commandes</span><span class="sxs-lookup"><span data-stu-id="217ac-1107">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="217ac-1108">Ajout de la vérification IoT pour informer les utilisateurs de l’extension IoT</span><span class="sxs-lookup"><span data-stu-id="217ac-1108">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="217ac-1109">Surveiller</span><span class="sxs-lookup"><span data-stu-id="217ac-1109">Monitor</span></span>

* <span data-ttu-id="217ac-1110">Ajout de la prise en charge des paramètres multi diagnostic.</span><span class="sxs-lookup"><span data-stu-id="217ac-1110">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="217ac-1111">Le paramètre `--name` est désormais requis pour `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="217ac-1111">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="217ac-1112">Ajout de la commande `monitor diagnostic-settings categories` pour obtenir la catégorie des paramètres de diagnostic</span><span class="sxs-lookup"><span data-stu-id="217ac-1112">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="217ac-1113">Réseau</span><span class="sxs-lookup"><span data-stu-id="217ac-1113">Network</span></span>

* <span data-ttu-id="217ac-1114">Résolution du problème se produisant lors de la tentative de passage au mode actif-passif, ou depuis ce dernier, avec `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="217ac-1114">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="217ac-1115">Ajout de la prise en charge de HTTP2 vers `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="217ac-1115">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="217ac-1116">Profil</span><span class="sxs-lookup"><span data-stu-id="217ac-1116">Profile</span></span>

* <span data-ttu-id="217ac-1117">Ajout de la prise en charge pour la connexion à l’aide d’identités affectées aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="217ac-1117">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="217ac-1118">Rôle</span><span class="sxs-lookup"><span data-stu-id="217ac-1118">Role</span></span>

* <span data-ttu-id="217ac-1119">Ajout de l’argument `--assignee-object-id` à `role assignment create` pour ignorer les requêtes de graphique</span><span class="sxs-lookup"><span data-stu-id="217ac-1119">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="217ac-1120">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="217ac-1120">Service Fabric</span></span>

* <span data-ttu-id="217ac-1121">Ajout d’erreurs détaillées à la réponse de validation lors de la création du cluster</span><span class="sxs-lookup"><span data-stu-id="217ac-1121">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="217ac-1122">Résolution du problème concernant le client manquant avec plusieurs commandes</span><span class="sxs-lookup"><span data-stu-id="217ac-1122">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="217ac-1123">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="217ac-1123">VM</span></span>

* <span data-ttu-id="217ac-1124">[PRÉVERSION] Prise en charge interzone pour `vmss`</span><span class="sxs-lookup"><span data-stu-id="217ac-1124">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="217ac-1125">[CHANGEMENT CASSANT] Modification de la valeur par défaut `vmss` de zone unique en équilibreur de charge « Standard »</span><span class="sxs-lookup"><span data-stu-id="217ac-1125">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="217ac-1126">[CHANGEMENT CASSANT] Modification de `externalIdentities` en `userAssignedIdentities` pour EMSI</span><span class="sxs-lookup"><span data-stu-id="217ac-1126">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="217ac-1127">[PRÉVERSION] Ajout de la prise en charge de l’échange de disque du système d’exploitation</span><span class="sxs-lookup"><span data-stu-id="217ac-1127">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="217ac-1128">Ajout de la prise en charge de l’utilisation des images de machine virtuelle à partir d’autres abonnements</span><span class="sxs-lookup"><span data-stu-id="217ac-1128">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="217ac-1129">Ajout des arguments `--plan-name`, `--plan-product`, `--plan-promotion-code` et `--plan-publisher` à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="217ac-1129">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="217ac-1130">Correction des problèmes d’erreur avec `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="217ac-1130">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="217ac-1131">Correction de l’utilisation excessive des ressources due à `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="217ac-1131">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="217ac-1132">19 décembre 2017</span><span class="sxs-lookup"><span data-stu-id="217ac-1132">December 19, 2017</span></span>

<span data-ttu-id="217ac-1133">Version 2.0.23</span><span class="sxs-lookup"><span data-stu-id="217ac-1133">Version 2.0.23</span></span>

* <span data-ttu-id="217ac-1134">Ajout de la prise en charge pour la connexion à l’aide d’identités affectées aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="217ac-1134">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="217ac-1135">Conteneur</span><span class="sxs-lookup"><span data-stu-id="217ac-1135">Container</span></span>

* <span data-ttu-id="217ac-1136">Correction de l’ordre incorrect des paramètres pour les journaux du conteneur</span><span class="sxs-lookup"><span data-stu-id="217ac-1136">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="217ac-1137">Réseau</span><span class="sxs-lookup"><span data-stu-id="217ac-1137">Network</span></span>

* <span data-ttu-id="217ac-1138">Ajout de l’argument `--disable-bgp-route-propagation` à `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="217ac-1138">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="217ac-1139">Ajout de l’argument `--ip-tags` à `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="217ac-1139">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="217ac-1140">Stockage</span><span class="sxs-lookup"><span data-stu-id="217ac-1140">Storage</span></span>

* <span data-ttu-id="217ac-1141">Ajout de la prise en charge du stockage V2</span><span class="sxs-lookup"><span data-stu-id="217ac-1141">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="217ac-1142">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="217ac-1142">VM</span></span>

* <span data-ttu-id="217ac-1143">[APERÇU] Ajout de la prise en charge des identités affectées aux utilisateurs pour les machines virtuelles et les VMSS</span><span class="sxs-lookup"><span data-stu-id="217ac-1143">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="217ac-1144">5 décembre 2017</span><span class="sxs-lookup"><span data-stu-id="217ac-1144">December 5, 2017</span></span>

<span data-ttu-id="217ac-1145">Version 2.0.22</span><span class="sxs-lookup"><span data-stu-id="217ac-1145">Version 2.0.22</span></span>

* <span data-ttu-id="217ac-1146">Suppression des commandes `az component`.</span><span class="sxs-lookup"><span data-stu-id="217ac-1146">Removed `az component` commands.</span></span> <span data-ttu-id="217ac-1147">Utilisation de `az extension` à la place</span><span class="sxs-lookup"><span data-stu-id="217ac-1147">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="217ac-1148">Principal</span><span class="sxs-lookup"><span data-stu-id="217ac-1148">Core</span></span>
* <span data-ttu-id="217ac-1149">Modification du point de terminaison de l’autorité AAD `AZURE_US_GOV_CLOUD` pour le faire passer de login.microsoftonline.com à login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="217ac-1149">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="217ac-1150">Résolution du problème au cours duquel les données de télémétrie étaient constamment renvoyées</span><span class="sxs-lookup"><span data-stu-id="217ac-1150">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="217ac-1151">ACS</span><span class="sxs-lookup"><span data-stu-id="217ac-1151">ACS</span></span>

* <span data-ttu-id="217ac-1152">Ajout des commandes `aks install-connector` et `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="217ac-1152">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="217ac-1153">Amélioration des rapports d’erreurs pour `acs create`</span><span class="sxs-lookup"><span data-stu-id="217ac-1153">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="217ac-1154">Correction de l’utilisation de `aks get-credentials -f` sans chemin d’accès complet</span><span class="sxs-lookup"><span data-stu-id="217ac-1154">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="217ac-1155">Advisor</span><span class="sxs-lookup"><span data-stu-id="217ac-1155">Advisor</span></span>

* <span data-ttu-id="217ac-1156">Version initiale</span><span class="sxs-lookup"><span data-stu-id="217ac-1156">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="217ac-1157">AppService</span><span class="sxs-lookup"><span data-stu-id="217ac-1157">Appservice</span></span>

* <span data-ttu-id="217ac-1158">Correction de la génération du nom de certificat avec `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="217ac-1158">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="217ac-1159">Correction de `webapp [list|show]` et `functionapp [list|show]` de manière à afficher les applications correctes</span><span class="sxs-lookup"><span data-stu-id="217ac-1159">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="217ac-1160">Ajout de la valeur par défaut pour `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="217ac-1160">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="217ac-1161">Consommation</span><span class="sxs-lookup"><span data-stu-id="217ac-1161">Consumption</span></span>

* <span data-ttu-id="217ac-1162">Ajout de la prise en charge de l’API version 2017-11-30</span><span class="sxs-lookup"><span data-stu-id="217ac-1162">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="217ac-1163">Conteneur</span><span class="sxs-lookup"><span data-stu-id="217ac-1163">Container</span></span>

* <span data-ttu-id="217ac-1164">Correction de la régression des ports par défaut</span><span class="sxs-lookup"><span data-stu-id="217ac-1164">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="217ac-1165">Surveiller</span><span class="sxs-lookup"><span data-stu-id="217ac-1165">Monitor</span></span>

* <span data-ttu-id="217ac-1166">Ajout de la prise en charge de plusieurs dimensions à la commande des mesures</span><span class="sxs-lookup"><span data-stu-id="217ac-1166">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="217ac-1167">Ressource</span><span class="sxs-lookup"><span data-stu-id="217ac-1167">Resource</span></span>

* <span data-ttu-id="217ac-1168">Ajout de l’argument `--include-response-body` à `resource show`</span><span class="sxs-lookup"><span data-stu-id="217ac-1168">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="217ac-1169">Rôle</span><span class="sxs-lookup"><span data-stu-id="217ac-1169">Role</span></span>

* <span data-ttu-id="217ac-1170">Ajout de l’affichage des affectations par défaut pour les administrateurs « classiques » à `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="217ac-1170">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="217ac-1171">Ajout de la prise en charge à `ad sp reset-credentials` pour l’ajout d’informations d’identification au lieu de leur remplacement</span><span class="sxs-lookup"><span data-stu-id="217ac-1171">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="217ac-1172">Amélioration des rapports d’erreurs pour `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="217ac-1172">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="217ac-1173">SQL</span><span class="sxs-lookup"><span data-stu-id="217ac-1173">SQL</span></span>

* <span data-ttu-id="217ac-1174">Ajout des commandes `sql db list-usages` et `sql db show-usage`</span><span class="sxs-lookup"><span data-stu-id="217ac-1174">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="217ac-1175">Ajout des commandes `sql server conn-policy show` et `sql server conn-policy update`</span><span class="sxs-lookup"><span data-stu-id="217ac-1175">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="217ac-1176">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="217ac-1176">VM</span></span>

* <span data-ttu-id="217ac-1177">Ajout des informations de zone à `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="217ac-1177">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="217ac-1178">14 novembre 2017</span><span class="sxs-lookup"><span data-stu-id="217ac-1178">November 14, 2017</span></span>

<span data-ttu-id="217ac-1179">Version 2.0.21</span><span class="sxs-lookup"><span data-stu-id="217ac-1179">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="217ac-1180">ACR</span><span class="sxs-lookup"><span data-stu-id="217ac-1180">ACR</span></span>

* <span data-ttu-id="217ac-1181">Ajout de la prise en charge pour la création de webhooks dans les régions de réplication</span><span class="sxs-lookup"><span data-stu-id="217ac-1181">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="217ac-1182">ACS</span><span class="sxs-lookup"><span data-stu-id="217ac-1182">ACS</span></span>

* <span data-ttu-id="217ac-1183">Modification de toutes les mentions « agent » en « nœud » dans AKS</span><span class="sxs-lookup"><span data-stu-id="217ac-1183">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="217ac-1184">Option `--orchestrator-release` déconseillée pour `acs create`</span><span class="sxs-lookup"><span data-stu-id="217ac-1184">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="217ac-1185">Changement de la taille de machine virtuelle par défaut pour AKS à `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="217ac-1185">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="217ac-1186">Résolution de `az aks browse` sur Windows</span><span class="sxs-lookup"><span data-stu-id="217ac-1186">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="217ac-1187">Résolution de `az aks get-credentials` sur Windows</span><span class="sxs-lookup"><span data-stu-id="217ac-1187">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="217ac-1188">AppService</span><span class="sxs-lookup"><span data-stu-id="217ac-1188">Appservice</span></span>

* <span data-ttu-id="217ac-1189">Ajout de la source de déploiement `config-zip` pour les applications Web et de fonction</span><span class="sxs-lookup"><span data-stu-id="217ac-1189">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="217ac-1190">Ajout de l’option `--docker-container-logging` à `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="217ac-1190">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="217ac-1191">Suppression de l’option `storage` du paramètre `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="217ac-1191">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="217ac-1192">Amélioration des messages d’erreur pour `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="217ac-1192">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="217ac-1193">Ajout de la prise en charge pour la création d’applications de fonction Linux</span><span class="sxs-lookup"><span data-stu-id="217ac-1193">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="217ac-1194">`list-locations` fixe</span><span class="sxs-lookup"><span data-stu-id="217ac-1194">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="217ac-1195">Batch</span><span class="sxs-lookup"><span data-stu-id="217ac-1195">Batch</span></span>

* <span data-ttu-id="217ac-1196">Correction du bogue dans la commande de création de pool lorsqu’un ID ressource a été utilisé avec l’indicateur `--image`</span><span class="sxs-lookup"><span data-stu-id="217ac-1196">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="217ac-1197">Batchai</span><span class="sxs-lookup"><span data-stu-id="217ac-1197">Batchai</span></span>

* <span data-ttu-id="217ac-1198">Ajout de l’option courte, `-s`, pour `--vm-size` quand la taille de machine virtuelle est fournie dans la commande `file-server create`</span><span class="sxs-lookup"><span data-stu-id="217ac-1198">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="217ac-1199">Ajout du nom de compte de stockage et des arguments de clé dans les paramètres `cluster create`</span><span class="sxs-lookup"><span data-stu-id="217ac-1199">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="217ac-1200">Résolution de la documentation pour `job list-files` et `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="217ac-1200">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="217ac-1201">Ajout de l’option courte, `-r`, pour `--cluster-name` quand le nom du cluster est fourni dans la commande `job create`</span><span class="sxs-lookup"><span data-stu-id="217ac-1201">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="217ac-1202">Cloud</span><span class="sxs-lookup"><span data-stu-id="217ac-1202">Cloud</span></span>

* <span data-ttu-id="217ac-1203">Modification de `cloud [register|update]` pour empêcher l’inscription des clouds qui ne disposent pas de tous les points de terminaison requis</span><span class="sxs-lookup"><span data-stu-id="217ac-1203">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="217ac-1204">Conteneur</span><span class="sxs-lookup"><span data-stu-id="217ac-1204">Container</span></span>

* <span data-ttu-id="217ac-1205">Ajout de la prise en charge pour ouvrir plusieurs ports</span><span class="sxs-lookup"><span data-stu-id="217ac-1205">Added support to open multiple ports</span></span>
* <span data-ttu-id="217ac-1206">Ajout de la stratégie de redémarrage du groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="217ac-1206">Added container group restart policy</span></span>
* <span data-ttu-id="217ac-1207">Ajout de la prise en charge pour monter le partage de fichier Azure en tant que volume</span><span class="sxs-lookup"><span data-stu-id="217ac-1207">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="217ac-1208">Mise à jour des documents d’assistance</span><span class="sxs-lookup"><span data-stu-id="217ac-1208">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="217ac-1209">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="217ac-1209">Data Lake Analytics</span></span>

* <span data-ttu-id="217ac-1210">Modification de `[job|account] list` pour retourner des informations plus concises</span><span class="sxs-lookup"><span data-stu-id="217ac-1210">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="217ac-1211">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="217ac-1211">Data Lake Store</span></span>

* <span data-ttu-id="217ac-1212">Modification de `account list` pour retourner des informations plus concises</span><span class="sxs-lookup"><span data-stu-id="217ac-1212">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="217ac-1213">Extension</span><span class="sxs-lookup"><span data-stu-id="217ac-1213">Extension</span></span>

* <span data-ttu-id="217ac-1214">Ajout de `extension list-available` pour permettre l’affichage de la liste des extensions officielles Microsoft</span><span class="sxs-lookup"><span data-stu-id="217ac-1214">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="217ac-1215">Ajout de `--name` à `extension [add|update]` pour permettre l’installation des extensions par nom</span><span class="sxs-lookup"><span data-stu-id="217ac-1215">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="217ac-1216">IoT</span><span class="sxs-lookup"><span data-stu-id="217ac-1216">IoT</span></span>

* <span data-ttu-id="217ac-1217">Ajout de la prise en charge pour les autorités de certification (CA) et les chaînes d’approbation</span><span class="sxs-lookup"><span data-stu-id="217ac-1217">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="217ac-1218">Surveiller</span><span class="sxs-lookup"><span data-stu-id="217ac-1218">Monitor</span></span>

* <span data-ttu-id="217ac-1219">Ajout des commandes `activity-log alert`</span><span class="sxs-lookup"><span data-stu-id="217ac-1219">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="217ac-1220">Réseau</span><span class="sxs-lookup"><span data-stu-id="217ac-1220">Network</span></span>

* <span data-ttu-id="217ac-1221">Ajout de la prise en charge pour les enregistrements DNS CAA</span><span class="sxs-lookup"><span data-stu-id="217ac-1221">Added support for CAA DNS records</span></span>
* <span data-ttu-id="217ac-1222">Résolution d’un problème empêchant la mise à jour des points de terminaison avec `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="217ac-1222">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="217ac-1223">Résolution d’un problème où `vnet update --dns-servers` ne fonctionnait pas, en fonction de la façon dont avait été créé le réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="217ac-1223">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="217ac-1224">Résolution d’un problème où les noms DNS relatifs n’étaient pas importés correctement par `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="217ac-1224">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="217ac-1225">Réservations</span><span class="sxs-lookup"><span data-stu-id="217ac-1225">Reservations</span></span>

* <span data-ttu-id="217ac-1226">Version préliminaire initiale</span><span class="sxs-lookup"><span data-stu-id="217ac-1226">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="217ac-1227">Ressource</span><span class="sxs-lookup"><span data-stu-id="217ac-1227">Resource</span></span>

* <span data-ttu-id="217ac-1228">Ajout de la prise en charge pour les ID de ressource au paramètre `--resource` et pour les verrous au niveau des ressources</span><span class="sxs-lookup"><span data-stu-id="217ac-1228">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="217ac-1229">SQL</span><span class="sxs-lookup"><span data-stu-id="217ac-1229">SQL</span></span>

* <span data-ttu-id="217ac-1230">Ajout du paramètre `--ignore-missing-vnet-service-endpoint` pour `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="217ac-1230">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="217ac-1231">Stockage</span><span class="sxs-lookup"><span data-stu-id="217ac-1231">Storage</span></span>

* <span data-ttu-id="217ac-1232">Modification de `storage account create` pour utiliser la référence SKU `Standard_RAGRS` par défaut</span><span class="sxs-lookup"><span data-stu-id="217ac-1232">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="217ac-1233">Correction du bogue lors du traitement des noms d’objets blob/de fichier qui incluent des caractères non-ascii</span><span class="sxs-lookup"><span data-stu-id="217ac-1233">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="217ac-1234">Correction du bogue qui empêchait l’utilisation de `--source-uri` avec `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="217ac-1234">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="217ac-1235">Ajout de commandes pour paramétrer et supprimer plusieurs objets avec `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="217ac-1235">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="217ac-1236">Résolution du problème de l’activation des métriques avec `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="217ac-1236">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="217ac-1237">Résolution du problème des fichiers de plus de 200 Go lors de l’utilisation de `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="217ac-1237">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="217ac-1238">Résolution du problème où `--bypass` et `--default-action` étaient ignorés par `storage account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="217ac-1238">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="217ac-1239">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="217ac-1239">VM</span></span>

* <span data-ttu-id="217ac-1240">Correction d’un bogue avec `vmss create` qui empêchait l’utilisation du niveau de taille `Basic`</span><span class="sxs-lookup"><span data-stu-id="217ac-1240">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="217ac-1241">Ajout d’arguments `--plan` à `[vm|vmss] create` pour les images personnalisées avec des informations de facturation</span><span class="sxs-lookup"><span data-stu-id="217ac-1241">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="217ac-1242">Ajout des commandes `vm secret `[add|remove|list]</span><span class="sxs-lookup"><span data-stu-id="217ac-1242">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="217ac-1243">Renommage de `vm format-secret` en `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="217ac-1243">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="217ac-1244">Ajout de l’argument `--encrypt format` à `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="217ac-1244">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="217ac-1245">24 octobre 2017</span><span class="sxs-lookup"><span data-stu-id="217ac-1245">October 24, 2017</span></span>

<span data-ttu-id="217ac-1246">Version 2.0.20</span><span class="sxs-lookup"><span data-stu-id="217ac-1246">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="217ac-1247">Principal</span><span class="sxs-lookup"><span data-stu-id="217ac-1247">Core</span></span>

* <span data-ttu-id="217ac-1248">Mise à jour de `2017-03-09-profile` pour consommer l’API `MGMT_STORAGE` version `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="217ac-1248">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="217ac-1249">ACR</span><span class="sxs-lookup"><span data-stu-id="217ac-1249">ACR</span></span>

* <span data-ttu-id="217ac-1250">Mise à jour de la gestion des ressources pour pointer vers la version d’API `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="217ac-1250">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="217ac-1251">Modification de la référence SKU « Bring Your Own Storage » en Classique</span><span class="sxs-lookup"><span data-stu-id="217ac-1251">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="217ac-1252">Changement des noms des références SKU de registre en De base, Standard, et Premium</span><span class="sxs-lookup"><span data-stu-id="217ac-1252">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="217ac-1253">ACS</span><span class="sxs-lookup"><span data-stu-id="217ac-1253">ACS</span></span>

* <span data-ttu-id="217ac-1254">[PRÉVERSION] Ajout des commandes `az aks`</span><span class="sxs-lookup"><span data-stu-id="217ac-1254">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="217ac-1255">Réparation de Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="217ac-1255">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="217ac-1256">AppService</span><span class="sxs-lookup"><span data-stu-id="217ac-1256">Appservice</span></span>

* <span data-ttu-id="217ac-1257">Résolution d’une erreur où le téléchargement des journaux `webapp` était incorrect</span><span class="sxs-lookup"><span data-stu-id="217ac-1257">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="217ac-1258">Composant</span><span class="sxs-lookup"><span data-stu-id="217ac-1258">Component</span></span>

* <span data-ttu-id="217ac-1259">Ajout de clarté dans les messages visant à déconseiller de tous les programmes d’installation et des invites de confirmation</span><span class="sxs-lookup"><span data-stu-id="217ac-1259">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="217ac-1260">Surveiller</span><span class="sxs-lookup"><span data-stu-id="217ac-1260">Monitor</span></span>

* <span data-ttu-id="217ac-1261">Ajout des commandes `action-group`</span><span class="sxs-lookup"><span data-stu-id="217ac-1261">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="217ac-1262">Ressource</span><span class="sxs-lookup"><span data-stu-id="217ac-1262">Resource</span></span>

* <span data-ttu-id="217ac-1263">Résolution d’une incompatibilité de la dépendance msrest dans `group export` avec les versions les plus récentes</span><span class="sxs-lookup"><span data-stu-id="217ac-1263">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="217ac-1264">Résolution de `policy assignment create` pour qu’il fonctionne avec les définitions de stratégie et les définitions d’ensemble de stratégie intégrées</span><span class="sxs-lookup"><span data-stu-id="217ac-1264">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="217ac-1265">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="217ac-1265">VM</span></span>

* <span data-ttu-id="217ac-1266">Ajout de l’argument `--accelerated-networking` à `vmss create`</span><span class="sxs-lookup"><span data-stu-id="217ac-1266">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="217ac-1267">9 octobre 2017</span><span class="sxs-lookup"><span data-stu-id="217ac-1267">October 9, 2017</span></span>

<span data-ttu-id="217ac-1268">Version 2.0.19</span><span class="sxs-lookup"><span data-stu-id="217ac-1268">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="217ac-1269">Principal</span><span class="sxs-lookup"><span data-stu-id="217ac-1269">Core</span></span>

* <span data-ttu-id="217ac-1270">Ajout de la gestion des URL d’autorisation AD FS avec une barre oblique à Azure Stack</span><span class="sxs-lookup"><span data-stu-id="217ac-1270">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="217ac-1271">AppService</span><span class="sxs-lookup"><span data-stu-id="217ac-1271">Appservice</span></span>

* <span data-ttu-id="217ac-1272">Ajout de la mise à jour générique avec la nouvelle commande `webapp update`</span><span class="sxs-lookup"><span data-stu-id="217ac-1272">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="217ac-1273">Batch</span><span class="sxs-lookup"><span data-stu-id="217ac-1273">Batch</span></span>

* <span data-ttu-id="217ac-1274">Mis à jour du kit de développement logiciel (SDK) à la version 4.0.0</span><span class="sxs-lookup"><span data-stu-id="217ac-1274">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="217ac-1275">Mise à jour de l’option `--image` de VirtualMachineConfiguration pour prendre en charge les références d’image ARM en plus de publish:offre:sku:version</span><span class="sxs-lookup"><span data-stu-id="217ac-1275">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="217ac-1276">Ajout de la prise en charge du nouveau modèle d’extension CLI pour les commandes d’extension Batch</span><span class="sxs-lookup"><span data-stu-id="217ac-1276">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="217ac-1277">Suppression de la prise en charge Batch des modèles de composants</span><span class="sxs-lookup"><span data-stu-id="217ac-1277">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="217ac-1278">Batchai</span><span class="sxs-lookup"><span data-stu-id="217ac-1278">Batchai</span></span>

* <span data-ttu-id="217ac-1279">Version initiale du module Batch AI</span><span class="sxs-lookup"><span data-stu-id="217ac-1279">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="217ac-1280">KeyVault</span><span class="sxs-lookup"><span data-stu-id="217ac-1280">Keyvault</span></span>

* <span data-ttu-id="217ac-1281">Résolution du problème d’authentification Key Vault lors de l’utilisation d’AD FS sur Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="217ac-1281">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="217ac-1282">(#4448)</span><span class="sxs-lookup"><span data-stu-id="217ac-1282">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="217ac-1283">Réseau</span><span class="sxs-lookup"><span data-stu-id="217ac-1283">Network</span></span>

* <span data-ttu-id="217ac-1284">La modification de l’argument `--server` de `application-gateway address-pool create` devient facultative, permettant les pools d’adresses vides</span><span class="sxs-lookup"><span data-stu-id="217ac-1284">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="217ac-1285">Mise à jour de `traffic-manager` pour prendre en charge les fonctionnalités les plus récentes</span><span class="sxs-lookup"><span data-stu-id="217ac-1285">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="217ac-1286">Ressource</span><span class="sxs-lookup"><span data-stu-id="217ac-1286">Resource</span></span>

* <span data-ttu-id="217ac-1287">Ajout de la prise en charge des options `--resource-group/-g` pour le nom du groupe de ressources dans `group`</span><span class="sxs-lookup"><span data-stu-id="217ac-1287">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="217ac-1288">Ajout des commandes à `account lock` pour travailler avec des verrous au niveau de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="217ac-1288">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="217ac-1289">Ajout des commandes à `group lock` pour travailler avec des verrous au niveau du groupe</span><span class="sxs-lookup"><span data-stu-id="217ac-1289">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="217ac-1290">Ajout des commandes à `resource lock` pour travailler avec des verrous au niveau des ressources</span><span class="sxs-lookup"><span data-stu-id="217ac-1290">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="217ac-1291">SQL</span><span class="sxs-lookup"><span data-stu-id="217ac-1291">Sql</span></span>

* <span data-ttu-id="217ac-1292">Ajout de la prise en charge pour le Chiffrement transparent des données (TDE) SQL et le chiffrement transparent des données avec Bring Your Own Key</span><span class="sxs-lookup"><span data-stu-id="217ac-1292">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="217ac-1293">Ajout de la commande `db list-deleted` et du paramètre `db restore --deleted-time`, ce qui offre la possibilité de rechercher et de restaurer les bases de données supprimées</span><span class="sxs-lookup"><span data-stu-id="217ac-1293">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="217ac-1294">Ajout de `db op list` et `db op cancel`, ce qui offre la capacité de répertorier et d’annuler des opérations en cours sur la base de données</span><span class="sxs-lookup"><span data-stu-id="217ac-1294">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="217ac-1295">Stockage</span><span class="sxs-lookup"><span data-stu-id="217ac-1295">Storage</span></span>

* <span data-ttu-id="217ac-1296">Ajout de la prise en charge d’instantané de partage de fichiers</span><span class="sxs-lookup"><span data-stu-id="217ac-1296">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="217ac-1297">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="217ac-1297">Vm</span></span>

* <span data-ttu-id="217ac-1298">Correction d’un bogue dans `vm show` où l’utilisation de `-d` a provoqué un incident dans les adresses IP privées manquantes</span><span class="sxs-lookup"><span data-stu-id="217ac-1298">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="217ac-1299">[VERSION PRÉLIMINAIRE] Ajout de la prise en charge de la mise à niveau propagée pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="217ac-1299">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="217ac-1300">Ajout de la prise en charge de la mise à jour des paramètres de chiffrement avec `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="217ac-1300">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="217ac-1301">Ajout du paramètre `--os-disk-size-gb` pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="217ac-1301">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="217ac-1302">Ajout du paramètre `--license-type` de Windows pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="217ac-1302">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="217ac-1303">22 septembre 2017</span><span class="sxs-lookup"><span data-stu-id="217ac-1303">September 22, 2017</span></span>

<span data-ttu-id="217ac-1304">Version 2.0.18</span><span class="sxs-lookup"><span data-stu-id="217ac-1304">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="217ac-1305">Ressource</span><span class="sxs-lookup"><span data-stu-id="217ac-1305">Resource</span></span>

* <span data-ttu-id="217ac-1306">Ajout de la prise en charge de l’affichage des définitions de stratégie intégrée</span><span class="sxs-lookup"><span data-stu-id="217ac-1306">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="217ac-1307">Ajout de la prise en charge du paramètre de mode pour la création de définitions de stratégie</span><span class="sxs-lookup"><span data-stu-id="217ac-1307">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="217ac-1308">Ajout de la prise en charge des définitions d’interface utilisateur et des modèles pour `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="217ac-1308">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="217ac-1309">[CHANGEMENT CASSANT] Modification du type de ressource `managedapp` de `appliances` en `applications` et de `applianceDefinitions` en `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="217ac-1309">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="217ac-1310">Réseau</span><span class="sxs-lookup"><span data-stu-id="217ac-1310">Network</span></span>

* <span data-ttu-id="217ac-1311">Ajout de la prise en charge de la zone de disponibilité aux sous-commandes `network lb` et `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="217ac-1311">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="217ac-1312">Ajout de la prise en charge de l’homologation Microsoft IPv6 pour `express-route`</span><span class="sxs-lookup"><span data-stu-id="217ac-1312">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="217ac-1313">Ajout des commandes du groupe de sécurité d’application `asg`</span><span class="sxs-lookup"><span data-stu-id="217ac-1313">Added `asg` application security group commands</span></span>
* <span data-ttu-id="217ac-1314">Ajout de l’argument `--application-security-groups` à `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="217ac-1314">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="217ac-1315">Ajout des arguments `--source-asgs` et `--destination-asgs` à `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="217ac-1315">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="217ac-1316">Ajout des arguments `--ddos-protection` et `--vm-protection` à `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="217ac-1316">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="217ac-1317">Ajout des commandes `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="217ac-1317">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="217ac-1318">Stockage</span><span class="sxs-lookup"><span data-stu-id="217ac-1318">Storage</span></span>

* <span data-ttu-id="217ac-1319">Résolution d’un problème qui pouvait causer l’échec des commandes `storage account network-rule` après la mise à jour du Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="217ac-1319">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="217ac-1320">Événement</span><span class="sxs-lookup"><span data-stu-id="217ac-1320">Eventgrid</span></span>

* <span data-ttu-id="217ac-1321">Mise à jour du Kit de développement logiciel (SDK) Python Azure Event Grid afin d’utiliser une version plus récente de l’API « 2017-09-15-preview »</span><span class="sxs-lookup"><span data-stu-id="217ac-1321">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="217ac-1322">SQL</span><span class="sxs-lookup"><span data-stu-id="217ac-1322">SQL</span></span>

* <span data-ttu-id="217ac-1323">La modification de l’`sql server list`argument`--resource-group` devient facultative.</span><span class="sxs-lookup"><span data-stu-id="217ac-1323">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="217ac-1324">En l’absence de précisions, tous les serveurs SQL dans l’abonnement seront retournés</span><span class="sxs-lookup"><span data-stu-id="217ac-1324">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="217ac-1325">Ajout du paramètre `--no-wait` à `db [create|copy|restore|update|replica create|create|update]` et `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="217ac-1325">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="217ac-1326">KeyVault</span><span class="sxs-lookup"><span data-stu-id="217ac-1326">Keyvault</span></span>

* <span data-ttu-id="217ac-1327">Ajout de la prise en charge des commandes Keyvault derrière un proxy</span><span class="sxs-lookup"><span data-stu-id="217ac-1327">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="217ac-1328">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="217ac-1328">VM</span></span>

* <span data-ttu-id="217ac-1329">Ajout de la prise en charge de zone de disponibilité pour `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="217ac-1329">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="217ac-1330">Résolution d’un problème à cause duquel l’utilisation de `--app-gateway ID` avec `vmss create` entraînait un échec</span><span class="sxs-lookup"><span data-stu-id="217ac-1330">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="217ac-1331">Ajout de l’argument `--asgs` à `vm create`</span><span class="sxs-lookup"><span data-stu-id="217ac-1331">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="217ac-1332">Ajout de la prise en charge des commandes en cours d’exécution sur des machines virtuelles avec `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="217ac-1332">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="217ac-1333">[PRÉVERSION] Ajout de la prise en charge du chiffrement de disque VMSS avec `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="217ac-1333">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="217ac-1334">Ajout de la prise en charge de la réalisation de la maintenance sur des machines virtuelles avec `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="217ac-1334">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="217ac-1335">ACS</span><span class="sxs-lookup"><span data-stu-id="217ac-1335">ACS</span></span>

* <span data-ttu-id="217ac-1336">[PRÉVERSION] Ajout de l’argument `--orchestrator-release` à `acs create` pour les régions ACS en préversion</span><span class="sxs-lookup"><span data-stu-id="217ac-1336">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="217ac-1337">AppService</span><span class="sxs-lookup"><span data-stu-id="217ac-1337">Appservice</span></span>

* <span data-ttu-id="217ac-1338">Ajout de la capacité à mettre à jour et à afficher les paramètres d’authentification avec `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="217ac-1338">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="217ac-1339">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="217ac-1339">Backup</span></span>

* <span data-ttu-id="217ac-1340">Version préliminaire</span><span class="sxs-lookup"><span data-stu-id="217ac-1340">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="217ac-1341">11 septembre 2017</span><span class="sxs-lookup"><span data-stu-id="217ac-1341">September 11, 2017</span></span>

<span data-ttu-id="217ac-1342">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="217ac-1342">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="217ac-1343">Principal</span><span class="sxs-lookup"><span data-stu-id="217ac-1343">Core</span></span>

* <span data-ttu-id="217ac-1344">Module de commande activé pour définir son propre ID de corrélation dans la télémétrie</span><span class="sxs-lookup"><span data-stu-id="217ac-1344">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="217ac-1345">Résolution du problème de vidage JSON lorsque la télémétrie est définie en mode diagnostics</span><span class="sxs-lookup"><span data-stu-id="217ac-1345">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="217ac-1346">Acs</span><span class="sxs-lookup"><span data-stu-id="217ac-1346">Acs</span></span>

* <span data-ttu-id="217ac-1347">Ajout de la commande `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="217ac-1347">Added `acs list-locations` command</span></span>
* <span data-ttu-id="217ac-1348">Faire en sorte que `ssh-key-file` soit fourni avec la valeur par défaut attendu</span><span class="sxs-lookup"><span data-stu-id="217ac-1348">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="217ac-1349">AppService</span><span class="sxs-lookup"><span data-stu-id="217ac-1349">Appservice</span></span>

* <span data-ttu-id="217ac-1350">Ajout de la possibilité de créer une application web dans un groupe de ressources autre que celui du plan de service actif</span><span class="sxs-lookup"><span data-stu-id="217ac-1350">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="217ac-1351">CDN</span><span class="sxs-lookup"><span data-stu-id="217ac-1351">CDN</span></span>

* <span data-ttu-id="217ac-1352">Correction du bogue « CustomDomain n’est pas itérable » pour `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="217ac-1352">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="217ac-1353">Extension</span><span class="sxs-lookup"><span data-stu-id="217ac-1353">Extension</span></span>

* <span data-ttu-id="217ac-1354">Version initiale</span><span class="sxs-lookup"><span data-stu-id="217ac-1354">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="217ac-1355">KeyVault</span><span class="sxs-lookup"><span data-stu-id="217ac-1355">Keyvault</span></span>

* <span data-ttu-id="217ac-1356">Résolution du problème où les autorisations étaient sensibles à la casse pour `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="217ac-1356">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="217ac-1357">Réseau</span><span class="sxs-lookup"><span data-stu-id="217ac-1357">Network</span></span>

* <span data-ttu-id="217ac-1358">Renommage de `vnet list-private-access-services` en `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="217ac-1358">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="217ac-1359">Argument `--private-access-services` renommé en `--service-endpoints` pour`vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="217ac-1359">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="217ac-1360">Ajout de la prise en charge de plusieurs plages IP et de ports à `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="217ac-1360">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="217ac-1361">Ajout de la prise en charge de la référence (SKU) pour `lb create`</span><span class="sxs-lookup"><span data-stu-id="217ac-1361">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="217ac-1362">Ajout de la prise en charge de la référence (SKU) pour `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="217ac-1362">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="217ac-1363">Ressource</span><span class="sxs-lookup"><span data-stu-id="217ac-1363">Resource</span></span>

* <span data-ttu-id="217ac-1364">Autoriser le passage dans les définitions de paramètres de stratégie de ressource dans `policy definition create`, et`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="217ac-1364">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="217ac-1365">Autoriser le passage dans les valeurs de paramètres pour `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="217ac-1365">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="217ac-1366">Autoriser le passage de JSON ou d’un fichier pour tous les paramètres</span><span class="sxs-lookup"><span data-stu-id="217ac-1366">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="217ac-1367">Incrémentation de la version de l’API</span><span class="sxs-lookup"><span data-stu-id="217ac-1367">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="217ac-1368">SQL</span><span class="sxs-lookup"><span data-stu-id="217ac-1368">SQL</span></span>

* <span data-ttu-id="217ac-1369">Ajout des commandes `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="217ac-1369">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="217ac-1370">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="217ac-1370">VM</span></span>

* <span data-ttu-id="217ac-1371">Résolu : n’affecte aucun accès tant que `--scope` n’est pas indiqué</span><span class="sxs-lookup"><span data-stu-id="217ac-1371">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="217ac-1372">Résolu : utilisation de la même dénomination d’extension que celle du portail</span><span class="sxs-lookup"><span data-stu-id="217ac-1372">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="217ac-1373">Suppression de `subscription` de la sortie `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="217ac-1373">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="217ac-1374">Résolu : la référence SKU de stockage `[vm|vmss] create` n’est pas appliquée sur les disques de données avec une image</span><span class="sxs-lookup"><span data-stu-id="217ac-1374">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="217ac-1375">Résolu : `vm format-secret --secrets` n’accepte pas d’ID séparés par un saut de ligne</span><span class="sxs-lookup"><span data-stu-id="217ac-1375">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="217ac-1376">31 août 2017</span><span class="sxs-lookup"><span data-stu-id="217ac-1376">August 31, 2017</span></span>

<span data-ttu-id="217ac-1377">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="217ac-1377">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="217ac-1378">KeyVault</span><span class="sxs-lookup"><span data-stu-id="217ac-1378">Keyvault</span></span>

* <span data-ttu-id="217ac-1379">Correction d’un bogue à cause duquel vous tentez de résoudre automatiquement l’encodage secret avec `secret download`</span><span class="sxs-lookup"><span data-stu-id="217ac-1379">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="217ac-1380">Sf</span><span class="sxs-lookup"><span data-stu-id="217ac-1380">Sf</span></span>

* <span data-ttu-id="217ac-1381">Déconseiller toutes les commandes en faveur de Service Fabric CLI (sfctl)</span><span class="sxs-lookup"><span data-stu-id="217ac-1381">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="217ac-1382">Stockage</span><span class="sxs-lookup"><span data-stu-id="217ac-1382">Storage</span></span>

* <span data-ttu-id="217ac-1383">Résolution du problème dans lequel la création de comptes de stockage dans les régions ne prenant pas en charge la fonctionnalité NetworkACLs était impossible</span><span class="sxs-lookup"><span data-stu-id="217ac-1383">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="217ac-1384">Déterminer le type de contenu et l’encodage du contenu lors du chargement d’objets blob et de fichiers si aucun type de contenu et d’encodage n’est spécifié.</span><span class="sxs-lookup"><span data-stu-id="217ac-1384">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="217ac-1385">28 août 2017</span><span class="sxs-lookup"><span data-stu-id="217ac-1385">August 28, 2017</span></span>

<span data-ttu-id="217ac-1386">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="217ac-1386">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="217ac-1387">Interface de ligne de commande</span><span class="sxs-lookup"><span data-stu-id="217ac-1387">CLI</span></span>

* <span data-ttu-id="217ac-1388">Ajout d’une remarque juridique pour `--version`</span><span class="sxs-lookup"><span data-stu-id="217ac-1388">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="217ac-1389">ACS</span><span class="sxs-lookup"><span data-stu-id="217ac-1389">ACS</span></span>

* <span data-ttu-id="217ac-1390">Correction des régions d’aperçu</span><span class="sxs-lookup"><span data-stu-id="217ac-1390">Corrected preview regions</span></span>
* <span data-ttu-id="217ac-1391">Mise en forme par défaut `dns_name_prefix` correctement</span><span class="sxs-lookup"><span data-stu-id="217ac-1391">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="217ac-1392">Optimisation de la sortie de commande des services ACS</span><span class="sxs-lookup"><span data-stu-id="217ac-1392">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="217ac-1393">AppService</span><span class="sxs-lookup"><span data-stu-id="217ac-1393">Appservice</span></span>

* <span data-ttu-id="217ac-1394">[CHANGEMENT CASSANT] Fixation des incohérences dans la sortie de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="217ac-1394">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="217ac-1395">Ajout d’un nouvel alias de `-i` pour `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="217ac-1395">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="217ac-1396">Exposé `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="217ac-1396">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="217ac-1397">Exposition de nouveaux arguments à partir de `az webapp delete` pour conserver le plan de service d'application, les métriques ou l’inscription DNS</span><span class="sxs-lookup"><span data-stu-id="217ac-1397">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="217ac-1398">Problème résolu : Détecter les paramètres d’emplacement correctement</span><span class="sxs-lookup"><span data-stu-id="217ac-1398">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="217ac-1399">IoT</span><span class="sxs-lookup"><span data-stu-id="217ac-1399">IoT</span></span>

* <span data-ttu-id="217ac-1400">Résolu #3934 : La création de la stratégie n’efface plus les stratégies existantes</span><span class="sxs-lookup"><span data-stu-id="217ac-1400">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="217ac-1401">Réseau</span><span class="sxs-lookup"><span data-stu-id="217ac-1401">Network</span></span>

* <span data-ttu-id="217ac-1402">[CHANGEMENT CASSANT] Renommage de `vnet list-private-access-services` en `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="217ac-1402">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="217ac-1403">[CHANGEMENT CASSANT] Renommage de l’option `--private-access-services` en `--service-endpoints` pour `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="217ac-1403">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="217ac-1404">Ajout de la prise en charge de plusieurs IP et de plusieurs pages de port pour `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="217ac-1404">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="217ac-1405">Ajout de la prise en charge de la référence (SKU) pour `lb create`</span><span class="sxs-lookup"><span data-stu-id="217ac-1405">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="217ac-1406">Ajout de la prise en charge de la référence (SKU) pour `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="217ac-1406">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="217ac-1407">Profil</span><span class="sxs-lookup"><span data-stu-id="217ac-1407">Profile</span></span>

* <span data-ttu-id="217ac-1408">exposés `--msi` et `--msi-port` pour vous connecter à l’aide d’une identité de machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="217ac-1408">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="217ac-1409">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="217ac-1409">Service Fabric</span></span>

* <span data-ttu-id="217ac-1410">Version préliminaire</span><span class="sxs-lookup"><span data-stu-id="217ac-1410">Preview release</span></span>
* <span data-ttu-id="217ac-1411">Règles d’utilisateur du Registre/de mot de passe simplifiées pour la commande</span><span class="sxs-lookup"><span data-stu-id="217ac-1411">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="217ac-1412">Invite de mot de passe fixe pour l’utilisateur, même après le passage de paramètre</span><span class="sxs-lookup"><span data-stu-id="217ac-1412">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="217ac-1413">Ajout de la prise en charge de vide `registry_cred`</span><span class="sxs-lookup"><span data-stu-id="217ac-1413">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="217ac-1414">Stockage</span><span class="sxs-lookup"><span data-stu-id="217ac-1414">Storage</span></span>

* <span data-ttu-id="217ac-1415">Paramétrage du niveau blob activé</span><span class="sxs-lookup"><span data-stu-id="217ac-1415">Enabled setting blob tier</span></span>
* <span data-ttu-id="217ac-1416">Ajout des arguments `--bypass` et `--default-action` à `storage account [create|update]` pour la prise en charge du tunneling de service</span><span class="sxs-lookup"><span data-stu-id="217ac-1416">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="217ac-1417">Ajout de commandes permettant d’ajouter des règles de réseau virtuel et des règles basées sur IP à `storage account network-rule`</span><span class="sxs-lookup"><span data-stu-id="217ac-1417">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="217ac-1418">Activation du chiffrement du service par la clé gérée du client</span><span class="sxs-lookup"><span data-stu-id="217ac-1418">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="217ac-1419">[CHANGEMENT CASSANT] Renommage de l’option `--encryption` en `--encryption-services` pour la commande `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="217ac-1419">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="217ac-1420">Problème résolu #4220 : `az storage account update encryption` - incompatibilité de syntaxe</span><span class="sxs-lookup"><span data-stu-id="217ac-1420">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="217ac-1421">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="217ac-1421">VM</span></span>

* <span data-ttu-id="217ac-1422">Correction d’un problème qui entraînait l’affichage d’informations supplémentaires erronées pour `vmss get-instance-view` lors de l’utilisation `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="217ac-1422">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="217ac-1423">Ajout de la prise en charge de `--lb-sku` pour `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="217ac-1423">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="217ac-1424">Suppression des noms humains de la liste rouge du nom de l’administrateur pour `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="217ac-1424">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="217ac-1425">Correction d’un problème qui entraînait `[vm|vmss] create` la levée d’une erreur si la commande ne parvenait pas à extraire des informations de plan à partir d’une image</span><span class="sxs-lookup"><span data-stu-id="217ac-1425">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="217ac-1426">Correction d’un incident qui se produisait lors de la création d’un groupe identique VMMD avec un équilibrage de charge (LB) interne</span><span class="sxs-lookup"><span data-stu-id="217ac-1426">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="217ac-1427">Correction d’un problème qui empêchait `--no-wait` le fonctionnement d’un argument avec `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="217ac-1427">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="217ac-1428">15 août 2017</span><span class="sxs-lookup"><span data-stu-id="217ac-1428">August 15, 2017</span></span>

<span data-ttu-id="217ac-1429">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="217ac-1429">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="217ac-1430">ACS</span><span class="sxs-lookup"><span data-stu-id="217ac-1430">ACS</span></span>

* <span data-ttu-id="217ac-1431">Correction du numéro de port sshMaster0 pour kubernetes</span><span class="sxs-lookup"><span data-stu-id="217ac-1431">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="217ac-1432">AppService</span><span class="sxs-lookup"><span data-stu-id="217ac-1432">Appservice</span></span>

* <span data-ttu-id="217ac-1433">Correction d’une exception qui se produisait lors de la création d’une nouvelle application web Linux basée sur git</span><span class="sxs-lookup"><span data-stu-id="217ac-1433">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="217ac-1434">Event Grid</span><span class="sxs-lookup"><span data-stu-id="217ac-1434">Event Grid</span></span>

* <span data-ttu-id="217ac-1435">Ajout de dépendances du kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="217ac-1435">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="217ac-1436">11 août 2017</span><span class="sxs-lookup"><span data-stu-id="217ac-1436">August 11, 2017</span></span>

<span data-ttu-id="217ac-1437">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="217ac-1437">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="217ac-1438">ACS</span><span class="sxs-lookup"><span data-stu-id="217ac-1438">ACS</span></span>

* <span data-ttu-id="217ac-1439">Ajout de nouvelles régions d’aperçu</span><span class="sxs-lookup"><span data-stu-id="217ac-1439">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="217ac-1440">Batch</span><span class="sxs-lookup"><span data-stu-id="217ac-1440">Batch</span></span>

* <span data-ttu-id="217ac-1441">Mise à jour vers Kit de développement logiciel (DSK) de lot 3.1.0 et Kit de développement logiciel (SDK) de gestion de lot 4.1.0</span><span class="sxs-lookup"><span data-stu-id="217ac-1441">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="217ac-1442">Ajout d'une nouvelle commande affichant le nombre de tâches d’un travail</span><span class="sxs-lookup"><span data-stu-id="217ac-1442">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="217ac-1443">Correction du bogue dans le traitement de l’URL de la signature d'accès partagé du fichier de ressources</span><span class="sxs-lookup"><span data-stu-id="217ac-1443">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="217ac-1444">Point de terminaison de compte Batch prend désormais en charge le préfixe « https:// » facultatif</span><span class="sxs-lookup"><span data-stu-id="217ac-1444">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="217ac-1445">Prise en charge de l’ajout des listes de plus de 100 tâches à un travail</span><span class="sxs-lookup"><span data-stu-id="217ac-1445">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="217ac-1446">Ajout de l’enregistrement de débogage pour le chargement du module de commande Extensions</span><span class="sxs-lookup"><span data-stu-id="217ac-1446">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="217ac-1447">Composant</span><span class="sxs-lookup"><span data-stu-id="217ac-1447">Component</span></span>

* <span data-ttu-id="217ac-1448">Ajout d’un avertissement de désapprobation aux commandes « az component »</span><span class="sxs-lookup"><span data-stu-id="217ac-1448">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="217ac-1449">Conteneur</span><span class="sxs-lookup"><span data-stu-id="217ac-1449">Container</span></span>

* <span data-ttu-id="217ac-1450">`create` : correction d’un problème qui empêchait l’autorisation de signe égal à l’intérieur d’une variable d’environnement</span><span class="sxs-lookup"><span data-stu-id="217ac-1450">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="217ac-1451">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="217ac-1451">Data Lake Store</span></span>

* <span data-ttu-id="217ac-1452">Contrôle de progression activé</span><span class="sxs-lookup"><span data-stu-id="217ac-1452">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="217ac-1453">Event Grid</span><span class="sxs-lookup"><span data-stu-id="217ac-1453">Event Grid</span></span>

* <span data-ttu-id="217ac-1454">Version initiale</span><span class="sxs-lookup"><span data-stu-id="217ac-1454">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="217ac-1455">Réseau</span><span class="sxs-lookup"><span data-stu-id="217ac-1455">Network</span></span>

* <span data-ttu-id="217ac-1456">`lb` : correction d’un problème qui empêchait certains noms de ressources enfant d’être résolus correctement lorsqu’ils étaient omis</span><span class="sxs-lookup"><span data-stu-id="217ac-1456">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="217ac-1457">`application-gateway {subresource} delete` : correction d’un problème en raison duquel `--no-wait` n’était pas honorée</span><span class="sxs-lookup"><span data-stu-id="217ac-1457">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="217ac-1458">`application-gateway http-settings update` : correction d’un problème `--connection-draining-timeout` qui empêchait la désactivation de</span><span class="sxs-lookup"><span data-stu-id="217ac-1458">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="217ac-1459">Correction de l’erreur argument du mot-clé inattendu `sa_data_size_kilobyes` avec`az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="217ac-1459">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="217ac-1460">Profil</span><span class="sxs-lookup"><span data-stu-id="217ac-1460">Profile</span></span>

* <span data-ttu-id="217ac-1461">`account list` : ajout de `--refresh` pour synchroniser les derniers abonnements à partir du serveur</span><span class="sxs-lookup"><span data-stu-id="217ac-1461">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="217ac-1462">Stockage</span><span class="sxs-lookup"><span data-stu-id="217ac-1462">Storage</span></span>

* <span data-ttu-id="217ac-1463">Activer le compte de stockage de mise à jour avec l’identité attribuée par le système</span><span class="sxs-lookup"><span data-stu-id="217ac-1463">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="217ac-1464">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="217ac-1464">VM</span></span>

* <span data-ttu-id="217ac-1465">`availability-set` : nombre de domaines d’erreur exposé sur convert</span><span class="sxs-lookup"><span data-stu-id="217ac-1465">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="217ac-1466">Commande `list-skus` exposée</span><span class="sxs-lookup"><span data-stu-id="217ac-1466">Exposed `list-skus` command</span></span>
* <span data-ttu-id="217ac-1467">Prise en charge pour affecter l’identité avec ou sans création d’attributions de rôle</span><span class="sxs-lookup"><span data-stu-id="217ac-1467">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="217ac-1468">Appliquer la référence (SKU) de stockage lors de l’attachement de disques de données</span><span class="sxs-lookup"><span data-stu-id="217ac-1468">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="217ac-1469">Suppression du nom du disque du système d’exploitation par défaut et de la référence (SKU) de stockage lors de l’utilisation des disques gérés</span><span class="sxs-lookup"><span data-stu-id="217ac-1469">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="217ac-1470">28 juillet 2017</span><span class="sxs-lookup"><span data-stu-id="217ac-1470">July 28, 2017</span></span>

<span data-ttu-id="217ac-1471">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="217ac-1471">Version 2.0.12</span></span>

* <span data-ttu-id="217ac-1472">Ajout de commandes de conteneur</span><span class="sxs-lookup"><span data-stu-id="217ac-1472">Added container commands</span></span>
* <span data-ttu-id="217ac-1473">Ajout de modules de facturation et de consommation</span><span class="sxs-lookup"><span data-stu-id="217ac-1473">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="217ac-1474">Principal</span><span class="sxs-lookup"><span data-stu-id="217ac-1474">Core</span></span>

* <span data-ttu-id="217ac-1475">Informations d’authentification du Kit de développement logiciel (SDK) de sortie pour les principaux de service avec des certificats</span><span class="sxs-lookup"><span data-stu-id="217ac-1475">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="217ac-1476">Correction des exceptions de progression de déploiement</span><span class="sxs-lookup"><span data-stu-id="217ac-1476">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="217ac-1477">Utiliser le point de terminaison ARM à partir du cloud actuel pour créer le client de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="217ac-1477">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="217ac-1478">Amélioration de la gestion simultanée de fichiers clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="217ac-1478">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="217ac-1479">Actualiser l’ID de la demande client pour chaque exécution de la commande</span><span class="sxs-lookup"><span data-stu-id="217ac-1479">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="217ac-1480">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel ( SDK) (#3635)</span><span class="sxs-lookup"><span data-stu-id="217ac-1480">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="217ac-1481">Rapports de progression pour les déploiements de modèle (#3510)</span><span class="sxs-lookup"><span data-stu-id="217ac-1481">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="217ac-1482">Ajout de la prise en charge des champs de sortie de la table de prélèvement via la requête jmespath (#3581)</span><span class="sxs-lookup"><span data-stu-id="217ac-1482">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="217ac-1483">Amélioration de la désactivation des arguments d’analyse et de l’historique Ajout avec des mouvements (#3434)</span><span class="sxs-lookup"><span data-stu-id="217ac-1483">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="217ac-1484">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="217ac-1484">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="217ac-1485">Déplacer tous les fichiers d’enregistrement existant vers le dernier dossier</span><span class="sxs-lookup"><span data-stu-id="217ac-1485">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="217ac-1486">Correction de l’idempotence pour VM/VMSS create (#3586)</span><span class="sxs-lookup"><span data-stu-id="217ac-1486">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="217ac-1487">Les chemins d’accès de la commande ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="217ac-1487">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="217ac-1488">Certains paramètres de type booléen ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="217ac-1488">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="217ac-1489">Prise en charge de la connexion à ADFS sur le serveur local de manière identique à Azure Stack</span><span class="sxs-lookup"><span data-stu-id="217ac-1489">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="217ac-1490">Correction des écritures simultanées dans clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="217ac-1490">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="217ac-1491">ACR</span><span class="sxs-lookup"><span data-stu-id="217ac-1491">ACR</span></span>

* <span data-ttu-id="217ac-1492">Ajout de la commande `show-usage` pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="217ac-1492">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="217ac-1493">Prise en charge de la mise à jour de la référence (SKU) pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="217ac-1493">Support SKU update for managed registries</span></span>
* <span data-ttu-id="217ac-1494">Ajout de registres gérés avec la référence (SKU) gérée</span><span class="sxs-lookup"><span data-stu-id="217ac-1494">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="217ac-1495">Ajout de webhooks pour les registres gérés avec le module de commande acr webhook</span><span class="sxs-lookup"><span data-stu-id="217ac-1495">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="217ac-1496">Ajout de l’authentification AAD avec la commande de connexion acr</span><span class="sxs-lookup"><span data-stu-id="217ac-1496">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="217ac-1497">Ajout de la commande de suppression pour les référentiels docker, les manifestes et les balises</span><span class="sxs-lookup"><span data-stu-id="217ac-1497">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="217ac-1498">ACS</span><span class="sxs-lookup"><span data-stu-id="217ac-1498">ACS</span></span>

* <span data-ttu-id="217ac-1499">Prise en charge des API version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="217ac-1499">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="217ac-1500">AppService</span><span class="sxs-lookup"><span data-stu-id="217ac-1500">Appservice</span></span>

* <span data-ttu-id="217ac-1501">Correction d’un bogue à cause duquel l’énumération d’une application Linux ne retournait absolument rien</span><span class="sxs-lookup"><span data-stu-id="217ac-1501">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="217ac-1502">Prise en charge de la récupération de références depuis ACR</span><span class="sxs-lookup"><span data-stu-id="217ac-1502">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="217ac-1503">Supprimer toutes les commandes sous `appservice web`</span><span class="sxs-lookup"><span data-stu-id="217ac-1503">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="217ac-1504">Masquer les mots de passe du registre docker de la commande de sortie (#3656)</span><span class="sxs-lookup"><span data-stu-id="217ac-1504">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="217ac-1505">Vérifier que le navigateur par défaut est utilisé sur macOs sans erreurs (#3623)</span><span class="sxs-lookup"><span data-stu-id="217ac-1505">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="217ac-1506">Améliorer l’aide de `webapp log tail` et `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="217ac-1506">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="217ac-1507">Commandes `traffic-routing` exposées pour configurer le routage statique (#3566)</span><span class="sxs-lookup"><span data-stu-id="217ac-1507">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="217ac-1508">Ajout de correctifs de fiabilité pour la configuration du contrôle de code source (#3245)</span><span class="sxs-lookup"><span data-stu-id="217ac-1508">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="217ac-1509">Suppression d’un argument non pris en charge `--node-version` de `webapp config update` pour les applications Web de Windows.</span><span class="sxs-lookup"><span data-stu-id="217ac-1509">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="217ac-1510">Utilisez à la place `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="217ac-1510">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="217ac-1511">Batch</span><span class="sxs-lookup"><span data-stu-id="217ac-1511">Batch</span></span>

* <span data-ttu-id="217ac-1512">Mise à jour vers kit de développement logiciel (SDK) de lot 3.0.0 avec prise en charge pour les machines virtuelles de faible priorité dans des pools</span><span class="sxs-lookup"><span data-stu-id="217ac-1512">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="217ac-1513">Renommage `pool create` option `--target-dedicated` en `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="217ac-1513">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="217ac-1514">Ajout des options `pool create`, `--target-low-priority-nodes` et `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="217ac-1514">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="217ac-1515">CDN</span><span class="sxs-lookup"><span data-stu-id="217ac-1515">CDN</span></span>

* <span data-ttu-id="217ac-1516">Fourniture d’un meilleur message d’erreur pour `cdn endpoint list` quand le profil spécifié par `--profile-name` n’existe pas</span><span class="sxs-lookup"><span data-stu-id="217ac-1516">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="217ac-1517">Cloud</span><span class="sxs-lookup"><span data-stu-id="217ac-1517">Cloud</span></span>

* <span data-ttu-id="217ac-1518">Modification de la version de l’API du point de terminaison de métadonnées du cloud au format AAAA-MM-JJ</span><span class="sxs-lookup"><span data-stu-id="217ac-1518">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="217ac-1519">Le point de terminaison de la galerie n’est pas nécessaire</span><span class="sxs-lookup"><span data-stu-id="217ac-1519">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="217ac-1520">Prise en charge de l’inscription du cloud, avec le point de terminaison ARM resource manager</span><span class="sxs-lookup"><span data-stu-id="217ac-1520">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="217ac-1521">Ajout d’une option pour `cloud set` permettant de choisir le profil lors de la sélection du cloud actuel</span><span class="sxs-lookup"><span data-stu-id="217ac-1521">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="217ac-1522">Exposé `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="217ac-1522">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="217ac-1523">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="217ac-1523">CosmosDB</span></span>

* <span data-ttu-id="217ac-1524">Correction relative à la permission de la création de collection avec une clé de partition personnalisée</span><span class="sxs-lookup"><span data-stu-id="217ac-1524">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="217ac-1525">Ajout de la prise en charge de la durée de vie par défaut de la collection</span><span class="sxs-lookup"><span data-stu-id="217ac-1525">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="217ac-1526">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="217ac-1526">Data Lake Analytics</span></span>

* <span data-ttu-id="217ac-1527">Ajout de commandes pour la gestion de la stratégie de calcul sous le titre `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="217ac-1527">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="217ac-1528">Ajout de `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="217ac-1528">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="217ac-1529">Ajout de `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="217ac-1529">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="217ac-1530">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="217ac-1530">Data Lake Store</span></span>

* <span data-ttu-id="217ac-1531">Ajout de la prise en charge pour la rotation de coffre de clés gérés par l’utilisateur dans `dls account update`</span><span class="sxs-lookup"><span data-stu-id="217ac-1531">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="217ac-1532">Mise à jour de la version du kit de développement logiciel (SDK) du système de fichiers Data Lake Store sous-jacente, réglant un problème de performance</span><span class="sxs-lookup"><span data-stu-id="217ac-1532">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="217ac-1533">Ajout de la commande `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="217ac-1533">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="217ac-1534">Cette commande tente d’activer un utilisateur de coffre de clés fourni par l’utilisateur pour utiliser le chiffrement des données dans un compte Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="217ac-1534">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="217ac-1535">Interactive</span><span class="sxs-lookup"><span data-stu-id="217ac-1535">Interactive</span></span>

* <span data-ttu-id="217ac-1536">Amélioration du temps de démarrage à l’aide des commandes en cache</span><span class="sxs-lookup"><span data-stu-id="217ac-1536">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="217ac-1537">Couverture de test accrue</span><span class="sxs-lookup"><span data-stu-id="217ac-1537">Increased test coverage</span></span>
* <span data-ttu-id="217ac-1538">Amélioration du mouvement « ? » pour injecter également dans la commande suivante</span><span class="sxs-lookup"><span data-stu-id="217ac-1538">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="217ac-1539">Correction d’erreurs interactives avec le profil 2017-03-09-profil-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="217ac-1539">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="217ac-1540">Autorisé `--version` en tant que paramètre pour le mode interactif (#3645)</span><span class="sxs-lookup"><span data-stu-id="217ac-1540">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="217ac-1541">Empêche le mode interactif de lever des erreurs à partir des listes de saisie semi-automatique de validation (#3570)</span><span class="sxs-lookup"><span data-stu-id="217ac-1541">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="217ac-1542">Rapports de progression pour les déploiements de modèles (#3510)</span><span class="sxs-lookup"><span data-stu-id="217ac-1542">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="217ac-1543">Ajout de l’indicateur `--progress`</span><span class="sxs-lookup"><span data-stu-id="217ac-1543">Added `--progress` flag</span></span>
* <span data-ttu-id="217ac-1544">Suppression `--debug` et `--verbose` des listes de saisie semi-automatique</span><span class="sxs-lookup"><span data-stu-id="217ac-1544">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="217ac-1545">Suppression `interactive` des listes de saisie semi-automatique (#3324)</span><span class="sxs-lookup"><span data-stu-id="217ac-1545">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="217ac-1546">IoT</span><span class="sxs-lookup"><span data-stu-id="217ac-1546">IoT</span></span>

* <span data-ttu-id="217ac-1547">La création de la stratégie n’efface plus les stratégies existantes.</span><span class="sxs-lookup"><span data-stu-id="217ac-1547">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="217ac-1548">(#3934)</span><span class="sxs-lookup"><span data-stu-id="217ac-1548">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="217ac-1549">Coffre de clés</span><span class="sxs-lookup"><span data-stu-id="217ac-1549">Key vault</span></span>

* <span data-ttu-id="217ac-1550">Ajout de commandes pour les fonctionnalités de récupération de coffre de clés :</span><span class="sxs-lookup"><span data-stu-id="217ac-1550">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="217ac-1551">`keyvault`sous-commandes `purge`, `recover`,`keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="217ac-1551">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="217ac-1552">`keyvault secret`sous-commandes `backup`, `restore`, `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="217ac-1552">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="217ac-1553">`keyvault certificate`sous-commandes `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="217ac-1553">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="217ac-1554">`keyvault key`sous-commandes `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="217ac-1554">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="217ac-1555">Ajout de l’intégration du coffre de clés du principal du service (#3133)</span><span class="sxs-lookup"><span data-stu-id="217ac-1555">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="217ac-1556">Mise à jour du plan de données du coffre de clés vers 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="217ac-1556">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="217ac-1557">(#3307)</span><span class="sxs-lookup"><span data-stu-id="217ac-1557">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="217ac-1558">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="217ac-1558">Lab</span></span>

* <span data-ttu-id="217ac-1559">Ajout de la prise en charge de la revendication de toutes les machines virtuelles dans le laboratoire via `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="217ac-1559">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="217ac-1560">Ajout du formateur de sortie de tableau pour `az lab vm list` et `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="217ac-1560">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="217ac-1561">Surveiller</span><span class="sxs-lookup"><span data-stu-id="217ac-1561">Monitor</span></span>

* <span data-ttu-id="217ac-1562">Correctif pour le fichier de modèle avec `monitor autoscale-settings get-parameters-template` commande (#3349)</span><span class="sxs-lookup"><span data-stu-id="217ac-1562">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="217ac-1563">Renommage de `monitor alert-rule-incidents list` en `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="217ac-1563">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="217ac-1564">Renommage de `monitor alert-rule-incidents show` en `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="217ac-1564">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="217ac-1565">Renommage de `monitor metric-defintions list` en `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="217ac-1565">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="217ac-1566">Renommage de `monitor alert-rules` en `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="217ac-1566">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="217ac-1567">Modifié `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="217ac-1567">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="217ac-1568">sous-commandes`condition` et `action` n’acceptent plus JSON</span><span class="sxs-lookup"><span data-stu-id="217ac-1568">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="217ac-1569">Ajout de nombreux paramètres simplifiant le processus de création de règle</span><span class="sxs-lookup"><span data-stu-id="217ac-1569">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="217ac-1570">`location` n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="217ac-1570">`location` no longer required</span></span>
  * <span data-ttu-id="217ac-1571">Ajout d’un nom et de la prise en charge de l’ID de la cible</span><span class="sxs-lookup"><span data-stu-id="217ac-1571">Add name and ID support for target</span></span>
  * <span data-ttu-id="217ac-1572">Suppression de `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="217ac-1572">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="217ac-1573">Le renommage de `is-enabled` en `enabled`n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="217ac-1573">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="217ac-1574">`description` par défaut sont désormais basées sur la condition fournie</span><span class="sxs-lookup"><span data-stu-id="217ac-1574">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="217ac-1575">Ajout d’exemples aidant à clarifier le nouveau format</span><span class="sxs-lookup"><span data-stu-id="217ac-1575">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="217ac-1576">Prise en charge des noms ou des ID pour les commandes `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="217ac-1576">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="217ac-1577">Ajout d’arguments d’usage et d’exemples pour `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="217ac-1577">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="217ac-1578">Réseau</span><span class="sxs-lookup"><span data-stu-id="217ac-1578">Network</span></span>

* <span data-ttu-id="217ac-1579">Ajout de la commande `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="217ac-1579">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="217ac-1580">Ajout de l’argument `--private-access-services` à `vnet subnet create` et `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="217ac-1580">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="217ac-1581">Correction d’un problème `application-gateway redirect-config create` qui causait l’échec de</span><span class="sxs-lookup"><span data-stu-id="217ac-1581">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="217ac-1582">Correction d’un problème `application-gateway redirect-config update` qui `--no-wait` empêchait le fonctionnement de</span><span class="sxs-lookup"><span data-stu-id="217ac-1582">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="217ac-1583">Correction d’un bogue lié à l’utilisation d’un `--servers` argument avec `application-gateway address-pool create` et `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="217ac-1583">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="217ac-1584">Ajout des commandes `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="217ac-1584">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="217ac-1585">Ajout de commandes à `application-gateway ssl-policy` : `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="217ac-1585">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="217ac-1586">Ajout d’arguments à `application-gateway ssl-policy set` : `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="217ac-1586">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="217ac-1587">Ajout d’arguments à `application-gateway http-settings create` et `application-gateway http-settings update` : `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="217ac-1587">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="217ac-1588">Ajout d’arguments à `application-gateway url-path-map create` et `application-gateway url-path-map update`, `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="217ac-1588">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="217ac-1589">Ajout d’un argument `--redirect-config` à `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="217ac-1589">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="217ac-1590">Ajout de la prise en charge de `--no-wait` pour `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="217ac-1590">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="217ac-1591">Ajout d’arguments à `application-gateway probe create` et `application-gateway probe update` : `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="217ac-1591">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="217ac-1592">Ajout d’un argument `--redirect-config` à `application-gateway rule create` et `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="217ac-1592">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="217ac-1593">Ajout de la prise en charge de `--accelerated-networking` pour `nic create` et `nic update`</span><span class="sxs-lookup"><span data-stu-id="217ac-1593">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="217ac-1594">Suppression de l’ `--internal-dns-name-suffix` argument à partir de `nic create`</span><span class="sxs-lookup"><span data-stu-id="217ac-1594">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="217ac-1595">Ajout de la prise en charge de `--dns-servers` pour `nic update` et `nic create` : ajout de la prise en charge pour les serveurs DNS :</span><span class="sxs-lookup"><span data-stu-id="217ac-1595">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="217ac-1596">Correction d’un bogue qui faisait `local-gateway create` ignorer `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="217ac-1596">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="217ac-1597">Ajout de la prise en charge de `--dns-servers` pour `vnet update`</span><span class="sxs-lookup"><span data-stu-id="217ac-1597">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="217ac-1598">Correction d’un bogue lors de la création d’une homologation sans filtrage de l’itinéraire avec `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="217ac-1598">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="217ac-1599">Correction d’un bogue qui empêchait le fonctionnement des arguments `--provider` et `--bandwidth` avec `express-route update`</span><span class="sxs-lookup"><span data-stu-id="217ac-1599">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="217ac-1600">Correction d’un bogue avec `network watcher show-topology` une logique de valeurs par défaut</span><span class="sxs-lookup"><span data-stu-id="217ac-1600">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="217ac-1601">Amélioration de la mise en forme de sortie pour `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="217ac-1601">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="217ac-1602">Utilisation de l’IP frontale par défaut pour `application-gateway http-listener create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="217ac-1602">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="217ac-1603">Utilisation d’un pool d’adresses par défaut, des paramètres HTTP et de l’écouteur HTTP pour `application-gateway rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="217ac-1603">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="217ac-1604">Utilisation de l’IP frontale par défaut et du pool principal `lb rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="217ac-1604">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="217ac-1605">Utilisation de l’IP frontale par défaut pour `lb inbound-nat-rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="217ac-1605">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="217ac-1606">Profil</span><span class="sxs-lookup"><span data-stu-id="217ac-1606">Profile</span></span>

* <span data-ttu-id="217ac-1607">Prise en charge de la connexion à l’intérieur d’une machine virtuelle avec une identité gérée</span><span class="sxs-lookup"><span data-stu-id="217ac-1607">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="217ac-1608">Prise en charge de la sortie pour `account show` au format de fichier d’authentification du Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="217ac-1608">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="217ac-1609">Affichage des avertissements de désapprobation lors de l’utilisation de '--expanded-view'</span><span class="sxs-lookup"><span data-stu-id="217ac-1609">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="217ac-1610">Ajout de la commande `get-access-token` permettant de fournir un jeton AAD brut</span><span class="sxs-lookup"><span data-stu-id="217ac-1610">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="217ac-1611">Prise en charge de la connexion avec un compte d’utilisateur sans abonnements associés</span><span class="sxs-lookup"><span data-stu-id="217ac-1611">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="217ac-1612">SGBDR</span><span class="sxs-lookup"><span data-stu-id="217ac-1612">RDBMS</span></span>

* <span data-ttu-id="217ac-1613">Prise en charge de l’énumération de serveurs à travers un abonnement (#3417)</span><span class="sxs-lookup"><span data-stu-id="217ac-1613">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="217ac-1614">Correction de `%s` non traité car il manque `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="217ac-1614">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="217ac-1615">Correction du mappage de la source du document et ajout de la tâche CI permettant la vérification de (#3361)</span><span class="sxs-lookup"><span data-stu-id="217ac-1615">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="217ac-1616">Correction concernant l’aide relative à MySQL et PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="217ac-1616">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="217ac-1617">Ressource</span><span class="sxs-lookup"><span data-stu-id="217ac-1617">Resource</span></span>

* <span data-ttu-id="217ac-1618">Amélioration des invites pour les paramètres manquants de `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="217ac-1618">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="217ac-1619">Amélioration de l’analyse de `--parameters KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="217ac-1619">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="217ac-1620">Correction des problèmes à cause desquels `group deployment create` les fichiers de paramètres n’étaient plus reconnus à l’aide de la `@<file>` syntaxe</span><span class="sxs-lookup"><span data-stu-id="217ac-1620">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="217ac-1621">Prise en charge de l’ `--ids` argument pour `resource` et `managedapp` les commandes</span><span class="sxs-lookup"><span data-stu-id="217ac-1621">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="217ac-1622">Correction de certains messages d’analyse et d’erreur (#3584)</span><span class="sxs-lookup"><span data-stu-id="217ac-1622">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="217ac-1623">Correction de l’analyse `--resource-type` permettant à la `lock` commande d’accepter `<resource-namespace>` et `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="217ac-1623">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="217ac-1624">Ajout de la vérification de paramètre des modèles de liaison de modèle (#3629)</span><span class="sxs-lookup"><span data-stu-id="217ac-1624">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="217ac-1625">Ajout de la prise en charge de la spécification des paramètres de déploiement à l’aide de la `KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="217ac-1625">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="217ac-1626">Rôle</span><span class="sxs-lookup"><span data-stu-id="217ac-1626">Role</span></span>

* <span data-ttu-id="217ac-1627">Prise en charge de la sortie au format de fichier d’authentification du Kit de développement logiciel (SDK) pour `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="217ac-1627">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="217ac-1628">Nettoyage des attributions de rôles et de l’application AAD liée lors de la suppression d’un principal de service (#3610)</span><span class="sxs-lookup"><span data-stu-id="217ac-1628">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="217ac-1629">Inclusion du format d’heure dans `app create` args `--start-date` et `--end-date` descriptions</span><span class="sxs-lookup"><span data-stu-id="217ac-1629">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="217ac-1630">Affichage des avertissements de désapprobation lors de l’utilisation de `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="217ac-1630">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="217ac-1631">Ajout de l’intégration du coffre de clés pour les commandes `create-for-rbac` et `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="217ac-1631">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="217ac-1632">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="217ac-1632">Service Fabric</span></span>
* <span data-ttu-id="217ac-1633">Correction d’un problème avec les fichiers volumineux dans les applications tronquées sur le chargement (#3666)</span><span class="sxs-lookup"><span data-stu-id="217ac-1633">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="217ac-1634">Ajout de tests pour les commandes Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="217ac-1634">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="217ac-1635">Correction de nombreuses commandes Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="217ac-1635">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="217ac-1636">SQL</span><span class="sxs-lookup"><span data-stu-id="217ac-1636">SQL</span></span>

* <span data-ttu-id="217ac-1637">Suppression du paramètre rompu `sql server create` `--identity`</span><span class="sxs-lookup"><span data-stu-id="217ac-1637">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="217ac-1638">Suppression des valeurs de mot de passe à partir de la sortie de commande `sql server create` et `sql server update`</span><span class="sxs-lookup"><span data-stu-id="217ac-1638">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="217ac-1639">Ajout des commandes `sql db list-editions` et `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="217ac-1639">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="217ac-1640">Stockage</span><span class="sxs-lookup"><span data-stu-id="217ac-1640">Storage</span></span>

* <span data-ttu-id="217ac-1641">Suppression d’une `--marker` option à partir des commandes `storage blob list`, `storage container list`et `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="217ac-1641">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="217ac-1642">Activation de la création d’un compte de stockage https-only</span><span class="sxs-lookup"><span data-stu-id="217ac-1642">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="217ac-1643">Mise à jour des métriques de stockage, de la journalisation et des commandes cors (#3495)</span><span class="sxs-lookup"><span data-stu-id="217ac-1643">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="217ac-1644">Reformulation d’un message d’exception de l’ajout CORS (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="217ac-1644">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="217ac-1645">Conversion du générateur à une liste en mode exécution d’essai de la commande de téléchargement de lot (#3592)</span><span class="sxs-lookup"><span data-stu-id="217ac-1645">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="217ac-1646">Correction du problème d’essai associé au lot de téléchargement du blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="217ac-1646">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="217ac-1647">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="217ac-1647">VM</span></span>

* <span data-ttu-id="217ac-1648">Prise en charge de la configuration du groupe de sécurité réseau</span><span class="sxs-lookup"><span data-stu-id="217ac-1648">Support configuring nsg</span></span>
* <span data-ttu-id="217ac-1649">Correction d’un bogue qui entraînait une configuration incorrecte du serveur DNS</span><span class="sxs-lookup"><span data-stu-id="217ac-1649">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="217ac-1650">Prise en charge des identités de service géré</span><span class="sxs-lookup"><span data-stu-id="217ac-1650">Support managed service identities</span></span>
* <span data-ttu-id="217ac-1651">Correction d’un problème à cause duquel `cmss create` avec un équilibreur de charge existant exigeait `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="217ac-1651">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="217ac-1652">Les disques de données créés avec le numéro d’unité logique `vm image create` commencent à 0</span><span class="sxs-lookup"><span data-stu-id="217ac-1652">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="217ac-1653">10 mai 2017</span><span class="sxs-lookup"><span data-stu-id="217ac-1653">May 10, 2017</span></span>

<span data-ttu-id="217ac-1654">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="217ac-1654">Version 2.0.6</span></span>

* <span data-ttu-id="217ac-1655">documentdb renommé en cosmosdb</span><span class="sxs-lookup"><span data-stu-id="217ac-1655">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="217ac-1656">Ajouter rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="217ac-1656">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="217ac-1657">Inclure les modules Data Lake Analytics et Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="217ac-1657">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="217ac-1658">Inclure le module Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="217ac-1658">Include Cognitive Services module</span></span>
* <span data-ttu-id="217ac-1659">Inclure le module Service Fabric</span><span class="sxs-lookup"><span data-stu-id="217ac-1659">Include Service Fabric module</span></span>
* <span data-ttu-id="217ac-1660">Inclure le module Interactive (az-shell renommé)</span><span class="sxs-lookup"><span data-stu-id="217ac-1660">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="217ac-1661">Ajouter la prise en charge des commandes CDN</span><span class="sxs-lookup"><span data-stu-id="217ac-1661">Add support for CDN commands</span></span>
* <span data-ttu-id="217ac-1662">Supprimer le module Container</span><span class="sxs-lookup"><span data-stu-id="217ac-1662">Remove Container module</span></span>
* <span data-ttu-id="217ac-1663">Ajouter « az -v » comme raccourci pour « az --version » ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="217ac-1663">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="217ac-1664">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="217ac-1664">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="217ac-1665">Principal</span><span class="sxs-lookup"><span data-stu-id="217ac-1665">Core</span></span>

* <span data-ttu-id="217ac-1666">principal : capturer les exceptions provoquées par un fournisseur non enregistré et l’enregistrer automatiquement</span><span class="sxs-lookup"><span data-stu-id="217ac-1666">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="217ac-1667">performance : conserver le cache de jeton adal en mémoire jusqu’à la fin du processus ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="217ac-1667">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="217ac-1668">Corriger les octets retournés par l’empreinte digitale hex -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="217ac-1668">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="217ac-1669">Téléchargement du certificat Key Vault et intégration AAD SP améliorés ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="217ac-1669">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="217ac-1670">Ajouter l’emplacement de Python à « az —version » ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="217ac-1670">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="217ac-1671">connexion : prise en charge de la connexion lorsqu’il n’y a aucun abonnement ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="217ac-1671">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="217ac-1672">principal : corriger une erreur lors de la connexion à l’aide d’un principal de service deux fois ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="217ac-1672">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="217ac-1673">principal : autoriser la configuration du chemin d’accès de accessTokens.json via une variable d’environnement ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="217ac-1673">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="217ac-1674">principal : autoriser l’application des valeurs par défaut configurées sur les arguments facultatifs ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="217ac-1674">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="217ac-1675">principal : performances améliorées</span><span class="sxs-lookup"><span data-stu-id="217ac-1675">core: Improved performance</span></span>
* <span data-ttu-id="217ac-1676">principal : certificats d’autorité de certification personnalisés - prise en charge de la définition de la variable d’environnement REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="217ac-1676">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="217ac-1677">principal : configuration du cloud - utiliser le point de terminaison « resource manager » si le point de terminaison « management » n’est pas défini</span><span class="sxs-lookup"><span data-stu-id="217ac-1677">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="217ac-1678">ACS</span><span class="sxs-lookup"><span data-stu-id="217ac-1678">ACS</span></span>

* <span data-ttu-id="217ac-1679">corriger le nombre de maîtres et d’agents sur un nombre entier au lieu d’une chaîne</span><span class="sxs-lookup"><span data-stu-id="217ac-1679">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="217ac-1680">exposer « az acs create --no-wait » et « az acs wait » pour la création asynchrone</span><span class="sxs-lookup"><span data-stu-id="217ac-1680">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="217ac-1681">exposer « az acs create --validate » pour les validations de test</span><span class="sxs-lookup"><span data-stu-id="217ac-1681">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="217ac-1682">supprimer le profil Windows avant l’appel PUT pour la commande de mise à l’échelle ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="217ac-1682">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="217ac-1683">AppService</span><span class="sxs-lookup"><span data-stu-id="217ac-1683">AppService</span></span>

* <span data-ttu-id="217ac-1684">functionapp : ajouter la prise en charge complète de functionapp, notamment créer, afficher, liste, supprimer, nom d’hôte, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="217ac-1684">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="217ac-1685">Ajout de Team Services (vsts) comme option de livraison continue à « config contrôle source web appservice »</span><span class="sxs-lookup"><span data-stu-id="217ac-1685">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="217ac-1686">Créer « az webapp » pour remplacer « az appservice web » (pour la rétrocompatibilité, « az appservice web » sera conservé dans les 2 prochaines versions)</span><span class="sxs-lookup"><span data-stu-id="217ac-1686">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="217ac-1687">Exposer des arguments pour configurer le déploiement et des « piles d’exécution » sur webapp create</span><span class="sxs-lookup"><span data-stu-id="217ac-1687">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="217ac-1688">Exposer « webapp list-runtimes »</span><span class="sxs-lookup"><span data-stu-id="217ac-1688">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="217ac-1689">prendre en charge la configuration des chaînes de connexion ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="217ac-1689">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="217ac-1690">prendre en charge le basculement d’emplacement avec aperçu</span><span class="sxs-lookup"><span data-stu-id="217ac-1690">support slot swap with preview</span></span>
* <span data-ttu-id="217ac-1691">Supprimer les erreurs des commandes appservice ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="217ac-1691">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="217ac-1692">Utiliser le groupe de ressources du plan app service pour les opérations de certificat ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="217ac-1692">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="217ac-1693">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="217ac-1693">CosmosDB</span></span>

* <span data-ttu-id="217ac-1694">Renommer le module documentdb en cosmosdb</span><span class="sxs-lookup"><span data-stu-id="217ac-1694">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="217ac-1695">Prise en charge ajoutée pour les API de plan de données documentdb : gestion de base de données et de collecte</span><span class="sxs-lookup"><span data-stu-id="217ac-1695">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="217ac-1696">Prise en charge ajoutée pour activer le basculement automatique sur les comptes de base de données</span><span class="sxs-lookup"><span data-stu-id="217ac-1696">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="217ac-1697">Prise en charge ajoutée pour la nouvelle stratégie de cohérence ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="217ac-1697">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="217ac-1698">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="217ac-1698">Data Lake Analytics</span></span>

* <span data-ttu-id="217ac-1699">Corriger un bogue dans lequel le filtrage sur le résultat et l’état des listes de travaux lève une erreur</span><span class="sxs-lookup"><span data-stu-id="217ac-1699">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="217ac-1700">Ajouter la prise en charge d’un nouveau type d’élément de catalogue : paquet.</span><span class="sxs-lookup"><span data-stu-id="217ac-1700">Add support for new catalog item type: package.</span></span> <span data-ttu-id="217ac-1701">accessible via : `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="217ac-1701">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="217ac-1702">A rendu possible le fait de répertorier les éléments de catalogue suivants à partir d’une base de données (aucune spécification de schéma requise) :</span><span class="sxs-lookup"><span data-stu-id="217ac-1702">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="217ac-1703">Table</span><span class="sxs-lookup"><span data-stu-id="217ac-1703">Table</span></span>
  * <span data-ttu-id="217ac-1704">Fonction table</span><span class="sxs-lookup"><span data-stu-id="217ac-1704">Table valued function</span></span>
  * <span data-ttu-id="217ac-1705">Affichage</span><span class="sxs-lookup"><span data-stu-id="217ac-1705">View</span></span>
  * <span data-ttu-id="217ac-1706">Statistiques de table.</span><span class="sxs-lookup"><span data-stu-id="217ac-1706">Table Statistics.</span></span> <span data-ttu-id="217ac-1707">Cela peut également être répertorié avec un schéma, mais sans spécifier un nom de table</span><span class="sxs-lookup"><span data-stu-id="217ac-1707">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="217ac-1708">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="217ac-1708">Data Lake Store</span></span>

* <span data-ttu-id="217ac-1709">Mettre à jour la version du Kit de développement logiciel (SDK) du système de fichiers sous-jacent, qui offre une meilleure prise en charge pour gérer les scénarios de limitation côté serveur</span><span class="sxs-lookup"><span data-stu-id="217ac-1709">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="217ac-1710">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="217ac-1710">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="217ac-1711">aide manquante pour afficher l’accès.</span><span class="sxs-lookup"><span data-stu-id="217ac-1711">missed help for access show.</span></span> <span data-ttu-id="217ac-1712">ajout en cours.</span><span class="sxs-lookup"><span data-stu-id="217ac-1712">adding it.</span></span> <span data-ttu-id="217ac-1713">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="217ac-1713">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="217ac-1714">Rechercher</span><span class="sxs-lookup"><span data-stu-id="217ac-1714">Find</span></span>

* <span data-ttu-id="217ac-1715">résultats de la recherche améliorés et autorisation du contrôle de version de l’index de recherche</span><span class="sxs-lookup"><span data-stu-id="217ac-1715">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="217ac-1716">KeyVault</span><span class="sxs-lookup"><span data-stu-id="217ac-1716">KeyVault</span></span>

* <span data-ttu-id="217ac-1717">BC : `az keyvault certificate download` remplacer -e dans chaîne ou élément binaire par PEM ou DER afin de mieux représenter les options</span><span class="sxs-lookup"><span data-stu-id="217ac-1717">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="217ac-1718">BC : Supprimer --expires et --not-before dans `keyvault certificate create` car ces paramètres ne sont pas pris en charge par le service</span><span class="sxs-lookup"><span data-stu-id="217ac-1718">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="217ac-1719">Ajoute le paramètre --validity à `keyvault certificate create` pour substituer de manière sélective la valeur dans --policy</span><span class="sxs-lookup"><span data-stu-id="217ac-1719">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="217ac-1720">Résout le problème dans `keyvault certificate get-default-policy` où « expires » et « not_before » étaient exposés mais « validity_in_months » ne l’était pas</span><span class="sxs-lookup"><span data-stu-id="217ac-1720">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="217ac-1721">correction de keyvault pour l’importation de pem et pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="217ac-1721">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="217ac-1722">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="217ac-1722">Lab</span></span>

* <span data-ttu-id="217ac-1723">Ajout des commandes créer, afficher, supprimer et liste pour l’environnement dans le laboratoire</span><span class="sxs-lookup"><span data-stu-id="217ac-1723">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="217ac-1724">Ajout des commandes afficher et liste pour afficher les modèles ARM dans le laboratoire</span><span class="sxs-lookup"><span data-stu-id="217ac-1724">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="217ac-1725">Ajout de l’indicateur --environment dans `az lab vm list` pour filtrer les machines virtuelles selon l’environnement du laboratoire</span><span class="sxs-lookup"><span data-stu-id="217ac-1725">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="217ac-1726">Ajout de la commande pratique `az lab formula export-artifacts` pour exporter une structure d’artefact dans une formule de laboratoire</span><span class="sxs-lookup"><span data-stu-id="217ac-1726">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="217ac-1727">Ajout de commandes pour gérer les secrets dans un laboratoire</span><span class="sxs-lookup"><span data-stu-id="217ac-1727">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="217ac-1728">Surveiller</span><span class="sxs-lookup"><span data-stu-id="217ac-1728">Monitor</span></span>

* <span data-ttu-id="217ac-1729">Correction de bogue : modélisation `--actions` de `az alert-rules create` pour consommer la chaîne JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="217ac-1729">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="217ac-1730">Correction de bogue : la création de paramètres de diagnostic n’accepte pas les métriques/journaux à partir des commandes d’affichage ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="217ac-1730">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="217ac-1731">Réseau</span><span class="sxs-lookup"><span data-stu-id="217ac-1731">Network</span></span>

* <span data-ttu-id="217ac-1732">Ajouter la commande `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="217ac-1732">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="217ac-1733">Ajouter la prise en charge du paramètre `--filters` pour `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="217ac-1733">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="217ac-1734">Ajouter la prise en charge pour le drainage de connexion Application Gateway</span><span class="sxs-lookup"><span data-stu-id="217ac-1734">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="217ac-1735">Ajouter la prise en charge pour la configuration du jeu de règles WAF d’Application Gateway</span><span class="sxs-lookup"><span data-stu-id="217ac-1735">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="217ac-1736">Ajouter la prise en charge des règles et des filtres de routage ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="217ac-1736">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="217ac-1737">Ajouter la prise en charge pour le routage géographique TrafficManager</span><span class="sxs-lookup"><span data-stu-id="217ac-1737">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="217ac-1738">Ajouter la prise en charge des sélecteurs de trafic basés sur la stratégie de connexion VPN</span><span class="sxs-lookup"><span data-stu-id="217ac-1738">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="217ac-1739">Ajouter la prise en charge pour les stratégies IPSec de la connexion VPN</span><span class="sxs-lookup"><span data-stu-id="217ac-1739">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="217ac-1740">Corriger le bogue avec `vpn-connection create` lors de l’utilisation des paramètres `--no-wait` ou `--validate`</span><span class="sxs-lookup"><span data-stu-id="217ac-1740">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="217ac-1741">Ajouter la prise en charge des passerelles de réseau virtuel actif-actif</span><span class="sxs-lookup"><span data-stu-id="217ac-1741">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="217ac-1742">Supprimer les valeurs NULL de la sortie des commandes `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="217ac-1742">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="217ac-1743">BC : résoudre un bogue dans la sortie de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="217ac-1743">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="217ac-1744">Corriger le bogue où l’argument « --key-length » de « vpn-connection create » n’était pas analysé correctement</span><span class="sxs-lookup"><span data-stu-id="217ac-1744">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="217ac-1745">Corriger le bogue dans `dns zone import` où les enregistrements n’étaient pas été importés correctement</span><span class="sxs-lookup"><span data-stu-id="217ac-1745">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="217ac-1746">Corriger le bogue où `traffic-manager endpoint update` ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="217ac-1746">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="217ac-1747">Ajouter des commandes d’aperçu « network watcher »</span><span class="sxs-lookup"><span data-stu-id="217ac-1747">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="217ac-1748">Profil</span><span class="sxs-lookup"><span data-stu-id="217ac-1748">Profile</span></span>

* <span data-ttu-id="217ac-1749">Prendre en charge la connexion lorsqu’il n’y a aucun abonnement trouvé ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="217ac-1749">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="217ac-1750">Prendre en charge un nom de paramètre court dans le jeu de comptes az --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="217ac-1750">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="217ac-1751">Redis</span><span class="sxs-lookup"><span data-stu-id="217ac-1751">Redis</span></span>

* <span data-ttu-id="217ac-1752">Ajout d’une commande de mise à jour qui ajoute également la possibilité de mettre à l’échelle pour le cache redis</span><span class="sxs-lookup"><span data-stu-id="217ac-1752">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="217ac-1753">Commande « update-settings » déconseillée</span><span class="sxs-lookup"><span data-stu-id="217ac-1753">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="217ac-1754">Ressource</span><span class="sxs-lookup"><span data-stu-id="217ac-1754">Resource</span></span>

* <span data-ttu-id="217ac-1755">Ajouter managedapp et les commandes de définition managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="217ac-1755">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="217ac-1756">Prendre en charge les commandes « provider operation » ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="217ac-1756">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="217ac-1757">Prendre en charge la création de ressource générique ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="217ac-1757">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="217ac-1758">Corriger l’analyse de ressource et la recherche de version d’API.</span><span class="sxs-lookup"><span data-stu-id="217ac-1758">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="217ac-1759">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="217ac-1759">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="217ac-1760">Ajouter des documents pour mise à jour du verrou az.</span><span class="sxs-lookup"><span data-stu-id="217ac-1760">Add docs for az lock update.</span></span> <span data-ttu-id="217ac-1761">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="217ac-1761">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="217ac-1762">Sortie d’erreur si vous essayez de lister des ressources pour un groupe qui n’existe pas.</span><span class="sxs-lookup"><span data-stu-id="217ac-1762">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="217ac-1763">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="217ac-1763">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="217ac-1764">[Compute] Résoudre les problèmes de mise à jour de VMSS et du groupe à haute disponibilité de machines virtuelles.</span><span class="sxs-lookup"><span data-stu-id="217ac-1764">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="217ac-1765">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="217ac-1765">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="217ac-1766">Corriger le verrouillage des commandes créer et supprimer si parent-resource-path est None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="217ac-1766">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="217ac-1767">Rôle</span><span class="sxs-lookup"><span data-stu-id="217ac-1767">Role</span></span>

* <span data-ttu-id="217ac-1768">create-for-rbac : vérifier que la date de fin du SP ne dépassera pas la date d’expiration du certificat ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="217ac-1768">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="217ac-1769">RBAC : ajouter la prise en charge complète de « ad group » ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="217ac-1769">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="217ac-1770">rôle : résoudre les problèmes de mise à jour de définition de rôle ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="217ac-1770">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="217ac-1771">create-for-rbac : vérifier que le mot de passe fourni par l’utilisateur est accepté</span><span class="sxs-lookup"><span data-stu-id="217ac-1771">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="217ac-1772">SQL</span><span class="sxs-lookup"><span data-stu-id="217ac-1772">SQL</span></span>

* <span data-ttu-id="217ac-1773">Ajout des commandes az sql server list-usages et az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="217ac-1773">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="217ac-1774">SQL : possibilité de se connecter directement au fournisseur de ressources ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="217ac-1774">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="217ac-1775">Stockage</span><span class="sxs-lookup"><span data-stu-id="217ac-1775">Storage</span></span>

* <span data-ttu-id="217ac-1776">Définir l’emplacement par défaut sur l’emplacement du groupe de ressources pour `storage account create`</span><span class="sxs-lookup"><span data-stu-id="217ac-1776">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="217ac-1777">Ajouter la prise en charge de la copie incrémentielle d’objet blob</span><span class="sxs-lookup"><span data-stu-id="217ac-1777">Add support for incremental blob copy</span></span>
* <span data-ttu-id="217ac-1778">Ajouter la prise en charge du chargement d’objet blob de blocs volumineux</span><span class="sxs-lookup"><span data-stu-id="217ac-1778">Add support for large block blob upload</span></span>
* <span data-ttu-id="217ac-1779">Modifier la taille de bloc à 100 Mo lorsque le fichier à charger est supérieur à 200 Go</span><span class="sxs-lookup"><span data-stu-id="217ac-1779">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="217ac-1780">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="217ac-1780">VM</span></span>

* <span data-ttu-id="217ac-1781">avail-set : rendre le compte de domaine UD&FD facultatif</span><span class="sxs-lookup"><span data-stu-id="217ac-1781">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="217ac-1782">remarque : commandes de machine virtuelle dans clouds souverains Veuillez éviter les fonctionnalités liées au disque managé, notamment :</span><span class="sxs-lookup"><span data-stu-id="217ac-1782">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="217ac-1783">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="217ac-1783">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="217ac-1784">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="217ac-1784">az vm/vmss disk</span></span>
  3. <span data-ttu-id="217ac-1785">Dans « az vm/vmss create », utiliser « —use-unmanaged-disk » pour éviter le disque managé Les autres commandes devraient fonctionner</span><span class="sxs-lookup"><span data-stu-id="217ac-1785">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="217ac-1786">vm/vmss : améliorer le texte d’avertissement lors de la génération de paires de clés ssh</span><span class="sxs-lookup"><span data-stu-id="217ac-1786">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="217ac-1787">vm/vmss : prendre en charge la création à partir d’une image de la Place de marché qui requiert des informations sur le plan ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="217ac-1787">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="217ac-1788">3 avril 2017</span><span class="sxs-lookup"><span data-stu-id="217ac-1788">April 3, 2017</span></span>

<span data-ttu-id="217ac-1789">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="217ac-1789">Version 2.0.2</span></span>

<span data-ttu-id="217ac-1790">Nous avons publié les composants ACR, Batch, KeyVault et SQL dans cette version</span><span class="sxs-lookup"><span data-stu-id="217ac-1790">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="217ac-1791">Principal</span><span class="sxs-lookup"><span data-stu-id="217ac-1791">Core</span></span>

* <span data-ttu-id="217ac-1792">Ajout des modules acr, lab, monitor et find à la liste par défaut</span><span class="sxs-lookup"><span data-stu-id="217ac-1792">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="217ac-1793">Connexion : ignorer les locataires erronés ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="217ac-1793">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="217ac-1794">login : définition de l’abonnement par défaut à la valeur « un » avec l’état « Activé » ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="217ac-1794">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="217ac-1795">Ajout de la prise en charge des commandes wait et de --no-wait à davantage de commandes ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="217ac-1795">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="217ac-1796">core : prise en charge de la connexion à l’aide du principal du service avec un certificat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="217ac-1796">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="217ac-1797">Ajout d’une invite pour les paramètres de modèle manquants.</span><span class="sxs-lookup"><span data-stu-id="217ac-1797">Add prompting for missing template parameters.</span></span> <span data-ttu-id="217ac-1798">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="217ac-1798">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="217ac-1799">Prise en charge de la définition de valeurs par défaut pour des arguments courants tels que le groupe de ressources par défaut, le site web par défaut et la machine virtuelle par défaut</span><span class="sxs-lookup"><span data-stu-id="217ac-1799">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="217ac-1800">Prise en charge de la connexion à un locataire spécifique</span><span class="sxs-lookup"><span data-stu-id="217ac-1800">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="217ac-1801">ACS</span><span class="sxs-lookup"><span data-stu-id="217ac-1801">ACS</span></span>

* <span data-ttu-id="217ac-1802">[ACS] Ajout de la prise en charge de la configuration d’un cluster ACS par défaut ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="217ac-1802">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="217ac-1803">Ajout de la prise en charge de l’invite de mot de passe de clé ssh.</span><span class="sxs-lookup"><span data-stu-id="217ac-1803">Add support for ssh key password prompting.</span></span> <span data-ttu-id="217ac-1804">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="217ac-1804">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="217ac-1805">Ajout de la prise en charge des clusters Windows.</span><span class="sxs-lookup"><span data-stu-id="217ac-1805">Add support for windows clusters.</span></span> <span data-ttu-id="217ac-1806">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="217ac-1806">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="217ac-1807">Basculement du rôle Propriétaire au rôle Contributeur.</span><span class="sxs-lookup"><span data-stu-id="217ac-1807">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="217ac-1808">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="217ac-1808">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="217ac-1809">AppService</span><span class="sxs-lookup"><span data-stu-id="217ac-1809">AppService</span></span>

* <span data-ttu-id="217ac-1810">appservice : prise en charge de l’obtention de l’adresse IP externe utilisée pour les enregistrements A DNS ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="217ac-1810">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="217ac-1811">appservice : prise en charge de la liaison des certificats avec caractères génériques ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="217ac-1811">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="217ac-1812">appservice : prise en charge des profils de publication de liste ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="217ac-1812">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="217ac-1813">AppService : déclenchement de la synchronisation de contrôle de code source après la configuration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="217ac-1813">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="217ac-1814">DataLake</span><span class="sxs-lookup"><span data-stu-id="217ac-1814">DataLake</span></span>

* <span data-ttu-id="217ac-1815">Version initiale du module Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="217ac-1815">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="217ac-1816">Version initiale du module Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="217ac-1816">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="217ac-1817">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="217ac-1817">DocuemntDB</span></span>

* <span data-ttu-id="217ac-1818">DocumentDB : ajout de la prise en charge de l’énumération des chaînes de connexion ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="217ac-1818">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="217ac-1819">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="217ac-1819">VM</span></span>

* <span data-ttu-id="217ac-1820">[Compute] Ajout de la prise en charge d’AppGateway à la création de groupe de machines virtuelles identiques ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="217ac-1820">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="217ac-1821">[VM/VMSS] Amélioration de la prise en charge de la mise en cache de disque ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="217ac-1821">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="217ac-1822">VM/VMSS : intégration de la logique de validation des informations d’identification utilisée par le portail ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="217ac-1822">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="217ac-1823">Ajout de la prise en charge des commandes wait et de --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="217ac-1823">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="217ac-1824">Groupe de machines virtuelles identiques : prise en charge de \* pour énumérer les vues d’instance parmi les machines virtuelles ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="217ac-1824">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="217ac-1825">Ajout --secrets pour machine virtuelle et groupe de machines virtuelles identiques ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="217ac-1825">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="217ac-1826">Autorisation de la création de machines virtuelles avec un disque dur virtuel spécialisé ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="217ac-1826">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="217ac-1827">27 février 2017</span><span class="sxs-lookup"><span data-stu-id="217ac-1827">February 27, 2017</span></span>

<span data-ttu-id="217ac-1828">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="217ac-1828">Version 2.0.0</span></span>

<span data-ttu-id="217ac-1829">Cette version d’Azure CLI 2.0 est la première instance mise à la disposition générale. La disponibilité générale s’applique à ces modules de commande :</span><span class="sxs-lookup"><span data-stu-id="217ac-1829">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="217ac-1830">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="217ac-1830">Container Service (acs)</span></span>
- <span data-ttu-id="217ac-1831">Compute (notamment Resource Manager, machine virtuelle, groupes de machines virtuelles identiques, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="217ac-1831">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="217ac-1832">Réseau</span><span class="sxs-lookup"><span data-stu-id="217ac-1832">Networking</span></span>
- <span data-ttu-id="217ac-1833">Stockage</span><span class="sxs-lookup"><span data-stu-id="217ac-1833">Storage</span></span>

<span data-ttu-id="217ac-1834">Ces modules de commande, pouvant être utilisés en production, sont pris en charge par le contrat de niveau de service (SLA) Microsoft standard. Vous pouvez ouvrir des incidents directement auprès du support technique Microsoft ou dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/). Vous pouvez poser des questions sur [StackOverflow à l’aide du mot-clé azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), ou contacter l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Vous pouvez fournir des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="217ac-1834">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="217ac-1835">Les commandes de ces modules sont stables et il n’est pas prévu que la syntaxe change dans les mises à jour ultérieures de cette version d’Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="217ac-1835">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="217ac-1836">Pour vérifier la version de l’interface CLI, utilisez `az --version`. La sortie indique la version de l’interface CLI proprement dite (2.0.0 dans cette version), les différents modules de commande et les versions de Python et de GCC que vous utilisez.</span><span class="sxs-lookup"><span data-stu-id="217ac-1836">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="217ac-1837">Certains de ces modules de commande présentent un suffixe « b*n* » ou « rc*n* ». Ces modules de commande, encore en préversion, seront mis à la disposition générale à l’avenir.</span><span class="sxs-lookup"><span data-stu-id="217ac-1837">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="217ac-1838">Nous avons également des versions d’évaluation nocturnes de l’interface CLI. Pour plus d’informations, consultez ces instructions sur l’[obtention des builds nocturnes](https://github.com/Azure/azure-cli#nightly-builds), ainsi que ces instructions sur [la contribution au code et la configuration d’un environnement de développement](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="217ac-1838">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="217ac-1839">Vous pouvez signaler des problèmes liés aux versions d’évaluation nocturnes comme suit :</span><span class="sxs-lookup"><span data-stu-id="217ac-1839">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="217ac-1840">Signalez des problèmes dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="217ac-1840">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="217ac-1841">Contactez l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="217ac-1841">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="217ac-1842">Fournissez des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="217ac-1842">Provide feedback from the command line with the `az feedback` command</span></span>

