---
title: Notes de publication d’Azure CLI
description: En savoir plus sur les dernières mises à jour d’Azure CLI
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 11/26/2019
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 75a3a3ee800edc20bd1c8ed7ab1ff542f5935c6c
ms.sourcegitcommit: 443e14098d6643cdb2e178847d1c79b1b95146ce
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/26/2019
ms.locfileid: "74543462"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="655ae-103">Notes de publication d’Azure CLI</span><span class="sxs-lookup"><span data-stu-id="655ae-103">Azure CLI release notes</span></span>

## <a name="november-26-2019"></a><span data-ttu-id="655ae-104">26 novembre 2019</span><span class="sxs-lookup"><span data-stu-id="655ae-104">November 26, 2019</span></span>

<span data-ttu-id="655ae-105">Version 2.0.77</span><span class="sxs-lookup"><span data-stu-id="655ae-105">Version 2.0.77</span></span>

### <a name="acr"></a><span data-ttu-id="655ae-106">ACR</span><span class="sxs-lookup"><span data-stu-id="655ae-106">ACR</span></span>

* <span data-ttu-id="655ae-107">Dépréciation du paramètre `--branch` dans acr task create/update</span><span class="sxs-lookup"><span data-stu-id="655ae-107">Deprecated paramater `--branch` from acr task create/update</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="655ae-108">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="655ae-108">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="655ae-109">Ajout de l’indicateur `--workspace-resource-id` pour permettre la création d’un cluster Azure Red Hat OpenShift avec supervision</span><span class="sxs-lookup"><span data-stu-id="655ae-109">Added `--workspace-resource-id` flag to allow creation of Azure Red Hat Openshift cluster with monitoring</span></span>
* <span data-ttu-id="655ae-110">Ajout de `monitor_profile` pour créer un cluster Azure Red Hat OpenShift avec supervision</span><span class="sxs-lookup"><span data-stu-id="655ae-110">Added `monitor_profile` to create Azure Red Hat OpenShift cluster with monitoring</span></span>

### <a name="aks"></a><span data-ttu-id="655ae-111">AKS</span><span class="sxs-lookup"><span data-stu-id="655ae-111">AKS</span></span>

* <span data-ttu-id="655ae-112">Ajout de la prise en charge de l’opération de rotation des certificats de cluster à l’aide de la commande « az aks rotate-certs ».</span><span class="sxs-lookup"><span data-stu-id="655ae-112">Added support cluster certificate rotation operation using "az aks rotate-certs".</span></span>

### <a name="appconfig"></a><span data-ttu-id="655ae-113">AppConfig</span><span class="sxs-lookup"><span data-stu-id="655ae-113">AppConfig</span></span>

* <span data-ttu-id="655ae-114">Ajout de la prise en charge de l’utilisation de « : » pour le séparateur `as az appconfig kv import`</span><span class="sxs-lookup"><span data-stu-id="655ae-114">Added support for using ":" for `as az appconfig kv import` separator</span></span>
* <span data-ttu-id="655ae-115">Résolution du problème de listage des valeurs de clés avec plusieurs étiquettes, y compris une étiquette Null.</span><span class="sxs-lookup"><span data-stu-id="655ae-115">Fixed issue for listing key values with multiple labels including null label.</span></span> 
* <span data-ttu-id="655ae-116">Mise à jour du SDK du plan de gestion, azure-mgmt-appconfiguration, vers la version 0.3.0.</span><span class="sxs-lookup"><span data-stu-id="655ae-116">Updated management plane sdk, azure-mgmt-appconfiguration, to version 0.3.0.</span></span> 

### <a name="appservice"></a><span data-ttu-id="655ae-117">AppService</span><span class="sxs-lookup"><span data-stu-id="655ae-117">AppService</span></span>

* <span data-ttu-id="655ae-118">Résolution du problème #11100 : Erreur d’attribut pour az webapp up lors de la création du plan de service</span><span class="sxs-lookup"><span data-stu-id="655ae-118">Fixed issue #11100: AttributeError for az webapp up when create service plan</span></span>
* <span data-ttu-id="655ae-119">az webapp up : En forçant la création ou le déploiement sur un site pour les langues prises en charge, aucune valeur par défaut n’est utilisée.</span><span class="sxs-lookup"><span data-stu-id="655ae-119">az webapp up: Forcing the creation or deployment to a site for supported languages, no defaults used.</span></span>
* <span data-ttu-id="655ae-120">Ajout de la prise en charge d’App Service Environment : az appservice ase show | list | list-addresses | list-plans | create | update | delete</span><span class="sxs-lookup"><span data-stu-id="655ae-120">Added support for App Service Environment: az appservice ase show | list | list-addresses | list-plans | create | update | delete</span></span>

### <a name="backup"></a><span data-ttu-id="655ae-121">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="655ae-121">Backup</span></span>

* <span data-ttu-id="655ae-122">Résolution du problème dans az backup policy list-associated-items.</span><span class="sxs-lookup"><span data-stu-id="655ae-122">Fixed issue in az backup policy list-associated-items.</span></span> <span data-ttu-id="655ae-123">Ajout du paramètre BackupManagementType facultatif.</span><span class="sxs-lookup"><span data-stu-id="655ae-123">Added optional BackupManagementType parameter.</span></span>

### <a name="compute"></a><span data-ttu-id="655ae-124">Calcul</span><span class="sxs-lookup"><span data-stu-id="655ae-124">Compute</span></span>

* <span data-ttu-id="655ae-125">Mise à jour de la version de l’API de calcul, des disques et des captures instantanées vers 2019-07-01</span><span class="sxs-lookup"><span data-stu-id="655ae-125">Upgraded API version of compute, disks, snapshots to 2019-07-01</span></span>
* <span data-ttu-id="655ae-126">vmss create : amélioration pour --orchestration-mode</span><span class="sxs-lookup"><span data-stu-id="655ae-126">vmss create: Improvement for --orchestration-mode</span></span>
* <span data-ttu-id="655ae-127">sig image-definition create : ajout de --os-state pour permettre de spécifier si les machines virtuelles créées sous cette image sont « généralisées » ou « spécialisées »</span><span class="sxs-lookup"><span data-stu-id="655ae-127">sig image-definition create: Added --os-state to allow specifying whether the virtual machines created under this image are 'Generalized' or 'Specialized'</span></span>
* <span data-ttu-id="655ae-128">sig image-definition create : ajout de --hyper-v-generation pour permettre la spécification de la génération de l’hyperviseur</span><span class="sxs-lookup"><span data-stu-id="655ae-128">sig image-definition create: Added --hyper-v-generation to allow specifying the hypervisor generation</span></span>
* <span data-ttu-id="655ae-129">sig image-version create : ajout de la prise en charge de --os-snapshot et de --data-snapshots</span><span class="sxs-lookup"><span data-stu-id="655ae-129">sig image-version create: Added support --os-snapshot and --data-snapshots</span></span>
* <span data-ttu-id="655ae-130">image create : ajout de --data-disk-caching pour autoriser la spécification du paramètre de mise en cache des disques de données</span><span class="sxs-lookup"><span data-stu-id="655ae-130">image create: Added --data-disk-caching to allow specifying caching setting of data disks</span></span>
* <span data-ttu-id="655ae-131">Mise à niveau du SDK Python Compute vers la version 10.0.0</span><span class="sxs-lookup"><span data-stu-id="655ae-131">Upgraded Python Compute SDK to 10.0.0</span></span>
* <span data-ttu-id="655ae-132">vm/vmss create : ajout de « Spot » à la propriété d’énumération « Priority »</span><span class="sxs-lookup"><span data-stu-id="655ae-132">vm/vmss create: Added 'Spot' to 'Priority' enum property</span></span>
* <span data-ttu-id="655ae-133">[Changement cassant] le paramètre « --max-billing » a été renommé « --max-price », pour les machines virtuelles et VMSS, à des fins de cohérence avec les applets de commande PowerShell et Swagger</span><span class="sxs-lookup"><span data-stu-id="655ae-133">[Breaking change] Renamed '--max-billing' parameter to '--max-price', for both VM and VMSS, to be consistent with Swagger and Powershell cmdlets</span></span>
* <span data-ttu-id="655ae-134">vm monitor log show : ajout de la prise en charge de l’interrogation du journal via l’espace de travail Log Analytics lié.</span><span class="sxs-lookup"><span data-stu-id="655ae-134">vm monitor log show: Added support for querying log over linked log analytics workspace.</span></span>

### <a name="iot"></a><span data-ttu-id="655ae-135">IOT</span><span class="sxs-lookup"><span data-stu-id="655ae-135">IOT</span></span>

* <span data-ttu-id="655ae-136">Correctif #2531 : ajout d’arguments facilitant la mise à jour des hubs.</span><span class="sxs-lookup"><span data-stu-id="655ae-136">Fix #2531: Added convenience arguments for hub update.</span></span>
* <span data-ttu-id="655ae-137">Correctif #8323 : ajout de paramètres manquants pour créer un point de terminaison personnalisé de stockage.</span><span class="sxs-lookup"><span data-stu-id="655ae-137">Fix #8323: Added missing parameters to create storage custom endpoint.</span></span>
* <span data-ttu-id="655ae-138">Correction d’un bogue de régression : restauration des modifications qui remplacent le point de terminaison de stockage par défaut.</span><span class="sxs-lookup"><span data-stu-id="655ae-138">Fix regression bug: Reverted the changes which overrides the default storage endpoint.</span></span>

### <a name="key-vault"></a><span data-ttu-id="655ae-139">Key Vault</span><span class="sxs-lookup"><span data-stu-id="655ae-139">Key Vault</span></span>

* <span data-ttu-id="655ae-140">Résolution du problème #11121 : lors de l’utilisation de `az keyvault certificate list`, le passage de `--include-pending` n’a plus besoin d’une valeur `true` ou `false`</span><span class="sxs-lookup"><span data-stu-id="655ae-140">Fixed #11121: When using `az keyvault certificate list`, passing `--include-pending` now doesn't require a value of `true` or `false`</span></span>

### <a name="netappfiles"></a><span data-ttu-id="655ae-141">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="655ae-141">NetAppFiles</span></span>

* <span data-ttu-id="655ae-142">Mise à niveau d’azure-mgmt-netapp vers 0.7.0, qui comprend des propriétés de volume supplémentaires associées aux opérations de réplication à venir</span><span class="sxs-lookup"><span data-stu-id="655ae-142">Upgraded azure-mgmt-netapp to 0.7.0 which includes some additional volume properties associated with upcoming replication operations</span></span>

### <a name="network"></a><span data-ttu-id="655ae-143">Réseau</span><span class="sxs-lookup"><span data-stu-id="655ae-143">Network</span></span>

* <span data-ttu-id="655ae-144">application-gateway waf-config : déprécié</span><span class="sxs-lookup"><span data-stu-id="655ae-144">application-gateway waf-config: deprecated</span></span>
* <span data-ttu-id="655ae-145">application-gateway waf-policy : ajout de règles managées par sous-groupes pour gérer des ensembles de règles managées et des règles d’exclusion</span><span class="sxs-lookup"><span data-stu-id="655ae-145">application-gateway waf-policy: Added subgroup managed-rules to manage managed rule sets and exclusion rules</span></span>
* <span data-ttu-id="655ae-146">application-gateway waf-policy : ajout d’un paramètre de stratégie de sous-groupe pour gérer la configuration globale d’une stratégie WAF</span><span class="sxs-lookup"><span data-stu-id="655ae-146">application-gateway waf-policy: Added subgroup policy-setting to manage global configuration of a waf-policy</span></span>
* <span data-ttu-id="655ae-147">[CHANGEMENT CASSANT] application-gateway waf-policy : règle de sous-groupe renommée en custom-rule</span><span class="sxs-lookup"><span data-stu-id="655ae-147">[BREAKING CHANGE] application-gateway waf-policy: Renamed subgroup rule to custom-rule</span></span>
* <span data-ttu-id="655ae-148">application-gateway http-listener : ajout de --firewall-policy lors de la création</span><span class="sxs-lookup"><span data-stu-id="655ae-148">application-gateway http-listener: Added --firewall-policy when create</span></span>
* <span data-ttu-id="655ae-149">application-gateway url-path-map rule : ajout de --firewall-policy lors de la création</span><span class="sxs-lookup"><span data-stu-id="655ae-149">application-gateway url-path-map rule: Added --firewall-policy when create</span></span>

### <a name="packaging"></a><span data-ttu-id="655ae-150">Packaging</span><span class="sxs-lookup"><span data-stu-id="655ae-150">Packaging</span></span>

* <span data-ttu-id="655ae-151">Réécriture du wrapper az dans Python</span><span class="sxs-lookup"><span data-stu-id="655ae-151">Rewrote the az wrapper in Python</span></span>
* <span data-ttu-id="655ae-152">Ajout de la prise en charge de Python 3.8</span><span class="sxs-lookup"><span data-stu-id="655ae-152">Added support for Python 3.8</span></span>
* <span data-ttu-id="655ae-153">Remplacement par Python 3 pour le package RPM</span><span class="sxs-lookup"><span data-stu-id="655ae-153">Changed to Python 3 for RPM package</span></span>

### <a name="profile"></a><span data-ttu-id="655ae-154">Profil</span><span class="sxs-lookup"><span data-stu-id="655ae-154">Profile</span></span>

* <span data-ttu-id="655ae-155">Suppression d’une erreur liée à l’exécution de `az login -u {} -p {}` avec un compte Microsoft</span><span class="sxs-lookup"><span data-stu-id="655ae-155">Polished error when running `az login -u {} -p {}` with Microsoft account</span></span>
* <span data-ttu-id="655ae-156">Suppression de `SSLError` liée à l’exécution de `az login` derrière un proxy avec un certificat racine auto-signé</span><span class="sxs-lookup"><span data-stu-id="655ae-156">Polished `SSLError` when running `az login` behind a proxy with self-signed root certificate</span></span>
* <span data-ttu-id="655ae-157">Résolution du problème #10578 : `az login` se bloque quand plusieurs instances sont lancées en même temps sur Windows ou WSL</span><span class="sxs-lookup"><span data-stu-id="655ae-157">Fixed #10578: `az login` hangs when more than one instances are launched at the same time on Windows or WSL</span></span>
* <span data-ttu-id="655ae-158">Résolution du problème #11059 : `az login --allow-no-subscriptions` échoue s’il existe des abonnements dans le locataire</span><span class="sxs-lookup"><span data-stu-id="655ae-158">Fixed #11059: `az login --allow-no-subscriptions` fails if there are subscriptions in the tenant</span></span>
* <span data-ttu-id="655ae-159">Résolution du problème #11238 : après avoir renommé un abonnement, la connexion avec MSI entraîne l’affichage du même abonnement deux fois</span><span class="sxs-lookup"><span data-stu-id="655ae-159">Fixed #11238: After renaming a subscription, logging in with MSI will result in the same subscription appearing twice</span></span>

### <a name="rbac"></a><span data-ttu-id="655ae-160">RBAC</span><span class="sxs-lookup"><span data-stu-id="655ae-160">RBAC</span></span>

* <span data-ttu-id="655ae-161">Résolution du problème #10996 : suppression de l’erreur liée à `--force-change-password-next-login` dans `az ad user update` quand `--password` n’est pas spécifié</span><span class="sxs-lookup"><span data-stu-id="655ae-161">Fixed #10996: Polish error for `--force-change-password-next-login` in `az ad user update` when `--password` is not specified</span></span>

### <a name="redis"></a><span data-ttu-id="655ae-162">Redis</span><span class="sxs-lookup"><span data-stu-id="655ae-162">Redis</span></span>

* <span data-ttu-id="655ae-163">Résolution de l’erreur #2902 : éviter de définir des configurations de mémoire lors de la mise à jour du cache de référence SKU de base</span><span class="sxs-lookup"><span data-stu-id="655ae-163">Fixed #2902: Avoid setting memory configs while updating Basic SKU cache</span></span>

### <a name="reservations"></a><span data-ttu-id="655ae-164">Réservations</span><span class="sxs-lookup"><span data-stu-id="655ae-164">Reservations</span></span>

* <span data-ttu-id="655ae-165">Mise à niveau du SDK vers 0.6.0</span><span class="sxs-lookup"><span data-stu-id="655ae-165">Upgraded SDK Version to 0.6.0</span></span>
* <span data-ttu-id="655ae-166">Ajout d’informations détaillées sur le plan de facturation après l’appel de Get-Gatalogs</span><span class="sxs-lookup"><span data-stu-id="655ae-166">Added billingplan details info after calling Get-Gatalogs</span></span>
* <span data-ttu-id="655ae-167">Ajout d’une nouvelle commande `az reservations reservation-order calculate` pour calculer le prix d’une réservation</span><span class="sxs-lookup"><span data-stu-id="655ae-167">Added new command `az reservations reservation-order calculate` to calculate the price for a reservation</span></span>
* <span data-ttu-id="655ae-168">Ajout d’une nouvelle commande `az reservations reservation-order purchase` pour acheter une nouvelle réservation</span><span class="sxs-lookup"><span data-stu-id="655ae-168">Added new command `az reservations reservation-order purchase` to purchase a new reservation</span></span>

### <a name="rest"></a><span data-ttu-id="655ae-169">Rest</span><span class="sxs-lookup"><span data-stu-id="655ae-169">Rest</span></span>
* <span data-ttu-id="655ae-170">`az rest` désormais mis à la disposition générale</span><span class="sxs-lookup"><span data-stu-id="655ae-170">Changed `az rest` to GA</span></span>

### <a name="sql"></a><span data-ttu-id="655ae-171">SQL</span><span class="sxs-lookup"><span data-stu-id="655ae-171">SQL</span></span>

* <span data-ttu-id="655ae-172">Mise à jour d’azure-mgmt-sql vers la version 0.15.0.</span><span class="sxs-lookup"><span data-stu-id="655ae-172">Updated azure-mgmt-sql to version 0.15.0.</span></span>

### <a name="storage"></a><span data-ttu-id="655ae-173">Stockage</span><span class="sxs-lookup"><span data-stu-id="655ae-173">Storage</span></span>

* <span data-ttu-id="655ae-174">storage account create : ajout de --enable-hierarchical-namespace pour prendre en charge la sémantique du système de fichiers dans le service BLOB.</span><span class="sxs-lookup"><span data-stu-id="655ae-174">storage account create: Added --enable-hierarchical-namespace to support filesystem semantics in blob service.</span></span>
* <span data-ttu-id="655ae-175">Suppression de l’exception non liée du message d’erreur</span><span class="sxs-lookup"><span data-stu-id="655ae-175">Removed unrelated exception from error message</span></span>
* <span data-ttu-id="655ae-176">Résolution des problèmes liés à un message d’erreur incorrect « Vous ne disposez pas des autorisations nécessaires pour effectuer cette opération. »</span><span class="sxs-lookup"><span data-stu-id="655ae-176">Fixed issues with incorrect error message "You do not have the required permissions needed to perform this operation."</span></span> <span data-ttu-id="655ae-177">en cas de blocage par des règles de réseau ou AuthenticationFailed.</span><span class="sxs-lookup"><span data-stu-id="655ae-177">when blocked by network rules or AuthenticationFailed.</span></span>

## <a name="november-4-2019"></a><span data-ttu-id="655ae-178">4 novembre 2019</span><span class="sxs-lookup"><span data-stu-id="655ae-178">November 4, 2019</span></span>

<span data-ttu-id="655ae-179">Version 2.0.76</span><span class="sxs-lookup"><span data-stu-id="655ae-179">Version 2.0.76</span></span>

### <a name="acr"></a><span data-ttu-id="655ae-180">ACR</span><span class="sxs-lookup"><span data-stu-id="655ae-180">ACR</span></span>

* <span data-ttu-id="655ae-181">Ajout d’un paramètre d’aperçu `--pack-image-tag` à la commande `az acr pack build`.</span><span class="sxs-lookup"><span data-stu-id="655ae-181">Added a preview parameter `--pack-image-tag` to command `az acr pack build`.</span></span>
* <span data-ttu-id="655ae-182">Ajout de la prise en charge de l’activation de l’audit lors de la création d’un registre</span><span class="sxs-lookup"><span data-stu-id="655ae-182">Added support for enabling auditing on creating a registry</span></span>
* <span data-ttu-id="655ae-183">Ajout de la prise en charge du contrôle d’accès en fonction du rôle délimité par le dépôt</span><span class="sxs-lookup"><span data-stu-id="655ae-183">Added support for Repository-scoped RBAC</span></span>

### <a name="aks"></a><span data-ttu-id="655ae-184">AKS</span><span class="sxs-lookup"><span data-stu-id="655ae-184">AKS</span></span>

* <span data-ttu-id="655ae-185">Ajout de `--enable-cluster-autoscaler`, `--min-count` et `--max-count` à la commande `az aks create`, ce qui active l’autoscaler de cluster pour le pool de nœuds.</span><span class="sxs-lookup"><span data-stu-id="655ae-185">Added `--enable-cluster-autoscaler`, `--min-count` and `--max-count` to the `az aks create` command, which enables cluster autoscaler for the node pool.</span></span>
* <span data-ttu-id="655ae-186">Ajout des indicateurs ci-dessus ainsi que de `--update-cluster-autoscaler` et `--disable-cluster-autoscaler` à la commande `az aks update`, ce qui permet d’effectuer des mises à jour de l’autoscaler de cluster.</span><span class="sxs-lookup"><span data-stu-id="655ae-186">Added the above flags as well as `--update-cluster-autoscaler` and `--disable-cluster-autoscaler` to the `az aks update` command, allowing updates to cluster autoscaler.</span></span>

### <a name="appconfig"></a><span data-ttu-id="655ae-187">AppConfig</span><span class="sxs-lookup"><span data-stu-id="655ae-187">AppConfig</span></span>

* <span data-ttu-id="655ae-188">Ajout du groupe de commandes de fonctionnalités appconfig pour gérer les indicateurs de fonctionnalité stockés dans une configuration d’application.</span><span class="sxs-lookup"><span data-stu-id="655ae-188">Added appconfig feature command group to manage feature flags stored in an App Configuration.</span></span>
* <span data-ttu-id="655ae-189">Correction de bogue mineur pour la commande Exporter vers un fichier appconfig kv.</span><span class="sxs-lookup"><span data-stu-id="655ae-189">Fixed minor bug for appconfig kv export to file command.</span></span> <span data-ttu-id="655ae-190">Arrêt de la lecture du contenu du fichier de destination pendant l’exportation.</span><span class="sxs-lookup"><span data-stu-id="655ae-190">Stop reading dest file contents during export.</span></span>

### <a name="appservice"></a><span data-ttu-id="655ae-191">AppService</span><span class="sxs-lookup"><span data-stu-id="655ae-191">AppService</span></span>

* <span data-ttu-id="655ae-192">`az appservice plan create`: Ajout de la prise en charge de la définition de « persitescaling » sur appservice plan create.</span><span class="sxs-lookup"><span data-stu-id="655ae-192">`az appservice plan create`: Added support to set 'persitescaling' on appservice plan create.</span></span>
* <span data-ttu-id="655ae-193">Résolution d’un problème où l’opération de liaison SSL de la configuration webapp supprimait les balises existantes de la ressource</span><span class="sxs-lookup"><span data-stu-id="655ae-193">Fixed an issue where webapp config ssl bind operation was removing existing tags from the resource</span></span>
* <span data-ttu-id="655ae-194">Ajout de l’indicateur `--build-remote` pour `az functionapp deployment source config-zip` afin de prendre en charge l’action de génération distante pendant le déploiement de l’application de fonction.</span><span class="sxs-lookup"><span data-stu-id="655ae-194">Added `--build-remote` flag for `az functionapp deployment source config-zip` to support remote build action during function app deployment.</span></span>
* <span data-ttu-id="655ae-195">Remplacement de la version du nœud par défaut sur les applications de fonction par ~10 pour Windows</span><span class="sxs-lookup"><span data-stu-id="655ae-195">Changed default node version on function apps to ~10 for Windows</span></span>
* <span data-ttu-id="655ae-196">Ajout de la propriété `--runtime-version` à `az functionapp create`</span><span class="sxs-lookup"><span data-stu-id="655ae-196">Added `--runtime-version` property to `az functionapp create`</span></span>

### <a name="arm"></a><span data-ttu-id="655ae-197">ARM</span><span class="sxs-lookup"><span data-stu-id="655ae-197">ARM</span></span>

* <span data-ttu-id="655ae-198">`az deployment/group deployment validate`: Ajout du paramètre `--handle-extended-json-format` pour prendre en charge le format multiligne et les commentaires dans le modèle json lors du déploiement.</span><span class="sxs-lookup"><span data-stu-id="655ae-198">`az deployment/group deployment validate`: Added `--handle-extended-json-format` parameter to support multiline and comments in json template when deployment.</span></span>
* <span data-ttu-id="655ae-199">Passage d’azure-mgmt-resource à 2019-07-01</span><span class="sxs-lookup"><span data-stu-id="655ae-199">Bumped azure-mgmt-resource to 2019-07-01</span></span>

### <a name="backup"></a><span data-ttu-id="655ae-200">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="655ae-200">Backup</span></span>

* <span data-ttu-id="655ae-201">Ajout de la prise en charge de la sauvegarde AzureFiles</span><span class="sxs-lookup"><span data-stu-id="655ae-201">Added AzureFiles backup support</span></span>

### <a name="compute"></a><span data-ttu-id="655ae-202">Calcul</span><span class="sxs-lookup"><span data-stu-id="655ae-202">Compute</span></span>

* <span data-ttu-id="655ae-203">`az vm create`: Ajout d’un avertissement lors de la spécification de la mise en réseau accélérée avec une carte réseau existante.</span><span class="sxs-lookup"><span data-stu-id="655ae-203">`az vm create`: Added warning when specifying accelerated networking and an existing NIC together.</span></span>
* <span data-ttu-id="655ae-204">`az vm create`: Ajout de `--vmss` pour spécifier un groupe identique de machines virtuelles existant auquel la machine virtuelle doit être affectée.</span><span class="sxs-lookup"><span data-stu-id="655ae-204">`az vm create`: Added `--vmss` to specify an existing virtual machine scale set that the virtual machine should be assigned to.</span></span>
* <span data-ttu-id="655ae-205">`az vm/vmss create`: Ajout d’une copie locale du fichier d’alias d’image afin qu’il soit accessible dans un environnement réseau restreint.</span><span class="sxs-lookup"><span data-stu-id="655ae-205">`az vm/vmss create`: Added a local copy of image alias file so that it can be accessed in a restricted network environment.</span></span>
* <span data-ttu-id="655ae-206">`az vmss create`: Ajout de `--orchestration-mode` pour spécifier la façon dont les machines virtuelles sont gérées par le groupe identique.</span><span class="sxs-lookup"><span data-stu-id="655ae-206">`az vmss create`: Added `--orchestration-mode` to specify how virtual machines are managed by the scale set.</span></span>
* <span data-ttu-id="655ae-207">`az vm/vmss update`: Ajout de `--ultra-ssd-enabled` pour autoriser la mise à jour du paramètre SSD Ultra.</span><span class="sxs-lookup"><span data-stu-id="655ae-207">`az vm/vmss update`: Added `--ultra-ssd-enabled` to allow updating ultra SSD setting.</span></span>
* <span data-ttu-id="655ae-208">[CHANGEMENT CASSANT] `az vm extension set` : Correction d’un bogue qui empêchait les utilisateurs de définir une extension sur une machine virtuelle avec `--ids`.</span><span class="sxs-lookup"><span data-stu-id="655ae-208">[BREAKING CHANGE] `az vm extension set`: Fixed bug where users could not set an extension on a VM with `--ids`.</span></span>
* <span data-ttu-id="655ae-209">Ajout de nouvelles commandes `az vm image terms accept/cancel/show` pour gérer les termes de l’image de la Place de marché Azure.</span><span class="sxs-lookup"><span data-stu-id="655ae-209">Added new commands `az vm image terms accept/cancel/show` to manage Azure Marketplace image terms.</span></span>
* <span data-ttu-id="655ae-210">Mise à jour de VMAccessForLinux vers la version 1.5</span><span class="sxs-lookup"><span data-stu-id="655ae-210">Updated VMAccessForLinux to version 1.5</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="655ae-211">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="655ae-211">CosmosDB</span></span>

* <span data-ttu-id="655ae-212">[CHANGEMENT CASSANT] `az sql container create` : Modification de `--partition-key-path` en paramètre obligatoire</span><span class="sxs-lookup"><span data-stu-id="655ae-212">[BREAKING CHANGE] `az sql container create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="655ae-213">[CHANGEMENT CASSANT] `az gremlin graph create` : Modification de `--partition-key-path` en paramètre obligatoire</span><span class="sxs-lookup"><span data-stu-id="655ae-213">[BREAKING CHANGE] `az gremlin graph create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="655ae-214">`az sql container create`: Ajout de `--unique-key-policy` et `--conflict-resolution-policy`</span><span class="sxs-lookup"><span data-stu-id="655ae-214">`az sql container create`: Added `--unique-key-policy` and `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="655ae-215">`az sql container create/update`: Mise à jour du schéma par défaut `--idx`</span><span class="sxs-lookup"><span data-stu-id="655ae-215">`az sql container create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="655ae-216">`gremlin graph create`: Ajout de `--conflict-resolution-policy`</span><span class="sxs-lookup"><span data-stu-id="655ae-216">`gremlin graph create`: Added `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="655ae-217">`gremlin graph create/update`: Mise à jour du schéma par défaut `--idx`</span><span class="sxs-lookup"><span data-stu-id="655ae-217">`gremlin graph create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="655ae-218">Faute de frappe corrigée dans un message d’aide</span><span class="sxs-lookup"><span data-stu-id="655ae-218">Fixed typo in help message</span></span>
* <span data-ttu-id="655ae-219">base de données : ajout d’informations de dépréciation</span><span class="sxs-lookup"><span data-stu-id="655ae-219">database: Added deprecation infomation</span></span>
* <span data-ttu-id="655ae-220">collection : ajout d’informations de dépréciation</span><span class="sxs-lookup"><span data-stu-id="655ae-220">collection: Added deprecation infomation</span></span>

### <a name="iot"></a><span data-ttu-id="655ae-221">IoT</span><span class="sxs-lookup"><span data-stu-id="655ae-221">IoT</span></span>

* <span data-ttu-id="655ae-222">Ajout d’un nouveau type de source de routage : DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="655ae-222">Added new routing source type: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="655ae-223">Correction des fonctionnalités manquantes dans `az iot hub create`</span><span class="sxs-lookup"><span data-stu-id="655ae-223">Fixed missing features in `az iot hub create`</span></span>

### <a name="key-vault"></a><span data-ttu-id="655ae-224">Key Vault</span><span class="sxs-lookup"><span data-stu-id="655ae-224">Key Vault</span></span>

* <span data-ttu-id="655ae-225">Correction d’une erreur inattendue lorsque le fichier de certificat n’existe pas</span><span class="sxs-lookup"><span data-stu-id="655ae-225">Fixed an unexpected error when certificate file does not exist</span></span>
* <span data-ttu-id="655ae-226">Résolution de `az keyvault recover/purge` qui ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="655ae-226">Fixed `az keyvault recover/purge` not working</span></span>

### <a name="netappfiles"></a><span data-ttu-id="655ae-227">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="655ae-227">NetAppFiles</span></span>

* <span data-ttu-id="655ae-228">Mise à niveau d’azure-mgmt-netapp vers 0.6.0 pour utiliser la version d’API 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="655ae-228">Upgraded azure-mgmt-netapp to 0.6.0 to use API version 2019-07-01.</span></span> <span data-ttu-id="655ae-229">Cette nouvelle version d’API comprend les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="655ae-229">This new API version includes:</span></span>

    - <span data-ttu-id="655ae-230">La création de volume `--protocol-types` accepte maintenant « NFSv4.1 » et non « NFSv4 »</span><span class="sxs-lookup"><span data-stu-id="655ae-230">Volume creation `--protocol-types` accepts now "NFSv4.1" not "NFSv4"</span></span>
    - <span data-ttu-id="655ae-231">La propriété de stratégie d’exportation de volume est maintenant nommée « nfsv41 » et non « nfsv4 »</span><span class="sxs-lookup"><span data-stu-id="655ae-231">Volume export policy property now named 'nfsv41' not 'nfsv4'</span></span>
    - <span data-ttu-id="655ae-232">Le volume `--creation-token` est renommé en `--file-path`</span><span class="sxs-lookup"><span data-stu-id="655ae-232">Volume `--creation-token` renamed to `--file-path`</span></span>
    - <span data-ttu-id="655ae-233">La date de création de l’instantané porte maintenant juste le nom « créé »</span><span class="sxs-lookup"><span data-stu-id="655ae-233">Snapshot creation date now named just 'created'</span></span>

### <a name="network"></a><span data-ttu-id="655ae-234">Réseau</span><span class="sxs-lookup"><span data-stu-id="655ae-234">Network</span></span>

* <span data-ttu-id="655ae-235">`az network private-dns link vnet create/update`: Prise en charge de la liaison de réseau virtuel entre locataires.</span><span class="sxs-lookup"><span data-stu-id="655ae-235">`az network private-dns link vnet create/update`: Support cross-tenant virtual network linking.</span></span>
* <span data-ttu-id="655ae-236">[CHANGEMENT CASSANT] `az network vnet subnet list` : Modification de `--resource-group` et `--vnet-name` pour être maintenant nécessaires.</span><span class="sxs-lookup"><span data-stu-id="655ae-236">[BREAKING CHANGE] `az network vnet subnet list`: Changed `--resource-group` and `--vnet-name` to be required now.</span></span>
* <span data-ttu-id="655ae-237">`az network public-ip prefix create`: Ajout de la prise en charge de la spécification de la version d’adresse IP (IPv4, IPv6) lors de la création</span><span class="sxs-lookup"><span data-stu-id="655ae-237">`az network public-ip prefix create`: Added support to specify IP address version (IPv4, IPv6) when creation</span></span>
* <span data-ttu-id="655ae-238">Passage d’azure-mgmt-network à 7.0.0 et d’api-version à 2019-09-01</span><span class="sxs-lookup"><span data-stu-id="655ae-238">Bumped azure-mgmt-network to 7.0.0 and api-version to 2019-09-01</span></span>
* <span data-ttu-id="655ae-239">`az network vrouter`: Ajout de la prise en charge du nouveau routeur virtuel de service et de l’appairage de routeur virtuel</span><span class="sxs-lookup"><span data-stu-id="655ae-239">`az network vrouter`: Added support for new service virtual router and virtual router peering</span></span>
* <span data-ttu-id="655ae-240">`az network express-route gateway connection`: Ajout de la prise en charge de `--internet-security`</span><span class="sxs-lookup"><span data-stu-id="655ae-240">`az network express-route gateway connection`: Added support for `--internet-security`</span></span>

### <a name="profile"></a><span data-ttu-id="655ae-241">Profil</span><span class="sxs-lookup"><span data-stu-id="655ae-241">Profile</span></span>

* <span data-ttu-id="655ae-242">Résolution de `az account get-access-token --resource-type ms-graph` qui ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="655ae-242">Fixed `az account get-access-token --resource-type ms-graph` not working</span></span>
* <span data-ttu-id="655ae-243">Suppression de l’avertissement de `az login`</span><span class="sxs-lookup"><span data-stu-id="655ae-243">Removed warning from `az login`</span></span>

### <a name="rbac"></a><span data-ttu-id="655ae-244">RBAC</span><span class="sxs-lookup"><span data-stu-id="655ae-244">RBAC</span></span>

* <span data-ttu-id="655ae-245">Résolution de `az ad app update --id {} --display-name {}` qui ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="655ae-245">Fixed `az ad app update --id {} --display-name {}` doesn't work</span></span>

### <a name="servicefabric"></a><span data-ttu-id="655ae-246">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="655ae-246">ServiceFabric</span></span>

* <span data-ttu-id="655ae-247">`az sf cluster create`: Résolution d’un problème en modifiant le groupe identique de machines virtuelles de calcul template.json Service Fabric Linux et Windows de disques standard en disques managés</span><span class="sxs-lookup"><span data-stu-id="655ae-247">`az sf cluster create`: Fixed an issue by modifying service fabric linux and windows template.json compute vmss from standard to managed disks</span></span>

### <a name="sql"></a><span data-ttu-id="655ae-248">SQL</span><span class="sxs-lookup"><span data-stu-id="655ae-248">SQL</span></span>

* <span data-ttu-id="655ae-249">Ajout de paramètres `--compute-model`, `--auto-pause-delay` et `--min-capacity` afin de prendre en charge les opérations CRUD pour la nouvelle offre SQL Database : Modèle de calcul serverless.</span><span class="sxs-lookup"><span data-stu-id="655ae-249">Added `--compute-model`, `--auto-pause-delay`, and `--min-capacity` parameters to support CRUD operations for new SQL Database offering: Serverless compute model.</span></span>

### <a name="storage"></a><span data-ttu-id="655ae-250">Stockage</span><span class="sxs-lookup"><span data-stu-id="655ae-250">Storage</span></span>

* <span data-ttu-id="655ae-251">`az storage account create/update`: Ajout du paramètre --enable-files-adds et du groupe d’arguments de propriétés Azure Active Directory pour prendre en charge l’authentification de service de domaine Azure Files Active Directory</span><span class="sxs-lookup"><span data-stu-id="655ae-251">`az storage account create/update`: Added --enable-files-adds parameter and Azure Active Directory Properties Argument group to support Azure Files Active Directory Domain Service Authentication</span></span>
* <span data-ttu-id="655ae-252">Développement de `az storage account keys list/renew` pour prendre en charge le listing ou la regénération des clés Kerberos du compte de stockage.</span><span class="sxs-lookup"><span data-stu-id="655ae-252">Expanded `az storage account keys list/renew` to support listing or regenerating Kerberos keys of storage account.</span></span>

## <a name="october-15-2019"></a><span data-ttu-id="655ae-253">15 octobre 2019</span><span class="sxs-lookup"><span data-stu-id="655ae-253">October 15, 2019</span></span>

<span data-ttu-id="655ae-254">Version 2.0.75</span><span class="sxs-lookup"><span data-stu-id="655ae-254">Version 2.0.75</span></span>

### <a name="aks"></a><span data-ttu-id="655ae-255">AKS</span><span class="sxs-lookup"><span data-stu-id="655ae-255">AKS</span></span>

* <span data-ttu-id="655ae-256">Remplacement de la valeur par défaut `--load-balancer-sku` par `standard` si elle est prise en charge par la version kubernetes</span><span class="sxs-lookup"><span data-stu-id="655ae-256">Changed `--load-balancer-sku` default value to `standard` if supported by the kubernetes version</span></span>
* <span data-ttu-id="655ae-257">Remplacement de la valeur par défaut `--vm-set-type` par `virtualmachinescalesets` si elle est prise en charge par la version kubernetes</span><span class="sxs-lookup"><span data-stu-id="655ae-257">Changed `--vm-set-type` default value to `virtualmachinescalesets` if supported by the kubernetes version</span></span>

### <a name="ams"></a><span data-ttu-id="655ae-258">AMS</span><span class="sxs-lookup"><span data-stu-id="655ae-258">AMS</span></span>

* <span data-ttu-id="655ae-259">[CHANGEMENT CASSANT] Remplacement du nom `job start` par `job create`</span><span class="sxs-lookup"><span data-stu-id="655ae-259">[BREAKING CHANGE] Changed the name of `job start` to `job create`</span></span>
* <span data-ttu-id="655ae-260">[CHANGEMENT CASSANT] Changement du paramètre `--ask` de `content-key-policy create` pour utiliser une chaîne hexadécimale de 32 caractères au lieu d’UTF8</span><span class="sxs-lookup"><span data-stu-id="655ae-260">[BREAKING CHANGE] Changed the `--ask` parameter of `content-key-policy create` to use a 32-character hex string instead of UTF8</span></span>

### <a name="appservice"></a><span data-ttu-id="655ae-261">AppService</span><span class="sxs-lookup"><span data-stu-id="655ae-261">AppService</span></span>

* <span data-ttu-id="655ae-262">Ajout des commandes `webapp config access-restriction show|set|add|remove`</span><span class="sxs-lookup"><span data-stu-id="655ae-262">Added commands `webapp config access-restriction show|set|add|remove`</span></span>
* <span data-ttu-id="655ae-263">Ajout d’une meilleure gestion des erreurs à `webapp up`</span><span class="sxs-lookup"><span data-stu-id="655ae-263">Added better error handling to `webapp up`</span></span>
* <span data-ttu-id="655ae-264">Ajout de la prise en charge de la référence SKU `Isolated` pour `appservice plan update`</span><span class="sxs-lookup"><span data-stu-id="655ae-264">Added support for `Isolated` SKU to `appservice plan update`</span></span>

### <a name="arm"></a><span data-ttu-id="655ae-265">ARM</span><span class="sxs-lookup"><span data-stu-id="655ae-265">ARM</span></span>

* <span data-ttu-id="655ae-266">Ajout du paramètre `--handle-extended-json-format` à `deployment create` pour prendre en charge le format multiligne et les commentaires dans le modèle json</span><span class="sxs-lookup"><span data-stu-id="655ae-266">Added `--handle-extended-json-format` parameter `deployment create` to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="655ae-267">Calcul</span><span class="sxs-lookup"><span data-stu-id="655ae-267">Compute</span></span>

* <span data-ttu-id="655ae-268">Ajout du paramètre `--enable-agent` pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="655ae-268">Added `--enable-agent` parameter to `vm create`</span></span>
* <span data-ttu-id="655ae-269">Changement de `vm create` pour utiliser automatiquement la référence SKU d’adresse IP publique standard lors de l’utilisation de zones</span><span class="sxs-lookup"><span data-stu-id="655ae-269">Changed `vm create` to use standard public IP SKU automatically when using zones</span></span>
* <span data-ttu-id="655ae-270">Changement de `vm create` pour créer automatiquement un nom d’ordinateur valide pour une machine virtuelle si aucun n’est fourni</span><span class="sxs-lookup"><span data-stu-id="655ae-270">Changed `vm create` to automatically create a valid computer name for a VM if none is provided</span></span>
* <span data-ttu-id="655ae-271">Ajout du paramètre `--computer-name-prefix` à `vmss create` pour prendre en charge le préfixe de nom d’ordinateur personnalisé des machines virtuelles dans VMSS</span><span class="sxs-lookup"><span data-stu-id="655ae-271">Added `--computer-name-prefix` parameter to `vmss create` to support custom computer name prefix of virtual machines in the VMSS</span></span>
* <span data-ttu-id="655ae-272">Ajout du paramètre `--workspace` à `vm create` pour activer automatiquement l’espace de travail Log Analytics</span><span class="sxs-lookup"><span data-stu-id="655ae-272">Add `--workspace` parameter to `vm create` to enable log analytics workspace automatically</span></span>
* <span data-ttu-id="655ae-273">Mise à jour de la version de l’API des galeries vers 2019-07-01</span><span class="sxs-lookup"><span data-stu-id="655ae-273">Updated galleries API version to 2019-07-01</span></span>

### <a name="core"></a><span data-ttu-id="655ae-274">Core</span><span class="sxs-lookup"><span data-stu-id="655ae-274">Core</span></span>

* <span data-ttu-id="655ae-275">Ajout de la vérification de la syntaxe pour le paramètre `--set` dans la commande de mise à jour générique</span><span class="sxs-lookup"><span data-stu-id="655ae-275">Added syntax check for `--set` parameter in generic update command</span></span>

### <a name="iot"></a><span data-ttu-id="655ae-276">IoT</span><span class="sxs-lookup"><span data-stu-id="655ae-276">IoT</span></span>

* <span data-ttu-id="655ae-277">Résolution d’un problème où `iot hub show` entraînait une erreur incorrecte « ressource introuvable »</span><span class="sxs-lookup"><span data-stu-id="655ae-277">Fixed an issue where `iot hub show` would incorrectly error with "resource not found"</span></span>

### <a name="monitor"></a><span data-ttu-id="655ae-278">Surveiller</span><span class="sxs-lookup"><span data-stu-id="655ae-278">Monitor</span></span>

* <span data-ttu-id="655ae-279">Ajout de la prise en charge de CRUD dans `monitor log-analytics workspace`</span><span class="sxs-lookup"><span data-stu-id="655ae-279">Added support for CRUD to `monitor log-analytics workspace`</span></span>

### <a name="network"></a><span data-ttu-id="655ae-280">Réseau</span><span class="sxs-lookup"><span data-stu-id="655ae-280">Network</span></span>

* <span data-ttu-id="655ae-281">Ajout de la prise en charge de la liaison virtuelle interlocataire dans `network private-dns link vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="655ae-281">Added support for cross-tenant virtual linking to `network private-dns link vnet [create|update]`</span></span>
* <span data-ttu-id="655ae-282">[CHANGEMENT CASSANT] Changement de `network vnet subnet list` pour exiger les paramètres `--resource-group` et `--vnet-name`</span><span class="sxs-lookup"><span data-stu-id="655ae-282">[BREAKING CHANGE] Changed `network vnet subnet list` to require `--resource-group` and `--vnet-name` parameters</span></span>

### <a name="sql"></a><span data-ttu-id="655ae-283">SQL</span><span class="sxs-lookup"><span data-stu-id="655ae-283">SQL</span></span>

* <span data-ttu-id="655ae-284">Ajout de commandes à `sql mi ad-admin` qui prennent en charge la définition d’un administrateur AAD sur des instances managées</span><span class="sxs-lookup"><span data-stu-id="655ae-284">Added commands to `sql mi ad-admin` that support setting an AAD administrator on managed instances</span></span>

### <a name="storage"></a><span data-ttu-id="655ae-285">Stockage</span><span class="sxs-lookup"><span data-stu-id="655ae-285">Storage</span></span>

* <span data-ttu-id="655ae-286">Ajout du paramètre `--preserve-s2s-access-tier` à `storage copy` pour préserver le niveau d’accès lors d’une copie de service à service</span><span class="sxs-lookup"><span data-stu-id="655ae-286">Added `--preserve-s2s-access-tier` parameter `storage copy` to preserve access tier during service to service copy</span></span>
* <span data-ttu-id="655ae-287">Ajout du paramètre `--enable-large-file-share` à `storage account [create|update]` afin de prendre en charge les gros partages de fichiers pour le compte de stockage</span><span class="sxs-lookup"><span data-stu-id="655ae-287">Added `--enable-large-file-share` parameter to `storage account [create|update]` to support large file shares for storage account</span></span>

## <a name="september-24-2019"></a><span data-ttu-id="655ae-288">24 septembre 2019</span><span class="sxs-lookup"><span data-stu-id="655ae-288">September 24, 2019</span></span>

<span data-ttu-id="655ae-289">Version 2.0.74</span><span class="sxs-lookup"><span data-stu-id="655ae-289">Version 2.0.74</span></span>

### <a name="acr"></a><span data-ttu-id="655ae-290">ACR</span><span class="sxs-lookup"><span data-stu-id="655ae-290">ACR</span></span>

* <span data-ttu-id="655ae-291">Ajout d’un paramètre `--type` obligatoire à `acr config retention update`</span><span class="sxs-lookup"><span data-stu-id="655ae-291">Added a required `--type` parameter to `acr config retention update`</span></span>
* <span data-ttu-id="655ae-292">[CHANGEMENT CASSANT] Remplacement du paramètre `--name -n` par `--registry -r ` pour le groupe de commandes `acr config`</span><span class="sxs-lookup"><span data-stu-id="655ae-292">[BREAKING CHNAGE] Renamed parameter `--name -n` changed to `--registry -r ` for `acr config` command group</span></span>

### <a name="aks"></a><span data-ttu-id="655ae-293">AKS</span><span class="sxs-lookup"><span data-stu-id="655ae-293">AKS</span></span>

* <span data-ttu-id="655ae-294">Ajout du paramètre `--load-balancer-sku` à la commande `aks create`, ce qui permet de créer un cluster AKS avec SLB</span><span class="sxs-lookup"><span data-stu-id="655ae-294">Added `--load-balancer-sku` parameter to `aks create` command, which allows for creating AKS cluster with SLB</span></span>
* <span data-ttu-id="655ae-295">Ajout des paramètres `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` et `--load-balancer-outbound-ip-prefixes` aux commandes `aks [create|update]`, ce qui permet de mettre à jour le profil d’équilibreur de charge d’un cluster AKS avec SLB</span><span class="sxs-lookup"><span data-stu-id="655ae-295">Added `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` and `--load-balancer-outbound-ip-prefixes` parameters to `aks [create|update]` commands, which allow for updating load balancer profile of an AKS cluster with SLB</span></span>
* <span data-ttu-id="655ae-296">Ajout du paramètre `--vm-set-type` à la commande `aks create`, ce qui permet de spécifier les types de machines virtuelles d’un cluster AKS (vmas ou vmss)</span><span class="sxs-lookup"><span data-stu-id="655ae-296">Added `--vm-set-type` parameter to `aks create` command, which allows to specify vm types of an AKS Cluster (vmas or vmss)</span></span>

### <a name="arm"></a><span data-ttu-id="655ae-297">ARM</span><span class="sxs-lookup"><span data-stu-id="655ae-297">ARM</span></span>

* <span data-ttu-id="655ae-298">Ajout du paramètre `--handle-extended-json-format` à la commande `group deployment create` pour prendre en charge les lignes multiples et les commentaires dans le modèle JSON</span><span class="sxs-lookup"><span data-stu-id="655ae-298">Added `--handle-extended-json-format` parameter to `group deployment create` command to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="655ae-299">Calcul</span><span class="sxs-lookup"><span data-stu-id="655ae-299">Compute</span></span>

* <span data-ttu-id="655ae-300">Ajout du paramètre `--terminate-notification-time` aux commandes `vmss [create|update]` pour prendre en charge la configuration de l’événement planifié d’arrêt</span><span class="sxs-lookup"><span data-stu-id="655ae-300">Added `--terminate-notification-time` parameter to `vmss [create|update]` commands to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="655ae-301">Ajout du paramètre `--enable-terminate-notification` à la commande `vmss update` pour prendre en charge la configuration de l’événement planifié d’arrêt</span><span class="sxs-lookup"><span data-stu-id="655ae-301">Added `--enable-terminate-notification` parameter to `vmss update` command to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="655ae-302">Ajout des paramètres `--priority,` `--eviction-policy,` `--max-billing` aux commandes `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="655ae-302">Added `--priority,` `--eviction-policy,` `--max-billing` parameters to `[vm|vmss] create` commands</span></span>
* <span data-ttu-id="655ae-303">Modification de `disk create` pour autoriser la spécification de la taille exacte du chargement de disque</span><span class="sxs-lookup"><span data-stu-id="655ae-303">Changed `disk create` to allow specifying the exact size of the disk upload</span></span>
* <span data-ttu-id="655ae-304">Ajout de la prise en charge des instantanés incrémentiels pour les disques managés à `snapshot create`</span><span class="sxs-lookup"><span data-stu-id="655ae-304">Added support for incremental snapshots for managed disks to `snapshot create`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="655ae-305">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="655ae-305">Cosmos DB</span></span>

* <span data-ttu-id="655ae-306">Ajout du paramètre `--type <key-type>` à la commande `cosmosdb keys list` pour afficher la clé, les clés en lecture seule ou les chaînes de connexion</span><span class="sxs-lookup"><span data-stu-id="655ae-306">Added `--type <key-type>` parameter to `cosmosdb keys list` command to show key, read only keys or connection strings</span></span>
* <span data-ttu-id="655ae-307">Ajout de la commande `cosmosdb keys regenerate`</span><span class="sxs-lookup"><span data-stu-id="655ae-307">Added `cosmosdb keys regenerate` command</span></span>
* <span data-ttu-id="655ae-308">[DÉPRÉCIATION] Dépréciation des commandes `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` et `cosmosdb list-read-only-keys`</span><span class="sxs-lookup"><span data-stu-id="655ae-308">[DEPRECATED] Deprecated `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` and `cosmosdb list-read-only-keys` commands</span></span>

### <a name="eventgrid"></a><span data-ttu-id="655ae-309">EventGrid</span><span class="sxs-lookup"><span data-stu-id="655ae-309">EventGrid</span></span>

* <span data-ttu-id="655ae-310">Correction du texte d’aide du point de terminaison de manière à faire référence au bon paramètre</span><span class="sxs-lookup"><span data-stu-id="655ae-310">Fixed the endpoint help text to refer to the right parameter</span></span>

### <a name="key-vault"></a><span data-ttu-id="655ae-311">Key Vault</span><span class="sxs-lookup"><span data-stu-id="655ae-311">Key Vault</span></span>

* <span data-ttu-id="655ae-312">Résolution d’un problème de connexion avec un locataire (`login -t`) qui pouvait provoquer l’échec de `keyvault create`</span><span class="sxs-lookup"><span data-stu-id="655ae-312">Fixed issue where logging in with a tenant (`login -t`) could cause `keyvault create` to fail</span></span>

### <a name="monitor"></a><span data-ttu-id="655ae-313">Surveiller</span><span class="sxs-lookup"><span data-stu-id="655ae-313">Monitor</span></span>

* <span data-ttu-id="655ae-314">Résolution d’un problème où le caractère `:` n’était pas autorisé dans l’argument `--condition` de `monitor metrics alert create`</span><span class="sxs-lookup"><span data-stu-id="655ae-314">Fixed issue where `:` character was not allowed in `--condition` argument to `monitor metrics alert create`</span></span>

### <a name="policy"></a><span data-ttu-id="655ae-315">Stratégie</span><span class="sxs-lookup"><span data-stu-id="655ae-315">Policy</span></span>

* <span data-ttu-id="655ae-316">Ajout de la prise en charge de l’API Policy version 2019-06-01</span><span class="sxs-lookup"><span data-stu-id="655ae-316">Added support for Policy API version 2019-06-01</span></span>
* <span data-ttu-id="655ae-317">Ajout du paramètre `--enforcement-mode` à la commande `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="655ae-317">Added `--enforcement-mode` parameter to `policy assignment create` command</span></span>

### <a name="storage"></a><span data-ttu-id="655ae-318">Stockage</span><span class="sxs-lookup"><span data-stu-id="655ae-318">Storage</span></span>

* <span data-ttu-id="655ae-319">Ajout du paramètre `--blob-type` à la commande `az storage copy`</span><span class="sxs-lookup"><span data-stu-id="655ae-319">Added `--blob-type` parameter to `az storage copy` command</span></span>

## <a name="september-10-2019"></a><span data-ttu-id="655ae-320">10 septembre 2019</span><span class="sxs-lookup"><span data-stu-id="655ae-320">September 10, 2019</span></span>

### <a name="acr"></a><span data-ttu-id="655ae-321">ACR</span><span class="sxs-lookup"><span data-stu-id="655ae-321">ACR</span></span>

* <span data-ttu-id="655ae-322">Ajout du groupe de commandes `acr config retention` pour configurer une stratégie de conservation</span><span class="sxs-lookup"><span data-stu-id="655ae-322">Added command group `acr config retention` to configure retention policy</span></span>

### <a name="aks"></a><span data-ttu-id="655ae-323">AKS</span><span class="sxs-lookup"><span data-stu-id="655ae-323">AKS</span></span>

* <span data-ttu-id="655ae-324">Ajout de la prise en charge de l’intégration ACR avec les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="655ae-324">Added support for ACR integration with the following commands:</span></span>
  * <span data-ttu-id="655ae-325">Ajout du paramètre `--attach-acr` à `aks [create|update]` pour attacher un ACR à un cluster AKS</span><span class="sxs-lookup"><span data-stu-id="655ae-325">Added `--attach-acr` parameter to `aks [create|update]` to attach an ACR to an AKS cluster</span></span>
  * <span data-ttu-id="655ae-326">Ajout du paramètre `--detach-acr` à `aks update` pour détacher l’ACR d’un cluster AKS</span><span class="sxs-lookup"><span data-stu-id="655ae-326">Added `--detach-acr` parameter to `aks update` to detach the ACR from an AKS cluster</span></span>

### <a name="arm"></a><span data-ttu-id="655ae-327">ARM</span><span class="sxs-lookup"><span data-stu-id="655ae-327">ARM</span></span>

* <span data-ttu-id="655ae-328">Mis à jour pour utiliser la version d’API 2019-05-10</span><span class="sxs-lookup"><span data-stu-id="655ae-328">Updated to use API version 2019-05-10</span></span>

### <a name="batch"></a><span data-ttu-id="655ae-329">Batch</span><span class="sxs-lookup"><span data-stu-id="655ae-329">Batch</span></span>

* <span data-ttu-id="655ae-330">Ajout de nouveaux paramètres de configuration JSON à `--json-file` pour `batch pool create` :</span><span class="sxs-lookup"><span data-stu-id="655ae-330">Added new JSON configuration settings to `--json-file` for `batch pool create`:</span></span>
  * <span data-ttu-id="655ae-331">Ajout de `MountConfigurations` pour les montages de système de fichiers (voir https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body pour les détails)</span><span class="sxs-lookup"><span data-stu-id="655ae-331">Added `MountConfigurations` for file system mounts (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
  * <span data-ttu-id="655ae-332">Ajout de la propriété facultative `publicIPs` sur `NetworkConfiguration` pour les adresses IP publiques sur les pools (voir https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body pour les détails)</span><span class="sxs-lookup"><span data-stu-id="655ae-332">Added optional property `publicIPs` on `NetworkConfiguration` for public IPs on pools (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
* <span data-ttu-id="655ae-333">Ajout de la prise en charge des galeries d’images partagées à `--image`</span><span class="sxs-lookup"><span data-stu-id="655ae-333">Added support for shared image galleries to `--image`</span></span>
* <span data-ttu-id="655ae-334">[CHANGEMENT CASSANT] Changement de la valeur par défaut `--start-task-wait-for-success` sur `batch pool create` qui devient `true`</span><span class="sxs-lookup"><span data-stu-id="655ae-334">[BREAKING CHANGE] Changed default value of `--start-task-wait-for-success` on `batch pool create` to be `true`</span></span>
* <span data-ttu-id="655ae-335">[CHANGEMENT CASSANT] Changement de la valeur par défaut pour `Scope` sur `AutoUserSpecification` pour qu’elle soit toujours Pool (était `Task` sur les nœuds Windows, `Pool` sur les nœuds Linux)</span><span class="sxs-lookup"><span data-stu-id="655ae-335">[BREAKING CHANGE] Changed default value for `Scope` on `AutoUserSpecification` to always be Pool (was `Task` on Windows nodes, `Pool` on Linux nodes)</span></span>
  * <span data-ttu-id="655ae-336">Cet argument ne peut être défini qu’à partir d’une configuration JSON avec `--json-file`</span><span class="sxs-lookup"><span data-stu-id="655ae-336">This argument can only be set from a JSON configuration with `--json-file`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="655ae-337">HDInsight</span><span class="sxs-lookup"><span data-stu-id="655ae-337">HDInsight</span></span>

* <span data-ttu-id="655ae-338">Version mise à la disposition générale</span><span class="sxs-lookup"><span data-stu-id="655ae-338">GA release</span></span>
* <span data-ttu-id="655ae-339">[CHANGEMENT CASSANT] Changement du paramètre `--workernode-count/-c` de `az hdinsight resize` pour le rendre obligatoire.</span><span class="sxs-lookup"><span data-stu-id="655ae-339">[BREAKING CHANGE] Changed parameter `--workernode-count/-c` of `az hdinsight resize` to be required.</span></span>

### <a name="key-vault"></a><span data-ttu-id="655ae-340">Key Vault</span><span class="sxs-lookup"><span data-stu-id="655ae-340">Key Vault</span></span>

* <span data-ttu-id="655ae-341">Résolution d’un problème où les sous-réseaux ne pouvaient pas être supprimés des règles réseau</span><span class="sxs-lookup"><span data-stu-id="655ae-341">Fixed issue where subnets couldn't be deleted from network rules</span></span>
* <span data-ttu-id="655ae-342">Résolution d’un problème où des sous-réseaux et des adresses IP dupliqués pouvaient être ajoutés aux règles réseau</span><span class="sxs-lookup"><span data-stu-id="655ae-342">Fixed issue where duplicated subnets and IP addresses could be added to network rules</span></span>

### <a name="network"></a><span data-ttu-id="655ae-343">Réseau</span><span class="sxs-lookup"><span data-stu-id="655ae-343">Network</span></span>

* <span data-ttu-id="655ae-344">Ajout du paramètre `--interval` à `network watcher flow-log` pour définir la valeur d’intervalle de l’analyse du trafic</span><span class="sxs-lookup"><span data-stu-id="655ae-344">Added `--interval` parameter to `network watcher flow-log` to set traffic analysis interval value</span></span>
* <span data-ttu-id="655ae-345">Ajout de `network application-gateway identity` pour gérer l’identité de la passerelle</span><span class="sxs-lookup"><span data-stu-id="655ae-345">Added `network application-gateway identity` to manage gateway identity</span></span>
* <span data-ttu-id="655ae-346">Ajout de la prise en charge de la définition de l’ID Key Vault sur `network application-gateway ssl-cert`</span><span class="sxs-lookup"><span data-stu-id="655ae-346">Added support for setting Key Vault ID to `network application-gateway ssl-cert`</span></span>
* <span data-ttu-id="655ae-347">Ajout de `network express-route peering peer-connection [show|list]`</span><span class="sxs-lookup"><span data-stu-id="655ae-347">Added `network express-route peering peer-connection [show|list]`</span></span>

### <a name="policy"></a><span data-ttu-id="655ae-348">Stratégie</span><span class="sxs-lookup"><span data-stu-id="655ae-348">Policy</span></span>

* <span data-ttu-id="655ae-349">Mis à jour pour utiliser la version d’API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="655ae-349">Updated to use API version 2019-01-01</span></span>

## <a name="august-27-2019"></a><span data-ttu-id="655ae-350">27 août 2019</span><span class="sxs-lookup"><span data-stu-id="655ae-350">August 27, 2019</span></span>

<span data-ttu-id="655ae-351">Version 2.0.72</span><span class="sxs-lookup"><span data-stu-id="655ae-351">Version 2.0.72</span></span>

### <a name="acr"></a><span data-ttu-id="655ae-352">ACR</span><span class="sxs-lookup"><span data-stu-id="655ae-352">ACR</span></span>

* <span data-ttu-id="655ae-353">[CHANGEMENT CASSANT] Suppression de la prise en charge de la référence SKU `classic`</span><span class="sxs-lookup"><span data-stu-id="655ae-353">[BREAKING CHANGE] Removed support for the `classic` SKU</span></span>

### <a name="api-management"></a><span data-ttu-id="655ae-354">Gestion des API</span><span class="sxs-lookup"><span data-stu-id="655ae-354">API Management</span></span>

* <span data-ttu-id="655ae-355">[PRÉVERSION] Ajout du groupe de commandes `apim`</span><span class="sxs-lookup"><span data-stu-id="655ae-355">[PREVIEW] Added `apim` command group</span></span>

### <a name="appservice"></a><span data-ttu-id="655ae-356">AppService</span><span class="sxs-lookup"><span data-stu-id="655ae-356">AppService</span></span>

* <span data-ttu-id="655ae-357">Résolution du problème avec la commande `webapp webjob continuous start` lors de la spécification d’un emplacement</span><span class="sxs-lookup"><span data-stu-id="655ae-357">Fixed issue with `webapp webjob continuous start` command when specifying a slot</span></span>
* <span data-ttu-id="655ae-358">Modification de `webapp up` pour détecter le dossier `env` et le supprimer du fichier utilisé pour le déploiement</span><span class="sxs-lookup"><span data-stu-id="655ae-358">Changed `webapp up` to detect `env` folder and remove it from the file used for deployment</span></span>

### <a name="keyvault"></a><span data-ttu-id="655ae-359">KeyVault</span><span class="sxs-lookup"><span data-stu-id="655ae-359">Keyvault</span></span>

* <span data-ttu-id="655ae-360">Correction d’un bogue dans `keyvault secret set` qui ignorait l’argument `--expires`</span><span class="sxs-lookup"><span data-stu-id="655ae-360">Fixed a bug in `keyvault secret set` that igored the `--expires` argument</span></span>

### <a name="network"></a><span data-ttu-id="655ae-361">Réseau</span><span class="sxs-lookup"><span data-stu-id="655ae-361">Network</span></span>

* <span data-ttu-id="655ae-362">Ajout de la prise en charge des adresses IPv6 pour les arguments `--private-ip-address-version`</span><span class="sxs-lookup"><span data-stu-id="655ae-362">Added support for IPv6 addresses to `--private-ip-address-version` arguments</span></span>
* <span data-ttu-id="655ae-363">Ajout des nouvelles commandes `network private-endpoint [create|update|list-types]` pour la gestion des points de terminaison privés</span><span class="sxs-lookup"><span data-stu-id="655ae-363">Added new commands `network private-endpoint [create|update|list-types]` for private endpoint management</span></span>
* <span data-ttu-id="655ae-364">Ajout du groupe de commandes `network private-link-service`</span><span class="sxs-lookup"><span data-stu-id="655ae-364">Added command group `network private-link-service`</span></span>
* <span data-ttu-id="655ae-365">Ajout des arguments `--private-endpoint-network-policies` et `--private-link-service-network-policies` à `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="655ae-365">Added `--private-endpoint-network-policies` and `--private-link-service-network-policies` arguments to `network vnet subnet update`</span></span>

### <a name="rbac"></a><span data-ttu-id="655ae-366">RBAC</span><span class="sxs-lookup"><span data-stu-id="655ae-366">RBAC</span></span>

* <span data-ttu-id="655ae-367">Correction du problème `ad app update --homepage` où la page d’accueil ne se mettait pas à jour</span><span class="sxs-lookup"><span data-stu-id="655ae-367">Fixed issue with `ad app update --homepage` where homepage would not be updated</span></span>

### <a name="servicefabric"></a><span data-ttu-id="655ae-368">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="655ae-368">ServiceFabric</span></span>

* <span data-ttu-id="655ae-369">Ajout de la prise en charge pour les noms Key Vault en casse mixte</span><span class="sxs-lookup"><span data-stu-id="655ae-369">Added support for mixed-case Key Vault names</span></span>
* <span data-ttu-id="655ae-370">Résolution du problème lors de l’utilisation de certificats dans Key Vault</span><span class="sxs-lookup"><span data-stu-id="655ae-370">Fixed issue when using certificates in Key Vault</span></span>
* <span data-ttu-id="655ae-371">Résolution du problème lors de l’utilisation des fichiers de certificat PFX</span><span class="sxs-lookup"><span data-stu-id="655ae-371">Fixed issue with using PFX certificate files</span></span>
* <span data-ttu-id="655ae-372">Correction du problème avec `sf cluster certificate add` quand le groupe de ressources Key Vault n’était pas spécifié</span><span class="sxs-lookup"><span data-stu-id="655ae-372">Fixed issue with `sf cluster certificate add` when Key Vault resource group wasn't specified</span></span>
* <span data-ttu-id="655ae-373">Correction du problème où `sf cluster set` ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="655ae-373">Fixed issue with `sf cluster set` not working</span></span>

### <a name="signalr"></a><span data-ttu-id="655ae-374">SignalR</span><span class="sxs-lookup"><span data-stu-id="655ae-374">SignalR</span></span>

* <span data-ttu-id="655ae-375">Ajout de nouvelles commandes :</span><span class="sxs-lookup"><span data-stu-id="655ae-375">Added new commands:</span></span>
  * <span data-ttu-id="655ae-376">`signalr cors`: Gérer SignalR CORS</span><span class="sxs-lookup"><span data-stu-id="655ae-376">`signalr cors`: Manage SignalR CORS</span></span>
  * <span data-ttu-id="655ae-377">`signalr restart`: Redémarrer un service SignalR</span><span class="sxs-lookup"><span data-stu-id="655ae-377">`signalr restart`: Restart a SignalR service</span></span>
  * <span data-ttu-id="655ae-378">`signalr update`: Mettre à jour un service SignalR</span><span class="sxs-lookup"><span data-stu-id="655ae-378">`signalr update`: Update a SignalR service</span></span>
* <span data-ttu-id="655ae-379">Ajout de l’argument `--service-mode` à `signalr create`</span><span class="sxs-lookup"><span data-stu-id="655ae-379">Added `--service-mode` argument to `signalr create`</span></span>

### <a name="storage"></a><span data-ttu-id="655ae-380">Stockage</span><span class="sxs-lookup"><span data-stu-id="655ae-380">Storage</span></span>

* <span data-ttu-id="655ae-381">Ajout de la commande `storage account revoke-delegation-keys`</span><span class="sxs-lookup"><span data-stu-id="655ae-381">Added `storage account revoke-delegation-keys` command</span></span>

## <a name="august-13-2019"></a><span data-ttu-id="655ae-382">13 août 2019</span><span class="sxs-lookup"><span data-stu-id="655ae-382">August 13, 2019</span></span>

<span data-ttu-id="655ae-383">Version 2.0.71</span><span class="sxs-lookup"><span data-stu-id="655ae-383">Version 2.0.71</span></span>

### <a name="appservice"></a><span data-ttu-id="655ae-384">AppService</span><span class="sxs-lookup"><span data-stu-id="655ae-384">AppService</span></span>

* <span data-ttu-id="655ae-385">Correction d’un problème entraînant l’échec des commandes `webapp webjob continuous` pour les emplacements</span><span class="sxs-lookup"><span data-stu-id="655ae-385">Fixed issue where `webapp webjob continuous` commands were failing for slots</span></span>

### <a name="botservice"></a><span data-ttu-id="655ae-386">BotService</span><span class="sxs-lookup"><span data-stu-id="655ae-386">BotService</span></span>

* <span data-ttu-id="655ae-387">[CHANGEMENT CASSANT] Suppression de la prise en charge de la création de bots SDK v3</span><span class="sxs-lookup"><span data-stu-id="655ae-387">[BREAKING CHANGE] Removed support for creating v3 SDK bots</span></span>

### <a name="cognitiveservices"></a><span data-ttu-id="655ae-388">CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="655ae-388">CognitiveServices</span></span>

* <span data-ttu-id="655ae-389">Ajout des commandes `cognitiveservices account network-rule`</span><span class="sxs-lookup"><span data-stu-id="655ae-389">Added `cognitiveservices account network-rule` commands</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="655ae-390">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="655ae-390">Cosmos DB</span></span>

* <span data-ttu-id="655ae-391">Suppression de l’avertissement lors de la mise à jour de plusieurs emplacements d’écriture</span><span class="sxs-lookup"><span data-stu-id="655ae-391">Removed warning when updating multiple write locations</span></span>
* <span data-ttu-id="655ae-392">Ajout de commandes CRUD pour les ressources CosmosDB SQL, MongoDB, Cassandra, Gremlin et Table et le débit de la ressource</span><span class="sxs-lookup"><span data-stu-id="655ae-392">Added CRUD commands for CosmosDB SQL, MongoDB, Cassandra, Gremlin and Table resources and resource's throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="655ae-393">HDInsight</span><span class="sxs-lookup"><span data-stu-id="655ae-393">HDInsight</span></span>

<span data-ttu-id="655ae-394">Cette version contient un grand nombre de modifications conséquentes.</span><span class="sxs-lookup"><span data-stu-id="655ae-394">This release contains a large number of breaking changes.</span></span>

* <span data-ttu-id="655ae-395">[CHANGEMENT CASSANT] Renommage des paramètres pour `hdinsight create` :</span><span class="sxs-lookup"><span data-stu-id="655ae-395">[BREAKING CHANGE] Renamed parameters for `hdinsight create`:</span></span>
  * <span data-ttu-id="655ae-396">Renommage de `--storage-default-container` en `--storage-container`</span><span class="sxs-lookup"><span data-stu-id="655ae-396">Renamed `--storage-default-container` to `--storage-container`</span></span>
  * <span data-ttu-id="655ae-397">Renommage de `--storage-default-filesystem` en `--storage-filesystem`</span><span class="sxs-lookup"><span data-stu-id="655ae-397">Renamed `--storage-default-filesystem` to `--storage-filesystem`</span></span>
* <span data-ttu-id="655ae-398">[CHANGEMENT CASSANT] Modification de l’argument `--name` de `application create` pour représenter le nom de l’application à la place du nom du cluster</span><span class="sxs-lookup"><span data-stu-id="655ae-398">[BREAKING CHANGE] Changed the `--name` argument of `application create` to represent the application name instead of the cluster name</span></span>
* <span data-ttu-id="655ae-399">Ajout d’un argument `--cluster-name` à `application create` pour remplacer l’ancienne fonctionnalité `--name`</span><span class="sxs-lookup"><span data-stu-id="655ae-399">Added `--cluster-name` argument to `application create` to replace old `--name` functionality</span></span>
* <span data-ttu-id="655ae-400">[CHANGEMENT CASSANT] Renommage des paramètres pour `application create` :</span><span class="sxs-lookup"><span data-stu-id="655ae-400">[BREAKING CHANGE] Renamed parameters for `application create`:</span></span>
  * <span data-ttu-id="655ae-401">Renommage de `--application-type` en `--type`</span><span class="sxs-lookup"><span data-stu-id="655ae-401">Renamed `--application-type` to `--type`</span></span>
  * <span data-ttu-id="655ae-402">Renommage de `--marketplace-identifier` en `--marketplace-id`</span><span class="sxs-lookup"><span data-stu-id="655ae-402">Renamed `--marketplace-identifier` to `--marketplace-id`</span></span>
  * <span data-ttu-id="655ae-403">Renommage de `--https-endpoint-access-mode` en `--access-mode`</span><span class="sxs-lookup"><span data-stu-id="655ae-403">Renamed `--https-endpoint-access-mode` to `--access-mode`</span></span>
  * <span data-ttu-id="655ae-404">`--https-endpoint-destination-port` renommé en `--destination-port`</span><span class="sxs-lookup"><span data-stu-id="655ae-404">Renamed  `--https-endpoint-destination-port` to `--destination-port`</span></span>
* <span data-ttu-id="655ae-405">[CHANGEMENT CASSANT] Suppression des paramètres pour `application create` :</span><span class="sxs-lookup"><span data-stu-id="655ae-405">[BREAKING CHANGE] Removed parameters for `application create`:</span></span>
  * `--https-endpoint-location`
  * `--https-endpoint-public-port`
  * `--ssh-endpoint-destination-port`
  * `--ssh-endpoint-location`
  * `--ssh-endpoint-public-port`
* <span data-ttu-id="655ae-406">MODIFICATION CONSÉQUENTE Renommage de `--target-instance-count` en `--workernode-count` pour `hdinsight resize`</span><span class="sxs-lookup"><span data-stu-id="655ae-406">[BREAKING CHNAGE] Renamed `--target-instance-count` to `--workernode-count` for `hdinsight resize`</span></span>
* <span data-ttu-id="655ae-407">[CHANGEMENT CASSANT] Modification de toutes les commandes du groupe `hdinsight script-action` pour utiliser le paramètre `--name` comme nom de l’action de script.</span><span class="sxs-lookup"><span data-stu-id="655ae-407">[BREAKING CHANGE] Changed all commands in the `hdinsight script-action` group to use the `--name` parameter as the name of the script action.</span></span>
* <span data-ttu-id="655ae-408">Ajout d’un argument `--cluster-name` à toutes les commandes `hdinsight script-action` pour remplacer l’ancienne fonctionnalité `--name`</span><span class="sxs-lookup"><span data-stu-id="655ae-408">Added `--cluster-name` argument to all `hdinsight script-action` commands to replace old `--name` functionality</span></span>
* <span data-ttu-id="655ae-409">[CHANGEMENT CASSANT] Renommage de l’option `--script-execution-id` en `--execution-id` pour toutes les commandes `hdinsight script-action`</span><span class="sxs-lookup"><span data-stu-id="655ae-409">[BREAKING CHANGE] Renamed `--script-execution-id` to `--execution-id` for all `hdinsight script-action` commands</span></span>
* <span data-ttu-id="655ae-410">[CHANGEMENT CASSANT] Renommage de `hdinsight script-action show` en `hdinsight script-action show-execution-details`</span><span class="sxs-lookup"><span data-stu-id="655ae-410">[BREAKING CHANGE] Renamed `hdinsight script-action show` to `hdinsight script-action show-execution-details`</span></span>
* <span data-ttu-id="655ae-411">[MODIFICATION CONSÉQUENTE] Modification des paramètres sur `hdinsight script-action execute --roles` pour qu’ils soient séparés par des espaces et non par des virgules</span><span class="sxs-lookup"><span data-stu-id="655ae-411">[BREAKING CHNAGE] Changed parameters to `hdinsight script-action execute --roles` to be space-separated instead of comma-separated</span></span>
* <span data-ttu-id="655ae-412">[CHANGEMENT CASSANT] Suppression du paramètre `--persisted` de `hdinsight script-action list`</span><span class="sxs-lookup"><span data-stu-id="655ae-412">[BREAKING CHANGE] Removed the `--persisted` parameter of `hdinsight script-action list`</span></span>
* <span data-ttu-id="655ae-413">Modification du paramètre `hdinsight create --cluster-configurations` pour qu’il accepte un chemin d’accès à un fichier JSON local ou une chaîne JSON</span><span class="sxs-lookup"><span data-stu-id="655ae-413">Changed the `hdinsight create --cluster-configurations` parameter to accept a path to a local JSON file or a JSON string</span></span>
* <span data-ttu-id="655ae-414">Ajout de la commande `hdinsight script-action list-execution-history`</span><span class="sxs-lookup"><span data-stu-id="655ae-414">Added command `hdinsight script-action list-execution-history`</span></span>
* <span data-ttu-id="655ae-415">Modification de `hdinsight monitor enable --workspace` pour qu’il accepte un ID ou un nom d’espace de travail Log Analytics</span><span class="sxs-lookup"><span data-stu-id="655ae-415">Changed `hdinsight monitor enable --workspace` to accept a Log Analytics workspace ID or workspace name</span></span>
* <span data-ttu-id="655ae-416">Ajout de l’argument `hdinsight monitor enable --primary-key`, qui est nécessaire si un ID d’espace de travail est fourni en tant que paramètre</span><span class="sxs-lookup"><span data-stu-id="655ae-416">Added the `hdinsight monitor enable --primary-key` argument, which is needed if a workspace ID is provided as the parameter</span></span>
* <span data-ttu-id="655ae-417">Ajout de plus d’exemples et mise à jour des descriptions des messages d’aide</span><span class="sxs-lookup"><span data-stu-id="655ae-417">Added more examples and updated descriptions for help messages</span></span>

### <a name="interactive"></a><span data-ttu-id="655ae-418">Interactive</span><span class="sxs-lookup"><span data-stu-id="655ae-418">Interactive</span></span>

* <span data-ttu-id="655ae-419">Résolution d’une erreur de chargement</span><span class="sxs-lookup"><span data-stu-id="655ae-419">Fixed a loading error</span></span>

### <a name="kubernetes"></a><span data-ttu-id="655ae-420">kubernetes</span><span class="sxs-lookup"><span data-stu-id="655ae-420">Kubernetes</span></span>

* <span data-ttu-id="655ae-421">Modification pour utiliser `https` si le port du conteneur du tableau de bord utilise `https`</span><span class="sxs-lookup"><span data-stu-id="655ae-421">Changed to use `https` if dashboard container port is using `https`</span></span>

### <a name="network"></a><span data-ttu-id="655ae-422">Réseau</span><span class="sxs-lookup"><span data-stu-id="655ae-422">Network</span></span>

* <span data-ttu-id="655ae-423">Ajout de l’argument `--yes` `network dns record-set cname delete`</span><span class="sxs-lookup"><span data-stu-id="655ae-423">Added `--yes` argument `network dns record-set cname delete`</span></span>

### <a name="profile"></a><span data-ttu-id="655ae-424">Profil</span><span class="sxs-lookup"><span data-stu-id="655ae-424">Profile</span></span>

* <span data-ttu-id="655ae-425">Ajout de l’argument `--resource-type` à `account get-access-token` pour obtenir des jetons d’accès aux ressources</span><span class="sxs-lookup"><span data-stu-id="655ae-425">Added `--resource-type` argument to `account get-access-token` to get resource access tokens</span></span>

### <a name="servicefabric"></a><span data-ttu-id="655ae-426">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="655ae-426">ServiceFabric</span></span>

* <span data-ttu-id="655ae-427">Ajout de toutes les versions de système d’exploitation prises en charge pour sf cluster create</span><span class="sxs-lookup"><span data-stu-id="655ae-427">Added all supported os version for sf cluster create</span></span>
* <span data-ttu-id="655ae-428">Résolution d’un bogue principal de validation de certificat</span><span class="sxs-lookup"><span data-stu-id="655ae-428">Fixed primary certificate validation bug</span></span>

### <a name="storage"></a><span data-ttu-id="655ae-429">Stockage</span><span class="sxs-lookup"><span data-stu-id="655ae-429">Storage</span></span>

* <span data-ttu-id="655ae-430">Ajout de la commande `storage copy`</span><span class="sxs-lookup"><span data-stu-id="655ae-430">Added command `storage copy`</span></span>

## <a name="july-30-2019"></a><span data-ttu-id="655ae-431">30 juillet 2019</span><span class="sxs-lookup"><span data-stu-id="655ae-431">July 30, 2019</span></span>

<span data-ttu-id="655ae-432">Version 2.0.70</span><span class="sxs-lookup"><span data-stu-id="655ae-432">Version 2.0.70</span></span>

### <a name="acr"></a><span data-ttu-id="655ae-433">ACR</span><span class="sxs-lookup"><span data-stu-id="655ae-433">ACR</span></span>

* <span data-ttu-id="655ae-434">Correction du problème #9952 (régression dans la commande `acr pack build`)</span><span class="sxs-lookup"><span data-stu-id="655ae-434">Fixed issue #9952 (a regression in the `acr pack build` command)</span></span>
* <span data-ttu-id="655ae-435">Suppression du nom de l’image du générateur par défaut dans `acr pack build`</span><span class="sxs-lookup"><span data-stu-id="655ae-435">Removed the default builder image name in `acr pack build`</span></span>

### <a name="appservice"></a><span data-ttu-id="655ae-436">AppService</span><span class="sxs-lookup"><span data-stu-id="655ae-436">Appservice</span></span>

* <span data-ttu-id="655ae-437">Modification de `webapp config ssl` pour afficher un message si une ressource est introuvable</span><span class="sxs-lookup"><span data-stu-id="655ae-437">Changed `webapp config ssl` to show a message if a resource is not found</span></span>
* <span data-ttu-id="655ae-438">Correction du problème où `functionapp create` n’acceptait pas le type de compte de stockage `Standard_RAGRS`</span><span class="sxs-lookup"><span data-stu-id="655ae-438">Fixed issue where `functionapp create` does not accept `Standard_RAGRS` storage account type</span></span>
* <span data-ttu-id="655ae-439">Correction d’un problème où `webapp up` échouait s’il était exécuté avec des versions antérieures de Python</span><span class="sxs-lookup"><span data-stu-id="655ae-439">Fixed an issue where `webapp up` would fail if run using older versions of python</span></span>

### <a name="network"></a><span data-ttu-id="655ae-440">Réseau</span><span class="sxs-lookup"><span data-stu-id="655ae-440">Network</span></span>

* <span data-ttu-id="655ae-441">Suppression du paramètre non valide `--ids` de `network nic ip-config add` (correctifs #9861)</span><span class="sxs-lookup"><span data-stu-id="655ae-441">Removed invalid parameter `--ids` from `network nic ip-config add` (fixes #9861)</span></span>
* <span data-ttu-id="655ae-442">Correctifs #9604.</span><span class="sxs-lookup"><span data-stu-id="655ae-442">Fixes #9604.</span></span> <span data-ttu-id="655ae-443">Ajout du paramètre `--root-certs` à `network application-gateway http-settings [create|update]` pour prendre en charge les certificats racines approuvés associés à l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="655ae-443">Added `--root-certs` parameter to `network application-gateway http-settings [create|update]` to support user associate trusted root certificates.</span></span>
* <span data-ttu-id="655ae-444">Correction de l’argument `--subscription` pour `network dns record-set ns create` (#9965)</span><span class="sxs-lookup"><span data-stu-id="655ae-444">Fixed arguent `--subscription` for `network dns record-set ns create` (#9965)</span></span>

### <a name="rbac"></a><span data-ttu-id="655ae-445">RBAC</span><span class="sxs-lookup"><span data-stu-id="655ae-445">RBAC</span></span>

* <span data-ttu-id="655ae-446">Ajout de la commande `user update`</span><span class="sxs-lookup"><span data-stu-id="655ae-446">Added `user update` command</span></span>
* <span data-ttu-id="655ae-447">[DÉPRÉCIATION] Dépréciation de `--upn-or-object-id` des commandes associées à l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="655ae-447">[DEPRECATED] Deprecated `--upn-or-object-id` from user-related commands</span></span>
    * <span data-ttu-id="655ae-448">Utiliser l’argument de remplacement `--id`</span><span class="sxs-lookup"><span data-stu-id="655ae-448">Use replacement argument `--id`</span></span>
* <span data-ttu-id="655ae-449">Ajout de l’argument `--id` aux commandes associées à l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="655ae-449">Added `--id` argument to user-related commands</span></span>

### <a name="sql"></a><span data-ttu-id="655ae-450">SQL</span><span class="sxs-lookup"><span data-stu-id="655ae-450">SQL</span></span>

* <span data-ttu-id="655ae-451">Ajout de commandes de gestion pour les clés d’instance managée et le protecteur TDE</span><span class="sxs-lookup"><span data-stu-id="655ae-451">Added management commands for managed instance keys and TDE protector</span></span>

### <a name="storage"></a><span data-ttu-id="655ae-452">Stockage</span><span class="sxs-lookup"><span data-stu-id="655ae-452">Storage</span></span>

* <span data-ttu-id="655ae-453">Ajout de la commande `storage remove`</span><span class="sxs-lookup"><span data-stu-id="655ae-453">Added `storage remove` command</span></span>
* <span data-ttu-id="655ae-454">Correction d’un problème avec `storage blob update`</span><span class="sxs-lookup"><span data-stu-id="655ae-454">Fixed an issue with `storage blob update`</span></span>

### <a name="vm"></a><span data-ttu-id="655ae-455">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="655ae-455">VM</span></span>

* <span data-ttu-id="655ae-456">Changement de `list-skus` pour utiliser une version API plus récente dans les détails de la zone de sortie</span><span class="sxs-lookup"><span data-stu-id="655ae-456">Changed `list-skus` to use newer api-version to output zone details</span></span>
* <span data-ttu-id="655ae-457">Remplacement de la valeur par défaut `--single-placement-group` par `false` pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="655ae-457">Changed default of `--single-placement-group` to `false` for `vmss create`</span></span>
* <span data-ttu-id="655ae-458">Ajout de la possibilité de sélectionner des références SKU de stockage ZRS pour `[snapshot|disk] create`</span><span class="sxs-lookup"><span data-stu-id="655ae-458">Added ability to select ZRS storage SKUs for `[snapshot|disk] create`</span></span>
* <span data-ttu-id="655ae-459">Ajout d’un nouveau groupe de commandes `vm host` pour prendre en charge des hôtes dédiés</span><span class="sxs-lookup"><span data-stu-id="655ae-459">Added new command group `vm host` to support dedicated hosts</span></span>
* <span data-ttu-id="655ae-460">Ajout des paramètres `--host` et `--host-group` sur `vm create` pour définir l’hôte dédié à la machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="655ae-460">Added parameters `--host` and `--host-group` on `vm create` to set VM dedicated host</span></span>

## <a name="july-16-2019"></a><span data-ttu-id="655ae-461">16 juillet 2019</span><span class="sxs-lookup"><span data-stu-id="655ae-461">July 16, 2019</span></span>

<span data-ttu-id="655ae-462">Version 2.0.69</span><span class="sxs-lookup"><span data-stu-id="655ae-462">Version 2.0.69</span></span>

### <a name="appservice"></a><span data-ttu-id="655ae-463">AppService</span><span class="sxs-lookup"><span data-stu-id="655ae-463">Appservice</span></span>

* <span data-ttu-id="655ae-464">Changement des commandes `webapp identity` pour retourner un message d’erreur approprié si le nom de ResourceGroupName ou de l’application n’est pas valide</span><span class="sxs-lookup"><span data-stu-id="655ae-464">Changed `webapp identity` commands to return a proper error message if ResourceGroupName or App name are invalid</span></span>
* <span data-ttu-id="655ae-465">Correction de `webapp list` pour retourner la valeur correcte pour le nombre de sites si aucun groupe de ressources n’a été fourni</span><span class="sxs-lookup"><span data-stu-id="655ae-465">Fixed `webapp list` to return the correct value for numberOfSites if no ResourceGroup was provided</span></span>
* <span data-ttu-id="655ae-466">Correction des effets secondaires de `appservice plan create` et de `webapp create`</span><span class="sxs-lookup"><span data-stu-id="655ae-466">Fixed side-effects of `appservice plan create` and `webapp create`</span></span>

### <a name="core"></a><span data-ttu-id="655ae-467">Core</span><span class="sxs-lookup"><span data-stu-id="655ae-467">Core</span></span>

* <span data-ttu-id="655ae-468">Résolution du problème où `--subscription` s’affichait alors qu’il ne devait pas</span><span class="sxs-lookup"><span data-stu-id="655ae-468">Fixed issue where `--subscription` would appear despite being not applicable</span></span>

### <a name="batch"></a><span data-ttu-id="655ae-469">Batch</span><span class="sxs-lookup"><span data-stu-id="655ae-469">Batch</span></span>

* <span data-ttu-id="655ae-470">[CHANGEMENT CASSANT] Remplacement de `batch pool node-agent-skus list` par `batch pool supported-images list`</span><span class="sxs-lookup"><span data-stu-id="655ae-470">[BREAKING CHANGE] Replaced `batch pool node-agent-skus list` with `batch pool supported-images list`</span></span>
* <span data-ttu-id="655ae-471">Ajout de la prise en charge des règles de sécurité bloquant l’accès réseau à un pool basé sur le port source du trafic lors de l’utilisation de l’option `--json-file` de `batch pool create network`</span><span class="sxs-lookup"><span data-stu-id="655ae-471">Added support for security rules blocking network access to a pool based on the source port of the traffic when using the `--json-file` option of `batch pool create network`</span></span>
* <span data-ttu-id="655ae-472">Ajout de la prise en charge de l’exécution de la tâche dans le répertoire de travail du conteneur ou dans le répertoire de travail de la tâche Batch lors de l’utilisation de l’option `--json-file` de `batch task create`</span><span class="sxs-lookup"><span data-stu-id="655ae-472">Added support for executing the task in the container working directory or in the Batch task working directory when using the `--json-file` option of `batch task create`</span></span>
* <span data-ttu-id="655ae-473">Correction d’une erreur dans l’option `--application-package-references` de `batch pool create` où elle fonctionnait uniquement avec les valeurs par défaut</span><span class="sxs-lookup"><span data-stu-id="655ae-473">Fixed error in `--application-package-references` option of `batch pool create` where it would only work with defaults</span></span>

### <a name="eventhubs"></a><span data-ttu-id="655ae-474">Eventhubs</span><span class="sxs-lookup"><span data-stu-id="655ae-474">Eventhubs</span></span>

* <span data-ttu-id="655ae-475">Ajout d’une validation pour le paramètre `--rights` des commandes `authorizationrule`</span><span class="sxs-lookup"><span data-stu-id="655ae-475">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="rdbms"></a><span data-ttu-id="655ae-476">SGBDR</span><span class="sxs-lookup"><span data-stu-id="655ae-476">RDBMS</span></span>

* <span data-ttu-id="655ae-477">Ajout d’un paramètre facultatif pour spécifier la référence SKU de réplica pour la commande de création de réplica</span><span class="sxs-lookup"><span data-stu-id="655ae-477">Added optional parameter to specify replica SKU for create replica command</span></span>
* <span data-ttu-id="655ae-478">Correction d’un problème d’échec des tests CI lors de la création du réplica MySQL</span><span class="sxs-lookup"><span data-stu-id="655ae-478">Fixed the issue with CI test failure with creating MySQL replica</span></span>

### <a name="relay"></a><span data-ttu-id="655ae-479">Relais</span><span class="sxs-lookup"><span data-stu-id="655ae-479">Relay</span></span>

* <span data-ttu-id="655ae-480">Correction d’un problème de connexion hybride quand l’autorisation du client est désactivée [#8775](https://github.com/azure/azure-cli/issues/8775)</span><span class="sxs-lookup"><span data-stu-id="655ae-480">Fixed issue with hybrid connection when client authroization disabled [#8775](https://github.com/azure/azure-cli/issues/8775)</span></span>
* <span data-ttu-id="655ae-481">Ajout du paramètre `--requires-transport-security` à `relay wcfrelay create`</span><span class="sxs-lookup"><span data-stu-id="655ae-481">Added parameter `--requires-transport-security` to `relay wcfrelay create`</span></span>

### <a name="servicebus"></a><span data-ttu-id="655ae-482">Servicebus</span><span class="sxs-lookup"><span data-stu-id="655ae-482">Servicebus</span></span>

* <span data-ttu-id="655ae-483">Ajout d’une validation pour le paramètre `--rights` des commandes `authorizationrule`</span><span class="sxs-lookup"><span data-stu-id="655ae-483">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="storage"></a><span data-ttu-id="655ae-484">Stockage</span><span class="sxs-lookup"><span data-stu-id="655ae-484">Storage</span></span>

* <span data-ttu-id="655ae-485">Activation des fichiers AADDS pour la mise à jour du compte de stockage</span><span class="sxs-lookup"><span data-stu-id="655ae-485">Enable Files AADDS for storage account update</span></span>
* <span data-ttu-id="655ae-486">Problème résolu `storage blob service-properties update --set`</span><span class="sxs-lookup"><span data-stu-id="655ae-486">Fixed issue `storage blob service-properties update --set`</span></span>

## <a name="july-2-2019"></a><span data-ttu-id="655ae-487">2 juillet 2019</span><span class="sxs-lookup"><span data-stu-id="655ae-487">July 2, 2019</span></span>

<span data-ttu-id="655ae-488">Version 2.0.68</span><span class="sxs-lookup"><span data-stu-id="655ae-488">Version 2.0.68</span></span>

### <a name="core"></a><span data-ttu-id="655ae-489">Core</span><span class="sxs-lookup"><span data-stu-id="655ae-489">Core</span></span>

* <span data-ttu-id="655ae-490">Les modules de commande sont désormais consolidés en un seul distribuable Python.</span><span class="sxs-lookup"><span data-stu-id="655ae-490">Command modules are now consolidated into a single Python distributable.</span></span> <span data-ttu-id="655ae-491">L’utilisation directe de nombreux packages `azure-cli-` sur PyPI est donc dépréciée.</span><span class="sxs-lookup"><span data-stu-id="655ae-491">This deprecates direct use of many `azure-cli-` packages on PyPI.</span></span>
  <span data-ttu-id="655ae-492">Cela doit réduire la taille de l’installation et affecter uniquement les utilisateurs ayant procédé à une installation directe par le biais de `pip`.</span><span class="sxs-lookup"><span data-stu-id="655ae-492">This should reduce install size and only affect users who have directly installed via `pip`.</span></span>

### <a name="acr"></a><span data-ttu-id="655ae-493">ACR</span><span class="sxs-lookup"><span data-stu-id="655ae-493">ACR</span></span>

* <span data-ttu-id="655ae-494">Ajout de la prise en charge des déclencheurs de minuteur à la tâche</span><span class="sxs-lookup"><span data-stu-id="655ae-494">Added support for Timer Triggers to Task</span></span>

### <a name="appservice"></a><span data-ttu-id="655ae-495">AppService</span><span class="sxs-lookup"><span data-stu-id="655ae-495">Appservice</span></span>

* <span data-ttu-id="655ae-496">Modification de `functionapp create` pour activer Application Insights par défaut</span><span class="sxs-lookup"><span data-stu-id="655ae-496">Changed `functionapp create` to enable application insights by default</span></span>
* <span data-ttu-id="655ae-497">[CHANGEMENT CASSANT] Suppression de la commande `functionapp devops-build` dépréciée.</span><span class="sxs-lookup"><span data-stu-id="655ae-497">[BREAKING CHANGE] Removed deprecated `functionapp devops-build` command.</span></span>
  *  <span data-ttu-id="655ae-498">Utilisez la nouvelle commande `az functionapp devops-pipeline` à la place</span><span class="sxs-lookup"><span data-stu-id="655ae-498">Use the new command `az functionapp devops-pipeline` instead</span></span>
* <span data-ttu-id="655ae-499">Ajout de la prise en charge du plan d’application de fonction Consommation Linux à `functionapp deployment config-zip`</span><span class="sxs-lookup"><span data-stu-id="655ae-499">Added Linux Consumption function app plan support to `functionapp deployment config-zip`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="655ae-500">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="655ae-500">Cosmos DB</span></span>

* <span data-ttu-id="655ae-501">Ajout de la prise en charge de la désactivation de TTL</span><span class="sxs-lookup"><span data-stu-id="655ae-501">Added support for disabling TTL</span></span>

### <a name="dls"></a><span data-ttu-id="655ae-502">DLS</span><span class="sxs-lookup"><span data-stu-id="655ae-502">DLS</span></span>

* <span data-ttu-id="655ae-503">Mise à jour de la version d’ADLS (0.0.45)</span><span class="sxs-lookup"><span data-stu-id="655ae-503">Updated ADLS version (0.0.45)</span></span>

### <a name="feedback"></a><span data-ttu-id="655ae-504">Commentaires</span><span class="sxs-lookup"><span data-stu-id="655ae-504">Feedback</span></span>

* <span data-ttu-id="655ae-505">Lors du signalement d’une commande d’extension ayant échoué, `az feedback` tente à présent d’ouvrir le navigateur à l’URL du projet/dépôt de l’extension à partir de l’index</span><span class="sxs-lookup"><span data-stu-id="655ae-505">When reporting a failed extension command, `az feedback` now attempts to open the browser to the project/repo url of the extension from the index</span></span>

### <a name="hdinsight"></a><span data-ttu-id="655ae-506">HDInsight</span><span class="sxs-lookup"><span data-stu-id="655ae-506">HDInsight</span></span>

* <span data-ttu-id="655ae-507">[CHANGEMENT CASSANT] Remplacement du nom du groupe de commandes `oms` par `monitor`</span><span class="sxs-lookup"><span data-stu-id="655ae-507">[BREAKING CHANGE] Changed `oms` command group name to `monitor`</span></span>
* <span data-ttu-id="655ae-508">[CHANGEMENT CASSANT] Paramètre `--http-password/-p` désormais obligatoire</span><span class="sxs-lookup"><span data-stu-id="655ae-508">[BREAKING CHANGE] Made `--http-password/-p` a required parameter</span></span> 
* <span data-ttu-id="655ae-509">Ajout de compléteurs pour le compléteur des paramètres `--cluster-admin-account` et `cluster-users-group-dns`</span><span class="sxs-lookup"><span data-stu-id="655ae-509">Added completers for `--cluster-admin-account` and `cluster-users-group-dns` parameters completer</span></span> 
* <span data-ttu-id="655ae-510">Paramètre `cluster-users-group-dns` désormais obligatoire quand `—esp` est présent</span><span class="sxs-lookup"><span data-stu-id="655ae-510">Changed `cluster-users-group-dns` parameter to be required when `—esp` is present</span></span>
* <span data-ttu-id="655ae-511">Ajout d’un délai d’expiration pour tous les compléteurs automatiques d’arguments existants</span><span class="sxs-lookup"><span data-stu-id="655ae-511">Added a timeout for all existing argument auto-completers</span></span>
* <span data-ttu-id="655ae-512">Ajout d’un délai d’expiration pour la transformation d’un nom de ressource en ID de ressource</span><span class="sxs-lookup"><span data-stu-id="655ae-512">Added a timeout for transforming resource name to resource id</span></span>
* <span data-ttu-id="655ae-513">Modification des compléteurs automatiques pour sélectionner des ressources à partir de n’importe quel groupe de ressources.</span><span class="sxs-lookup"><span data-stu-id="655ae-513">Changed Auto-completers to select resources from any resource group.</span></span> <span data-ttu-id="655ae-514">Le groupe de ressources peut être différent de celui spécifié avec `-g`</span><span class="sxs-lookup"><span data-stu-id="655ae-514">It can be a different resource group than the one specified with `-g`</span></span>
* <span data-ttu-id="655ae-515">Ajout de la prise en charge des paramètres `--sub-domain-suffix` et `--disable_gateway_auth` dans la commande `hdinsight application create`</span><span class="sxs-lookup"><span data-stu-id="655ae-515">Added support for `--sub-domain-suffix` and `--disable_gateway_auth` parameters in the `hdinsight application create` command</span></span>

### <a name="managed-services"></a><span data-ttu-id="655ae-516">Services gérés</span><span class="sxs-lookup"><span data-stu-id="655ae-516">Managed Services</span></span>

* <span data-ttu-id="655ae-517">Introduction du module de commande des services gérés en préversion</span><span class="sxs-lookup"><span data-stu-id="655ae-517">Introducing managed service command module in preview</span></span>

### <a name="profile"></a><span data-ttu-id="655ae-518">Profil</span><span class="sxs-lookup"><span data-stu-id="655ae-518">Profile</span></span>
* <span data-ttu-id="655ae-519">Suppression de l’argument `--subscription` pour la commande de déconnexion</span><span class="sxs-lookup"><span data-stu-id="655ae-519">Suppress `--subscription` argument for logout command</span></span>

### <a name="rbac"></a><span data-ttu-id="655ae-520">RBAC</span><span class="sxs-lookup"><span data-stu-id="655ae-520">RBAC</span></span>

* <span data-ttu-id="655ae-521">[CHANGEMENT CASSANT] Suppression de l’argument `--password` pour `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="655ae-521">[BREAKING CHANGE] Removed `--password` argument for `create-for-rbac`</span></span>
* <span data-ttu-id="655ae-522">Ajout du paramètre `--assignee-principal-type` à la commande `create` pour éviter les défaillances intermittentes dues à la latence de réplication du serveur de graphique AAD</span><span class="sxs-lookup"><span data-stu-id="655ae-522">Added `--assignee-principal-type` parameter to `create` command to avoid intermittent failures caused by AAD graph server replication latency</span></span>
* <span data-ttu-id="655ae-523">Correction d’un incident dans `ad signed-in-user` lors de l’énumération des objets détenus</span><span class="sxs-lookup"><span data-stu-id="655ae-523">Fixed a crash in `ad signed-in-user` when listing owned objects</span></span>
* <span data-ttu-id="655ae-524">Correction d’un incident lié au fait que `ad sp` ne trouve pas la bonne application à partir d’un principal de service</span><span class="sxs-lookup"><span data-stu-id="655ae-524">Fixed issue where `ad sp` would not find the right application from a service principal</span></span>

### <a name="rdbms"></a><span data-ttu-id="655ae-525">SGBDR</span><span class="sxs-lookup"><span data-stu-id="655ae-525">RDBMS</span></span>

* <span data-ttu-id="655ae-526">Ajout de la prise en charge de la réplication pour MariaDB</span><span class="sxs-lookup"><span data-stu-id="655ae-526">Added support for replication for MariaDB</span></span>

### <a name="sql"></a><span data-ttu-id="655ae-527">SQL</span><span class="sxs-lookup"><span data-stu-id="655ae-527">SQL</span></span>

* <span data-ttu-id="655ae-528">Valeurs autorisées documentées pour `sql db create --sample-name`</span><span class="sxs-lookup"><span data-stu-id="655ae-528">Documented allowed values for `sql db create --sample-name`</span></span>

### <a name="storage"></a><span data-ttu-id="655ae-529">Stockage</span><span class="sxs-lookup"><span data-stu-id="655ae-529">Storage</span></span>

* <span data-ttu-id="655ae-530">Ajout de la prise en charge des jetons SAS de délégation d’utilisateur avec `--as-user` à `storage blob generate-sas`</span><span class="sxs-lookup"><span data-stu-id="655ae-530">Added user delegation SAS token support with `--as-user` to `storage blob generate-sas`</span></span> 
* <span data-ttu-id="655ae-531">Ajout de la prise en charge des jetons SAS de délégation d’utilisateur avec `--as-user` à `storage container generate-sas`</span><span class="sxs-lookup"><span data-stu-id="655ae-531">Added user delegation SAS token support with `--as-user` to `storage container generate-sas`</span></span> 

### <a name="vm"></a><span data-ttu-id="655ae-532">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="655ae-532">VM</span></span>

* <span data-ttu-id="655ae-533">Correction d’un bogue contraignant `vmss create` à retourner un message d’erreur en cas d’exécution avec `--no-wait`</span><span class="sxs-lookup"><span data-stu-id="655ae-533">Fixed bug where `vmss create` returns an error message when run with `--no-wait`</span></span>
* <span data-ttu-id="655ae-534">Suppression de la validation côté client pour `vmss create --single-placement-group`.</span><span class="sxs-lookup"><span data-stu-id="655ae-534">Removed client-side validation for `vmss create --single-placement-group`.</span></span> <span data-ttu-id="655ae-535">N’échoue pas si `--single-placement-group` a la valeur `true` et si `--instance-count` est supérieur à 100 ou si des zones de disponibilité sont spécifiées, mais laisse cette validation au service de calcul</span><span class="sxs-lookup"><span data-stu-id="655ae-535">Does not fail if `--single-placement-group` is set to `true` and`--instance-count` is greater than 100 or availability zones are specified, but leaves this validation to the compute service</span></span>
* <span data-ttu-id="655ae-536">Correction d’un bogue entraînant l’échec de `[vm|vmss] extension image list` en cas d’utilisation avec `--latest`</span><span class="sxs-lookup"><span data-stu-id="655ae-536">Fixed bug where `[vm|vmss] extension image list` fails when used with `--latest`</span></span>


## <a name="june-18-2019"></a><span data-ttu-id="655ae-537">18 juin 2019</span><span class="sxs-lookup"><span data-stu-id="655ae-537">June 18, 2019</span></span>

<span data-ttu-id="655ae-538">Version 2.0.67</span><span class="sxs-lookup"><span data-stu-id="655ae-538">Version 2.0.67</span></span>

### <a name="core"></a><span data-ttu-id="655ae-539">Core</span><span class="sxs-lookup"><span data-stu-id="655ae-539">Core</span></span>

<span data-ttu-id="655ae-540">Cette version introduit une nouvelle étiquette [Préversion] qui permet d’indiquer plus clairement aux clients la présence d’un groupe de commandes, d’une commande ou d’un argument en préversion.</span><span class="sxs-lookup"><span data-stu-id="655ae-540">This release introduces a new [Preview] tag to more clearly communicate to customers when a command group, command or argument is in preview status.</span></span> <span data-ttu-id="655ae-541">Auparavant, cet état était mentionné dans le texte de l’aide ou communiqué implicitement par le numéro de version du module de commande.</span><span class="sxs-lookup"><span data-stu-id="655ae-541">This was previously called out in help text or communicated implicitly by the command module version number.</span></span>
<span data-ttu-id="655ae-542">À l’avenir, l’interface CLI supprimera les numéros de version des packages individuels.</span><span class="sxs-lookup"><span data-stu-id="655ae-542">The CLI will be removing version numbers for individual packages in the future.</span></span> <span data-ttu-id="655ae-543">Si une commande est en préversion, tous ses arguments le sont également.</span><span class="sxs-lookup"><span data-stu-id="655ae-543">If a command is in preview, all of its arguments are as well.</span></span> <span data-ttu-id="655ae-544">Si un groupe de commandes est étiqueté comme étant en préversion, toutes les commandes et tous les arguments sont également considérés comme étant en préversion.</span><span class="sxs-lookup"><span data-stu-id="655ae-544">If a command group is labeled as being in preview, then all commands and arguments are considered to be in preview as well.</span></span>

<span data-ttu-id="655ae-545">Conséquence de ce changement, plusieurs groupes de commandes peuvent « soudainement » apparaître comme étant en préversion avec cette version.</span><span class="sxs-lookup"><span data-stu-id="655ae-545">As a result of this change, several command groups may seem to "suddenly" appear to be in a preview status with this release.</span></span> <span data-ttu-id="655ae-546">En fait, la plupart des packages étaient en préversion, mais ils sont considérés comme étant dans un état de disponibilité générale avec cette version.</span><span class="sxs-lookup"><span data-stu-id="655ae-546">What actually happened is that most packages were in a preview status, but are being deemed GA with this release</span></span>

### <a name="acr"></a><span data-ttu-id="655ae-547">ACR</span><span class="sxs-lookup"><span data-stu-id="655ae-547">ACR</span></span>
* <span data-ttu-id="655ae-548">Ajout de la commande « acr check-health »</span><span class="sxs-lookup"><span data-stu-id="655ae-548">Added 'acr check-health' command</span></span>
* <span data-ttu-id="655ae-549">Amélioration de la gestion des erreurs pour les jetons AAD et pour la récupération des commandes externes</span><span class="sxs-lookup"><span data-stu-id="655ae-549">Improved error handling for AAD tokens and for retrieving external commands</span></span>

### <a name="acs"></a><span data-ttu-id="655ae-550">ACS</span><span class="sxs-lookup"><span data-stu-id="655ae-550">ACS</span></span>
* <span data-ttu-id="655ae-551">Les commandes ACS dépréciées sont désormais masquées de l’affichage de l’aide</span><span class="sxs-lookup"><span data-stu-id="655ae-551">Deprecated ACS commands are now hidden from help view</span></span>

### <a name="ams"></a><span data-ttu-id="655ae-552">AMS</span><span class="sxs-lookup"><span data-stu-id="655ae-552">AMS</span></span>
* <span data-ttu-id="655ae-553">[CHANGEMENT CASSANT] Changement apporté pour retourner les chaînes de temps ISO 8601 pour archive-window-length et key-frame-interval-duration</span><span class="sxs-lookup"><span data-stu-id="655ae-553">[BREAKING CHANGE] Changed to return ISO 8601 time strings for archive-window-length and key-frame-interval-duration</span></span>

### <a name="appservice"></a><span data-ttu-id="655ae-554">AppService</span><span class="sxs-lookup"><span data-stu-id="655ae-554">AppService</span></span>
* <span data-ttu-id="655ae-555">Ajout du routage basé sur l’emplacement pour `webapp deleted list` et `webapp deleted restore`</span><span class="sxs-lookup"><span data-stu-id="655ae-555">Added location based routing for `webapp deleted list` and `webapp deleted restore`</span></span>
* <span data-ttu-id="655ae-556">Correction d’un problème lié à l’impossibilité de cliquer sur l’URL cible journalisée d’une application web (« Vous pouvez lancer l’application... ») dans Azure Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="655ae-556">Fixed issue where webapp up logged target URL ("You can launch the app at...") was not clickable in Azure Cloud Shell</span></span>
* <span data-ttu-id="655ae-557">Correction d’un problème entraînant l’échec de la création d’applications avec certaines références SKU (erreur AlwaysOn)</span><span class="sxs-lookup"><span data-stu-id="655ae-557">Fixed an issue where creating apps with the some SKUs was failing with an AlwaysOn error</span></span>
* <span data-ttu-id="655ae-558">Ajout d’une fonction de prévalidation à `[appservice|webapp] create`</span><span class="sxs-lookup"><span data-stu-id="655ae-558">Added pre-validation to `[appservice|webapp] create`</span></span>
* <span data-ttu-id="655ae-559">Correction de `[webapp|functionapp] traffic-routing` de manière à utiliser le bon actionHostName</span><span class="sxs-lookup"><span data-stu-id="655ae-559">Fixed `[webapp|functionapp] traffic-routing` to use the correct actionHostName</span></span>
* <span data-ttu-id="655ae-560">Ajout de la prise en charge de l’emplacement aux commandes `functionapp`</span><span class="sxs-lookup"><span data-stu-id="655ae-560">Added slot support to `functionapp` commands</span></span>

### <a name="batch"></a><span data-ttu-id="655ae-561">Batch</span><span class="sxs-lookup"><span data-stu-id="655ae-561">Batch</span></span>
* <span data-ttu-id="655ae-562">Correction de la régression d’authentification AAD provoquée par un rapport d’erreur trop agressif pour l’authentification par clé partagée</span><span class="sxs-lookup"><span data-stu-id="655ae-562">Fixed AAD auth regression caused by over-aggressive error reporting for Shared Key Auth</span></span>

### <a name="batchai"></a><span data-ttu-id="655ae-563">Batch AI</span><span class="sxs-lookup"><span data-stu-id="655ae-563">BatchAI</span></span>
* <span data-ttu-id="655ae-564">Les commandes BatchAI sont maintenant dépréciées et masquées</span><span class="sxs-lookup"><span data-stu-id="655ae-564">BatchAI commands are now deprecated and hidden</span></span>

### <a name="botservice"></a><span data-ttu-id="655ae-565">BotService</span><span class="sxs-lookup"><span data-stu-id="655ae-565">BotService</span></span>
* <span data-ttu-id="655ae-566">Ajout de messages d’avertissement « support interrompu »/« mode maintenance » pour les commandes prenant en charge le SDK v3</span><span class="sxs-lookup"><span data-stu-id="655ae-566">Added "discontinued support"/"maintenance mode" warning messages for commands that support the v3 SDK</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="655ae-567">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="655ae-567">CosmosDB</span></span>
* <span data-ttu-id="655ae-568">[DÉPRÉCIATION] Dépréciation de la commande `cosmosdb list-keys`</span><span class="sxs-lookup"><span data-stu-id="655ae-568">[DEPRECATED] Deprecated the `cosmosdb list-keys` command</span></span>
* <span data-ttu-id="655ae-569">Ajout de la commande `cosmosdb keys list` (remplace `cosmosdb list-keys`)</span><span class="sxs-lookup"><span data-stu-id="655ae-569">Added the `cosmosdb keys list` command - replaces `cosmosdb list-keys`</span></span>
* <span data-ttu-id="655ae-570">`cosmsodb create/update`: Ajout d’un nouveau format pour --location afin d’autoriser la définition de la propriété « isZoneRedundant ».</span><span class="sxs-lookup"><span data-stu-id="655ae-570">`cosmsodb create/update`: Added new format for --location to allow setting "isZoneRedundant" property.</span></span> <span data-ttu-id="655ae-571">Ancien format déprécié</span><span class="sxs-lookup"><span data-stu-id="655ae-571">Deprecated old format</span></span>

### <a name="eventgrid"></a><span data-ttu-id="655ae-572">EventGrid</span><span class="sxs-lookup"><span data-stu-id="655ae-572">EventGrid</span></span>
* <span data-ttu-id="655ae-573">Ajout de commandes `eventgrid domain` pour les opérations CRUD liées aux domaines</span><span class="sxs-lookup"><span data-stu-id="655ae-573">Added `eventgrid domain` commands for domain CRUD operations</span></span>
* <span data-ttu-id="655ae-574">Ajout de commandes `eventgrid domain topic` pour les opérations CRUD liées aux rubriques de domaine</span><span class="sxs-lookup"><span data-stu-id="655ae-574">Added `eventgrid domain topic` commands for domain topics CRUD operations</span></span>
* <span data-ttu-id="655ae-575">Ajout de l’argument `--odata-query` à `eventgrid [topic|event-subscription] list` pour filtrer les résultats à l’aide de la syntaxe OData</span><span class="sxs-lookup"><span data-stu-id="655ae-575">Added `--odata-query` argument to `eventgrid [topic|event-subscription] list` for filtering results using OData syntax</span></span>
* <span data-ttu-id="655ae-576">`event-subscription create/update`: Ajout de servicebusqueue comme nouvelle valeur pour le paramètre `--endpoint-type`</span><span class="sxs-lookup"><span data-stu-id="655ae-576">`event-subscription create/update`: Added servicebusqueue as new values for the `--endpoint-type` parameter</span></span>
* <span data-ttu-id="655ae-577">[CHANGEMENT CASSANT] Suppression de la prise en charge de `--included-event-types All` avec `eventgrid event-subscription [create|update]`</span><span class="sxs-lookup"><span data-stu-id="655ae-577">[BREAKING CHANGE] Removed support for `--included-event-types All` with `eventgrid event-subscription [create|update]`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="655ae-578">HDInsight</span><span class="sxs-lookup"><span data-stu-id="655ae-578">HDInsight</span></span>
* <span data-ttu-id="655ae-579">Ajout de la prise en charge du paramètre `--ssh-public-key` dans la commande `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="655ae-579">Added support for `--ssh-public-key` parameter in `hdinsight create` command</span></span>

### <a name="iot"></a><span data-ttu-id="655ae-580">IoT</span><span class="sxs-lookup"><span data-stu-id="655ae-580">IoT</span></span>
* <span data-ttu-id="655ae-581">Ajout de la prise en charge pour régénérer les clés de stratégie d’autorisation</span><span class="sxs-lookup"><span data-stu-id="655ae-581">Added support to regenerate authorization policy keys</span></span>
* <span data-ttu-id="655ae-582">Ajout du SDK et de la prise en charge du service de provisionnement de dépôt DigitalTwin</span><span class="sxs-lookup"><span data-stu-id="655ae-582">Added SDK and support for DigitalTwin Repository Provisioning Service</span></span>

### <a name="network"></a><span data-ttu-id="655ae-583">Réseau</span><span class="sxs-lookup"><span data-stu-id="655ae-583">Network</span></span>
* <span data-ttu-id="655ae-584">Ajout de la prise en charge de la zone pour NAT Gateway</span><span class="sxs-lookup"><span data-stu-id="655ae-584">Added Zone support for Nat Gateway</span></span>
* <span data-ttu-id="655ae-585">Ajout de la commande `network list-service-tags`</span><span class="sxs-lookup"><span data-stu-id="655ae-585">Added command `network list-service-tags`</span></span>
* <span data-ttu-id="655ae-586">Correction d’un problème avec `dns zone import` empêchant les utilisateurs d’importer les enregistrements A génériques</span><span class="sxs-lookup"><span data-stu-id="655ae-586">Fixed issue with `dns zone import` where users could not import wildcard A records</span></span>
* <span data-ttu-id="655ae-587">Correction d’un problème avec `watcher flow-log configure` empêchant l’activation de la journalisation de flux dans certaines régions</span><span class="sxs-lookup"><span data-stu-id="655ae-587">Fixed issue with `watcher flow-log configure` where flow logging could not be enabled in certain regions</span></span>

### <a name="resource"></a><span data-ttu-id="655ae-588">Ressource</span><span class="sxs-lookup"><span data-stu-id="655ae-588">Resource</span></span>
* <span data-ttu-id="655ae-589">Ajout de la commande `az rest` pour passer des appels REST</span><span class="sxs-lookup"><span data-stu-id="655ae-589">Added `az rest` command for making REST calls</span></span>
* <span data-ttu-id="655ae-590">Correction d’une erreur liée à l’utilisation de `policy assignment list` avec un groupe de ressources ou un niveau d’abonnement `--scope`</span><span class="sxs-lookup"><span data-stu-id="655ae-590">Fixed error when using `policy assignment list` with a resource group or subscription level `--scope`</span></span>

### <a name="servicebus"></a><span data-ttu-id="655ae-591">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="655ae-591">ServiceBus</span></span>
* <span data-ttu-id="655ae-592">Correction d’une erreur liée à `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span><span class="sxs-lookup"><span data-stu-id="655ae-592">Fixed issue with `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span></span>

### <a name="sql"></a><span data-ttu-id="655ae-593">SQL</span><span class="sxs-lookup"><span data-stu-id="655ae-593">SQL</span></span>
* <span data-ttu-id="655ae-594">Modification apportée à `--location` pour le rendre facultatif pour `sql [server|mi] create` : utilise l’emplacement du groupe de ressources s’il n’est pas spécifié</span><span class="sxs-lookup"><span data-stu-id="655ae-594">Changed `--location` to be optional for `sql [server|mi] create` - uses resource group location if not specified</span></span>
* <span data-ttu-id="655ae-595">Correction de l’erreur « L’objet 'NoneType' n’est pas itérable » pour `sql db list-editions --available`</span><span class="sxs-lookup"><span data-stu-id="655ae-595">Fixed "'NoneType' object is not iterable" error for `sql db list-editions --available`</span></span>

### <a name="sqlvm"></a><span data-ttu-id="655ae-596">SQLVm</span><span class="sxs-lookup"><span data-stu-id="655ae-596">SQLVm</span></span>
* <span data-ttu-id="655ae-597">[CHANGEMENT CASSANT] Modification de `sql vm create` pour exiger le paramètre `--license-type`</span><span class="sxs-lookup"><span data-stu-id="655ae-597">[BREAKING CHNAGE] Changed `sql vm create` to require `--license-type` parameter</span></span>
* <span data-ttu-id="655ae-598">Modification apportée pour autoriser la définition d’une référence SKU d’image SQL lors de la création ou de la mise à jour d’une machine virtuelle SQL</span><span class="sxs-lookup"><span data-stu-id="655ae-598">Changed to allow setting SQL image SKU when creating or updating a sql vm</span></span>

### <a name="storage"></a><span data-ttu-id="655ae-599">Stockage</span><span class="sxs-lookup"><span data-stu-id="655ae-599">Storage</span></span>
* <span data-ttu-id="655ae-600">Correction d’un problème lié à une clé de compte manquante pour `storage container generate-sas`</span><span class="sxs-lookup"><span data-stu-id="655ae-600">Fixed issue with missing account key for `storage container generate-sas`</span></span>
* <span data-ttu-id="655ae-601">Correction d’un problème lié à `storage blob sync` sur Linux</span><span class="sxs-lookup"><span data-stu-id="655ae-601">Fixed issue with `storage blob sync` on Linux</span></span>

### <a name="vm"></a><span data-ttu-id="655ae-602">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="655ae-602">VM</span></span>
* <span data-ttu-id="655ae-603">[PRÉVERSION] Ajout de commandes `vm image template` pour générer des images de machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="655ae-603">[PREVIEW] Added `vm image template` commands to build VM images</span></span>

## <a name="june-4-2019"></a><span data-ttu-id="655ae-604">4 juin 2019</span><span class="sxs-lookup"><span data-stu-id="655ae-604">June 4, 2019</span></span>

<span data-ttu-id="655ae-605">Version 2.0.66</span><span class="sxs-lookup"><span data-stu-id="655ae-605">Version 2.0.66</span></span>

### <a name="core"></a><span data-ttu-id="655ae-606">Core</span><span class="sxs-lookup"><span data-stu-id="655ae-606">Core</span></span>
* <span data-ttu-id="655ae-607">Correction du bogue où des commandes échouent si `--output yaml` est utilisé avec `--query`</span><span class="sxs-lookup"><span data-stu-id="655ae-607">Fixed bug where commands fail if `--output yaml` is used with `--query`</span></span>

### <a name="acr"></a><span data-ttu-id="655ae-608">ACR</span><span class="sxs-lookup"><span data-stu-id="655ae-608">ACR</span></span>
* <span data-ttu-id="655ae-609">Ajout du groupe de commandes « acr pack » pour la création de tâches de génération rapide à l’aide de Buildpacks.</span><span class="sxs-lookup"><span data-stu-id="655ae-609">Added 'acr pack' command group for creating quick build Tasks using Buildpacks.</span></span>

### <a name="acs"></a><span data-ttu-id="655ae-610">ACS</span><span class="sxs-lookup"><span data-stu-id="655ae-610">ACS</span></span>
* <span data-ttu-id="655ae-611">Autoriser l’activation/la désactivation du module complémentaire kube-dashboard AKS</span><span class="sxs-lookup"><span data-stu-id="655ae-611">Allow enabling/disabling AKS kube-dashboard addon</span></span>
* <span data-ttu-id="655ae-612">Afficher un message convivial lorsque l’abonnement n’est pas autorisé à utiliser Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="655ae-612">Print a friendly message when the subscription is not whitelisted to use Azure Red Hat OpenShift</span></span>

### <a name="batch"></a><span data-ttu-id="655ae-613">Batch</span><span class="sxs-lookup"><span data-stu-id="655ae-613">Batch</span></span>
* <span data-ttu-id="655ae-614">Amélioration de la gestion des erreurs en l’absence de connexion à un compte \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span><span class="sxs-lookup"><span data-stu-id="655ae-614">Improved error handling when not logged in to an account \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span></span>

### <a name="iot"></a><span data-ttu-id="655ae-615">IoT</span><span class="sxs-lookup"><span data-stu-id="655ae-615">IoT</span></span>
* <span data-ttu-id="655ae-616">Ajout de la prise en charge du basculement manuel</span><span class="sxs-lookup"><span data-stu-id="655ae-616">Added support for manual failover</span></span>

### <a name="network"></a><span data-ttu-id="655ae-617">Réseau</span><span class="sxs-lookup"><span data-stu-id="655ae-617">Network</span></span>
* <span data-ttu-id="655ae-618">Ajout de commandes `network application-gateway waf-policy` pour prendre en charge des règles de pare-feu d’applications web personnalisées.</span><span class="sxs-lookup"><span data-stu-id="655ae-618">Added `network application-gateway waf-policy` commands to support custom WAF rules.</span></span>
* <span data-ttu-id="655ae-619">Ajout des arguments `--waf-policy` et `--max-capacity` à `network application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="655ae-619">Added `--waf-policy` and `--max-capacity` arguments to `network application-gateway [create|update]`</span></span> 

### <a name="resource"></a><span data-ttu-id="655ae-620">Ressource</span><span class="sxs-lookup"><span data-stu-id="655ae-620">Resource</span></span>
* <span data-ttu-id="655ae-621">Amélioration du message d’erreur émis par la commande `deployment create` quand aucun appareil TTY n’est disponible</span><span class="sxs-lookup"><span data-stu-id="655ae-621">Improved error message from `deployment create` when there is no TTY available</span></span>

### <a name="role"></a><span data-ttu-id="655ae-622">Role</span><span class="sxs-lookup"><span data-stu-id="655ae-622">Role</span></span>
* <span data-ttu-id="655ae-623">Mise à jour du texte d’aide</span><span class="sxs-lookup"><span data-stu-id="655ae-623">Updated help text.</span></span>

### <a name="compute"></a><span data-ttu-id="655ae-624">Calcul</span><span class="sxs-lookup"><span data-stu-id="655ae-624">Compute</span></span>
* <span data-ttu-id="655ae-625">Ajout de la prise en charge dans `vm create` des machines virtuelles à partir d’une image managée avec des LUN de disque de données qui ne démarrent pas de 0 ou qui ignorent des nombres</span><span class="sxs-lookup"><span data-stu-id="655ae-625">Added support to `vm create` for VMs from a managed image with data-disk luns that do not start from 0 or that skip numbers</span></span>

## <a name="may-21-2019"></a><span data-ttu-id="655ae-626">21 mai 2019</span><span class="sxs-lookup"><span data-stu-id="655ae-626">May 21, 2019</span></span>

<span data-ttu-id="655ae-627">Version 2.0.65</span><span class="sxs-lookup"><span data-stu-id="655ae-627">Version 2.0.65</span></span>

### <a name="core"></a><span data-ttu-id="655ae-628">Core</span><span class="sxs-lookup"><span data-stu-id="655ae-628">Core</span></span>
* <span data-ttu-id="655ae-629">Ajout de meilleurs commentaires pour les erreurs d’authentification</span><span class="sxs-lookup"><span data-stu-id="655ae-629">Added better feedback for authentication errors</span></span>
* <span data-ttu-id="655ae-630">Correction d’un problème où l’interface CLI chargeait des extensions qui n’étaient pas compatibles avec sa version principale</span><span class="sxs-lookup"><span data-stu-id="655ae-630">Fixed issue where the CLI would load extensions that were not compatible with its core version</span></span>
* <span data-ttu-id="655ae-631">Correction d’un problème lié au lancement lorsque `clouds.config` est endommagé</span><span class="sxs-lookup"><span data-stu-id="655ae-631">Fixed issue with launching when `clouds.config` is corrupted</span></span>

### <a name="acr"></a><span data-ttu-id="655ae-632">ACR</span><span class="sxs-lookup"><span data-stu-id="655ae-632">ACR</span></span>
* <span data-ttu-id="655ae-633">Ajout de la prise en charge des identités managées aux tâches</span><span class="sxs-lookup"><span data-stu-id="655ae-633">Added support for Managed Identities to Tasks</span></span>

### <a name="acs"></a><span data-ttu-id="655ae-634">ACS</span><span class="sxs-lookup"><span data-stu-id="655ae-634">ACS</span></span>
* <span data-ttu-id="655ae-635">Correction de la commande `openshift create` lorsqu’elle est utilisée avec le client AAD du client</span><span class="sxs-lookup"><span data-stu-id="655ae-635">Fixed `openshift create` command when used with customer AAD client</span></span>

### <a name="appservice"></a><span data-ttu-id="655ae-636">AppService</span><span class="sxs-lookup"><span data-stu-id="655ae-636">AppService</span></span>
* <span data-ttu-id="655ae-637">[DÉPRÉCIATION] Commande `functionapp devops-build` dépréciée (Elle sera supprimée de la prochaine version)</span><span class="sxs-lookup"><span data-stu-id="655ae-637">[DEPRECATED] Deprecated `functionapp devops-build` command - will be removed in next release</span></span>
* <span data-ttu-id="655ae-638">Changement apporté à `functionapp devops-pipeline` pour extraire un journal de génération d’Azure DevOps en mode détaillé</span><span class="sxs-lookup"><span data-stu-id="655ae-638">Changed `functionapp devops-pipeline` to fetch build log from Azure DevOps in verbose mode</span></span>
* <span data-ttu-id="655ae-639">[CHANGEMENT CASSANT] Suppression de l’indicateur `--use_local_settings` de la commande `functionapp devops-pipeline` (aucune opération)</span><span class="sxs-lookup"><span data-stu-id="655ae-639">[BREAKING CHANGE] Removed `--use_local_settings` flag from `functionapp devops-pipeline` command - was a no-op</span></span>
* <span data-ttu-id="655ae-640">Changement apporté à `webapp up` pour retourner une sortie JSON si `--logs` n’est pas utilisé</span><span class="sxs-lookup"><span data-stu-id="655ae-640">Changed `webapp up` to return JSON output if `--logs` is not used</span></span>
* <span data-ttu-id="655ae-641">Ajout de la prise en charge de l’écriture de ressources par défaut à la configuration locale pour `webapp up`</span><span class="sxs-lookup"><span data-stu-id="655ae-641">Added support for writing default resources to local config for `webapp up`</span></span>
* <span data-ttu-id="655ae-642">Ajout de la prise en charge à `webapp up` pour redéployer une application sans utiliser l’argument `--location`</span><span class="sxs-lookup"><span data-stu-id="655ae-642">Added support to `webapp up` for redeploying an app without using the `--location` argument</span></span>
* <span data-ttu-id="655ae-643">Résolution d’un problème où, lors de la création ASP de la référence SKU Gratuite, la valeur de référence Gratuit ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="655ae-643">Fixed an issue where for Linux Free SKU ASP creation use Free as SKU value was not working</span></span>

### <a name="botservice"></a><span data-ttu-id="655ae-644">BotService</span><span class="sxs-lookup"><span data-stu-id="655ae-644">BotService</span></span>
* <span data-ttu-id="655ae-645">Modification autorisant toutes les casses pour les paramètres `--lang` des commandes</span><span class="sxs-lookup"><span data-stu-id="655ae-645">Changed to allow all casing for `--lang` parameters for commands</span></span>
* <span data-ttu-id="655ae-646">Mise à jour de la description du module de commande</span><span class="sxs-lookup"><span data-stu-id="655ae-646">Updated description for command module</span></span>

### <a name="consumption"></a><span data-ttu-id="655ae-647">Consommation</span><span class="sxs-lookup"><span data-stu-id="655ae-647">Consumption</span></span>
* <span data-ttu-id="655ae-648">Ajout du paramètre obligatoire manquant lors de l’exécution de `consumption usage list --billing-period-name`</span><span class="sxs-lookup"><span data-stu-id="655ae-648">Added missing required parameter when running `consumption usage list --billing-period-name`</span></span>

### <a name="iot"></a><span data-ttu-id="655ae-649">IoT</span><span class="sxs-lookup"><span data-stu-id="655ae-649">IoT</span></span>
* <span data-ttu-id="655ae-650">Ajout de la prise en charge permettant de répertorier toutes les clés</span><span class="sxs-lookup"><span data-stu-id="655ae-650">Added support to list all keys</span></span>

### <a name="network"></a><span data-ttu-id="655ae-651">Réseau</span><span class="sxs-lookup"><span data-stu-id="655ae-651">Network</span></span>
* [CHANGEMENT CASSANT]: Removed `network interface-endpoints` command group - use `network private-endpoints`
[BREAKING CHANGE]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* <span data-ttu-id="655ae-653">Ajout de l’argument `--nat-gateway` à `network vnet subnet [create|update]` pour attacher à une passerelle NAT</span><span class="sxs-lookup"><span data-stu-id="655ae-653">Added `--nat-gateway` argument to `network vnet subnet [create|update]` for attaching to a NAT gateway</span></span>
* <span data-ttu-id="655ae-654">Correction d’un problème avec `dns zone import` où les noms d’enregistrement pouvaient ne pas correspondre à un type d’enregistrement</span><span class="sxs-lookup"><span data-stu-id="655ae-654">Fixed issue with `dns zone import` where record names could not match a record type</span></span>

### <a name="rdbms"></a><span data-ttu-id="655ae-655">SGBDR</span><span class="sxs-lookup"><span data-stu-id="655ae-655">RDBMS</span></span>
* <span data-ttu-id="655ae-656">Ajout de la prise en charge de MySQL et Postgres pour la géoréplication</span><span class="sxs-lookup"><span data-stu-id="655ae-656">Added postgres and mysql support for geo replication</span></span>

### <a name="rbac"></a><span data-ttu-id="655ae-657">RBAC</span><span class="sxs-lookup"><span data-stu-id="655ae-657">RBAC</span></span>
* <span data-ttu-id="655ae-658">Ajout de la prise en charge de l’étendue du groupe de gestion dans `role assignment`</span><span class="sxs-lookup"><span data-stu-id="655ae-658">Added support for management group scope to `role assignment`</span></span>

### <a name="storage"></a><span data-ttu-id="655ae-659">Stockage</span><span class="sxs-lookup"><span data-stu-id="655ae-659">Storage</span></span>
* <span data-ttu-id="655ae-660">`storage blob sync` : ajout de la commande de synchronisation pour le blob de stockage</span><span class="sxs-lookup"><span data-stu-id="655ae-660">`storage blob sync`: add sync command for storage blob</span></span>

### <a name="compute"></a><span data-ttu-id="655ae-661">Calcul</span><span class="sxs-lookup"><span data-stu-id="655ae-661">Compute</span></span>
* <span data-ttu-id="655ae-662">Ajout de `--computer-name` à `vm create` pour définir le nom d’une machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="655ae-662">Added `--computer-name` to `vm create` for setting a VM's computer name</span></span>
* <span data-ttu-id="655ae-663">`--ssh-key-value` renommé en `--ssh-key-values` pour `[vm|vmss] create` - peut maintenant accepter plusieurs chemins d’accès ou valeurs de clé publique SSH</span><span class="sxs-lookup"><span data-stu-id="655ae-663">Renamed `--ssh-key-value` renamed to `--ssh-key-values` for `[vm|vmss] create` - can now accept multiple ssh public key values or paths</span></span>
  * <span data-ttu-id="655ae-664">__Remarque__: il ne s’agit **pas** d’un changement cassant - `--ssh-key-value` sera analysé correctement, car il correspond uniquement à `--ssh-key-values`</span><span class="sxs-lookup"><span data-stu-id="655ae-664">__Note__: This is **not** a breaking change - `--ssh-key-value` will be parsed correctly as it matches only `--ssh-key-values`</span></span>
* <span data-ttu-id="655ae-665">Modification de l’argument `--type` qui devient facultatif dans `ppg create`</span><span class="sxs-lookup"><span data-stu-id="655ae-665">Changed the `--type` argument of `ppg create` to be optional</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="655ae-666">6 mai 2019</span><span class="sxs-lookup"><span data-stu-id="655ae-666">May 6, 2019</span></span>

<span data-ttu-id="655ae-667">Version 2.0.64</span><span class="sxs-lookup"><span data-stu-id="655ae-667">Version 2.0.64</span></span>

### <a name="acs"></a><span data-ttu-id="655ae-668">ACS</span><span class="sxs-lookup"><span data-stu-id="655ae-668">ACS</span></span>
* <span data-ttu-id="655ae-669">[CHANGEMENT CASSANT] Suppression de l’indicateur `--fqdn` sur les commandes `openshift`</span><span class="sxs-lookup"><span data-stu-id="655ae-669">[BREAKING CHANGE] Removed `--fqdn` flag on `openshift` commands</span></span>
* <span data-ttu-id="655ae-670">Modification permettant d’utiliser la version d’API en disponibilité générale d’Azure Red Hat Openshift</span><span class="sxs-lookup"><span data-stu-id="655ae-670">Changed to use Azure Red Hat Openshift GA API Version</span></span>
* <span data-ttu-id="655ae-671">Ajout de l’indicateur `customer-admin-group-id` à `openshift create`</span><span class="sxs-lookup"><span data-stu-id="655ae-671">Added `customer-admin-group-id` flag to `openshift create`</span></span>
* <span data-ttu-id="655ae-672">[Mise à la disposition générale] Suppression de `(PREVIEW)` de l’option `aks create` `--network-policy`</span><span class="sxs-lookup"><span data-stu-id="655ae-672">[GA] Removed `(PREVIEW)` from `aks create` option `--network-policy`</span></span>

### <a name="appservice"></a><span data-ttu-id="655ae-673">AppService</span><span class="sxs-lookup"><span data-stu-id="655ae-673">Appservice</span></span>
* <span data-ttu-id="655ae-674">[DÉPRÉCIATION] Commande `functionapp devops-build` dépréciée</span><span class="sxs-lookup"><span data-stu-id="655ae-674">[DEPRECATED] Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="655ae-675">Renommée `functionapp devops-pipeline`</span><span class="sxs-lookup"><span data-stu-id="655ae-675">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="655ae-676">Correction du processus d’obtention du nom d’utilisateur pour Cloud Shell qui provoquait l’échec de `webapp up`</span><span class="sxs-lookup"><span data-stu-id="655ae-676">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="655ae-677">Mise à jour de la documentation `appservice plan --sku` pour refléter les plans App Service pris en charge</span><span class="sxs-lookup"><span data-stu-id="655ae-677">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="655ae-678">Ajout d’arguments facultatifs pour le groupe et le plan de ressources à `webapp up`</span><span class="sxs-lookup"><span data-stu-id="655ae-678">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="655ae-679">Ajout de dispositifs de prise en charge à `webapp ssh` pour respecter la variable d’environnement `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`</span><span class="sxs-lookup"><span data-stu-id="655ae-679">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="655ae-680">Ajout de la prise en charge de `appserviceplan create` pour la référence SKU Linux gratuite</span><span class="sxs-lookup"><span data-stu-id="655ae-680">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="655ae-681">Mise en veille de 30 s de `webapp up` après la définition de `SCM_DO_BUILD_DURING_DEPLOYMENT=true` pour gérer le démarrage à froid de kudu</span><span class="sxs-lookup"><span data-stu-id="655ae-681">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="655ae-682">Ajout de la prise en charge du runtime `powershell` à `functionapp create` sur Windows</span><span class="sxs-lookup"><span data-stu-id="655ae-682">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="655ae-683">Ajout de la commande `create-remote-connection`</span><span class="sxs-lookup"><span data-stu-id="655ae-683">Added `create-remote-connection` command</span></span>

### <a name="batch"></a><span data-ttu-id="655ae-684">Batch</span><span class="sxs-lookup"><span data-stu-id="655ae-684">Batch</span></span>
* <span data-ttu-id="655ae-685">Correction du bogue dans le validateur pour les options `--application-package-references`</span><span class="sxs-lookup"><span data-stu-id="655ae-685">Fixed bug in validator for `--application-package-references` options</span></span>

### <a name="botservice"></a><span data-ttu-id="655ae-686">Botservice</span><span class="sxs-lookup"><span data-stu-id="655ae-686">Botservice</span></span>
* <span data-ttu-id="655ae-687">[CHANGEMENT CASSANT] Modification apportée à `bot create -v v4 -k webapp` pour créer un bot d’application web vide par défaut (autrement dit, aucun bot n’est déployé sur App Service)</span><span class="sxs-lookup"><span data-stu-id="655ae-687">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to create an empty Web App Bot by default (i.e. no bot is deployed to the App Service)</span></span>
* <span data-ttu-id="655ae-688">Ajout de l’indicateur `--echo` à `bot create` pour utiliser l’ancien comportement avec `-v v4`</span><span class="sxs-lookup"><span data-stu-id="655ae-688">Added `--echo` flag to `bot create` to use the old behavior with `-v v4`</span></span>
* <span data-ttu-id="655ae-689">[CHANGEMENT CASSANT] Modification de la valeur par défaut de `--version` qui devient `v4`</span><span class="sxs-lookup"><span data-stu-id="655ae-689">[BREAKING CHANGE] Changed the default value of  `--version` to `v4`</span></span>
  * <span data-ttu-id="655ae-690">__REMARQUE :__  `bot prepare-publish` utilise toujours l’ancienne valeur par défaut</span><span class="sxs-lookup"><span data-stu-id="655ae-690">__NOTE:__ `bot prepare-publish` still uses the its old default</span></span>
* <span data-ttu-id="655ae-691">[CHANGEMENT CASSANT] Modification de `--lang` qui n’a plus la valeur par défaut `Csharp`.</span><span class="sxs-lookup"><span data-stu-id="655ae-691">[BREAKING CHANGE] Changed `--lang` to no longer default to `Csharp`.</span></span> <span data-ttu-id="655ae-692">Si la commande nécessite `--lang` et que celui-ci n’est pas fourni, la commande génère à présent une erreur</span><span class="sxs-lookup"><span data-stu-id="655ae-692">If the command requires `--lang` and it is not provided, the command will now error out</span></span>
* <span data-ttu-id="655ae-693">[CHANGEMENT CASSANT] Modification des arguments `--appid` et `--password` de `bot create` afin que ceux-ci soient requis et puisse maintenant être créés via `ad app create`</span><span class="sxs-lookup"><span data-stu-id="655ae-693">[BREAKING CHANGE] Changed the `--appid` and `--password` args for `bot create` to be required and can now be created via `ad app create`</span></span>
* <span data-ttu-id="655ae-694">Ajout de la validation `--appid` et `--password`</span><span class="sxs-lookup"><span data-stu-id="655ae-694">Added `--appid` and `--password` validation</span></span>
* <span data-ttu-id="655ae-695">[CHANGEMENT CASSANT] Modification apportée à la commande `bot create -v v4` afin qu’elle ne crée ni n’utilise un compte de stockage ou Application Insights</span><span class="sxs-lookup"><span data-stu-id="655ae-695">[BREAKING CHANGE] Changed `bot create -v v4` to not create or use a Storage Account or Application Insights</span></span>
* <span data-ttu-id="655ae-696">[CHANGEMENT CASSANT] Modification de `bot create -v v3` pour exiger une région où Application Insights est disponible</span><span class="sxs-lookup"><span data-stu-id="655ae-696">[BREAKING CHANGE] Changed `bot create -v v3` to require a region where Application Insights is available</span></span>
* <span data-ttu-id="655ae-697">[CHANGEMENT CASSANT] Modification de `bot update` qui affecte maintenant uniquement les propriétés spécifiques d’un bot</span><span class="sxs-lookup"><span data-stu-id="655ae-697">[BREAKING CHANGE] Changed `bot update` to now affect only specific properties of a bot</span></span>
* <span data-ttu-id="655ae-698">[CHANGEMENT CASSANT] Modification des indicateurs `--lang` qui acceptent `Javascript` au lieu de `Node`</span><span class="sxs-lookup"><span data-stu-id="655ae-698">[BREAKING CHANGE] Changed `--lang` flags to accept `Javascript` instead of `Node`</span></span>
* <span data-ttu-id="655ae-699">[CHANGEMENT CASSANT] Suppression de `Node` comme valeur `--lang` autorisée</span><span class="sxs-lookup"><span data-stu-id="655ae-699">[BREAKING CHANGE] Removed `Node` as an allowed `--lang` value</span></span>
* <span data-ttu-id="655ae-700">[CHANGEMENT CASSANT] Modification de `bot create -v v4 -k webapp` afin que `SCM_DO_BUILD_DURING_DEPLOYMENT` ne soit plus défini sur True.</span><span class="sxs-lookup"><span data-stu-id="655ae-700">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to no longer set `SCM_DO_BUILD_DURING_DEPLOYMENT` to true.</span></span> <span data-ttu-id="655ae-701">Tous les déploiements via Kudu agissent conformément à leur comportement par défaut</span><span class="sxs-lookup"><span data-stu-id="655ae-701">All deployments through Kudu will act according to their default behavior</span></span>
* <span data-ttu-id="655ae-702">Modification de la commande `bot download` pour des bots sans fichiers `.bot` afin de créer le fichier de configuration spécifique à une langue avec des valeurs de paramètres d’application pour le bot</span><span class="sxs-lookup"><span data-stu-id="655ae-702">Changed `bot download` for bots without `.bot` files to create the language-specific configuration file with values from the Application Settings for the bot</span></span>
* <span data-ttu-id="655ae-703">Ajout de la prise en charge de `Typescript` pour `bot prepare-deploy`</span><span class="sxs-lookup"><span data-stu-id="655ae-703">Added `Typescript` support to `bot prepare-deploy`</span></span>
* <span data-ttu-id="655ae-704">Ajout du message d’avertissement à `bot prepare-deploy` pour les bots `Javascript` et `Typescript` quand `--code-dir` ne contient pas `package.json`</span><span class="sxs-lookup"><span data-stu-id="655ae-704">Added warning message to `bot prepare-deploy` for `Javascript` and `Typescript` bots for when `--code-dir` does not contain `package.json`</span></span>
* <span data-ttu-id="655ae-705">Modification de `bot prepare-deploy` qui retourne `true` en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="655ae-705">Changed `bot prepare-deploy` to return `true` if successful</span></span>
* <span data-ttu-id="655ae-706">Ajout de la journalisation commentée à `bot prepare-deploy`</span><span class="sxs-lookup"><span data-stu-id="655ae-706">Added verbose logging to `bot prepare-deploy`</span></span>
* <span data-ttu-id="655ae-707">Ajout d’un plus grand nombre de régions Application Insights disponibles dans `az bot create -v v3`</span><span class="sxs-lookup"><span data-stu-id="655ae-707">Added more available Application Insights regions to `az bot create -v v3`</span></span>

### <a name="configure"></a><span data-ttu-id="655ae-708">Configuration</span><span class="sxs-lookup"><span data-stu-id="655ae-708">Configure</span></span>
* <span data-ttu-id="655ae-709">Ajout de la prise en charge des configurations de valeur par défaut d’argument en fonction d’un dossier</span><span class="sxs-lookup"><span data-stu-id="655ae-709">Added support for folder based argument default value configurations</span></span>

### <a name="eventhubs"></a><span data-ttu-id="655ae-710">Eventhubs</span><span class="sxs-lookup"><span data-stu-id="655ae-710">Eventhubs</span></span>
* <span data-ttu-id="655ae-711">Ajout des commandes `namespace network-rule`</span><span class="sxs-lookup"><span data-stu-id="655ae-711">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="655ae-712">Ajout de l’argument `--default-action` pour les règles réseau à `namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="655ae-712">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="655ae-713">Réseau</span><span class="sxs-lookup"><span data-stu-id="655ae-713">Network</span></span>
* <span data-ttu-id="655ae-714">[CHANGEMENT CASSANT] Remplacement de l’argument `--cache` par `--defer` pour `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="655ae-714">[BREAKING CHANGE] Replaced `--cache` arugment with `--defer` for `vnet [create|update]`</span></span> 

### <a name="policy-insights"></a><span data-ttu-id="655ae-715">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="655ae-715">Policy Insights</span></span>
* <span data-ttu-id="655ae-716">Ajout de la prise en charge pour `--expand PolicyEvaluationDetails` pour interroger les détails de l’évaluation de stratégie sur la ressource</span><span class="sxs-lookup"><span data-stu-id="655ae-716">Added support for `--expand PolicyEvaluationDetails` to query policy evaluation details on the resource</span></span>

### <a name="role"></a><span data-ttu-id="655ae-717">Role</span><span class="sxs-lookup"><span data-stu-id="655ae-717">Role</span></span>
* <span data-ttu-id="655ae-718">[DÉPRÉCIATION] Changement apporté à `create-for-rbac` concernant le masquage de l’argument '--password' - Fin de la prise en charge en mai 2019</span><span class="sxs-lookup"><span data-stu-id="655ae-718">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

### <a name="service-bus"></a><span data-ttu-id="655ae-719">Service Bus</span><span class="sxs-lookup"><span data-stu-id="655ae-719">Service Bus</span></span>
* <span data-ttu-id="655ae-720">Ajout des commandes `namespace network-rule`</span><span class="sxs-lookup"><span data-stu-id="655ae-720">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="655ae-721">Ajout de l’argument `--default-action` pour les règles réseau à `namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="655ae-721">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>
* <span data-ttu-id="655ae-722">Correction de `topic [create|update]` qui autorise `--max-size` à prendre en charge les valeurs 10, 20, 40 et 80 Go avec la référence SKU Premium</span><span class="sxs-lookup"><span data-stu-id="655ae-722">Fixed `topic [create|update]` to allow `--max-size` support for 10, 20, 40 and 80GB values with premium SKU</span></span>

### <a name="sql"></a><span data-ttu-id="655ae-723">SQL</span><span class="sxs-lookup"><span data-stu-id="655ae-723">SQL</span></span>
* <span data-ttu-id="655ae-724">Ajout des commandes `sql virtual-cluster [list|show|delete]`</span><span class="sxs-lookup"><span data-stu-id="655ae-724">Added `sql virtual-cluster [list|show|delete]` commands</span></span>

### <a name="vm"></a><span data-ttu-id="655ae-725">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="655ae-725">VM</span></span>
* <span data-ttu-id="655ae-726">Ajout de `--protect-from-scale-in` et `--protect-from-scale-set-actions` à `vmss update` pour activer les mises à jour de la stratégie de protection des instances de machine virtuelle VMSS</span><span class="sxs-lookup"><span data-stu-id="655ae-726">Added `--protect-from-scale-in` and `--protect-from-scale-set-actions` to `vmss update` to enable updates to the protection policy of VMSS VM instances</span></span>
* <span data-ttu-id="655ae-727">Ajout de `--instance-id` à `vmss update` pour activer la mise à jour générique des instances de machine virtuelle VMSS</span><span class="sxs-lookup"><span data-stu-id="655ae-727">Added `--instance-id` to `vmss update` to enable generic update of VMSS VM instances</span></span>
* <span data-ttu-id="655ae-728">Ajout de `--instance-id` à `vmss wait`</span><span class="sxs-lookup"><span data-stu-id="655ae-728">Added `--instance-id` to `vmss wait`</span></span>
* <span data-ttu-id="655ae-729">Ajout du nouveau groupe de commandes `ppg` pour gérer les groupes de placements de proximité</span><span class="sxs-lookup"><span data-stu-id="655ae-729">Added new `ppg` command group for managing Proximity Placement Groups</span></span>
* <span data-ttu-id="655ae-730">Ajout de `--ppg` à `[vm|vmss] create` et `vm availability-set create` pour la gestion des groupes de placements de proximité</span><span class="sxs-lookup"><span data-stu-id="655ae-730">Added `--ppg` to `[vm|vmss] create` and `vm availability-set create` for managing PPGs</span></span>
* <span data-ttu-id="655ae-731">Ajout du paramètre `--hyper-v-generation` pour `image create`</span><span class="sxs-lookup"><span data-stu-id="655ae-731">Added `--hyper-v-generation` parameter to `image create`</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="655ae-732">23 avril 2019</span><span class="sxs-lookup"><span data-stu-id="655ae-732">April 23, 2019</span></span>

<span data-ttu-id="655ae-733">Version 2.0.63</span><span class="sxs-lookup"><span data-stu-id="655ae-733">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="655ae-734">ACS</span><span class="sxs-lookup"><span data-stu-id="655ae-734">ACS</span></span>
* <span data-ttu-id="655ae-735">Changement apporté à `aks get-credentials` pour demander confirmation en cas de remplacement de valeurs dupliquées</span><span class="sxs-lookup"><span data-stu-id="655ae-735">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="655ae-736">Suppression de `(PREVIEW)` des commandes Dev Spaces « aks use-dev-spaces » et « aks remove-dev-spaces »</span><span class="sxs-lookup"><span data-stu-id="655ae-736">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="655ae-737">AMS</span><span class="sxs-lookup"><span data-stu-id="655ae-737">AMS</span></span>
* <span data-ttu-id="655ae-738">Correction d’un bogue lié à la mise à jour des filtres de composant et de compte</span><span class="sxs-lookup"><span data-stu-id="655ae-738">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="655ae-739">AppService</span><span class="sxs-lookup"><span data-stu-id="655ae-739">AppService</span></span>
* <span data-ttu-id="655ae-740">Ajout de la prise en charge d’ASE et de délais d’expiration à `webapp ssh`</span><span class="sxs-lookup"><span data-stu-id="655ae-740">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="655ae-741">Ajout de la prise en charge de l’établissement de CI/CD dans un pipeline Azure DevOps entre un dépôt Github et des applications de fonction</span><span class="sxs-lookup"><span data-stu-id="655ae-741">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="655ae-742">Ajout de l’argument `--github-pat` à `functionapp devops-build create` pour accepter un jeton d’accès personnel Github</span><span class="sxs-lookup"><span data-stu-id="655ae-742">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="655ae-743">Ajout de l’argument `--github-repository` à `functionapp devops-build create` pour accepter un dépôt Github contenant le code source d’une application de fonction</span><span class="sxs-lookup"><span data-stu-id="655ae-743">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="655ae-744">Résolution d’un problème provoquant l’échec de `az webapp up --logs` avec une erreur et la mise à jour de la version par défaut NETCORE avec la version 2.1</span><span class="sxs-lookup"><span data-stu-id="655ae-744">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="655ae-745">Suppression des paramètres d’application de fonction inutiles lors de la création d’une telle application avec un plan de consommation</span><span class="sxs-lookup"><span data-stu-id="655ae-745">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="655ae-746">Changement apporté à `webapp up` pour ajouter un numéro à la fin de la chaîne asp par défaut afin de créer un ASP basé sur les options de la référence SKU</span><span class="sxs-lookup"><span data-stu-id="655ae-746">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="655ae-747">Ajout de `-b` en tant qu’option à `webapp up` pour lancer l’application dans le navigateur</span><span class="sxs-lookup"><span data-stu-id="655ae-747">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="655ae-748">Changement apporté à `webapp deployment source config zip` pour gérer la variable d’environnement `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`</span><span class="sxs-lookup"><span data-stu-id="655ae-748">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="655ae-749">Gestionnaire de déploiement</span><span class="sxs-lookup"><span data-stu-id="655ae-749">Deployment Manager</span></span>
* <span data-ttu-id="655ae-750">[PRÉVERSION] Création et gestion d’artefacts prenant en charge les lancements</span><span class="sxs-lookup"><span data-stu-id="655ae-750">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="655ae-751">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="655ae-751">Lab</span></span>
* <span data-ttu-id="655ae-752">Correction d’un bogue provoquant une sortie anticipée</span><span class="sxs-lookup"><span data-stu-id="655ae-752">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="655ae-753">Réseau</span><span class="sxs-lookup"><span data-stu-id="655ae-753">Network</span></span>
* <span data-ttu-id="655ae-754">Ajout d’une délégation de serveurs nommés automatiquement à `dns zone create` dans le parent durant la création d’une zone enfant</span><span class="sxs-lookup"><span data-stu-id="655ae-754">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="655ae-755">Ressource</span><span class="sxs-lookup"><span data-stu-id="655ae-755">Resource</span></span>
* <span data-ttu-id="655ae-756">[DÉPRÉCIATION] Dépréciation des arguments `--link-id`, `--target-id` et `--filter-string` de `resource link`</span><span class="sxs-lookup"><span data-stu-id="655ae-756">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="655ae-757">Arguments remplacés par `--link`, `--target` et `--filter`</span><span class="sxs-lookup"><span data-stu-id="655ae-757">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="655ae-758">Correction d’un problème empêchant le fonctionnement des commandes `resource link [create|update]`</span><span class="sxs-lookup"><span data-stu-id="655ae-758">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="655ae-759">Correction d’un problème où une suppression effectuée à l’aide d’un ID de ressource pouvait entraîner un plantage en cas d’erreur</span><span class="sxs-lookup"><span data-stu-id="655ae-759">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="655ae-760">SQL</span><span class="sxs-lookup"><span data-stu-id="655ae-760">SQL</span></span>
* <span data-ttu-id="655ae-761">Ajout de la prise en charge d’un fuseau horaire personnalisé sur les instances managées</span><span class="sxs-lookup"><span data-stu-id="655ae-761">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="655ae-762">Changement apporté pour autoriser l’utilisation d’un nom de pool élastique avec `sql db update`</span><span class="sxs-lookup"><span data-stu-id="655ae-762">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="655ae-763">Ajout de la prise en charge de `--no-wait` pour `sql server [create|update]`</span><span class="sxs-lookup"><span data-stu-id="655ae-763">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="655ae-764">Ajout de la commande `sql server wait`</span><span class="sxs-lookup"><span data-stu-id="655ae-764">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="655ae-765">Stockage</span><span class="sxs-lookup"><span data-stu-id="655ae-765">Storage</span></span>
* <span data-ttu-id="655ae-766">Résolution du problème lié aux jetons SAS à double encodage dans `storage blob generate-sas`</span><span class="sxs-lookup"><span data-stu-id="655ae-766">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="655ae-767">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="655ae-767">VM</span></span>
* <span data-ttu-id="655ae-768">Ajout de l’indicateur `--skip-shutdown` à `vm|vmss stop` pour mettre hors tension les machines virtuelles sans les arrêter</span><span class="sxs-lookup"><span data-stu-id="655ae-768">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="655ae-769">Ajout de l’argument `--storage-account-type` à `sig image-version create` pour définir le type de compte du profil de publication</span><span class="sxs-lookup"><span data-stu-id="655ae-769">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="655ae-770">Ajout de l’argument `--target-regions` à `sig image-version create` pour autoriser la définition de types de comptes de stockage spécifiques à une région</span><span class="sxs-lookup"><span data-stu-id="655ae-770">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="655ae-771">9 avril 2019</span><span class="sxs-lookup"><span data-stu-id="655ae-771">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="655ae-772">Core</span><span class="sxs-lookup"><span data-stu-id="655ae-772">Core</span></span>
* <span data-ttu-id="655ae-773">Correction du problème où certaines extensions affichaient une version `Unknown` et ne pouvaient pas être mises à jour</span><span class="sxs-lookup"><span data-stu-id="655ae-773">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="655ae-774">ACR</span><span class="sxs-lookup"><span data-stu-id="655ae-774">ACR</span></span>
* <span data-ttu-id="655ae-775">Ajout de la prise en charge de l’exécution d’une image sans contexte</span><span class="sxs-lookup"><span data-stu-id="655ae-775">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="655ae-776">AMS</span><span class="sxs-lookup"><span data-stu-id="655ae-776">AMS</span></span>
* [DÉPRÉCIATION]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [CHANGEMENT CASSANT]: Renamed the `--bitrate` parameter to `--first-quality`
[BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="655ae-779">Ajout de la prise en charge de nouveaux paramètres de chiffrement dans `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="655ae-779">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="655ae-780">Ajout du nouveau paramètre `--filters` à `ams streaming-locator create`</span><span class="sxs-lookup"><span data-stu-id="655ae-780">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="655ae-781">AppService</span><span class="sxs-lookup"><span data-stu-id="655ae-781">AppService</span></span>
* <span data-ttu-id="655ae-782">Ajout de la prise en charge de `--logs` pour `webapp up`</span><span class="sxs-lookup"><span data-stu-id="655ae-782">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="655ae-783">Correction des problèmes de génération de `azure-pipelines.yml` avec la commande `functionapp devops-build create`</span><span class="sxs-lookup"><span data-stu-id="655ae-783">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="655ae-784">Amélioration des indicateurs et de la gestion des erreurs `unctionapp devops-build create`</span><span class="sxs-lookup"><span data-stu-id="655ae-784">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="655ae-785">[CHANGEMENT CASSANT] Suppression de l’indicateur `--local-git` pour la commande `devops-build` ; la détection et la gestion d’un Git local sont obligatoires pour créer des pipelines Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="655ae-785">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="655ae-786">Ajout de la prise en charge de la création de plan de fonction pour Linux</span><span class="sxs-lookup"><span data-stu-id="655ae-786">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="655ae-787">Ajout de la possibilité de changer de plan sous une application de fonction avec `functionapp update --plan`</span><span class="sxs-lookup"><span data-stu-id="655ae-787">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="655ae-788">Ajout de la prise en charge de paramètres de scale-out pour le plan Azure Functions Premium</span><span class="sxs-lookup"><span data-stu-id="655ae-788">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="655ae-789">CDN</span><span class="sxs-lookup"><span data-stu-id="655ae-789">CDN</span></span>
* <span data-ttu-id="655ae-790">Ajout de la prise en charge de `Microsoft_Standard` et de `Standard_ChinaCdn`</span><span class="sxs-lookup"><span data-stu-id="655ae-790">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="655ae-791">Commentaires</span><span class="sxs-lookup"><span data-stu-id="655ae-791">Feedback</span></span>
* <span data-ttu-id="655ae-792">Changement apporté à `feedback` pour afficher les métadonnées sur les commandes exécutées récemment</span><span class="sxs-lookup"><span data-stu-id="655ae-792">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="655ae-793">Changement apporté à `feedback` pour inviter l’utilisateur à ouvrir un navigateur et à utiliser un modèle de message de problème afin de faciliter le processus de création du ticket</span><span class="sxs-lookup"><span data-stu-id="655ae-793">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="655ae-794">Changement apporté à `feedback` pour afficher le corps du message du problème quand la commande est exécutée avec '--verbose'</span><span class="sxs-lookup"><span data-stu-id="655ae-794">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="655ae-795">Surveiller</span><span class="sxs-lookup"><span data-stu-id="655ae-795">Monitor</span></span>
* <span data-ttu-id="655ae-796">Correction du problème où « count » n’était pas une valeur autorisée avec `metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="655ae-796">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="655ae-797">Réseau</span><span class="sxs-lookup"><span data-stu-id="655ae-797">Network</span></span>
* <span data-ttu-id="655ae-798">Correction du problème empêchant l’affichage du format de table avec `vnet-gateway list-bgp-peer-status`</span><span class="sxs-lookup"><span data-stu-id="655ae-798">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="655ae-799">Ajout des commandes `list-request-headers` et `list-response-headers` à `application-gateway rewrite-rule`</span><span class="sxs-lookup"><span data-stu-id="655ae-799">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="655ae-800">Ajout de la commande `list-server-variables` à `application-gateway rewrite-rule condition`</span><span class="sxs-lookup"><span data-stu-id="655ae-800">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="655ae-801">Correction du problème où la mise à jour de l’état d’une liaison sur un port express-route levait une exception d’attribut inconnu `express-route port update`</span><span class="sxs-lookup"><span data-stu-id="655ae-801">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="655ae-802">PrivateDNS</span><span class="sxs-lookup"><span data-stu-id="655ae-802">PrivateDNS</span></span>
* <span data-ttu-id="655ae-803">Ajout de `network private-dns` pour les zones de DNS privé</span><span class="sxs-lookup"><span data-stu-id="655ae-803">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="655ae-804">Ressource</span><span class="sxs-lookup"><span data-stu-id="655ae-804">Resource</span></span>
* <span data-ttu-id="655ae-805">Correction du problème avec `deployment create` et `group deployment create` où un fichier de paramètres avec un ensemble de paramètres vide ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="655ae-805">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="655ae-806">Role</span><span class="sxs-lookup"><span data-stu-id="655ae-806">Role</span></span>
* <span data-ttu-id="655ae-807">Correction de `create-for-rbac` pour gérer `--years` correctement</span><span class="sxs-lookup"><span data-stu-id="655ae-807">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="655ae-808">[CHANGEMENT CASSANT] Changement apporté à `role assignment delete` pour afficher une invite lors d’une suppression sans condition de toutes les attributions sous l’abonnement</span><span class="sxs-lookup"><span data-stu-id="655ae-808">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="655ae-809">SQL</span><span class="sxs-lookup"><span data-stu-id="655ae-809">SQL</span></span>
* <span data-ttu-id="655ae-810">Mise à jour de `sql mi [create|update]` avec les propriétés proxyOverride et publicDataEndpointEnabledd</span><span class="sxs-lookup"><span data-stu-id="655ae-810">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="655ae-811">Stockage</span><span class="sxs-lookup"><span data-stu-id="655ae-811">Storage</span></span>
* <span data-ttu-id="655ae-812">[CHANGEMENT CASSANT] Suppression du résultat de `storage blob delete`</span><span class="sxs-lookup"><span data-stu-id="655ae-812">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="655ae-813">Ajout de `--full-uri` à `storage blob generate-sas` pour créer l’URI complet pour l’objet blob avec SAS</span><span class="sxs-lookup"><span data-stu-id="655ae-813">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="655ae-814">Ajout de `--file-snapshot` à `storage file copy start` pour copier le fichier à partir de l’instantané</span><span class="sxs-lookup"><span data-stu-id="655ae-814">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="655ae-815">Changement apporté à `storage blob copy cancel` pour afficher uniquement l’erreur au lieu de l’exception pour NoPendingCopyOperation</span><span class="sxs-lookup"><span data-stu-id="655ae-815">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="655ae-816">26 mars 2019</span><span class="sxs-lookup"><span data-stu-id="655ae-816">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="655ae-817">Core</span><span class="sxs-lookup"><span data-stu-id="655ae-817">Core</span></span>
* <span data-ttu-id="655ae-818">Résolution des problèmes d’incompatibilité des extensions de développement</span><span class="sxs-lookup"><span data-stu-id="655ae-818">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="655ae-819">La gestion des erreurs redirige les clients vers la page des problèmes</span><span class="sxs-lookup"><span data-stu-id="655ae-819">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="655ae-820">Cloud</span><span class="sxs-lookup"><span data-stu-id="655ae-820">Cloud</span></span>
* <span data-ttu-id="655ae-821">Correction d’une erreur « abonnement introuvable » dans `cloud set`</span><span class="sxs-lookup"><span data-stu-id="655ae-821">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="655ae-822">ACR</span><span class="sxs-lookup"><span data-stu-id="655ae-822">ACR</span></span>
* <span data-ttu-id="655ae-823">Correction d’un problème concernant des sources redondantes lors de l’importation d’images</span><span class="sxs-lookup"><span data-stu-id="655ae-823">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="655ae-824">Ajout de `--auth-mode` aux commandes `acr build`, `acr run`, `acr task create` et `acr task update`</span><span class="sxs-lookup"><span data-stu-id="655ae-824">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="655ae-825">Ajout du groupe de commandes 'acr task credential' pour la gestion des informations d’identification pour une tâche</span><span class="sxs-lookup"><span data-stu-id="655ae-825">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="655ae-826">Ajout de '--no-wait' à la commande `acr build`</span><span class="sxs-lookup"><span data-stu-id="655ae-826">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="655ae-827">AppService</span><span class="sxs-lookup"><span data-stu-id="655ae-827">AppService</span></span>
* <span data-ttu-id="655ae-828">Correction du bogue où `webapp up` ne gérait pas correctement l’exécution dans un scénario de répertoire vide ou de code inconnu</span><span class="sxs-lookup"><span data-stu-id="655ae-828">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="655ae-829">Correction du bogue où les emplacements ne fonctionnaient pas pour `[webapp|functionapp] config ssl bind`</span><span class="sxs-lookup"><span data-stu-id="655ae-829">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="655ae-830">Service BOT</span><span class="sxs-lookup"><span data-stu-id="655ae-830">BOT Service</span></span>
* <span data-ttu-id="655ae-831">Ajout de `bot prepare-deploy` pour préparer le déploiement de bots via `webapp`</span><span class="sxs-lookup"><span data-stu-id="655ae-831">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="655ae-832">Modification de `bot create --kind registration` pour afficher le mot de passe si celui-ci n’est pas fourni</span><span class="sxs-lookup"><span data-stu-id="655ae-832">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="655ae-833">[CHANGEMENT CASSANT] Changement de `--endpoint` dans `bot create --kind registration` pour qu’il soit par défaut dans une chaîne vide au lieu d’être requis</span><span class="sxs-lookup"><span data-stu-id="655ae-833">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="655ae-834">Ajout de `SCM_DO_BUILD_DURING_DEPLOYMENT` aux paramètres d’application du modèle ARM pour Web App Bots v4</span><span class="sxs-lookup"><span data-stu-id="655ae-834">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="655ae-835">CDN</span><span class="sxs-lookup"><span data-stu-id="655ae-835">CDN</span></span>
* <span data-ttu-id="655ae-836">Ajout de la prise en charge de `--no-wait` pour `cdn endpoint [create|update|start|stop|delete|load|purge]`</span><span class="sxs-lookup"><span data-stu-id="655ae-836">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* <span data-ttu-id="655ae-837">[CHANGEMENT CASSANT] : Changement du comportement de mise en cache de chaînes de requête par défaut de `cdn endpoint create`.</span><span class="sxs-lookup"><span data-stu-id="655ae-837">[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour.</span></span> <span data-ttu-id="655ae-838">Sa valeur par défaut n’est plus « IgnoreQueryString ».</span><span class="sxs-lookup"><span data-stu-id="655ae-838">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="655ae-839">Il est maintenant défini par le service</span><span class="sxs-lookup"><span data-stu-id="655ae-839">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="655ae-840">Cosmosdb</span><span class="sxs-lookup"><span data-stu-id="655ae-840">Cosmosdb</span></span>
* <span data-ttu-id="655ae-841">Ajout de la prise en charge de `--enable-multiple-write-locations` lors de la mise à jour de compte</span><span class="sxs-lookup"><span data-stu-id="655ae-841">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="655ae-842">Ajout du sous-groupe `network-rule` avec les commandes `add`, `remove` et `list` pour gérer les règles de réseau virtuel d’un compte Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="655ae-842">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="655ae-843">Interactive</span><span class="sxs-lookup"><span data-stu-id="655ae-843">Interactive</span></span>
* <span data-ttu-id="655ae-844">Correction d’une incompatibilité avec l’extension Interactive installée via azdev</span><span class="sxs-lookup"><span data-stu-id="655ae-844">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="655ae-845">Surveiller</span><span class="sxs-lookup"><span data-stu-id="655ae-845">Monitor</span></span>
* <span data-ttu-id="655ae-846">Changement visant à autoriser la valeur de dimension `*` pour `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="655ae-846">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="655ae-847">Réseau</span><span class="sxs-lookup"><span data-stu-id="655ae-847">Network</span></span>
* <span data-ttu-id="655ae-848">Ajout du groupe de commandes `rewrite-rule` à `application-gateway`</span><span class="sxs-lookup"><span data-stu-id="655ae-848">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="655ae-849">Profil</span><span class="sxs-lookup"><span data-stu-id="655ae-849">Profile</span></span>
* <span data-ttu-id="655ae-850">Ajout de la prise en charge du compte de niveau locataire pour Managed Service Identity dans `login`</span><span class="sxs-lookup"><span data-stu-id="655ae-850">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="655ae-851">Postgres</span><span class="sxs-lookup"><span data-stu-id="655ae-851">Postgres</span></span> 
* <span data-ttu-id="655ae-852">Ajout des commandes `replica` et de la commande `restart server` postgresql</span><span class="sxs-lookup"><span data-stu-id="655ae-852">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="655ae-853">Changement permettant d’obtenir l’emplacement par défaut du groupe de ressources lorsqu’il n’a pas été fourni, pour la création de serveurs et l’ajout d’une validation pour les jours de conservation</span><span class="sxs-lookup"><span data-stu-id="655ae-853">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="655ae-854">Ressource</span><span class="sxs-lookup"><span data-stu-id="655ae-854">Resource</span></span>
* <span data-ttu-id="655ae-855">Amélioration de la sortie de table pour `deployment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="655ae-855">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="655ae-856">Correction du problème avec `deployment [create|validate]` où le secureObject de type n’était pas reconnu</span><span class="sxs-lookup"><span data-stu-id="655ae-856">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="655ae-857">Graph</span><span class="sxs-lookup"><span data-stu-id="655ae-857">Graph</span></span>
* <span data-ttu-id="655ae-858">Ajout de la prise en charge de `--end-date` pour `ad [app|sp] credential reset`</span><span class="sxs-lookup"><span data-stu-id="655ae-858">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="655ae-859">Ajout de la prise en charge permettant d’ajouter des autorisations avec `ad app permission add`</span><span class="sxs-lookup"><span data-stu-id="655ae-859">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="655ae-860">Correction d’un bogue avec `ad app permission list` où il n’existait aucune autorisation</span><span class="sxs-lookup"><span data-stu-id="655ae-860">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="655ae-861">Modification de `ad sp delete` pour ignorer la suppression d’attribution de rôle si le compte actuel n’a aucun abonnement</span><span class="sxs-lookup"><span data-stu-id="655ae-861">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="655ae-862">Modification de `ad app create` pour avoir `--identifier-uris` par défaut dans une liste vide si non fourni</span><span class="sxs-lookup"><span data-stu-id="655ae-862">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="655ae-863">storage</span><span class="sxs-lookup"><span data-stu-id="655ae-863">storage</span></span>
* <span data-ttu-id="655ae-864">Ajout de `--snapshot` à `storage file download-batch` pour télécharger depuis un instantané de partage</span><span class="sxs-lookup"><span data-stu-id="655ae-864">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="655ae-865">Modification de la barre de progression `storage blob [download-batch|upload-batch]` pour qu’elle soit moins détaillée et qu’elle indique les objets blob actuels</span><span class="sxs-lookup"><span data-stu-id="655ae-865">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="655ae-866">Correction du problème avec `storage account update` lors de la mise à jour des paramètres de chiffrement</span><span class="sxs-lookup"><span data-stu-id="655ae-866">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="655ae-867">Correction d’un problème où `storage blob show` échouait quand oauth était utilisé (`--auth-mode=login`)</span><span class="sxs-lookup"><span data-stu-id="655ae-867">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="655ae-868">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="655ae-868">VM</span></span>
* <span data-ttu-id="655ae-869">Ajout de la commande `image update`</span><span class="sxs-lookup"><span data-stu-id="655ae-869">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="655ae-870">12 mars 2019</span><span class="sxs-lookup"><span data-stu-id="655ae-870">March 12, 2019</span></span>

<span data-ttu-id="655ae-871">Version 2.0.60</span><span class="sxs-lookup"><span data-stu-id="655ae-871">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="655ae-872">Core</span><span class="sxs-lookup"><span data-stu-id="655ae-872">Core</span></span>

* <span data-ttu-id="655ae-873">Correction d’une erreur dans `cloud set` concernant un abonnement introuvable</span><span class="sxs-lookup"><span data-stu-id="655ae-873">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="655ae-874">ACR</span><span class="sxs-lookup"><span data-stu-id="655ae-874">ACR</span></span>

* <span data-ttu-id="655ae-875">Correction d’un problème concernant des sources redondantes lors de l’importation d’images</span><span class="sxs-lookup"><span data-stu-id="655ae-875">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="655ae-876">ACS</span><span class="sxs-lookup"><span data-stu-id="655ae-876">ACS</span></span>

* <span data-ttu-id="655ae-877">Changement apporté pour que le paramètre `--listen-address` dans `aks browse` soit ignoré s’il n’est pas pris en charge par kubectl</span><span class="sxs-lookup"><span data-stu-id="655ae-877">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="655ae-878">AppService</span><span class="sxs-lookup"><span data-stu-id="655ae-878">AppService</span></span>

* <span data-ttu-id="655ae-879">Ajout de `[webapp|functionapp] deployment list-publishing-credentials` pour obtenir l’URL de publication Kudu et ses informations d’identification</span><span class="sxs-lookup"><span data-stu-id="655ae-879">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="655ae-880">Suppression d’une instruction print erronée pour `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="655ae-880">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="655ae-881">Correction de `functionapp` pour définir la bonne image runtime dans les plans App Service Linux</span><span class="sxs-lookup"><span data-stu-id="655ae-881">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="655ae-882">Suppression de l’étiquette de préversion pour `webapp up` et ajout d’améliorations à la commande</span><span class="sxs-lookup"><span data-stu-id="655ae-882">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="655ae-883">Botservice</span><span class="sxs-lookup"><span data-stu-id="655ae-883">Botservice</span></span>

* <span data-ttu-id="655ae-884">Ajout de `SCM_DO_BUILD_DURING_DEPLOYMENT` aux paramètres d’application du modèle ARM pour Web App Bots v4</span><span class="sxs-lookup"><span data-stu-id="655ae-884">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="655ae-885">Ajout de `Microsoft-BotFramework-AppId` et de `Microsoft-BotFramework-AppPassword` aux paramètres d’application du modèle ARM pour Web App Bots v4</span><span class="sxs-lookup"><span data-stu-id="655ae-885">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="655ae-886">Suppression des guillemets simples dans la sortie de la commande `bot publish`, à la fin de `bot create`</span><span class="sxs-lookup"><span data-stu-id="655ae-886">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="655ae-887">Modification de `bot publish` pour le rendre asynchrone</span><span class="sxs-lookup"><span data-stu-id="655ae-887">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="655ae-888">Conteneur</span><span class="sxs-lookup"><span data-stu-id="655ae-888">Container</span></span>

* <span data-ttu-id="655ae-889">Ajout de l’argument `--no-wait` à `container [start|restart]`</span><span class="sxs-lookup"><span data-stu-id="655ae-889">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="655ae-890">Event Hub</span><span class="sxs-lookup"><span data-stu-id="655ae-890">EventHub</span></span>

* <span data-ttu-id="655ae-891">Ajout de l’indicateur `--skip-empty-archives` à `eventhub create|update` pour prendre en charge les archives vides dans les captures</span><span class="sxs-lookup"><span data-stu-id="655ae-891">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="655ae-892">Rechercher</span><span class="sxs-lookup"><span data-stu-id="655ae-892">Find</span></span>

* <span data-ttu-id="655ae-893">Mise à jour importante de fonctionnalités</span><span class="sxs-lookup"><span data-stu-id="655ae-893">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="655ae-894">HDInsight</span><span class="sxs-lookup"><span data-stu-id="655ae-894">HDInsight</span></span>

* <span data-ttu-id="655ae-895">Ajout du paramètre `--storage-account-managed-identity` à `hdinsight create` pour prendre en charge le MSI ADLS Gen2</span><span class="sxs-lookup"><span data-stu-id="655ae-895">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="655ae-896">Réseau</span><span class="sxs-lookup"><span data-stu-id="655ae-896">Network</span></span>

* <span data-ttu-id="655ae-897">Correction d’un problème concernant `vpn-connection update`, qui provoquait l’échec de la mise à jour d’une connexion VPN établie entre deux passerelles appartenant à des abonnements différents</span><span class="sxs-lookup"><span data-stu-id="655ae-897">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="655ae-898">Rdbms</span><span class="sxs-lookup"><span data-stu-id="655ae-898">Rdbms</span></span>

* <span data-ttu-id="655ae-899">Correctifs mineurs permettant d’obtenir l’emplacement par défaut du groupe de ressources lorsqu’il n’a pas été fourni, pour la création de serveurs et l’ajout d’une validation pour les jours de rétention</span><span class="sxs-lookup"><span data-stu-id="655ae-899">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="655ae-900">Role</span><span class="sxs-lookup"><span data-stu-id="655ae-900">Role</span></span>

* <span data-ttu-id="655ae-901">Correction de `role definition update` pour utiliser l’ID afin de résoudre correctement les définitions</span><span class="sxs-lookup"><span data-stu-id="655ae-901">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="655ae-902">Modification de `ad app credential reset` pour ne plus partir du principe que le principal de service de l’application existe toujours</span><span class="sxs-lookup"><span data-stu-id="655ae-902">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="655ae-903">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="655ae-903">Service Fabric</span></span>

* <span data-ttu-id="655ae-904">Correction du problème où `sf cluster list` n’était pas itérable</span><span class="sxs-lookup"><span data-stu-id="655ae-904">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="655ae-905">26 février 2019</span><span class="sxs-lookup"><span data-stu-id="655ae-905">February 26, 2019</span></span>

<span data-ttu-id="655ae-906">Version 2.0.59</span><span class="sxs-lookup"><span data-stu-id="655ae-906">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="655ae-907">Core</span><span class="sxs-lookup"><span data-stu-id="655ae-907">Core</span></span>

* <span data-ttu-id="655ae-908">Correction du problème où l’utilisation de `--subscription NAME` levait une exception dans certains cas</span><span class="sxs-lookup"><span data-stu-id="655ae-908">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="655ae-909">ACR</span><span class="sxs-lookup"><span data-stu-id="655ae-909">ACR</span></span>

* <span data-ttu-id="655ae-910">Ajout du paramètre `--target` pour les commandes `acr build`, `acr task create` et `acr task update`</span><span class="sxs-lookup"><span data-stu-id="655ae-910">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="655ae-911">Amélioration de la gestion des erreurs pour les commandes de runtime quand vous n’êtes pas connecté à Azure</span><span class="sxs-lookup"><span data-stu-id="655ae-911">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="655ae-912">ACS</span><span class="sxs-lookup"><span data-stu-id="655ae-912">ACS</span></span>

* <span data-ttu-id="655ae-913">Ajout de l’option `--listen-address` à `aks port-forward`</span><span class="sxs-lookup"><span data-stu-id="655ae-913">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="655ae-914">AppService</span><span class="sxs-lookup"><span data-stu-id="655ae-914">AppService</span></span>

* <span data-ttu-id="655ae-915">Ajout de la commande `functionapp devops-build`</span><span class="sxs-lookup"><span data-stu-id="655ae-915">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="655ae-916">Batch</span><span class="sxs-lookup"><span data-stu-id="655ae-916">Batch</span></span>
* <span data-ttu-id="655ae-917">[CHANGEMENT CASSANT] Suppression de la commande `batch pool upgrade os`</span><span class="sxs-lookup"><span data-stu-id="655ae-917">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="655ae-918">[CHANGEMENT CASSANT] Suppression de la propriété `Pacakges` des réponses `Application`</span><span class="sxs-lookup"><span data-stu-id="655ae-918">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="655ae-919">Ajout de la commande `batch application package list` pour lister les packages d’une application</span><span class="sxs-lookup"><span data-stu-id="655ae-919">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="655ae-920">[CHANGEMENT CASSANT] Remplacement de `--application-id` par `--application-name` dans toutes les commandes `batch application`</span><span class="sxs-lookup"><span data-stu-id="655ae-920">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="655ae-921">Ajout de l’argument `--json-file` aux commandes permettant de demander la réponse d’API brute</span><span class="sxs-lookup"><span data-stu-id="655ae-921">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="655ae-922">Mise à jour de la validation pour inclure automatiquement `https://` dans tous les points de terminaison si manquant</span><span class="sxs-lookup"><span data-stu-id="655ae-922">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="655ae-923">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="655ae-923">CosmosDB</span></span>

* <span data-ttu-id="655ae-924">Ajout du sous-groupe `network-rule` avec les commandes `add`, `remove` et `list` pour gérer les règles de réseau virtuel d’un compte Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="655ae-924">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="655ae-925">Kusto</span><span class="sxs-lookup"><span data-stu-id="655ae-925">Kusto</span></span>

* <span data-ttu-id="655ae-926">[CHANGEMENT CASSANT] Changement des types `hot_cache_period` et `soft_delete_period` de la base de données en format de durée ISO8601</span><span class="sxs-lookup"><span data-stu-id="655ae-926">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="655ae-927">Réseau</span><span class="sxs-lookup"><span data-stu-id="655ae-927">Network</span></span>

* <span data-ttu-id="655ae-928">Ajout de l’argument `--express-route-gateway-bypass` à `vpn-connection [create|update]`</span><span class="sxs-lookup"><span data-stu-id="655ae-928">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="655ae-929">Ajout de groupes de commandes à partir des extensions `express-route`</span><span class="sxs-lookup"><span data-stu-id="655ae-929">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="655ae-930">Ajout des groupes de commandes `express-route gateway` et `express-route port`</span><span class="sxs-lookup"><span data-stu-id="655ae-930">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="655ae-931">Ajout d’un argument `--legacy-mode` à `express-route peering [create|update]`</span><span class="sxs-lookup"><span data-stu-id="655ae-931">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="655ae-932">Ajout des arguments `--allow-classic-operations` et `--express-route-port` à `express-route [create|update]`</span><span class="sxs-lookup"><span data-stu-id="655ae-932">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="655ae-933">Ajout de l’argument `--gateway-default-site` à `vnet-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="655ae-933">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="655ae-934">Ajout des commandes `ipsec-policy` à `vnet-gateway`</span><span class="sxs-lookup"><span data-stu-id="655ae-934">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="655ae-935">Ressource</span><span class="sxs-lookup"><span data-stu-id="655ae-935">Resource</span></span>

* <span data-ttu-id="655ae-936">Correction du problème de `deployment create` où le champ de type n’était pas sensible à la casse</span><span class="sxs-lookup"><span data-stu-id="655ae-936">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="655ae-937">Ajout de la prise en charge du fichier de paramètres basé sur l’URI sur `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="655ae-937">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="655ae-938">Ajout de la prise en charge des définitions et des paramètres basés sur l’URI sur `policy set-definition update`</span><span class="sxs-lookup"><span data-stu-id="655ae-938">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="655ae-939">Correction de la gestion des paramètres et des règles pour `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="655ae-939">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="655ae-940">Correction du problème avec `resource show/update/delete/tag/invoke-action` où les ID inter-abonnements n’honoraient pas correctement l’ID d’abonnement</span><span class="sxs-lookup"><span data-stu-id="655ae-940">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="655ae-941">Role</span><span class="sxs-lookup"><span data-stu-id="655ae-941">Role</span></span>

* <span data-ttu-id="655ae-942">Ajout de la prise en charge des rôles d’application sur `ad app [create|update]`</span><span class="sxs-lookup"><span data-stu-id="655ae-942">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="655ae-943">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="655ae-943">VM</span></span>

* <span data-ttu-id="655ae-944">Correction du problème avec `vm create where `--accelerated-networking\` qui n’était pas activé par défaut pour Ubuntu 18.0</span><span class="sxs-lookup"><span data-stu-id="655ae-944">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="655ae-945">12 février 2019</span><span class="sxs-lookup"><span data-stu-id="655ae-945">February 12, 2019</span></span>

<span data-ttu-id="655ae-946">Version 2.0.58</span><span class="sxs-lookup"><span data-stu-id="655ae-946">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="655ae-947">Core</span><span class="sxs-lookup"><span data-stu-id="655ae-947">Core</span></span>

* <span data-ttu-id="655ae-948">`az --version` affiche désormais une notification si vous avez des packages qui peuvent être mis à jour</span><span class="sxs-lookup"><span data-stu-id="655ae-948">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="655ae-949">Correction de la régression où `--ids` ne pouvait plus être utilisé avec une sortie JSON</span><span class="sxs-lookup"><span data-stu-id="655ae-949">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="655ae-950">ACR</span><span class="sxs-lookup"><span data-stu-id="655ae-950">ACR</span></span>
* <span data-ttu-id="655ae-951">[CHANGEMENT CASSANT] Suppression du groupe de commandes `acr build-task`</span><span class="sxs-lookup"><span data-stu-id="655ae-951">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="655ae-952">[CHANGEMENT CASSANT] Suppression des options `--tag` et `--manifest` dans `acr repository delete`</span><span class="sxs-lookup"><span data-stu-id="655ae-952">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="655ae-953">ACS</span><span class="sxs-lookup"><span data-stu-id="655ae-953">ACS</span></span>
* <span data-ttu-id="655ae-954">Ajout de la prise en charge des noms qui ne respectent pas la casse à `aks [enable-addons|disable-addons]`</span><span class="sxs-lookup"><span data-stu-id="655ae-954">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="655ae-955">Ajout de la prise en charge de l’opération de mise à jour d’Azure Active Directory à l’aide de `aks update-credentials --reset-aad`</span><span class="sxs-lookup"><span data-stu-id="655ae-955">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="655ae-956">Ajout d’une clarification indiquant que `--output` est ignoré pour `aks get-credentials`</span><span class="sxs-lookup"><span data-stu-id="655ae-956">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="655ae-957">AMS</span><span class="sxs-lookup"><span data-stu-id="655ae-957">AMS</span></span>
* <span data-ttu-id="655ae-958">Ajout des commandes `ams streaming-endpoint [start | stop | create | update] wait`</span><span class="sxs-lookup"><span data-stu-id="655ae-958">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="655ae-959">Ajout des commandes `ams live-event [create | start | stop | reset] wait`</span><span class="sxs-lookup"><span data-stu-id="655ae-959">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="655ae-960">AppService</span><span class="sxs-lookup"><span data-stu-id="655ae-960">Appservice</span></span>
* <span data-ttu-id="655ae-961">Ajout des possibilités de création et de configuration de fonctions à l’aide de conteneurs ACR</span><span class="sxs-lookup"><span data-stu-id="655ae-961">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="655ae-962">Ajout de la prise en charge de la mise à jour des configurations d’applications web via JSON</span><span class="sxs-lookup"><span data-stu-id="655ae-962">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="655ae-963">Amélioration de l’aide pour `appservice-plan-update`</span><span class="sxs-lookup"><span data-stu-id="655ae-963">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="655ae-964">Ajout de la prise en charge d’Application Insights sur functionapp create</span><span class="sxs-lookup"><span data-stu-id="655ae-964">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="655ae-965">Résolution des problèmes liés à webapp SSH</span><span class="sxs-lookup"><span data-stu-id="655ae-965">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="655ae-966">Botservice</span><span class="sxs-lookup"><span data-stu-id="655ae-966">Botservice</span></span>
* <span data-ttu-id="655ae-967">Amélioration de l’expérience utilisateur pour `bot publish`</span><span class="sxs-lookup"><span data-stu-id="655ae-967">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="655ae-968">Ajout d’un avertissement pour les délais d’expiration au moment de l’exécution de `npm install` durant `az bot publish`</span><span class="sxs-lookup"><span data-stu-id="655ae-968">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="655ae-969">Suppression du caractère non valide `.` de `--name` dans `az bot create`</span><span class="sxs-lookup"><span data-stu-id="655ae-969">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="655ae-970">Changement apporté pour mettre fin aux noms de ressources aléatoires durant la création du Stockage Azure, du plan App Service, de Function App/Web App et d’Application Insights</span><span class="sxs-lookup"><span data-stu-id="655ae-970">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="655ae-971">[DÉPRÉCIATION] Dépréciation de l’argument `--proj-name` en faveur de `--proj-file-path`</span><span class="sxs-lookup"><span data-stu-id="655ae-971">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="655ae-972">Changement apporté à `az bot publish` pour supprimer les fichiers de déploiements IIS Node.js récupérés (fetch), s’ils n’existent pas déjà</span><span class="sxs-lookup"><span data-stu-id="655ae-972">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="655ae-973">Ajout de l’argument `--keep-node-modules` à `az bot publish` pour éviter la suppression du dossier `node_modules` dans App Service</span><span class="sxs-lookup"><span data-stu-id="655ae-973">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="655ae-974">Ajout de la paire clé/valeur `"publishCommand"` à la sortie de `az bot create` au moment de la création d’une fonction Azure ou d’un bot Web App</span><span class="sxs-lookup"><span data-stu-id="655ae-974">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="655ae-975">La valeur de `"publishCommand"` est une commande `az bot publish` préremplie avec les paramètres obligatoires pour publier le bot venant d’être créé</span><span class="sxs-lookup"><span data-stu-id="655ae-975">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="655ae-976">Mise à jour de `"WEBSITE_NODE_DEFAULT_VERSION"` dans le modèle ARM pour permettre aux bots du kit SDK v4 d’utiliser la version 10.14.1 au lieu de la version 8.9.4</span><span class="sxs-lookup"><span data-stu-id="655ae-976">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="655ae-977">Key Vault</span><span class="sxs-lookup"><span data-stu-id="655ae-977">Key Vault</span></span>
* <span data-ttu-id="655ae-978">Correction du problème lié à `keyvault secret backup`, où certains utilisateurs recevaient une erreur `unexpected_keyword` quand ils utilisaient `--id`</span><span class="sxs-lookup"><span data-stu-id="655ae-978">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="655ae-979">Surveiller</span><span class="sxs-lookup"><span data-stu-id="655ae-979">Monitor</span></span>
* <span data-ttu-id="655ae-980">Changement apporté à `monitor metrics alert [create|update]` pour autoriser la valeur de dimension `*`</span><span class="sxs-lookup"><span data-stu-id="655ae-980">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="655ae-981">Réseau</span><span class="sxs-lookup"><span data-stu-id="655ae-981">Network</span></span>
* <span data-ttu-id="655ae-982">Changement apporté à `dns zone export` pour que les enregistrements CNAME exportés soient des noms de domaine complets</span><span class="sxs-lookup"><span data-stu-id="655ae-982">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="655ae-983">Ajout du paramètre `--gateway-name` à `nic ip-config address-pool [add|remove]` pour permettre la prise en charge des pools d’adresses back-end d’Application Gateway</span><span class="sxs-lookup"><span data-stu-id="655ae-983">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="655ae-984">Ajout des arguments `--traffic-analytics` et `--workspace` à `network watcher flow-log configure` pour permettre la prise en charge de l’analyse du trafic via un espace de travail Log Analytics</span><span class="sxs-lookup"><span data-stu-id="655ae-984">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="655ae-985">Ajout de `--idle-timeout` et `--floating-ip` à `lb inbound-nat-pool [create|update]`</span><span class="sxs-lookup"><span data-stu-id="655ae-985">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="655ae-986">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="655ae-986">Policy Insights</span></span>
* <span data-ttu-id="655ae-987">Ajout des commandes `policy remediation` pour permettre la prise en charge des fonctionnalités de correction des stratégies de ressources</span><span class="sxs-lookup"><span data-stu-id="655ae-987">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="655ae-988">SGBDR</span><span class="sxs-lookup"><span data-stu-id="655ae-988">RDBMS</span></span>
* <span data-ttu-id="655ae-989">Amélioration du message d’aide et des paramètres de commande</span><span class="sxs-lookup"><span data-stu-id="655ae-989">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="655ae-990">Redis</span><span class="sxs-lookup"><span data-stu-id="655ae-990">Redis</span></span>
* <span data-ttu-id="655ae-991">Ajout de commandes pour la gestion des règles de pare-feu (create, update, delete, show, list)</span><span class="sxs-lookup"><span data-stu-id="655ae-991">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="655ae-992">Ajout de commandes pour la gestion de la liaison avec le serveur (create, delete, show, list)</span><span class="sxs-lookup"><span data-stu-id="655ae-992">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="655ae-993">Ajout de commandes pour la gestion de la planification des correctifs (create, update, delete, show)</span><span class="sxs-lookup"><span data-stu-id="655ae-993">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="655ae-994">Ajout de la prise en charge des zones de disponibilité et de la version minimale de TLS dans redis create</span><span class="sxs-lookup"><span data-stu-id="655ae-994">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="655ae-995">[CHANGEMENT CASSANT] Suppression des commandes `redis update-settings` et `redis list-all`</span><span class="sxs-lookup"><span data-stu-id="655ae-995">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="655ae-996">[CHANGEMENT CASSANT] Le paramètre de `redis create` : « paramètres du locataire » n’est pas accepté au format clé[=valeur]</span><span class="sxs-lookup"><span data-stu-id="655ae-996">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="655ae-997">[DÉPRÉCIATION] Ajout d’un message d’avertissement concernant la dépréciation de la commande `redis import-method`</span><span class="sxs-lookup"><span data-stu-id="655ae-997">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="655ae-998">Role</span><span class="sxs-lookup"><span data-stu-id="655ae-998">Role</span></span>
* <span data-ttu-id="655ae-999">[CHANGEMENT CASSANT] Déplacement de la commande `az identity` ici à partir des commandes `vm`</span><span class="sxs-lookup"><span data-stu-id="655ae-999">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="655ae-1000">Machine virtuelle SQL</span><span class="sxs-lookup"><span data-stu-id="655ae-1000">SQL VM</span></span>
* <span data-ttu-id="655ae-1001">[DÉPRÉCIATION] Dépréciation de l’argument `--boostrap-acc-pwd` en raison d’une faute de frappe</span><span class="sxs-lookup"><span data-stu-id="655ae-1001">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="655ae-1002">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="655ae-1002">VM</span></span>
* <span data-ttu-id="655ae-1003">Changement de `vm list-skus` pour autoriser l’utilisation de `--all` à la place de `--all true`</span><span class="sxs-lookup"><span data-stu-id="655ae-1003">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="655ae-1004">Ajout de `vmss run-command [invoke | list | show]`</span><span class="sxs-lookup"><span data-stu-id="655ae-1004">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="655ae-1005">Correction d’un bogue qui entraînait l’échec de `vmss encryption enable`, s’il était exécuté</span><span class="sxs-lookup"><span data-stu-id="655ae-1005">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="655ae-1006">[CHANGEMENT CASSANT] Déplacement de la commande `az identity` vers les commandes `role`</span><span class="sxs-lookup"><span data-stu-id="655ae-1006">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="655ae-1007">31 janvier 2019</span><span class="sxs-lookup"><span data-stu-id="655ae-1007">January 31, 2019</span></span>

<span data-ttu-id="655ae-1008">Version 2.0.57</span><span class="sxs-lookup"><span data-stu-id="655ae-1008">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="655ae-1009">Core</span><span class="sxs-lookup"><span data-stu-id="655ae-1009">Core</span></span>

* <span data-ttu-id="655ae-1010">Correctif pour le [problème 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="655ae-1010">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="655ae-1011">28 janvier 2019</span><span class="sxs-lookup"><span data-stu-id="655ae-1011">January 28, 2019</span></span>

<span data-ttu-id="655ae-1012">Version 2.0.56</span><span class="sxs-lookup"><span data-stu-id="655ae-1012">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="655ae-1013">ACR</span><span class="sxs-lookup"><span data-stu-id="655ae-1013">ACR</span></span>
* <span data-ttu-id="655ae-1014">Ajout de la prise en charge des règles de réseau virtuel (VNet)/d’adresses IP</span><span class="sxs-lookup"><span data-stu-id="655ae-1014">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="655ae-1015">ACS</span><span class="sxs-lookup"><span data-stu-id="655ae-1015">ACS</span></span>
* <span data-ttu-id="655ae-1016">Ajout de l’aperçu des nœuds virtuels</span><span class="sxs-lookup"><span data-stu-id="655ae-1016">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="655ae-1017">Ajout des commandes d’OpenShift managé</span><span class="sxs-lookup"><span data-stu-id="655ae-1017">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="655ae-1018">Ajout de la prise en charge des mises à jour du principal de service avec `aks update-credentials -reset-service-principal`</span><span class="sxs-lookup"><span data-stu-id="655ae-1018">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="655ae-1019">AMS</span><span class="sxs-lookup"><span data-stu-id="655ae-1019">AMS</span></span>
* <span data-ttu-id="655ae-1020">[CHANGEMENT CASSANT] Renommage de `ams asset get-streaming-locators` en `ams asset list-streaming-locators`</span><span class="sxs-lookup"><span data-stu-id="655ae-1020">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="655ae-1021">[CHANGEMENT CASSANT] Renommage de `ams streaming-locator get-content-keys` en `ams streaming-locator list-content-keys`</span><span class="sxs-lookup"><span data-stu-id="655ae-1021">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="655ae-1022">AppService</span><span class="sxs-lookup"><span data-stu-id="655ae-1022">Appservice</span></span>
* <span data-ttu-id="655ae-1023">Ajout de la prise en charge d’Application Insights sur `functionapp create`</span><span class="sxs-lookup"><span data-stu-id="655ae-1023">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="655ae-1024">Ajout de la prise en charge de la création de plans App Service (notamment Elastic Premium) à Function App</span><span class="sxs-lookup"><span data-stu-id="655ae-1024">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="655ae-1025">Correction de problèmes de configuration des applications avec les plans Elastic Premium</span><span class="sxs-lookup"><span data-stu-id="655ae-1025">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="655ae-1026">Conteneur</span><span class="sxs-lookup"><span data-stu-id="655ae-1026">Container</span></span>
* <span data-ttu-id="655ae-1027">Ajout de la commande `container start`</span><span class="sxs-lookup"><span data-stu-id="655ae-1027">Added `container start` command</span></span>
* <span data-ttu-id="655ae-1028">Changements apportés afin de permettre l’utilisation de valeurs décimales pour le processeur durant la création d’un conteneur</span><span class="sxs-lookup"><span data-stu-id="655ae-1028">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="655ae-1029">EventGrid</span><span class="sxs-lookup"><span data-stu-id="655ae-1029">EventGrid</span></span>
* <span data-ttu-id="655ae-1030">Ajout du paramètre `--deadletter-endpoint` pour `event-subscription [create|update]`</span><span class="sxs-lookup"><span data-stu-id="655ae-1030">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="655ae-1031">Ajout de storagequeue et hybridconnection en tant que nouvelles valeurs pour « event-subscription [create|update] --endpoint-type »</span><span class="sxs-lookup"><span data-stu-id="655ae-1031">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="655ae-1032">Ajout des paramètres `--max-delivery-attempts` et `--event-ttl` à `event-subscription create` pour spécifier la stratégie de nouvelles tentatives des événements</span><span class="sxs-lookup"><span data-stu-id="655ae-1032">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="655ae-1033">Ajout d’un message d’avertissement à `event-subscription [create|update]` en cas d’utilisation de Webhook en tant que destination pour un abonnement à un événement</span><span class="sxs-lookup"><span data-stu-id="655ae-1033">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="655ae-1034">Ajout du paramètre source-resource-id pour toutes les commandes relatives à un abonnement aux événements et marquage de tous les autres paramètres relatifs aux ressources sources comme étant dépréciés</span><span class="sxs-lookup"><span data-stu-id="655ae-1034">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="655ae-1035">HDInsight</span><span class="sxs-lookup"><span data-stu-id="655ae-1035">HDInsight</span></span>
* <span data-ttu-id="655ae-1036">[CHANGEMENT CASSANT] Suppression des paramètres `--virtual-network` et `--subnet-name` dans `hdinsight [application] create`</span><span class="sxs-lookup"><span data-stu-id="655ae-1036">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="655ae-1037">[CHANGEMENT CASSANT] Changement apporté à `hdinsight create --storage-account` pour accepter le nom ou l’ID du compte de stockage à la place des points de terminaison d’objet blob</span><span class="sxs-lookup"><span data-stu-id="655ae-1037">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="655ae-1038">Ajout des paramètres `--vnet-name` et `--subnet-name` à `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="655ae-1038">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="655ae-1039">Ajout de la prise en charge du Pack Sécurité Entreprise et du chiffrement de disque à `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="655ae-1039">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="655ae-1040">Ajout de la commande `hdinsight rotate-disk-encryption-key`</span><span class="sxs-lookup"><span data-stu-id="655ae-1040">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="655ae-1041">Ajout de la commande `hdinsight update`</span><span class="sxs-lookup"><span data-stu-id="655ae-1041">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="655ae-1042">IoT</span><span class="sxs-lookup"><span data-stu-id="655ae-1042">IoT</span></span>
* <span data-ttu-id="655ae-1043">Ajout du format d’encodage à la commande routing-endpoint</span><span class="sxs-lookup"><span data-stu-id="655ae-1043">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="655ae-1044">Kusto</span><span class="sxs-lookup"><span data-stu-id="655ae-1044">Kusto</span></span>
* <span data-ttu-id="655ae-1045">Préversion</span><span class="sxs-lookup"><span data-stu-id="655ae-1045">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="655ae-1046">Surveiller</span><span class="sxs-lookup"><span data-stu-id="655ae-1046">Monitor</span></span>
* <span data-ttu-id="655ae-1047">Changement apporté à la comparaison d’ID pour qu’elle ne respecte pas la casse</span><span class="sxs-lookup"><span data-stu-id="655ae-1047">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="655ae-1048">Profil</span><span class="sxs-lookup"><span data-stu-id="655ae-1048">Profile</span></span>
* <span data-ttu-id="655ae-1049">Activation du compte de niveau locataire pour la fonctionnalité Managed Service Identity pour `login`</span><span class="sxs-lookup"><span data-stu-id="655ae-1049">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="655ae-1050">Réseau</span><span class="sxs-lookup"><span data-stu-id="655ae-1050">Network</span></span>
* <span data-ttu-id="655ae-1051">Correction d’un problème lié à `express-route update` où l’argument `--bandwidth` était ignoré</span><span class="sxs-lookup"><span data-stu-id="655ae-1051">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="655ae-1052">Correction d’un problème lié à `ddos-protection update` où set comprehension entraînait la génération d’un rapport des appels de procédure</span><span class="sxs-lookup"><span data-stu-id="655ae-1052">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="655ae-1053">Ressource</span><span class="sxs-lookup"><span data-stu-id="655ae-1053">Resource</span></span>
* <span data-ttu-id="655ae-1054">Ajout de la prise en charge du fichier de paramètres d’URI à `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="655ae-1054">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="655ae-1055">Ajout de la prise en charge de l’identité managée à `policy assignment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="655ae-1055">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="655ae-1056">Machine virtuelle SQL</span><span class="sxs-lookup"><span data-stu-id="655ae-1056">SQL Virtual Machine</span></span>
* <span data-ttu-id="655ae-1057">Préversion</span><span class="sxs-lookup"><span data-stu-id="655ae-1057">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="655ae-1058">Stockage</span><span class="sxs-lookup"><span data-stu-id="655ae-1058">Storage</span></span>
* <span data-ttu-id="655ae-1059">Changement d’une correction pour mettre à jour uniquement les propriétés modifiées sur le même objet</span><span class="sxs-lookup"><span data-stu-id="655ae-1059">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="655ae-1060">Correction (n° 8021). Les données binaires sont encodées au format base 64 quand elles sont retournées</span><span class="sxs-lookup"><span data-stu-id="655ae-1060">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="655ae-1061">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="655ae-1061">VM</span></span>
* <span data-ttu-id="655ae-1062">Changement apporté à `vm encryption enable` pour valider le coffre de clés de chiffrement de disque et vérifier l’existence du coffre de clés de chiffrement à clé</span><span class="sxs-lookup"><span data-stu-id="655ae-1062">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="655ae-1063">Ajout de l’indicateur `--force` à `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="655ae-1063">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="655ae-1064">15 janvier 2019</span><span class="sxs-lookup"><span data-stu-id="655ae-1064">January 15, 2019</span></span>

<span data-ttu-id="655ae-1065">Version 2.0.55</span><span class="sxs-lookup"><span data-stu-id="655ae-1065">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="655ae-1066">ACR</span><span class="sxs-lookup"><span data-stu-id="655ae-1066">ACR</span></span>
* <span data-ttu-id="655ae-1067">Changement apporté pour forcer l’envoi (push) d’un chart Helm qui n’existe pas</span><span class="sxs-lookup"><span data-stu-id="655ae-1067">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="655ae-1068">changement apporté pour autoriser les opérations de runtime sans requêtes ARM</span><span class="sxs-lookup"><span data-stu-id="655ae-1068">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="655ae-1069">[DÉPRÉCIATION] Dépréciation du paramètre `--resource-group` dans les commandes :</span><span class="sxs-lookup"><span data-stu-id="655ae-1069">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="655ae-1070">ACS</span><span class="sxs-lookup"><span data-stu-id="655ae-1070">ACS</span></span>
* <span data-ttu-id="655ae-1071">Ajout de la prise en charge des nouvelles régions ACI</span><span class="sxs-lookup"><span data-stu-id="655ae-1071">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="655ae-1072">AppService</span><span class="sxs-lookup"><span data-stu-id="655ae-1072">Appservice</span></span>
* <span data-ttu-id="655ae-1073">Correction d’un problème lié au chargement des certificats des applications hébergées sur un ASE, où ASE RG et App RG sont différents</span><span class="sxs-lookup"><span data-stu-id="655ae-1073">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="655ae-1074">Changement apporté à `webapp up` pour utiliser la référence (SKU) P1V1 en tant que valeur par défaut pour Linux</span><span class="sxs-lookup"><span data-stu-id="655ae-1074">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="655ae-1075">Correction apporté à `[webapp|functionapp] deployment source config-zip` pour afficher le message d’erreur approprié en cas d’échec d’un déploiement</span><span class="sxs-lookup"><span data-stu-id="655ae-1075">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="655ae-1076">Ajout de la commande `webapp ssh`</span><span class="sxs-lookup"><span data-stu-id="655ae-1076">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="655ae-1077">Botservice</span><span class="sxs-lookup"><span data-stu-id="655ae-1077">Botservice</span></span>
* <span data-ttu-id="655ae-1078">Ajout de mises à jour de l’état de déploiement à `bot create`</span><span class="sxs-lookup"><span data-stu-id="655ae-1078">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="655ae-1079">Configuration</span><span class="sxs-lookup"><span data-stu-id="655ae-1079">Configure</span></span>
* <span data-ttu-id="655ae-1080">Ajout de `none` en tant que format de sortie configurable</span><span class="sxs-lookup"><span data-stu-id="655ae-1080">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="655ae-1081">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="655ae-1081">CosmosDB</span></span>
* <span data-ttu-id="655ae-1082">Ajout de la prise en charge de la création d’une base de données avec débit partagé</span><span class="sxs-lookup"><span data-stu-id="655ae-1082">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="655ae-1083">HDInsight</span><span class="sxs-lookup"><span data-stu-id="655ae-1083">HDInsight</span></span>
* <span data-ttu-id="655ae-1084">Ajout de commandes pour la gestion des applications</span><span class="sxs-lookup"><span data-stu-id="655ae-1084">Added commands for managing applications</span></span>
* <span data-ttu-id="655ae-1085">Ajout de commandes pour la gestion des actions de script</span><span class="sxs-lookup"><span data-stu-id="655ae-1085">Added commands for managing script actions</span></span>
* <span data-ttu-id="655ae-1086">Ajout de commandes pour la gestion d’OMS (Operations Management Suite)</span><span class="sxs-lookup"><span data-stu-id="655ae-1086">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="655ae-1087">Ajout de la prise en charge permettant de lister l’utilisation régionale à `hdinsight list-usage`</span><span class="sxs-lookup"><span data-stu-id="655ae-1087">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="655ae-1088">[CHANGEMENT CASSANT] Suppression du type de cluster par défaut dans `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="655ae-1088">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="655ae-1089">Réseau</span><span class="sxs-lookup"><span data-stu-id="655ae-1089">Network</span></span>
* <span data-ttu-id="655ae-1090">Ajout des arguments `--custom-headers` et `--status-code-ranges` à `traffic-manager profile [create|update]`</span><span class="sxs-lookup"><span data-stu-id="655ae-1090">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="655ae-1091">Ajout de nouveaux types de routage : Sous-réseau et valeurs multiples</span><span class="sxs-lookup"><span data-stu-id="655ae-1091">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="655ae-1092">Ajout des arguments `--custom-headers` et `--subnets` à `traffic-manager endpoint [create|update]`</span><span class="sxs-lookup"><span data-stu-id="655ae-1092">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="655ae-1093">Correction du problème où la fourniture de `--vnets ""` à `ddos-protection update` provoquait une erreur</span><span class="sxs-lookup"><span data-stu-id="655ae-1093">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="655ae-1094">Role</span><span class="sxs-lookup"><span data-stu-id="655ae-1094">Role</span></span>
* <span data-ttu-id="655ae-1095">[DÉPRÉCIATION] Dépréciation de l’argument `--password` pour `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="655ae-1095">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="655ae-1096">Utilisation de mots de passe sécurisés générés par l’interface CLI à la place</span><span class="sxs-lookup"><span data-stu-id="655ae-1096">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="655ae-1097">Sécurité</span><span class="sxs-lookup"><span data-stu-id="655ae-1097">Security</span></span>
* <span data-ttu-id="655ae-1098">Version initiale</span><span class="sxs-lookup"><span data-stu-id="655ae-1098">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="655ae-1099">Stockage</span><span class="sxs-lookup"><span data-stu-id="655ae-1099">Storage</span></span>
* <span data-ttu-id="655ae-1100">[CHANGEMENT CASSANT] Changement apporté à `storage [blob|file|container|share] list` pour que le nombre par défaut de résultats soit de 5 000.</span><span class="sxs-lookup"><span data-stu-id="655ae-1100">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="655ae-1101">Utilisation de `--num-results *` pour que le comportement d’origine permette de retourner tous les résultats</span><span class="sxs-lookup"><span data-stu-id="655ae-1101">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="655ae-1102">Ajout du paramètre `--marker` pour `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="655ae-1102">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="655ae-1103">Ajout du marqueur de journal de la page suivante à STDERR pour `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="655ae-1103">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="655ae-1104">Ajout de la commande `storage blob service-properties update` avec prise en charge des sites web statiques</span><span class="sxs-lookup"><span data-stu-id="655ae-1104">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="655ae-1105">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="655ae-1105">VM</span></span>
* <span data-ttu-id="655ae-1106">Changement apporté à `vm [disk|unmanaged-disk]` et `vmss disk` pour avoir des paramètres plus cohérents</span><span class="sxs-lookup"><span data-stu-id="655ae-1106">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="655ae-1107">Ajout de la prise en charge du référencement d’images entre locataires à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="655ae-1107">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="655ae-1108">Résolution d’un bogue lié à la configuration par défaut dans `vm diagnostics get-default-config --windows-os`</span><span class="sxs-lookup"><span data-stu-id="655ae-1108">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="655ae-1109">Ajout de l’argument `--provision-after-extensions` à `vmss extension set` pour définir les extensions à provisionner avant de définir l’extension</span><span class="sxs-lookup"><span data-stu-id="655ae-1109">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="655ae-1110">Ajout de l’argument `--replica-count` à `sig image-version update` pour définir le nombre de réplications par défaut</span><span class="sxs-lookup"><span data-stu-id="655ae-1110">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="655ae-1111">Résolution d’un bogue lié à `image create --source` où le disque d’OS source est confondu avec une machine virtuelle portant le même nom, même si l’ID de ressource complet est fourni</span><span class="sxs-lookup"><span data-stu-id="655ae-1111">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="655ae-1112">20 décembre 2018</span><span class="sxs-lookup"><span data-stu-id="655ae-1112">December 20, 2018</span></span>

<span data-ttu-id="655ae-1113">Version 2.0.54</span><span class="sxs-lookup"><span data-stu-id="655ae-1113">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="655ae-1114">AppService</span><span class="sxs-lookup"><span data-stu-id="655ae-1114">Appservice</span></span>
* <span data-ttu-id="655ae-1115">Correction d’un problème qui causait l’échec du redéploiement pour `webapp up`</span><span class="sxs-lookup"><span data-stu-id="655ae-1115">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="655ae-1116">Ajout de la prise en charge du référencement et de la restauration des instantanés d’applications web</span><span class="sxs-lookup"><span data-stu-id="655ae-1116">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="655ae-1117">Ajout de la prise en charge pour l’indicateur `--runtime` aux applications de fonction Windows</span><span class="sxs-lookup"><span data-stu-id="655ae-1117">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="655ae-1118">IotCentral</span><span class="sxs-lookup"><span data-stu-id="655ae-1118">IoTCentral</span></span>
* <span data-ttu-id="655ae-1119">Correction de l’appel d’API des commandes de mise à jour</span><span class="sxs-lookup"><span data-stu-id="655ae-1119">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="655ae-1120">Role</span><span class="sxs-lookup"><span data-stu-id="655ae-1120">Role</span></span>
* <span data-ttu-id="655ae-1121">[CHANGEMENT CASSANT] Remplacement de `ad [app|sp] list` par une liste des 100 premiers objets par défaut uniquement</span><span class="sxs-lookup"><span data-stu-id="655ae-1121">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="655ae-1122">SQL</span><span class="sxs-lookup"><span data-stu-id="655ae-1122">SQL</span></span>
* <span data-ttu-id="655ae-1123">Ajout de la prise en charge du classement personnalisé sur les instances managées</span><span class="sxs-lookup"><span data-stu-id="655ae-1123">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="655ae-1124">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="655ae-1124">VM</span></span>
* <span data-ttu-id="655ae-1125">Ajout du paramètre `---os-type` pour `disk create`</span><span class="sxs-lookup"><span data-stu-id="655ae-1125">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="655ae-1126">18 décembre 2018</span><span class="sxs-lookup"><span data-stu-id="655ae-1126">December 18, 2018</span></span>

<span data-ttu-id="655ae-1127">Version 2.0.53</span><span class="sxs-lookup"><span data-stu-id="655ae-1127">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="655ae-1128">ACR</span><span class="sxs-lookup"><span data-stu-id="655ae-1128">ACR</span></span>
* <span data-ttu-id="655ae-1129">Ajout de la prise en charge de l’importation d’image à partir des registres de conteneurs externes</span><span class="sxs-lookup"><span data-stu-id="655ae-1129">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="655ae-1130">Condensé de la disposition du tableau pour la liste des tâches</span><span class="sxs-lookup"><span data-stu-id="655ae-1130">Condensed the table layout for task list</span></span>
* <span data-ttu-id="655ae-1131">Ajout de la prise en charge des URL Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="655ae-1131">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="655ae-1132">ACS</span><span class="sxs-lookup"><span data-stu-id="655ae-1132">ACS</span></span>
* <span data-ttu-id="655ae-1133">Ajout de l’aperçu des nœuds virtuels</span><span class="sxs-lookup"><span data-stu-id="655ae-1133">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="655ae-1134">Suppression du mot « (PRÉVERSION) » des arguments AAD pour `aks create`</span><span class="sxs-lookup"><span data-stu-id="655ae-1134">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="655ae-1135">[DÉPRÉCIATION] Dépréciation des commandes `az acs`.</span><span class="sxs-lookup"><span data-stu-id="655ae-1135">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="655ae-1136">Le service ACS sera mis hors service le 31 janvier 2020.</span><span class="sxs-lookup"><span data-stu-id="655ae-1136">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="655ae-1137">Ajout de la prise en charge de la stratégie de réseau lors de la création de clusters AKS</span><span class="sxs-lookup"><span data-stu-id="655ae-1137">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="655ae-1138">Suppression du caractère obligatoire de l’argument `--nodepool-name` pour `aks scale` s’il n’existe qu’un seul pool de nœuds</span><span class="sxs-lookup"><span data-stu-id="655ae-1138">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="655ae-1139">AppService</span><span class="sxs-lookup"><span data-stu-id="655ae-1139">Appservice</span></span>
* <span data-ttu-id="655ae-1140">Problème résolu quand `webapp config container` n’honore pas le paramètre `--slot`</span><span class="sxs-lookup"><span data-stu-id="655ae-1140">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="655ae-1141">Botservice</span><span class="sxs-lookup"><span data-stu-id="655ae-1141">Botservice</span></span>
* <span data-ttu-id="655ae-1142">Ajout de la prise en charge de l’analyse de fichier `.bot` lors de l’appel de `bot show`</span><span class="sxs-lookup"><span data-stu-id="655ae-1142">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="655ae-1143">Correction du bogue d’approvisionnement AppInsights</span><span class="sxs-lookup"><span data-stu-id="655ae-1143">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="655ae-1144">Correction du bogue d’espace blanc lors du traitement de chemins d’accès de fichier</span><span class="sxs-lookup"><span data-stu-id="655ae-1144">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="655ae-1145">Réduction des appels réseau Kudu</span><span class="sxs-lookup"><span data-stu-id="655ae-1145">Reduced Kudu network calls</span></span>
* <span data-ttu-id="655ae-1146">Amélioration de l’expérience utilisateur des commandes générales</span><span class="sxs-lookup"><span data-stu-id="655ae-1146">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="655ae-1147">Consommation</span><span class="sxs-lookup"><span data-stu-id="655ae-1147">Consumption</span></span>
* <span data-ttu-id="655ae-1148">Correction des bogues dans l’API de budget pour afficher les notifications</span><span class="sxs-lookup"><span data-stu-id="655ae-1148">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="655ae-1149">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="655ae-1149">CosmosDB</span></span>
* <span data-ttu-id="655ae-1150">Ajout de la prise en charge de la mise à jour de compte (multimaître vers maître unique)</span><span class="sxs-lookup"><span data-stu-id="655ae-1150">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="655ae-1151">Cartes</span><span class="sxs-lookup"><span data-stu-id="655ae-1151">Maps</span></span>
* <span data-ttu-id="655ae-1152">Ajout de la prise en charge de la référence (SKU) S1 pour `maps account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="655ae-1152">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="655ae-1153">Réseau</span><span class="sxs-lookup"><span data-stu-id="655ae-1153">Network</span></span>
* <span data-ttu-id="655ae-1154">Ajout de la prise en charge de `--format`, `--log-version` et `watcher flow-log configure`</span><span class="sxs-lookup"><span data-stu-id="655ae-1154">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="655ae-1155">Correction du problème avec `dns zone update`, où l’utilisation de "" pour effacer les réseaux virtuels de résolution d’inscription ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="655ae-1155">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="655ae-1156">Ressource</span><span class="sxs-lookup"><span data-stu-id="655ae-1156">Resource</span></span>
* <span data-ttu-id="655ae-1157">Correction de la gestion du paramètre d’étendue pour les groupes d’administration dans `policy assignment [create|list|delete|show|update]`</span><span class="sxs-lookup"><span data-stu-id="655ae-1157">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="655ae-1158">Ajout de la commande `resource wait`</span><span class="sxs-lookup"><span data-stu-id="655ae-1158">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="655ae-1159">Stockage</span><span class="sxs-lookup"><span data-stu-id="655ae-1159">Storage</span></span>
*  <span data-ttu-id="655ae-1160">Possibilité de mettre à jour la version de schéma de journal pour les services de stockage dans `storage logging update`</span><span class="sxs-lookup"><span data-stu-id="655ae-1160">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="655ae-1161">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="655ae-1161">VM</span></span>
* <span data-ttu-id="655ae-1162">Correction d’incident dans `vm identity remove`, lorsque la machine virtuelle spécifiée n’a aucune identité de service managé affectée</span><span class="sxs-lookup"><span data-stu-id="655ae-1162">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="655ae-1163">4 décembre 2018</span><span class="sxs-lookup"><span data-stu-id="655ae-1163">December 4, 2018</span></span>

<span data-ttu-id="655ae-1164">Version 2.0.52</span><span class="sxs-lookup"><span data-stu-id="655ae-1164">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="655ae-1165">Core</span><span class="sxs-lookup"><span data-stu-id="655ae-1165">Core</span></span>
* <span data-ttu-id="655ae-1166">L’approvisionnement des ressources entre locataires est désormais pris en charge pour le principal du service multi-locataire.</span><span class="sxs-lookup"><span data-stu-id="655ae-1166">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="655ae-1167">Les ID d’une commande avec sortie TSV n’étaient pas analysés correctement. Ce bogue a été corrigé.</span><span class="sxs-lookup"><span data-stu-id="655ae-1167">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="655ae-1168">AppService</span><span class="sxs-lookup"><span data-stu-id="655ae-1168">Appservice</span></span>
* <span data-ttu-id="655ae-1169">[APERÇU] Une commande `webapp up` a été ajoutée pour faciliter la création et le déploiement de contenu dans l’application.</span><span class="sxs-lookup"><span data-stu-id="655ae-1169">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="655ae-1170">Le bogue qui survenait sur les applications Windows basées sur des conteneurs en raison du changement de serveur principal a été corrigé.</span><span class="sxs-lookup"><span data-stu-id="655ae-1170">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="655ae-1171">Réseau</span><span class="sxs-lookup"><span data-stu-id="655ae-1171">Network</span></span>
* <span data-ttu-id="655ae-1172">L’argument `--exclusion` a été ajouté à `application-gateway waf-config set` pour prendre en charge les exclusions WAF</span><span class="sxs-lookup"><span data-stu-id="655ae-1172">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="655ae-1173">Role</span><span class="sxs-lookup"><span data-stu-id="655ae-1173">Role</span></span>
* <span data-ttu-id="655ae-1174">Les identificateurs personnalisés sont désormais pris en charge pour l’authentification par mot de passe.</span><span class="sxs-lookup"><span data-stu-id="655ae-1174">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="655ae-1175">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="655ae-1175">VM</span></span>
* <span data-ttu-id="655ae-1176">[DÉPRÉCIATION] Dépréciation du paramètre `vm extension [show|wait] --expand`</span><span class="sxs-lookup"><span data-stu-id="655ae-1176">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="655ae-1177">Le paramètre `--force` a été ajouté à `vm restart` pour redéployer les machines virtuelles qui ne répondent pas.</span><span class="sxs-lookup"><span data-stu-id="655ae-1177">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="655ae-1178">Le paramètre `[vm|vmss] create --authentication-type` a été modifié pour accepter la valeur « all » pour créer une machine virtuelle avec à la fois un mot de passe et une authentification SSH.</span><span class="sxs-lookup"><span data-stu-id="655ae-1178">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="655ae-1179">Le paramètre `image create --os-disk-caching` a été ajouté pour définir la mise en cache du disque du système d’exploitation pour une image.</span><span class="sxs-lookup"><span data-stu-id="655ae-1179">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="655ae-1180">20 novembre 2018</span><span class="sxs-lookup"><span data-stu-id="655ae-1180">November 20, 2018</span></span>

<span data-ttu-id="655ae-1181">Version 2.0.51</span><span class="sxs-lookup"><span data-stu-id="655ae-1181">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="655ae-1182">Core</span><span class="sxs-lookup"><span data-stu-id="655ae-1182">Core</span></span>
* <span data-ttu-id="655ae-1183">Modification du nom de connexion MSI pour ne pas réutiliser le nom d’abonnement dans une identité</span><span class="sxs-lookup"><span data-stu-id="655ae-1183">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="655ae-1184">ACR</span><span class="sxs-lookup"><span data-stu-id="655ae-1184">ACR</span></span>
* <span data-ttu-id="655ae-1185">Ajout d’un jeton de contexte à l’étape de tâche</span><span class="sxs-lookup"><span data-stu-id="655ae-1185">Added context token to task step</span></span>
* <span data-ttu-id="655ae-1186">Ajout de prise en charge pour la configuration des secrets dans acr run pour refléter acr task</span><span class="sxs-lookup"><span data-stu-id="655ae-1186">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="655ae-1187">Amélioration de la prise en charge de `--top` et `--orderby` pour les commandes `show-tags` et `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="655ae-1187">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="655ae-1188">AppService</span><span class="sxs-lookup"><span data-stu-id="655ae-1188">Appservice</span></span>
* <span data-ttu-id="655ae-1189">Augmentation du délai d’expiration par défaut du déploiement zip pour interroger l’état à 5 min, ce qui ajoute également une propriété de délai d’expiration pour personnaliser cette valeur</span><span class="sxs-lookup"><span data-stu-id="655ae-1189">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="655ae-1190">Mise à jour de la valeur par défaut `node_version`.</span><span class="sxs-lookup"><span data-stu-id="655ae-1190">Updated the default `node_version`.</span></span> <span data-ttu-id="655ae-1191">La réinitialisation d’une action d’échange d’emplacements pendant un échange en deux phases conserve toutes les chaînes de connexion et paramètres d’application</span><span class="sxs-lookup"><span data-stu-id="655ae-1191">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="655ae-1192">Suppression de la vérification de référence SKU côté client pour app service plan create de Linux</span><span class="sxs-lookup"><span data-stu-id="655ae-1192">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="655ae-1193">Correction de l’erreur qui survenait lors de tentatives d’obtention de l’état zipdeploy</span><span class="sxs-lookup"><span data-stu-id="655ae-1193">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="655ae-1194">IotCentral</span><span class="sxs-lookup"><span data-stu-id="655ae-1194">IotCentral</span></span>
* <span data-ttu-id="655ae-1195">Ajouter de la vérification de disponibilité du sous-domaine lors de la création d’une application IoT Central</span><span class="sxs-lookup"><span data-stu-id="655ae-1195">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="655ae-1196">KeyVault</span><span class="sxs-lookup"><span data-stu-id="655ae-1196">KeyVault</span></span>
* <span data-ttu-id="655ae-1197">Correction du bogue dans lequel des erreurs pouvaient avoir été ignorées</span><span class="sxs-lookup"><span data-stu-id="655ae-1197">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="655ae-1198">Réseau</span><span class="sxs-lookup"><span data-stu-id="655ae-1198">Network</span></span>
* <span data-ttu-id="655ae-1199">Ajout de sous-commandes `root-cert` à `application-gateway` pour traiter les certificats racine de confiance</span><span class="sxs-lookup"><span data-stu-id="655ae-1199">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="655ae-1200">Ajout des options `--min-capacity` et `--custom-error-pages` à `application-gateway [create|update]` :</span><span class="sxs-lookup"><span data-stu-id="655ae-1200">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="655ae-1201">Ajout de `--zones` pour la prise en charge de zone de disponibilité à `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="655ae-1201">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="655ae-1202">Ajout des arguments `--file-upload-limit`, `--max-request-body-size` et `--request-body-check` à `application-gateway waf-config set`</span><span class="sxs-lookup"><span data-stu-id="655ae-1202">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="655ae-1203">Rdbms</span><span class="sxs-lookup"><span data-stu-id="655ae-1203">Rdbms</span></span>
* <span data-ttu-id="655ae-1204">Ajouts de commandes mariadb vnet</span><span class="sxs-lookup"><span data-stu-id="655ae-1204">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="655ae-1205">Contrôle d’accès en fonction du rôle (RBAC)</span><span class="sxs-lookup"><span data-stu-id="655ae-1205">Rbac</span></span>
* <span data-ttu-id="655ae-1206">Résolution d’un problème qui survenait lors de tentatives de mise à jour d’informations d’identification immuables dans `ad app update`</span><span class="sxs-lookup"><span data-stu-id="655ae-1206">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="655ae-1207">Ajout d’avertissements de sortie pour indiquer des changements cassants dans un futur proche pour `ad [app|sp] list`</span><span class="sxs-lookup"><span data-stu-id="655ae-1207">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="655ae-1208">Stockage</span><span class="sxs-lookup"><span data-stu-id="655ae-1208">Storage</span></span>
* <span data-ttu-id="655ae-1209">Amélioration du traitement des « corner cases » pour les commandes de copie de stockage</span><span class="sxs-lookup"><span data-stu-id="655ae-1209">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="655ae-1210">Résolution d’un problème où `storage blob copy start-batch` n’utilisait pas les informations d’identification de connexion lorsque les comptes source et de destination étaient identiques</span><span class="sxs-lookup"><span data-stu-id="655ae-1210">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="655ae-1211">Correction du bogue avec `storage [blob|file] url` où `sas_token` n’était pas intégré dans l’URL</span><span class="sxs-lookup"><span data-stu-id="655ae-1211">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="655ae-1212">Ajout d’un avertissement de changement cassant à `[blob|container] list` : bientôt, seuls les 5 000 premiers résultats seront affichés par défaut dans la sortie</span><span class="sxs-lookup"><span data-stu-id="655ae-1212">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="655ae-1213">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="655ae-1213">VM</span></span>
* <span data-ttu-id="655ae-1214">Ajout de la prise en charge de `[vm|vmss] create --storage-sku` pour spécifier la référence SKU de compte de stockage pour les disques de données et de système d’exploitation managés de façon distincte</span><span class="sxs-lookup"><span data-stu-id="655ae-1214">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="655ae-1215">Remplacement des paramètres de nom de version `sig image-version` par `--image-version -e`</span><span class="sxs-lookup"><span data-stu-id="655ae-1215">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="655ae-1216">Version déconseillée de la valeur `--image-version-name` d’argument `sig image-version` remplacée par `--image-version`</span><span class="sxs-lookup"><span data-stu-id="655ae-1216">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="655ae-1217">Ajout de la prise en charge pour utiliser le disque de système d’exploitation local pour `[vm|vmss] create --ephemeral-os-disk`</span><span class="sxs-lookup"><span data-stu-id="655ae-1217">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="655ae-1218">Ajout de la prise en charge de `--no-wait` pour `snapshot create/update`</span><span class="sxs-lookup"><span data-stu-id="655ae-1218">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="655ae-1219">Ajout de la commande `snapshot wait`</span><span class="sxs-lookup"><span data-stu-id="655ae-1219">Added `snapshot wait` command</span></span>
* <span data-ttu-id="655ae-1220">Ajout de la prise en charge pour utiliser le nom d’instance avec `[vm|vmss] extension set --extension-instance-name`</span><span class="sxs-lookup"><span data-stu-id="655ae-1220">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="655ae-1221">6 novembre 2018</span><span class="sxs-lookup"><span data-stu-id="655ae-1221">November 6, 2018</span></span>

<span data-ttu-id="655ae-1222">Version 2.0.50</span><span class="sxs-lookup"><span data-stu-id="655ae-1222">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="655ae-1223">Core</span><span class="sxs-lookup"><span data-stu-id="655ae-1223">Core</span></span>
* <span data-ttu-id="655ae-1224">Ajout de la prise en charge pour le principal de service sn+issuer auth</span><span class="sxs-lookup"><span data-stu-id="655ae-1224">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="655ae-1225">ACR</span><span class="sxs-lookup"><span data-stu-id="655ae-1225">ACR</span></span>
* <span data-ttu-id="655ae-1226">Ajout de la prise en charge pour les événements git de demande d’envoi et de tirage pour le déclencheur de tâche source</span><span class="sxs-lookup"><span data-stu-id="655ae-1226">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="655ae-1227">Modification de l’utilisation de fichiers Dockerfile par défaut s’il n’est pas spécifié dans la commande build</span><span class="sxs-lookup"><span data-stu-id="655ae-1227">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="655ae-1228">ACS</span><span class="sxs-lookup"><span data-stu-id="655ae-1228">ACS</span></span>
* <span data-ttu-id="655ae-1229">[Changement cassant] : `enable_cloud_console_aks_browse` supprimé pour activer « az aks browse » par défaut</span><span class="sxs-lookup"><span data-stu-id="655ae-1229">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="655ae-1230">Advisor</span><span class="sxs-lookup"><span data-stu-id="655ae-1230">Advisor</span></span>
* <span data-ttu-id="655ae-1231">Version mise à la disposition générale</span><span class="sxs-lookup"><span data-stu-id="655ae-1231">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="655ae-1232">AMS</span><span class="sxs-lookup"><span data-stu-id="655ae-1232">AMS</span></span>
* <span data-ttu-id="655ae-1233">Ajout de nouveaux groupes de commandes :</span><span class="sxs-lookup"><span data-stu-id="655ae-1233">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="655ae-1234">Ajout de nouvelles commandes :</span><span class="sxs-lookup"><span data-stu-id="655ae-1234">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="655ae-1235">Ajout de la prise en charge des paramètres de chiffrement de `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="655ae-1235">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="655ae-1236">Ajout de la prise en charge de `ams transform output remove` qui peut désormais être effectuée en transmettant le chemin de l’index pour le supprimer</span><span class="sxs-lookup"><span data-stu-id="655ae-1236">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="655ae-1237">Ajout des arguments `--correlation-data` et `--label` au groupe de commandes `ams job`</span><span class="sxs-lookup"><span data-stu-id="655ae-1237">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="655ae-1238">Ajout des arguments `--storage-account` et `--container` au groupe de commandes `ams asset`</span><span class="sxs-lookup"><span data-stu-id="655ae-1238">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="655ae-1239">Ajout des valeurs par défaut pour le délai d’expiration (présent + 23h) et les autorisations (lecture) dans la commande `ams asset get-sas-url`</span><span class="sxs-lookup"><span data-stu-id="655ae-1239">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="655ae-1240">[Changement cassant] : commande `ams streaming locator` remplacée par `ams streaming-locator`</span><span class="sxs-lookup"><span data-stu-id="655ae-1240">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="655ae-1241">[Changement cassant] : mise à jour de l’argument `--content-keys` de `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="655ae-1241">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="655ae-1242">[Changement cassant] : `--content-policy-name` renommé en `--content-key-policy-name` dans la commande `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="655ae-1242">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="655ae-1243">[Changement cassant] : remplacer la commande `ams streaming policy` par `ams streaming-policy`</span><span class="sxs-lookup"><span data-stu-id="655ae-1243">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="655ae-1244">[Changement cassant] : argument `--preset-names` remplacé par `--preset` dans le groupe de commandes `ams transform`.</span><span class="sxs-lookup"><span data-stu-id="655ae-1244">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="655ae-1245">À présent vous ne pouvez définir qu’une sortie/présélection à la fois (pour en ajouter d’autres, vous devez exécuter `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="655ae-1245">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="655ae-1246">En outre, vous pouvez définir StandardEncoderPreset de façon personnalisée en transmettant le chemin à votre JSON personnalisé</span><span class="sxs-lookup"><span data-stu-id="655ae-1246">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="655ae-1247">[Changement cassant] : `--output-asset-names ` renommé en `--output-assets` dans la commande `ams job start`.</span><span class="sxs-lookup"><span data-stu-id="655ae-1247">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="655ae-1248">Il accepte désormais une liste de ressources séparée par des espaces au format « assetName=label ».</span><span class="sxs-lookup"><span data-stu-id="655ae-1248">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="655ae-1249">Une ressource sans étiquette peut être envoyée comme ceci : « assetName= »</span><span class="sxs-lookup"><span data-stu-id="655ae-1249">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="655ae-1250">AppService</span><span class="sxs-lookup"><span data-stu-id="655ae-1250">AppService</span></span>
* <span data-ttu-id="655ae-1251">Correction d’un bogue dans `az webapp config backup update` qui empêche de définir une planification de sauvegarde si elle n’est pas déjà définie</span><span class="sxs-lookup"><span data-stu-id="655ae-1251">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="655ae-1252">Configuration</span><span class="sxs-lookup"><span data-stu-id="655ae-1252">Configure</span></span>
* <span data-ttu-id="655ae-1253">Ajout de YAML aux options de format de sortie</span><span class="sxs-lookup"><span data-stu-id="655ae-1253">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="655ae-1254">Conteneur</span><span class="sxs-lookup"><span data-stu-id="655ae-1254">Container</span></span>
* <span data-ttu-id="655ae-1255">Modification pour afficher l’identité lors de l’exportation d’un groupe de conteneurs vers yaml</span><span class="sxs-lookup"><span data-stu-id="655ae-1255">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="655ae-1256">Event Hub</span><span class="sxs-lookup"><span data-stu-id="655ae-1256">EventHub</span></span>
* <span data-ttu-id="655ae-1257">Ajout d’un indicateur `--enable-kafka` pour prendre en charge Kafka dans `eventhub namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="655ae-1257">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="655ae-1258">Interactive</span><span class="sxs-lookup"><span data-stu-id="655ae-1258">Interactive</span></span>
* <span data-ttu-id="655ae-1259">Interactive installe maintenant l’extension `interactive`, ce qui permettra des mises à jour et prises en charge plus rapides</span><span class="sxs-lookup"><span data-stu-id="655ae-1259">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="655ae-1260">Surveiller</span><span class="sxs-lookup"><span data-stu-id="655ae-1260">Monitor</span></span>
* <span data-ttu-id="655ae-1261">Ajout de la prise en charge pour les noms de métriques qui incluent les caractères barre oblique (/) et point (.) à `--condition` dans `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="655ae-1261">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="655ae-1262">Réseau</span><span class="sxs-lookup"><span data-stu-id="655ae-1262">Network</span></span>
* <span data-ttu-id="655ae-1263">Noms de commande `network interface-endpoint` déconseillés en faveur de `network private-endpoint`</span><span class="sxs-lookup"><span data-stu-id="655ae-1263">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="655ae-1264">Problème résolu à l’endroit où l’argument `--peer-circuit` n’accepte pas d’ID dans `express-route peering connection create`</span><span class="sxs-lookup"><span data-stu-id="655ae-1264">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="655ae-1265">Problème résolu à l’endroit où `--ip-tags` ne fonctionnait pas correctement avec `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="655ae-1265">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="655ae-1266">Profil</span><span class="sxs-lookup"><span data-stu-id="655ae-1266">Profile</span></span>
* <span data-ttu-id="655ae-1267">Ajout de `--use-cert-sn-issuer` à `az login` pour la connexion principale du service à l’aide du certificat de déploiement automatique</span><span class="sxs-lookup"><span data-stu-id="655ae-1267">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="655ae-1268">SGBDR</span><span class="sxs-lookup"><span data-stu-id="655ae-1268">RDBMS</span></span>
* <span data-ttu-id="655ae-1269">Ajout de commandes de réplica mysql</span><span class="sxs-lookup"><span data-stu-id="655ae-1269">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="655ae-1270">Ressource</span><span class="sxs-lookup"><span data-stu-id="655ae-1270">Resource</span></span>
* <span data-ttu-id="655ae-1271">Ajout de la prise en charge pour les groupes d’administration et les abonnements aux commandes `policy definition|set-definition`</span><span class="sxs-lookup"><span data-stu-id="655ae-1271">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="655ae-1272">Role</span><span class="sxs-lookup"><span data-stu-id="655ae-1272">Role</span></span>
* <span data-ttu-id="655ae-1273">Ajout de la prise en charge pour la gestion d’autorisation API, les utilisateurs connectés ainsi que la gestion des mots de passe et informations d’identification des certificats de l’application</span><span class="sxs-lookup"><span data-stu-id="655ae-1273">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="655ae-1274">Modification de `ad sp create-for-rbac` pour clarifier la confusion entre displayName et le nom de principal du service</span><span class="sxs-lookup"><span data-stu-id="655ae-1274">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="655ae-1275">Ajout de la prise en charge pour attribuer les autorisations aux applications AAD</span><span class="sxs-lookup"><span data-stu-id="655ae-1275">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="655ae-1276">Stockage</span><span class="sxs-lookup"><span data-stu-id="655ae-1276">Storage</span></span>
* <span data-ttu-id="655ae-1277">Ajout de la prise en charge pour vous connecter aux services de stockage uniquement avec les signatures d’accès partagé et les points de terminaison (sans nom de compte ou clé), comme décrit dans `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span><span class="sxs-lookup"><span data-stu-id="655ae-1277">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="655ae-1278">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="655ae-1278">VM</span></span>
* <span data-ttu-id="655ae-1279">Ajout de l’argument `storage-sku` à `image create` pour définir le type de compte de stockage par défaut de l’image</span><span class="sxs-lookup"><span data-stu-id="655ae-1279">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="655ae-1280">Correction du bogue avec `vm resize` à l’endroit où l’option `--no-wait` a entraîné un incident avec la commande</span><span class="sxs-lookup"><span data-stu-id="655ae-1280">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="655ae-1281">Modification du format de sortie de la table `vm encryption show` pour afficher l’état</span><span class="sxs-lookup"><span data-stu-id="655ae-1281">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="655ae-1282">Modification de `vm secret format` pour exiger la sortie json/jsonc</span><span class="sxs-lookup"><span data-stu-id="655ae-1282">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="655ae-1283">Avertit l’utilisateur et les valeurs par défaut à la sortie json si un format de sortie indésirable est sélectionné</span><span class="sxs-lookup"><span data-stu-id="655ae-1283">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="655ae-1284">Amélioration de la validation de l’argument pour `vm create --image`</span><span class="sxs-lookup"><span data-stu-id="655ae-1284">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="655ae-1285">23 octobre 2018</span><span class="sxs-lookup"><span data-stu-id="655ae-1285">October 23, 2018</span></span>

<span data-ttu-id="655ae-1286">Version 2.0.49</span><span class="sxs-lookup"><span data-stu-id="655ae-1286">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="655ae-1287">Core</span><span class="sxs-lookup"><span data-stu-id="655ae-1287">Core</span></span>
* <span data-ttu-id="655ae-1288">Correction du problème avec `--ids` où `--subscription` serait prioritaire sur l’abonnement dans `--ids`</span><span class="sxs-lookup"><span data-stu-id="655ae-1288">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="655ae-1289">Ajout d’avertissements explicites lorsque les paramètres sont ignorés par `--ids`</span><span class="sxs-lookup"><span data-stu-id="655ae-1289">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="655ae-1290">ACR</span><span class="sxs-lookup"><span data-stu-id="655ae-1290">ACR</span></span>
* <span data-ttu-id="655ae-1291">Correction d’un problème de codage ACR Build dans Python2</span><span class="sxs-lookup"><span data-stu-id="655ae-1291">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="655ae-1292">CDN</span><span class="sxs-lookup"><span data-stu-id="655ae-1292">CDN</span></span>
* <span data-ttu-id="655ae-1293">[CHANGEMENT CASSANT] Modification du comportement de mise en cache de chaîne de requête par défaut de `cdn endpoint create` afin que ce ne soit plus « IgnoreQueryString » par défaut.</span><span class="sxs-lookup"><span data-stu-id="655ae-1293">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="655ae-1294">Il est maintenant défini par le service</span><span class="sxs-lookup"><span data-stu-id="655ae-1294">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="655ae-1295">Conteneur</span><span class="sxs-lookup"><span data-stu-id="655ae-1295">Container</span></span>
* <span data-ttu-id="655ae-1296">Ajout de `Private` comme un type valide pour passer à «--ip-address»</span><span class="sxs-lookup"><span data-stu-id="655ae-1296">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="655ae-1297">Modification pour permettre l’utilisation d’un seul ID de sous-réseau pour configurer un réseau virtuel pour le groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="655ae-1297">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="655ae-1298">Modification pour permettre l’utilisation d’un nom de réseau virtuel ou d’un ID de ressource pour permettre l’utilisation de réseaux virtuels à partir de groupes de ressources différents</span><span class="sxs-lookup"><span data-stu-id="655ae-1298">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="655ae-1299">Ajout de `--assign-identity` pour ajouter une identité MSI à un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="655ae-1299">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="655ae-1300">Ajout de `--scope` pour créer une attribution de rôle pour l’identité MSI attribuée par le système</span><span class="sxs-lookup"><span data-stu-id="655ae-1300">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="655ae-1301">Ajout d’un avertissement lors de la création d’un groupe de conteneurs avec une image sans processus à long terme</span><span class="sxs-lookup"><span data-stu-id="655ae-1301">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="655ae-1302">Correction de problèmes de sortie de table pour les commandes `list` et `show`</span><span class="sxs-lookup"><span data-stu-id="655ae-1302">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="655ae-1303">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="655ae-1303">CosmosDB</span></span>
* <span data-ttu-id="655ae-1304">Ajout de la prise en charge de `--enable-multiple-write-locations` pour `cosmosdb create`</span><span class="sxs-lookup"><span data-stu-id="655ae-1304">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="655ae-1305">Interactive</span><span class="sxs-lookup"><span data-stu-id="655ae-1305">Interactive</span></span>
* <span data-ttu-id="655ae-1306">Modifié pour assurer l’apparition du paramètre d’abonnement global dans les paramètres</span><span class="sxs-lookup"><span data-stu-id="655ae-1306">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="655ae-1307">IoT Central</span><span class="sxs-lookup"><span data-stu-id="655ae-1307">IoT Central</span></span>
* <span data-ttu-id="655ae-1308">Ajout d’options de modèle et de nom d’affichage pour la création de l’application IoT central</span><span class="sxs-lookup"><span data-stu-id="655ae-1308">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="655ae-1309">[CHANGEMENT CASSANT] Suppression de la prise en charge de la référence SKU F1, utilisez la référence SKU S1 à la place</span><span class="sxs-lookup"><span data-stu-id="655ae-1309">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="655ae-1310">Surveiller</span><span class="sxs-lookup"><span data-stu-id="655ae-1310">Monitor</span></span>
* <span data-ttu-id="655ae-1311">Change en `monitor activity-log list` :</span><span class="sxs-lookup"><span data-stu-id="655ae-1311">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="655ae-1312">Prise en charge ajoutée pour répertorier tous les événements au niveau de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="655ae-1312">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="655ae-1313">Ajout du paramètre `--offset` pour créer plus facilement des requêtes de temps</span><span class="sxs-lookup"><span data-stu-id="655ae-1313">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="655ae-1314">Amélioration de la validation pour `--start-time` et `--end-time` pour utiliser des plages de formats ISO8601 plus larges et des formats dateHeure plus conviviaux</span><span class="sxs-lookup"><span data-stu-id="655ae-1314">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="655ae-1315">Ajout de `--namespace` comme alias pour l’option déconseillée `--resource-provider`</span><span class="sxs-lookup"><span data-stu-id="655ae-1315">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="655ae-1316">`--filters` déconseillé, car aucune valeur autre que celles avec des options fortement typées ne sont prises en charge par le service</span><span class="sxs-lookup"><span data-stu-id="655ae-1316">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="655ae-1317">Change en `monitor metrics list` :</span><span class="sxs-lookup"><span data-stu-id="655ae-1317">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="655ae-1318">Ajout du paramètre `--offset` pour créer plus facilement des requêtes de temps</span><span class="sxs-lookup"><span data-stu-id="655ae-1318">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="655ae-1319">Amélioration de la validation pour `--start-time` et `--end-time` pour utiliser des plages de formats ISO8601 plus larges et des formats dateHeure plus conviviaux</span><span class="sxs-lookup"><span data-stu-id="655ae-1319">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="655ae-1320">Amélioration de la validation pour les arguments `--event-hub` et `--event-hub-rule` à `monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="655ae-1320">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="655ae-1321">Réseau</span><span class="sxs-lookup"><span data-stu-id="655ae-1321">Network</span></span>
* <span data-ttu-id="655ae-1322">Ajout des arguments `--app-gateway-address-pools` et `--gateway-name` à `nic create`, pour prendre en charge l’ajout de pools d’adresses principaux Application Gateway à une carte réseau</span><span class="sxs-lookup"><span data-stu-id="655ae-1322">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="655ae-1323">Ajout des arguments `--app-gateway-address-pools` et `--gateway-name` à `nic ip-config create/update`, pour prendre en charge l’ajout de pools d’adresses principaux Application Gateway à une carte réseau</span><span class="sxs-lookup"><span data-stu-id="655ae-1323">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="655ae-1324">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="655ae-1324">ServiceBus</span></span>
* <span data-ttu-id="655ae-1325">Ajout de `migration_state` en lecture seule à MigrationConfigProperties pour afficher l’état actuel de migration d’espace de noms Standard à Premium de Service Bus</span><span class="sxs-lookup"><span data-stu-id="655ae-1325">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="655ae-1326">SQL</span><span class="sxs-lookup"><span data-stu-id="655ae-1326">SQL</span></span>
* <span data-ttu-id="655ae-1327">`sql failover-group create` et `sql failover-group update` corrigés pour fonctionner avec la stratégie de basculement manuel</span><span class="sxs-lookup"><span data-stu-id="655ae-1327">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="655ae-1328">Stockage</span><span class="sxs-lookup"><span data-stu-id="655ae-1328">Storage</span></span>
* <span data-ttu-id="655ae-1329">Formatage de sortie de `az storage cors list` corrigé, tous les éléments affichent une clé de « Service » correcte</span><span class="sxs-lookup"><span data-stu-id="655ae-1329">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="655ae-1330">Ajout du paramètre `--bypass-immutability-policy` pour la suppression du conteneur de stratégie d’immuabilité bloquée</span><span class="sxs-lookup"><span data-stu-id="655ae-1330">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="655ae-1331">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="655ae-1331">VM</span></span>
* <span data-ttu-id="655ae-1332">Mode de mise en cache configuré sur `None` pour la série de machines Lv/Lv2 dans `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="655ae-1332">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="655ae-1333">Mise à jour de la liste des tailles prises en charge, prenant en charge l’accélérateur de mise en réseau pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="655ae-1333">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="655ae-1334">Ajout des arguments fortement typés pour les configurations d’E/S et Mbits/s Ultrassd pour `disk create`</span><span class="sxs-lookup"><span data-stu-id="655ae-1334">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="655ae-1335">16 octobre 2018</span><span class="sxs-lookup"><span data-stu-id="655ae-1335">October 16, 2018</span></span>

<span data-ttu-id="655ae-1336">Version 2.0.48</span><span class="sxs-lookup"><span data-stu-id="655ae-1336">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="655ae-1337">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="655ae-1337">VM</span></span>
* <span data-ttu-id="655ae-1338">Résolution du problème de kit de développement logiciel qui a provoqué l’échec d’installation de Homebrew</span><span class="sxs-lookup"><span data-stu-id="655ae-1338">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="655ae-1339">9 octobre 2018</span><span class="sxs-lookup"><span data-stu-id="655ae-1339">October 9, 2018</span></span>

<span data-ttu-id="655ae-1340">Version 2.0.47</span><span class="sxs-lookup"><span data-stu-id="655ae-1340">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="655ae-1341">Core</span><span class="sxs-lookup"><span data-stu-id="655ae-1341">Core</span></span>
* <span data-ttu-id="655ae-1342">Gestion améliorée des erreurs « Demande incorrecte »</span><span class="sxs-lookup"><span data-stu-id="655ae-1342">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="655ae-1343">ACR</span><span class="sxs-lookup"><span data-stu-id="655ae-1343">ACR</span></span>
* <span data-ttu-id="655ae-1344">Prise en charge de format de tableau similaire, comme le client helm</span><span class="sxs-lookup"><span data-stu-id="655ae-1344">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="655ae-1345">ACS</span><span class="sxs-lookup"><span data-stu-id="655ae-1345">ACS</span></span>
* <span data-ttu-id="655ae-1346">Ajout de `aks [create|scale] --nodepool-name` pour configurer le nom du pool de nœuds, tronqué à 12 caractères, par défaut : nodepool1</span><span class="sxs-lookup"><span data-stu-id="655ae-1346">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="655ae-1347">Correction d’une erreur pour revenir à « scp » lorsque Parimiko échoue</span><span class="sxs-lookup"><span data-stu-id="655ae-1347">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="655ae-1348">Modification de `aks create` pour ne plus nécessiter `--aad-tenant-id`</span><span class="sxs-lookup"><span data-stu-id="655ae-1348">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="655ae-1349">Fusion améliorée des informations d'identification Kubernetes lorsque des entrées dupliquées sont présentes</span><span class="sxs-lookup"><span data-stu-id="655ae-1349">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="655ae-1350">Conteneur</span><span class="sxs-lookup"><span data-stu-id="655ae-1350">Container</span></span>
* <span data-ttu-id="655ae-1351">Modification de `functionapp create` pour prendre en charge la création d’un type de plan de consommation Linux avec un runtime spécifique</span><span class="sxs-lookup"><span data-stu-id="655ae-1351">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="655ae-1352">[PRÉVERSION] Prise en charge de l’hébergement d’applications web sur les conteneurs Windows</span><span class="sxs-lookup"><span data-stu-id="655ae-1352">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="655ae-1353">Event Hub</span><span class="sxs-lookup"><span data-stu-id="655ae-1353">Event Hub</span></span>
* <span data-ttu-id="655ae-1354">Correction de la commande `eventhub update`</span><span class="sxs-lookup"><span data-stu-id="655ae-1354">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="655ae-1355">[CHANGEMENT CASSANT] Modification des commandes `list` pour gérer des erreurs resource(s) NotFound(404) d’une manière habituelle au lieu d’afficher une liste vide</span><span class="sxs-lookup"><span data-stu-id="655ae-1355">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="655ae-1356">Extensions</span><span class="sxs-lookup"><span data-stu-id="655ae-1356">Extensions</span></span>
* <span data-ttu-id="655ae-1357">Correction d’une erreur de tentative d’ajout d’une extension déjà installée</span><span class="sxs-lookup"><span data-stu-id="655ae-1357">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="655ae-1358">HDInsight</span><span class="sxs-lookup"><span data-stu-id="655ae-1358">HDInsight</span></span>
* <span data-ttu-id="655ae-1359">Version initiale</span><span class="sxs-lookup"><span data-stu-id="655ae-1359">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="655ae-1360">IoT</span><span class="sxs-lookup"><span data-stu-id="655ae-1360">IoT</span></span>
* <span data-ttu-id="655ae-1361">Ajout de la commande d’installation de l’extension à une bannière pour la première exécution</span><span class="sxs-lookup"><span data-stu-id="655ae-1361">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="655ae-1362">KeyVault</span><span class="sxs-lookup"><span data-stu-id="655ae-1362">KeyVault</span></span>
* <span data-ttu-id="655ae-1363">Modification pour restreindre les commandes de stockage keyvault au dernier profil API</span><span class="sxs-lookup"><span data-stu-id="655ae-1363">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="655ae-1364">Réseau</span><span class="sxs-lookup"><span data-stu-id="655ae-1364">Network</span></span>
* <span data-ttu-id="655ae-1365">Correction de `network dns zone create` : la commande réussit même si l’utilisateur a configuré un emplacement par défaut.</span><span class="sxs-lookup"><span data-stu-id="655ae-1365">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="655ae-1366">Voir #6052</span><span class="sxs-lookup"><span data-stu-id="655ae-1366">See #6052</span></span>
* <span data-ttu-id="655ae-1367">Remplacement de `--remote-vnet-id` pour `network vnet peering create`</span><span class="sxs-lookup"><span data-stu-id="655ae-1367">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="655ae-1368">Ajout de `--remote-vnet` à `network vnet peering create`, qui accepte un nom ou ID</span><span class="sxs-lookup"><span data-stu-id="655ae-1368">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="655ae-1369">Prise en charge de multiples préfixes de sous-réseau pour `network vnet create` avec `--subnet-prefixes`</span><span class="sxs-lookup"><span data-stu-id="655ae-1369">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="655ae-1370">Prise en charge de multiple préfixes de sous-réseau pour `network vnet subnet [create|update]` avec `--address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="655ae-1370">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="655ae-1371">Correction d’une erreur relative à `network application-gateway create` qui empêchait la création de passerelles avec les références SKU `WAF_v2` ou `Standard_v2`</span><span class="sxs-lookup"><span data-stu-id="655ae-1371">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="655ae-1372">Ajout de l’argument d’usage `--service-endpoint-policy` à `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="655ae-1372">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="655ae-1373">Role</span><span class="sxs-lookup"><span data-stu-id="655ae-1373">Role</span></span>
* <span data-ttu-id="655ae-1374">Prise en charge du listing des propriétaires d’applications Azure AD à `ad app owner`</span><span class="sxs-lookup"><span data-stu-id="655ae-1374">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="655ae-1375">Prise en charge du listing des propriétaires de principaux de service Azure AD à `ad sp owner`</span><span class="sxs-lookup"><span data-stu-id="655ae-1375">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="655ae-1376">Modification pour garantir que les commandes de mise à jour et de création de définition de rôle acceptent les configurations à autorisations multiples</span><span class="sxs-lookup"><span data-stu-id="655ae-1376">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="655ae-1377">Modification de `ad sp create-for-rbac` pour garantir que l’URI de la page d’accueil est toujours « https »</span><span class="sxs-lookup"><span data-stu-id="655ae-1377">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="655ae-1378">Service Bus</span><span class="sxs-lookup"><span data-stu-id="655ae-1378">Service Bus</span></span>
* <span data-ttu-id="655ae-1379">[CHANGEMENT CASSANT] Modification des commandes `list` pour gérer des erreurs resource(s) NotFound(404) d’une manière habituelle au lieu d’afficher une liste vide</span><span class="sxs-lookup"><span data-stu-id="655ae-1379">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="655ae-1380">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="655ae-1380">VM</span></span>
* <span data-ttu-id="655ae-1381">Correction du champ vide `accessSas` dans `disk grant-access`</span><span class="sxs-lookup"><span data-stu-id="655ae-1381">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="655ae-1382">Modification de `vmss create` pour réserver une plage de port de frontend assez large pour gérer le surprovisionnement</span><span class="sxs-lookup"><span data-stu-id="655ae-1382">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="655ae-1383">Correction des commandes de mise à jour pour `sig`</span><span class="sxs-lookup"><span data-stu-id="655ae-1383">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="655ae-1384">Prise en charge `--no-wait` de la gestion de versions d’images dans `sig`</span><span class="sxs-lookup"><span data-stu-id="655ae-1384">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="655ae-1385">Modification de `vm list-ip-addresses` pour afficher la zone de disponibilité des adresses IP publiques</span><span class="sxs-lookup"><span data-stu-id="655ae-1385">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="655ae-1386">Modification de `[vm|vmss] disk attach` pour définir le numéro d’identité logique (LUN) par défaut du disque sur le premier emplacement disponible</span><span class="sxs-lookup"><span data-stu-id="655ae-1386">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="655ae-1387">21 septembre 2018</span><span class="sxs-lookup"><span data-stu-id="655ae-1387">September 21, 2018</span></span>

<span data-ttu-id="655ae-1388">Version 2.0.46</span><span class="sxs-lookup"><span data-stu-id="655ae-1388">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="655ae-1389">ACR</span><span class="sxs-lookup"><span data-stu-id="655ae-1389">ACR</span></span>
* <span data-ttu-id="655ae-1390">Ajout de commandes de tâche ACR</span><span class="sxs-lookup"><span data-stu-id="655ae-1390">Added ACR Task commands</span></span>
* <span data-ttu-id="655ae-1391">Ajout de la commande d’exécution rapide</span><span class="sxs-lookup"><span data-stu-id="655ae-1391">Added quick run command</span></span>
* <span data-ttu-id="655ae-1392">Groupe de commandes `build-task` déconseillé</span><span class="sxs-lookup"><span data-stu-id="655ae-1392">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="655ae-1393">Ajout du groupe de commandes `helm` pour prendre en charge la gestion des graphiques Helm avec ACR</span><span class="sxs-lookup"><span data-stu-id="655ae-1393">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="655ae-1394">Ajout de la prise en charge de la création idempotent pour les registres managés</span><span class="sxs-lookup"><span data-stu-id="655ae-1394">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="655ae-1395">Ajout d’un indicateur de non-format pour l’affichage des journaux d’activité de génération</span><span class="sxs-lookup"><span data-stu-id="655ae-1395">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="655ae-1396">ACS</span><span class="sxs-lookup"><span data-stu-id="655ae-1396">ACS</span></span>
* <span data-ttu-id="655ae-1397">Modification de la commande `install-connector` pour configurer le nom de domaine complet maître AKS</span><span class="sxs-lookup"><span data-stu-id="655ae-1397">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="655ae-1398">Correction de la création d’attribution de rôle pour vnet-subnet-id lorsque le principal de service n’est pas spécifié, et pour skip-role-assignemnt</span><span class="sxs-lookup"><span data-stu-id="655ae-1398">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="655ae-1399">AppService</span><span class="sxs-lookup"><span data-stu-id="655ae-1399">AppService</span></span>

* <span data-ttu-id="655ae-1400">Ajout de la prise en charge de la gestion des opérations (continues et déclenchées) des Webjobs</span><span class="sxs-lookup"><span data-stu-id="655ae-1400">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="655ae-1401">az webapp config set prend en charge la propriété FTS-state. Aussi ajout de la prise en charge de az functionapp config set & show</span><span class="sxs-lookup"><span data-stu-id="655ae-1401">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="655ae-1402">Ajout de la prise en charge de Bring Your Own Storage pour les applications web</span><span class="sxs-lookup"><span data-stu-id="655ae-1402">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="655ae-1403">Ajout de la prise en charge du référencement et de la restauration des applications web supprimées</span><span class="sxs-lookup"><span data-stu-id="655ae-1403">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="655ae-1404">Batch</span><span class="sxs-lookup"><span data-stu-id="655ae-1404">Batch</span></span>
* <span data-ttu-id="655ae-1405">Modification de l’ajout des tâches via `--json-file` pour prendre en charge la syntaxe AddTaskCollectionParameter</span><span class="sxs-lookup"><span data-stu-id="655ae-1405">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="655ae-1406">Mise à jour de la documentation des formats `--json-file` acceptés</span><span class="sxs-lookup"><span data-stu-id="655ae-1406">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="655ae-1407">Ajout de `--max-tasks-per-node-option` à `batch pool create`</span><span class="sxs-lookup"><span data-stu-id="655ae-1407">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="655ae-1408">Modification du comportement de `batch account` pour afficher la connexion au compte si aucune option n’est spécifiée</span><span class="sxs-lookup"><span data-stu-id="655ae-1408">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="655ae-1409">Batch AI</span><span class="sxs-lookup"><span data-stu-id="655ae-1409">Batch AI</span></span> 
* <span data-ttu-id="655ae-1410">Correction de l’échec de création de compte de stockage automatique dans la commande `batchai cluster create`</span><span class="sxs-lookup"><span data-stu-id="655ae-1410">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="655ae-1411">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="655ae-1411">Cognitive Services</span></span>
* <span data-ttu-id="655ae-1412">Ajout de Completer pour les arguments `--sku`, `--kind` et `--location`</span><span class="sxs-lookup"><span data-stu-id="655ae-1412">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="655ae-1413">Ajout de la commande `cognitiveservices account list-usage`</span><span class="sxs-lookup"><span data-stu-id="655ae-1413">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="655ae-1414">Ajout de la commande `cognitiveservices account list-kinds`</span><span class="sxs-lookup"><span data-stu-id="655ae-1414">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="655ae-1415">Ajout de la commande `cognitiveservices account list`</span><span class="sxs-lookup"><span data-stu-id="655ae-1415">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="655ae-1416">`cognitiveservices list` déconseillé</span><span class="sxs-lookup"><span data-stu-id="655ae-1416">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="655ae-1417">Modification de `--name` afin de le rendre facultatif pour `cognitiveservices account list-skus`</span><span class="sxs-lookup"><span data-stu-id="655ae-1417">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="655ae-1418">Conteneur</span><span class="sxs-lookup"><span data-stu-id="655ae-1418">Container</span></span>
* <span data-ttu-id="655ae-1419">Ajout de la possibilité de redémarrer et d’arrêter un groupe de conteneurs en cours d’exécution</span><span class="sxs-lookup"><span data-stu-id="655ae-1419">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="655ae-1420">Ajout de `--network-profile` pour autoriser le passage dans un profil réseau</span><span class="sxs-lookup"><span data-stu-id="655ae-1420">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="655ae-1421">Ajout de `--subnet` et `--vnet_name` pour autoriser la création de groupes de conteneurs dans un réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="655ae-1421">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="655ae-1422">Modification de la sortie de table pour afficher l’état du groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="655ae-1422">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="655ae-1423">DataLake</span><span class="sxs-lookup"><span data-stu-id="655ae-1423">Datalake</span></span>
* <span data-ttu-id="655ae-1424">Ajout de commandes pour les règles de réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="655ae-1424">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="655ae-1425">Shell interactif</span><span class="sxs-lookup"><span data-stu-id="655ae-1425">Interactive Shell</span></span>
* <span data-ttu-id="655ae-1426">Correction des erreurs sur Windows où les commandes ne s’exécutent pas correctement</span><span class="sxs-lookup"><span data-stu-id="655ae-1426">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="655ae-1427">Correction du problème de chargement de commande dans le Shell interactif provoqué par les objets déconseillés</span><span class="sxs-lookup"><span data-stu-id="655ae-1427">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="655ae-1428">IoT</span><span class="sxs-lookup"><span data-stu-id="655ae-1428">IoT</span></span>
* <span data-ttu-id="655ae-1429">Ajout de la prise en charge du routage des hubs IoT</span><span class="sxs-lookup"><span data-stu-id="655ae-1429">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="655ae-1430">Key Vault</span><span class="sxs-lookup"><span data-stu-id="655ae-1430">Key Vault</span></span>
* <span data-ttu-id="655ae-1431">Correction de l’importation de la clé Key Vault pour les clés RSA</span><span class="sxs-lookup"><span data-stu-id="655ae-1431">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="655ae-1432">Réseau</span><span class="sxs-lookup"><span data-stu-id="655ae-1432">Network</span></span>
* <span data-ttu-id="655ae-1433">Ajout des commandes `network public-ip prefix` pour prendre en charge les fonctionnalités de préfixes d’adresses IP publiques</span><span class="sxs-lookup"><span data-stu-id="655ae-1433">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="655ae-1434">Ajout des commandes `network service-endpoint` pour prendre en charge les fonctionnalités de stratégie de point de terminaison de service</span><span class="sxs-lookup"><span data-stu-id="655ae-1434">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="655ae-1435">Ajout des commandes `network lb outbound-rule` pour prendre en charge la création de règles de trafic sortant d’un équilibreur de charge standard</span><span class="sxs-lookup"><span data-stu-id="655ae-1435">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="655ae-1436">Ajout de `--public-ip-prefix` à `network lb frontend-ip create/update` pour prendre en charge les configurations IP frontales à l’aide de préfixes d’adresses IP publiques</span><span class="sxs-lookup"><span data-stu-id="655ae-1436">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="655ae-1437">Ajout de `--enable-tcp-reset` à `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span><span class="sxs-lookup"><span data-stu-id="655ae-1437">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="655ae-1438">Ajout de `--disable-outbound-snat` à `network lb rule create/update`</span><span class="sxs-lookup"><span data-stu-id="655ae-1438">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="655ae-1439">Autoriser `network watcher flow-log show/configure` à être utilisé avec des groupes de sécurité réseau classiques</span><span class="sxs-lookup"><span data-stu-id="655ae-1439">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="655ae-1440">Ajouter la commande `network watcher run-configuration-diagnostic`</span><span class="sxs-lookup"><span data-stu-id="655ae-1440">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="655ae-1441">Correction de la commande `network watcher test-connectivity` et ajout des propriétés `--method`, `--valid-status-codes` et `--headers`</span><span class="sxs-lookup"><span data-stu-id="655ae-1441">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="655ae-1442">`network express-route create/update`: ajout de l’indicateur `--allow-global-reach`</span><span class="sxs-lookup"><span data-stu-id="655ae-1442">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="655ae-1443">`network vnet subnet create/update`: ajout de la prise en charge de `--delegation`</span><span class="sxs-lookup"><span data-stu-id="655ae-1443">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="655ae-1444">Ajout de la commande `network vnet subnet list-available-delegations`</span><span class="sxs-lookup"><span data-stu-id="655ae-1444">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="655ae-1445">`network traffic-manager profile create/update`: ajout de la prise en charge de `--interval`, `--timeout` et `--max-failures` pour les options Deprecated de configuration du moniteur `--monitor-path`, `--monitor-port` et `--monitor-protocol` en faveur de `--path`, `--port`, `--protocol`</span><span class="sxs-lookup"><span data-stu-id="655ae-1445">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="655ae-1446">`network lb frontend-ip create/update`: correction de la logique de réglage de la méthode d’allocation d’adresses IP privées. Si une adresse IP privée est fournie, l’allocation sera statique. Si aucune adresse IP privée n’est fournie, ou qu’une chaîne vide est fournie pour l’adresse IP privée, l’allocation est dynamique.</span><span class="sxs-lookup"><span data-stu-id="655ae-1446">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="655ae-1447">`dns record-set * create/update`: ajout de la prise en charge de `--target-resource`</span><span class="sxs-lookup"><span data-stu-id="655ae-1447">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="655ae-1448">Ajout des commandes `network interface-endpoint` pour interroger les objets de point de terminaison de l’interface</span><span class="sxs-lookup"><span data-stu-id="655ae-1448">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="655ae-1449">Ajout de `network profile show/list/delete` pour la gestion partielle des profils de réseau</span><span class="sxs-lookup"><span data-stu-id="655ae-1449">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="655ae-1450">Ajout des commandes `network express-route peering connection` pour gérer les connexions de peering entre les routes ExpressRoutes</span><span class="sxs-lookup"><span data-stu-id="655ae-1450">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="655ae-1451">SGBDR</span><span class="sxs-lookup"><span data-stu-id="655ae-1451">RDBMS</span></span>
* <span data-ttu-id="655ae-1452">Ajout de la prise en charge du service MariaDB</span><span class="sxs-lookup"><span data-stu-id="655ae-1452">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="655ae-1453">Réservation</span><span class="sxs-lookup"><span data-stu-id="655ae-1453">Reservation</span></span>
* <span data-ttu-id="655ae-1454">Ajout de CosmosDb dans le type d’énumération des ressources réservées</span><span class="sxs-lookup"><span data-stu-id="655ae-1454">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="655ae-1455">Ajout de la propriété de nom dans un modèle Patch</span><span class="sxs-lookup"><span data-stu-id="655ae-1455">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="655ae-1456">Gérer l’application</span><span class="sxs-lookup"><span data-stu-id="655ae-1456">Manage App</span></span>
* <span data-ttu-id="655ae-1457">Correction du bogue dans `managedapp create --kind MarketPlace` à l’origine du blocage de la création d’instance d’une application Marketplace gérée</span><span class="sxs-lookup"><span data-stu-id="655ae-1457">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="655ae-1458">Modification des commandes `feature` afin qu’elles soient limitées aux profils pris en charge</span><span class="sxs-lookup"><span data-stu-id="655ae-1458">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="655ae-1459">Role</span><span class="sxs-lookup"><span data-stu-id="655ae-1459">Role</span></span>
* <span data-ttu-id="655ae-1460">Ajout de la prise en charge pour répertorier les appartenances de l’utilisateur à des groupes</span><span class="sxs-lookup"><span data-stu-id="655ae-1460">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="655ae-1461">SignalR</span><span class="sxs-lookup"><span data-stu-id="655ae-1461">SignalR</span></span>
* <span data-ttu-id="655ae-1462">Première version</span><span class="sxs-lookup"><span data-stu-id="655ae-1462">First release</span></span>

### <a name="storage"></a><span data-ttu-id="655ae-1463">Stockage</span><span class="sxs-lookup"><span data-stu-id="655ae-1463">Storage</span></span>
* <span data-ttu-id="655ae-1464">Ajout du paramètre `--auth-mode login` pour l’utilisation des informations d’identification de l’utilisateur pour autoriser les objets blob et les files d’attente</span><span class="sxs-lookup"><span data-stu-id="655ae-1464">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="655ae-1465">Ajout de `storage container immutability-policy/legal-hold` pour gérer le stockage immuable</span><span class="sxs-lookup"><span data-stu-id="655ae-1465">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="655ae-1466">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="655ae-1466">VM</span></span>
* <span data-ttu-id="655ae-1467">Correction d’un problème `vm create --generate-ssh-keys` qui remplace le fichier de clé privée si le fichier de clé publique est manquant (#4725, #6780)</span><span class="sxs-lookup"><span data-stu-id="655ae-1467">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="655ae-1468">Ajout de la prise en charge pour la galerie d’images partagée via `az sig`</span><span class="sxs-lookup"><span data-stu-id="655ae-1468">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="655ae-1469">28 Août 2018</span><span class="sxs-lookup"><span data-stu-id="655ae-1469">August 28, 2018</span></span>

<span data-ttu-id="655ae-1470">Version 2.0.45</span><span class="sxs-lookup"><span data-stu-id="655ae-1470">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="655ae-1471">Core</span><span class="sxs-lookup"><span data-stu-id="655ae-1471">Core</span></span>

* <span data-ttu-id="655ae-1472">Résolution du problème de chargement de fichier de configuration vide</span><span class="sxs-lookup"><span data-stu-id="655ae-1472">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="655ae-1473">Ajout de la prise en charge du profil `2018-03-01-hybrid` pour Azure Stack</span><span class="sxs-lookup"><span data-stu-id="655ae-1473">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="655ae-1474">ACR</span><span class="sxs-lookup"><span data-stu-id="655ae-1474">ACR</span></span>

* <span data-ttu-id="655ae-1475">Ajout d’une solution pour les opérations d’exécution sans les requêtes ARM</span><span class="sxs-lookup"><span data-stu-id="655ae-1475">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="655ae-1476">Exclusion des fichiers de contrôle de version (par exemple, .git, .gitignore) chargés par défaut dans les fichiers tar dans la commande `build`</span><span class="sxs-lookup"><span data-stu-id="655ae-1476">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="655ae-1477">ACS</span><span class="sxs-lookup"><span data-stu-id="655ae-1477">ACS</span></span>

* <span data-ttu-id="655ae-1478">Modification de `aks create` à la valeur par défaut sur les machines virtuelles `Standard_DS2_v2`</span><span class="sxs-lookup"><span data-stu-id="655ae-1478">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="655ae-1479">Modification de `aks get-credentials` afin d’appeler de nouvelles API pour l’obtention des informations d’identification des clusters</span><span class="sxs-lookup"><span data-stu-id="655ae-1479">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="655ae-1480">AppService</span><span class="sxs-lookup"><span data-stu-id="655ae-1480">AppService</span></span>

* <span data-ttu-id="655ae-1481">Prise en charge de CORS sur functionapp et webapp</span><span class="sxs-lookup"><span data-stu-id="655ae-1481">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="655ae-1482">Ajout de la prise en charge de la balise ARM sur les commandes de création</span><span class="sxs-lookup"><span data-stu-id="655ae-1482">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="655ae-1483">Modification de `[webapp|functionapp] identity show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="655ae-1483">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="655ae-1484">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="655ae-1484">Backup</span></span>

* <span data-ttu-id="655ae-1485">Modification de `backup vault backup-properties show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="655ae-1485">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="655ae-1486">Service de robot</span><span class="sxs-lookup"><span data-stu-id="655ae-1486">Bot Service</span></span>

* <span data-ttu-id="655ae-1487">Version initiale de l’interface CLI de Bot Service</span><span class="sxs-lookup"><span data-stu-id="655ae-1487">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="655ae-1488">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="655ae-1488">Cognitive Services</span></span>

* <span data-ttu-id="655ae-1489">Ajout du nouveau paramètre `--api-properties,` requis pour la création de certains services</span><span class="sxs-lookup"><span data-stu-id="655ae-1489">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="655ae-1490">IoT</span><span class="sxs-lookup"><span data-stu-id="655ae-1490">IoT</span></span>

* <span data-ttu-id="655ae-1491">Résolution du problème relatif à l’association de hubs liés</span><span class="sxs-lookup"><span data-stu-id="655ae-1491">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="655ae-1492">Surveiller</span><span class="sxs-lookup"><span data-stu-id="655ae-1492">Monitor</span></span>

* <span data-ttu-id="655ae-1493">Ajout des commandes `monitor metrics alert` permettant de recevoir des alertes sur les métriques quasiment en temps réel</span><span class="sxs-lookup"><span data-stu-id="655ae-1493">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="655ae-1494">Commandes `monitor alert` déconseillées</span><span class="sxs-lookup"><span data-stu-id="655ae-1494">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="655ae-1495">Réseau</span><span class="sxs-lookup"><span data-stu-id="655ae-1495">Network</span></span>

* <span data-ttu-id="655ae-1496">Modification de `network application-gateway ssl-policy predefined show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="655ae-1496">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="655ae-1497">Ressource</span><span class="sxs-lookup"><span data-stu-id="655ae-1497">Resource</span></span>

* <span data-ttu-id="655ae-1498">Modification de `provider operation show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="655ae-1498">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="655ae-1499">Stockage</span><span class="sxs-lookup"><span data-stu-id="655ae-1499">Storage</span></span>

* <span data-ttu-id="655ae-1500">Modification de `storage share policy show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="655ae-1500">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="655ae-1501">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="655ae-1501">VM</span></span>

* <span data-ttu-id="655ae-1502">Modification de `vm/vmss identity show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="655ae-1502">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="655ae-1503">Remplacement de `--storage-caching` pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="655ae-1503">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="655ae-1504">14 août 2018</span><span class="sxs-lookup"><span data-stu-id="655ae-1504">Auguest 14, 2018</span></span>

<span data-ttu-id="655ae-1505">Version 2.0.44</span><span class="sxs-lookup"><span data-stu-id="655ae-1505">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="655ae-1506">Core</span><span class="sxs-lookup"><span data-stu-id="655ae-1506">Core</span></span>

* <span data-ttu-id="655ae-1507">Correction de l’affichage numérique dans la sortie `table`</span><span class="sxs-lookup"><span data-stu-id="655ae-1507">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="655ae-1508">Ajout du format de sortie YAML</span><span class="sxs-lookup"><span data-stu-id="655ae-1508">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="655ae-1509">Télémétrie</span><span class="sxs-lookup"><span data-stu-id="655ae-1509">Telemetry</span></span>

* <span data-ttu-id="655ae-1510">Amélioration des rapports de télémétrie</span><span class="sxs-lookup"><span data-stu-id="655ae-1510">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="655ae-1511">ACR</span><span class="sxs-lookup"><span data-stu-id="655ae-1511">ACR</span></span>

* <span data-ttu-id="655ae-1512">Ajout des commandes `content-trust policy`</span><span class="sxs-lookup"><span data-stu-id="655ae-1512">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="655ae-1513">Résolution du problème où `.dockerignore` n’était pas honorée</span><span class="sxs-lookup"><span data-stu-id="655ae-1513">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="655ae-1514">ACS</span><span class="sxs-lookup"><span data-stu-id="655ae-1514">ACS</span></span>

* <span data-ttu-id="655ae-1515">Modification de `az acs/aks install-cli` afin d’effectuer l’installation sous `%USERPROFILE%\.azure-kubectl` sur Windows</span><span class="sxs-lookup"><span data-stu-id="655ae-1515">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="655ae-1516">Modification de `az aks install-connector` afin de détecter si le cluster dispose du contrôle RBAC et de configurer le connecteur ACI correctement</span><span class="sxs-lookup"><span data-stu-id="655ae-1516">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="655ae-1517">Remplacement par l’attribution de rôle au sous-réseau lorsque l’attribution est fournie</span><span class="sxs-lookup"><span data-stu-id="655ae-1517">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="655ae-1518">Ajout de l’option nouveau « ignorer attribution de rôle » pour le sous-réseau lorsque l’attribution est fournie</span><span class="sxs-lookup"><span data-stu-id="655ae-1518">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="655ae-1519">Modification ignorant l’attribution de rôle au sous-réseau lorsque l’attribution existe déjà</span><span class="sxs-lookup"><span data-stu-id="655ae-1519">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="655ae-1520">AppService</span><span class="sxs-lookup"><span data-stu-id="655ae-1520">AppService</span></span>

* <span data-ttu-id="655ae-1521">Correction d’un bogue empêchant de créer une application de fonction à l’aide de comptes de stockage dans les groupes de ressources externes</span><span class="sxs-lookup"><span data-stu-id="655ae-1521">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="655ae-1522">Correction d’un incident lors du déploiement de dossier zip</span><span class="sxs-lookup"><span data-stu-id="655ae-1522">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="655ae-1523">Batch AI</span><span class="sxs-lookup"><span data-stu-id="655ae-1523">BatchAI</span></span>

* <span data-ttu-id="655ae-1524">Modification de la sortie de l’enregistreur d’événements pour la création du compte de stockage automatique afin de spécifier l’information « ressource *groupe*».</span><span class="sxs-lookup"><span data-stu-id="655ae-1524">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="655ae-1525">Conteneur</span><span class="sxs-lookup"><span data-stu-id="655ae-1525">Container</span></span>

* <span data-ttu-id="655ae-1526">Ajout de `--secure-environment-variables` pour transmettre des variables d’environnement sécurisées vers un conteneur</span><span class="sxs-lookup"><span data-stu-id="655ae-1526">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="655ae-1527">IoT</span><span class="sxs-lookup"><span data-stu-id="655ae-1527">IoT</span></span>

* <span data-ttu-id="655ae-1528">[CHANGEMENT CASSANT] Suppression des commandes obsolètes déplacées vers l’extension iot</span><span class="sxs-lookup"><span data-stu-id="655ae-1528">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="655ae-1529">Mise à jour des éléments afin de ne pas prendre en compte le domaine `azure-devices.net`</span><span class="sxs-lookup"><span data-stu-id="655ae-1529">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="655ae-1530">Iot Central</span><span class="sxs-lookup"><span data-stu-id="655ae-1530">Iot Central</span></span>

* <span data-ttu-id="655ae-1531">Version initiale du module IoT Central</span><span class="sxs-lookup"><span data-stu-id="655ae-1531">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="655ae-1532">KeyVault</span><span class="sxs-lookup"><span data-stu-id="655ae-1532">KeyVault</span></span>


* <span data-ttu-id="655ae-1533">Ajout des commandes pour la gestion des comptes de stockage et les définitions SAS</span><span class="sxs-lookup"><span data-stu-id="655ae-1533">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="655ae-1534">Ajout de commandes pour les règles réseau</span><span class="sxs-lookup"><span data-stu-id="655ae-1534">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="655ae-1535">Ajout du paramètre `--id` aux opérations relatives au mots de passe confidentiels, clés et certificats</span><span class="sxs-lookup"><span data-stu-id="655ae-1535">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="655ae-1536">Ajout de la prise en charge pour la version multi-api avec gestion des coffres de clés</span><span class="sxs-lookup"><span data-stu-id="655ae-1536">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="655ae-1537">Ajout de la prise en charge pour la version multi-api avec plan de données des coffres de clés</span><span class="sxs-lookup"><span data-stu-id="655ae-1537">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="655ae-1538">Relais</span><span class="sxs-lookup"><span data-stu-id="655ae-1538">Relay</span></span>

* <span data-ttu-id="655ae-1539">Version initiale</span><span class="sxs-lookup"><span data-stu-id="655ae-1539">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="655ae-1540">SQL</span><span class="sxs-lookup"><span data-stu-id="655ae-1540">Sql</span></span>

* <span data-ttu-id="655ae-1541">Ajout des commandes `sql failover-group`</span><span class="sxs-lookup"><span data-stu-id="655ae-1541">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="655ae-1542">Stockage</span><span class="sxs-lookup"><span data-stu-id="655ae-1542">Storage</span></span>

* <span data-ttu-id="655ae-1543">[CHANGEMENT CASSANT] Modification de `storage account show-usage` afin d’exiger le paramètre `--location` et de répertorier par région</span><span class="sxs-lookup"><span data-stu-id="655ae-1543">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="655ae-1544">Modification du paramètre `--resource-group` afin de le rendre facultatif pour les commandes `storage account`</span><span class="sxs-lookup"><span data-stu-id="655ae-1544">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="655ae-1545">Suppression des avertissements concernant l’échec de la condition préalable pour les défaillances isolées dans les commandes batch pour les messages agrégés uniques</span><span class="sxs-lookup"><span data-stu-id="655ae-1545">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="655ae-1546">Modification des commandes `[blob|file] delete-batch` afin de ne plus produire des tableaux ayant la valeur null</span><span class="sxs-lookup"><span data-stu-id="655ae-1546">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="655ae-1547">Modification des commandes `blob [download|upload|delete-batch]` afin de lire le jeton de SAS à partir de l’url du conteneur</span><span class="sxs-lookup"><span data-stu-id="655ae-1547">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="655ae-1548">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="655ae-1548">VM</span></span>

* <span data-ttu-id="655ae-1549">Ajout des filtres courants à `vm list-skus` pour une plus grande simplicité d’utilisation</span><span class="sxs-lookup"><span data-stu-id="655ae-1549">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="655ae-1550">31 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="655ae-1550">July 31, 2018</span></span>

<span data-ttu-id="655ae-1551">Version 2.0.43</span><span class="sxs-lookup"><span data-stu-id="655ae-1551">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="655ae-1552">ACR</span><span class="sxs-lookup"><span data-stu-id="655ae-1552">ACR</span></span>

* <span data-ttu-id="655ae-1553">Ajout de l’indicateur `--with-secure-properties` à la commande `acr build-task show`</span><span class="sxs-lookup"><span data-stu-id="655ae-1553">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="655ae-1554">Ajout de la commande `acr build-task update-build`</span><span class="sxs-lookup"><span data-stu-id="655ae-1554">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="655ae-1555">ACS</span><span class="sxs-lookup"><span data-stu-id="655ae-1555">ACS</span></span>

* <span data-ttu-id="655ae-1556">Retour au return 0 (réussite) à la fin de `az aks browse` en appuyant sur [Ctrl + C]</span><span class="sxs-lookup"><span data-stu-id="655ae-1556">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="655ae-1557">Batch</span><span class="sxs-lookup"><span data-stu-id="655ae-1557">Batch</span></span>

* <span data-ttu-id="655ae-1558">Correction du bug lors de l’affichage des jetons AAD dans le Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="655ae-1558">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="655ae-1559">Conteneur</span><span class="sxs-lookup"><span data-stu-id="655ae-1559">Container</span></span>

* <span data-ttu-id="655ae-1560">Suppression de l’exigence pour `--log-analytics-workspace-key` pour le nom ou l’identifiant lors de l’abonnement standard</span><span class="sxs-lookup"><span data-stu-id="655ae-1560">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="655ae-1561">Réseau</span><span class="sxs-lookup"><span data-stu-id="655ae-1561">Network</span></span>

* <span data-ttu-id="655ae-1562">Ajout du serveur DNS au profil du 09/03/2017 pour Azure Stack</span><span class="sxs-lookup"><span data-stu-id="655ae-1562">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="655ae-1563">Ressource</span><span class="sxs-lookup"><span data-stu-id="655ae-1563">Resource</span></span>

* <span data-ttu-id="655ae-1564">Ajout de `--rollback-on-error` à `group deployment create` pour exécuter un déploiement correct et connu en cas d’erreur</span><span class="sxs-lookup"><span data-stu-id="655ae-1564">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="655ae-1565">Correction d’un problème où `--parameters {}` avec `group deployment create` entraînait une erreur</span><span class="sxs-lookup"><span data-stu-id="655ae-1565">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="655ae-1566">Role</span><span class="sxs-lookup"><span data-stu-id="655ae-1566">Role</span></span>

* <span data-ttu-id="655ae-1567">Ajout de la prise en charge du profil stack du 09/03/2017</span><span class="sxs-lookup"><span data-stu-id="655ae-1567">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="655ae-1568">Correction d’un problème où les paramètres de mise à jour génériques à `app update` ne fonctionnaient pas correctement</span><span class="sxs-lookup"><span data-stu-id="655ae-1568">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="655ae-1569">Recherche</span><span class="sxs-lookup"><span data-stu-id="655ae-1569">Search</span></span>

* <span data-ttu-id="655ae-1570">Ajout de commandes pour le service de recherches d’Azure</span><span class="sxs-lookup"><span data-stu-id="655ae-1570">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="655ae-1571">Service Bus</span><span class="sxs-lookup"><span data-stu-id="655ae-1571">Service Bus</span></span>

* <span data-ttu-id="655ae-1572">Ajout d’un groupe de commandes de migration pour migrer un espace de noms d’un Service Bus Standard à un Premium</span><span class="sxs-lookup"><span data-stu-id="655ae-1572">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="655ae-1573">Ajout de nouvelles propriétés facultatives à la file d’attente du Service Bus et à l’abonnement</span><span class="sxs-lookup"><span data-stu-id="655ae-1573">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="655ae-1574">`--enable-batched-operations` et `--enable-dead-lettering-on-message-expiration` dans `queue`</span><span class="sxs-lookup"><span data-stu-id="655ae-1574">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="655ae-1575">`--dead-letter-on-filter-exceptions` dans `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="655ae-1575">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="655ae-1576">Stockage</span><span class="sxs-lookup"><span data-stu-id="655ae-1576">Storage</span></span>

* <span data-ttu-id="655ae-1577">Ajout de la prise en charge du téléchargement de fichiers volumineux à l’aide d’une connexion unique</span><span class="sxs-lookup"><span data-stu-id="655ae-1577">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="655ae-1578">Conversion des commandes `show` qui manquaient d’échouer avec le code de sortie 3 sur une ressource manquante</span><span class="sxs-lookup"><span data-stu-id="655ae-1578">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="655ae-1579">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="655ae-1579">VM</span></span>

* <span data-ttu-id="655ae-1580">Ajout d’une prise en charge pour lister les groupes disponibles par abonnement</span><span class="sxs-lookup"><span data-stu-id="655ae-1580">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="655ae-1581">Ajout de la prise en charge de `StandardSSD_LRS`</span><span class="sxs-lookup"><span data-stu-id="655ae-1581">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="655ae-1582">Ajout d’une prise en charge des groupes de sécurité d’application dans la création du groupe identique de machines virtuelles</span><span class="sxs-lookup"><span data-stu-id="655ae-1582">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="655ae-1583">[CHANGEMENT CASSANT] Changement de `[vm|vmss] create`, `[vm|vmss] identity assign`, et `[vm|vmss] identity remove` pour sortir les identités des utilisateurs au format de dictionnaire</span><span class="sxs-lookup"><span data-stu-id="655ae-1583">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="655ae-1584">18 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="655ae-1584">July 18, 2018</span></span>

<span data-ttu-id="655ae-1585">Version 2.0.42</span><span class="sxs-lookup"><span data-stu-id="655ae-1585">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="655ae-1586">Core</span><span class="sxs-lookup"><span data-stu-id="655ae-1586">Core</span></span>

* <span data-ttu-id="655ae-1587">Ajout de la prise en charge de la connexion basée sur le navigateur dans la fenêtre d’interpréteur de commandes Windows pour Linux</span><span class="sxs-lookup"><span data-stu-id="655ae-1587">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="655ae-1588">Ajout de l’indicateur `--force-string` pour toutes les commandes de mise à jour générique</span><span class="sxs-lookup"><span data-stu-id="655ae-1588">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="655ae-1589">[CHANGEMENT CASSANT] Modification des commandes « d’affichage » pour connecter le message d’erreur et échec avec un code de sortie de 3 sur une ressource manquante</span><span class="sxs-lookup"><span data-stu-id="655ae-1589">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="655ae-1590">ACR</span><span class="sxs-lookup"><span data-stu-id="655ae-1590">ACR</span></span>

* <span data-ttu-id="655ae-1591">[CHANGEMENT CASSANT] Mise à jour de « --no-push » vers un indicateur pur dans la commande « ACR Build »</span><span class="sxs-lookup"><span data-stu-id="655ae-1591">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="655ae-1592">Ajout des commandes `show` et `update` sous le groupe `acr repository`</span><span class="sxs-lookup"><span data-stu-id="655ae-1592">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="655ae-1593">Ajout de l’indicateur `--detail` à `show-manifests` et `show-tags` pour afficher des informations plus détaillées</span><span class="sxs-lookup"><span data-stu-id="655ae-1593">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="655ae-1594">Ajout du paramètre `--image` pour prendre en charge l’obtention des détails de build ou des journaux d’activité par une image</span><span class="sxs-lookup"><span data-stu-id="655ae-1594">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="655ae-1595">ACS</span><span class="sxs-lookup"><span data-stu-id="655ae-1595">ACS</span></span>

* <span data-ttu-id="655ae-1596">Modification de `az aks create` en sortie d’erreur si `--max-pods` est inférieur à 5</span><span class="sxs-lookup"><span data-stu-id="655ae-1596">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="655ae-1597">AppService</span><span class="sxs-lookup"><span data-stu-id="655ae-1597">AppService</span></span>

* <span data-ttu-id="655ae-1598">Ajout de la prise en charge pour les références (SKU) PremiumV2</span><span class="sxs-lookup"><span data-stu-id="655ae-1598">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="655ae-1599">Batch</span><span class="sxs-lookup"><span data-stu-id="655ae-1599">Batch</span></span>

* <span data-ttu-id="655ae-1600">Correction d’un bogue relatif à l’utilisation des informations d’identification de jeton dans le mode Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="655ae-1600">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="655ae-1601">Modification de l’entrée JSON pour respecter la casse</span><span class="sxs-lookup"><span data-stu-id="655ae-1601">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="655ae-1602">Batch AI</span><span class="sxs-lookup"><span data-stu-id="655ae-1602">Batch AI</span></span>

* <span data-ttu-id="655ae-1603">Correction de la commande `az batchai job exec`</span><span class="sxs-lookup"><span data-stu-id="655ae-1603">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="655ae-1604">Conteneur</span><span class="sxs-lookup"><span data-stu-id="655ae-1604">Container</span></span>

* <span data-ttu-id="655ae-1605">Suppression des exigences pour le nom d’utilisateur et le mot de passe pour les registres non dockerhub</span><span class="sxs-lookup"><span data-stu-id="655ae-1605">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="655ae-1606">Correction de l’erreur lors de la création de groupes de conteneur à partir du fichier yaml</span><span class="sxs-lookup"><span data-stu-id="655ae-1606">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="655ae-1607">Réseau</span><span class="sxs-lookup"><span data-stu-id="655ae-1607">Network</span></span>

* <span data-ttu-id="655ae-1608">Ajout de la prise en charge de `--no-wait` pour `network nic [create|update|delete]`</span><span class="sxs-lookup"><span data-stu-id="655ae-1608">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="655ae-1609">Ajout de `network nic wait`</span><span class="sxs-lookup"><span data-stu-id="655ae-1609">Added `network nic wait`</span></span>
* <span data-ttu-id="655ae-1610">Argument `--ids` déconseillé pour `network vnet [subnet|peering] list`</span><span class="sxs-lookup"><span data-stu-id="655ae-1610">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="655ae-1611">Ajout de l’indicateur `--include-default` pour inclure les règles de sécurité par défaut dans la sortie de `network nsg rule list`</span><span class="sxs-lookup"><span data-stu-id="655ae-1611">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="655ae-1612">Ressource</span><span class="sxs-lookup"><span data-stu-id="655ae-1612">Resource</span></span>

* <span data-ttu-id="655ae-1613">Ajout de la prise en charge de `--no-wait` pour `group deployment delete`</span><span class="sxs-lookup"><span data-stu-id="655ae-1613">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="655ae-1614">Ajout de la prise en charge de `--no-wait` pour `deployment delete`</span><span class="sxs-lookup"><span data-stu-id="655ae-1614">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="655ae-1615">Ajout de la commande `deployment wait`</span><span class="sxs-lookup"><span data-stu-id="655ae-1615">Added `deployment wait` command</span></span>
* <span data-ttu-id="655ae-1616">Résolution du problème qui causait l’affichage par erreur des commandes `az deployment` du niveau de l’abonnement pour le profil 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="655ae-1616">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="655ae-1617">SQL</span><span class="sxs-lookup"><span data-stu-id="655ae-1617">SQL</span></span>

* <span data-ttu-id="655ae-1618">Résolution de l’erreur « Le nom du groupe de ressources fourni ne correspond pas au nom de l’URL » lors de la spécification du nom du pool élastique pour les commandes `sql db copy` et `sql db replica create`</span><span class="sxs-lookup"><span data-stu-id="655ae-1618">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="655ae-1619">Autoriser la configuration de SQL Server par défaut en exécutant `az configure --defaults sql-server=<name>`</span><span class="sxs-lookup"><span data-stu-id="655ae-1619">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="655ae-1620">Implémentation de formateurs de table pour les commandes `sql server`, `sql server firewall-rule`, `sql list-usages` et `sql show-usage`</span><span class="sxs-lookup"><span data-stu-id="655ae-1620">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="655ae-1621">Stockage</span><span class="sxs-lookup"><span data-stu-id="655ae-1621">Storage</span></span>

* <span data-ttu-id="655ae-1622">Ajout de la propriété `pageRanges` à la sortie `storage blob show` qui sera renseignée pour les objets blob de pages</span><span class="sxs-lookup"><span data-stu-id="655ae-1622">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="655ae-1623">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="655ae-1623">VM</span></span>

* <span data-ttu-id="655ae-1624">[CHANGEMENT CASSANT] Modification de `vmss create` pour utiliser `Standard_DS1_v2` comme taille d’instance par défaut</span><span class="sxs-lookup"><span data-stu-id="655ae-1624">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="655ae-1625">Ajout de la prise en charge de `--no-wait` pour `vm extension [set|delete]` et `vmss extension [set|delete]`</span><span class="sxs-lookup"><span data-stu-id="655ae-1625">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="655ae-1626">Ajout de `vm extension wait`</span><span class="sxs-lookup"><span data-stu-id="655ae-1626">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="655ae-1627">3 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="655ae-1627">July 3, 2018</span></span>

<span data-ttu-id="655ae-1628">Version 2.0.41</span><span class="sxs-lookup"><span data-stu-id="655ae-1628">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="655ae-1629">AKS</span><span class="sxs-lookup"><span data-stu-id="655ae-1629">AKS</span></span>

* <span data-ttu-id="655ae-1630">Modification de la surveillance pour utiliser l’ID d’abonnement</span><span class="sxs-lookup"><span data-stu-id="655ae-1630">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="655ae-1631">3 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="655ae-1631">July 3, 2018</span></span>

<span data-ttu-id="655ae-1632">Version 2.0.40</span><span class="sxs-lookup"><span data-stu-id="655ae-1632">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="655ae-1633">Core</span><span class="sxs-lookup"><span data-stu-id="655ae-1633">Core</span></span>

* <span data-ttu-id="655ae-1634">Ajout d’un nouveau flux de code d’autorisation pour une connexion interactive</span><span class="sxs-lookup"><span data-stu-id="655ae-1634">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="655ae-1635">ACR</span><span class="sxs-lookup"><span data-stu-id="655ae-1635">ACR</span></span>

* <span data-ttu-id="655ae-1636">Ajout de l’interrogation de l’état du build</span><span class="sxs-lookup"><span data-stu-id="655ae-1636">Added polling build status</span></span>
* <span data-ttu-id="655ae-1637">Ajout de la prise en charge des valeurs d’énumération ne respectant pas la casse</span><span class="sxs-lookup"><span data-stu-id="655ae-1637">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="655ae-1638">Ajout des paramètres `--top` et `--orderby` pour `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="655ae-1638">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="655ae-1639">ACS</span><span class="sxs-lookup"><span data-stu-id="655ae-1639">ACS</span></span>

* <span data-ttu-id="655ae-1640">[CHANGEMENT CASSANT] Active le contrôle d’accès en fonction du rôle Kubernetes par défaut</span><span class="sxs-lookup"><span data-stu-id="655ae-1640">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="655ae-1641">Ajout de l’argument `--disable-rbac` et dépréciation de `--enable-rbac` dans la mesure où il s’agit actuellement de la valeur par défaut</span><span class="sxs-lookup"><span data-stu-id="655ae-1641">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="655ae-1642">Mise à jour des options de la commande `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="655ae-1642">Updated options for `aks browse` command.</span></span> <span data-ttu-id="655ae-1643">Ajout de la prise en charge de `--listen-port`</span><span class="sxs-lookup"><span data-stu-id="655ae-1643">Added `--listen-port` support</span></span>
* <span data-ttu-id="655ae-1644">Mise à jour du package de graphique Helm par défaut pour la commande `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="655ae-1644">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="655ae-1645">Use virtual-kubelet-for-aks-latest.tgz</span><span class="sxs-lookup"><span data-stu-id="655ae-1645">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="655ae-1646">Ajout des commandes `aks enable-addons` et `aks disable-addons` pour mettre à jour un cluster existant</span><span class="sxs-lookup"><span data-stu-id="655ae-1646">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="655ae-1647">AppService</span><span class="sxs-lookup"><span data-stu-id="655ae-1647">AppService</span></span>

* <span data-ttu-id="655ae-1648">Ajout de la prise en charge de la désactivation d’identité via `webapp identity remove`</span><span class="sxs-lookup"><span data-stu-id="655ae-1648">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="655ae-1649">Suppression de la balise `preview` pour la fonctionnalité Identité</span><span class="sxs-lookup"><span data-stu-id="655ae-1649">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="655ae-1650">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="655ae-1650">Backup</span></span>

* <span data-ttu-id="655ae-1651">Mise à jour de la définition du module</span><span class="sxs-lookup"><span data-stu-id="655ae-1651">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="655ae-1652">Batch AI</span><span class="sxs-lookup"><span data-stu-id="655ae-1652">BatchAI</span></span>

* <span data-ttu-id="655ae-1653">Correction de la sortie de table pour les commandes `batchai cluster node list` et `batchai job node list`</span><span class="sxs-lookup"><span data-stu-id="655ae-1653">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="655ae-1654">Cloud</span><span class="sxs-lookup"><span data-stu-id="655ae-1654">Cloud</span></span>

* <span data-ttu-id="655ae-1655">Ajout du suffixe de serveur `acr login` à la configuration du cloud</span><span class="sxs-lookup"><span data-stu-id="655ae-1655">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="655ae-1656">Conteneur</span><span class="sxs-lookup"><span data-stu-id="655ae-1656">Container</span></span>

* <span data-ttu-id="655ae-1657">Modification de `container create` sur valeur par défaut en opération à long terme</span><span class="sxs-lookup"><span data-stu-id="655ae-1657">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="655ae-1658">Ajout des paramètres Log Analytics `--log-analytics-workspace` et `--log-analytics-workspace-key`</span><span class="sxs-lookup"><span data-stu-id="655ae-1658">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="655ae-1659">Ajout du paramètre `--protocol` pour spécifier le protocole réseau à utiliser</span><span class="sxs-lookup"><span data-stu-id="655ae-1659">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="655ae-1660">Extension</span><span class="sxs-lookup"><span data-stu-id="655ae-1660">Extension</span></span>

* <span data-ttu-id="655ae-1661">Modification de `extension list-available` pour afficher uniquement les extensions compatibles avec la version CLI</span><span class="sxs-lookup"><span data-stu-id="655ae-1661">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="655ae-1662">Réseau</span><span class="sxs-lookup"><span data-stu-id="655ae-1662">Network</span></span>

* <span data-ttu-id="655ae-1663">Résolution du problème où les types d’enregistrement étaient sensibles à la casse pour ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="655ae-1663">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="655ae-1664">Rdbms</span><span class="sxs-lookup"><span data-stu-id="655ae-1664">Rdbms</span></span>

* <span data-ttu-id="655ae-1665">Ajout des commandes `[postgres|myql] server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="655ae-1665">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="655ae-1666">Ressource</span><span class="sxs-lookup"><span data-stu-id="655ae-1666">Resource</span></span>

* <span data-ttu-id="655ae-1667">Ajout d’un nouveau groupe d’opérations `deployment`</span><span class="sxs-lookup"><span data-stu-id="655ae-1667">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="655ae-1668">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="655ae-1668">VM</span></span>

* <span data-ttu-id="655ae-1669">Ajout de la prise en charge de la suppression de l’identité affectée au système</span><span class="sxs-lookup"><span data-stu-id="655ae-1669">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="655ae-1670">25 juin 2018</span><span class="sxs-lookup"><span data-stu-id="655ae-1670">June 25, 2018</span></span>

<span data-ttu-id="655ae-1671">Version 2.0.39</span><span class="sxs-lookup"><span data-stu-id="655ae-1671">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="655ae-1672">Interface de ligne de commande</span><span class="sxs-lookup"><span data-stu-id="655ae-1672">CLI</span></span>

* <span data-ttu-id="655ae-1673">Mise à jour de la suppression du fichier dans le programme d’installation MSI pour résoudre le problème d’installation de l’extension</span><span class="sxs-lookup"><span data-stu-id="655ae-1673">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="655ae-1674">19 juin 2018</span><span class="sxs-lookup"><span data-stu-id="655ae-1674">June 19, 2018</span></span>

<span data-ttu-id="655ae-1675">Version 2.0.38</span><span class="sxs-lookup"><span data-stu-id="655ae-1675">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="655ae-1676">Core</span><span class="sxs-lookup"><span data-stu-id="655ae-1676">Core</span></span>

* <span data-ttu-id="655ae-1677">Ajout de la prise en charge globale de `--subscription` pour la plupart des commandes</span><span class="sxs-lookup"><span data-stu-id="655ae-1677">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="655ae-1678">ACR</span><span class="sxs-lookup"><span data-stu-id="655ae-1678">ACR</span></span>

* <span data-ttu-id="655ae-1679">Ajout de `azure-storage-blob` comme dépendance</span><span class="sxs-lookup"><span data-stu-id="655ae-1679">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="655ae-1680">Modification de la configuration de l’UC par défaut avec `acr build-task create` pour utiliser 2 cœurs</span><span class="sxs-lookup"><span data-stu-id="655ae-1680">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="655ae-1681">ACS</span><span class="sxs-lookup"><span data-stu-id="655ae-1681">ACS</span></span>

* <span data-ttu-id="655ae-1682">Mise à jour des options de la commande `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="655ae-1682">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="655ae-1683">Ajout de la prise en charge de `--update`</span><span class="sxs-lookup"><span data-stu-id="655ae-1683">Added `--update` support</span></span>
* <span data-ttu-id="655ae-1684">Modification de `aks get-credentials --admin` pour ne pas remplacer le contexte utilisateur dans `$HOME/.kube/config`</span><span class="sxs-lookup"><span data-stu-id="655ae-1684">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="655ae-1685">Exposition de la propriété en lecture seule `nodeResourceGroup` sur les clusters managés</span><span class="sxs-lookup"><span data-stu-id="655ae-1685">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="655ae-1686">Correction de l’erreur de commande `acs browse`</span><span class="sxs-lookup"><span data-stu-id="655ae-1686">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="655ae-1687">`--connector-name` rendu facultatif pour `aks install-connector`, `aks upgrade-connector` et `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="655ae-1687">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="655ae-1688">Ajout de nouvelles régions Azure Container Instance pour `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="655ae-1688">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="655ae-1689">Ajout de l’emplacement normalisé dans le nom de mise en production Helm et le nom du nœud pour `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="655ae-1689">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="655ae-1690">AppService</span><span class="sxs-lookup"><span data-stu-id="655ae-1690">AppService</span></span>

* <span data-ttu-id="655ae-1691">Ajout de la prise en charge des versions urllib plus récentes</span><span class="sxs-lookup"><span data-stu-id="655ae-1691">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="655ae-1692">Ajout de la prise en charge pour `functionapp create` pour utiliser un plan App Service à partir de groupes de ressources externes</span><span class="sxs-lookup"><span data-stu-id="655ae-1692">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="655ae-1693">Batch</span><span class="sxs-lookup"><span data-stu-id="655ae-1693">Batch</span></span>

* <span data-ttu-id="655ae-1694">Suppression de la dépendance `azure-batch-extensions`</span><span class="sxs-lookup"><span data-stu-id="655ae-1694">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="655ae-1695">Batch AI</span><span class="sxs-lookup"><span data-stu-id="655ae-1695">Batch AI</span></span>

* <span data-ttu-id="655ae-1696">Ajout de la prise en charge des espaces de travail.</span><span class="sxs-lookup"><span data-stu-id="655ae-1696">Added support for workspaces.</span></span> <span data-ttu-id="655ae-1697">Les espaces de travail permettent de regrouper les clusters, serveurs de fichiers et expériences, supprimant la limitation du nombre de ressources qui peuvent être créées</span><span class="sxs-lookup"><span data-stu-id="655ae-1697">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="655ae-1698">Ajout de la prise en charge des expériences.</span><span class="sxs-lookup"><span data-stu-id="655ae-1698">Added support for experiments.</span></span> <span data-ttu-id="655ae-1699">Les expériences permettent de regrouper les tâches dans des collections, supprimant la limitation du nombre de tâches créées</span><span class="sxs-lookup"><span data-stu-id="655ae-1699">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="655ae-1700">Ajout de la prise en charge pour configurer `/dev/shm` pour les travaux en cours d’exécution dans un conteneur docker</span><span class="sxs-lookup"><span data-stu-id="655ae-1700">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="655ae-1701">Ajout des commandes `batchai cluster node exec` et `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="655ae-1701">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="655ae-1702">Ces commandes permettent d’exécuter des commandes directement sur les nœuds et fournissent la fonctionnalité de réacheminement de port.</span><span class="sxs-lookup"><span data-stu-id="655ae-1702">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="655ae-1703">Ajout de la prise en charge des commandes `--ids` et `batchai`</span><span class="sxs-lookup"><span data-stu-id="655ae-1703">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="655ae-1704">[CHANGEMENT CASSANT] Tous les clusters et serveurs de fichiers doivent être créés dans des espaces de travail</span><span class="sxs-lookup"><span data-stu-id="655ae-1704">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="655ae-1705">[CHANGEMENT CASSANT] Les travaux doivent être créés dans des expériences</span><span class="sxs-lookup"><span data-stu-id="655ae-1705">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="655ae-1706">[CHANGEMENT CASSANT] Suppression de `--nfs-resource-group` des commandes `cluster create` et `job create`.</span><span class="sxs-lookup"><span data-stu-id="655ae-1706">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="655ae-1707">Pour monter un NFS appartenant à un autre espace de travail/groupe de ressources, indiquez l’ID ARM du serveur de fichiers via l’option `--nfs`</span><span class="sxs-lookup"><span data-stu-id="655ae-1707">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="655ae-1708">[CHANGEMENT CASSANT] Suppression de `--cluster-resource-group` de la commande `job create`.</span><span class="sxs-lookup"><span data-stu-id="655ae-1708">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="655ae-1709">Pour soumettre un travail sur un cluster appartenant à un autre espace de travail/groupe de ressources, indiquez l’ID ARM du cluster via l’option `--cluster`</span><span class="sxs-lookup"><span data-stu-id="655ae-1709">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="655ae-1710">[CHANGEMENT CASSANT] Suppression de l’attribut `location` des travaux, clusters et serveurs de fichiers.</span><span class="sxs-lookup"><span data-stu-id="655ae-1710">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="655ae-1711">L’emplacement est maintenant un attribut d’espace de travail.</span><span class="sxs-lookup"><span data-stu-id="655ae-1711">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="655ae-1712">[CHANGEMENT CASSANT] Suppression de `--location` des commandes `job create`, `cluster create` et `file-server create`</span><span class="sxs-lookup"><span data-stu-id="655ae-1712">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="655ae-1713">[CHANGEMENT CASSANT] Modification des noms des options courtes pour rendre l’interface plus cohérente :</span><span class="sxs-lookup"><span data-stu-id="655ae-1713">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="655ae-1714">[`--config`, `-c`] renommé en [`--config-file`, `-f`]</span><span class="sxs-lookup"><span data-stu-id="655ae-1714">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="655ae-1715">[`--cluster`, `-r`] renommé en [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="655ae-1715">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="655ae-1716">[`--cluster`, `-n`] renommé en [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="655ae-1716">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="655ae-1717">[`--job`, `-n`] renommé en [`--job`, `-j`]</span><span class="sxs-lookup"><span data-stu-id="655ae-1717">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="655ae-1718">Cartes</span><span class="sxs-lookup"><span data-stu-id="655ae-1718">Maps</span></span>

* <span data-ttu-id="655ae-1719">[CHANGEMENT CASSANT] Modification de `maps account create` pour accepter les Conditions d’utilisation, soit par l’invite interactive ou par l’indicateur `--accept-tos`</span><span class="sxs-lookup"><span data-stu-id="655ae-1719">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="655ae-1720">Réseau</span><span class="sxs-lookup"><span data-stu-id="655ae-1720">Network</span></span>

* <span data-ttu-id="655ae-1721">Ajout de la prise en charge de `https` à `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="655ae-1721">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="655ae-1722">Correction d’un problème où `--endpoint-status` était sensible à la casse.</span><span class="sxs-lookup"><span data-stu-id="655ae-1722">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="655ae-1723">#6502</span><span class="sxs-lookup"><span data-stu-id="655ae-1723">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="655ae-1724">Réservations</span><span class="sxs-lookup"><span data-stu-id="655ae-1724">Reservations</span></span>

* <span data-ttu-id="655ae-1725">[CHANGEMENT CASSANT] Ajout du paramètre obligatoire `ReservedResourceType` à `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="655ae-1725">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="655ae-1726">Ajout du paramètre `Location` à `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="655ae-1726">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="655ae-1727">[CHANGEMENT CASSANT] Suppression de `kind` de `ReservationProperties`</span><span class="sxs-lookup"><span data-stu-id="655ae-1727">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="655ae-1728">[CHANGEMENT CASSANT] `capabilities` renommé en `sku_properties` dans `Catalog`</span><span class="sxs-lookup"><span data-stu-id="655ae-1728">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="655ae-1729">[CHANGEMENT CASSANT] Suppression des propriétés `size` et `tier` de `Catalog`</span><span class="sxs-lookup"><span data-stu-id="655ae-1729">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="655ae-1730">Ajout du paramètre `InstanceFlexibility` à `reservations reservation update`</span><span class="sxs-lookup"><span data-stu-id="655ae-1730">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="655ae-1731">Role</span><span class="sxs-lookup"><span data-stu-id="655ae-1731">Role</span></span>

* <span data-ttu-id="655ae-1732">Amélioration de la gestion des erreurs</span><span class="sxs-lookup"><span data-stu-id="655ae-1732">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="655ae-1733">SQL</span><span class="sxs-lookup"><span data-stu-id="655ae-1733">SQL</span></span>

* <span data-ttu-id="655ae-1734">Correction de l’erreur déroutante lors de l’exécution de `az sql db list-editions` pour un emplacement qui n’est pas disponible pour votre abonnement</span><span class="sxs-lookup"><span data-stu-id="655ae-1734">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="655ae-1735">Stockage</span><span class="sxs-lookup"><span data-stu-id="655ae-1735">Storage</span></span>

* <span data-ttu-id="655ae-1736">Modification de la sortie de table pour que `storage blob download` soit plus lisible</span><span class="sxs-lookup"><span data-stu-id="655ae-1736">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="655ae-1737">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="655ae-1737">VM</span></span>

* <span data-ttu-id="655ae-1738">Amélioration de la vérification de la taille de la machine virtuelle pour la prise en charge de la mise en réseau accélérée dans `vm create`</span><span class="sxs-lookup"><span data-stu-id="655ae-1738">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="655ae-1739">Ajout d’un avertissement pour `vmss create` indiquant que la taille de la machine virtuelle par défaut va passer de `Standard_D1_v2` à `Standard_DS1_v2`</span><span class="sxs-lookup"><span data-stu-id="655ae-1739">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="655ae-1740">Ajout de `--force-update` à `[vm|vmss] extension set` pour mettre à jour l’extension, même lorsque la configuration n’a pas changé</span><span class="sxs-lookup"><span data-stu-id="655ae-1740">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="655ae-1741">13 juin 2018</span><span class="sxs-lookup"><span data-stu-id="655ae-1741">June 13, 2018</span></span>

<span data-ttu-id="655ae-1742">Version 2.0.37</span><span class="sxs-lookup"><span data-stu-id="655ae-1742">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="655ae-1743">Core</span><span class="sxs-lookup"><span data-stu-id="655ae-1743">Core</span></span>

* <span data-ttu-id="655ae-1744">Amélioration de la télémétrie interactive</span><span class="sxs-lookup"><span data-stu-id="655ae-1744">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="655ae-1745">13 juin 2018</span><span class="sxs-lookup"><span data-stu-id="655ae-1745">June 13, 2018</span></span>

<span data-ttu-id="655ae-1746">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="655ae-1746">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="655ae-1747">AKS</span><span class="sxs-lookup"><span data-stu-id="655ae-1747">AKS</span></span>

* <span data-ttu-id="655ae-1748">Ajout d’options réseau avancées à `aks create`</span><span class="sxs-lookup"><span data-stu-id="655ae-1748">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="655ae-1749">Ajout d’arguments à `aks create` pour permettre la surveillance et le routage HTTP</span><span class="sxs-lookup"><span data-stu-id="655ae-1749">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="655ae-1750">Ajout de l’argument `--no-ssh-key` à `aks create`</span><span class="sxs-lookup"><span data-stu-id="655ae-1750">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="655ae-1751">Ajout de l’argument `--enable-rbac` à `aks create`</span><span class="sxs-lookup"><span data-stu-id="655ae-1751">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="655ae-1752">[PRÉVERSION] Ajout de la prise en charge pour l’authentification basée sur Azure Active Directory à `aks create`</span><span class="sxs-lookup"><span data-stu-id="655ae-1752">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="655ae-1753">AppService</span><span class="sxs-lookup"><span data-stu-id="655ae-1753">AppService</span></span>

* <span data-ttu-id="655ae-1754">Résolution d’un problème lié à des versions urllib incompatibles</span><span class="sxs-lookup"><span data-stu-id="655ae-1754">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="655ae-1755">5 juin 2018</span><span class="sxs-lookup"><span data-stu-id="655ae-1755">June 5, 2018</span></span>

<span data-ttu-id="655ae-1756">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="655ae-1756">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="655ae-1757">Interactive</span><span class="sxs-lookup"><span data-stu-id="655ae-1757">Interactive</span></span>

* <span data-ttu-id="655ae-1758">Ajout de limites aux dépendances du mode interactif</span><span class="sxs-lookup"><span data-stu-id="655ae-1758">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="655ae-1759">5 juin 2018</span><span class="sxs-lookup"><span data-stu-id="655ae-1759">June 5, 2018</span></span>

<span data-ttu-id="655ae-1760">Version 2.0.34</span><span class="sxs-lookup"><span data-stu-id="655ae-1760">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="655ae-1761">Core</span><span class="sxs-lookup"><span data-stu-id="655ae-1761">Core</span></span>

* <span data-ttu-id="655ae-1762">Prise en charge supplémentaire pour les références de ressources inter-client</span><span class="sxs-lookup"><span data-stu-id="655ae-1762">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="655ae-1763">Amélioration de la fiabilité de téléchargement des données de télémétrie</span><span class="sxs-lookup"><span data-stu-id="655ae-1763">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="655ae-1764">ACR</span><span class="sxs-lookup"><span data-stu-id="655ae-1764">ACR</span></span>

* <span data-ttu-id="655ae-1765">Prise en charge supplémentaire pour VSTS en tant qu’emplacement source distant</span><span class="sxs-lookup"><span data-stu-id="655ae-1765">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="655ae-1766">Ajout de la commande `acr import`</span><span class="sxs-lookup"><span data-stu-id="655ae-1766">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="655ae-1767">AKS</span><span class="sxs-lookup"><span data-stu-id="655ae-1767">AKS</span></span>

* <span data-ttu-id="655ae-1768">`aks get-credentials` a été modifié pour créer le fichier de configuration kube avec des autorisations de système de fichiers plus sécurisées</span><span class="sxs-lookup"><span data-stu-id="655ae-1768">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="655ae-1769">Batch</span><span class="sxs-lookup"><span data-stu-id="655ae-1769">Batch</span></span>

* <span data-ttu-id="655ae-1770">Résolution du bogue concernant la mise en forme dans la table de liste de pool [[problème #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="655ae-1770">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="655ae-1771">IOT</span><span class="sxs-lookup"><span data-stu-id="655ae-1771">IOT</span></span>

* <span data-ttu-id="655ae-1772">Prise en charge ajoutée pour la création de IoT Hubs de niveau de base</span><span class="sxs-lookup"><span data-stu-id="655ae-1772">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="655ae-1773">Réseau</span><span class="sxs-lookup"><span data-stu-id="655ae-1773">Network</span></span>

* <span data-ttu-id="655ae-1774">`network vnet peering` amélioré</span><span class="sxs-lookup"><span data-stu-id="655ae-1774">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="655ae-1775">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="655ae-1775">Policy Insights</span></span>

* <span data-ttu-id="655ae-1776">Version initiale</span><span class="sxs-lookup"><span data-stu-id="655ae-1776">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="655ae-1777">ARM</span><span class="sxs-lookup"><span data-stu-id="655ae-1777">ARM</span></span>

* <span data-ttu-id="655ae-1778">Ajout des commandes `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="655ae-1778">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="655ae-1779">SQL</span><span class="sxs-lookup"><span data-stu-id="655ae-1779">SQL</span></span>

* <span data-ttu-id="655ae-1780">Ajout de nouvelles commandes d’instance gérée :</span><span class="sxs-lookup"><span data-stu-id="655ae-1780">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="655ae-1781">Ajout de nouvelles commandes de base de données gérée :</span><span class="sxs-lookup"><span data-stu-id="655ae-1781">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="655ae-1782">Stockage</span><span class="sxs-lookup"><span data-stu-id="655ae-1782">Storage</span></span>

* <span data-ttu-id="655ae-1783">Ajout de types MimeTypes supplémentaires pour les formats json et javascript pour être déduit à partir des extensions de fichier</span><span class="sxs-lookup"><span data-stu-id="655ae-1783">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="655ae-1784">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="655ae-1784">VM</span></span>

* <span data-ttu-id="655ae-1785">`vm list-skus` a été modifié pour utiliser des colonnes corrigées et ajouter l’avertissement que `Tier` et `Size` seront supprimés</span><span class="sxs-lookup"><span data-stu-id="655ae-1785">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="655ae-1786">Ajout de l’option `--accelerated-networking` à `vm create`</span><span class="sxs-lookup"><span data-stu-id="655ae-1786">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="655ae-1787">Ajout de `--tags` à `identity create`</span><span class="sxs-lookup"><span data-stu-id="655ae-1787">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="655ae-1788">22 mai 2018</span><span class="sxs-lookup"><span data-stu-id="655ae-1788">May 22, 2018</span></span>

<span data-ttu-id="655ae-1789">Version 2.0.33</span><span class="sxs-lookup"><span data-stu-id="655ae-1789">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="655ae-1790">Core</span><span class="sxs-lookup"><span data-stu-id="655ae-1790">Core</span></span>

* <span data-ttu-id="655ae-1791">Ajout de la prise en charge pour le développement de `@` dans les noms de fichiers</span><span class="sxs-lookup"><span data-stu-id="655ae-1791">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="655ae-1792">ACS</span><span class="sxs-lookup"><span data-stu-id="655ae-1792">ACS</span></span>

* <span data-ttu-id="655ae-1793">Ajout de nouvelles commandes Dev Spaces `aks use-dev-spaces` et `aks remove-dev-spaces`</span><span class="sxs-lookup"><span data-stu-id="655ae-1793">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="655ae-1794">Faute de frappe corrigée dans un message d’aide</span><span class="sxs-lookup"><span data-stu-id="655ae-1794">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="655ae-1795">AppService</span><span class="sxs-lookup"><span data-stu-id="655ae-1795">AppService</span></span>

* <span data-ttu-id="655ae-1796">Amélioration des commandes de mise à jour générique</span><span class="sxs-lookup"><span data-stu-id="655ae-1796">Improved generic update commands</span></span>
* <span data-ttu-id="655ae-1797">Ajout de la prise en charge asynchrone pour `webapp deployment source config-zip`</span><span class="sxs-lookup"><span data-stu-id="655ae-1797">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="655ae-1798">Conteneur</span><span class="sxs-lookup"><span data-stu-id="655ae-1798">Container</span></span>

* <span data-ttu-id="655ae-1799">Prise en charge ajoutée pour l’exportation d’un groupe de conteneurs au format yaml</span><span class="sxs-lookup"><span data-stu-id="655ae-1799">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="655ae-1800">Prise en charge ajoutée pour l’utilisation d’un fichier yaml afin de créer/mettre à jour un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="655ae-1800">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="655ae-1801">Extension</span><span class="sxs-lookup"><span data-stu-id="655ae-1801">Extension</span></span>

* <span data-ttu-id="655ae-1802">Amélioration de la suppression des extensions</span><span class="sxs-lookup"><span data-stu-id="655ae-1802">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="655ae-1803">Interactive</span><span class="sxs-lookup"><span data-stu-id="655ae-1803">Interactive</span></span>

* <span data-ttu-id="655ae-1804">La journalisation a été modifiée pour désactiver l’analyseur pour les saisies semi-automatiques</span><span class="sxs-lookup"><span data-stu-id="655ae-1804">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="655ae-1805">Gestion améliorée des caches d’aide incorrects</span><span class="sxs-lookup"><span data-stu-id="655ae-1805">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="655ae-1806">KeyVault</span><span class="sxs-lookup"><span data-stu-id="655ae-1806">KeyVault</span></span>

* <span data-ttu-id="655ae-1807">Commandes keyvault corrigées afin de fonctionner dans Cloud Shell ou dans des machines virtuelles avec l’identité</span><span class="sxs-lookup"><span data-stu-id="655ae-1807">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="655ae-1808">Réseau</span><span class="sxs-lookup"><span data-stu-id="655ae-1808">Network</span></span>

* <span data-ttu-id="655ae-1809">Résolution d’un problème où `network watcher show-topology` ne fonctionnait pas avec le nom de réseau virtuel et/ou de sous-réseau [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="655ae-1809">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="655ae-1810">Correction d’un problème où certaines commandes `network watcher` revendiquaient que Network Watcher n’était pas activé pour certaines régions alors qu’il l’était [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="655ae-1810">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="655ae-1811">SQL</span><span class="sxs-lookup"><span data-stu-id="655ae-1811">SQL</span></span>

* <span data-ttu-id="655ae-1812">[CHANGEMENT CASSANT] Objets de réponse retournés modifiés à partir des commandes `db` et `dw`</span><span class="sxs-lookup"><span data-stu-id="655ae-1812">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="655ae-1813">Propriété `serviceLevelObjective` renommée en `currentServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="655ae-1813">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="655ae-1814">Suppression des propriétés `currentServiceObjectiveId` et `requestedServiceObjectiveId`</span><span class="sxs-lookup"><span data-stu-id="655ae-1814">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="655ae-1815">Propriété `maxSizeBytes` modifiée en valeur entière au lieu d’une chaîne</span><span class="sxs-lookup"><span data-stu-id="655ae-1815">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="655ae-1816">[CHANGEMENT CASSANT] Les propriétés `db` et `dw` suivantes ont été modifiées pour être en lecture seule :</span><span class="sxs-lookup"><span data-stu-id="655ae-1816">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="655ae-1817">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="655ae-1817">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="655ae-1818">Pour mettre à jour, utilisez le paramètre `--service-objective` ou définissez la propriété `sku.name`</span><span class="sxs-lookup"><span data-stu-id="655ae-1818">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="655ae-1819">`edition`.</span><span class="sxs-lookup"><span data-stu-id="655ae-1819">`edition`.</span></span> <span data-ttu-id="655ae-1820">Pour mettre à jour, utilisez le paramètre `--edition` ou définissez la propriété `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="655ae-1820">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="655ae-1821">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="655ae-1821">`elasticPoolName`.</span></span> <span data-ttu-id="655ae-1822">Pour mettre à jour, utilisez le paramètre `--elastic-pool` ou définissez la propriété `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="655ae-1822">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="655ae-1823">[CHANGEMENT CASSANT] Les propriétés `elastic-pool` suivantes ont été modifiées pour être en lecture seule :</span><span class="sxs-lookup"><span data-stu-id="655ae-1823">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="655ae-1824">`edition`.</span><span class="sxs-lookup"><span data-stu-id="655ae-1824">`edition`.</span></span> <span data-ttu-id="655ae-1825">Pour mettre à jour, utilisez le paramètre `--edition`</span><span class="sxs-lookup"><span data-stu-id="655ae-1825">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="655ae-1826">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="655ae-1826">`dtu`.</span></span> <span data-ttu-id="655ae-1827">Pour mettre à jour, utilisez le paramètre `--capacity`</span><span class="sxs-lookup"><span data-stu-id="655ae-1827">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="655ae-1828">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="655ae-1828">`databaseDtuMin`.</span></span> <span data-ttu-id="655ae-1829">Pour mettre à jour, utilisez le paramètre `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="655ae-1829">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="655ae-1830">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="655ae-1830">`databaseDtuMax`.</span></span> <span data-ttu-id="655ae-1831">Pour mettre à jour, utilisez le paramètre `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="655ae-1831">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="655ae-1832">Ajout des paramètres `--family` et `--capacity` aux commandes `db`, `dw` et `elastic-pool`</span><span class="sxs-lookup"><span data-stu-id="655ae-1832">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="655ae-1833">Ajout de formateurs de table aux commandes `db`, `dw` et `elastic-pool`</span><span class="sxs-lookup"><span data-stu-id="655ae-1833">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="655ae-1834">Stockage</span><span class="sxs-lookup"><span data-stu-id="655ae-1834">Storage</span></span>

* <span data-ttu-id="655ae-1835">Ajout d’un compléteur pour l’argument `--account-name`</span><span class="sxs-lookup"><span data-stu-id="655ae-1835">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="655ae-1836">Correction d’un problème avec `storage entity query`</span><span class="sxs-lookup"><span data-stu-id="655ae-1836">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="655ae-1837">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="655ae-1837">VM</span></span>

* <span data-ttu-id="655ae-1838">[CHANGEMENT CASSANT] Suppression de `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="655ae-1838">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="655ae-1839">La même prise en charge est accessible via `vm update` ou `vm disk attach`</span><span class="sxs-lookup"><span data-stu-id="655ae-1839">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="655ae-1840">Correction de l’image de l’extension efficace dans `[vm|vmss] extension`</span><span class="sxs-lookup"><span data-stu-id="655ae-1840">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="655ae-1841">Ajout de`--boot-diagnostics-storage` à `vm create` pour capturer le journal de démarrage</span><span class="sxs-lookup"><span data-stu-id="655ae-1841">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="655ae-1842">Ajout de `--license-type` à `[vm|vmss] update`</span><span class="sxs-lookup"><span data-stu-id="655ae-1842">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="655ae-1843">7 mai 2018</span><span class="sxs-lookup"><span data-stu-id="655ae-1843">May 7, 2018</span></span>

<span data-ttu-id="655ae-1844">Version 2.0.32</span><span class="sxs-lookup"><span data-stu-id="655ae-1844">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="655ae-1845">Core</span><span class="sxs-lookup"><span data-stu-id="655ae-1845">Core</span></span>

* <span data-ttu-id="655ae-1846">Correction d’une exception non gérée lors de la récupération des clés secrètes à partir d’un compte de principal de service avec certificat</span><span class="sxs-lookup"><span data-stu-id="655ae-1846">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="655ae-1847">Nouvelle prise en charge limitée pour les arguments positionnels</span><span class="sxs-lookup"><span data-stu-id="655ae-1847">Added limited support for positional arguments</span></span>
* <span data-ttu-id="655ae-1848">Correction d’un problème où `--query` ne pouvait pas être utilisé avec `--ids`.</span><span class="sxs-lookup"><span data-stu-id="655ae-1848">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="655ae-1849">#5591</span><span class="sxs-lookup"><span data-stu-id="655ae-1849">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="655ae-1850">Amélioration des scénarios de redirection à partir des commandes en utilisant `--ids`.</span><span class="sxs-lookup"><span data-stu-id="655ae-1850">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="655ae-1851">Prend en charge `-o tsv` avec une requête spécifiée ou `-o json` sans spécification de requête</span><span class="sxs-lookup"><span data-stu-id="655ae-1851">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="655ae-1852">Ajout de suggestions de commande en cas d’erreur engendrées par des fautes de frappe des utilisateurs dans les commandes</span><span class="sxs-lookup"><span data-stu-id="655ae-1852">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="655ae-1853">Amélioration de l’erreur lorsque les utilisateurs entrent `az ''`</span><span class="sxs-lookup"><span data-stu-id="655ae-1853">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="655ae-1854">Ajout de la prise en charge des types de ressources personnalisés pour les modules et les extensions de commande</span><span class="sxs-lookup"><span data-stu-id="655ae-1854">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="655ae-1855">ACR</span><span class="sxs-lookup"><span data-stu-id="655ae-1855">ACR</span></span>

* <span data-ttu-id="655ae-1856">Ajout de commandes de build de l’ACR</span><span class="sxs-lookup"><span data-stu-id="655ae-1856">Added ACR Build commands</span></span>
* <span data-ttu-id="655ae-1857">Améliorations des messages d’erreur dus aux ressources introuvables</span><span class="sxs-lookup"><span data-stu-id="655ae-1857">Improved resource not found error messages</span></span>
* <span data-ttu-id="655ae-1858">Amélioration des performances de création de ressources et de la gestion des erreurs</span><span class="sxs-lookup"><span data-stu-id="655ae-1858">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="655ae-1859">Amélioration de la connexion ACR dans des consoles non standards et des WSL</span><span class="sxs-lookup"><span data-stu-id="655ae-1859">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="655ae-1860">Amélioration des messages d’erreur dus aux commandes de dépôt</span><span class="sxs-lookup"><span data-stu-id="655ae-1860">Improved repository commands error messages</span></span>
* <span data-ttu-id="655ae-1861">Mise à jour des colonnes de la table et du classement</span><span class="sxs-lookup"><span data-stu-id="655ae-1861">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="655ae-1862">ACS</span><span class="sxs-lookup"><span data-stu-id="655ae-1862">ACS</span></span>

* <span data-ttu-id="655ae-1863">Ajout d’un avertissement indiquant que `az aks` est un service en préversion</span><span class="sxs-lookup"><span data-stu-id="655ae-1863">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="655ae-1864">Résolution du problème d’autorisation dans `aks install-connector` lorsque `--aci-resource-group` n’est pas spécifié</span><span class="sxs-lookup"><span data-stu-id="655ae-1864">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="655ae-1865">AMS</span><span class="sxs-lookup"><span data-stu-id="655ae-1865">AMS</span></span>

* <span data-ttu-id="655ae-1866">Version initiale - Gérer des ressources Azure Media Services</span><span class="sxs-lookup"><span data-stu-id="655ae-1866">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="655ae-1867">AppService</span><span class="sxs-lookup"><span data-stu-id="655ae-1867">Appservice</span></span>

* <span data-ttu-id="655ae-1868">Correction d’un bogue dans `webapp delete` lorsque `--slot` est fourni</span><span class="sxs-lookup"><span data-stu-id="655ae-1868">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="655ae-1869">`--runtime-version` retiré de `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="655ae-1869">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="655ae-1870">Ajout de la prise en charge de min\_tls\_version & https2.0</span><span class="sxs-lookup"><span data-stu-id="655ae-1870">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="655ae-1871">Ajout de la prise en charge pour les multiconteneurs</span><span class="sxs-lookup"><span data-stu-id="655ae-1871">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="655ae-1872">Batch AI</span><span class="sxs-lookup"><span data-stu-id="655ae-1872">Batch AI</span></span>

* <span data-ttu-id="655ae-1873">`batchai create cluster` modifié pour respecter la priorité de machine virtuelle configurée dans le fichier de configuration du cluster</span><span class="sxs-lookup"><span data-stu-id="655ae-1873">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="655ae-1874">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="655ae-1874">Cognitive Services</span></span>

* <span data-ttu-id="655ae-1875">Faute de frappe corrigée dans l’exemple de `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="655ae-1875">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="655ae-1876">Consommation</span><span class="sxs-lookup"><span data-stu-id="655ae-1876">Consumption</span></span>

* <span data-ttu-id="655ae-1877">Ajout de nouvelles commandes pour l’API Budget</span><span class="sxs-lookup"><span data-stu-id="655ae-1877">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="655ae-1878">Conteneur</span><span class="sxs-lookup"><span data-stu-id="655ae-1878">Container</span></span>

* <span data-ttu-id="655ae-1879">Suppression de l’exigence pour `--registry-server` pour `container create` lorsqu’un serveur de registre est inclus dans le nom de l’image</span><span class="sxs-lookup"><span data-stu-id="655ae-1879">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="655ae-1880">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="655ae-1880">Cosmos DB</span></span>

* <span data-ttu-id="655ae-1881">Présentation de la prise en charge d’un réseau virtuel pour Azure CLI - Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="655ae-1881">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="655ae-1882">DMS</span><span class="sxs-lookup"><span data-stu-id="655ae-1882">DMS</span></span>

* <span data-ttu-id="655ae-1883">Version initiale - Ajoute la prise en charge de l’instruction SQL pour le scénario de migration de SQL Azure</span><span class="sxs-lookup"><span data-stu-id="655ae-1883">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="655ae-1884">Extension</span><span class="sxs-lookup"><span data-stu-id="655ae-1884">Extension</span></span>

* <span data-ttu-id="655ae-1885">Correction d’un bogue où les métadonnées d’extension cessaient d’être affichées</span><span class="sxs-lookup"><span data-stu-id="655ae-1885">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="655ae-1886">Interactive</span><span class="sxs-lookup"><span data-stu-id="655ae-1886">Interactive</span></span>

* <span data-ttu-id="655ae-1887">Autorise le fonctionnement de compléments interactifs avec des arguments positionnel</span><span class="sxs-lookup"><span data-stu-id="655ae-1887">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="655ae-1888">Sortie plus conviviale lorsque les utilisateurs entrent \'</span><span class="sxs-lookup"><span data-stu-id="655ae-1888">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="655ae-1889">Achèvements corrigés pour les paramètres sans aide</span><span class="sxs-lookup"><span data-stu-id="655ae-1889">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="655ae-1890">Descriptions corrigées pour les groupes de commandes</span><span class="sxs-lookup"><span data-stu-id="655ae-1890">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="655ae-1891">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="655ae-1891">Lab</span></span>

* <span data-ttu-id="655ae-1892">Régressions corrigées de conversion Knack</span><span class="sxs-lookup"><span data-stu-id="655ae-1892">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="655ae-1893">Réseau</span><span class="sxs-lookup"><span data-stu-id="655ae-1893">Network</span></span>

* <span data-ttu-id="655ae-1894">[CHANGEMENT CASSANT] Suppression du paramètre `--ids` pour :</span><span class="sxs-lookup"><span data-stu-id="655ae-1894">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="655ae-1895">Profil</span><span class="sxs-lookup"><span data-stu-id="655ae-1895">Profile</span></span>

* <span data-ttu-id="655ae-1896">Correction de la détection de source `disk create`</span><span class="sxs-lookup"><span data-stu-id="655ae-1896">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="655ae-1897">[CHANGEMENT CASSANT] Suppression de `--msi-port` et `--identity-port` car ils ne sont plus utilisés</span><span class="sxs-lookup"><span data-stu-id="655ae-1897">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="655ae-1898">Correction d’une faute de frappe dans le bref résumé de `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="655ae-1898">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="655ae-1899">Redis</span><span class="sxs-lookup"><span data-stu-id="655ae-1899">Redis</span></span>

* <span data-ttu-id="655ae-1900">`redis patch-schedule patch-schedule show` déconseillé en faveur de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="655ae-1900">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="655ae-1901">`redis list-all` déconseillé.</span><span class="sxs-lookup"><span data-stu-id="655ae-1901">Deprecated `redis list-all`.</span></span> <span data-ttu-id="655ae-1902">Cette fonctionnalité a été pliée dans `redis list`</span><span class="sxs-lookup"><span data-stu-id="655ae-1902">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="655ae-1903">`redis import-method` déconseillé en faveur de `redis import`</span><span class="sxs-lookup"><span data-stu-id="655ae-1903">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="655ae-1904">Ajout de la prise en charge de `--ids` pour diverses commandes</span><span class="sxs-lookup"><span data-stu-id="655ae-1904">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="655ae-1905">Role</span><span class="sxs-lookup"><span data-stu-id="655ae-1905">Role</span></span>

* <span data-ttu-id="655ae-1906">[CHANGEMENT CASSANT] Suppression de `ad sp reset-credentials` déconseillé</span><span class="sxs-lookup"><span data-stu-id="655ae-1906">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="655ae-1907">Stockage</span><span class="sxs-lookup"><span data-stu-id="655ae-1907">Storage</span></span>

* <span data-ttu-id="655ae-1908">Autorise l’application du jeton SAS de destination pour une copie d’objets blob si le SAS source et la clé de compte ne sont pas spécifiés</span><span class="sxs-lookup"><span data-stu-id="655ae-1908">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="655ae-1909">Exposé--délai d’expiration de socket pour les chargements et téléchargements d’objets blob</span><span class="sxs-lookup"><span data-stu-id="655ae-1909">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="655ae-1910">Traite les noms d’objets blob commençant par des séparateurs de chemin d’accès comme des chemins d’accès relatifs</span><span class="sxs-lookup"><span data-stu-id="655ae-1910">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="655ae-1911">Autorise `storage blob copy --source-sas` avec le caractère de démarrage de requête, « ? »</span><span class="sxs-lookup"><span data-stu-id="655ae-1911">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="655ae-1912">`storage entity query --marker` corrigé pour accepter une liste de clé =valeurs</span><span class="sxs-lookup"><span data-stu-id="655ae-1912">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="655ae-1913">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="655ae-1913">VM</span></span>

* <span data-ttu-id="655ae-1914">Correction d’une logique de détection invalide sur l’URI de l’objet blob non gérée</span><span class="sxs-lookup"><span data-stu-id="655ae-1914">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="655ae-1915">Ajout de la prise en charge du chiffrement de disque sans principaux de service fournis par l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="655ae-1915">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="655ae-1916">[CHANGEMENT CASSANT] Ne pas utiliser « ManagedIdentityExtension » de machine virtuelle pour la prise en charge de MSI</span><span class="sxs-lookup"><span data-stu-id="655ae-1916">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="655ae-1917">Ajout de la prise en charge pour la stratégie d’éviction vers `vmss`</span><span class="sxs-lookup"><span data-stu-id="655ae-1917">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="655ae-1918">[CHANGEMENT CASSANT] Suppression de `--ids` de :</span><span class="sxs-lookup"><span data-stu-id="655ae-1918">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="655ae-1919">Ajout de la prise en charge des accélérateurs d’écriture</span><span class="sxs-lookup"><span data-stu-id="655ae-1919">Added write accelerator support</span></span>
* <span data-ttu-id="655ae-1920">Ajout de `vmss perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="655ae-1920">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="655ae-1921">Correction de `vm diagnostics set` pour détecter la fiabilité du type de système d’exploitation de la machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="655ae-1921">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="655ae-1922">Modification de `vm resize` pour vérifier si la taille demandée est différente de celle actuellement définie et pour mettre à jour uniquement en cas de modifications</span><span class="sxs-lookup"><span data-stu-id="655ae-1922">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="655ae-1923">10 avril 2018</span><span class="sxs-lookup"><span data-stu-id="655ae-1923">April 10, 2018</span></span>

<span data-ttu-id="655ae-1924">Version 2.0.31</span><span class="sxs-lookup"><span data-stu-id="655ae-1924">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="655ae-1925">ACR</span><span class="sxs-lookup"><span data-stu-id="655ae-1925">ACR</span></span>

* <span data-ttu-id="655ae-1926">Gestion améliorée des erreurs de secours wincred</span><span class="sxs-lookup"><span data-stu-id="655ae-1926">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="655ae-1927">ACS</span><span class="sxs-lookup"><span data-stu-id="655ae-1927">ACS</span></span>

* <span data-ttu-id="655ae-1928">Modification de la durée de validité des SPN créés par AKS à 5 ans</span><span class="sxs-lookup"><span data-stu-id="655ae-1928">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="655ae-1929">AppService</span><span class="sxs-lookup"><span data-stu-id="655ae-1929">Appservice</span></span>

* [CHANGEMENT CASSANT]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="655ae-1931">Correction d’une exception non interceptée pour les plans webapp inexistants</span><span class="sxs-lookup"><span data-stu-id="655ae-1931">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="655ae-1932">Batch AI</span><span class="sxs-lookup"><span data-stu-id="655ae-1932">BatchAI</span></span>

* <span data-ttu-id="655ae-1933">Ajout de la prise en charge de l’API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="655ae-1933">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="655ae-1934">Montage au niveau du travail</span><span class="sxs-lookup"><span data-stu-id="655ae-1934">Job level mounting</span></span>
  - <span data-ttu-id="655ae-1935">Variables d’environnement avec les valeurs des secrets</span><span class="sxs-lookup"><span data-stu-id="655ae-1935">Environment variables with secret values</span></span>
  - <span data-ttu-id="655ae-1936">Paramètres des compteurs de performances</span><span class="sxs-lookup"><span data-stu-id="655ae-1936">Performance counters settings</span></span>
  - <span data-ttu-id="655ae-1937">Création de rapports de segments de ligne spécifiques à un travail</span><span class="sxs-lookup"><span data-stu-id="655ae-1937">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="655ae-1938">Prise en charge des sous-dossiers dans les listes de fichiers de l’API</span><span class="sxs-lookup"><span data-stu-id="655ae-1938">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="655ae-1939">Création de rapports d’utilisation et de limites</span><span class="sxs-lookup"><span data-stu-id="655ae-1939">Usage and limits reporting</span></span>
  - <span data-ttu-id="655ae-1940">Autorisation de la spécification du type de mise en cache pour les serveurs NFS</span><span class="sxs-lookup"><span data-stu-id="655ae-1940">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="655ae-1941">Prise en charge des images personnalisées</span><span class="sxs-lookup"><span data-stu-id="655ae-1941">Support for custom images</span></span>
  - <span data-ttu-id="655ae-1942">Ajout de la prise en charge de la boîte à outils pyTorch</span><span class="sxs-lookup"><span data-stu-id="655ae-1942">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="655ae-1943">Ajout de la commande `job wait` qui permet d’attendre la fin du travail et d’obtenir le code de sortie du travail</span><span class="sxs-lookup"><span data-stu-id="655ae-1943">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="655ae-1944">Ajout de la commande `usage show` pour répertorier l’utilisation actuelle des ressources Batch AI et les limites pour les différentes régions</span><span class="sxs-lookup"><span data-stu-id="655ae-1944">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="655ae-1945">Prise en charge des clouds nationaux</span><span class="sxs-lookup"><span data-stu-id="655ae-1945">National clouds are supported</span></span>
* <span data-ttu-id="655ae-1946">Ajout d’arguments de ligne de commande de travail pour monter des systèmes de fichiers au niveau du travail en plus des fichiers de configuration</span><span class="sxs-lookup"><span data-stu-id="655ae-1946">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="655ae-1947">Ajout de plus d’options pour personnaliser les clusters : priorité des machines virtuelles, sous-réseau, nombre de nœuds initial pour les clusters avec mise à l’échelle automatique, spécification d’une image personnalisée</span><span class="sxs-lookup"><span data-stu-id="655ae-1947">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="655ae-1948">Ajout d’une option de ligne de commande pour spécifier le type de mise en cache pour les NFS gérés par Batch AI</span><span class="sxs-lookup"><span data-stu-id="655ae-1948">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="655ae-1949">Simplification de la spécification du montage du système de fichiers dans les fichiers config.</span><span class="sxs-lookup"><span data-stu-id="655ae-1949">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="655ae-1950">Il est désormais possible d’omettre les informations d’identification pour les partages de fichiers Azure et les conteneurs d’objets blob Azure : CLI remplira les informations d’identification manquantes à l’aide de la clé du compte de stockage fournie par le biais des paramètres de ligne de commande ou spécifiée via la variable d’environnement, ou interrogera la clé à partir du stockage Azure (si le compte de stockage appartient à l’abonnement actuel)</span><span class="sxs-lookup"><span data-stu-id="655ae-1950">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="655ae-1951">La commande de flux de fichiers de travail se remplit désormais automatiquement lorsque le travail est terminé (réussite, échec, terminé ou supprimé)</span><span class="sxs-lookup"><span data-stu-id="655ae-1951">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="655ae-1952">Amélioration de la sortie `table` pour les opérations `show`</span><span class="sxs-lookup"><span data-stu-id="655ae-1952">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="655ae-1953">Ajout de l’option `--use-auto-storage` pour la création du cluster.</span><span class="sxs-lookup"><span data-stu-id="655ae-1953">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="655ae-1954">Cette option simplifie la gestion des comptes de stockage et le montage de partages de fichiers Azure et de conteneurs d’objets blob Azure vers des clusters</span><span class="sxs-lookup"><span data-stu-id="655ae-1954">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="655ae-1955">Ajout de l’option `--generate-ssh-keys` à `cluster create` et `file-server create`</span><span class="sxs-lookup"><span data-stu-id="655ae-1955">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="655ae-1956">Ajout de la possibilité de fournir la tâche de configuration de nœud via la ligne de commande</span><span class="sxs-lookup"><span data-stu-id="655ae-1956">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="655ae-1957">[CHANGEMENT CASSANT] Déplacement des commandes `job stream-file` et `job list-files` sous le groupe `job file`</span><span class="sxs-lookup"><span data-stu-id="655ae-1957">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="655ae-1958">[CHANGEMENT CASSANT] Renommage de `--admin-user-name` en `--user-name` dans la commande `file-server create` pour être cohérent avec la commande `cluster create`</span><span class="sxs-lookup"><span data-stu-id="655ae-1958">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="655ae-1959">Facturation</span><span class="sxs-lookup"><span data-stu-id="655ae-1959">Billing</span></span>

* <span data-ttu-id="655ae-1960">Ajout de commandes d’inscription de compte</span><span class="sxs-lookup"><span data-stu-id="655ae-1960">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="655ae-1961">Consommation</span><span class="sxs-lookup"><span data-stu-id="655ae-1961">Consumption</span></span>

* <span data-ttu-id="655ae-1962">Ajout des commandes `marketplace`</span><span class="sxs-lookup"><span data-stu-id="655ae-1962">Added `marketplace` commands</span></span>
* <span data-ttu-id="655ae-1963">[CHANGEMENT CASSANT] Renommage de `reservations summaries` en `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="655ae-1963">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="655ae-1964">[CHANGEMENT CASSANT] Renommage de `reservations details` en `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="655ae-1964">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="655ae-1965">[CHANGEMENT CASSANT] Suppression des options abrégées de `--reservation-order-id` et `--reservation-id` pour les commandes `reservation`</span><span class="sxs-lookup"><span data-stu-id="655ae-1965">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="655ae-1966">[CHANGEMENT CASSANT] Suppression des options abrégées de `--grain` pour les commandes `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="655ae-1966">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="655ae-1967">[CHANGEMENT CASSANT] Suppression des options abrégées de `--include-meter-details` pour les commandes `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="655ae-1967">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="655ae-1968">Conteneur</span><span class="sxs-lookup"><span data-stu-id="655ae-1968">Container</span></span>

* <span data-ttu-id="655ae-1969">Ajout des paramètres de montage de volume de référentiel Git `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` et `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="655ae-1969">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="655ae-1970">Résolution de [#5926](https://github.com/Azure/azure-cli/issues/5926) : `az container exec` échoue lorsque le nom du conteneur -- est spécifié</span><span class="sxs-lookup"><span data-stu-id="655ae-1970">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="655ae-1971">Extension</span><span class="sxs-lookup"><span data-stu-id="655ae-1971">Extension</span></span>

* <span data-ttu-id="655ae-1972">Modification du message de vérification de distribution pour qu’il soit au niveau du débogage</span><span class="sxs-lookup"><span data-stu-id="655ae-1972">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="655ae-1973">Interactive</span><span class="sxs-lookup"><span data-stu-id="655ae-1973">Interactive</span></span>

* <span data-ttu-id="655ae-1974">Modification pour arrêter la saisie semi-automatique sur les commandes non reconnues</span><span class="sxs-lookup"><span data-stu-id="655ae-1974">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="655ae-1975">Ajout d’événements de raccordement avant et après la création du sous-arbre de commande</span><span class="sxs-lookup"><span data-stu-id="655ae-1975">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="655ae-1976">Ajout de la saisie semi-automatique pour les paramètres `--ids`</span><span class="sxs-lookup"><span data-stu-id="655ae-1976">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="655ae-1977">Réseau</span><span class="sxs-lookup"><span data-stu-id="655ae-1977">Network</span></span>

* <span data-ttu-id="655ae-1978">Résolution de [#5936](https://github.com/Azure/azure-cli/issues/5936) : les balises `application-gateway create` n’ont pas pu déterminer l’ensemble</span><span class="sxs-lookup"><span data-stu-id="655ae-1978">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="655ae-1979">Ajout de l’argument `--auth-certs` pour joindre des certificats d’authentification pour `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="655ae-1979">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="655ae-1980">#4910</span><span class="sxs-lookup"><span data-stu-id="655ae-1980">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="655ae-1981">Ajout de commandes `ddos-protection` pour créer des plans de protection DDoS</span><span class="sxs-lookup"><span data-stu-id="655ae-1981">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="655ae-1982">Prise en charge de `--ddos-protection-plan` pour `vnet [create|update]` pour associer un réseau virtuel à un plan de protection DDoS</span><span class="sxs-lookup"><span data-stu-id="655ae-1982">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="655ae-1983">Résolution du problème avec l’ indicateur `--disable-bgp-route-propagation` dans `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="655ae-1983">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="655ae-1984">Suppression des arguments factices `--public-ip-address-type` et `--subnet-type` pour `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="655ae-1984">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="655ae-1985">Ajout de la prise en charge des enregistrements TXT avec les séquences d’échappement RFC 1035 à `network dns zone [import|export]` et `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="655ae-1985">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="655ae-1986">Profil</span><span class="sxs-lookup"><span data-stu-id="655ae-1986">Profile</span></span>

* <span data-ttu-id="655ae-1987">Ajout de la prise en charge des comptes Azure Classic dans `account list`</span><span class="sxs-lookup"><span data-stu-id="655ae-1987">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="655ae-1988">[CHANGEMENT CASSANT] Suppression des arguments `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="655ae-1988">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="655ae-1989">SGBDR</span><span class="sxs-lookup"><span data-stu-id="655ae-1989">RDBMS</span></span>

* <span data-ttu-id="655ae-1990">Ajout de la commande `georestore`</span><span class="sxs-lookup"><span data-stu-id="655ae-1990">Added `georestore` command</span></span>
* <span data-ttu-id="655ae-1991">Suppression de la restriction de taille de stockage de la commande `create`</span><span class="sxs-lookup"><span data-stu-id="655ae-1991">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="655ae-1992">Ressource</span><span class="sxs-lookup"><span data-stu-id="655ae-1992">Resource</span></span>

* <span data-ttu-id="655ae-1993">Ajout de la prise en charge de `--metadata` pour `policy definition create`</span><span class="sxs-lookup"><span data-stu-id="655ae-1993">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="655ae-1994">Ajout de la prise en charge de `--metadata`, `--set`, `--add` et `--remove` à `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="655ae-1994">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="655ae-1995">SQL</span><span class="sxs-lookup"><span data-stu-id="655ae-1995">SQL</span></span>

* <span data-ttu-id="655ae-1996">Ajout de `sql elastic-pool op list` et `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="655ae-1996">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="655ae-1997">Stockage</span><span class="sxs-lookup"><span data-stu-id="655ae-1997">Storage</span></span>

* <span data-ttu-id="655ae-1998">Amélioration des messages d’erreur pour les chaînes de connexion incorrectes</span><span class="sxs-lookup"><span data-stu-id="655ae-1998">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="655ae-1999">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="655ae-1999">VM</span></span>

* <span data-ttu-id="655ae-2000">Ajout de la prise en charge pour configurer le nombre de domaines d’erreur de plateforme sur `vmss create`</span><span class="sxs-lookup"><span data-stu-id="655ae-2000">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="655ae-2001">Modification de `vmss create` sur la valeur par défaut de l’équilibreur de charge Standard pour les groupes identiques désactivés zonaux, grands ou avec un seul groupe de placement</span><span class="sxs-lookup"><span data-stu-id="655ae-2001">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [CHANGEMENT CASSANT]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="655ae-2003">Ajout de la prise en charge des références SKU d’IP public à `vm create`</span><span class="sxs-lookup"><span data-stu-id="655ae-2003">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="655ae-2004">Ajout des arguments `--keyvault` et `--resource-group` à `vm secret format` pour prendre en charge des scénarios où la commande ne parvient pas à résoudre l’ID de coffre.</span><span class="sxs-lookup"><span data-stu-id="655ae-2004">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="655ae-2005">#5718</span><span class="sxs-lookup"><span data-stu-id="655ae-2005">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="655ae-2006">Amélioration des erreurs pour `[vm|vmss create]` lorsque l’emplacement d’un groupe de ressources ne possède aucune prise en charge de zone</span><span class="sxs-lookup"><span data-stu-id="655ae-2006">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="655ae-2007">27 mars 2018</span><span class="sxs-lookup"><span data-stu-id="655ae-2007">March 27, 2018</span></span>

<span data-ttu-id="655ae-2008">Version 2.0.30</span><span class="sxs-lookup"><span data-stu-id="655ae-2008">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="655ae-2009">Core</span><span class="sxs-lookup"><span data-stu-id="655ae-2009">Core</span></span>

* <span data-ttu-id="655ae-2010">Afficher le message pour les extensions marquées en tant que préversions dans l’aide</span><span class="sxs-lookup"><span data-stu-id="655ae-2010">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="655ae-2011">ACS</span><span class="sxs-lookup"><span data-stu-id="655ae-2011">ACS</span></span>

* <span data-ttu-id="655ae-2012">Corriger l’erreur de vérification de certificat SSL pour `aks install-cli` dans Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="655ae-2012">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="655ae-2013">AppService</span><span class="sxs-lookup"><span data-stu-id="655ae-2013">Appservice</span></span>

* <span data-ttu-id="655ae-2014">Ajout de la prise en charge HTTPS exclusive à `webapp update`</span><span class="sxs-lookup"><span data-stu-id="655ae-2014">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="655ae-2015">Ajout de la prise en charge des emplacements à `az webapp identity [assign|show]` et `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="655ae-2015">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="655ae-2016">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="655ae-2016">Backup</span></span>

* <span data-ttu-id="655ae-2017">Ajout de la commande `az backup protection isenabled-for-vm`</span><span class="sxs-lookup"><span data-stu-id="655ae-2017">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="655ae-2018">Cette commande peut être utilisée pour vérifier si une machine virtuelle est sauvegardée par un coffre dans l’abonnement</span><span class="sxs-lookup"><span data-stu-id="655ae-2018">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="655ae-2019">Activation des ID d’objet Azure pour les paramètres `--resource-group` et `--vault-name`, pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="655ae-2019">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="655ae-2020">Modification des paramètres `--name` pour accepter le format de sortie des commandes `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="655ae-2020">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="655ae-2021">Conteneur</span><span class="sxs-lookup"><span data-stu-id="655ae-2021">Container</span></span>

* <span data-ttu-id="655ae-2022">Ajout de la commande `container exec`</span><span class="sxs-lookup"><span data-stu-id="655ae-2022">Added `container exec` command.</span></span> <span data-ttu-id="655ae-2023">Exécute les commandes dans un conteneur, pour un groupe de conteneurs en exécution.</span><span class="sxs-lookup"><span data-stu-id="655ae-2023">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="655ae-2024">Autoriser la sortie de table pour la création et la mise à jour d’un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="655ae-2024">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="655ae-2025">Extension</span><span class="sxs-lookup"><span data-stu-id="655ae-2025">Extension</span></span>

* <span data-ttu-id="655ae-2026">Ajout d’un message pour `extension add` si l’extension est en préversion</span><span class="sxs-lookup"><span data-stu-id="655ae-2026">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="655ae-2027">Modification de `extension list-available` afin d’afficher les données complètes d’extension avec `--show-details`</span><span class="sxs-lookup"><span data-stu-id="655ae-2027">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="655ae-2028">[CHANGEMENT CASSANT] Modification de `extension list-available` afin d’afficher les données simplifiées d’extension par défaut</span><span class="sxs-lookup"><span data-stu-id="655ae-2028">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="655ae-2029">Interactive</span><span class="sxs-lookup"><span data-stu-id="655ae-2029">Interactive</span></span>

* <span data-ttu-id="655ae-2030">Modification des saisies semi-automatiques pour procéder à l’activation dès le chargement de la table de commande</span><span class="sxs-lookup"><span data-stu-id="655ae-2030">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="655ae-2031">Correction du bogue par l’exécution du paramètre `--style`</span><span class="sxs-lookup"><span data-stu-id="655ae-2031">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="655ae-2032">Analyseur lexical interactif instancié après le vidage de la table de commande, si manquant</span><span class="sxs-lookup"><span data-stu-id="655ae-2032">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="655ae-2033">Amélioration de la prise en charge de Completer</span><span class="sxs-lookup"><span data-stu-id="655ae-2033">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="655ae-2034">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="655ae-2034">Lab</span></span>

* <span data-ttu-id="655ae-2035">Correction des bogues avec la commande `create environment`</span><span class="sxs-lookup"><span data-stu-id="655ae-2035">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="655ae-2036">Surveiller</span><span class="sxs-lookup"><span data-stu-id="655ae-2036">Monitor</span></span>

* <span data-ttu-id="655ae-2037">Ajout de la prise en charge de `--top`, `--orderby` et `--namespace` à `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="655ae-2037">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="655ae-2038">Résolution de [#4529](https://github.com/Azure/azure-cli/issues/5785) : `metrics list` accepte une liste de mesures séparées par des espaces pour la récupération</span><span class="sxs-lookup"><span data-stu-id="655ae-2038">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="655ae-2039">Ajout de la prise en charge de `--namespace` à `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="655ae-2039">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="655ae-2040">Réseau</span><span class="sxs-lookup"><span data-stu-id="655ae-2040">Network</span></span>

* <span data-ttu-id="655ae-2041">Ajout de la prise en charge des zones de DNS privé</span><span class="sxs-lookup"><span data-stu-id="655ae-2041">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="655ae-2042">Profil</span><span class="sxs-lookup"><span data-stu-id="655ae-2042">Profile</span></span>

* <span data-ttu-id="655ae-2043">Ajout d’un avertissement pour `--identity-port` et `--msi-port` à `login`</span><span class="sxs-lookup"><span data-stu-id="655ae-2043">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="655ae-2044">SGBDR</span><span class="sxs-lookup"><span data-stu-id="655ae-2044">RDBMS</span></span>

* <span data-ttu-id="655ae-2045">Ajout de la version d’API mise à la disposition générale du modèle d’entreprise 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="655ae-2045">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="655ae-2046">Ressource</span><span class="sxs-lookup"><span data-stu-id="655ae-2046">Resource</span></span>

* [CHANGEMENT CASSANT]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="655ae-2048">Role</span><span class="sxs-lookup"><span data-stu-id="655ae-2048">Role</span></span>

* <span data-ttu-id="655ae-2049">Ajout de la prise en charge des configurations d’accès et des clients natifs requis à `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="655ae-2049">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="655ae-2050">Modification des commandes `rbac` afin de renvoyer moins de 1 000 ID sur la résolution d’objet</span><span class="sxs-lookup"><span data-stu-id="655ae-2050">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="655ae-2051">Ajout des commandes de gestion des informations d’identification `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="655ae-2051">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="655ae-2052">[CHANGEMENT CASSANT] Suppression des propriétés de la sortie `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="655ae-2052">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="655ae-2053">Ajout de la prise en charge des autorisations `dataActions` et `notDataActions` à `role definition`</span><span class="sxs-lookup"><span data-stu-id="655ae-2053">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="655ae-2054">Stockage</span><span class="sxs-lookup"><span data-stu-id="655ae-2054">Storage</span></span>

* <span data-ttu-id="655ae-2055">Résolution du problème lié au chargement des fichiers présentant une taille comprise entre 195 Go et 200 Go</span><span class="sxs-lookup"><span data-stu-id="655ae-2055">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="655ae-2056">Résolution de [#4049](https://github.com/Azure/azure-cli/issues/4049) : problèmes avec les chargements d’objets blob d’ajout ignorant les paramètres de condition</span><span class="sxs-lookup"><span data-stu-id="655ae-2056">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="655ae-2057">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="655ae-2057">VM</span></span>

* <span data-ttu-id="655ae-2058">Ajout d’un avertissement à `vmss create` concernant les changements cassants à venir pour les ensembles comprenant plus de 100 instances</span><span class="sxs-lookup"><span data-stu-id="655ae-2058">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="655ae-2059">Ajout de la prise en charge de la résilience dans la zone à `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="655ae-2059">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="655ae-2060">Modification de la vue d’instance de disque pour signaler un meilleur état de chiffrement</span><span class="sxs-lookup"><span data-stu-id="655ae-2060">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="655ae-2061">[CHANGEMENT CASSANT] Modification de `vm extension delete` afin d’annuler la capacité de génération de sortie</span><span class="sxs-lookup"><span data-stu-id="655ae-2061">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="655ae-2062">13 mars 2018</span><span class="sxs-lookup"><span data-stu-id="655ae-2062">March 13, 2018</span></span>

<span data-ttu-id="655ae-2063">Version 2.0.29</span><span class="sxs-lookup"><span data-stu-id="655ae-2063">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="655ae-2064">ACR</span><span class="sxs-lookup"><span data-stu-id="655ae-2064">ACR</span></span>

* <span data-ttu-id="655ae-2065">Ajout de la prise en charge du paramètre `--image` pour `repository delete`</span><span class="sxs-lookup"><span data-stu-id="655ae-2065">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="655ae-2066">Paramètres `--manifest` et `--tag` de la commande `repository delete` déconseillés</span><span class="sxs-lookup"><span data-stu-id="655ae-2066">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="655ae-2067">Ajout de la commande `repository untag` pour supprimer une balise sans supprimer les données</span><span class="sxs-lookup"><span data-stu-id="655ae-2067">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="655ae-2068">ACS</span><span class="sxs-lookup"><span data-stu-id="655ae-2068">ACS</span></span>

* <span data-ttu-id="655ae-2069">Ajout de la commande `aks upgrade-connector` pour mettre à niveau un connecteur existant</span><span class="sxs-lookup"><span data-stu-id="655ae-2069">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="655ae-2070">Modification des fichiers de configuration `kubectl` pour utiliser un YAML de style bloc plus lisible</span><span class="sxs-lookup"><span data-stu-id="655ae-2070">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="655ae-2071">Advisor</span><span class="sxs-lookup"><span data-stu-id="655ae-2071">Advisor</span></span>

* <span data-ttu-id="655ae-2072">[CHANGEMENT CASSANT] Renommage de `advisor configuration get` en `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="655ae-2072">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="655ae-2073">[CHANGEMENT CASSANT] Renommage de `advisor configuration set` en `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="655ae-2073">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="655ae-2074">[CHANGEMENT CASSANT] Suppression de `advisor recommendation generate`</span><span class="sxs-lookup"><span data-stu-id="655ae-2074">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="655ae-2075">Ajout du paramètre `--refresh` pour `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="655ae-2075">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="655ae-2076">Ajout de la commande `advisor recommendation show`</span><span class="sxs-lookup"><span data-stu-id="655ae-2076">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="655ae-2077">AppService</span><span class="sxs-lookup"><span data-stu-id="655ae-2077">Appservice</span></span>

* <span data-ttu-id="655ae-2078">`[webapp|functionapp] assign-identity` déconseillé</span><span class="sxs-lookup"><span data-stu-id="655ae-2078">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="655ae-2079">Ajout des commandes d’identité gérée `webapp identity [assign|show]` et `functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="655ae-2079">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="655ae-2080">Eventhubs</span><span class="sxs-lookup"><span data-stu-id="655ae-2080">Eventhubs</span></span>

* <span data-ttu-id="655ae-2081">Version initiale</span><span class="sxs-lookup"><span data-stu-id="655ae-2081">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="655ae-2082">Extension</span><span class="sxs-lookup"><span data-stu-id="655ae-2082">Extension</span></span>

* <span data-ttu-id="655ae-2083">Ajout d’un contrôle supplémentaire pour avertir l’utilisateur si le distributeur utilisé est différent de celui stocké dans le fichier source du package, car cela peut entraîner des erreurs</span><span class="sxs-lookup"><span data-stu-id="655ae-2083">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="655ae-2084">Interactive</span><span class="sxs-lookup"><span data-stu-id="655ae-2084">Interactive</span></span>

* <span data-ttu-id="655ae-2085">Résolution de [#5625](https://github.com/Azure/azure-cli/issues/5625) : conservation de l’historique entre différentes sessions</span><span class="sxs-lookup"><span data-stu-id="655ae-2085">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="655ae-2086">Résolution de [#3016](https://github.com/Azure/azure-cli/issues/3016) : historique non enregistré alors qu’il était dans la portée</span><span class="sxs-lookup"><span data-stu-id="655ae-2086">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="655ae-2087">Résolution de [#5688](https://github.com/Azure/azure-cli/issues/5688) : la saisie automatique n’apparaît pas si le chargement de la table de commande a rencontré une exception</span><span class="sxs-lookup"><span data-stu-id="655ae-2087">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="655ae-2088">Résolu : indicateur de progression pour les opérations à long terme</span><span class="sxs-lookup"><span data-stu-id="655ae-2088">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="655ae-2089">Surveiller</span><span class="sxs-lookup"><span data-stu-id="655ae-2089">Monitor</span></span>

* <span data-ttu-id="655ae-2090">Les commandes `monitor autoscale-settings` ont été déconseillées</span><span class="sxs-lookup"><span data-stu-id="655ae-2090">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="655ae-2091">Ajout des commandes `monitor autoscale`</span><span class="sxs-lookup"><span data-stu-id="655ae-2091">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="655ae-2092">Ajout des commandes `monitor autoscale profile`</span><span class="sxs-lookup"><span data-stu-id="655ae-2092">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="655ae-2093">Ajout des commandes `monitor autoscale rule`</span><span class="sxs-lookup"><span data-stu-id="655ae-2093">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="655ae-2094">Réseau</span><span class="sxs-lookup"><span data-stu-id="655ae-2094">Network</span></span>

* <span data-ttu-id="655ae-2095">[CHANGEMENT CASSANT] Suppression du paramètre `--tags` de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="655ae-2095">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="655ae-2096">Suppression de certaines valeurs par défaut erronées pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="655ae-2096">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="655ae-2097">Ajout des commandes `network watcher connection-monitor`</span><span class="sxs-lookup"><span data-stu-id="655ae-2097">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="655ae-2098">Ajout des paramètres `--vnet` et `--subnet` à `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="655ae-2098">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="655ae-2099">Profil</span><span class="sxs-lookup"><span data-stu-id="655ae-2099">Profile</span></span>

* <span data-ttu-id="655ae-2100">Paramètre `--msi` déconseillé pour `az login`</span><span class="sxs-lookup"><span data-stu-id="655ae-2100">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="655ae-2101">Ajout du paramètre `--identity` pour `az login` afin de remplacer `--msi`</span><span class="sxs-lookup"><span data-stu-id="655ae-2101">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="655ae-2102">SGBDR</span><span class="sxs-lookup"><span data-stu-id="655ae-2102">RDBMS</span></span>

* <span data-ttu-id="655ae-2103">[PRÉVERSION] Modifiée pour utiliser l’API 2017-12-01-préversion</span><span class="sxs-lookup"><span data-stu-id="655ae-2103">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="655ae-2104">Service Bus</span><span class="sxs-lookup"><span data-stu-id="655ae-2104">Service Bus</span></span>

* <span data-ttu-id="655ae-2105">Version initiale</span><span class="sxs-lookup"><span data-stu-id="655ae-2105">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="655ae-2106">Stockage</span><span class="sxs-lookup"><span data-stu-id="655ae-2106">Storage</span></span>

* <span data-ttu-id="655ae-2107">Résolution de [#4971](https://github.com/Azure/azure-cli/issues/4971) : `storage blob copy` prend désormais en charge les autres clouds Azure</span><span class="sxs-lookup"><span data-stu-id="655ae-2107">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="655ae-2108">Résolution de [#5286](https://github.com/Azure/azure-cli/issues/5286) : les commandes batch `storage blob [delete-batch|download-batch|upload-batch]` ne génèrent plus d’erreur lors d’échecs de la condition préalable</span><span class="sxs-lookup"><span data-stu-id="655ae-2108">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="655ae-2109">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="655ae-2109">VM</span></span>

* <span data-ttu-id="655ae-2110">Ajout de prise en charge de `[vm|vmss] create` pour attacher des disques de données non gérées et configurer la mise en cache</span><span class="sxs-lookup"><span data-stu-id="655ae-2110">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="655ae-2111">`[vm|vmss] assign-identity` et `[vm|vmss] remove-identity` sont déconseillés</span><span class="sxs-lookup"><span data-stu-id="655ae-2111">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="655ae-2112">Ajout des commandes `vm identity [assign|remove|show]` et `vmss identity [assign|remove|show]` pour remplacer des commandes déconseillées</span><span class="sxs-lookup"><span data-stu-id="655ae-2112">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="655ae-2113">Modification de la priorité par défaut dans `vmss create` à None</span><span class="sxs-lookup"><span data-stu-id="655ae-2113">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="655ae-2114">27 février 2018</span><span class="sxs-lookup"><span data-stu-id="655ae-2114">February 27, 2018</span></span>

<span data-ttu-id="655ae-2115">Version 2.0.28</span><span class="sxs-lookup"><span data-stu-id="655ae-2115">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="655ae-2116">Core</span><span class="sxs-lookup"><span data-stu-id="655ae-2116">Core</span></span>

* <span data-ttu-id="655ae-2117">Résolution de [#5184](https://github.com/Azure/azure-cli/issues/5184) : problème d’installation d’Homebrew</span><span class="sxs-lookup"><span data-stu-id="655ae-2117">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="655ae-2118">Ajout de la prise en charge de télémétrie d’extension avec des clés personnalisées</span><span class="sxs-lookup"><span data-stu-id="655ae-2118">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="655ae-2119">Ajout de la connexion HTTP à `--debug`</span><span class="sxs-lookup"><span data-stu-id="655ae-2119">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="655ae-2120">ACS</span><span class="sxs-lookup"><span data-stu-id="655ae-2120">ACS</span></span>

* <span data-ttu-id="655ae-2121">Modification pour utiliser le graphique Helm `virtual-kubelet-for-aks` pour `aks install-connector` par défaut</span><span class="sxs-lookup"><span data-stu-id="655ae-2121">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="655ae-2122">Résolution de #7161 : autorisation insuffisante des principaux de service pour la création de groupe de conteneurs ACI</span><span class="sxs-lookup"><span data-stu-id="655ae-2122">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="655ae-2123">Ajout des paramètres `--aci-container-group`, `--location` et `--image-tag` à `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="655ae-2123">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="655ae-2124">Suppression de l’avis de désapprobation de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="655ae-2124">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="655ae-2125">AppService</span><span class="sxs-lookup"><span data-stu-id="655ae-2125">Appservice</span></span>

* <span data-ttu-id="655ae-2126">Mises à jour pour la nouvelle version du kit de développement logiciel (SDK) (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="655ae-2126">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="655ae-2127">Résolu [#5538](https://github.com/Azure/azure-cli/issues/5538) : `Free` défini comme une SKU invalide</span><span class="sxs-lookup"><span data-stu-id="655ae-2127">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="655ae-2128">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="655ae-2128">Cognitive Services</span></span>

* <span data-ttu-id="655ae-2129">Mise à jour de l’avis lors de la création d’un compte Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="655ae-2129">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="655ae-2130">Consommation</span><span class="sxs-lookup"><span data-stu-id="655ae-2130">Consumption</span></span>

* <span data-ttu-id="655ae-2131">Ajout de nouvelles commandes pour l’API priceSheet</span><span class="sxs-lookup"><span data-stu-id="655ae-2131">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="655ae-2132">Mise à jour des formats existants Détails d’utilisations et Détails de la réservation</span><span class="sxs-lookup"><span data-stu-id="655ae-2132">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="655ae-2133">Conteneur</span><span class="sxs-lookup"><span data-stu-id="655ae-2133">Container</span></span>

* <span data-ttu-id="655ae-2134">Ajout des arguments `--secrets` et `--secrets-mount-path` à `container create` pour utiliser des secrets dans ACI</span><span class="sxs-lookup"><span data-stu-id="655ae-2134">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="655ae-2135">Réseau</span><span class="sxs-lookup"><span data-stu-id="655ae-2135">Network</span></span>

* <span data-ttu-id="655ae-2136">Résolution de [#5559](https://github.com/Azure/azure-cli/issues/5559) : client manquant dans `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="655ae-2136">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="655ae-2137">Ressource</span><span class="sxs-lookup"><span data-stu-id="655ae-2137">Resource</span></span>

* <span data-ttu-id="655ae-2138">Modification de `group deployment export` pour afficher un modèle et des erreurs partiels sur échec</span><span class="sxs-lookup"><span data-stu-id="655ae-2138">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="655ae-2139">Role</span><span class="sxs-lookup"><span data-stu-id="655ae-2139">Role</span></span>

* <span data-ttu-id="655ae-2140">Ajout de `role assignment list-changelogs` pour permettre l’audit des rôles du principal de service</span><span class="sxs-lookup"><span data-stu-id="655ae-2140">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="655ae-2141">SQL</span><span class="sxs-lookup"><span data-stu-id="655ae-2141">SQL</span></span>

* <span data-ttu-id="655ae-2142">Ajout de la prise en charge de la redondance de zone pour les bases de données et les pools élastiques lors de création et mise à jour</span><span class="sxs-lookup"><span data-stu-id="655ae-2142">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="655ae-2143">Stockage</span><span class="sxs-lookup"><span data-stu-id="655ae-2143">Storage</span></span>

* <span data-ttu-id="655ae-2144">Activation de la spécification de préfixe/destination pour `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="655ae-2144">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="655ae-2145">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="655ae-2145">VM</span></span>

* <span data-ttu-id="655ae-2146">Ajout de prise en charge de jonction / séparation de disques sur une instance de groupe de machines virtuelles identiques uniques</span><span class="sxs-lookup"><span data-stu-id="655ae-2146">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="655ae-2147">13 février 2018</span><span class="sxs-lookup"><span data-stu-id="655ae-2147">February 13, 2018</span></span>

<span data-ttu-id="655ae-2148">Version 2.0.27</span><span class="sxs-lookup"><span data-stu-id="655ae-2148">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="655ae-2149">Core</span><span class="sxs-lookup"><span data-stu-id="655ae-2149">Core</span></span>

* <span data-ttu-id="655ae-2150">Modification de l’authentification pour passer au système de clé sur l’ID d’abonnement et le nom sur la connexion MSI</span><span class="sxs-lookup"><span data-stu-id="655ae-2150">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="655ae-2151">ACS</span><span class="sxs-lookup"><span data-stu-id="655ae-2151">ACS</span></span>

* <span data-ttu-id="655ae-2152">[CHANGEMENT CASSANT] Renommage de `aks get-versions` en `aks get-upgrades` pour des raisons de précision</span><span class="sxs-lookup"><span data-stu-id="655ae-2152">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="655ae-2153">Modification de `aks get-versions` pour afficher les versions Kubernetes disponibles pour `aks create`</span><span class="sxs-lookup"><span data-stu-id="655ae-2153">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="655ae-2154">Modification des valeurs par défaut de `aks create` de manière à laisser le serveur choisir la version de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="655ae-2154">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="655ae-2155">Mise à jour des messages d’aide faisant référence au principal du service généré par AKS</span><span class="sxs-lookup"><span data-stu-id="655ae-2155">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="655ae-2156">Modification des tailles de nœud par défaut pour `aks create` pour passer de « Standard\_D1\_v2 » à « Standard\_DS1\_v2 »</span><span class="sxs-lookup"><span data-stu-id="655ae-2156">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="655ae-2157">Meilleure fiabilité lors de la localisation du pod de tableau de bord pour `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="655ae-2157">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="655ae-2158">Correction de `aks get-credentials` pour gérer les erreurs Unicode lors du chargement des fichiers de configuration Kubernetes</span><span class="sxs-lookup"><span data-stu-id="655ae-2158">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="655ae-2159">Ajout d’un message à `az aks install-cli` pour aider à l’obtention de `kubectl` dans `$PATH`</span><span class="sxs-lookup"><span data-stu-id="655ae-2159">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="655ae-2160">AppService</span><span class="sxs-lookup"><span data-stu-id="655ae-2160">Appservice</span></span>

* <span data-ttu-id="655ae-2161">Résolution du problème dans lequel `webapp [backup|restore]` a échoué en raison d’une référence null</span><span class="sxs-lookup"><span data-stu-id="655ae-2161">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="655ae-2162">Ajout de la prise en charge supplémentaire des plans App Service par défaut via `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="655ae-2162">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="655ae-2163">CDN</span><span class="sxs-lookup"><span data-stu-id="655ae-2163">CDN</span></span>

* <span data-ttu-id="655ae-2164">Ajout des commandes `cdn custom-domain [enable-https|disable-https]`</span><span class="sxs-lookup"><span data-stu-id="655ae-2164">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="655ae-2165">Conteneur</span><span class="sxs-lookup"><span data-stu-id="655ae-2165">Container</span></span>

* <span data-ttu-id="655ae-2166">Ajout de l’option `--follow` à `az container logs` pour les journaux d’activité de diffusion en continu</span><span class="sxs-lookup"><span data-stu-id="655ae-2166">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="655ae-2167">Ajout de la commande `container attach` qui associe les flux d’erreur et de sortie standard locaux à un conteneur d’un groupe de conteneur</span><span class="sxs-lookup"><span data-stu-id="655ae-2167">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="655ae-2168">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="655ae-2168">CosmosDB</span></span>

* <span data-ttu-id="655ae-2169">Ajout de la prise en charge de la définition de fonctionnalités</span><span class="sxs-lookup"><span data-stu-id="655ae-2169">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="655ae-2170">Extension</span><span class="sxs-lookup"><span data-stu-id="655ae-2170">Extension</span></span>

* <span data-ttu-id="655ae-2171">Ajout de la prise en charge du paramètre `--pip-proxy` pour les commandes `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="655ae-2171">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="655ae-2172">Ajout de la prise en charge de l’argument `--pip-extra-index-urls` pour les commandes `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="655ae-2172">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="655ae-2173">Commentaires</span><span class="sxs-lookup"><span data-stu-id="655ae-2173">Feedback</span></span>

* <span data-ttu-id="655ae-2174">Ajout d’informations d’extension aux données de télémétrie</span><span class="sxs-lookup"><span data-stu-id="655ae-2174">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="655ae-2175">Interactive</span><span class="sxs-lookup"><span data-stu-id="655ae-2175">Interactive</span></span>

* <span data-ttu-id="655ae-2176">Résolution du problème dans lequel l’utilisateur est invité à se connecter à l’aide du mode interactif dans Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="655ae-2176">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="655ae-2177">Correction de la régression avec les listes de saisie semi-automatique des paramètres manquants</span><span class="sxs-lookup"><span data-stu-id="655ae-2177">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="655ae-2178">IoT</span><span class="sxs-lookup"><span data-stu-id="655ae-2178">IoT</span></span>

* <span data-ttu-id="655ae-2179">Résolution du problème dans lequel `iot dps access policy [create|update]` renvoie une erreur « introuvable » en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="655ae-2179">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="655ae-2180">Résolution du problème dans lequel `iot dps linked-hub [create|update]` renvoie une erreur « introuvable » en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="655ae-2180">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="655ae-2181">Ajout de la prise en charge de `--no-wait` pour `iot dps access policy [create|update]` et `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="655ae-2181">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="655ae-2182">Modification de `iot hub create` pour autoriser la spécification du nombre de partitions</span><span class="sxs-lookup"><span data-stu-id="655ae-2182">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="655ae-2183">Surveiller</span><span class="sxs-lookup"><span data-stu-id="655ae-2183">Monitor</span></span>

* <span data-ttu-id="655ae-2184">Correction de la commande `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="655ae-2184">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="655ae-2185">Réseau</span><span class="sxs-lookup"><span data-stu-id="655ae-2185">Network</span></span>

* <span data-ttu-id="655ae-2186">Correction de l’option `--tags` pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="655ae-2186">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="655ae-2187">Profil</span><span class="sxs-lookup"><span data-stu-id="655ae-2187">Profile</span></span>

* <span data-ttu-id="655ae-2188">Activation `az login` à partir du mode interactif</span><span class="sxs-lookup"><span data-stu-id="655ae-2188">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="655ae-2189">Ressource</span><span class="sxs-lookup"><span data-stu-id="655ae-2189">Resource</span></span>

* <span data-ttu-id="655ae-2190">Rajout de `feature show`</span><span class="sxs-lookup"><span data-stu-id="655ae-2190">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="655ae-2191">Role</span><span class="sxs-lookup"><span data-stu-id="655ae-2191">Role</span></span>

* <span data-ttu-id="655ae-2192">Ajout de l’argument `--available-to-other-tenants` à `ad app update`</span><span class="sxs-lookup"><span data-stu-id="655ae-2192">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="655ae-2193">SQL</span><span class="sxs-lookup"><span data-stu-id="655ae-2193">SQL</span></span>

* <span data-ttu-id="655ae-2194">Ajout des commandes `sql server dns-alias`</span><span class="sxs-lookup"><span data-stu-id="655ae-2194">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="655ae-2195">Ajout de `sql db rename`</span><span class="sxs-lookup"><span data-stu-id="655ae-2195">Added `sql db rename`</span></span>
* <span data-ttu-id="655ae-2196">Ajout de la prise en charge de l’argument `--ids` pour toutes les commandes sql</span><span class="sxs-lookup"><span data-stu-id="655ae-2196">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="655ae-2197">Stockage</span><span class="sxs-lookup"><span data-stu-id="655ae-2197">Storage</span></span>

* <span data-ttu-id="655ae-2198">Ajout des commandes `storage blob service-properties delete-policy` et `storage blob undelete` pour permettre une suppression réversible</span><span class="sxs-lookup"><span data-stu-id="655ae-2198">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="655ae-2199">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="655ae-2199">VM</span></span>

* <span data-ttu-id="655ae-2200">Correction d’un incident lorsque le chiffrement de la machine virtuelle ne peut pas être initialisé entièrement</span><span class="sxs-lookup"><span data-stu-id="655ae-2200">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="655ae-2201">Ajout de la sortie d’ID du principal lors de l’activation de MSI</span><span class="sxs-lookup"><span data-stu-id="655ae-2201">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="655ae-2202">`vm boot-diagnostics get-boot-log` fixe</span><span class="sxs-lookup"><span data-stu-id="655ae-2202">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="655ae-2203">31 janvier 2018</span><span class="sxs-lookup"><span data-stu-id="655ae-2203">January 31, 2018</span></span>

<span data-ttu-id="655ae-2204">Version 2.0.26</span><span class="sxs-lookup"><span data-stu-id="655ae-2204">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="655ae-2205">Core</span><span class="sxs-lookup"><span data-stu-id="655ae-2205">Core</span></span>

* <span data-ttu-id="655ae-2206">Ajout de la prise en charge de la récupération du jeton brut dans le contexte MSI</span><span class="sxs-lookup"><span data-stu-id="655ae-2206">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="655ae-2207">Suppression de la chaîne de l’indicateur d’interrogation après la fin de LRO sur le fichier cmd.exe de Windows</span><span class="sxs-lookup"><span data-stu-id="655ae-2207">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="655ae-2208">Ajout d’un avertissement qui s’affiche lorsque l’utilisation d’une valeur par défaut configurée a été remplacée par une entrée de niveau INFO.</span><span class="sxs-lookup"><span data-stu-id="655ae-2208">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="655ae-2209">Utilisation de `--verbose` pour voir</span><span class="sxs-lookup"><span data-stu-id="655ae-2209">Use `--verbose` to see</span></span>
* <span data-ttu-id="655ae-2210">Ajouter un indicateur de progression pour les commandes wait</span><span class="sxs-lookup"><span data-stu-id="655ae-2210">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="655ae-2211">ACS</span><span class="sxs-lookup"><span data-stu-id="655ae-2211">ACS</span></span>

* <span data-ttu-id="655ae-2212">Clarification de l’argument `--disable-browser`</span><span class="sxs-lookup"><span data-stu-id="655ae-2212">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="655ae-2213">Amélioration de la touche TAB pour les arguments `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="655ae-2213">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="655ae-2214">AppService</span><span class="sxs-lookup"><span data-stu-id="655ae-2214">Appservice</span></span>

* <span data-ttu-id="655ae-2215">`webapp log [tail|download]` fixe</span><span class="sxs-lookup"><span data-stu-id="655ae-2215">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="655ae-2216">Suppression de la vérification de `kind` sur les fonctions et les applications web</span><span class="sxs-lookup"><span data-stu-id="655ae-2216">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="655ae-2217">CDN</span><span class="sxs-lookup"><span data-stu-id="655ae-2217">CDN</span></span>

* <span data-ttu-id="655ae-2218">Résolution du problème de client manquant avec `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="655ae-2218">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="655ae-2219">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="655ae-2219">CosmosDB</span></span>

* <span data-ttu-id="655ae-2220">Correction de la description du paramètre pour les stratégies de basculement</span><span class="sxs-lookup"><span data-stu-id="655ae-2220">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="655ae-2221">Interactive</span><span class="sxs-lookup"><span data-stu-id="655ae-2221">Interactive</span></span>

* <span data-ttu-id="655ae-2222">Résolution du problème dans lequel les listes de saisie semi-automatique d’option de commande ne s’affichent plus</span><span class="sxs-lookup"><span data-stu-id="655ae-2222">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="655ae-2223">Réseau</span><span class="sxs-lookup"><span data-stu-id="655ae-2223">Network</span></span>

* <span data-ttu-id="655ae-2224">Ajout de la protection pour `--cert-password` à `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="655ae-2224">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="655ae-2225">Résolution du problème lié à `application-gateway update` où `--sku` a appliqué par erreur une valeur par défaut</span><span class="sxs-lookup"><span data-stu-id="655ae-2225">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="655ae-2226">Ajout de la protection pour `--shared-key` et `--authorization-key` à `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="655ae-2226">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="655ae-2227">Résolution du problème de client manquant avec `asg create`</span><span class="sxs-lookup"><span data-stu-id="655ae-2227">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="655ae-2228">Ajout du paramètre `--file-name / -f` pour les noms exportés à `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="655ae-2228">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="655ae-2229">Les problèmes suivants liés à `dns zone export` ont été résolus :</span><span class="sxs-lookup"><span data-stu-id="655ae-2229">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="655ae-2230">Résolution du problème dans lequel des enregistrements TXT longs ont été mal exportés</span><span class="sxs-lookup"><span data-stu-id="655ae-2230">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="655ae-2231">Résolution du problème dans lequel des enregistrements TXT entre guillemets ont été mal exportés sans guillemets placés dans une séquence d’échappement.</span><span class="sxs-lookup"><span data-stu-id="655ae-2231">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="655ae-2232">Résolution du problème où certains enregistrements ont été importés à deux reprises avec `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="655ae-2232">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="655ae-2233">Restauration des commandes `vnet-gateway root-cert` et `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="655ae-2233">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="655ae-2234">Profil</span><span class="sxs-lookup"><span data-stu-id="655ae-2234">Profile</span></span>

* <span data-ttu-id="655ae-2235">Correction de `get-access-token` pour qu’il fonctionne à l’intérieur d’une machine virtuelle avec l’identité</span><span class="sxs-lookup"><span data-stu-id="655ae-2235">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="655ae-2236">Ressource</span><span class="sxs-lookup"><span data-stu-id="655ae-2236">Resource</span></span>

* <span data-ttu-id="655ae-2237">Correction du bogue lié à `deployment [create|validate]` où un avertissement ne s’est pas affiché correctement quand un champ ’type’ du modèle contient des valeurs en majuscules</span><span class="sxs-lookup"><span data-stu-id="655ae-2237">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="655ae-2238">Stockage</span><span class="sxs-lookup"><span data-stu-id="655ae-2238">Storage</span></span>

* <span data-ttu-id="655ae-2239">Résolution du problème lié à la migration des comptes Storage V1 vers Storage V2</span><span class="sxs-lookup"><span data-stu-id="655ae-2239">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="655ae-2240">Ajout de la création progressive de rapports pour toutes les commandes de chargement/téléchargement</span><span class="sxs-lookup"><span data-stu-id="655ae-2240">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="655ae-2241">Résolution du bogue empêchant l’option d’argument « -n » avec `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="655ae-2241">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="655ae-2242">Ajout de la colonne de « snapshot » ajouté à la sortie de table pour `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="655ae-2242">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="655ae-2243">Résolution des bogues dans lesquels différents paramètres devaient être analysés en tant qu’entiers</span><span class="sxs-lookup"><span data-stu-id="655ae-2243">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="655ae-2244">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="655ae-2244">VM</span></span>

* <span data-ttu-id="655ae-2245">Ajout de la commande `vm image accept-terms` pour autoriser la création de machines virtuelles à partir d’images moyennant des frais supplémentaires</span><span class="sxs-lookup"><span data-stu-id="655ae-2245">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="655ae-2246">Correction de `[vm|vmss create]` pour garantir l’exécution des commandes sous un proxy avec des certificats non signés</span><span class="sxs-lookup"><span data-stu-id="655ae-2246">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="655ae-2247">[APERÇU] Ajout de la prise en charge de la priorité « faible» au groupe de machines virtuelles identiques</span><span class="sxs-lookup"><span data-stu-id="655ae-2247">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="655ae-2248">Ajout de la protection pour `--admin-password` à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="655ae-2248">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="655ae-2249">17 janvier 2018</span><span class="sxs-lookup"><span data-stu-id="655ae-2249">January 17, 2018</span></span>

<span data-ttu-id="655ae-2250">Version 2.0.25</span><span class="sxs-lookup"><span data-stu-id="655ae-2250">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="655ae-2251">ACR</span><span class="sxs-lookup"><span data-stu-id="655ae-2251">ACR</span></span>

* <span data-ttu-id="655ae-2252">Ajout d’une connexion acr de secours en cas d’erreurs d’informations d’identification Windows</span><span class="sxs-lookup"><span data-stu-id="655ae-2252">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="655ae-2253">Activation des journaux d’activité du Registre</span><span class="sxs-lookup"><span data-stu-id="655ae-2253">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="655ae-2254">ACS</span><span class="sxs-lookup"><span data-stu-id="655ae-2254">ACS</span></span>

* <span data-ttu-id="655ae-2255">Correction de la commande `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="655ae-2255">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="655ae-2256">Suppression de l’exigence de rôle SPN</span><span class="sxs-lookup"><span data-stu-id="655ae-2256">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="655ae-2257">AppService</span><span class="sxs-lookup"><span data-stu-id="655ae-2257">Appservice</span></span>

* <span data-ttu-id="655ae-2258">Correction du bogue avec `config ssl upload` où `hosting_environment_profile` avait la valeur null</span><span class="sxs-lookup"><span data-stu-id="655ae-2258">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="655ae-2259">Ajout de la prise en charge des URL personnalisées pour `browse`</span><span class="sxs-lookup"><span data-stu-id="655ae-2259">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="655ae-2260">Prise en charge de l’emplacement fixe pour `log tail`</span><span class="sxs-lookup"><span data-stu-id="655ae-2260">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="655ae-2261">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="655ae-2261">Backup</span></span>

* <span data-ttu-id="655ae-2262">Modification de l’option `--container-name` de `backup item list` désormais facultative</span><span class="sxs-lookup"><span data-stu-id="655ae-2262">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="655ae-2263">Ajout d’options de compte de stockage à `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="655ae-2263">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="655ae-2264">Correction de la vérification de l’emplacement dans `backup protection enable-for-vm`, ne tient désormais plus compte de la casse</span><span class="sxs-lookup"><span data-stu-id="655ae-2264">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="655ae-2265">Correction d’un problème qui causait l’échec des commandes avec un nom de conteneur non valide</span><span class="sxs-lookup"><span data-stu-id="655ae-2265">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="655ae-2266">Modification de `backup item list` pour inclure « État d’intégrité » par défaut</span><span class="sxs-lookup"><span data-stu-id="655ae-2266">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="655ae-2267">Batch</span><span class="sxs-lookup"><span data-stu-id="655ae-2267">Batch</span></span>

* <span data-ttu-id="655ae-2268">Modification de `batch login` pour retourner des détails d’authentification</span><span class="sxs-lookup"><span data-stu-id="655ae-2268">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="655ae-2269">Cloud</span><span class="sxs-lookup"><span data-stu-id="655ae-2269">Cloud</span></span>

* <span data-ttu-id="655ae-2270">Ne requiert plus de points de terminaison lors de la définition de `--profile` sur un cloud</span><span class="sxs-lookup"><span data-stu-id="655ae-2270">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="655ae-2271">Consommation</span><span class="sxs-lookup"><span data-stu-id="655ae-2271">Consumption</span></span>

* <span data-ttu-id="655ae-2272">Ajout de nouvelles commandes pour les réservations : `consumption reservations summaries` et `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="655ae-2272">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="655ae-2273">Event Grid</span><span class="sxs-lookup"><span data-stu-id="655ae-2273">Event Grid</span></span>

* <span data-ttu-id="655ae-2274">[CHANGEMENT CASSANT] Déplacement des commandes `az eventgrid topic event-subscription` vers `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="655ae-2274">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="655ae-2275">[CHANGEMENT CASSANT] Déplacement des commandes `az eventgrid resource event-subscription` vers `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="655ae-2275">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="655ae-2276">[CHANGEMENT CASSANT] Suppression de la commande `eventgrid event-subscription show-endpoint-url`</span><span class="sxs-lookup"><span data-stu-id="655ae-2276">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="655ae-2277">Utilisation de `eventgrid event-subscription show --include-full-endpoint-url` à la place</span><span class="sxs-lookup"><span data-stu-id="655ae-2277">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="655ae-2278">Ajout de la commande `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="655ae-2278">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="655ae-2279">Ajout de la commande `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="655ae-2279">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="655ae-2280">Ajout du paramètre `--ids` pour les commandes `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="655ae-2280">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="655ae-2281">Ajout de la prise en charge de la saisie semi-automatique via la touche TAB pour les noms de rubrique</span><span class="sxs-lookup"><span data-stu-id="655ae-2281">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="655ae-2282">Interactive</span><span class="sxs-lookup"><span data-stu-id="655ae-2282">Interactive</span></span>

* <span data-ttu-id="655ae-2283">Correction d’un problème qui empêchait le fonctionnement du mode interactif avec Python 2.x</span><span class="sxs-lookup"><span data-stu-id="655ae-2283">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="655ae-2284">Corrections d’erreurs au démarrage</span><span class="sxs-lookup"><span data-stu-id="655ae-2284">Fixed errors on startup</span></span>
* <span data-ttu-id="655ae-2285">Correction du problème de commandes ne s’exécutant pas en mode interactif</span><span class="sxs-lookup"><span data-stu-id="655ae-2285">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="655ae-2286">IoT</span><span class="sxs-lookup"><span data-stu-id="655ae-2286">IoT</span></span>

* <span data-ttu-id="655ae-2287">Ajout de la prise en charge du service de provisionnement des appareils</span><span class="sxs-lookup"><span data-stu-id="655ae-2287">Added support for device provisioning service</span></span>
* <span data-ttu-id="655ae-2288">Ajout de messages de désapprobation dans les commandes et l’aide relative aux commandes</span><span class="sxs-lookup"><span data-stu-id="655ae-2288">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="655ae-2289">Ajout de la vérification IoT pour informer les utilisateurs de l’extension IoT</span><span class="sxs-lookup"><span data-stu-id="655ae-2289">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="655ae-2290">Surveiller</span><span class="sxs-lookup"><span data-stu-id="655ae-2290">Monitor</span></span>

* <span data-ttu-id="655ae-2291">Ajout de la prise en charge des paramètres multi diagnostic.</span><span class="sxs-lookup"><span data-stu-id="655ae-2291">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="655ae-2292">Le paramètre `--name` est désormais requis pour `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="655ae-2292">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="655ae-2293">Ajout de la commande `monitor diagnostic-settings categories` pour obtenir la catégorie des paramètres de diagnostic</span><span class="sxs-lookup"><span data-stu-id="655ae-2293">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="655ae-2294">Réseau</span><span class="sxs-lookup"><span data-stu-id="655ae-2294">Network</span></span>

* <span data-ttu-id="655ae-2295">Résolution du problème se produisant lors de la tentative de passage au mode actif-passif, ou depuis ce dernier, avec `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="655ae-2295">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="655ae-2296">Ajout de la prise en charge de HTTP2 vers `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="655ae-2296">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="655ae-2297">Profil</span><span class="sxs-lookup"><span data-stu-id="655ae-2297">Profile</span></span>

* <span data-ttu-id="655ae-2298">Ajout de la prise en charge pour la connexion à l’aide d’identités affectées aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="655ae-2298">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="655ae-2299">Role</span><span class="sxs-lookup"><span data-stu-id="655ae-2299">Role</span></span>

* <span data-ttu-id="655ae-2300">Ajout de l’argument `--assignee-object-id` à `role assignment create` pour ignorer les requêtes de graphique</span><span class="sxs-lookup"><span data-stu-id="655ae-2300">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="655ae-2301">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="655ae-2301">Service Fabric</span></span>

* <span data-ttu-id="655ae-2302">Ajout d’erreurs détaillées à la réponse de validation lors de la création du cluster</span><span class="sxs-lookup"><span data-stu-id="655ae-2302">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="655ae-2303">Résolution du problème concernant le client manquant avec plusieurs commandes</span><span class="sxs-lookup"><span data-stu-id="655ae-2303">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="655ae-2304">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="655ae-2304">VM</span></span>

* <span data-ttu-id="655ae-2305">[PRÉVERSION] Prise en charge interzone pour `vmss`</span><span class="sxs-lookup"><span data-stu-id="655ae-2305">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="655ae-2306">[CHANGEMENT CASSANT] Modification de la valeur par défaut `vmss` de zone unique en équilibreur de charge « Standard »</span><span class="sxs-lookup"><span data-stu-id="655ae-2306">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="655ae-2307">[CHANGEMENT CASSANT] Modification de `externalIdentities` en `userAssignedIdentities` pour EMSI</span><span class="sxs-lookup"><span data-stu-id="655ae-2307">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="655ae-2308">[PRÉVERSION] Ajout de la prise en charge de l’échange de disque du système d’exploitation</span><span class="sxs-lookup"><span data-stu-id="655ae-2308">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="655ae-2309">Ajout de la prise en charge de l’utilisation des images de machine virtuelle à partir d’autres abonnements</span><span class="sxs-lookup"><span data-stu-id="655ae-2309">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="655ae-2310">Ajout des arguments `--plan-name`, `--plan-product`, `--plan-promotion-code` et `--plan-publisher` à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="655ae-2310">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="655ae-2311">Correction des problèmes d’erreur avec `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="655ae-2311">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="655ae-2312">Correction de l’utilisation excessive des ressources due à `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="655ae-2312">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="655ae-2313">19 décembre 2017</span><span class="sxs-lookup"><span data-stu-id="655ae-2313">December 19, 2017</span></span>

<span data-ttu-id="655ae-2314">Version 2.0.23</span><span class="sxs-lookup"><span data-stu-id="655ae-2314">Version 2.0.23</span></span>

* <span data-ttu-id="655ae-2315">Ajout de la prise en charge pour la connexion à l’aide d’identités affectées aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="655ae-2315">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="655ae-2316">Conteneur</span><span class="sxs-lookup"><span data-stu-id="655ae-2316">Container</span></span>

* <span data-ttu-id="655ae-2317">Correction de l’ordre incorrect des paramètres pour les journaux d’activité du conteneur</span><span class="sxs-lookup"><span data-stu-id="655ae-2317">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="655ae-2318">Réseau</span><span class="sxs-lookup"><span data-stu-id="655ae-2318">Network</span></span>

* <span data-ttu-id="655ae-2319">Ajout de l’argument `--disable-bgp-route-propagation` à `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="655ae-2319">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="655ae-2320">Ajout de l’argument `--ip-tags` à `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="655ae-2320">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="655ae-2321">Stockage</span><span class="sxs-lookup"><span data-stu-id="655ae-2321">Storage</span></span>

* <span data-ttu-id="655ae-2322">Ajout de la prise en charge du stockage V2</span><span class="sxs-lookup"><span data-stu-id="655ae-2322">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="655ae-2323">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="655ae-2323">VM</span></span>

* <span data-ttu-id="655ae-2324">[APERÇU] Ajout de la prise en charge des identités affectées aux utilisateurs pour les machines virtuelles et les VMSS</span><span class="sxs-lookup"><span data-stu-id="655ae-2324">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="655ae-2325">5 décembre 2017</span><span class="sxs-lookup"><span data-stu-id="655ae-2325">December 5, 2017</span></span>

<span data-ttu-id="655ae-2326">Version 2.0.22</span><span class="sxs-lookup"><span data-stu-id="655ae-2326">Version 2.0.22</span></span>

* <span data-ttu-id="655ae-2327">Suppression des commandes `az component`.</span><span class="sxs-lookup"><span data-stu-id="655ae-2327">Removed `az component` commands.</span></span> <span data-ttu-id="655ae-2328">Utilisation de `az extension` à la place</span><span class="sxs-lookup"><span data-stu-id="655ae-2328">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="655ae-2329">Core</span><span class="sxs-lookup"><span data-stu-id="655ae-2329">Core</span></span>
* <span data-ttu-id="655ae-2330">Modification du point de terminaison de l’autorité AAD `AZURE_US_GOV_CLOUD` pour le faire passer de login.microsoftonline.com à login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="655ae-2330">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="655ae-2331">Résolution du problème au cours duquel les données de télémétrie étaient constamment renvoyées</span><span class="sxs-lookup"><span data-stu-id="655ae-2331">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="655ae-2332">ACS</span><span class="sxs-lookup"><span data-stu-id="655ae-2332">ACS</span></span>

* <span data-ttu-id="655ae-2333">Ajout des commandes `aks install-connector` et `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="655ae-2333">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="655ae-2334">Amélioration des rapports d’erreurs pour `acs create`</span><span class="sxs-lookup"><span data-stu-id="655ae-2334">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="655ae-2335">Correction de l’utilisation de `aks get-credentials -f` sans chemin d’accès complet</span><span class="sxs-lookup"><span data-stu-id="655ae-2335">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="655ae-2336">Advisor</span><span class="sxs-lookup"><span data-stu-id="655ae-2336">Advisor</span></span>

* <span data-ttu-id="655ae-2337">Version initiale</span><span class="sxs-lookup"><span data-stu-id="655ae-2337">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="655ae-2338">AppService</span><span class="sxs-lookup"><span data-stu-id="655ae-2338">Appservice</span></span>

* <span data-ttu-id="655ae-2339">Correction de la génération du nom de certificat avec `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="655ae-2339">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="655ae-2340">Correction de `webapp [list|show]` et `functionapp [list|show]` de manière à afficher les applications correctes</span><span class="sxs-lookup"><span data-stu-id="655ae-2340">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="655ae-2341">Ajout de la valeur par défaut pour `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="655ae-2341">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="655ae-2342">Consommation</span><span class="sxs-lookup"><span data-stu-id="655ae-2342">Consumption</span></span>

* <span data-ttu-id="655ae-2343">Ajout de la prise en charge de l’API version 2017-11-30</span><span class="sxs-lookup"><span data-stu-id="655ae-2343">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="655ae-2344">Conteneur</span><span class="sxs-lookup"><span data-stu-id="655ae-2344">Container</span></span>

* <span data-ttu-id="655ae-2345">Correction de la régression des ports par défaut</span><span class="sxs-lookup"><span data-stu-id="655ae-2345">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="655ae-2346">Surveiller</span><span class="sxs-lookup"><span data-stu-id="655ae-2346">Monitor</span></span>

* <span data-ttu-id="655ae-2347">Ajout de la prise en charge de plusieurs dimensions à la commande des mesures</span><span class="sxs-lookup"><span data-stu-id="655ae-2347">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="655ae-2348">Ressource</span><span class="sxs-lookup"><span data-stu-id="655ae-2348">Resource</span></span>

* <span data-ttu-id="655ae-2349">Ajout de l’argument `--include-response-body` à `resource show`</span><span class="sxs-lookup"><span data-stu-id="655ae-2349">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="655ae-2350">Role</span><span class="sxs-lookup"><span data-stu-id="655ae-2350">Role</span></span>

* <span data-ttu-id="655ae-2351">Ajout de l’affichage des affectations par défaut pour les administrateurs « classiques » à `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="655ae-2351">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="655ae-2352">Ajout de la prise en charge à `ad sp reset-credentials` pour l’ajout d’informations d’identification au lieu de leur remplacement</span><span class="sxs-lookup"><span data-stu-id="655ae-2352">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="655ae-2353">Amélioration des rapports d’erreurs pour `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="655ae-2353">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="655ae-2354">SQL</span><span class="sxs-lookup"><span data-stu-id="655ae-2354">SQL</span></span>

* <span data-ttu-id="655ae-2355">Ajout des commandes `sql db list-usages` et `sql db show-usage`</span><span class="sxs-lookup"><span data-stu-id="655ae-2355">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="655ae-2356">Ajout des commandes `sql server conn-policy show` et `sql server conn-policy update`</span><span class="sxs-lookup"><span data-stu-id="655ae-2356">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="655ae-2357">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="655ae-2357">VM</span></span>

* <span data-ttu-id="655ae-2358">Ajout des informations de zone à `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="655ae-2358">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="655ae-2359">14 novembre 2017</span><span class="sxs-lookup"><span data-stu-id="655ae-2359">November 14, 2017</span></span>

<span data-ttu-id="655ae-2360">Version 2.0.21</span><span class="sxs-lookup"><span data-stu-id="655ae-2360">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="655ae-2361">ACR</span><span class="sxs-lookup"><span data-stu-id="655ae-2361">ACR</span></span>

* <span data-ttu-id="655ae-2362">Ajout de la prise en charge pour la création de webhooks dans les régions de réplication</span><span class="sxs-lookup"><span data-stu-id="655ae-2362">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="655ae-2363">ACS</span><span class="sxs-lookup"><span data-stu-id="655ae-2363">ACS</span></span>

* <span data-ttu-id="655ae-2364">Modification de toutes les mentions « agent » en « nœud » dans AKS</span><span class="sxs-lookup"><span data-stu-id="655ae-2364">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="655ae-2365">Option `--orchestrator-release` déconseillée pour `acs create`</span><span class="sxs-lookup"><span data-stu-id="655ae-2365">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="655ae-2366">Changement de la taille de machine virtuelle par défaut pour AKS à `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="655ae-2366">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="655ae-2367">Résolution de `az aks browse` sur Windows</span><span class="sxs-lookup"><span data-stu-id="655ae-2367">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="655ae-2368">Résolution de `az aks get-credentials` sur Windows</span><span class="sxs-lookup"><span data-stu-id="655ae-2368">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="655ae-2369">AppService</span><span class="sxs-lookup"><span data-stu-id="655ae-2369">Appservice</span></span>

* <span data-ttu-id="655ae-2370">Ajout de la source de déploiement `config-zip` pour les applications Web et de fonction</span><span class="sxs-lookup"><span data-stu-id="655ae-2370">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="655ae-2371">Ajout de l’option `--docker-container-logging` à `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="655ae-2371">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="655ae-2372">Suppression de l’option `storage` du paramètre `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="655ae-2372">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="655ae-2373">Amélioration des messages d’erreur pour `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="655ae-2373">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="655ae-2374">Ajout de la prise en charge pour la création d’applications de fonction Linux</span><span class="sxs-lookup"><span data-stu-id="655ae-2374">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="655ae-2375">`list-locations` fixe</span><span class="sxs-lookup"><span data-stu-id="655ae-2375">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="655ae-2376">Batch</span><span class="sxs-lookup"><span data-stu-id="655ae-2376">Batch</span></span>

* <span data-ttu-id="655ae-2377">Correction du bogue dans la commande de création de pool lorsqu’un ID ressource a été utilisé avec l’indicateur `--image`</span><span class="sxs-lookup"><span data-stu-id="655ae-2377">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="655ae-2378">Batchai</span><span class="sxs-lookup"><span data-stu-id="655ae-2378">Batchai</span></span>

* <span data-ttu-id="655ae-2379">Ajout de l’option courte, `-s`, pour `--vm-size` quand la taille de machine virtuelle est fournie dans la commande `file-server create`</span><span class="sxs-lookup"><span data-stu-id="655ae-2379">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="655ae-2380">Ajout du nom de compte de stockage et des arguments de clé dans les paramètres `cluster create`</span><span class="sxs-lookup"><span data-stu-id="655ae-2380">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="655ae-2381">Résolution de la documentation pour `job list-files` et `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="655ae-2381">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="655ae-2382">Ajout de l’option courte, `-r`, pour `--cluster-name` quand le nom du cluster est fourni dans la commande `job create`</span><span class="sxs-lookup"><span data-stu-id="655ae-2382">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="655ae-2383">Cloud</span><span class="sxs-lookup"><span data-stu-id="655ae-2383">Cloud</span></span>

* <span data-ttu-id="655ae-2384">Modification de `cloud [register|update]` pour empêcher l’inscription des clouds qui ne disposent pas de tous les points de terminaison requis</span><span class="sxs-lookup"><span data-stu-id="655ae-2384">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="655ae-2385">Conteneur</span><span class="sxs-lookup"><span data-stu-id="655ae-2385">Container</span></span>

* <span data-ttu-id="655ae-2386">Ajout de la prise en charge pour ouvrir plusieurs ports</span><span class="sxs-lookup"><span data-stu-id="655ae-2386">Added support to open multiple ports</span></span>
* <span data-ttu-id="655ae-2387">Ajout de la stratégie de redémarrage du groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="655ae-2387">Added container group restart policy</span></span>
* <span data-ttu-id="655ae-2388">Ajout de la prise en charge pour monter le partage de fichier Azure en tant que volume</span><span class="sxs-lookup"><span data-stu-id="655ae-2388">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="655ae-2389">Mise à jour des documents d’assistance</span><span class="sxs-lookup"><span data-stu-id="655ae-2389">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="655ae-2390">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="655ae-2390">Data Lake Analytics</span></span>

* <span data-ttu-id="655ae-2391">Modification de `[job|account] list` pour retourner des informations plus concises</span><span class="sxs-lookup"><span data-stu-id="655ae-2391">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="655ae-2392">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="655ae-2392">Data Lake Store</span></span>

* <span data-ttu-id="655ae-2393">Modification de `account list` pour retourner des informations plus concises</span><span class="sxs-lookup"><span data-stu-id="655ae-2393">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="655ae-2394">Extension</span><span class="sxs-lookup"><span data-stu-id="655ae-2394">Extension</span></span>

* <span data-ttu-id="655ae-2395">Ajout de `extension list-available` pour permettre l’affichage de la liste des extensions officielles Microsoft</span><span class="sxs-lookup"><span data-stu-id="655ae-2395">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="655ae-2396">Ajout de `--name` à `extension [add|update]` pour permettre l’installation des extensions par nom</span><span class="sxs-lookup"><span data-stu-id="655ae-2396">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="655ae-2397">IoT</span><span class="sxs-lookup"><span data-stu-id="655ae-2397">IoT</span></span>

* <span data-ttu-id="655ae-2398">Ajout de la prise en charge pour les autorités de certification (CA) et les chaînes d’approbation</span><span class="sxs-lookup"><span data-stu-id="655ae-2398">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="655ae-2399">Surveiller</span><span class="sxs-lookup"><span data-stu-id="655ae-2399">Monitor</span></span>

* <span data-ttu-id="655ae-2400">Ajout des commandes `activity-log alert`</span><span class="sxs-lookup"><span data-stu-id="655ae-2400">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="655ae-2401">Réseau</span><span class="sxs-lookup"><span data-stu-id="655ae-2401">Network</span></span>

* <span data-ttu-id="655ae-2402">Ajout de la prise en charge pour les enregistrements DNS CAA</span><span class="sxs-lookup"><span data-stu-id="655ae-2402">Added support for CAA DNS records</span></span>
* <span data-ttu-id="655ae-2403">Résolution d’un problème empêchant la mise à jour des points de terminaison avec `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="655ae-2403">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="655ae-2404">Résolution d’un problème où `vnet update --dns-servers` ne fonctionnait pas, en fonction de la façon dont avait été créé le réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="655ae-2404">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="655ae-2405">Résolution d’un problème où les noms DNS relatifs n’étaient pas importés correctement par `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="655ae-2405">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="655ae-2406">Réservations</span><span class="sxs-lookup"><span data-stu-id="655ae-2406">Reservations</span></span>

* <span data-ttu-id="655ae-2407">Version préliminaire initiale</span><span class="sxs-lookup"><span data-stu-id="655ae-2407">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="655ae-2408">Ressource</span><span class="sxs-lookup"><span data-stu-id="655ae-2408">Resource</span></span>

* <span data-ttu-id="655ae-2409">Ajout de la prise en charge pour les ID de ressource au paramètre `--resource` et pour les verrous au niveau des ressources</span><span class="sxs-lookup"><span data-stu-id="655ae-2409">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="655ae-2410">SQL</span><span class="sxs-lookup"><span data-stu-id="655ae-2410">SQL</span></span>

* <span data-ttu-id="655ae-2411">Ajout du paramètre `--ignore-missing-vnet-service-endpoint` pour `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="655ae-2411">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="655ae-2412">Stockage</span><span class="sxs-lookup"><span data-stu-id="655ae-2412">Storage</span></span>

* <span data-ttu-id="655ae-2413">Modification de `storage account create` pour utiliser la référence SKU `Standard_RAGRS` par défaut</span><span class="sxs-lookup"><span data-stu-id="655ae-2413">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="655ae-2414">Correction du bogue lors du traitement des noms d’objets blob/de fichier qui incluent des caractères non-ascii</span><span class="sxs-lookup"><span data-stu-id="655ae-2414">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="655ae-2415">Correction du bogue qui empêchait l’utilisation de `--source-uri` avec `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="655ae-2415">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="655ae-2416">Ajout de commandes pour paramétrer et supprimer plusieurs objets avec `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="655ae-2416">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="655ae-2417">Résolution du problème de l’activation des métriques avec `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="655ae-2417">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="655ae-2418">Résolution du problème des fichiers de plus de 200 Go lors de l’utilisation de `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="655ae-2418">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="655ae-2419">Résolution du problème où `--bypass` et `--default-action` étaient ignorés par `storage account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="655ae-2419">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="655ae-2420">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="655ae-2420">VM</span></span>

* <span data-ttu-id="655ae-2421">Correction d’un bogue avec `vmss create` qui empêchait l’utilisation du niveau de taille `Basic`</span><span class="sxs-lookup"><span data-stu-id="655ae-2421">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="655ae-2422">Ajout d’arguments `--plan` à `[vm|vmss] create` pour les images personnalisées avec des informations de facturation</span><span class="sxs-lookup"><span data-stu-id="655ae-2422">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="655ae-2423">Ajout des commandes `vm secret `[add|remove|list]</span><span class="sxs-lookup"><span data-stu-id="655ae-2423">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="655ae-2424">Renommage de `vm format-secret` en `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="655ae-2424">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="655ae-2425">Ajout de l’argument `--encrypt format` à `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="655ae-2425">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="655ae-2426">24 octobre 2017</span><span class="sxs-lookup"><span data-stu-id="655ae-2426">October 24, 2017</span></span>

<span data-ttu-id="655ae-2427">Version 2.0.20</span><span class="sxs-lookup"><span data-stu-id="655ae-2427">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="655ae-2428">Core</span><span class="sxs-lookup"><span data-stu-id="655ae-2428">Core</span></span>

* <span data-ttu-id="655ae-2429">Mise à jour de `2017-03-09-profile` pour consommer l’API `MGMT_STORAGE` version `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="655ae-2429">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="655ae-2430">ACR</span><span class="sxs-lookup"><span data-stu-id="655ae-2430">ACR</span></span>

* <span data-ttu-id="655ae-2431">Mise à jour de la gestion des ressources pour pointer vers la version d’API `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="655ae-2431">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="655ae-2432">Modification de la référence SKU « Bring Your Own Storage » en Classique</span><span class="sxs-lookup"><span data-stu-id="655ae-2432">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="655ae-2433">Changement des noms des références SKU de registre en De base, Standard, et Premium</span><span class="sxs-lookup"><span data-stu-id="655ae-2433">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="655ae-2434">ACS</span><span class="sxs-lookup"><span data-stu-id="655ae-2434">ACS</span></span>

* <span data-ttu-id="655ae-2435">[PRÉVERSION] Ajout des commandes `az aks`</span><span class="sxs-lookup"><span data-stu-id="655ae-2435">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="655ae-2436">Réparation de Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="655ae-2436">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="655ae-2437">AppService</span><span class="sxs-lookup"><span data-stu-id="655ae-2437">Appservice</span></span>

* <span data-ttu-id="655ae-2438">Résolution d’une erreur où le téléchargement des journaux d’activité `webapp` était incorrect</span><span class="sxs-lookup"><span data-stu-id="655ae-2438">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="655ae-2439">Composant</span><span class="sxs-lookup"><span data-stu-id="655ae-2439">Component</span></span>

* <span data-ttu-id="655ae-2440">Ajout de clarté dans les messages visant à déconseiller de tous les programmes d’installation et des invites de confirmation</span><span class="sxs-lookup"><span data-stu-id="655ae-2440">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="655ae-2441">Surveiller</span><span class="sxs-lookup"><span data-stu-id="655ae-2441">Monitor</span></span>

* <span data-ttu-id="655ae-2442">Ajout des commandes `action-group`</span><span class="sxs-lookup"><span data-stu-id="655ae-2442">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="655ae-2443">Ressource</span><span class="sxs-lookup"><span data-stu-id="655ae-2443">Resource</span></span>

* <span data-ttu-id="655ae-2444">Résolution d’une incompatibilité de la dépendance msrest dans `group export` avec les versions les plus récentes</span><span class="sxs-lookup"><span data-stu-id="655ae-2444">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="655ae-2445">Résolution de `policy assignment create` pour qu’il fonctionne avec les définitions de stratégie et les définitions d’ensemble de stratégie intégrées</span><span class="sxs-lookup"><span data-stu-id="655ae-2445">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="655ae-2446">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="655ae-2446">VM</span></span>

* <span data-ttu-id="655ae-2447">Ajout de l’argument `--accelerated-networking` à `vmss create`</span><span class="sxs-lookup"><span data-stu-id="655ae-2447">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="655ae-2448">9 octobre 2017</span><span class="sxs-lookup"><span data-stu-id="655ae-2448">October 9, 2017</span></span>

<span data-ttu-id="655ae-2449">Version 2.0.19</span><span class="sxs-lookup"><span data-stu-id="655ae-2449">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="655ae-2450">Core</span><span class="sxs-lookup"><span data-stu-id="655ae-2450">Core</span></span>

* <span data-ttu-id="655ae-2451">Ajout de la gestion des URL d’autorisation AD FS avec une barre oblique à Azure Stack</span><span class="sxs-lookup"><span data-stu-id="655ae-2451">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="655ae-2452">AppService</span><span class="sxs-lookup"><span data-stu-id="655ae-2452">Appservice</span></span>

* <span data-ttu-id="655ae-2453">Ajout de la mise à jour générique avec la nouvelle commande `webapp update`</span><span class="sxs-lookup"><span data-stu-id="655ae-2453">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="655ae-2454">Batch</span><span class="sxs-lookup"><span data-stu-id="655ae-2454">Batch</span></span>

* <span data-ttu-id="655ae-2455">Mis à jour du kit de développement logiciel (SDK) à la version 4.0.0</span><span class="sxs-lookup"><span data-stu-id="655ae-2455">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="655ae-2456">Mise à jour de l’option `--image` de VirtualMachineConfiguration pour prendre en charge les références d’image ARM en plus de publish:offre:sku:version</span><span class="sxs-lookup"><span data-stu-id="655ae-2456">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="655ae-2457">Ajout de la prise en charge du nouveau modèle d’extension CLI pour les commandes d’extension Batch</span><span class="sxs-lookup"><span data-stu-id="655ae-2457">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="655ae-2458">Suppression de la prise en charge Batch des modèles de composants</span><span class="sxs-lookup"><span data-stu-id="655ae-2458">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="655ae-2459">Batchai</span><span class="sxs-lookup"><span data-stu-id="655ae-2459">Batchai</span></span>

* <span data-ttu-id="655ae-2460">Version initiale du module Batch AI</span><span class="sxs-lookup"><span data-stu-id="655ae-2460">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="655ae-2461">KeyVault</span><span class="sxs-lookup"><span data-stu-id="655ae-2461">Keyvault</span></span>

* <span data-ttu-id="655ae-2462">Résolution du problème d’authentification Key Vault lors de l’utilisation d’AD FS sur Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="655ae-2462">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="655ae-2463">(#4448)</span><span class="sxs-lookup"><span data-stu-id="655ae-2463">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="655ae-2464">Réseau</span><span class="sxs-lookup"><span data-stu-id="655ae-2464">Network</span></span>

* <span data-ttu-id="655ae-2465">La modification de l’argument `--server` de `application-gateway address-pool create` devient facultative, permettant les pools d’adresses vides</span><span class="sxs-lookup"><span data-stu-id="655ae-2465">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="655ae-2466">Mise à jour de `traffic-manager` pour prendre en charge les fonctionnalités les plus récentes</span><span class="sxs-lookup"><span data-stu-id="655ae-2466">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="655ae-2467">Ressource</span><span class="sxs-lookup"><span data-stu-id="655ae-2467">Resource</span></span>

* <span data-ttu-id="655ae-2468">Ajout de la prise en charge des options `--resource-group/-g` pour le nom du groupe de ressources dans `group`</span><span class="sxs-lookup"><span data-stu-id="655ae-2468">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="655ae-2469">Ajout des commandes à `account lock` pour travailler avec des verrous au niveau de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="655ae-2469">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="655ae-2470">Ajout des commandes à `group lock` pour travailler avec des verrous au niveau du groupe</span><span class="sxs-lookup"><span data-stu-id="655ae-2470">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="655ae-2471">Ajout des commandes à `resource lock` pour travailler avec des verrous au niveau des ressources</span><span class="sxs-lookup"><span data-stu-id="655ae-2471">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="655ae-2472">SQL</span><span class="sxs-lookup"><span data-stu-id="655ae-2472">Sql</span></span>

* <span data-ttu-id="655ae-2473">Ajout de la prise en charge pour le Chiffrement transparent des données (TDE) SQL et le chiffrement transparent des données avec Bring Your Own Key</span><span class="sxs-lookup"><span data-stu-id="655ae-2473">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="655ae-2474">Ajout de la commande `db list-deleted` et du paramètre `db restore --deleted-time`, ce qui offre la possibilité de rechercher et de restaurer les bases de données supprimées</span><span class="sxs-lookup"><span data-stu-id="655ae-2474">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="655ae-2475">Ajout de `db op list` et `db op cancel`, ce qui offre la capacité de répertorier et d’annuler des opérations en cours sur la base de données</span><span class="sxs-lookup"><span data-stu-id="655ae-2475">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="655ae-2476">Stockage</span><span class="sxs-lookup"><span data-stu-id="655ae-2476">Storage</span></span>

* <span data-ttu-id="655ae-2477">Ajout de la prise en charge d’instantané de partage de fichiers</span><span class="sxs-lookup"><span data-stu-id="655ae-2477">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="655ae-2478">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="655ae-2478">Vm</span></span>

* <span data-ttu-id="655ae-2479">Correction d’un bogue dans `vm show` où l’utilisation de `-d` a provoqué un incident dans les adresses IP privées manquantes</span><span class="sxs-lookup"><span data-stu-id="655ae-2479">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="655ae-2480">[VERSION PRÉLIMINAIRE] Ajout de la prise en charge de la mise à niveau propagée pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="655ae-2480">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="655ae-2481">Ajout de la prise en charge de la mise à jour des paramètres de chiffrement avec `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="655ae-2481">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="655ae-2482">Ajout du paramètre `--os-disk-size-gb` pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="655ae-2482">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="655ae-2483">Ajout du paramètre `--license-type` de Windows pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="655ae-2483">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="655ae-2484">22 septembre 2017</span><span class="sxs-lookup"><span data-stu-id="655ae-2484">September 22, 2017</span></span>

<span data-ttu-id="655ae-2485">Version 2.0.18</span><span class="sxs-lookup"><span data-stu-id="655ae-2485">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="655ae-2486">Ressource</span><span class="sxs-lookup"><span data-stu-id="655ae-2486">Resource</span></span>

* <span data-ttu-id="655ae-2487">Ajout de la prise en charge de l’affichage des définitions de stratégie intégrée</span><span class="sxs-lookup"><span data-stu-id="655ae-2487">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="655ae-2488">Ajout de la prise en charge du paramètre de mode pour la création de définitions de stratégie</span><span class="sxs-lookup"><span data-stu-id="655ae-2488">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="655ae-2489">Ajout de la prise en charge des définitions d’interface utilisateur et des modèles pour `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="655ae-2489">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="655ae-2490">[CHANGEMENT CASSANT] Modification du type de ressource `managedapp` de `appliances` en `applications` et de `applianceDefinitions` en `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="655ae-2490">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="655ae-2491">Réseau</span><span class="sxs-lookup"><span data-stu-id="655ae-2491">Network</span></span>

* <span data-ttu-id="655ae-2492">Ajout de la prise en charge de la zone de disponibilité aux sous-commandes `network lb` et `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="655ae-2492">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="655ae-2493">Ajout de la prise en charge du peering Microsoft IPv6 pour `express-route`</span><span class="sxs-lookup"><span data-stu-id="655ae-2493">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="655ae-2494">Ajout des commandes du groupe de sécurité d’application `asg`</span><span class="sxs-lookup"><span data-stu-id="655ae-2494">Added `asg` application security group commands</span></span>
* <span data-ttu-id="655ae-2495">Ajout de l’argument `--application-security-groups` à `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="655ae-2495">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="655ae-2496">Ajout des arguments `--source-asgs` et `--destination-asgs` à `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="655ae-2496">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="655ae-2497">Ajout des arguments `--ddos-protection` et `--vm-protection` à `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="655ae-2497">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="655ae-2498">Ajout des commandes `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="655ae-2498">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="655ae-2499">Stockage</span><span class="sxs-lookup"><span data-stu-id="655ae-2499">Storage</span></span>

* <span data-ttu-id="655ae-2500">Résolution d’un problème qui pouvait causer l’échec des commandes `storage account network-rule` après la mise à jour du Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="655ae-2500">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="655ae-2501">Événement</span><span class="sxs-lookup"><span data-stu-id="655ae-2501">Eventgrid</span></span>

* <span data-ttu-id="655ae-2502">Mise à jour du Kit de développement logiciel (SDK) Python Azure Event Grid afin d’utiliser une version plus récente de l’API « 2017-09-15-preview »</span><span class="sxs-lookup"><span data-stu-id="655ae-2502">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="655ae-2503">SQL</span><span class="sxs-lookup"><span data-stu-id="655ae-2503">SQL</span></span>

* <span data-ttu-id="655ae-2504">La modification de l’`sql server list`argument`--resource-group` devient facultative.</span><span class="sxs-lookup"><span data-stu-id="655ae-2504">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="655ae-2505">En l’absence de précisions, tous les serveurs SQL dans l’abonnement seront retournés</span><span class="sxs-lookup"><span data-stu-id="655ae-2505">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="655ae-2506">Ajout du paramètre `--no-wait` à `db [create|copy|restore|update|replica create|create|update]` et `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="655ae-2506">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="655ae-2507">KeyVault</span><span class="sxs-lookup"><span data-stu-id="655ae-2507">Keyvault</span></span>

* <span data-ttu-id="655ae-2508">Ajout de la prise en charge des commandes Keyvault derrière un proxy</span><span class="sxs-lookup"><span data-stu-id="655ae-2508">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="655ae-2509">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="655ae-2509">VM</span></span>

* <span data-ttu-id="655ae-2510">Ajout de la prise en charge de zone de disponibilité pour `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="655ae-2510">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="655ae-2511">Résolution d’un problème à cause duquel l’utilisation de `--app-gateway ID` avec `vmss create` entraînait un échec</span><span class="sxs-lookup"><span data-stu-id="655ae-2511">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="655ae-2512">Ajout de l’argument `--asgs` à `vm create`</span><span class="sxs-lookup"><span data-stu-id="655ae-2512">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="655ae-2513">Ajout de la prise en charge des commandes en cours d’exécution sur des machines virtuelles avec `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="655ae-2513">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="655ae-2514">[PRÉVERSION] Ajout de la prise en charge du chiffrement de disque VMSS avec `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="655ae-2514">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="655ae-2515">Ajout de la prise en charge de la réalisation de la maintenance sur des machines virtuelles avec `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="655ae-2515">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="655ae-2516">ACS</span><span class="sxs-lookup"><span data-stu-id="655ae-2516">ACS</span></span>

* <span data-ttu-id="655ae-2517">[PRÉVERSION] Ajout de l’argument `--orchestrator-release` à `acs create` pour les régions ACS en préversion</span><span class="sxs-lookup"><span data-stu-id="655ae-2517">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="655ae-2518">AppService</span><span class="sxs-lookup"><span data-stu-id="655ae-2518">Appservice</span></span>

* <span data-ttu-id="655ae-2519">Ajout de la capacité à mettre à jour et à afficher les paramètres d’authentification avec `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="655ae-2519">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="655ae-2520">Sauvegarde</span><span class="sxs-lookup"><span data-stu-id="655ae-2520">Backup</span></span>

* <span data-ttu-id="655ae-2521">Préversion</span><span class="sxs-lookup"><span data-stu-id="655ae-2521">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="655ae-2522">11 septembre 2017</span><span class="sxs-lookup"><span data-stu-id="655ae-2522">September 11, 2017</span></span>

<span data-ttu-id="655ae-2523">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="655ae-2523">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="655ae-2524">Core</span><span class="sxs-lookup"><span data-stu-id="655ae-2524">Core</span></span>

* <span data-ttu-id="655ae-2525">Module de commande activé pour définir son propre ID de corrélation dans la télémétrie</span><span class="sxs-lookup"><span data-stu-id="655ae-2525">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="655ae-2526">Résolution du problème de vidage JSON lorsque la télémétrie est définie en mode diagnostics</span><span class="sxs-lookup"><span data-stu-id="655ae-2526">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="655ae-2527">Acs</span><span class="sxs-lookup"><span data-stu-id="655ae-2527">Acs</span></span>

* <span data-ttu-id="655ae-2528">Ajout de la commande `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="655ae-2528">Added `acs list-locations` command</span></span>
* <span data-ttu-id="655ae-2529">Faire en sorte que `ssh-key-file` soit fourni avec la valeur par défaut attendu</span><span class="sxs-lookup"><span data-stu-id="655ae-2529">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="655ae-2530">AppService</span><span class="sxs-lookup"><span data-stu-id="655ae-2530">Appservice</span></span>

* <span data-ttu-id="655ae-2531">Ajout de la possibilité de créer une application web dans un groupe de ressources autre que celui du plan de service actif</span><span class="sxs-lookup"><span data-stu-id="655ae-2531">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="655ae-2532">CDN</span><span class="sxs-lookup"><span data-stu-id="655ae-2532">CDN</span></span>

* <span data-ttu-id="655ae-2533">Correction du bogue « CustomDomain n’est pas itérable » pour `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="655ae-2533">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="655ae-2534">Extension</span><span class="sxs-lookup"><span data-stu-id="655ae-2534">Extension</span></span>

* <span data-ttu-id="655ae-2535">Version initiale</span><span class="sxs-lookup"><span data-stu-id="655ae-2535">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="655ae-2536">KeyVault</span><span class="sxs-lookup"><span data-stu-id="655ae-2536">Keyvault</span></span>

* <span data-ttu-id="655ae-2537">Résolution du problème où les autorisations étaient sensibles à la casse pour `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="655ae-2537">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="655ae-2538">Réseau</span><span class="sxs-lookup"><span data-stu-id="655ae-2538">Network</span></span>

* <span data-ttu-id="655ae-2539">Renommage de `vnet list-private-access-services` en `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="655ae-2539">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="655ae-2540">Argument `--private-access-services` renommé en `--service-endpoints` pour`vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="655ae-2540">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="655ae-2541">Ajout de la prise en charge de plusieurs plages IP et de ports à `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="655ae-2541">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="655ae-2542">Ajout de la prise en charge de la référence (SKU) pour `lb create`</span><span class="sxs-lookup"><span data-stu-id="655ae-2542">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="655ae-2543">Ajout de la prise en charge de la référence (SKU) pour `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="655ae-2543">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="655ae-2544">Ressource</span><span class="sxs-lookup"><span data-stu-id="655ae-2544">Resource</span></span>

* <span data-ttu-id="655ae-2545">Autoriser le passages dans les définitions de paramètres de stratégie de ressource dans `policy definition create`, et`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="655ae-2545">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="655ae-2546">Autoriser le passage dans les valeurs de paramètres pour `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="655ae-2546">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="655ae-2547">Autoriser le passage de JSON ou d’un fichier pour tous les paramètres</span><span class="sxs-lookup"><span data-stu-id="655ae-2547">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="655ae-2548">Incrémentation de la version de l’API</span><span class="sxs-lookup"><span data-stu-id="655ae-2548">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="655ae-2549">SQL</span><span class="sxs-lookup"><span data-stu-id="655ae-2549">SQL</span></span>

* <span data-ttu-id="655ae-2550">Ajout des commandes `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="655ae-2550">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="655ae-2551">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="655ae-2551">VM</span></span>

* <span data-ttu-id="655ae-2552">Problème résolu : n’affecte aucun accès tant que `--scope` n’est pas indiqué</span><span class="sxs-lookup"><span data-stu-id="655ae-2552">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="655ae-2553">Problème résolu : utilisation de la même dénomination d’extension que celle du portail</span><span class="sxs-lookup"><span data-stu-id="655ae-2553">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="655ae-2554">Suppression de `subscription` de la sortie `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="655ae-2554">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="655ae-2555">Résolu : la référence SKU de stockage `[vm|vmss] create` n’est pas appliquée sur les disques de données avec une image</span><span class="sxs-lookup"><span data-stu-id="655ae-2555">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="655ae-2556">Résolu : `vm format-secret --secrets` n’accepte pas d’ID séparés par un saut de ligne</span><span class="sxs-lookup"><span data-stu-id="655ae-2556">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="655ae-2557">31 août 2017</span><span class="sxs-lookup"><span data-stu-id="655ae-2557">August 31, 2017</span></span>

<span data-ttu-id="655ae-2558">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="655ae-2558">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="655ae-2559">KeyVault</span><span class="sxs-lookup"><span data-stu-id="655ae-2559">Keyvault</span></span>

* <span data-ttu-id="655ae-2560">Correction d’un bogue à cause duquel vous tentez de résoudre automatiquement l’encodage secret avec `secret download`</span><span class="sxs-lookup"><span data-stu-id="655ae-2560">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="655ae-2561">Sf</span><span class="sxs-lookup"><span data-stu-id="655ae-2561">Sf</span></span>

* <span data-ttu-id="655ae-2562">Déconseiller toutes les commandes en faveur de Service Fabric CLI (sfctl)</span><span class="sxs-lookup"><span data-stu-id="655ae-2562">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="655ae-2563">Stockage</span><span class="sxs-lookup"><span data-stu-id="655ae-2563">Storage</span></span>

* <span data-ttu-id="655ae-2564">Résolution du problème dans lequel la création de comptes de stockage dans les régions ne prenant pas en charge la fonctionnalité NetworkACLs était impossible</span><span class="sxs-lookup"><span data-stu-id="655ae-2564">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="655ae-2565">Déterminer le type de contenu et l’encodage du contenu lors du chargement d’objets blob et de fichiers si aucun type de contenu et d’encodage n’est spécifié.</span><span class="sxs-lookup"><span data-stu-id="655ae-2565">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="655ae-2566">28 août 2017</span><span class="sxs-lookup"><span data-stu-id="655ae-2566">August 28, 2017</span></span>

<span data-ttu-id="655ae-2567">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="655ae-2567">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="655ae-2568">Interface de ligne de commande</span><span class="sxs-lookup"><span data-stu-id="655ae-2568">CLI</span></span>

* <span data-ttu-id="655ae-2569">Ajout d’une remarque juridique pour `--version`</span><span class="sxs-lookup"><span data-stu-id="655ae-2569">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="655ae-2570">ACS</span><span class="sxs-lookup"><span data-stu-id="655ae-2570">ACS</span></span>

* <span data-ttu-id="655ae-2571">Correction des régions d’aperçu</span><span class="sxs-lookup"><span data-stu-id="655ae-2571">Corrected preview regions</span></span>
* <span data-ttu-id="655ae-2572">Mise en forme par défaut `dns_name_prefix` correctement</span><span class="sxs-lookup"><span data-stu-id="655ae-2572">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="655ae-2573">Optimisation de la sortie de commande des services ACS</span><span class="sxs-lookup"><span data-stu-id="655ae-2573">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="655ae-2574">AppService</span><span class="sxs-lookup"><span data-stu-id="655ae-2574">Appservice</span></span>

* <span data-ttu-id="655ae-2575">[CHANGEMENT CASSANT] Fixation des incohérences dans la sortie de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="655ae-2575">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="655ae-2576">Ajout d’un nouvel alias de `-i` pour `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="655ae-2576">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="655ae-2577">Exposé `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="655ae-2577">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="655ae-2578">Exposition de nouveaux arguments à partir de `az webapp delete` pour conserver le plan de service d'application, les métriques ou l’inscription DNS</span><span class="sxs-lookup"><span data-stu-id="655ae-2578">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="655ae-2579">Problème résolu : détecter les paramètres d’emplacement correctement</span><span class="sxs-lookup"><span data-stu-id="655ae-2579">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="655ae-2580">IoT</span><span class="sxs-lookup"><span data-stu-id="655ae-2580">IoT</span></span>

* <span data-ttu-id="655ae-2581">Résolution de #3934 : la création de la stratégie n’efface plus les stratégies existantes</span><span class="sxs-lookup"><span data-stu-id="655ae-2581">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="655ae-2582">Réseau</span><span class="sxs-lookup"><span data-stu-id="655ae-2582">Network</span></span>

* <span data-ttu-id="655ae-2583">[CHANGEMENT CASSANT] Renommage de `vnet list-private-access-services` en `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="655ae-2583">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="655ae-2584">[CHANGEMENT CASSANT] Renommage de l’option `--private-access-services` en `--service-endpoints` pour `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="655ae-2584">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="655ae-2585">Ajout de la prise en charge de plusieurs IP et de plusieurs pages de port pour `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="655ae-2585">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="655ae-2586">Ajout de la prise en charge de la référence (SKU) pour `lb create`</span><span class="sxs-lookup"><span data-stu-id="655ae-2586">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="655ae-2587">Ajout de la prise en charge de la référence (SKU) pour `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="655ae-2587">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="655ae-2588">Profil</span><span class="sxs-lookup"><span data-stu-id="655ae-2588">Profile</span></span>

* <span data-ttu-id="655ae-2589">exposés `--msi` et `--msi-port` pour vous connecter à l’aide d’une identité de machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="655ae-2589">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="655ae-2590">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="655ae-2590">Service Fabric</span></span>

* <span data-ttu-id="655ae-2591">Préversion</span><span class="sxs-lookup"><span data-stu-id="655ae-2591">Preview release</span></span>
* <span data-ttu-id="655ae-2592">Règles d’utilisateur du Registre/de mot de passe simplifiées pour la commande</span><span class="sxs-lookup"><span data-stu-id="655ae-2592">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="655ae-2593">Invite de mot de passe fixe pour l’utilisateur, même après le passage de paramètre</span><span class="sxs-lookup"><span data-stu-id="655ae-2593">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="655ae-2594">Ajout de la prise en charge de vide `registry_cred`</span><span class="sxs-lookup"><span data-stu-id="655ae-2594">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="655ae-2595">Stockage</span><span class="sxs-lookup"><span data-stu-id="655ae-2595">Storage</span></span>

* <span data-ttu-id="655ae-2596">Paramétrage du niveau blob activé</span><span class="sxs-lookup"><span data-stu-id="655ae-2596">Enabled setting blob tier</span></span>
* <span data-ttu-id="655ae-2597">Ajout des arguments `--bypass` et `--default-action` à `storage account [create|update]` pour la prise en charge du tunneling de service</span><span class="sxs-lookup"><span data-stu-id="655ae-2597">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="655ae-2598">Ajout de commandes permettant d’ajouter des règles de réseau virtuel et des règles basées sur IP à `storage account network-rule`</span><span class="sxs-lookup"><span data-stu-id="655ae-2598">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="655ae-2599">Activation du chiffrement du service par la clé gérée du client</span><span class="sxs-lookup"><span data-stu-id="655ae-2599">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="655ae-2600">[CHANGEMENT CASSANT] Renommage de l’option `--encryption` en `--encryption-services` pour la commande `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="655ae-2600">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="655ae-2601">Problème résolu #4220 : `az storage account update encryption` - incompatibilité de syntaxe</span><span class="sxs-lookup"><span data-stu-id="655ae-2601">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="655ae-2602">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="655ae-2602">VM</span></span>

* <span data-ttu-id="655ae-2603">Correction d’un problème qui entraînait l’affichage d’informations supplémentaires erronées pour `vmss get-instance-view` lors de l’utilisation `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="655ae-2603">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="655ae-2604">Ajout de la prise en charge de `--lb-sku` pour `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="655ae-2604">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="655ae-2605">Suppression des noms humains de la liste rouge du nom de l’administrateur pour `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="655ae-2605">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="655ae-2606">Correction d’un problème qui entraînait `[vm|vmss] create` la levée d’une erreur si la commande ne parvenait pas à extraire des informations de plan à partir d’une image</span><span class="sxs-lookup"><span data-stu-id="655ae-2606">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="655ae-2607">Correction d’un incident qui se produisait lors de la création d’un groupe identique VMMD avec un équilibrage de charge (LB) interne</span><span class="sxs-lookup"><span data-stu-id="655ae-2607">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="655ae-2608">Correction d’un problème qui empêchait `--no-wait` le fonctionnement d’un argument avec `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="655ae-2608">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="655ae-2609">15 août 2017</span><span class="sxs-lookup"><span data-stu-id="655ae-2609">August 15, 2017</span></span>

<span data-ttu-id="655ae-2610">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="655ae-2610">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="655ae-2611">ACS</span><span class="sxs-lookup"><span data-stu-id="655ae-2611">ACS</span></span>

* <span data-ttu-id="655ae-2612">Correction du numéro de port sshMaster0 pour kubernetes</span><span class="sxs-lookup"><span data-stu-id="655ae-2612">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="655ae-2613">AppService</span><span class="sxs-lookup"><span data-stu-id="655ae-2613">Appservice</span></span>

* <span data-ttu-id="655ae-2614">Correction d’une exception qui se produisait lors de la création d’une nouvelle application web Linux basée sur git</span><span class="sxs-lookup"><span data-stu-id="655ae-2614">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="655ae-2615">Event Grid</span><span class="sxs-lookup"><span data-stu-id="655ae-2615">Event Grid</span></span>

* <span data-ttu-id="655ae-2616">Ajout de dépendances du kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="655ae-2616">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="655ae-2617">11 août 2017</span><span class="sxs-lookup"><span data-stu-id="655ae-2617">August 11, 2017</span></span>

<span data-ttu-id="655ae-2618">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="655ae-2618">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="655ae-2619">ACS</span><span class="sxs-lookup"><span data-stu-id="655ae-2619">ACS</span></span>

* <span data-ttu-id="655ae-2620">Ajout de nouvelles régions d’aperçu</span><span class="sxs-lookup"><span data-stu-id="655ae-2620">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="655ae-2621">Batch</span><span class="sxs-lookup"><span data-stu-id="655ae-2621">Batch</span></span>

* <span data-ttu-id="655ae-2622">Mise à jour vers Kit de développement logiciel (DSK) de lot 3.1.0 et Kit de développement logiciel (SDK) de gestion de lot 4.1.0</span><span class="sxs-lookup"><span data-stu-id="655ae-2622">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="655ae-2623">Ajout d'une nouvelle commande affichant le nombre de tâches d’un travail</span><span class="sxs-lookup"><span data-stu-id="655ae-2623">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="655ae-2624">Correction du bogue dans le traitement de l’URL de la signature d'accès partagé du fichier de ressources</span><span class="sxs-lookup"><span data-stu-id="655ae-2624">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="655ae-2625">Point de terminaison de compte Batch prend désormais en charge le préfixe « https:// » facultatif</span><span class="sxs-lookup"><span data-stu-id="655ae-2625">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="655ae-2626">Prise en charge de l’ajout des listes de plus de 100 tâches à un travail</span><span class="sxs-lookup"><span data-stu-id="655ae-2626">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="655ae-2627">Ajout de l’enregistrement de débogage pour le chargement du module de commande Extensions</span><span class="sxs-lookup"><span data-stu-id="655ae-2627">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="655ae-2628">Composant</span><span class="sxs-lookup"><span data-stu-id="655ae-2628">Component</span></span>

* <span data-ttu-id="655ae-2629">Ajout d’un avertissement de désapprobation aux commandes « az component »</span><span class="sxs-lookup"><span data-stu-id="655ae-2629">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="655ae-2630">Conteneur</span><span class="sxs-lookup"><span data-stu-id="655ae-2630">Container</span></span>

* <span data-ttu-id="655ae-2631">`create`: correction d’un problème qui empêchait l’utilisation du signe égal à l’intérieur d’une variable d’environnement</span><span class="sxs-lookup"><span data-stu-id="655ae-2631">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="655ae-2632">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="655ae-2632">Data Lake Store</span></span>

* <span data-ttu-id="655ae-2633">Contrôle de progression activé</span><span class="sxs-lookup"><span data-stu-id="655ae-2633">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="655ae-2634">Event Grid</span><span class="sxs-lookup"><span data-stu-id="655ae-2634">Event Grid</span></span>

* <span data-ttu-id="655ae-2635">Version initiale</span><span class="sxs-lookup"><span data-stu-id="655ae-2635">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="655ae-2636">Réseau</span><span class="sxs-lookup"><span data-stu-id="655ae-2636">Network</span></span>

* <span data-ttu-id="655ae-2637">`lb`: correction d’un problème qui empêchait certains noms de ressources enfant d’être résolus correctement lorsqu’ils étaient omis</span><span class="sxs-lookup"><span data-stu-id="655ae-2637">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="655ae-2638">`application-gateway {subresource} delete`: correction d’un problème en raison duquel `--no-wait` n’était pas honorée</span><span class="sxs-lookup"><span data-stu-id="655ae-2638">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="655ae-2639">`application-gateway http-settings update`: correction d’un problème qui empêchait la désactivation de `--connection-draining-timeout`</span><span class="sxs-lookup"><span data-stu-id="655ae-2639">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="655ae-2640">Correction de erreur argument du mot-clé inattendu `sa_data_size_kilobyes` avec`az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="655ae-2640">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="655ae-2641">Profil</span><span class="sxs-lookup"><span data-stu-id="655ae-2641">Profile</span></span>

* <span data-ttu-id="655ae-2642">`account list`: ajout de `--refresh` pour synchroniser les derniers abonnements à partir du serveur</span><span class="sxs-lookup"><span data-stu-id="655ae-2642">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="655ae-2643">Stockage</span><span class="sxs-lookup"><span data-stu-id="655ae-2643">Storage</span></span>

* <span data-ttu-id="655ae-2644">Activer le compte de stockage de mise à jour avec l’identité attribuée par le système</span><span class="sxs-lookup"><span data-stu-id="655ae-2644">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="655ae-2645">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="655ae-2645">VM</span></span>

* <span data-ttu-id="655ae-2646">`availability-set`: nombre de domaines d’erreur exposés lors de la conversion</span><span class="sxs-lookup"><span data-stu-id="655ae-2646">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="655ae-2647">Commande `list-skus` exposée</span><span class="sxs-lookup"><span data-stu-id="655ae-2647">Exposed `list-skus` command</span></span>
* <span data-ttu-id="655ae-2648">Prise en charge pour affecter l’identité avec ou sans création d’attributions de rôle</span><span class="sxs-lookup"><span data-stu-id="655ae-2648">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="655ae-2649">Appliquer la référence (SKU) de stockage lors de l’attachement de disques de données</span><span class="sxs-lookup"><span data-stu-id="655ae-2649">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="655ae-2650">Suppression du nom du disque du système d’exploitation par défaut et de la référence (SKU) de stockage lors de l’utilisation des disques managés</span><span class="sxs-lookup"><span data-stu-id="655ae-2650">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="655ae-2651">28 juillet 2017</span><span class="sxs-lookup"><span data-stu-id="655ae-2651">July 28, 2017</span></span>

<span data-ttu-id="655ae-2652">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="655ae-2652">Version 2.0.12</span></span>

* <span data-ttu-id="655ae-2653">Ajout de commandes de conteneur</span><span class="sxs-lookup"><span data-stu-id="655ae-2653">Added container commands</span></span>
* <span data-ttu-id="655ae-2654">Ajout de modules de facturation et de consommation</span><span class="sxs-lookup"><span data-stu-id="655ae-2654">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="655ae-2655">Core</span><span class="sxs-lookup"><span data-stu-id="655ae-2655">Core</span></span>

* <span data-ttu-id="655ae-2656">Informations d’authentification du Kit de développement logiciel (SDK) de sortie pour les principaux de service avec des certificats</span><span class="sxs-lookup"><span data-stu-id="655ae-2656">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="655ae-2657">Correction des exceptions de progression de déploiement</span><span class="sxs-lookup"><span data-stu-id="655ae-2657">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="655ae-2658">Utiliser le point de terminaison ARM à partir du cloud actuel pour créer le client de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="655ae-2658">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="655ae-2659">Amélioration de la gestion simultanée de fichiers clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="655ae-2659">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="655ae-2660">Actualiser l’ID de la demande client pour chaque exécution de la commande</span><span class="sxs-lookup"><span data-stu-id="655ae-2660">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="655ae-2661">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel ( SDK) (#3635)</span><span class="sxs-lookup"><span data-stu-id="655ae-2661">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="655ae-2662">Rapports de progression pour les déploiements de modèle (#3510)</span><span class="sxs-lookup"><span data-stu-id="655ae-2662">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="655ae-2663">Ajout de la prise en charge des champs de sortie de la table de prélèvement via la requête jmespath (#3581)</span><span class="sxs-lookup"><span data-stu-id="655ae-2663">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="655ae-2664">Amélioration de la désactivation des arguments d’analyse et de l’historique Ajout avec des mouvements (#3434)</span><span class="sxs-lookup"><span data-stu-id="655ae-2664">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="655ae-2665">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="655ae-2665">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="655ae-2666">Déplacer tous les fichiers d’enregistrement existant vers le dernier dossier</span><span class="sxs-lookup"><span data-stu-id="655ae-2666">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="655ae-2667">Correction de l’idempotence pour VM/VMSS create (#3586)</span><span class="sxs-lookup"><span data-stu-id="655ae-2667">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="655ae-2668">Les chemins d’accès de la commande ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="655ae-2668">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="655ae-2669">Certains paramètres de type booléen ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="655ae-2669">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="655ae-2670">Prise en charge de la connexion à ADFS sur le serveur local de manière identique à Azure Stack</span><span class="sxs-lookup"><span data-stu-id="655ae-2670">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="655ae-2671">Correction des écritures simultanées dans clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="655ae-2671">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="655ae-2672">ACR</span><span class="sxs-lookup"><span data-stu-id="655ae-2672">ACR</span></span>

* <span data-ttu-id="655ae-2673">Ajout de la commande `show-usage` pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="655ae-2673">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="655ae-2674">Prise en charge de la mise à jour de la référence (SKU) pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="655ae-2674">Support SKU update for managed registries</span></span>
* <span data-ttu-id="655ae-2675">Ajout de registres gérés avec la référence (SKU) gérée</span><span class="sxs-lookup"><span data-stu-id="655ae-2675">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="655ae-2676">Ajout de webhooks pour les registres gérés avec le module de commande acr webhook</span><span class="sxs-lookup"><span data-stu-id="655ae-2676">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="655ae-2677">Ajout de l’authentification AAD avec la commande de connexion acr</span><span class="sxs-lookup"><span data-stu-id="655ae-2677">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="655ae-2678">Ajout de la commande de suppression pour les référentiels docker, les manifestes et les balises</span><span class="sxs-lookup"><span data-stu-id="655ae-2678">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="655ae-2679">ACS</span><span class="sxs-lookup"><span data-stu-id="655ae-2679">ACS</span></span>

* <span data-ttu-id="655ae-2680">Prise en charge des API version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="655ae-2680">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="655ae-2681">AppService</span><span class="sxs-lookup"><span data-stu-id="655ae-2681">Appservice</span></span>

* <span data-ttu-id="655ae-2682">Correction d’un bogue à cause duquel l’énumération d’une application Linux ne retournait absolument rien</span><span class="sxs-lookup"><span data-stu-id="655ae-2682">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="655ae-2683">Prise en charge de la récupération de références depuis ACR</span><span class="sxs-lookup"><span data-stu-id="655ae-2683">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="655ae-2684">Supprimer toutes les commandes sous `appservice web`</span><span class="sxs-lookup"><span data-stu-id="655ae-2684">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="655ae-2685">Masquer les mots de passe du registre docker de la commande de sortie (#3656)</span><span class="sxs-lookup"><span data-stu-id="655ae-2685">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="655ae-2686">Vérifier que le navigateur par défaut est utilisé sur macOs sans erreurs (#3623)</span><span class="sxs-lookup"><span data-stu-id="655ae-2686">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="655ae-2687">Améliorer l’aide de `webapp log tail` et `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="655ae-2687">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="655ae-2688">Commandes `traffic-routing` exposées pour configurer le routage statique (#3566)</span><span class="sxs-lookup"><span data-stu-id="655ae-2688">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="655ae-2689">Ajout de correctifs de fiabilité pour la configuration du contrôle de code source (#3245)</span><span class="sxs-lookup"><span data-stu-id="655ae-2689">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="655ae-2690">Suppression d’un argument non pris en charge `--node-version` de `webapp config update` pour les applications Web de Windows.</span><span class="sxs-lookup"><span data-stu-id="655ae-2690">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="655ae-2691">Utilisez à la place `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="655ae-2691">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="655ae-2692">Batch</span><span class="sxs-lookup"><span data-stu-id="655ae-2692">Batch</span></span>

* <span data-ttu-id="655ae-2693">Mise à jour vers kit de développement logiciel (SDK) de lot 3.0.0 avec prise en charge pour les machines virtuelles de faible priorité dans des pools</span><span class="sxs-lookup"><span data-stu-id="655ae-2693">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="655ae-2694">Renommage `pool create` option `--target-dedicated` en `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="655ae-2694">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="655ae-2695">Ajout des options `pool create`, `--target-low-priority-nodes` et `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="655ae-2695">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="655ae-2696">CDN</span><span class="sxs-lookup"><span data-stu-id="655ae-2696">CDN</span></span>

* <span data-ttu-id="655ae-2697">Fourniture d’un meilleur message d’erreur pour `cdn endpoint list` quand le profil spécifié par `--profile-name` n’existe pas</span><span class="sxs-lookup"><span data-stu-id="655ae-2697">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="655ae-2698">Cloud</span><span class="sxs-lookup"><span data-stu-id="655ae-2698">Cloud</span></span>

* <span data-ttu-id="655ae-2699">Modification de la version de l’API du point de terminaison de métadonnées du cloud au format AAAA-MM-JJ</span><span class="sxs-lookup"><span data-stu-id="655ae-2699">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="655ae-2700">Le point de terminaison de la galerie n’est pas nécessaire</span><span class="sxs-lookup"><span data-stu-id="655ae-2700">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="655ae-2701">Prise en charge de l’inscription du cloud, avec le point de terminaison ARM resource manager</span><span class="sxs-lookup"><span data-stu-id="655ae-2701">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="655ae-2702">Ajout d’une option pour `cloud set` permettant de choisir le profil lors de la sélection du cloud actuel</span><span class="sxs-lookup"><span data-stu-id="655ae-2702">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="655ae-2703">Exposé `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="655ae-2703">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="655ae-2704">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="655ae-2704">CosmosDB</span></span>

* <span data-ttu-id="655ae-2705">Correction relative à la permission de la création de collection avec une clé de partition personnalisée</span><span class="sxs-lookup"><span data-stu-id="655ae-2705">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="655ae-2706">Ajout de la prise en charge de la durée de vie par défaut de la collection</span><span class="sxs-lookup"><span data-stu-id="655ae-2706">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="655ae-2707">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="655ae-2707">Data Lake Analytics</span></span>

* <span data-ttu-id="655ae-2708">Ajout de commandes pour la gestion de la stratégie de calcul sous le titre `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="655ae-2708">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="655ae-2709">Ajout de `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="655ae-2709">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="655ae-2710">Ajout de `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="655ae-2710">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="655ae-2711">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="655ae-2711">Data Lake Store</span></span>

* <span data-ttu-id="655ae-2712">Ajout de la prise en charge pour la rotation de coffre de clés gérés par l’utilisateur dans `dls account update`</span><span class="sxs-lookup"><span data-stu-id="655ae-2712">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="655ae-2713">Mise à jour de la version du kit de développement logiciel (SDK) du système de fichiers Data Lake Store sous-jacente, réglant un problème de performance</span><span class="sxs-lookup"><span data-stu-id="655ae-2713">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="655ae-2714">Ajout de la commande `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="655ae-2714">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="655ae-2715">Cette commande tente d’activer un utilisateur de coffre de clés fourni par l’utilisateur pour utiliser le chiffrement des données dans un compte Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="655ae-2715">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="655ae-2716">Interactive</span><span class="sxs-lookup"><span data-stu-id="655ae-2716">Interactive</span></span>

* <span data-ttu-id="655ae-2717">Amélioration du temps de démarrage à l’aide des commandes en cache</span><span class="sxs-lookup"><span data-stu-id="655ae-2717">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="655ae-2718">Couverture de test accrue</span><span class="sxs-lookup"><span data-stu-id="655ae-2718">Increased test coverage</span></span>
* <span data-ttu-id="655ae-2719">Amélioration du mouvement « ? » pour injecter également dans la commande suivante</span><span class="sxs-lookup"><span data-stu-id="655ae-2719">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="655ae-2720">Correction d’erreurs interactives avec le profil 2017-03-09-profil-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="655ae-2720">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="655ae-2721">Autorisé `--version` en tant que paramètre pour le mode interactif (#3645)</span><span class="sxs-lookup"><span data-stu-id="655ae-2721">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="655ae-2722">Empêche le mode interactif de lever des erreurs à partir des listes de saisie semi-automatique de validation (#3570)</span><span class="sxs-lookup"><span data-stu-id="655ae-2722">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="655ae-2723">Rapports de progression pour les déploiements de modèles (#3510)</span><span class="sxs-lookup"><span data-stu-id="655ae-2723">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="655ae-2724">Ajout de l’indicateur `--progress`</span><span class="sxs-lookup"><span data-stu-id="655ae-2724">Added `--progress` flag</span></span>
* <span data-ttu-id="655ae-2725">Suppression `--debug` et `--verbose` des listes de saisie semi-automatique</span><span class="sxs-lookup"><span data-stu-id="655ae-2725">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="655ae-2726">Suppression `interactive` des listes de saisie semi-automatique (#3324)</span><span class="sxs-lookup"><span data-stu-id="655ae-2726">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="655ae-2727">IoT</span><span class="sxs-lookup"><span data-stu-id="655ae-2727">IoT</span></span>

* <span data-ttu-id="655ae-2728">La création de la stratégie n’efface plus les stratégies existantes.</span><span class="sxs-lookup"><span data-stu-id="655ae-2728">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="655ae-2729">(#3934)</span><span class="sxs-lookup"><span data-stu-id="655ae-2729">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="655ae-2730">Coffre de clés</span><span class="sxs-lookup"><span data-stu-id="655ae-2730">Key vault</span></span>

* <span data-ttu-id="655ae-2731">Ajout de commandes pour les fonctionnalités de récupération de coffre de clés :</span><span class="sxs-lookup"><span data-stu-id="655ae-2731">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="655ae-2732">`keyvault`sous-commandes `purge`, `recover`,`keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="655ae-2732">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="655ae-2733">`keyvault secret`sous-commandes `backup`, `restore`, `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="655ae-2733">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="655ae-2734">`keyvault certificate`sous-commandes `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="655ae-2734">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="655ae-2735">`keyvault key`sous-commandes `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="655ae-2735">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="655ae-2736">Ajout de l’intégration du coffre de clés du principal du service (#3133)</span><span class="sxs-lookup"><span data-stu-id="655ae-2736">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="655ae-2737">Mise à jour du plan de données du coffre de clés vers 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="655ae-2737">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="655ae-2738">(#3307)</span><span class="sxs-lookup"><span data-stu-id="655ae-2738">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="655ae-2739">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="655ae-2739">Lab</span></span>

* <span data-ttu-id="655ae-2740">Ajout de la prise en charge de la revendication de toutes les machines virtuelles dans le laboratoire via `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="655ae-2740">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="655ae-2741">Ajout du formateur de sortie de tableau pour `az lab vm list` et `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="655ae-2741">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="655ae-2742">Surveiller</span><span class="sxs-lookup"><span data-stu-id="655ae-2742">Monitor</span></span>

* <span data-ttu-id="655ae-2743">Correctif pour le fichier de modèle avec `monitor autoscale-settings get-parameters-template` commande (#3349)</span><span class="sxs-lookup"><span data-stu-id="655ae-2743">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="655ae-2744">Renommage de `monitor alert-rule-incidents list` en `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="655ae-2744">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="655ae-2745">Renommage de `monitor alert-rule-incidents show` en `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="655ae-2745">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="655ae-2746">Renommage de `monitor metric-defintions list` en `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="655ae-2746">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="655ae-2747">Renommage de `monitor alert-rules` en `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="655ae-2747">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="655ae-2748">Modifié `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="655ae-2748">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="655ae-2749">sous-commandes`condition` et `action` n’acceptent plus JSON</span><span class="sxs-lookup"><span data-stu-id="655ae-2749">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="655ae-2750">Ajout de nombreux paramètres simplifiant le processus de création de règle</span><span class="sxs-lookup"><span data-stu-id="655ae-2750">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="655ae-2751">`location` n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="655ae-2751">`location` no longer required</span></span>
  * <span data-ttu-id="655ae-2752">Ajout d’un nom et de la prise en charge de l’ID de la cible</span><span class="sxs-lookup"><span data-stu-id="655ae-2752">Add name and ID support for target</span></span>
  * <span data-ttu-id="655ae-2753">Suppression de `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="655ae-2753">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="655ae-2754">Le renommage de `is-enabled` en `enabled`n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="655ae-2754">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="655ae-2755">`description` par défaut sont désormais basées sur la condition fournie</span><span class="sxs-lookup"><span data-stu-id="655ae-2755">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="655ae-2756">Ajout d’exemples aidant à clarifier le nouveau format</span><span class="sxs-lookup"><span data-stu-id="655ae-2756">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="655ae-2757">Prise en charge des noms ou des ID pour les commandes `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="655ae-2757">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="655ae-2758">Ajout d’arguments d’usage et d’exemples pour `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="655ae-2758">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="655ae-2759">Réseau</span><span class="sxs-lookup"><span data-stu-id="655ae-2759">Network</span></span>

* <span data-ttu-id="655ae-2760">Ajout de la commande `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="655ae-2760">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="655ae-2761">Ajout de l’argument `--private-access-services` à `vnet subnet create` et `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="655ae-2761">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="655ae-2762">Correction d’un problème `application-gateway redirect-config create` qui causait l’échec de</span><span class="sxs-lookup"><span data-stu-id="655ae-2762">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="655ae-2763">Correction d’un problème `application-gateway redirect-config update` qui `--no-wait` empêchait le fonctionnement de</span><span class="sxs-lookup"><span data-stu-id="655ae-2763">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="655ae-2764">Correction d’un bogue lié à l’utilisation d’un `--servers` argument avec `application-gateway address-pool create` et `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="655ae-2764">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="655ae-2765">Ajout des commandes `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="655ae-2765">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="655ae-2766">Ajout de commandes à `application-gateway ssl-policy` : `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="655ae-2766">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="655ae-2767">Ajout d’arguments à `application-gateway ssl-policy set` : `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="655ae-2767">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="655ae-2768">Ajout d’arguments à `application-gateway http-settings create` et `application-gateway http-settings update` : `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="655ae-2768">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="655ae-2769">Ajout d’arguments à `application-gateway url-path-map create` et `application-gateway url-path-map update`, `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="655ae-2769">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="655ae-2770">Ajout d’un argument `--redirect-config` à `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="655ae-2770">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="655ae-2771">Ajout de la prise en charge de `--no-wait` pour `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="655ae-2771">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="655ae-2772">Ajout d’arguments à `application-gateway probe create` et `application-gateway probe update` : `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="655ae-2772">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="655ae-2773">Ajout d’un argument `--redirect-config` à `application-gateway rule create` et `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="655ae-2773">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="655ae-2774">Ajout de la prise en charge de `--accelerated-networking` pour `nic create` et `nic update`</span><span class="sxs-lookup"><span data-stu-id="655ae-2774">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="655ae-2775">Suppression de l’ `--internal-dns-name-suffix` argument à partir de `nic create`</span><span class="sxs-lookup"><span data-stu-id="655ae-2775">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="655ae-2776">Ajout de la prise en charge de `--dns-servers` pour `nic update` et `nic create` : ajout de la prise en charge de --dns-servers</span><span class="sxs-lookup"><span data-stu-id="655ae-2776">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="655ae-2777">Correction d’un bogue qui faisait `local-gateway create` ignorer `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="655ae-2777">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="655ae-2778">Ajout de la prise en charge de `--dns-servers` pour `vnet update`</span><span class="sxs-lookup"><span data-stu-id="655ae-2778">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="655ae-2779">Correction d’un bogue lors de la création d’un peering sans filtrage de l’itinéraire avec `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="655ae-2779">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="655ae-2780">Correction d’un bogue qui empêchait le fonctionnement des arguments `--provider` et `--bandwidth` avec `express-route update`</span><span class="sxs-lookup"><span data-stu-id="655ae-2780">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="655ae-2781">Correction d’un bogue avec `network watcher show-topology` une logique de valeurs par défaut</span><span class="sxs-lookup"><span data-stu-id="655ae-2781">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="655ae-2782">Amélioration de la mise en forme de sortie pour `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="655ae-2782">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="655ae-2783">Utilisation de l’IP frontale par défaut pour `application-gateway http-listener create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="655ae-2783">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="655ae-2784">Utilisation d’un pool d’adresses par défaut, des paramètres HTTP et de l’écouteur HTTP pour `application-gateway rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="655ae-2784">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="655ae-2785">Utilisation de l’IP frontale par défaut et du pool principal `lb rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="655ae-2785">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="655ae-2786">Utilisation de l’IP frontale par défaut pour `lb inbound-nat-rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="655ae-2786">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="655ae-2787">Profil</span><span class="sxs-lookup"><span data-stu-id="655ae-2787">Profile</span></span>

* <span data-ttu-id="655ae-2788">Prise en charge de la connexion à l’intérieur d’une machine virtuelle avec une identité gérée</span><span class="sxs-lookup"><span data-stu-id="655ae-2788">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="655ae-2789">Prise en charge de la sortie pour `account show` au format de fichier d’authentification du Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="655ae-2789">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="655ae-2790">Affichage des avertissements de désapprobation lors de l’utilisation de '--expanded-view'</span><span class="sxs-lookup"><span data-stu-id="655ae-2790">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="655ae-2791">Ajout de la commande `get-access-token` permettant de fournir un jeton AAD brut</span><span class="sxs-lookup"><span data-stu-id="655ae-2791">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="655ae-2792">Prise en charge de la connexion avec un compte d’utilisateur sans abonnements associés</span><span class="sxs-lookup"><span data-stu-id="655ae-2792">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="655ae-2793">SGBDR</span><span class="sxs-lookup"><span data-stu-id="655ae-2793">RDBMS</span></span>

* <span data-ttu-id="655ae-2794">Prise en charge de l’énumération de serveurs à travers un abonnement (#3417)</span><span class="sxs-lookup"><span data-stu-id="655ae-2794">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="655ae-2795">Correction de `%s` non traité car il manque `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="655ae-2795">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="655ae-2796">Correction du mappage de la source du document et ajout de la tâche CI permettant la vérification de (#3361)</span><span class="sxs-lookup"><span data-stu-id="655ae-2796">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="655ae-2797">Correction concernant l’aide relative à MySQL et PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="655ae-2797">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="655ae-2798">Ressource</span><span class="sxs-lookup"><span data-stu-id="655ae-2798">Resource</span></span>

* <span data-ttu-id="655ae-2799">Amélioration des invites pour les paramètres manquants de `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="655ae-2799">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="655ae-2800">Amélioration de l’analyse de `--parameters KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="655ae-2800">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="655ae-2801">Correction des problèmes à cause desquels `group deployment create` les fichiers de paramètres n’étaient plus reconnus à l’aide de la `@<file>` syntaxe</span><span class="sxs-lookup"><span data-stu-id="655ae-2801">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="655ae-2802">Prise en charge de l’ `--ids` argument pour `resource` et `managedapp` les commandes</span><span class="sxs-lookup"><span data-stu-id="655ae-2802">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="655ae-2803">Correction de certains messages d’analyse et d’erreur (#3584)</span><span class="sxs-lookup"><span data-stu-id="655ae-2803">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="655ae-2804">Correction de l’analyse `--resource-type` permettant à la `lock` commande d’accepter `<resource-namespace>` et `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="655ae-2804">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="655ae-2805">Ajout de la vérification de paramètre des modèles de liaison de modèle (#3629)</span><span class="sxs-lookup"><span data-stu-id="655ae-2805">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="655ae-2806">Ajout de la prise en charge de la spécification des paramètres de déploiement à l’aide de la `KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="655ae-2806">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="655ae-2807">Role</span><span class="sxs-lookup"><span data-stu-id="655ae-2807">Role</span></span>

* <span data-ttu-id="655ae-2808">Prise en charge de la sortie au format de fichier d’authentification du Kit de développement logiciel (SDK) pour `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="655ae-2808">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="655ae-2809">Nettoyage des attributions de rôles et de l’application AAD liée lors de la suppression d’un principal de service (#3610)</span><span class="sxs-lookup"><span data-stu-id="655ae-2809">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="655ae-2810">Inclusion du format d’heure dans `app create` args `--start-date` et `--end-date` descriptions</span><span class="sxs-lookup"><span data-stu-id="655ae-2810">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="655ae-2811">Affichage des avertissements de désapprobation lors de l’utilisation de `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="655ae-2811">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="655ae-2812">Ajout de l’intégration du coffre de clés pour les commandes `create-for-rbac` et `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="655ae-2812">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="655ae-2813">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="655ae-2813">Service Fabric</span></span>
* <span data-ttu-id="655ae-2814">Correction d’un problème avec les fichiers volumineux dans les applications tronquées sur le chargement (#3666)</span><span class="sxs-lookup"><span data-stu-id="655ae-2814">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="655ae-2815">Ajout de tests pour les commandes Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="655ae-2815">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="655ae-2816">Correction de nombreuses commandes Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="655ae-2816">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="655ae-2817">SQL</span><span class="sxs-lookup"><span data-stu-id="655ae-2817">SQL</span></span>

* <span data-ttu-id="655ae-2818">Suppression du paramètre rompu `sql server create` `--identity`</span><span class="sxs-lookup"><span data-stu-id="655ae-2818">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="655ae-2819">Suppression des valeurs de mot de passe à partir de la sortie de commande `sql server create` et `sql server update`</span><span class="sxs-lookup"><span data-stu-id="655ae-2819">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="655ae-2820">Ajout des commandes `sql db list-editions` et `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="655ae-2820">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="655ae-2821">Stockage</span><span class="sxs-lookup"><span data-stu-id="655ae-2821">Storage</span></span>

* <span data-ttu-id="655ae-2822">Suppression d’une `--marker` option à partir des commandes `storage blob list`, `storage container list`et `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="655ae-2822">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="655ae-2823">Activation de la création d’un compte de stockage https-only</span><span class="sxs-lookup"><span data-stu-id="655ae-2823">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="655ae-2824">Mise à jour des métriques de stockage, de la journalisation et des commandes cors (#3495)</span><span class="sxs-lookup"><span data-stu-id="655ae-2824">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="655ae-2825">Reformulation d’un message d’exception de l’ajout CORS (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="655ae-2825">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="655ae-2826">Conversion du générateur à une liste en mode exécution d’essai de la commande de téléchargement de lot (#3592)</span><span class="sxs-lookup"><span data-stu-id="655ae-2826">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="655ae-2827">Correction du problème d’essai associé au lot de téléchargement du blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="655ae-2827">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="655ae-2828">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="655ae-2828">VM</span></span>

* <span data-ttu-id="655ae-2829">Prise en charge de la configuration du groupe de sécurité réseau</span><span class="sxs-lookup"><span data-stu-id="655ae-2829">Support configuring nsg</span></span>
* <span data-ttu-id="655ae-2830">Correction d’un bogue qui entraînait une configuration incorrecte du serveur DNS</span><span class="sxs-lookup"><span data-stu-id="655ae-2830">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="655ae-2831">Prise en charge des identités de service géré</span><span class="sxs-lookup"><span data-stu-id="655ae-2831">Support managed service identities</span></span>
* <span data-ttu-id="655ae-2832">Correction d’un problème à cause duquel `cmss create` avec un équilibreur de charge existant exigeait `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="655ae-2832">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="655ae-2833">Les disques de données créés avec le numéro d’unité logique `vm image create` commencent à 0</span><span class="sxs-lookup"><span data-stu-id="655ae-2833">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="655ae-2834">10 mai 2017</span><span class="sxs-lookup"><span data-stu-id="655ae-2834">May 10, 2017</span></span>

<span data-ttu-id="655ae-2835">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="655ae-2835">Version 2.0.6</span></span>

* <span data-ttu-id="655ae-2836">documentdb renommé en cosmosdb</span><span class="sxs-lookup"><span data-stu-id="655ae-2836">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="655ae-2837">Ajouter rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="655ae-2837">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="655ae-2838">Inclure les modules Data Lake Analytics et Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="655ae-2838">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="655ae-2839">Inclure le module Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="655ae-2839">Include Cognitive Services module</span></span>
* <span data-ttu-id="655ae-2840">Inclure le module Service Fabric</span><span class="sxs-lookup"><span data-stu-id="655ae-2840">Include Service Fabric module</span></span>
* <span data-ttu-id="655ae-2841">Inclure le module Interactive (az-shell renommé)</span><span class="sxs-lookup"><span data-stu-id="655ae-2841">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="655ae-2842">Ajouter la prise en charge des commandes CDN</span><span class="sxs-lookup"><span data-stu-id="655ae-2842">Add support for CDN commands</span></span>
* <span data-ttu-id="655ae-2843">Supprimer le module Container</span><span class="sxs-lookup"><span data-stu-id="655ae-2843">Remove Container module</span></span>
* <span data-ttu-id="655ae-2844">Ajouter « az -v » comme raccourci pour « az --version » ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="655ae-2844">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="655ae-2845">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="655ae-2845">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="655ae-2846">Core</span><span class="sxs-lookup"><span data-stu-id="655ae-2846">Core</span></span>

* <span data-ttu-id="655ae-2847">principal : capturer les exceptions provoquées par un fournisseur non enregistré et l’enregistrer automatiquement</span><span class="sxs-lookup"><span data-stu-id="655ae-2847">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="655ae-2848">performance : conserver le cache de jeton adal en mémoire jusqu’à la fin du processus ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="655ae-2848">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="655ae-2849">Corriger les octets retournés par l’empreinte digitale hex -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="655ae-2849">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="655ae-2850">Téléchargement du certificat Key Vault et intégration AAD SP améliorés ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="655ae-2850">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="655ae-2851">Ajouter l’emplacement de Python à « az —version » ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="655ae-2851">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="655ae-2852">connexion : prise en charge de la connexion lorsqu’il n’y a aucun abonnement ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="655ae-2852">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="655ae-2853">principal : corriger une erreur lors de la connexion à l’aide d’un principal de service deux fois ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="655ae-2853">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="655ae-2854">principal : autoriser la configuration du chemin d’accès d’accessTokens.json via une variable d’environnement ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="655ae-2854">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="655ae-2855">principal : autoriser l’application des valeurs par défaut configurées sur les arguments facultatifs ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="655ae-2855">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="655ae-2856">principal : performances améliorées</span><span class="sxs-lookup"><span data-stu-id="655ae-2856">core: Improved performance</span></span>
* <span data-ttu-id="655ae-2857">principal : certificats d’autorité de certification personnalisés, prise en charge de la définition de la variable d’environnement REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="655ae-2857">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="655ae-2858">principal : configuration du cloud, utiliser le point de terminaison « resource manager » si le point de terminaison « management » n’est pas défini</span><span class="sxs-lookup"><span data-stu-id="655ae-2858">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="655ae-2859">ACS</span><span class="sxs-lookup"><span data-stu-id="655ae-2859">ACS</span></span>

* <span data-ttu-id="655ae-2860">corriger le nombre de maîtres et d’agents sur un nombre entier au lieu d’une chaîne</span><span class="sxs-lookup"><span data-stu-id="655ae-2860">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="655ae-2861">exposer « az acs create --no-wait » et « az acs wait » pour la création asynchrone</span><span class="sxs-lookup"><span data-stu-id="655ae-2861">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="655ae-2862">exposer « az acs create --validate » pour les validations de test</span><span class="sxs-lookup"><span data-stu-id="655ae-2862">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="655ae-2863">supprimer le profil Windows avant l’appel PUT pour la commande de mise à l’échelle ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="655ae-2863">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="655ae-2864">AppService</span><span class="sxs-lookup"><span data-stu-id="655ae-2864">AppService</span></span>

* <span data-ttu-id="655ae-2865">functionapp : ajouter la prise en charge complète de functionapp, notamment créer, afficher, liste, supprimer, nom d’hôte, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="655ae-2865">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="655ae-2866">Ajout de Team Services (vsts) comme option de livraison continue à « config contrôle source web appservice »</span><span class="sxs-lookup"><span data-stu-id="655ae-2866">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="655ae-2867">Créer « az webapp » pour remplacer « az appservice web » (pour la rétrocompatibilité, « az appservice web » sera conservé dans les 2 prochaines versions)</span><span class="sxs-lookup"><span data-stu-id="655ae-2867">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="655ae-2868">Exposer des arguments pour configurer le déploiement et des « piles d’exécution » sur webapp create</span><span class="sxs-lookup"><span data-stu-id="655ae-2868">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="655ae-2869">Exposer « webapp list-runtimes »</span><span class="sxs-lookup"><span data-stu-id="655ae-2869">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="655ae-2870">prendre en charge la configuration des chaînes de connexion ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="655ae-2870">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="655ae-2871">prendre en charge le basculement d’emplacement avec aperçu</span><span class="sxs-lookup"><span data-stu-id="655ae-2871">support slot swap with preview</span></span>
* <span data-ttu-id="655ae-2872">Supprimer les erreurs des commandes appservice ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="655ae-2872">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="655ae-2873">Utiliser le groupe de ressources du plan app service pour les opérations de certificat ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="655ae-2873">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="655ae-2874">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="655ae-2874">CosmosDB</span></span>

* <span data-ttu-id="655ae-2875">Renommer le module documentdb en cosmosdb</span><span class="sxs-lookup"><span data-stu-id="655ae-2875">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="655ae-2876">Prise en charge ajoutée pour les API de plan de données documentdb : gestion de base de données et de collecte</span><span class="sxs-lookup"><span data-stu-id="655ae-2876">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="655ae-2877">Prise en charge ajoutée pour activer le basculement automatique sur les comptes de base de données</span><span class="sxs-lookup"><span data-stu-id="655ae-2877">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="655ae-2878">Prise en charge ajoutée pour la nouvelle stratégie de cohérence ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="655ae-2878">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="655ae-2879">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="655ae-2879">Data Lake Analytics</span></span>

* <span data-ttu-id="655ae-2880">Corriger un bogue dans lequel le filtrage sur le résultat et l’état des listes de travaux lève une erreur</span><span class="sxs-lookup"><span data-stu-id="655ae-2880">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="655ae-2881">Ajouter la prise en charge d’un nouveau type d’élément de catalogue : paquet.</span><span class="sxs-lookup"><span data-stu-id="655ae-2881">Add support for new catalog item type: package.</span></span> <span data-ttu-id="655ae-2882">accessible via : `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="655ae-2882">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="655ae-2883">A rendu possible le fait de répertorier les éléments de catalogue suivants à partir d’une base de données (aucune spécification de schéma requise) :</span><span class="sxs-lookup"><span data-stu-id="655ae-2883">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="655ae-2884">Table</span><span class="sxs-lookup"><span data-stu-id="655ae-2884">Table</span></span>
  * <span data-ttu-id="655ae-2885">Fonction table</span><span class="sxs-lookup"><span data-stu-id="655ae-2885">Table valued function</span></span>
  * <span data-ttu-id="655ae-2886">Affichage</span><span class="sxs-lookup"><span data-stu-id="655ae-2886">View</span></span>
  * <span data-ttu-id="655ae-2887">Statistiques de table.</span><span class="sxs-lookup"><span data-stu-id="655ae-2887">Table Statistics.</span></span> <span data-ttu-id="655ae-2888">Cela peut également être répertorié avec un schéma, mais sans spécifier un nom de table</span><span class="sxs-lookup"><span data-stu-id="655ae-2888">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="655ae-2889">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="655ae-2889">Data Lake Store</span></span>

* <span data-ttu-id="655ae-2890">Mettre à jour la version du Kit de développement logiciel (SDK) du système de fichiers sous-jacent, qui offre une meilleure prise en charge pour gérer les scénarios de limitation côté serveur</span><span class="sxs-lookup"><span data-stu-id="655ae-2890">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="655ae-2891">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="655ae-2891">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="655ae-2892">aide manquante pour afficher l’accès.</span><span class="sxs-lookup"><span data-stu-id="655ae-2892">missed help for access show.</span></span> <span data-ttu-id="655ae-2893">ajout en cours.</span><span class="sxs-lookup"><span data-stu-id="655ae-2893">adding it.</span></span> <span data-ttu-id="655ae-2894">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="655ae-2894">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="655ae-2895">Rechercher</span><span class="sxs-lookup"><span data-stu-id="655ae-2895">Find</span></span>

* <span data-ttu-id="655ae-2896">résultats de la recherche améliorés et autorisation du contrôle de version de l’index de recherche</span><span class="sxs-lookup"><span data-stu-id="655ae-2896">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="655ae-2897">KeyVault</span><span class="sxs-lookup"><span data-stu-id="655ae-2897">KeyVault</span></span>

* <span data-ttu-id="655ae-2898">BC : `az keyvault certificate download` remplacer -e dans chaîne ou élément binaire par PEM ou DER afin de mieux représenter les options</span><span class="sxs-lookup"><span data-stu-id="655ae-2898">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="655ae-2899">BC : supprimer --expires et --not-before dans `keyvault certificate create`, car ces paramètres ne sont pas pris en charge par le service</span><span class="sxs-lookup"><span data-stu-id="655ae-2899">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="655ae-2900">Ajoute le paramètre --validity à `keyvault certificate create` pour substituer de manière sélective la valeur dans --policy</span><span class="sxs-lookup"><span data-stu-id="655ae-2900">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="655ae-2901">Résout le problème dans `keyvault certificate get-default-policy` où « expires » et « not_before » étaient exposés mais « validity_in_months » ne l’était pas</span><span class="sxs-lookup"><span data-stu-id="655ae-2901">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="655ae-2902">correction de keyvault pour l’importation de pem et pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="655ae-2902">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="655ae-2903">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="655ae-2903">Lab</span></span>

* <span data-ttu-id="655ae-2904">Ajout des commandes créer, afficher, supprimer et liste pour l’environnement dans le laboratoire</span><span class="sxs-lookup"><span data-stu-id="655ae-2904">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="655ae-2905">Ajout des commandes afficher et liste pour afficher les modèles ARM dans le laboratoire</span><span class="sxs-lookup"><span data-stu-id="655ae-2905">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="655ae-2906">Ajout de l’indicateur --environment dans `az lab vm list` pour filtrer les machines virtuelles selon l’environnement du laboratoire</span><span class="sxs-lookup"><span data-stu-id="655ae-2906">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="655ae-2907">Ajout de la commande pratique `az lab formula export-artifacts` pour exporter une structure d’artefact dans une formule de laboratoire</span><span class="sxs-lookup"><span data-stu-id="655ae-2907">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="655ae-2908">Ajout de commandes pour gérer les secrets dans un laboratoire</span><span class="sxs-lookup"><span data-stu-id="655ae-2908">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="655ae-2909">Surveiller</span><span class="sxs-lookup"><span data-stu-id="655ae-2909">Monitor</span></span>

* <span data-ttu-id="655ae-2910">Résolution de bogue : modélisation de `--actions` de `az alert-rules create` pour consommer la chaîne JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="655ae-2910">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="655ae-2911">Correction de bogue : la création de paramètres de diagnostic n’accepte pas les métriques/journaux à partir des commandes d’affichage ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="655ae-2911">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="655ae-2912">Réseau</span><span class="sxs-lookup"><span data-stu-id="655ae-2912">Network</span></span>

* <span data-ttu-id="655ae-2913">Ajouter la commande `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="655ae-2913">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="655ae-2914">Ajouter la prise en charge du paramètre `--filters` pour `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="655ae-2914">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="655ae-2915">Ajouter la prise en charge pour le drainage de connexion Application Gateway</span><span class="sxs-lookup"><span data-stu-id="655ae-2915">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="655ae-2916">Ajouter la prise en charge pour la configuration du jeu de règles WAF d’Application Gateway</span><span class="sxs-lookup"><span data-stu-id="655ae-2916">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="655ae-2917">Ajouter la prise en charge des règles et des filtres de routage ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="655ae-2917">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="655ae-2918">Ajouter la prise en charge pour le routage géographique TrafficManager</span><span class="sxs-lookup"><span data-stu-id="655ae-2918">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="655ae-2919">Ajouter la prise en charge des sélecteurs de trafic basés sur la stratégie de connexion VPN</span><span class="sxs-lookup"><span data-stu-id="655ae-2919">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="655ae-2920">Ajouter la prise en charge pour les stratégies IPSec de la connexion VPN</span><span class="sxs-lookup"><span data-stu-id="655ae-2920">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="655ae-2921">Corriger le bogue avec `vpn-connection create` lors de l’utilisation des paramètres `--no-wait` ou `--validate`</span><span class="sxs-lookup"><span data-stu-id="655ae-2921">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="655ae-2922">Ajouter la prise en charge des passerelles de réseau virtuel actif-actif</span><span class="sxs-lookup"><span data-stu-id="655ae-2922">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="655ae-2923">Supprimer les valeurs NULL de la sortie des commandes `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="655ae-2923">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="655ae-2924">BC : résoudre un bogue dans la sortie de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="655ae-2924">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="655ae-2925">Corriger le bogue où l’argument « --key-length » de « vpn-connection create » n’était pas analysé correctement</span><span class="sxs-lookup"><span data-stu-id="655ae-2925">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="655ae-2926">Corriger le bogue dans `dns zone import` où les enregistrements n’étaient pas été importés correctement</span><span class="sxs-lookup"><span data-stu-id="655ae-2926">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="655ae-2927">Corriger le bogue où `traffic-manager endpoint update` ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="655ae-2927">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="655ae-2928">Ajouter des commandes d’aperçu « network watcher »</span><span class="sxs-lookup"><span data-stu-id="655ae-2928">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="655ae-2929">Profil</span><span class="sxs-lookup"><span data-stu-id="655ae-2929">Profile</span></span>

* <span data-ttu-id="655ae-2930">Prendre en charge la connexion lorsqu’il n’y a aucun abonnement trouvé ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="655ae-2930">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="655ae-2931">Prendre en charge un nom de paramètre court dans le jeu de comptes az --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="655ae-2931">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="655ae-2932">Redis</span><span class="sxs-lookup"><span data-stu-id="655ae-2932">Redis</span></span>

* <span data-ttu-id="655ae-2933">Ajout d’une commande de mise à jour qui ajoute également la possibilité de mettre à l’échelle pour le cache redis</span><span class="sxs-lookup"><span data-stu-id="655ae-2933">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="655ae-2934">Commande « update-settings » déconseillée</span><span class="sxs-lookup"><span data-stu-id="655ae-2934">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="655ae-2935">Ressource</span><span class="sxs-lookup"><span data-stu-id="655ae-2935">Resource</span></span>

* <span data-ttu-id="655ae-2936">Ajouter managedapp et les commandes de définition managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="655ae-2936">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="655ae-2937">Prendre en charge les commandes « provider operation » ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="655ae-2937">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="655ae-2938">Prendre en charge la création de ressource générique ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="655ae-2938">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="655ae-2939">Corriger l’analyse de ressource et la recherche de version d’API.</span><span class="sxs-lookup"><span data-stu-id="655ae-2939">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="655ae-2940">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="655ae-2940">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="655ae-2941">Ajouter des documents pour mise à jour du verrou az.</span><span class="sxs-lookup"><span data-stu-id="655ae-2941">Add docs for az lock update.</span></span> <span data-ttu-id="655ae-2942">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="655ae-2942">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="655ae-2943">Sortie d’erreur si vous essayez de lister des ressources pour un groupe qui n’existe pas.</span><span class="sxs-lookup"><span data-stu-id="655ae-2943">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="655ae-2944">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="655ae-2944">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="655ae-2945">[Compute] Résoudre les problèmes de mise à jour de VMSS et du groupe à haute disponibilité de machines virtuelles.</span><span class="sxs-lookup"><span data-stu-id="655ae-2945">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="655ae-2946">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="655ae-2946">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="655ae-2947">Corriger le verrouillage des commandes créer et supprimer si parent-resource-path est None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="655ae-2947">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="655ae-2948">Role</span><span class="sxs-lookup"><span data-stu-id="655ae-2948">Role</span></span>

* <span data-ttu-id="655ae-2949">create-for-rbac : vérifier que la date de fin du SP ne dépassera pas la date d’expiration du certificat ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="655ae-2949">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="655ae-2950">RBAC : ajouter la prise en charge complète de « ad group » ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="655ae-2950">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="655ae-2951">rôle : résoudre les problèmes de mise à jour de définition de rôle ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="655ae-2951">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="655ae-2952">create-for-rbac : vérifier que le mot de passe fourni par l’utilisateur est accepté</span><span class="sxs-lookup"><span data-stu-id="655ae-2952">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="655ae-2953">SQL</span><span class="sxs-lookup"><span data-stu-id="655ae-2953">SQL</span></span>

* <span data-ttu-id="655ae-2954">Ajout des commandes az sql server list-usages et az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="655ae-2954">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="655ae-2955">SQL : possibilité de se connecter directement au fournisseur de ressources ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="655ae-2955">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="655ae-2956">Stockage</span><span class="sxs-lookup"><span data-stu-id="655ae-2956">Storage</span></span>

* <span data-ttu-id="655ae-2957">Définir l’emplacement par défaut sur l’emplacement du groupe de ressources pour `storage account create`</span><span class="sxs-lookup"><span data-stu-id="655ae-2957">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="655ae-2958">Ajouter la prise en charge de la copie incrémentielle d’objet blob</span><span class="sxs-lookup"><span data-stu-id="655ae-2958">Add support for incremental blob copy</span></span>
* <span data-ttu-id="655ae-2959">Ajouter la prise en charge du chargement d’objet blob de blocs volumineux</span><span class="sxs-lookup"><span data-stu-id="655ae-2959">Add support for large block blob upload</span></span>
* <span data-ttu-id="655ae-2960">Modifier la taille de bloc à 100 Mo lorsque le fichier à charger est supérieur à 200 Go</span><span class="sxs-lookup"><span data-stu-id="655ae-2960">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="655ae-2961">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="655ae-2961">VM</span></span>

* <span data-ttu-id="655ae-2962">avail-set : rendre le compte de domaine UD&FD facultatif</span><span class="sxs-lookup"><span data-stu-id="655ae-2962">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="655ae-2963">Remarque : commandes de machine virtuelle dans clouds souverains. Veuillez éviter les fonctionnalités liées au disque managé, notamment :</span><span class="sxs-lookup"><span data-stu-id="655ae-2963">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="655ae-2964">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="655ae-2964">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="655ae-2965">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="655ae-2965">az vm/vmss disk</span></span>
  3. <span data-ttu-id="655ae-2966">Dans « az vm/vmss create », utiliser « —use-unmanaged-disk » pour éviter le disque managé Les autres commandes devraient fonctionner</span><span class="sxs-lookup"><span data-stu-id="655ae-2966">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="655ae-2967">vm/vmss : améliorer le texte d’avertissement lors de la génération de paires de clés ssh</span><span class="sxs-lookup"><span data-stu-id="655ae-2967">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="655ae-2968">vm/vmss : prendre en charge la création à partir d’une image de la Place de marché qui requiert des informations sur le plan ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="655ae-2968">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="655ae-2969">3 avril 2017</span><span class="sxs-lookup"><span data-stu-id="655ae-2969">April 3, 2017</span></span>

<span data-ttu-id="655ae-2970">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="655ae-2970">Version 2.0.2</span></span>

<span data-ttu-id="655ae-2971">Nous avons publié les composants ACR, Batch, KeyVault et SQL dans cette version</span><span class="sxs-lookup"><span data-stu-id="655ae-2971">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="655ae-2972">Core</span><span class="sxs-lookup"><span data-stu-id="655ae-2972">Core</span></span>

* <span data-ttu-id="655ae-2973">Ajout des modules acr, lab, monitor et find à la liste par défaut</span><span class="sxs-lookup"><span data-stu-id="655ae-2973">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="655ae-2974">Connexion : ignorer les locataires erronés ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="655ae-2974">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="655ae-2975">login : définition de l’abonnement par défaut à la valeur « un » avec l’état « Activé » ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="655ae-2975">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="655ae-2976">Ajout de la prise en charge des commandes wait et de --no-wait à davantage de commandes ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="655ae-2976">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="655ae-2977">core : prise en charge de la connexion à l’aide du principal du service avec un certificat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="655ae-2977">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="655ae-2978">Ajout d’une invite pour les paramètres de modèle manquants.</span><span class="sxs-lookup"><span data-stu-id="655ae-2978">Add prompting for missing template parameters.</span></span> <span data-ttu-id="655ae-2979">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="655ae-2979">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="655ae-2980">Prise en charge de la définition de valeurs par défaut pour des arguments courants tels que le groupe de ressources par défaut, le site web par défaut et la machine virtuelle par défaut</span><span class="sxs-lookup"><span data-stu-id="655ae-2980">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="655ae-2981">Prise en charge de la connexion à un locataire spécifique</span><span class="sxs-lookup"><span data-stu-id="655ae-2981">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="655ae-2982">ACS</span><span class="sxs-lookup"><span data-stu-id="655ae-2982">ACS</span></span>

* <span data-ttu-id="655ae-2983">[ACS] Ajout de la prise en charge de la configuration d’un cluster ACS par défaut ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="655ae-2983">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="655ae-2984">Ajout de la prise en charge de l’invite de mot de passe de clé ssh.</span><span class="sxs-lookup"><span data-stu-id="655ae-2984">Add support for ssh key password prompting.</span></span> <span data-ttu-id="655ae-2985">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="655ae-2985">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="655ae-2986">Ajout de la prise en charge des clusters Windows.</span><span class="sxs-lookup"><span data-stu-id="655ae-2986">Add support for windows clusters.</span></span> <span data-ttu-id="655ae-2987">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="655ae-2987">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="655ae-2988">Basculement du rôle Propriétaire au rôle Contributeur.</span><span class="sxs-lookup"><span data-stu-id="655ae-2988">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="655ae-2989">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="655ae-2989">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="655ae-2990">AppService</span><span class="sxs-lookup"><span data-stu-id="655ae-2990">AppService</span></span>

* <span data-ttu-id="655ae-2991">appservice : prise en charge de l’obtention de l’adresse IP externe utilisée pour les enregistrements A DNS ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="655ae-2991">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="655ae-2992">appservice : prise en charge de la liaison des certificats avec caractères génériques ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="655ae-2992">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="655ae-2993">appservice : prise en charge des profils de publication de liste ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="655ae-2993">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="655ae-2994">AppService : déclenchement de la synchronisation de contrôle de code source après la configuration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="655ae-2994">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="655ae-2995">DataLake</span><span class="sxs-lookup"><span data-stu-id="655ae-2995">DataLake</span></span>

* <span data-ttu-id="655ae-2996">Version initiale du module Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="655ae-2996">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="655ae-2997">Version initiale du module Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="655ae-2997">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="655ae-2998">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="655ae-2998">DocuemntDB</span></span>

* <span data-ttu-id="655ae-2999">DocumentDB : ajout de la prise en charge de l’énumération des chaînes de connexion ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="655ae-2999">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="655ae-3000">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="655ae-3000">VM</span></span>

* <span data-ttu-id="655ae-3001">[Compute] Ajout de la prise en charge d’AppGateway à la création de groupe de machines virtuelles identiques ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="655ae-3001">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="655ae-3002">[VM/VMSS] Amélioration de la prise en charge de la mise en cache de disque ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="655ae-3002">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="655ae-3003">VM/VMSS : intégration de la logique de validation des informations d’identification utilisée par le portail ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="655ae-3003">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="655ae-3004">Ajout de la prise en charge des commandes wait et de --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="655ae-3004">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="655ae-3005">Groupe de machines virtuelles identiques : prise en charge de \* pour énumérer les vues d’instance parmi les machines virtuelles ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="655ae-3005">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="655ae-3006">Ajout --secrets pour machine virtuelle et groupe de machines virtuelles identiques ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="655ae-3006">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="655ae-3007">Autorisation de la création de machines virtuelles avec un disque dur virtuel spécialisé ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="655ae-3007">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="655ae-3008">27 février 2017</span><span class="sxs-lookup"><span data-stu-id="655ae-3008">February 27, 2017</span></span>

<span data-ttu-id="655ae-3009">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="655ae-3009">Version 2.0.0</span></span>

<span data-ttu-id="655ae-3010">Cette version d’Azure CLI 2.0 est la première instance mise à la disposition générale. La disponibilité générale s’applique à ces modules de commande :</span><span class="sxs-lookup"><span data-stu-id="655ae-3010">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="655ae-3011">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="655ae-3011">Container Service (acs)</span></span>
- <span data-ttu-id="655ae-3012">Compute (notamment Resource Manager, machine virtuelle, groupes de machines virtuelles identiques, Disques managés)</span><span class="sxs-lookup"><span data-stu-id="655ae-3012">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="655ae-3013">Réseau</span><span class="sxs-lookup"><span data-stu-id="655ae-3013">Networking</span></span>
- <span data-ttu-id="655ae-3014">Stockage</span><span class="sxs-lookup"><span data-stu-id="655ae-3014">Storage</span></span>

<span data-ttu-id="655ae-3015">Ces modules de commande, pouvant être utilisés en production, sont pris en charge par le contrat de niveau de service (SLA) Microsoft standard. Vous pouvez ouvrir des incidents directement auprès du support technique Microsoft ou dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/). Vous pouvez poser des questions sur [StackOverflow à l’aide du mot-clé azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), ou contacter l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Vous pouvez fournir des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="655ae-3015">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="655ae-3016">Les commandes de ces modules sont stables et il n’est pas prévu que la syntaxe change dans les mises à jour ultérieures de cette version d’Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="655ae-3016">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="655ae-3017">Pour vérifier la version de l’interface CLI, utilisez `az --version`. La sortie indique la version de l’interface CLI proprement dite (2.0.0 dans cette version), les différents modules de commande et les versions de Python et de GCC que vous utilisez.</span><span class="sxs-lookup"><span data-stu-id="655ae-3017">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="655ae-3018">Certains de ces modules de commande présentent un suffixe « b*n* » ou « rc*n* ». Ces modules de commande, encore en préversion, seront mis à la disposition générale à l’avenir.</span><span class="sxs-lookup"><span data-stu-id="655ae-3018">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="655ae-3019">Nous avons également des versions d’évaluation nocturnes de l’interface CLI. Pour plus d’informations, consultez ces instructions sur l’[obtention des builds nocturnes](https://github.com/Azure/azure-cli#nightly-builds), ainsi que ces instructions sur [la contribution au code et la configuration d’un environnement de développement](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="655ae-3019">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="655ae-3020">Vous pouvez signaler des problèmes liés aux versions d’évaluation nocturnes comme suit :</span><span class="sxs-lookup"><span data-stu-id="655ae-3020">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="655ae-3021">Signalez des problèmes dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="655ae-3021">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="655ae-3022">Contactez l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="655ae-3022">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="655ae-3023">Fournissez des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="655ae-3023">Provide feedback from the command line with the `az feedback` command</span></span>

