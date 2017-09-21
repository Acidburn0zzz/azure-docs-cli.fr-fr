---
title: "Notes de publication d’Azure CLI 2.0"
description: "En savoir plus sur les dernières mises à jour d’Azure CLI 2.0"
keywords: Azure CLI 2.0, notes de publication
author: sptramer
ms.author: sttramer
manager: douge
ms.date: 04/03/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: ce0428f7-0a59-4e72-9237-d907b171af51
ms.openlocfilehash: 39e4710a29ac57730919b82ab76b9c9a4b9ca786
ms.sourcegitcommit: 43d4f838d132ab9bcfa59dbda3b544c06373b6a9
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/22/2017
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="439f1-104">Notes de publication d’Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="439f1-104">Azure CLI 2.0 release notes</span></span>

## <a name="august-15-2017"></a><span data-ttu-id="439f1-105">15 août 2017</span><span class="sxs-lookup"><span data-stu-id="439f1-105">August 15, 2017</span></span>

<span data-ttu-id="439f1-106">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="439f1-106">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="439f1-107">ACS</span><span class="sxs-lookup"><span data-stu-id="439f1-107">ACS</span></span>

* <span data-ttu-id="439f1-108">Correction du numéro de port sshMaster0 pour kubernetes</span><span class="sxs-lookup"><span data-stu-id="439f1-108">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="439f1-109">AppService</span><span class="sxs-lookup"><span data-stu-id="439f1-109">Appservice</span></span>

* <span data-ttu-id="439f1-110">Correction d’une exception qui se produisait lors de la création d’une nouvelle application web Linux basée sur git</span><span class="sxs-lookup"><span data-stu-id="439f1-110">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="439f1-111">Event Grid</span><span class="sxs-lookup"><span data-stu-id="439f1-111">Event Grid</span></span>

* <span data-ttu-id="439f1-112">Ajout de dépendances du kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="439f1-112">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="439f1-113">11 août 2017</span><span class="sxs-lookup"><span data-stu-id="439f1-113">August 11, 2017</span></span>

<span data-ttu-id="439f1-114">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="439f1-114">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="439f1-115">ACS</span><span class="sxs-lookup"><span data-stu-id="439f1-115">ACS</span></span>

* <span data-ttu-id="439f1-116">Ajout de nouvelles régions d’aperçu</span><span class="sxs-lookup"><span data-stu-id="439f1-116">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="439f1-117">Batch</span><span class="sxs-lookup"><span data-stu-id="439f1-117">Batch</span></span>

* <span data-ttu-id="439f1-118">Mise à jour vers Kit de développement logiciel (DSK) de lot 3.1.0 et Kit de développement logiciel (SDK) de gestion de lot 4.1.0</span><span class="sxs-lookup"><span data-stu-id="439f1-118">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="439f1-119">Ajout d'une nouvelle commande affichant le nombre de tâches d’un travail</span><span class="sxs-lookup"><span data-stu-id="439f1-119">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="439f1-120">Correction du bogue dans le traitement de l’URL de la signature d'accès partagé du fichier de ressources</span><span class="sxs-lookup"><span data-stu-id="439f1-120">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="439f1-121">Point de terminaison de compte Batch prend désormais en charge le préfixe « https:// » facultatif</span><span class="sxs-lookup"><span data-stu-id="439f1-121">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="439f1-122">Prise en charge de l’ajout des listes de plus de 100 tâches à un travail</span><span class="sxs-lookup"><span data-stu-id="439f1-122">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="439f1-123">Ajout de l’enregistrement de débogage pour le chargement du module de commande Extensions</span><span class="sxs-lookup"><span data-stu-id="439f1-123">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="439f1-124">Composant</span><span class="sxs-lookup"><span data-stu-id="439f1-124">Component</span></span>

* <span data-ttu-id="439f1-125">Ajout d’un avertissement de désapprobation aux commandes « az component »</span><span class="sxs-lookup"><span data-stu-id="439f1-125">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="439f1-126">Conteneur</span><span class="sxs-lookup"><span data-stu-id="439f1-126">Container</span></span>

* <span data-ttu-id="439f1-127">`create` : correction d’un problème qui empêchait l’autorisation de signe égal à l’intérieur d’une variable d’environnement</span><span class="sxs-lookup"><span data-stu-id="439f1-127">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="439f1-128">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="439f1-128">Data Lake Store</span></span>

* <span data-ttu-id="439f1-129">Contrôle de progression activé</span><span class="sxs-lookup"><span data-stu-id="439f1-129">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="439f1-130">Event Grid</span><span class="sxs-lookup"><span data-stu-id="439f1-130">Event Grid</span></span>

* <span data-ttu-id="439f1-131">Version initiale</span><span class="sxs-lookup"><span data-stu-id="439f1-131">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="439f1-132">Réseau</span><span class="sxs-lookup"><span data-stu-id="439f1-132">Network</span></span>

* <span data-ttu-id="439f1-133">`lb` : correction d’un problème qui empêchait certains noms de ressources enfant d’être résolus correctement lorsqu’ils étaient omis</span><span class="sxs-lookup"><span data-stu-id="439f1-133">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="439f1-134">`application-gateway {subresource} delete` : correction d’un problème en raison duquel `--no-wait` n’était pas honorée</span><span class="sxs-lookup"><span data-stu-id="439f1-134">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="439f1-135">`application-gateway http-settings update` : correction d’un problème `--connection-draining-timeout` qui empêchait la désactivation de</span><span class="sxs-lookup"><span data-stu-id="439f1-135">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="439f1-136">Correction de erreur argument du mot-clé inattendu `sa_data_size_kilobyes` avec`az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="439f1-136">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="439f1-137">Profil</span><span class="sxs-lookup"><span data-stu-id="439f1-137">Profile</span></span>

* <span data-ttu-id="439f1-138">`account list` : ajout de `--refresh` pour synchroniser les derniers abonnements à partir du serveur</span><span class="sxs-lookup"><span data-stu-id="439f1-138">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="439f1-139">Storage</span><span class="sxs-lookup"><span data-stu-id="439f1-139">Storage</span></span>

* <span data-ttu-id="439f1-140">Activer le compte de stockage de mise à jour avec l’identité attribuée par le système</span><span class="sxs-lookup"><span data-stu-id="439f1-140">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="439f1-141">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="439f1-141">VM</span></span>

* <span data-ttu-id="439f1-142">`availability-set` : nombre de domaines d’erreur exposé sur convert</span><span class="sxs-lookup"><span data-stu-id="439f1-142">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="439f1-143">Commande `list-skus` exposée</span><span class="sxs-lookup"><span data-stu-id="439f1-143">Exposed `list-skus` command</span></span>
* <span data-ttu-id="439f1-144">Prise en charge pour affecter l’identité avec ou sans création d’attributions de rôle</span><span class="sxs-lookup"><span data-stu-id="439f1-144">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="439f1-145">Appliquer la référence (SKU) de stockage lors de l’attachement de disques de données</span><span class="sxs-lookup"><span data-stu-id="439f1-145">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="439f1-146">Suppression du nom du disque du système d’exploitation par défaut et de la référence (SKU) de stockage lors de l’utilisation des disques gérés</span><span class="sxs-lookup"><span data-stu-id="439f1-146">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="439f1-147">28 juillet 2017</span><span class="sxs-lookup"><span data-stu-id="439f1-147">July 28, 2017</span></span>

<span data-ttu-id="439f1-148">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="439f1-148">Version 2.0.12</span></span>

* <span data-ttu-id="439f1-149">Ajout de commandes de conteneur</span><span class="sxs-lookup"><span data-stu-id="439f1-149">Added container commands</span></span>
* <span data-ttu-id="439f1-150">Ajout de modules de facturation et de consommation</span><span class="sxs-lookup"><span data-stu-id="439f1-150">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="439f1-151">Principal</span><span class="sxs-lookup"><span data-stu-id="439f1-151">Core</span></span>

* <span data-ttu-id="439f1-152">Informations d’authentification du Kit de développement logiciel (SDK) de sortie pour les principaux de service avec des certificats</span><span class="sxs-lookup"><span data-stu-id="439f1-152">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="439f1-153">Correction des exceptions de progression de déploiement</span><span class="sxs-lookup"><span data-stu-id="439f1-153">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="439f1-154">Utiliser le point de terminaison ARM à partir du cloud actuel pour créer le client de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="439f1-154">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="439f1-155">Amélioration de la gestion simultanée de fichiers clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="439f1-155">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="439f1-156">Actualiser l’ID de la demande client pour chaque exécution de la commande</span><span class="sxs-lookup"><span data-stu-id="439f1-156">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="439f1-157">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel ( SDK) (#3635)</span><span class="sxs-lookup"><span data-stu-id="439f1-157">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="439f1-158">Rapports de progression pour les déploiements de modèle (#3510)</span><span class="sxs-lookup"><span data-stu-id="439f1-158">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="439f1-159">Ajout de la prise en charge des champs de sortie de la table de prélèvement via la requête jmespath (#3581)</span><span class="sxs-lookup"><span data-stu-id="439f1-159">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="439f1-160">Amélioration de la désactivation des arguments d’analyse et de l’historique Ajout avec des mouvements (#3434)</span><span class="sxs-lookup"><span data-stu-id="439f1-160">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="439f1-161">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="439f1-161">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="439f1-162">Déplacer tous les fichiers d’enregistrement existant vers le dernier dossier</span><span class="sxs-lookup"><span data-stu-id="439f1-162">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="439f1-163">Correction de l’idempotence pour VM/VMSS create (#3586)</span><span class="sxs-lookup"><span data-stu-id="439f1-163">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="439f1-164">Les chemins d’accès de la commande ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="439f1-164">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="439f1-165">Certains paramètres de type booléen ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="439f1-165">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="439f1-166">Prise en charge de la connexion à ADFS sur le serveur local de manière identique à Azure Stack</span><span class="sxs-lookup"><span data-stu-id="439f1-166">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="439f1-167">Correction des écritures simultanées dans clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="439f1-167">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="439f1-168">ACR</span><span class="sxs-lookup"><span data-stu-id="439f1-168">ACR</span></span>

* <span data-ttu-id="439f1-169">Ajout de la commande `show-usage` pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="439f1-169">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="439f1-170">Prise en charge de la mise à jour de la référence (SKU) pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="439f1-170">Support SKU update for managed registries</span></span>
* <span data-ttu-id="439f1-171">Ajout de registres gérés avec la référence (SKU) gérée</span><span class="sxs-lookup"><span data-stu-id="439f1-171">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="439f1-172">Ajout de webhooks pour les registres gérés avec le module de commande acr webhook</span><span class="sxs-lookup"><span data-stu-id="439f1-172">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="439f1-173">Ajout de l’authentification AAD avec la commande de connexion acr</span><span class="sxs-lookup"><span data-stu-id="439f1-173">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="439f1-174">Ajout de la commande de suppression pour les référentiels docker, les manifestes et les balises</span><span class="sxs-lookup"><span data-stu-id="439f1-174">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="439f1-175">ACS</span><span class="sxs-lookup"><span data-stu-id="439f1-175">ACS</span></span>

* <span data-ttu-id="439f1-176">Prise en charge des API version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="439f1-176">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="439f1-177">AppService</span><span class="sxs-lookup"><span data-stu-id="439f1-177">Appservice</span></span>

* <span data-ttu-id="439f1-178">Correction d’un bogue à cause duquel l’énumération d’une application Linux ne retournait absolument rien</span><span class="sxs-lookup"><span data-stu-id="439f1-178">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="439f1-179">Prise en charge de la récupération de références depuis ACR</span><span class="sxs-lookup"><span data-stu-id="439f1-179">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="439f1-180">Supprimer toutes les commandes sous `appservice web`</span><span class="sxs-lookup"><span data-stu-id="439f1-180">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="439f1-181">Masquer les mots de passe du registre docker de la commande de sortie (#3656)</span><span class="sxs-lookup"><span data-stu-id="439f1-181">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="439f1-182">Vérifier que le navigateur par défaut est utilisé sur macOs sans erreurs (#3623)</span><span class="sxs-lookup"><span data-stu-id="439f1-182">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="439f1-183">Améliorer l’aide de `webapp log tail` et `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="439f1-183">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="439f1-184">Commandes `traffic-routing` exposées pour configurer le routage statique (#3566)</span><span class="sxs-lookup"><span data-stu-id="439f1-184">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="439f1-185">Ajout de correctifs de fiabilité pour la configuration du contrôle de code source (#3245)</span><span class="sxs-lookup"><span data-stu-id="439f1-185">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="439f1-186">Suppression d’un argument non pris en charge `--node-version` de `webapp config update` pour les applications Web de Windows.</span><span class="sxs-lookup"><span data-stu-id="439f1-186">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="439f1-187">Utilisez à la place `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="439f1-187">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="439f1-188">Batch</span><span class="sxs-lookup"><span data-stu-id="439f1-188">Batch</span></span>

* <span data-ttu-id="439f1-189">Mise à jour vers kit de développement logiciel (SDK) de lot 3.0.0 avec prise en charge pour les machines virtuelles de faible priorité dans des pools</span><span class="sxs-lookup"><span data-stu-id="439f1-189">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="439f1-190">Renommage `pool create` option `--target-dedicated` en `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="439f1-190">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="439f1-191">Ajout des options `pool create`, `--target-low-priority-nodes` et `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="439f1-191">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="439f1-192">CDN</span><span class="sxs-lookup"><span data-stu-id="439f1-192">CDN</span></span>

* <span data-ttu-id="439f1-193">Fourni un meilleur message d’erreur pour `cdn endpoint list` quand le profil spécifié par `--profile-name` n’existe pas.</span><span class="sxs-lookup"><span data-stu-id="439f1-193">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist.</span></span>

### <a name="cloud"></a><span data-ttu-id="439f1-194">Cloud</span><span class="sxs-lookup"><span data-stu-id="439f1-194">Cloud</span></span>

* <span data-ttu-id="439f1-195">Modification de la version de l’API du point de terminaison de métadonnées du cloud au format AAAA-MM-JJ</span><span class="sxs-lookup"><span data-stu-id="439f1-195">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="439f1-196">Le point de terminaison de la galerie n’est pas nécessaire</span><span class="sxs-lookup"><span data-stu-id="439f1-196">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="439f1-197">Prise en charge de l’inscription du cloud, avec le point de terminaison ARM resource manager</span><span class="sxs-lookup"><span data-stu-id="439f1-197">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="439f1-198">Ajout d’une option pour `cloud set` permettant de choisir le profil lors de la sélection du cloud actuel</span><span class="sxs-lookup"><span data-stu-id="439f1-198">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="439f1-199">Exposé `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="439f1-199">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="439f1-200">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="439f1-200">CosmosDB</span></span>

* <span data-ttu-id="439f1-201">Correction relative à la permission de la création de collection avec une clé de partition personnalisée</span><span class="sxs-lookup"><span data-stu-id="439f1-201">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="439f1-202">Ajout de la prise en charge de la durée de vie par défaut de la collection.</span><span class="sxs-lookup"><span data-stu-id="439f1-202">Added support for collection default TTL.</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="439f1-203">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="439f1-203">Data Lake Analytics</span></span>

* <span data-ttu-id="439f1-204">Ajout de commandes pour la gestion de la stratégie de calcul sous le titre `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="439f1-204">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="439f1-205">Ajout de `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="439f1-205">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="439f1-206">Ajout de `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="439f1-206">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="439f1-207">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="439f1-207">Data Lake Store</span></span>

* <span data-ttu-id="439f1-208">Ajout de la prise en charge pour la rotation de coffre de clés gérés par l’utilisateur dans `dls account update`</span><span class="sxs-lookup"><span data-stu-id="439f1-208">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="439f1-209">Mise à jour de la version du kit de développement logiciel (SDK) du système de fichiers Data Lake Store sous-jacente, réglant un problème de performance</span><span class="sxs-lookup"><span data-stu-id="439f1-209">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="439f1-210">Ajout de la commande `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="439f1-210">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="439f1-211">Cette commande tente d’activer un utilisateur de coffre de clés fourni par l’utilisateur pour utiliser le chiffrement des données dans un compte Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="439f1-211">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="439f1-212">Interactive</span><span class="sxs-lookup"><span data-stu-id="439f1-212">Interactive</span></span>

* <span data-ttu-id="439f1-213">Amélioration du temps de démarrage à l’aide des commandes en cache</span><span class="sxs-lookup"><span data-stu-id="439f1-213">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="439f1-214">Couverture de test accrue</span><span class="sxs-lookup"><span data-stu-id="439f1-214">Increased test coverage</span></span>
* <span data-ttu-id="439f1-215">Amélioration du mouvement « ? » pour injecter également dans la commande suivante</span><span class="sxs-lookup"><span data-stu-id="439f1-215">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="439f1-216">Correction d’erreurs interactives avec le profil 2017-03-09-profil-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="439f1-216">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="439f1-217">Autorisé `--version` en tant que paramètre pour le mode interactif (#3645)</span><span class="sxs-lookup"><span data-stu-id="439f1-217">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="439f1-218">Empêche le mode interactif de lever des erreurs à partir des listes de saisie semi-automatique de validation (#3570)</span><span class="sxs-lookup"><span data-stu-id="439f1-218">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="439f1-219">Rapports de progression pour les déploiements de modèles (#3510)</span><span class="sxs-lookup"><span data-stu-id="439f1-219">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="439f1-220">Ajout de l’indicateur `--progress`</span><span class="sxs-lookup"><span data-stu-id="439f1-220">Added `--progress` flag</span></span>
* <span data-ttu-id="439f1-221">Suppression `--debug` et `--verbose` des listes de saisie semi-automatique</span><span class="sxs-lookup"><span data-stu-id="439f1-221">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="439f1-222">Suppression `interactive` des listes de saisie semi-automatique (#3324)</span><span class="sxs-lookup"><span data-stu-id="439f1-222">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="439f1-223">IoT</span><span class="sxs-lookup"><span data-stu-id="439f1-223">IoT</span></span>

* <span data-ttu-id="439f1-224">La création de la stratégie n’efface plus les stratégies existantes.</span><span class="sxs-lookup"><span data-stu-id="439f1-224">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="439f1-225">(#3934)</span><span class="sxs-lookup"><span data-stu-id="439f1-225">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="439f1-226">Coffre de clés</span><span class="sxs-lookup"><span data-stu-id="439f1-226">Key vault</span></span>

* <span data-ttu-id="439f1-227">Ajout de commandes pour les fonctionnalités de récupération de coffre de clés :</span><span class="sxs-lookup"><span data-stu-id="439f1-227">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="439f1-228">`keyvault`sous-commandes `purge`, `recover`,`keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="439f1-228">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="439f1-229">`keyvault secret`sous-commandes `backup`, `restore`, `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="439f1-229">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="439f1-230">`keyvault certificate`sous-commandes `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="439f1-230">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="439f1-231">`keyvault key`sous-commandes `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="439f1-231">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="439f1-232">Ajout de l’intégration du coffre de clés du principal du service (#3133)</span><span class="sxs-lookup"><span data-stu-id="439f1-232">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="439f1-233">Mise à jour du plan de données du coffre de clés vers 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="439f1-233">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="439f1-234">(#3307)</span><span class="sxs-lookup"><span data-stu-id="439f1-234">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="439f1-235">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="439f1-235">Lab</span></span>

* <span data-ttu-id="439f1-236">Ajout de la prise en charge de la revendication de toutes les machines virtuelles dans le laboratoire via `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="439f1-236">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="439f1-237">Ajout du formateur de sortie de tableau pour `az lab vm list` et `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="439f1-237">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="439f1-238">Surveiller</span><span class="sxs-lookup"><span data-stu-id="439f1-238">Monitor</span></span>

* <span data-ttu-id="439f1-239">Correctif pour le fichier de modèle avec `monitor autoscale-settings get-parameters-template` commande (#3349)</span><span class="sxs-lookup"><span data-stu-id="439f1-239">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="439f1-240">Renommage de `monitor alert-rule-incidents list` en `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="439f1-240">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="439f1-241">Renommage de `monitor alert-rule-incidents show` en `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="439f1-241">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="439f1-242">Renommage de `monitor metric-defintions list` en `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="439f1-242">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="439f1-243">Renommage de `monitor alert-rules` en `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="439f1-243">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="439f1-244">Modifié `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="439f1-244">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="439f1-245">sous-commandes`condition` et `action` n’acceptent plus JSON</span><span class="sxs-lookup"><span data-stu-id="439f1-245">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="439f1-246">Ajout de nombreux paramètres simplifiant le processus de création de règle</span><span class="sxs-lookup"><span data-stu-id="439f1-246">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="439f1-247">`location` n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="439f1-247">`location` no longer required</span></span>
  * <span data-ttu-id="439f1-248">Ajout d’un nom et de la prise en charge de l’ID de la cible</span><span class="sxs-lookup"><span data-stu-id="439f1-248">Add name and ID support for target</span></span>
  * <span data-ttu-id="439f1-249">Suppression de `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="439f1-249">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="439f1-250">Le renommage de `is-enabled` en `enabled`n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="439f1-250">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="439f1-251">`description` par défaut sont désormais basées sur la condition fournie</span><span class="sxs-lookup"><span data-stu-id="439f1-251">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="439f1-252">Ajout d’exemples aidant à clarifier le nouveau format</span><span class="sxs-lookup"><span data-stu-id="439f1-252">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="439f1-253">Prise en charge des noms ou des ID pour les commandes `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="439f1-253">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="439f1-254">Ajout d’arguments d’usage et d’exemples pour `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="439f1-254">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="439f1-255">Réseau</span><span class="sxs-lookup"><span data-stu-id="439f1-255">Network</span></span>

* <span data-ttu-id="439f1-256">Ajout de la commande `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="439f1-256">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="439f1-257">Ajout de l’argument `--private-access-services` à `vnet subnet create` et `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="439f1-257">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="439f1-258">Correction d’un problème `application-gateway redirect-config create` qui causait l’échec de</span><span class="sxs-lookup"><span data-stu-id="439f1-258">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="439f1-259">Correction d’un problème `application-gateway redirect-config update` qui `--no-wait` empêchait le fonctionnement de</span><span class="sxs-lookup"><span data-stu-id="439f1-259">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="439f1-260">Correction d’un bogue lié à l’utilisation d’un `--servers` argument avec `application-gateway address-pool create` et `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="439f1-260">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="439f1-261">Ajout des commandes `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="439f1-261">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="439f1-262">Ajout de commandes à `application-gateway ssl-policy` : `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="439f1-262">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="439f1-263">Ajout d’arguments à `application-gateway ssl-policy set` : `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="439f1-263">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="439f1-264">Ajout d’arguments à `application-gateway http-settings create` et `application-gateway http-settings update` : `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="439f1-264">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="439f1-265">Ajout d’arguments à `application-gateway url-path-map create` et `application-gateway url-path-map update`, `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="439f1-265">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="439f1-266">Ajout d’un argument `--redirect-config` à `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="439f1-266">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="439f1-267">Ajout de la prise en charge de `--no-wait` pour `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="439f1-267">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="439f1-268">Ajout d’arguments à `application-gateway probe create` et `application-gateway probe update` : `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="439f1-268">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="439f1-269">Ajout d’un argument `--redirect-config` à `application-gateway rule create` et `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="439f1-269">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="439f1-270">Ajout de la prise en charge de `--accelerated-networking` pour `nic create` et `nic update`</span><span class="sxs-lookup"><span data-stu-id="439f1-270">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="439f1-271">Suppression de l’ `--internal-dns-name-suffix` argument à partir de `nic create`</span><span class="sxs-lookup"><span data-stu-id="439f1-271">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="439f1-272">Ajout de la prise en charge de `--dns-servers` pour `nic update` et `nic create` : ajout de la prise en charge pour les serveurs DNS :</span><span class="sxs-lookup"><span data-stu-id="439f1-272">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="439f1-273">Correction d’un bogue qui faisait `local-gateway create` ignorer `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="439f1-273">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="439f1-274">Ajout de la prise en charge de `--dns-servers` pour `vnet update`</span><span class="sxs-lookup"><span data-stu-id="439f1-274">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="439f1-275">Correction d’un bogue lors de la création d’une homologation sans filtrage de l’itinéraire avec `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="439f1-275">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="439f1-276">Correction d’un bogue qui empêchait le fonctionnement des arguments `--provider` et `--bandwidth` avec `express-route update`</span><span class="sxs-lookup"><span data-stu-id="439f1-276">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="439f1-277">Correction d’un bogue avec `network watcher show-topology` une logique de valeurs par défaut</span><span class="sxs-lookup"><span data-stu-id="439f1-277">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="439f1-278">Amélioration de la mise en forme de sortie pour `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="439f1-278">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="439f1-279">Utilisation de l’IP frontale par défaut pour `application-gateway http-listener create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="439f1-279">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="439f1-280">Utilisation d’un pool d’adresses par défaut, des paramètres HTTP et de l’écouteur HTTP pour `application-gateway rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="439f1-280">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="439f1-281">Utilisation de l’IP frontale par défaut et du pool principal `lb rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="439f1-281">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="439f1-282">Utilisation de l’IP frontale par défaut pour `lb inbound-nat-rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="439f1-282">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="439f1-283">Profil</span><span class="sxs-lookup"><span data-stu-id="439f1-283">Profile</span></span>

* <span data-ttu-id="439f1-284">Prise en charge de la connexion à l’intérieur d’une machine virtuelle avec une identité gérée</span><span class="sxs-lookup"><span data-stu-id="439f1-284">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="439f1-285">Prise en charge de la sortie pour `account show` au format de fichier d’authentification du Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="439f1-285">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="439f1-286">Affichage des avertissements de désapprobation lors de l’utilisation de '--expanded-view'</span><span class="sxs-lookup"><span data-stu-id="439f1-286">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="439f1-287">Ajout de la commande `get-access-token` permettant de fournir un jeton AAD brut</span><span class="sxs-lookup"><span data-stu-id="439f1-287">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="439f1-288">Prise en charge de la connexion avec un compte d’utilisateur sans abonnements associés</span><span class="sxs-lookup"><span data-stu-id="439f1-288">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="439f1-289">SGBDR</span><span class="sxs-lookup"><span data-stu-id="439f1-289">RDBMS</span></span>

* <span data-ttu-id="439f1-290">Prise en charge de l’énumération de serveurs à travers un abonnement (#3417)</span><span class="sxs-lookup"><span data-stu-id="439f1-290">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="439f1-291">Correction de `%s` non traité car il manque `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="439f1-291">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="439f1-292">Correction du mappage de la source du document et ajout de la tâche CI permettant la vérification de (#3361)</span><span class="sxs-lookup"><span data-stu-id="439f1-292">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="439f1-293">Correction concernant l’aide relative à MySQL et PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="439f1-293">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="439f1-294">Ressource</span><span class="sxs-lookup"><span data-stu-id="439f1-294">Resource</span></span>

* <span data-ttu-id="439f1-295">Amélioration des invites pour les paramètres manquants de `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="439f1-295">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="439f1-296">Amélioration de l’analyse de `--parameters KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="439f1-296">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="439f1-297">Correction des problèmes à cause desquels `group deployment create` les fichiers de paramètres n’étaient plus reconnus à l’aide de la `@<file>` syntaxe</span><span class="sxs-lookup"><span data-stu-id="439f1-297">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="439f1-298">Prise en charge de l’ `--ids` argument pour `resource` et `managedapp` les commandes</span><span class="sxs-lookup"><span data-stu-id="439f1-298">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="439f1-299">Correction de certains messages d’analyse et d’erreur (#3584)</span><span class="sxs-lookup"><span data-stu-id="439f1-299">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="439f1-300">Correction de l’analyse `--resource-type` permettant à la `lock` commande d’accepter `<resource-namespace>` et `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="439f1-300">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="439f1-301">Ajout de la vérification de paramètre des modèles de liaison de modèle (#3629)</span><span class="sxs-lookup"><span data-stu-id="439f1-301">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="439f1-302">Ajout de la prise en charge de la spécification des paramètres de déploiement à l’aide de la `KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="439f1-302">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="439f1-303">Rôle</span><span class="sxs-lookup"><span data-stu-id="439f1-303">Role</span></span>

* <span data-ttu-id="439f1-304">Prise en charge de la sortie au format de fichier d’authentification du Kit de développement logiciel (SDK) pour `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="439f1-304">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="439f1-305">Nettoyage des attributions de rôles et de l’application AAD liée lors de la suppression d’un principal de service (#3610)</span><span class="sxs-lookup"><span data-stu-id="439f1-305">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="439f1-306">Inclusion du format d’heure dans `app create` args `--start-date` et `--end-date` descriptions</span><span class="sxs-lookup"><span data-stu-id="439f1-306">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="439f1-307">Affichage des avertissements de désapprobation lors de l’utilisation de `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="439f1-307">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="439f1-308">Ajout de l’intégration du coffre de clés pour les commandes `create-for-rbac` et `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="439f1-308">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="439f1-309">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="439f1-309">Service Fabric</span></span>
* <span data-ttu-id="439f1-310">Correction d’un problème avec les fichiers volumineux dans les applications tronquées sur le chargement (#3666)</span><span class="sxs-lookup"><span data-stu-id="439f1-310">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="439f1-311">Ajout de tests pour les commandes Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="439f1-311">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="439f1-312">Correction de nombreuses commandes Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="439f1-312">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="439f1-313">SQL</span><span class="sxs-lookup"><span data-stu-id="439f1-313">SQL</span></span>

* <span data-ttu-id="439f1-314">Suppression du paramètre rompu `sql server create` `--identity`</span><span class="sxs-lookup"><span data-stu-id="439f1-314">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="439f1-315">Suppression des valeurs de mot de passe à partir de la sortie de commande `sql server create` et `sql server update`</span><span class="sxs-lookup"><span data-stu-id="439f1-315">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="439f1-316">Ajout des commandes `sql db list-editions` et `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="439f1-316">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="439f1-317">Storage</span><span class="sxs-lookup"><span data-stu-id="439f1-317">Storage</span></span>

* <span data-ttu-id="439f1-318">Suppression d’une `--marker` option à partir des commandes `storage blob list`, `storage container list`et `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="439f1-318">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="439f1-319">Activation de la création d’un compte de stockage https-only</span><span class="sxs-lookup"><span data-stu-id="439f1-319">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="439f1-320">Mise à jour des métriques de stockage, de la journalisation et des commandes cors (#3495)</span><span class="sxs-lookup"><span data-stu-id="439f1-320">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="439f1-321">Reformulation d’un message d’exception de l’ajout CORS (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="439f1-321">Rephrased exception message from CORS add (#3638) (#3362)</span></span>  
* <span data-ttu-id="439f1-322">Conversion du générateur à une liste en mode exécution d’essai de la commande de téléchargement de lot (#3592)</span><span class="sxs-lookup"><span data-stu-id="439f1-322">Converted generator to a list in download batch command dry run mode (#3592)</span></span> 
* <span data-ttu-id="439f1-323">Correction du problème d’essai associé au lot de téléchargement du blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="439f1-323">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="439f1-324">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="439f1-324">VM</span></span>

* <span data-ttu-id="439f1-325">Prise en charge de la configuration du groupe de sécurité réseau</span><span class="sxs-lookup"><span data-stu-id="439f1-325">Support configuring nsg</span></span>
* <span data-ttu-id="439f1-326">Correction d’un bogue qui entraînait une configuration incorrecte du serveur DNS</span><span class="sxs-lookup"><span data-stu-id="439f1-326">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="439f1-327">Prise en charge des identités de service géré</span><span class="sxs-lookup"><span data-stu-id="439f1-327">Support managed service identities</span></span>
* <span data-ttu-id="439f1-328">Correction d’un problème à cause duquel `cmss create` avec un équilibreur de charge existant exigeait `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="439f1-328">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`.</span></span>
* <span data-ttu-id="439f1-329">Les disques de données créés avec le numéro d’unité logique `vm image create` commencent à 0</span><span class="sxs-lookup"><span data-stu-id="439f1-329">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="439f1-330">10 mai 2017</span><span class="sxs-lookup"><span data-stu-id="439f1-330">May 10, 2017</span></span>

<span data-ttu-id="439f1-331">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="439f1-331">Version 2.0.6</span></span>

* <span data-ttu-id="439f1-332">documentdb renommé en cosmosdb</span><span class="sxs-lookup"><span data-stu-id="439f1-332">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="439f1-333">Ajouter rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="439f1-333">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="439f1-334">Inclure les modules Data Lake Analytics et Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="439f1-334">Include Data Lake Analytics and Data Lake Store modules.</span></span>
* <span data-ttu-id="439f1-335">Inclure le module Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="439f1-335">Include Cognitive Services module.</span></span>
* <span data-ttu-id="439f1-336">Inclure le module Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="439f1-336">Include Service Fabric module.</span></span>
* <span data-ttu-id="439f1-337">Inclure le module Interactive (az-shell renommé).</span><span class="sxs-lookup"><span data-stu-id="439f1-337">Include Interactive module (rename of az-shell).</span></span>
* <span data-ttu-id="439f1-338">Ajouter la prise en charge des commandes CDN.</span><span class="sxs-lookup"><span data-stu-id="439f1-338">Add support for CDN commands.</span></span>
* <span data-ttu-id="439f1-339">Supprimer le module Container.</span><span class="sxs-lookup"><span data-stu-id="439f1-339">Remove Container module.</span></span>
* <span data-ttu-id="439f1-340">Ajouter « az -v » comme raccourci pour « az --version » ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="439f1-340">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="439f1-341">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="439f1-341">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="439f1-342">Principal</span><span class="sxs-lookup"><span data-stu-id="439f1-342">Core</span></span>

* <span data-ttu-id="439f1-343">principal : capturer les exceptions provoquées par un fournisseur non enregistré et l’enregistrer automatiquement</span><span class="sxs-lookup"><span data-stu-id="439f1-343">core: capture exceptions caused by unregistered provider and auto-register it</span></span>   
* <span data-ttu-id="439f1-344">performance : conserver le cache de jeton adal en mémoire jusqu’à la fin du processus ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="439f1-344">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="439f1-345">Corriger les octets retournés par l’empreinte digitale hex -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="439f1-345">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="439f1-346">Téléchargement du certificat Key Vault et intégration AAD SP améliorés ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="439f1-346">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="439f1-347">Ajouter l’emplacement de Python à « az —version » ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="439f1-347">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="439f1-348">connexion : prise en charge de la connexion lorsqu’il n’y a aucun abonnement ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="439f1-348">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="439f1-349">principal : corriger une erreur lors de la connexion à l’aide d’un principal de service deux fois ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="439f1-349">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="439f1-350">principal : autoriser la configuration du chemin d’accès de accessTokens.json via une variable d’environnement ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="439f1-350">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="439f1-351">principal : autoriser l’application des valeurs par défaut configurées sur les arguments facultatifs ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="439f1-351">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="439f1-352">principal : performances améliorées</span><span class="sxs-lookup"><span data-stu-id="439f1-352">core: Improved performance</span></span>
* <span data-ttu-id="439f1-353">principal : certificats d’autorité de certification personnalisés - prise en charge de la définition de la variable d’environnement REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="439f1-353">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="439f1-354">principal : configuration du cloud - utiliser le point de terminaison « resource manager » si le point de terminaison « management » n’est pas défini</span><span class="sxs-lookup"><span data-stu-id="439f1-354">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="439f1-355">ACS</span><span class="sxs-lookup"><span data-stu-id="439f1-355">ACS</span></span>

* <span data-ttu-id="439f1-356">corriger le nombre de maîtres et d’agents sur un nombre entier au lieu d’une chaîne</span><span class="sxs-lookup"><span data-stu-id="439f1-356">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="439f1-357">exposer « az acs create --no-wait » et « az acs wait » pour la création asynchrone</span><span class="sxs-lookup"><span data-stu-id="439f1-357">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="439f1-358">exposer « az acs create --validate » pour les validations de test</span><span class="sxs-lookup"><span data-stu-id="439f1-358">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="439f1-359">supprimer le profil Windows avant l’appel PUT pour la commande de mise à l’échelle ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="439f1-359">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="439f1-360">AppService</span><span class="sxs-lookup"><span data-stu-id="439f1-360">AppService</span></span>

* <span data-ttu-id="439f1-361">functionapp : ajouter la prise en charge complète de functionapp, notamment créer, afficher, liste, supprimer, nom d’hôte, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="439f1-361">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="439f1-362">Ajout de Team Services (vsts) comme option de livraison continue à « config contrôle source web appservice »</span><span class="sxs-lookup"><span data-stu-id="439f1-362">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="439f1-363">Créer « az webapp » pour remplacer « az appservice web » (pour la rétrocompatibilité, « az appservice web » sera conservé dans les 2 prochaines versions)</span><span class="sxs-lookup"><span data-stu-id="439f1-363">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="439f1-364">Exposer des arguments pour configurer le déploiement et des « piles d’exécution » sur webapp create</span><span class="sxs-lookup"><span data-stu-id="439f1-364">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="439f1-365">Exposer « webapp list-runtimes »</span><span class="sxs-lookup"><span data-stu-id="439f1-365">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="439f1-366">prendre en charge la configuration des chaînes de connexion ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="439f1-366">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="439f1-367">prendre en charge le basculement d’emplacement avec aperçu</span><span class="sxs-lookup"><span data-stu-id="439f1-367">support slot swap with preview</span></span>
* <span data-ttu-id="439f1-368">Supprimer les erreurs des commandes appservice ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="439f1-368">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="439f1-369">Utiliser le groupe de ressources du plan app service pour les opérations de certificat ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="439f1-369">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="439f1-370">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="439f1-370">CosmosDB</span></span>

* <span data-ttu-id="439f1-371">Renommer le module documentdb en cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="439f1-371">Rename documentdb module to cosmosdb.</span></span>
* <span data-ttu-id="439f1-372">Prise en charge ajoutée pour les API de plan de données documentdb : gestion de base de données et de collecte</span><span class="sxs-lookup"><span data-stu-id="439f1-372">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="439f1-373">Prise en charge ajoutée pour activer le basculement automatique sur les comptes de base de données</span><span class="sxs-lookup"><span data-stu-id="439f1-373">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="439f1-374">Prise en charge ajoutée pour la nouvelle stratégie de cohérence ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="439f1-374">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="439f1-375">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="439f1-375">Data Lake Analytics</span></span>

* <span data-ttu-id="439f1-376">Corriger un bogue dans lequel le filtrage sur le résultat et l’état des listes de travaux lève une erreur.</span><span class="sxs-lookup"><span data-stu-id="439f1-376">Fix a bug where filtering on result and state for job lists would throw an error.</span></span>
* <span data-ttu-id="439f1-377">Ajouter la prise en charge d’un nouveau type d’élément de catalogue : paquet.</span><span class="sxs-lookup"><span data-stu-id="439f1-377">Add support for new catalog item type: package.</span></span> <span data-ttu-id="439f1-378">accessible via : `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="439f1-378">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="439f1-379">A rendu possible le fait de répertorier les éléments de catalogue suivants à partir d’une base de données (aucune spécification de schéma requise) :</span><span class="sxs-lookup"><span data-stu-id="439f1-379">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="439f1-380">Table</span><span class="sxs-lookup"><span data-stu-id="439f1-380">Table</span></span>
  * <span data-ttu-id="439f1-381">Fonction table</span><span class="sxs-lookup"><span data-stu-id="439f1-381">Table valued function</span></span>
  * <span data-ttu-id="439f1-382">Affichage</span><span class="sxs-lookup"><span data-stu-id="439f1-382">View</span></span>
  * <span data-ttu-id="439f1-383">Statistiques de table.</span><span class="sxs-lookup"><span data-stu-id="439f1-383">Table Statistics.</span></span> <span data-ttu-id="439f1-384">Cela peut également être répertorié avec un schéma, mais sans spécifier un nom de table.</span><span class="sxs-lookup"><span data-stu-id="439f1-384">This can also be listed with a schema, but without specifying a table name.</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="439f1-385">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="439f1-385">Data Lake Store</span></span>

* <span data-ttu-id="439f1-386">Mettre à jour la version du Kit de développement logiciel (SDK) du système de fichiers sous-jacent, qui offre une meilleure prise en charge pour gérer les scénarios de limitation côté serveur.</span><span class="sxs-lookup"><span data-stu-id="439f1-386">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios.</span></span>
* <span data-ttu-id="439f1-387">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="439f1-387">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="439f1-388">aide manquante pour afficher l’accès.</span><span class="sxs-lookup"><span data-stu-id="439f1-388">missed help for access show.</span></span> <span data-ttu-id="439f1-389">ajout en cours.</span><span class="sxs-lookup"><span data-stu-id="439f1-389">adding it.</span></span> <span data-ttu-id="439f1-390">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="439f1-390">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="439f1-391">Rechercher</span><span class="sxs-lookup"><span data-stu-id="439f1-391">Find</span></span>

* <span data-ttu-id="439f1-392">résultats de la recherche améliorés et autorisation du contrôle de version de l’index de recherche</span><span class="sxs-lookup"><span data-stu-id="439f1-392">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="439f1-393">KeyVault</span><span class="sxs-lookup"><span data-stu-id="439f1-393">KeyVault</span></span>

* <span data-ttu-id="439f1-394">BC : `az keyvault certificate download` remplacer -e dans chaîne ou élément binaire par PEM ou DER afin de mieux représenter les options</span><span class="sxs-lookup"><span data-stu-id="439f1-394">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="439f1-395">BC : Supprimer --expires et --not-before dans `keyvault certificate create` car ces paramètres ne sont pas pris en charge par le service.</span><span class="sxs-lookup"><span data-stu-id="439f1-395">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service.</span></span>
* <span data-ttu-id="439f1-396">Ajoute le paramètre --validity à `keyvault certificate create` pour substituer de manière sélective la valeur dans --policy</span><span class="sxs-lookup"><span data-stu-id="439f1-396">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="439f1-397">Résout le problème dans `keyvault certificate get-default-policy` où « expires » et « not_before » étaient exposés mais « validity_in_months » ne l’était pas.</span><span class="sxs-lookup"><span data-stu-id="439f1-397">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not.</span></span>
* <span data-ttu-id="439f1-398">correction de keyvault pour l’importation de pem et pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="439f1-398">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="439f1-399">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="439f1-399">Lab</span></span>

* <span data-ttu-id="439f1-400">Ajout des commandes créer, afficher, supprimer et liste pour l’environnement dans le laboratoire.</span><span class="sxs-lookup"><span data-stu-id="439f1-400">Adding create, show, delete & list commands for environment in the lab.</span></span>
* <span data-ttu-id="439f1-401">Ajout des commandes afficher et liste pour afficher les modèles ARM dans le laboratoire.</span><span class="sxs-lookup"><span data-stu-id="439f1-401">Adding show & list commands to view ARM templates in the lab.</span></span>
* <span data-ttu-id="439f1-402">Ajout de l’indicateur --environment dans `az lab vm list` pour filtrer les machines virtuelles selon l’environnement du laboratoire.</span><span class="sxs-lookup"><span data-stu-id="439f1-402">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab.</span></span>
* <span data-ttu-id="439f1-403">Ajout de la commande pratique `az lab formula export-artifacts` pour exporter une structure d’artefact dans une formule de laboratoire.</span><span class="sxs-lookup"><span data-stu-id="439f1-403">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula.</span></span>
* <span data-ttu-id="439f1-404">Ajout de commandes pour gérer les secrets dans un laboratoire.</span><span class="sxs-lookup"><span data-stu-id="439f1-404">Add commands to manage secrets within a Lab.</span></span>

### <a name="monitor"></a><span data-ttu-id="439f1-405">Surveiller</span><span class="sxs-lookup"><span data-stu-id="439f1-405">Monitor</span></span>

* <span data-ttu-id="439f1-406">Correction de bogue : modélisation `--actions` de `az alert-rules create` pour consommer la chaîne JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="439f1-406">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="439f1-407">Correction de bogue : la création de paramètres de diagnostic n’accepte pas les métriques/journaux à partir des commandes d’affichage ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="439f1-407">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="439f1-408">Réseau</span><span class="sxs-lookup"><span data-stu-id="439f1-408">Network</span></span>

* <span data-ttu-id="439f1-409">Ajouter la commande `network watcher test-connectivity`.</span><span class="sxs-lookup"><span data-stu-id="439f1-409">Add `network watcher test-connectivity` command.</span></span>
* <span data-ttu-id="439f1-410">Ajouter la prise en charge du paramètre `--filters` pour `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="439f1-410">Add support for `--filters` parameter for `network watcher packet-capture create`.</span></span>
* <span data-ttu-id="439f1-411">Ajouter la prise en charge pour le drainage de connexion Application Gateway.</span><span class="sxs-lookup"><span data-stu-id="439f1-411">Add support for Application Gateway connection draining.</span></span>
* <span data-ttu-id="439f1-412">Ajouter la prise en charge pour la configuration du jeu de règles WAF d’Application Gateway.</span><span class="sxs-lookup"><span data-stu-id="439f1-412">Add support for Application Gateway WAF rule set configuration.</span></span>
* <span data-ttu-id="439f1-413">Ajouter la prise en charge des règles et des filtres de routage ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="439f1-413">Add support for ExpressRoute route filters and rules.</span></span>
* <span data-ttu-id="439f1-414">Ajouter la prise en charge pour le routage géographique TrafficManager.</span><span class="sxs-lookup"><span data-stu-id="439f1-414">Add support for TrafficManager geographic routing.</span></span>
* <span data-ttu-id="439f1-415">Ajouter la prise en charge des sélecteurs de trafic basés sur la stratégie de connexion VPN.</span><span class="sxs-lookup"><span data-stu-id="439f1-415">Add support for VPN connection policy-based traffic selectors.</span></span>
* <span data-ttu-id="439f1-416">Ajouter la prise en charge pour les stratégies IPSec de la connexion VPN.</span><span class="sxs-lookup"><span data-stu-id="439f1-416">Add support for VPN connection IPSec policies.</span></span>
* <span data-ttu-id="439f1-417">Corriger le bogue avec `vpn-connection create` lors de l’utilisation des paramètres `--no-wait` ou `--validate`.</span><span class="sxs-lookup"><span data-stu-id="439f1-417">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters.</span></span>
* <span data-ttu-id="439f1-418">Ajouter la prise en charge des passerelles de réseau virtuel actif-actif</span><span class="sxs-lookup"><span data-stu-id="439f1-418">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="439f1-419">Supprimer les valeurs NULL de la sortie des commandes `network vpn-connection list/show`.</span><span class="sxs-lookup"><span data-stu-id="439f1-419">Remove nulls values from output of `network vpn-connection list/show` commands.</span></span>
* <span data-ttu-id="439f1-420">BC : résoudre un bogue dans la sortie de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="439f1-420">BC: Fix bug in the output of `vpn-connection create`</span></span> 
* <span data-ttu-id="439f1-421">Corriger le bogue où l’argument « --key-length » de « vpn-connection create » n’était pas analysé correctement.</span><span class="sxs-lookup"><span data-stu-id="439f1-421">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly.</span></span>
* <span data-ttu-id="439f1-422">Corriger le bogue dans `dns zone import` où les enregistrements n’étaient pas été importés correctement.</span><span class="sxs-lookup"><span data-stu-id="439f1-422">Fix bug in `dns zone import` where records were not imported correctly.</span></span>
* <span data-ttu-id="439f1-423">Corriger le bogue où `traffic-manager endpoint update` ne fonctionnait pas.</span><span class="sxs-lookup"><span data-stu-id="439f1-423">Fix bug where `traffic-manager endpoint update` did not work.</span></span>
* <span data-ttu-id="439f1-424">Ajouter des commandes d’aperçu « network watcher ».</span><span class="sxs-lookup"><span data-stu-id="439f1-424">Add 'network watcher' preview commands.</span></span>

### <a name="profile"></a><span data-ttu-id="439f1-425">Profil</span><span class="sxs-lookup"><span data-stu-id="439f1-425">Profile</span></span>

* <span data-ttu-id="439f1-426">Prendre en charge la connexion lorsqu’il n’y a aucun abonnement trouvé ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="439f1-426">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="439f1-427">Prendre en charge un nom de paramètre court dans le jeu de comptes az --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="439f1-427">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="439f1-428">Redis</span><span class="sxs-lookup"><span data-stu-id="439f1-428">Redis</span></span>

* <span data-ttu-id="439f1-429">Ajout d’une commande de mise à jour qui ajoute également la possibilité de mettre à l’échelle pour le cache redis</span><span class="sxs-lookup"><span data-stu-id="439f1-429">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="439f1-430">Commande « update-settings » déconseillée.</span><span class="sxs-lookup"><span data-stu-id="439f1-430">Deprecates the 'update-settings' command.</span></span>

### <a name="resource"></a><span data-ttu-id="439f1-431">Ressource</span><span class="sxs-lookup"><span data-stu-id="439f1-431">Resource</span></span>

* <span data-ttu-id="439f1-432">Ajouter managedapp et les commandes de définition managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="439f1-432">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="439f1-433">Prendre en charge les commandes « provider operation » ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="439f1-433">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="439f1-434">Prendre en charge la création de ressource générique ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="439f1-434">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="439f1-435">Corriger l’analyse de ressource et la recherche de version d’API.</span><span class="sxs-lookup"><span data-stu-id="439f1-435">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="439f1-436">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="439f1-436">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="439f1-437">Ajouter des documents pour mise à jour du verrou az.</span><span class="sxs-lookup"><span data-stu-id="439f1-437">Add docs for az lock update.</span></span> <span data-ttu-id="439f1-438">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="439f1-438">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="439f1-439">Sortie d’erreur si vous essayez de lister des ressources pour un groupe qui n’existe pas.</span><span class="sxs-lookup"><span data-stu-id="439f1-439">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="439f1-440">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="439f1-440">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="439f1-441">[Compute] Résoudre les problèmes de mise à jour de VMSS et du groupe à haute disponibilité de machines virtuelles.</span><span class="sxs-lookup"><span data-stu-id="439f1-441">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="439f1-442">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="439f1-442">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="439f1-443">Corriger le verrouillage des commandes créer et supprimer si parent-resource-path est None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="439f1-443">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="439f1-444">Rôle</span><span class="sxs-lookup"><span data-stu-id="439f1-444">Role</span></span>

* <span data-ttu-id="439f1-445">create-for-rbac : vérifier que la date de fin du SP ne dépassera pas la date d’expiration du certificat ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="439f1-445">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="439f1-446">RBAC : ajouter la prise en charge complète de « ad group » ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="439f1-446">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="439f1-447">rôle : résoudre les problèmes de mise à jour de définition de rôle ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="439f1-447">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="439f1-448">create-for-rbac : vérifier que le mot de passe fourni par l’utilisateur est accepté</span><span class="sxs-lookup"><span data-stu-id="439f1-448">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="439f1-449">SQL</span><span class="sxs-lookup"><span data-stu-id="439f1-449">SQL</span></span>

* <span data-ttu-id="439f1-450">Commandes az sql server list-usages et az sql db list-usages ajoutées.</span><span class="sxs-lookup"><span data-stu-id="439f1-450">Added az sql server list-usages and az sql db list-usages commands.</span></span>
* <span data-ttu-id="439f1-451">SQL : possibilité de se connecter directement au fournisseur de ressources ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="439f1-451">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="439f1-452">Storage</span><span class="sxs-lookup"><span data-stu-id="439f1-452">Storage</span></span>

* <span data-ttu-id="439f1-453">Définir l’emplacement par défaut sur l’emplacement du groupe de ressources pour `storage account create`.</span><span class="sxs-lookup"><span data-stu-id="439f1-453">Default location to resource group location for `storage account create`.</span></span>
* <span data-ttu-id="439f1-454">Ajouter la prise en charge de la copie incrémentielle d’objet blob</span><span class="sxs-lookup"><span data-stu-id="439f1-454">Add support for incremental blob copy</span></span>
* <span data-ttu-id="439f1-455">Ajouter la prise en charge du chargement d’objet blob de blocs volumineux</span><span class="sxs-lookup"><span data-stu-id="439f1-455">Add support for large block blob upload</span></span>
* <span data-ttu-id="439f1-456">Modifier la taille de bloc à 100 Mo lorsque le fichier à charger est supérieur à 200 Go</span><span class="sxs-lookup"><span data-stu-id="439f1-456">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="439f1-457">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="439f1-457">VM</span></span>

* <span data-ttu-id="439f1-458">avail-set : rendre le compte de domaine UD&FD facultatif</span><span class="sxs-lookup"><span data-stu-id="439f1-458">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="439f1-459">remarque : commandes de machine virtuelle dans clouds souverains Veuillez éviter les fonctionnalités liées au disque managé, notamment :</span><span class="sxs-lookup"><span data-stu-id="439f1-459">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="439f1-460">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="439f1-460">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="439f1-461">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="439f1-461">az vm/vmss disk</span></span>
  3. <span data-ttu-id="439f1-462">Dans « az vm/vmss create », utiliser « —use-unmanaged-disk » pour éviter le disque managé Les autres commandes devraient fonctionner</span><span class="sxs-lookup"><span data-stu-id="439f1-462">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="439f1-463">vm/vmss : améliorer le texte d’avertissement lors de la génération de paires de clés ssh</span><span class="sxs-lookup"><span data-stu-id="439f1-463">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="439f1-464">vm/vmss : prendre en charge la création à partir d’une image de la Place de marché qui requiert des informations sur le plan ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="439f1-464">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="439f1-465">3 avril 2017</span><span class="sxs-lookup"><span data-stu-id="439f1-465">April 3, 2017</span></span>

<span data-ttu-id="439f1-466">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="439f1-466">Version 2.0.2</span></span>

<span data-ttu-id="439f1-467">Nous avons publié les composants ACR, Batch, KeyVault et SQL dans cette version.</span><span class="sxs-lookup"><span data-stu-id="439f1-467">We released the ACR, Batch, KeyVault, and SQL components in this release.</span></span>

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

### <a name="core"></a><span data-ttu-id="439f1-468">Principal</span><span class="sxs-lookup"><span data-stu-id="439f1-468">Core</span></span>

* <span data-ttu-id="439f1-469">Ajout des modules acr, lab, monitor et find à la liste par défaut.</span><span class="sxs-lookup"><span data-stu-id="439f1-469">Add acr, lab, monitor, and find modules to default list.</span></span>
* <span data-ttu-id="439f1-470">Connexion : ignorer les locataires erronés ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="439f1-470">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="439f1-471">login : définition de l’abonnement par défaut à la valeur « un » avec l’état « Activé » ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="439f1-471">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="439f1-472">Ajout de la prise en charge des commandes wait et de --no-wait à davantage de commandes ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="439f1-472">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="439f1-473">core : prise en charge de la connexion à l’aide du principal du service avec un certificat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="439f1-473">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="439f1-474">Ajout d’une invite pour les paramètres de modèle manquants.</span><span class="sxs-lookup"><span data-stu-id="439f1-474">Add prompting for missing template parameters.</span></span> <span data-ttu-id="439f1-475">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="439f1-475">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="439f1-476">Prise en charge de la définition de valeurs par défaut pour des arguments courants tels que le groupe de ressources par défaut, le site web par défaut et la machine virtuelle par défaut</span><span class="sxs-lookup"><span data-stu-id="439f1-476">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="439f1-477">Prise en charge de la connexion à un locataire spécifique</span><span class="sxs-lookup"><span data-stu-id="439f1-477">Support login to specific tenant</span></span>
 
### <a name="acs"></a><span data-ttu-id="439f1-478">ACS</span><span class="sxs-lookup"><span data-stu-id="439f1-478">ACS</span></span>

* <span data-ttu-id="439f1-479">[ACS] Ajout de la prise en charge de la configuration d’un cluster ACS par défaut ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="439f1-479">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="439f1-480">Ajout de la prise en charge de l’invite de mot de passe de clé ssh.</span><span class="sxs-lookup"><span data-stu-id="439f1-480">Add support for ssh key password prompting.</span></span> <span data-ttu-id="439f1-481">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="439f1-481">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="439f1-482">Ajout de la prise en charge des clusters Windows.</span><span class="sxs-lookup"><span data-stu-id="439f1-482">Add support for windows clusters.</span></span> <span data-ttu-id="439f1-483">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="439f1-483">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="439f1-484">Basculement du rôle Propriétaire au rôle Contributeur.</span><span class="sxs-lookup"><span data-stu-id="439f1-484">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="439f1-485">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="439f1-485">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>
 
### <a name="appservice"></a><span data-ttu-id="439f1-486">AppService</span><span class="sxs-lookup"><span data-stu-id="439f1-486">AppService</span></span>

* <span data-ttu-id="439f1-487">appservice : prise en charge de l’obtention de l’adresse IP externe utilisée pour les enregistrements A DNS ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="439f1-487">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="439f1-488">appservice : prise en charge de la liaison des certificats avec caractères génériques ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="439f1-488">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="439f1-489">appservice : prise en charge des profils de publication de liste ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="439f1-489">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="439f1-490">AppService : déclenchement de la synchronisation de contrôle de code source après la configuration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="439f1-490">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>
 
### <a name="datalake"></a><span data-ttu-id="439f1-491">DataLake</span><span class="sxs-lookup"><span data-stu-id="439f1-491">DataLake</span></span>

* <span data-ttu-id="439f1-492">Version initiale du module Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="439f1-492">Initial release of Data Lake Analytics module.</span></span>
* <span data-ttu-id="439f1-493">Version initiale du module Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="439f1-493">Initial release of Data Lake Store module.</span></span>
 
### <a name="docuemntdb"></a><span data-ttu-id="439f1-494">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="439f1-494">DocuemntDB</span></span>

* <span data-ttu-id="439f1-495">DocumentDB : ajout de la prise en charge de l’énumération des chaînes de connexion ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="439f1-495">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="439f1-496">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="439f1-496">VM</span></span>

* <span data-ttu-id="439f1-497">[Compute] Ajout de la prise en charge d’AppGateway à la création de groupe de machines virtuelles identiques ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="439f1-497">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="439f1-498">[VM/VMSS] Amélioration de la prise en charge de la mise en cache de disque ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="439f1-498">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="439f1-499">VM/VMSS : intégration de la logique de validation des informations d’identification utilisée par le portail ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="439f1-499">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="439f1-500">Ajout de la prise en charge des commandes wait et de --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="439f1-500">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="439f1-501">Groupe de machines virtuelles identiques : prise en charge de * pour énumérer les vues d’instance parmi les machines virtuelles ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="439f1-501">Virtual machine scale set: support * to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="439f1-502">Ajout de --secrets pour les machines virtuelles et les groupes de machines virtuelles identiques ([#2212} (https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="439f1-502">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="439f1-503">Autorisation de la création de machines virtuelles avec un disque dur virtuel spécialisé ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="439f1-503">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="439f1-504">27 février 2017</span><span class="sxs-lookup"><span data-stu-id="439f1-504">February 27, 2017</span></span>

<span data-ttu-id="439f1-505">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="439f1-505">Version 2.0.0</span></span>

<span data-ttu-id="439f1-506">Cette version d’Azure CLI 2.0 est la première version en « Disponibilité générale ».</span><span class="sxs-lookup"><span data-stu-id="439f1-506">This release of Azure CLI 2.0 is the first "Generally Available" release.</span></span>
<span data-ttu-id="439f1-507">La disponibilité générale s’applique à ces modules de commande :</span><span class="sxs-lookup"><span data-stu-id="439f1-507">General availability applies to these command modules:</span></span>
- <span data-ttu-id="439f1-508">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="439f1-508">Container Service (acs)</span></span>
- <span data-ttu-id="439f1-509">Compute (notamment Resource Manager, machine virtuelle, groupes de machines virtuelles identiques, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="439f1-509">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="439f1-510">Réseau</span><span class="sxs-lookup"><span data-stu-id="439f1-510">Networking</span></span>
- <span data-ttu-id="439f1-511">Stockage</span><span class="sxs-lookup"><span data-stu-id="439f1-511">Storage</span></span>

<span data-ttu-id="439f1-512">Ces modules de commande peuvent être utilisés en production et sont pris en charge par le contrat SLA Microsoft standard.</span><span class="sxs-lookup"><span data-stu-id="439f1-512">These command modules can be used in production and are supported by standard Microsoft SLA.</span></span>
<span data-ttu-id="439f1-513">Vous pouvez ouvrir des incidents directement auprès du support technique de Microsoft ou dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/).</span><span class="sxs-lookup"><span data-stu-id="439f1-513">You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/).</span></span>
<span data-ttu-id="439f1-514">Vous pouvez poser des questions sur [StackOverflow à l’aide du mot clé azure-cli](http://stackoverflow.com/questions/tagged/azure-cli) ou contacter l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Vous pouvez fournir des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="439f1-514">You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). You can provide feedback from the command line with the `az feedback` command.</span></span>

<span data-ttu-id="439f1-515">Les commandes de ces modules sont stables et il n’est pas prévu que la syntaxe change dans les mises à jour ultérieures de cette version d’Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="439f1-515">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI.</span></span>

<span data-ttu-id="439f1-516">Pour vérifier la version de l’interface CLI, utilisez `az --version`.</span><span class="sxs-lookup"><span data-stu-id="439f1-516">To verify the version of the CLI, use `az --version`.</span></span>
<span data-ttu-id="439f1-517">La sortie indique la version de l’interface CLI proprement dite (2.0.0 dans cette version), les différents modules de commande et les versions de Python et de GCC que vous utilisez.</span><span class="sxs-lookup"><span data-stu-id="439f1-517">The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using.</span></span>

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
> <span data-ttu-id="439f1-518">Certains des modules de commande ont un suffixe « b*n* » ou « rc*n* ».</span><span class="sxs-lookup"><span data-stu-id="439f1-518">Some of the command modules have a "b*n*" or "rc*n*" postfix.</span></span>
> <span data-ttu-id="439f1-519">Ces modules de commande sont toujours en préversion et seront à la disposition générale ultérieurement.</span><span class="sxs-lookup"><span data-stu-id="439f1-519">These command modules are still in preview and will become generally available in the future.</span></span>

<span data-ttu-id="439f1-520">Nous avons également des versions d’évaluation nocturnes de l’interface CLI.</span><span class="sxs-lookup"><span data-stu-id="439f1-520">We also have nightly preview builds of the CLI.</span></span>
<span data-ttu-id="439f1-521">Pour plus d’informations, consultez ces instructions sur [l’obtention des builds nocturnes](https://github.com/Azure/azure-cli#nightly-builds) et ces instructions sur [la contribution au code et la configuration d’un environnement de développement](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="439f1-521">For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup).</span></span>

<span data-ttu-id="439f1-522">Vous pouvez signaler des problèmes liés aux versions d’évaluation nocturnes comme suit :</span><span class="sxs-lookup"><span data-stu-id="439f1-522">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="439f1-523">Signalez des problèmes dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="439f1-523">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="439f1-524">Contactez l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="439f1-524">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span></span>
- <span data-ttu-id="439f1-525">Fournissez des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="439f1-525">Provide feedback from the command line with the `az feedback` command.</span></span>

