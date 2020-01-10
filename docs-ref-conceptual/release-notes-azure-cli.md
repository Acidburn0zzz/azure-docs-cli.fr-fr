---
title: Notes de publication d’Azure CLI
description: En savoir plus sur les dernières mises à jour d’Azure CLI
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 01/07/2020
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 9fc54add3bfb2a75d1912c47f0a2571d9d065ec0
ms.sourcegitcommit: 5646008e7a521dd9a8a627418f57bd92ee180352
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/07/2020
ms.locfileid: "75694272"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="de833-103">Notes de publication d’Azure CLI</span><span class="sxs-lookup"><span data-stu-id="de833-103">Azure CLI release notes</span></span>

## <a name="january-07-2020"></a><span data-ttu-id="de833-104">7 janvier 2020</span><span class="sxs-lookup"><span data-stu-id="de833-104">January 07, 2020</span></span>

<span data-ttu-id="de833-105">Version 2.0.79</span><span class="sxs-lookup"><span data-stu-id="de833-105">Version 2.0.79</span></span>

### <a name="acr"></a><span data-ttu-id="de833-106">ACR</span><span class="sxs-lookup"><span data-stu-id="de833-106">ACR</span></span>

* <span data-ttu-id="de833-107">[CHANGEMENT CASSANT] Suppression du paramètre « --os » pour « acr build », « acr task create/update », « acr run » et « acr pack ».</span><span class="sxs-lookup"><span data-stu-id="de833-107">[BREAKING CHANGE] Remove '--os' parameter for 'acr build', 'acr task create/update', 'acr run', and 'acr pack'.</span></span> <span data-ttu-id="de833-108">Utilisez « --platform » à la place.</span><span class="sxs-lookup"><span data-stu-id="de833-108">Use '--platform' instead.</span></span>

### <a name="appconfig"></a><span data-ttu-id="de833-109">AppConfig</span><span class="sxs-lookup"><span data-stu-id="de833-109">AppConfig</span></span>

* <span data-ttu-id="de833-110">Ajout de la prise en charge de l’importation/exportation des indicateurs de fonctionnalité</span><span class="sxs-lookup"><span data-stu-id="de833-110">Add support for importing/exporting feature flags</span></span>
* <span data-ttu-id="de833-111">Ajout de la nouvelle commande « az appconfig kv set-keyvault » pour la création d’une référence KeyVault</span><span class="sxs-lookup"><span data-stu-id="de833-111">Add new command 'az appconfig kv set-keyvault' for creating keyvault reference</span></span>
* <span data-ttu-id="de833-112">Prise en charge de différentes conventions de nommage lors de l’exportation d’indicateurs de fonctionnalité dans un fichier</span><span class="sxs-lookup"><span data-stu-id="de833-112">Support various naming conventions when exporting feature flags to file</span></span>

### <a name="appservice"></a><span data-ttu-id="de833-113">AppService</span><span class="sxs-lookup"><span data-stu-id="de833-113">AppService</span></span>

* <span data-ttu-id="de833-114">Résolution du problème #7154 : Mise à jour de la documentation pour la commande <> afin d’utiliser des accents graves (backtick) plutôt que des guillemets simples</span><span class="sxs-lookup"><span data-stu-id="de833-114">Fix issue #7154: Updating documentation for command <> to use back ticks instead of single quotes</span></span>
* <span data-ttu-id="de833-115">Résolution du problème #11287 : webapp up : Faire en sorte que l’application créée à l’aide de « up » ait « SSL activé » par défaut</span><span class="sxs-lookup"><span data-stu-id="de833-115">Fix issue #11287: webapp up: By default make the app created using up 'should be 'SSL enabled'</span></span>
* <span data-ttu-id="de833-116">Résolution du problème #11592 : Ajout de la commande az webapp up flag pour les sites statiques HTML</span><span class="sxs-lookup"><span data-stu-id="de833-116">Fix issue #11592: Add az webapp up flag for html static sites</span></span>

### <a name="arm"></a><span data-ttu-id="de833-117">ARM</span><span class="sxs-lookup"><span data-stu-id="de833-117">ARM</span></span>

* <span data-ttu-id="de833-118">Correction de `az resource tag` : Impossible de mettre à jour les balises du coffre Recovery Services</span><span class="sxs-lookup"><span data-stu-id="de833-118">Fix `az resource tag`: Recovery Services Vault tags cannot be updated</span></span>

### <a name="backup"></a><span data-ttu-id="de833-119">Backup</span><span class="sxs-lookup"><span data-stu-id="de833-119">Backup</span></span>

* <span data-ttu-id="de833-120">Ajout de la nouvelle commande « backup protection undelete » pour activer la fonctionnalité de suppression réversible pour la charge de travail IaasVM</span><span class="sxs-lookup"><span data-stu-id="de833-120">Added new command 'backup protection undelete' to enable soft-delete feature for IaasVM workload</span></span>
* <span data-ttu-id="de833-121">Ajout du nouveau paramètre « --soft-delete-feature-state » pour définir la commande backup-properties</span><span class="sxs-lookup"><span data-stu-id="de833-121">Added new parameter '--soft-delete-feature-state' to set backup-properties command</span></span>
* <span data-ttu-id="de833-122">Ajout de la prise en charge de l’exclusion de disque pour la charge de travail IaasVM</span><span class="sxs-lookup"><span data-stu-id="de833-122">Added disk exclusion support for IaasVM workload</span></span>

### <a name="compute"></a><span data-ttu-id="de833-123">Calcul</span><span class="sxs-lookup"><span data-stu-id="de833-123">Compute</span></span>

* <span data-ttu-id="de833-124">Résolution de l’échec de `vm create` dans le profil Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="de833-124">Fix `vm create` failure in Azure Stack profile.</span></span>
* <span data-ttu-id="de833-125">vm monitor metrics tail/list-definitions : prise en charge des définitions de métriques et de listes pour une machine virtuelle.</span><span class="sxs-lookup"><span data-stu-id="de833-125">vm monitor metrics tail/list-definitions: support query metric and list definitions for a vm.</span></span>
* <span data-ttu-id="de833-126">Ajout d’une nouvelle action de réapplication de commande pour az vm</span><span class="sxs-lookup"><span data-stu-id="de833-126">Add new reapply command action for az vm</span></span>

### <a name="misc"></a><span data-ttu-id="de833-127">Divers</span><span class="sxs-lookup"><span data-stu-id="de833-127">Misc.</span></span>

* <span data-ttu-id="de833-128">Ajout de la commande d’aperçu `az version show` pour afficher les versions des modules et extensions Azure CLI au format JSON par défaut ou au format configuré par --output</span><span class="sxs-lookup"><span data-stu-id="de833-128">Add preview command `az version show` to show the versions of Azure CLI modules and extensions in JSON format by default or format configured by --output</span></span>

### <a name="event-hubs"></a><span data-ttu-id="de833-129">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="de833-129">Event Hubs</span></span>

* <span data-ttu-id="de833-130">[CHANGEMENT CASSANT] Suppression de l’option d’état « ReceiveDisabled » des commandes « az eventhubs eventhub update » et « az eventhubs eventhub create ».</span><span class="sxs-lookup"><span data-stu-id="de833-130">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az eventhubs eventhub update' and 'az eventhubs eventhub create'.</span></span> <span data-ttu-id="de833-131">Cette option n’est pas valide pour les entités Event Hub.</span><span class="sxs-lookup"><span data-stu-id="de833-131">This option is not valid for Event Hub entities.</span></span>

### <a name="service-bus"></a><span data-ttu-id="de833-132">Service Bus</span><span class="sxs-lookup"><span data-stu-id="de833-132">Service Bus</span></span>

* <span data-ttu-id="de833-133">[CHANGEMENT CASSANT] Suppression de l’option d’état « ReceiveDisabled » des commandes « az servicebus topic create », « az servicebus topic update », « az servicebus queue create » et « az servicebus queue update ».</span><span class="sxs-lookup"><span data-stu-id="de833-133">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az servicebus topic create', 'az servicebus topic update', 'az servicebus queue create', and 'az servicebus queue update'.</span></span> <span data-ttu-id="de833-134">Cette option n’est pas valide pour les rubriques et files d’attente Service Bus.</span><span class="sxs-lookup"><span data-stu-id="de833-134">This option is not valid for Service Bus topics and queues.</span></span>

### <a name="rbac"></a><span data-ttu-id="de833-135">RBAC</span><span class="sxs-lookup"><span data-stu-id="de833-135">RBAC</span></span>

* <span data-ttu-id="de833-136">Correctif 11712 : `az ad app/sp show` ne retourne pas le code de sortie 3 quand le principal d’application ou de service n’existe pas</span><span class="sxs-lookup"><span data-stu-id="de833-136">Fix #11712: `az ad app/sp show` does not return exit code 3 when the application or service principal does not exist</span></span>

### <a name="storage"></a><span data-ttu-id="de833-137">Stockage</span><span class="sxs-lookup"><span data-stu-id="de833-137">Storage</span></span>

* <span data-ttu-id="de833-138">`az storage account create`: Suppression de l’indicateur d’aperçu pour le paramètre --enable-hierarchical-namespace</span><span class="sxs-lookup"><span data-stu-id="de833-138">`az storage account create`: Remove preview flag for --enable-hierarchical-namespace parameter</span></span>
* <span data-ttu-id="de833-139">Mise à jour de la version d’azure-mgmt-storage vers la version 7.0.0 pour utiliser la version d’API du 01/06/2019</span><span class="sxs-lookup"><span data-stu-id="de833-139">Update azure-mgmt-storage version to 7.0.0 to use api version 2019-06-01</span></span>
* <span data-ttu-id="de833-140">Ajout des nouveaux paramètres `--enable-delete-retention` et `--delete-retention-days` afin de prendre en charge la gestion de la stratégie de conservation de suppression pour les propriétés blob-service du compte de stockage.</span><span class="sxs-lookup"><span data-stu-id="de833-140">Add new parameters `--enable-delete-retention` and `--delete-retention-days` to support managing delete retention policy for storage account blob-service-properties.</span></span>

## <a name="december-17-2019"></a><span data-ttu-id="de833-141">17 décembre 2019</span><span class="sxs-lookup"><span data-stu-id="de833-141">December 17, 2019</span></span>

<span data-ttu-id="de833-142">2.0.78</span><span class="sxs-lookup"><span data-stu-id="de833-142">2.0.78</span></span>

### <a name="acr"></a><span data-ttu-id="de833-143">ACR</span><span class="sxs-lookup"><span data-stu-id="de833-143">ACR</span></span>

* <span data-ttu-id="de833-144">Ajout de la prise en charge du contexte local dans acr task run</span><span class="sxs-lookup"><span data-stu-id="de833-144">Added support Local context in acr task run</span></span>

### <a name="acs"></a><span data-ttu-id="de833-145">ACS</span><span class="sxs-lookup"><span data-stu-id="de833-145">ACS</span></span>

* <span data-ttu-id="de833-146">[CHANGEMENT CASSANT]az openshift create : renommage de `--workspace-resource-id` en `--workspace-id`.</span><span class="sxs-lookup"><span data-stu-id="de833-146">[BREAKING CHANGE]az openshift create: rename `--workspace-resource-id` to `--workspace-id`.</span></span>

### <a name="ams"></a><span data-ttu-id="de833-147">AMS</span><span class="sxs-lookup"><span data-stu-id="de833-147">AMS</span></span>

* <span data-ttu-id="de833-148">Mise à jour des commandes show pour retourner 3 quand la ressource est introuvable</span><span class="sxs-lookup"><span data-stu-id="de833-148">Updated show commands to return 3 when resource not found</span></span>

### <a name="appconfig"></a><span data-ttu-id="de833-149">AppConfig</span><span class="sxs-lookup"><span data-stu-id="de833-149">AppConfig</span></span>

* <span data-ttu-id="de833-150">Correction d’un bogue lié à l’ajout de la version d’API à l’URL de demande.</span><span class="sxs-lookup"><span data-stu-id="de833-150">Fixed bug when appending api-version to request url.</span></span> <span data-ttu-id="de833-151">La solution existante ne fonctionne pas avec la pagination.</span><span class="sxs-lookup"><span data-stu-id="de833-151">The existing solution doesn't work with pagination.</span></span>
* <span data-ttu-id="de833-152">Ajout de la prise en charge de l’affichage des langues en plus de l’anglais comme notre Unicode de support du service back-end pour la globalisation.</span><span class="sxs-lookup"><span data-stu-id="de833-152">Added support for showing languages besides English as our backend service support unicode for globalization.</span></span>

### <a name="appservice"></a><span data-ttu-id="de833-153">AppService</span><span class="sxs-lookup"><span data-stu-id="de833-153">AppService</span></span>

* <span data-ttu-id="de833-154">Résolution du problème #11217 : webapp : az webapp config ssl upload doit prendre en charge le paramètre d’emplacement (slot)</span><span class="sxs-lookup"><span data-stu-id="de833-154">Fixed issue #11217: webapp: az webapp config ssl upload should support slot parameter</span></span>
* <span data-ttu-id="de833-155">Résolution du problème #10965 : Erreur : Le nom n'est pas vide.</span><span class="sxs-lookup"><span data-stu-id="de833-155">Fixed issue #10965: Error: Name cannot be empty.</span></span> <span data-ttu-id="de833-156">Autoriser la suppression par adresse IP (ip_address) et sous-réseau (subnet)</span><span class="sxs-lookup"><span data-stu-id="de833-156">Allow remove by ip_address and subnet</span></span>
* <span data-ttu-id="de833-157">Ajout de la prise en charge de l’importation de certificats à partir du coffre de clés `az webapp config ssl import`</span><span class="sxs-lookup"><span data-stu-id="de833-157">Added support for importing certificates from Key Vault `az webapp config ssl import`</span></span>

### <a name="arm"></a><span data-ttu-id="de833-158">ARM</span><span class="sxs-lookup"><span data-stu-id="de833-158">ARM</span></span>

* <span data-ttu-id="de833-159">Mise à jour du package azure-mgmt-resource pour utiliser la version 6.0.0</span><span class="sxs-lookup"><span data-stu-id="de833-159">Updated azure-mgmt-resource package to use 6.0.0</span></span>
* <span data-ttu-id="de833-160">Prise en charge interlocataire pour la commande `az group deployment create` en ajoutant le nouveau paramètre `--aux-subs`</span><span class="sxs-lookup"><span data-stu-id="de833-160">Cross Tenant Support for `az group deployment create` command by adding new parameter `--aux-subs`</span></span>
* <span data-ttu-id="de833-161">Ajout du nouveau paramètre `--metadata` afin de prendre en charge l’ajout d’informations de métadonnées pour les définitions d’ensemble de stratégie.</span><span class="sxs-lookup"><span data-stu-id="de833-161">Added new parameter `--metadata` to support adding metadata information for policy set definitions.</span></span>

### <a name="backup"></a><span data-ttu-id="de833-162">Backup</span><span class="sxs-lookup"><span data-stu-id="de833-162">Backup</span></span>

* <span data-ttu-id="de833-163">Ajout de la prise en charge de la sauvegarde pour la charge de travail SQL et SAP Hana.</span><span class="sxs-lookup"><span data-stu-id="de833-163">Added Backup support for SQL and SAP Hana workload.</span></span>

### <a name="botservice"></a><span data-ttu-id="de833-164">BotService</span><span class="sxs-lookup"><span data-stu-id="de833-164">BotService</span></span>

* <span data-ttu-id="de833-165">[Changement cassant] Suppression de l’indicateur « --version » de la commande d’aperçu « az bot create ».</span><span class="sxs-lookup"><span data-stu-id="de833-165">[Breaking change] Remove '--version' flag from preview command 'az bot create'.</span></span> <span data-ttu-id="de833-166">Seuls les bots du SDK v4 sont pris en charge.</span><span class="sxs-lookup"><span data-stu-id="de833-166">Only v4 SDK bots are supported.</span></span>
* <span data-ttu-id="de833-167">Ajout de la vérification de la disponibilité du nom pour « az bot create ».</span><span class="sxs-lookup"><span data-stu-id="de833-167">Added name availability check for 'az bot create'.</span></span>
* <span data-ttu-id="de833-168">Ajout de la prise en charge de la mise à jour de l’URL d’icône pour un bot par le biais de « az bot update ».</span><span class="sxs-lookup"><span data-stu-id="de833-168">Added support for updating the icon URL for a bot via 'az bot update'.</span></span>
* <span data-ttu-id="de833-169">Ajout de la prise en charge de la mise à jour d’un canal Direct Line par le biais de « az bot directline update ».</span><span class="sxs-lookup"><span data-stu-id="de833-169">Added support for updating a Direct Line channel via 'az bot directline update'.</span></span>
* <span data-ttu-id="de833-170">Ajout de la prise en charge de l’indicateur « --enable-enhanced-auth » à « az bot directline create ».</span><span class="sxs-lookup"><span data-stu-id="de833-170">Added '--enable-enhanced-auth' flag support to 'az bot directline create'.</span></span>
* <span data-ttu-id="de833-171">Les groupes de commandes suivants sont en disponibilité générale et non en préversion : « az bot authsetting ».</span><span class="sxs-lookup"><span data-stu-id="de833-171">The following command groups are GA and not in preview: 'az bot authsetting'.</span></span>
* <span data-ttu-id="de833-172">Les commandes suivantes dans « az bot » sont en disponibilité générale et non en préversion : « create », « prepare-deploy », « show », « delete », « update ».</span><span class="sxs-lookup"><span data-stu-id="de833-172">The following commands in 'az bot' are GA and not in preview: 'create', 'prepare-deploy', 'show', 'delete', 'update'.</span></span>
* <span data-ttu-id="de833-173">Résolution du problème lié au fait que « az bot prepare-deploy » convertit la valeur « --proj-file-path » en minuscules (par exemple, « Test.csproj » en « test.csproj »).</span><span class="sxs-lookup"><span data-stu-id="de833-173">Fixed 'az bot prepare-deploy' changing '--proj-file-path' value to lower case (e.g. "Test.csproj" to "test.csproj").</span></span>

### <a name="compute"></a><span data-ttu-id="de833-174">Calcul</span><span class="sxs-lookup"><span data-stu-id="de833-174">Compute</span></span>

* <span data-ttu-id="de833-175">vmss create/update : Ajout de --scale-in-policy, qui détermine quelles machines virtuelles sont choisies pour la suppression quand un groupe de machines virtuelles identiques (VMSS) fait l’objet d’un scale-in.</span><span class="sxs-lookup"><span data-stu-id="de833-175">vmss create/update: Added --scale-in-policy, which decides which virtual machines are chosen for removal when a VMSS is scaled-in.</span></span>
* <span data-ttu-id="de833-176">vm/vmss update : Ajout de --priority.</span><span class="sxs-lookup"><span data-stu-id="de833-176">vm/vmss update: Added --priority.</span></span>
* <span data-ttu-id="de833-177">vm/vmss update : Ajout de --max-price.</span><span class="sxs-lookup"><span data-stu-id="de833-177">vm/vmss update: Added --max-price.</span></span>
* <span data-ttu-id="de833-178">Ajout du groupe de commandes disk-encryption-set (create, show, update, delete, list).</span><span class="sxs-lookup"><span data-stu-id="de833-178">Added disk-encryption-set command group (create, show, update, delete, list).</span></span>
* <span data-ttu-id="de833-179">disk create : Ajout de --encryption-type et de --disk-encryption-set.</span><span class="sxs-lookup"><span data-stu-id="de833-179">disk create: Added --encryption-type and --disk-encryption-set.</span></span>
* <span data-ttu-id="de833-180">vm/vmss create : Ajout de --os-disk-encryption-set et de --data-disk-encryption-sets.</span><span class="sxs-lookup"><span data-stu-id="de833-180">vm/vmss create: Added --os-disk-encryption-set and --data-disk-encryption-sets.</span></span>

### <a name="core"></a><span data-ttu-id="de833-181">Core</span><span class="sxs-lookup"><span data-stu-id="de833-181">Core</span></span>

* <span data-ttu-id="de833-182">Suppression de la prise en charge pour Python 3.4</span><span class="sxs-lookup"><span data-stu-id="de833-182">Removed support for Python 3.4</span></span>
* <span data-ttu-id="de833-183">Intégrer l’enquête HaTS à plusieurs commandes</span><span class="sxs-lookup"><span data-stu-id="de833-183">Plug in HaTS survey in multiple commands</span></span>

### <a name="dls"></a><span data-ttu-id="de833-184">DLS</span><span class="sxs-lookup"><span data-stu-id="de833-184">DLS</span></span>

* <span data-ttu-id="de833-185">Mise à jour de la version du SDK ADLS (0.0.48).</span><span class="sxs-lookup"><span data-stu-id="de833-185">Updated ADLS sdk version (0.0.48).</span></span>

### <a name="install"></a><span data-ttu-id="de833-186">Installer</span><span class="sxs-lookup"><span data-stu-id="de833-186">Install</span></span>

* <span data-ttu-id="de833-187">Prise en charge du script d’installation pour Python 3.8</span><span class="sxs-lookup"><span data-stu-id="de833-187">Install script support python 3.8</span></span>

### <a name="iot"></a><span data-ttu-id="de833-188">IOT</span><span class="sxs-lookup"><span data-stu-id="de833-188">IOT</span></span>

* <span data-ttu-id="de833-189">[CHANGEMENT CASSANT] Suppression du paramètre --failover-region du basculement manuel.</span><span class="sxs-lookup"><span data-stu-id="de833-189">[BREAKING CHANGE] Removed --failover-region parameter from manual-failover.</span></span> <span data-ttu-id="de833-190">À présent, le basculement s’effectuera vers la région secondaire géographiquement associée.</span><span class="sxs-lookup"><span data-stu-id="de833-190">Now it will failover to assigned geo-paired secondary region.</span></span>

### <a name="key-vault"></a><span data-ttu-id="de833-191">Key Vault</span><span class="sxs-lookup"><span data-stu-id="de833-191">Key Vault</span></span>

* <span data-ttu-id="de833-192">Résolution du problème #8095 : `az keyvault storage remove` : amélioration du message d’aide</span><span class="sxs-lookup"><span data-stu-id="de833-192">Fixed #8095: `az keyvault storage remove`: improve the help message</span></span>
* <span data-ttu-id="de833-193">Résolution du problème #8921 : `az keyvault key/secret/certificate list/list-deleted/list-versions` : correction du bogue de validation sur le paramètre `--maxresults`</span><span class="sxs-lookup"><span data-stu-id="de833-193">Fixed #8921: `az keyvault key/secret/certificate list/list-deleted/list-versions`: fix the validation bug on parameter `--maxresults`</span></span>
* <span data-ttu-id="de833-194">Résolution du problème #10512 : `az keyvault set-policy` : amélioration du message d’erreur quand aucune des valeurs `--object-id`, `--spn` ou `--upn` n’est spécifiée</span><span class="sxs-lookup"><span data-stu-id="de833-194">Fixed #10512: `az keyvault set-policy`: improve the error message when none of `--object-id`, `--spn` or `--upn` is specified</span></span>
* <span data-ttu-id="de833-195">Résolution du problème #10846 : `az keyvault secret show-deleted` : quand la valeur `--id` est spécifiée, `--name/-n` n’est pas nécessaire</span><span class="sxs-lookup"><span data-stu-id="de833-195">Fixed #10846: `az keyvault secret show-deleted`: when `--id` is specified, `--name/-n` is not required</span></span>
* <span data-ttu-id="de833-196">Résolution du problème #11084 : `az keyvault secret download` : amélioration du message d’aide du paramètre `--encoding`</span><span class="sxs-lookup"><span data-stu-id="de833-196">Fixed #11084: `az keyvault secret download`: improve the help message of parameter `--encoding`</span></span>

### <a name="network"></a><span data-ttu-id="de833-197">Réseau</span><span class="sxs-lookup"><span data-stu-id="de833-197">Network</span></span>

* <span data-ttu-id="de833-198">az network application-gateway probe : Ajout de la prise en charge de l’option --port afin de spécifier un port pour la détection des serveurs back-end lors d’une opération de création et de mise à jour</span><span class="sxs-lookup"><span data-stu-id="de833-198">az network application-gateway probe: Added support --port option to specify a port for probing backend servers when create and update</span></span>
* <span data-ttu-id="de833-199">az network application-gateway url-path-map create/update : correction du bogue pour `--waf-policy`</span><span class="sxs-lookup"><span data-stu-id="de833-199">az network application-gateway url-path-map create/update: bug fix for `--waf-policy`</span></span>
* <span data-ttu-id="de833-200">az network application-gateway : Ajout de la prise en charge de `--rewrite-rule-set`</span><span class="sxs-lookup"><span data-stu-id="de833-200">az network application-gateway: Added support `--rewrite-rule-set`</span></span>
* <span data-ttu-id="de833-201">az network list-service-aliases : Ajout de la prise en charge du listage des alias de service qui peuvent être utilisés pour les stratégies de point de terminaison de service</span><span class="sxs-lookup"><span data-stu-id="de833-201">az network list-service-aliases: Added support list service aliases which can be used for Service Endpoint Policies</span></span>
* <span data-ttu-id="de833-202">az network dns zone import : Ajout de la prise en charge de .@ dans le nom des enregistrements</span><span class="sxs-lookup"><span data-stu-id="de833-202">az network dns zone import: Added support .@ in record name</span></span>

### <a name="packaging"></a><span data-ttu-id="de833-203">Packaging</span><span class="sxs-lookup"><span data-stu-id="de833-203">Packaging</span></span>

* <span data-ttu-id="de833-204">Rajout de builds edge pour pip install</span><span class="sxs-lookup"><span data-stu-id="de833-204">Added back edge builds for pip install</span></span>
* <span data-ttu-id="de833-205">Ajout du package Ubuntu eoan</span><span class="sxs-lookup"><span data-stu-id="de833-205">Added Ubuntu eoan package</span></span>

### <a name="policy"></a><span data-ttu-id="de833-206">Stratégie</span><span class="sxs-lookup"><span data-stu-id="de833-206">Policy</span></span>

* <span data-ttu-id="de833-207">Ajout de la prise en charge de l’API des stratégies version 2019-09-01.</span><span class="sxs-lookup"><span data-stu-id="de833-207">Added support for Policy API version 2019-09-01.</span></span>
* <span data-ttu-id="de833-208">az policy set-definition : Ajout de la prise en charge du regroupement dans les définitions d’ensemble de stratégies avec le paramètre `--definition-groups`</span><span class="sxs-lookup"><span data-stu-id="de833-208">az policy set-definition: Added support grouping within policy set definitions with `--definition-groups` parameter</span></span>

### <a name="redis"></a><span data-ttu-id="de833-209">Redis</span><span class="sxs-lookup"><span data-stu-id="de833-209">Redis</span></span>

* <span data-ttu-id="de833-210">Ajout du paramètre d’aperçu `--replicas-per-master` à la commande `az redis create`</span><span class="sxs-lookup"><span data-stu-id="de833-210">Added preview param `--replicas-per-master` to `az redis create` command</span></span>
* <span data-ttu-id="de833-211">Mise à jour d’azure-mgmt-redis version 6.0.0 vers la version 7.0.0 RC1</span><span class="sxs-lookup"><span data-stu-id="de833-211">Updated azure-mgmt-redis from 6.0.0 to 7.0.0rc1</span></span>

### <a name="servicefabric"></a><span data-ttu-id="de833-212">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="de833-212">ServiceFabric</span></span>

* <span data-ttu-id="de833-213">Correction du problème #10963 lié à la logique d’ajout de type de nœud : L’ajout d’un nouveau type de nœud avec le niveau de durabilité Gold générera toujours une erreur CLI</span><span class="sxs-lookup"><span data-stu-id="de833-213">Fixed in node-type add logic including #10963: Adding new node type with durability level Gold will always throw CLI error</span></span>
* <span data-ttu-id="de833-214">Mise à jour de la version de ServiceFabricNodeVmExt vers la version 1.1 dans le modèle de création</span><span class="sxs-lookup"><span data-stu-id="de833-214">Updated ServiceFabricNodeVmExt version to 1.1 in creation template</span></span>

### <a name="sql"></a><span data-ttu-id="de833-215">SQL</span><span class="sxs-lookup"><span data-stu-id="de833-215">SQL</span></span>

* <span data-ttu-id="de833-216">Ajout de paramètres « --read-scale » et « --read-replicas » aux commandes sql db create et sql db update pour prendre en charge la gestion de l’échelle lecture.</span><span class="sxs-lookup"><span data-stu-id="de833-216">Added "--read-scale" and "--read-replicas" parameters to sql db create and update commands, to support read scale management.</span></span>

### <a name="storage"></a><span data-ttu-id="de833-217">Stockage</span><span class="sxs-lookup"><span data-stu-id="de833-217">Storage</span></span>

* <span data-ttu-id="de833-218">Propriété Partages de fichiers volumineux de la version en disponibilité générale pour les commandes storage account create et storage account update</span><span class="sxs-lookup"><span data-stu-id="de833-218">GA Release Large File Shares property for storage account create and update command</span></span>
* <span data-ttu-id="de833-219">Prise en charge des jetons SAS de délégation d’utilisateur de la version en disponibilité générale</span><span class="sxs-lookup"><span data-stu-id="de833-219">GA Release User Delegation SAS token Support</span></span>
* <span data-ttu-id="de833-220">Ajout des nouvelles commandes `az storage account blob-service-properties show` et `az storage account blob-service-properties update --enable-change-feed` afin de gérer les propriétés du service blob pour le compte de stockage.</span><span class="sxs-lookup"><span data-stu-id="de833-220">Added new commands `az storage account blob-service-properties show` and `az storage account blob-service-properties update --enable-change-feed` to manage blob service properties for storage account.</span></span>
* <span data-ttu-id="de833-221">[CHANGEMENT CASSANT À VENIR] `az storage copy` : le caractère `*` n’est plus pris en charge comme caractère générique dans l’URL, mais les nouveaux paramètres --include-pattern et --exclude-pattern seront ajoutés avec une prise en charge du caractère générique `*`.</span><span class="sxs-lookup"><span data-stu-id="de833-221">[COMING BREAKING CHANGE] `az storage copy`: `*` character is no longer supported as a wildcard in URL, but new parameters --include-pattern and --exclude-pattern will be added with `*` wildcard support.</span></span>
* <span data-ttu-id="de833-222">Résolution du problème #11043 : Ajout de la prise en charge de la suppression de l’intégralité du conteneur/partage dans la commande `az storage remove`</span><span class="sxs-lookup"><span data-stu-id="de833-222">Fixed issue #11043: Added support to remove whole container/share in `az storage remove` command</span></span>

## <a name="november-26-2019"></a><span data-ttu-id="de833-223">26 novembre 2019</span><span class="sxs-lookup"><span data-stu-id="de833-223">November 26, 2019</span></span>

<span data-ttu-id="de833-224">Version 2.0.77</span><span class="sxs-lookup"><span data-stu-id="de833-224">Version 2.0.77</span></span>

### <a name="acr"></a><span data-ttu-id="de833-225">ACR</span><span class="sxs-lookup"><span data-stu-id="de833-225">ACR</span></span>

* <span data-ttu-id="de833-226">Dépréciation du paramètre `--branch` dans acr task create/update</span><span class="sxs-lookup"><span data-stu-id="de833-226">Deprecated parameter `--branch` from acr task create/update</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="de833-227">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="de833-227">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="de833-228">Ajout de l’indicateur `--workspace-resource-id` pour permettre la création d’un cluster Azure Red Hat OpenShift avec supervision</span><span class="sxs-lookup"><span data-stu-id="de833-228">Added `--workspace-resource-id` flag to allow creation of Azure Red Hat Openshift cluster with monitoring</span></span>
* <span data-ttu-id="de833-229">Ajout de `monitor_profile` pour créer un cluster Azure Red Hat OpenShift avec supervision</span><span class="sxs-lookup"><span data-stu-id="de833-229">Added `monitor_profile` to create Azure Red Hat OpenShift cluster with monitoring</span></span>

### <a name="aks"></a><span data-ttu-id="de833-230">AKS</span><span class="sxs-lookup"><span data-stu-id="de833-230">AKS</span></span>

* <span data-ttu-id="de833-231">Ajout de la prise en charge de l’opération de rotation des certificats de cluster à l’aide de la commande « az aks rotate-certs ».</span><span class="sxs-lookup"><span data-stu-id="de833-231">Added support cluster certificate rotation operation using "az aks rotate-certs".</span></span>

### <a name="appconfig"></a><span data-ttu-id="de833-232">AppConfig</span><span class="sxs-lookup"><span data-stu-id="de833-232">AppConfig</span></span>

* <span data-ttu-id="de833-233">Ajout de la prise en charge de l’utilisation de « : » pour le séparateur `as az appconfig kv import`</span><span class="sxs-lookup"><span data-stu-id="de833-233">Added support for using ":" for `as az appconfig kv import` separator</span></span>
* <span data-ttu-id="de833-234">Résolution du problème de listage des valeurs de clés avec plusieurs étiquettes, y compris une étiquette Null.</span><span class="sxs-lookup"><span data-stu-id="de833-234">Fixed issue for listing key values with multiple labels including null label.</span></span> 
* <span data-ttu-id="de833-235">Mise à jour du SDK du plan de gestion, azure-mgmt-appconfiguration, vers la version 0.3.0.</span><span class="sxs-lookup"><span data-stu-id="de833-235">Updated management plane sdk, azure-mgmt-appconfiguration, to version 0.3.0.</span></span> 

### <a name="appservice"></a><span data-ttu-id="de833-236">AppService</span><span class="sxs-lookup"><span data-stu-id="de833-236">AppService</span></span>

* <span data-ttu-id="de833-237">Résolution du problème #11100 : Erreur d’attribut pour az webapp up lors de la création du plan de service</span><span class="sxs-lookup"><span data-stu-id="de833-237">Fixed issue #11100: AttributeError for az webapp up when create service plan</span></span>
* <span data-ttu-id="de833-238">az webapp up : En forçant la création ou le déploiement sur un site pour les langues prises en charge, aucune valeur par défaut n’est utilisée.</span><span class="sxs-lookup"><span data-stu-id="de833-238">az webapp up: Forcing the creation or deployment to a site for supported languages, no defaults used.</span></span>
* <span data-ttu-id="de833-239">Ajout de la prise en charge d’App Service Environment : az appservice ase show | list | list-addresses | list-plans | create | update | delete</span><span class="sxs-lookup"><span data-stu-id="de833-239">Added support for App Service Environment: az appservice ase show | list | list-addresses | list-plans | create | update | delete</span></span>

### <a name="backup"></a><span data-ttu-id="de833-240">Backup</span><span class="sxs-lookup"><span data-stu-id="de833-240">Backup</span></span>

* <span data-ttu-id="de833-241">Résolution du problème dans az backup policy list-associated-items.</span><span class="sxs-lookup"><span data-stu-id="de833-241">Fixed issue in az backup policy list-associated-items.</span></span> <span data-ttu-id="de833-242">Ajout du paramètre BackupManagementType facultatif.</span><span class="sxs-lookup"><span data-stu-id="de833-242">Added optional BackupManagementType parameter.</span></span>

### <a name="compute"></a><span data-ttu-id="de833-243">Calcul</span><span class="sxs-lookup"><span data-stu-id="de833-243">Compute</span></span>

* <span data-ttu-id="de833-244">Mise à jour de la version de l’API de calcul, des disques et des captures instantanées vers 2019-07-01</span><span class="sxs-lookup"><span data-stu-id="de833-244">Upgraded API version of compute, disks, snapshots to 2019-07-01</span></span>
* <span data-ttu-id="de833-245">vmss create : amélioration pour --orchestration-mode</span><span class="sxs-lookup"><span data-stu-id="de833-245">vmss create: Improvement for --orchestration-mode</span></span>
* <span data-ttu-id="de833-246">sig image-definition create : ajout de --os-state pour permettre de spécifier si les machines virtuelles créées sous cette image sont « généralisées » ou « spécialisées »</span><span class="sxs-lookup"><span data-stu-id="de833-246">sig image-definition create: Added --os-state to allow specifying whether the virtual machines created under this image are 'Generalized' or 'Specialized'</span></span>
* <span data-ttu-id="de833-247">sig image-definition create : ajout de --hyper-v-generation pour permettre la spécification de la génération de l’hyperviseur</span><span class="sxs-lookup"><span data-stu-id="de833-247">sig image-definition create: Added --hyper-v-generation to allow specifying the hypervisor generation</span></span>
* <span data-ttu-id="de833-248">sig image-version create : ajout de la prise en charge de --os-snapshot et de --data-snapshots</span><span class="sxs-lookup"><span data-stu-id="de833-248">sig image-version create: Added support --os-snapshot and --data-snapshots</span></span>
* <span data-ttu-id="de833-249">image create : ajout de --data-disk-caching pour autoriser la spécification du paramètre de mise en cache des disques de données</span><span class="sxs-lookup"><span data-stu-id="de833-249">image create: Added --data-disk-caching to allow specifying caching setting of data disks</span></span>
* <span data-ttu-id="de833-250">Mise à niveau du SDK Python Compute vers la version 10.0.0</span><span class="sxs-lookup"><span data-stu-id="de833-250">Upgraded Python Compute SDK to 10.0.0</span></span>
* <span data-ttu-id="de833-251">vm/vmss create : ajout de « Spot » à la propriété d’énumération « Priority »</span><span class="sxs-lookup"><span data-stu-id="de833-251">vm/vmss create: Added 'Spot' to 'Priority' enum property</span></span>
* <span data-ttu-id="de833-252">[Changement cassant] le paramètre « --max-billing » a été renommé « --max-price », pour les machines virtuelles et VMSS, à des fins de cohérence avec les applets de commande PowerShell et Swagger</span><span class="sxs-lookup"><span data-stu-id="de833-252">[Breaking change] Renamed '--max-billing' parameter to '--max-price', for both VM and VMSS, to be consistent with Swagger and Powershell cmdlets</span></span>
* <span data-ttu-id="de833-253">vm monitor log show : ajout de la prise en charge de l’interrogation du journal via l’espace de travail Log Analytics lié.</span><span class="sxs-lookup"><span data-stu-id="de833-253">vm monitor log show: Added support for querying log over linked log analytics workspace.</span></span>

### <a name="iot"></a><span data-ttu-id="de833-254">IOT</span><span class="sxs-lookup"><span data-stu-id="de833-254">IOT</span></span>

* <span data-ttu-id="de833-255">Correctif #2531 : ajout d’arguments facilitant la mise à jour des hubs.</span><span class="sxs-lookup"><span data-stu-id="de833-255">Fix #2531: Added convenience arguments for hub update.</span></span>
* <span data-ttu-id="de833-256">Correctif #8323 : ajout de paramètres manquants pour créer un point de terminaison personnalisé de stockage.</span><span class="sxs-lookup"><span data-stu-id="de833-256">Fix #8323: Added missing parameters to create storage custom endpoint.</span></span>
* <span data-ttu-id="de833-257">Correction d’un bogue de régression : restauration des modifications qui remplacent le point de terminaison de stockage par défaut.</span><span class="sxs-lookup"><span data-stu-id="de833-257">Fix regression bug: Reverted the changes which overrides the default storage endpoint.</span></span>

### <a name="key-vault"></a><span data-ttu-id="de833-258">Key Vault</span><span class="sxs-lookup"><span data-stu-id="de833-258">Key Vault</span></span>

* <span data-ttu-id="de833-259">Résolution du problème #11121 : lors de l’utilisation de `az keyvault certificate list`, le passage de `--include-pending` n’a plus besoin d’une valeur `true` ou `false`</span><span class="sxs-lookup"><span data-stu-id="de833-259">Fixed #11121: When using `az keyvault certificate list`, passing `--include-pending` now doesn't require a value of `true` or `false`</span></span>

### <a name="netappfiles"></a><span data-ttu-id="de833-260">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="de833-260">NetAppFiles</span></span>

* <span data-ttu-id="de833-261">Mise à niveau d’azure-mgmt-netapp vers 0.7.0, qui comprend des propriétés de volume supplémentaires associées aux opérations de réplication à venir</span><span class="sxs-lookup"><span data-stu-id="de833-261">Upgraded azure-mgmt-netapp to 0.7.0 which includes some additional volume properties associated with upcoming replication operations</span></span>

### <a name="network"></a><span data-ttu-id="de833-262">Réseau</span><span class="sxs-lookup"><span data-stu-id="de833-262">Network</span></span>

* <span data-ttu-id="de833-263">application-gateway waf-config : déprécié</span><span class="sxs-lookup"><span data-stu-id="de833-263">application-gateway waf-config: deprecated</span></span>
* <span data-ttu-id="de833-264">application-gateway waf-policy : ajout de règles managées par sous-groupes pour gérer des ensembles de règles managées et des règles d’exclusion</span><span class="sxs-lookup"><span data-stu-id="de833-264">application-gateway waf-policy: Added subgroup managed-rules to manage managed rule sets and exclusion rules</span></span>
* <span data-ttu-id="de833-265">application-gateway waf-policy : ajout d’un paramètre de stratégie de sous-groupe pour gérer la configuration globale d’une stratégie WAF</span><span class="sxs-lookup"><span data-stu-id="de833-265">application-gateway waf-policy: Added subgroup policy-setting to manage global configuration of a waf-policy</span></span>
* <span data-ttu-id="de833-266">[CHANGEMENT CASSANT] application-gateway waf-policy : règle de sous-groupe renommée en custom-rule</span><span class="sxs-lookup"><span data-stu-id="de833-266">[BREAKING CHANGE] application-gateway waf-policy: Renamed subgroup rule to custom-rule</span></span>
* <span data-ttu-id="de833-267">application-gateway http-listener : ajout de --firewall-policy lors de la création</span><span class="sxs-lookup"><span data-stu-id="de833-267">application-gateway http-listener: Added --firewall-policy when create</span></span>
* <span data-ttu-id="de833-268">application-gateway url-path-map rule : ajout de --firewall-policy lors de la création</span><span class="sxs-lookup"><span data-stu-id="de833-268">application-gateway url-path-map rule: Added --firewall-policy when create</span></span>

### <a name="packaging"></a><span data-ttu-id="de833-269">Packaging</span><span class="sxs-lookup"><span data-stu-id="de833-269">Packaging</span></span>

* <span data-ttu-id="de833-270">Réécriture du wrapper az dans Python</span><span class="sxs-lookup"><span data-stu-id="de833-270">Rewrote the az wrapper in Python</span></span>
* <span data-ttu-id="de833-271">Ajout de la prise en charge de Python 3.8</span><span class="sxs-lookup"><span data-stu-id="de833-271">Added support for Python 3.8</span></span>
* <span data-ttu-id="de833-272">Remplacement par Python 3 pour le package RPM</span><span class="sxs-lookup"><span data-stu-id="de833-272">Changed to Python 3 for RPM package</span></span>

### <a name="profile"></a><span data-ttu-id="de833-273">Profil</span><span class="sxs-lookup"><span data-stu-id="de833-273">Profile</span></span>

* <span data-ttu-id="de833-274">Suppression d’une erreur liée à l’exécution de `az login -u {} -p {}` avec un compte Microsoft</span><span class="sxs-lookup"><span data-stu-id="de833-274">Polished error when running `az login -u {} -p {}` with Microsoft account</span></span>
* <span data-ttu-id="de833-275">Suppression de `SSLError` liée à l’exécution de `az login` derrière un proxy avec un certificat racine auto-signé</span><span class="sxs-lookup"><span data-stu-id="de833-275">Polished `SSLError` when running `az login` behind a proxy with self-signed root certificate</span></span>
* <span data-ttu-id="de833-276">Résolution du problème #10578 : `az login` se bloque quand plusieurs instances sont lancées en même temps sur Windows ou WSL</span><span class="sxs-lookup"><span data-stu-id="de833-276">Fixed #10578: `az login` hangs when more than one instances are launched at the same time on Windows or WSL</span></span>
* <span data-ttu-id="de833-277">Résolution du problème #11059 : `az login --allow-no-subscriptions` échoue s’il existe des abonnements dans le locataire</span><span class="sxs-lookup"><span data-stu-id="de833-277">Fixed #11059: `az login --allow-no-subscriptions` fails if there are subscriptions in the tenant</span></span>
* <span data-ttu-id="de833-278">Résolution du problème #11238 : après avoir renommé un abonnement, la connexion avec MSI entraîne l’affichage du même abonnement deux fois</span><span class="sxs-lookup"><span data-stu-id="de833-278">Fixed #11238: After renaming a subscription, logging in with MSI will result in the same subscription appearing twice</span></span>

### <a name="rbac"></a><span data-ttu-id="de833-279">RBAC</span><span class="sxs-lookup"><span data-stu-id="de833-279">RBAC</span></span>

* <span data-ttu-id="de833-280">Résolution du problème #10996 : suppression de l’erreur liée à `--force-change-password-next-login` dans `az ad user update` quand `--password` n’est pas spécifié</span><span class="sxs-lookup"><span data-stu-id="de833-280">Fixed #10996: Polish error for `--force-change-password-next-login` in `az ad user update` when `--password` is not specified</span></span>

### <a name="redis"></a><span data-ttu-id="de833-281">Redis</span><span class="sxs-lookup"><span data-stu-id="de833-281">Redis</span></span>

* <span data-ttu-id="de833-282">Résolution de l’erreur #2902 : éviter de définir des configurations de mémoire lors de la mise à jour du cache de référence SKU de base</span><span class="sxs-lookup"><span data-stu-id="de833-282">Fixed #2902: Avoid setting memory configs while updating Basic SKU cache</span></span>

### <a name="reservations"></a><span data-ttu-id="de833-283">Réservations</span><span class="sxs-lookup"><span data-stu-id="de833-283">Reservations</span></span>

* <span data-ttu-id="de833-284">Mise à niveau du SDK vers 0.6.0</span><span class="sxs-lookup"><span data-stu-id="de833-284">Upgraded SDK Version to 0.6.0</span></span>
* <span data-ttu-id="de833-285">Ajout d’informations détaillées sur le plan de facturation après l’appel de Get-Gatalogs</span><span class="sxs-lookup"><span data-stu-id="de833-285">Added billingplan details info after calling Get-Gatalogs</span></span>
* <span data-ttu-id="de833-286">Ajout d’une nouvelle commande `az reservations reservation-order calculate` pour calculer le prix d’une réservation</span><span class="sxs-lookup"><span data-stu-id="de833-286">Added new command `az reservations reservation-order calculate` to calculate the price for a reservation</span></span>
* <span data-ttu-id="de833-287">Ajout d’une nouvelle commande `az reservations reservation-order purchase` pour acheter une nouvelle réservation</span><span class="sxs-lookup"><span data-stu-id="de833-287">Added new command `az reservations reservation-order purchase` to purchase a new reservation</span></span>

### <a name="rest"></a><span data-ttu-id="de833-288">Rest</span><span class="sxs-lookup"><span data-stu-id="de833-288">Rest</span></span>
* <span data-ttu-id="de833-289">`az rest` désormais mis à la disposition générale</span><span class="sxs-lookup"><span data-stu-id="de833-289">Changed `az rest` to GA</span></span>

### <a name="sql"></a><span data-ttu-id="de833-290">SQL</span><span class="sxs-lookup"><span data-stu-id="de833-290">SQL</span></span>

* <span data-ttu-id="de833-291">Mise à jour d’azure-mgmt-sql vers la version 0.15.0.</span><span class="sxs-lookup"><span data-stu-id="de833-291">Updated azure-mgmt-sql to version 0.15.0.</span></span>

### <a name="storage"></a><span data-ttu-id="de833-292">Stockage</span><span class="sxs-lookup"><span data-stu-id="de833-292">Storage</span></span>

* <span data-ttu-id="de833-293">storage account create : ajout de --enable-hierarchical-namespace pour prendre en charge la sémantique du système de fichiers dans le service BLOB.</span><span class="sxs-lookup"><span data-stu-id="de833-293">storage account create: Added --enable-hierarchical-namespace to support filesystem semantics in blob service.</span></span>
* <span data-ttu-id="de833-294">Suppression de l’exception non liée du message d’erreur</span><span class="sxs-lookup"><span data-stu-id="de833-294">Removed unrelated exception from error message</span></span>
* <span data-ttu-id="de833-295">Résolution des problèmes liés à un message d’erreur incorrect « Vous ne disposez pas des autorisations nécessaires pour effectuer cette opération. »</span><span class="sxs-lookup"><span data-stu-id="de833-295">Fixed issues with incorrect error message "You do not have the required permissions needed to perform this operation."</span></span> <span data-ttu-id="de833-296">en cas de blocage par des règles de réseau ou AuthenticationFailed.</span><span class="sxs-lookup"><span data-stu-id="de833-296">when blocked by network rules or AuthenticationFailed.</span></span>

## <a name="november-4-2019"></a><span data-ttu-id="de833-297">4 novembre 2019</span><span class="sxs-lookup"><span data-stu-id="de833-297">November 4, 2019</span></span>

<span data-ttu-id="de833-298">Version 2.0.76</span><span class="sxs-lookup"><span data-stu-id="de833-298">Version 2.0.76</span></span>

### <a name="acr"></a><span data-ttu-id="de833-299">ACR</span><span class="sxs-lookup"><span data-stu-id="de833-299">ACR</span></span>

* <span data-ttu-id="de833-300">Ajout d’un paramètre d’aperçu `--pack-image-tag` à la commande `az acr pack build`.</span><span class="sxs-lookup"><span data-stu-id="de833-300">Added a preview parameter `--pack-image-tag` to command `az acr pack build`.</span></span>
* <span data-ttu-id="de833-301">Ajout de la prise en charge de l’activation de l’audit lors de la création d’un registre</span><span class="sxs-lookup"><span data-stu-id="de833-301">Added support for enabling auditing on creating a registry</span></span>
* <span data-ttu-id="de833-302">Ajout de la prise en charge du contrôle d’accès en fonction du rôle délimité par le dépôt</span><span class="sxs-lookup"><span data-stu-id="de833-302">Added support for Repository-scoped RBAC</span></span>

### <a name="aks"></a><span data-ttu-id="de833-303">AKS</span><span class="sxs-lookup"><span data-stu-id="de833-303">AKS</span></span>

* <span data-ttu-id="de833-304">Ajout de `--enable-cluster-autoscaler`, `--min-count` et `--max-count` à la commande `az aks create`, ce qui active l’autoscaler de cluster pour le pool de nœuds.</span><span class="sxs-lookup"><span data-stu-id="de833-304">Added `--enable-cluster-autoscaler`, `--min-count` and `--max-count` to the `az aks create` command, which enables cluster autoscaler for the node pool.</span></span>
* <span data-ttu-id="de833-305">Ajout des indicateurs ci-dessus ainsi que de `--update-cluster-autoscaler` et `--disable-cluster-autoscaler` à la commande `az aks update`, ce qui permet d’effectuer des mises à jour de l’autoscaler de cluster.</span><span class="sxs-lookup"><span data-stu-id="de833-305">Added the above flags as well as `--update-cluster-autoscaler` and `--disable-cluster-autoscaler` to the `az aks update` command, allowing updates to cluster autoscaler.</span></span>

### <a name="appconfig"></a><span data-ttu-id="de833-306">AppConfig</span><span class="sxs-lookup"><span data-stu-id="de833-306">AppConfig</span></span>

* <span data-ttu-id="de833-307">Ajout du groupe de commandes de fonctionnalités appconfig pour gérer les indicateurs de fonctionnalité stockés dans une configuration d’application.</span><span class="sxs-lookup"><span data-stu-id="de833-307">Added appconfig feature command group to manage feature flags stored in an App Configuration.</span></span>
* <span data-ttu-id="de833-308">Correction de bogue mineur pour la commande Exporter vers un fichier appconfig kv.</span><span class="sxs-lookup"><span data-stu-id="de833-308">Fixed minor bug for appconfig kv export to file command.</span></span> <span data-ttu-id="de833-309">Arrêt de la lecture du contenu du fichier de destination pendant l’exportation.</span><span class="sxs-lookup"><span data-stu-id="de833-309">Stop reading dest file contents during export.</span></span>

### <a name="appservice"></a><span data-ttu-id="de833-310">AppService</span><span class="sxs-lookup"><span data-stu-id="de833-310">AppService</span></span>

* <span data-ttu-id="de833-311">`az appservice plan create`: Ajout de la prise en charge de la définition de « persitescaling » sur appservice plan create.</span><span class="sxs-lookup"><span data-stu-id="de833-311">`az appservice plan create`: Added support to set 'persitescaling' on appservice plan create.</span></span>
* <span data-ttu-id="de833-312">Résolution d’un problème où l’opération de liaison SSL de la configuration webapp supprimait les balises existantes de la ressource</span><span class="sxs-lookup"><span data-stu-id="de833-312">Fixed an issue where webapp config ssl bind operation was removing existing tags from the resource</span></span>
* <span data-ttu-id="de833-313">Ajout de l’indicateur `--build-remote` pour `az functionapp deployment source config-zip` afin de prendre en charge l’action de génération distante pendant le déploiement de l’application de fonction.</span><span class="sxs-lookup"><span data-stu-id="de833-313">Added `--build-remote` flag for `az functionapp deployment source config-zip` to support remote build action during function app deployment.</span></span>
* <span data-ttu-id="de833-314">Remplacement de la version du nœud par défaut sur les applications de fonction par ~10 pour Windows</span><span class="sxs-lookup"><span data-stu-id="de833-314">Changed default node version on function apps to ~10 for Windows</span></span>
* <span data-ttu-id="de833-315">Ajout de la propriété `--runtime-version` à `az functionapp create`</span><span class="sxs-lookup"><span data-stu-id="de833-315">Added `--runtime-version` property to `az functionapp create`</span></span>

### <a name="arm"></a><span data-ttu-id="de833-316">ARM</span><span class="sxs-lookup"><span data-stu-id="de833-316">ARM</span></span>

* <span data-ttu-id="de833-317">`az deployment/group deployment validate`: Ajout du paramètre `--handle-extended-json-format` pour prendre en charge le format multiligne et les commentaires dans le modèle json lors du déploiement.</span><span class="sxs-lookup"><span data-stu-id="de833-317">`az deployment/group deployment validate`: Added `--handle-extended-json-format` parameter to support multiline and comments in json template when deployment.</span></span>
* <span data-ttu-id="de833-318">Passage d’azure-mgmt-resource à 2019-07-01</span><span class="sxs-lookup"><span data-stu-id="de833-318">Bumped azure-mgmt-resource to 2019-07-01</span></span>

### <a name="backup"></a><span data-ttu-id="de833-319">Backup</span><span class="sxs-lookup"><span data-stu-id="de833-319">Backup</span></span>

* <span data-ttu-id="de833-320">Ajout de la prise en charge de la sauvegarde AzureFiles</span><span class="sxs-lookup"><span data-stu-id="de833-320">Added AzureFiles backup support</span></span>

### <a name="compute"></a><span data-ttu-id="de833-321">Calcul</span><span class="sxs-lookup"><span data-stu-id="de833-321">Compute</span></span>

* <span data-ttu-id="de833-322">`az vm create`: Ajout d’un avertissement lors de la spécification de la mise en réseau accélérée avec une carte réseau existante.</span><span class="sxs-lookup"><span data-stu-id="de833-322">`az vm create`: Added warning when specifying accelerated networking and an existing NIC together.</span></span>
* <span data-ttu-id="de833-323">`az vm create`: Ajout de `--vmss` pour spécifier un groupe identique de machines virtuelles existant auquel la machine virtuelle doit être affectée.</span><span class="sxs-lookup"><span data-stu-id="de833-323">`az vm create`: Added `--vmss` to specify an existing virtual machine scale set that the virtual machine should be assigned to.</span></span>
* <span data-ttu-id="de833-324">`az vm/vmss create`: Ajout d’une copie locale du fichier d’alias d’image afin qu’il soit accessible dans un environnement réseau restreint.</span><span class="sxs-lookup"><span data-stu-id="de833-324">`az vm/vmss create`: Added a local copy of image alias file so that it can be accessed in a restricted network environment.</span></span>
* <span data-ttu-id="de833-325">`az vmss create`: Ajout de `--orchestration-mode` pour spécifier la façon dont les machines virtuelles sont gérées par le groupe identique.</span><span class="sxs-lookup"><span data-stu-id="de833-325">`az vmss create`: Added `--orchestration-mode` to specify how virtual machines are managed by the scale set.</span></span>
* <span data-ttu-id="de833-326">`az vm/vmss update`: Ajout de `--ultra-ssd-enabled` pour autoriser la mise à jour du paramètre SSD Ultra.</span><span class="sxs-lookup"><span data-stu-id="de833-326">`az vm/vmss update`: Added `--ultra-ssd-enabled` to allow updating ultra SSD setting.</span></span>
* <span data-ttu-id="de833-327">[CHANGEMENT CASSANT] `az vm extension set` : Correction d’un bogue qui empêchait les utilisateurs de définir une extension sur une machine virtuelle avec `--ids`.</span><span class="sxs-lookup"><span data-stu-id="de833-327">[BREAKING CHANGE] `az vm extension set`: Fixed bug where users could not set an extension on a VM with `--ids`.</span></span>
* <span data-ttu-id="de833-328">Ajout de nouvelles commandes `az vm image terms accept/cancel/show` pour gérer les termes de l’image de la Place de marché Azure.</span><span class="sxs-lookup"><span data-stu-id="de833-328">Added new commands `az vm image terms accept/cancel/show` to manage Azure Marketplace image terms.</span></span>
* <span data-ttu-id="de833-329">Mise à jour de VMAccessForLinux vers la version 1.5</span><span class="sxs-lookup"><span data-stu-id="de833-329">Updated VMAccessForLinux to version 1.5</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="de833-330">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="de833-330">CosmosDB</span></span>

* <span data-ttu-id="de833-331">[CHANGEMENT CASSANT] `az sql container create` : Modification de `--partition-key-path` en paramètre obligatoire</span><span class="sxs-lookup"><span data-stu-id="de833-331">[BREAKING CHANGE] `az sql container create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="de833-332">[CHANGEMENT CASSANT] `az gremlin graph create` : Modification de `--partition-key-path` en paramètre obligatoire</span><span class="sxs-lookup"><span data-stu-id="de833-332">[BREAKING CHANGE] `az gremlin graph create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="de833-333">`az sql container create`: Ajout de `--unique-key-policy` et `--conflict-resolution-policy`</span><span class="sxs-lookup"><span data-stu-id="de833-333">`az sql container create`: Added `--unique-key-policy` and `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="de833-334">`az sql container create/update`: Mise à jour du schéma par défaut `--idx`</span><span class="sxs-lookup"><span data-stu-id="de833-334">`az sql container create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="de833-335">`gremlin graph create`: Ajout de `--conflict-resolution-policy`</span><span class="sxs-lookup"><span data-stu-id="de833-335">`gremlin graph create`: Added `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="de833-336">`gremlin graph create/update`: Mise à jour du schéma par défaut `--idx`</span><span class="sxs-lookup"><span data-stu-id="de833-336">`gremlin graph create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="de833-337">Faute de frappe corrigée dans un message d’aide</span><span class="sxs-lookup"><span data-stu-id="de833-337">Fixed typo in help message</span></span>
* <span data-ttu-id="de833-338">base de données : ajout d’informations de dépréciation</span><span class="sxs-lookup"><span data-stu-id="de833-338">database: Added deprecation infomation</span></span>
* <span data-ttu-id="de833-339">collection : ajout d’informations de dépréciation</span><span class="sxs-lookup"><span data-stu-id="de833-339">collection: Added deprecation infomation</span></span>

### <a name="iot"></a><span data-ttu-id="de833-340">IoT</span><span class="sxs-lookup"><span data-stu-id="de833-340">IoT</span></span>

* <span data-ttu-id="de833-341">Ajout d’un nouveau type de source de routage : DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="de833-341">Added new routing source type: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="de833-342">Correction des fonctionnalités manquantes dans `az iot hub create`</span><span class="sxs-lookup"><span data-stu-id="de833-342">Fixed missing features in `az iot hub create`</span></span>

### <a name="key-vault"></a><span data-ttu-id="de833-343">Key Vault</span><span class="sxs-lookup"><span data-stu-id="de833-343">Key Vault</span></span>

* <span data-ttu-id="de833-344">Correction d’une erreur inattendue lorsque le fichier de certificat n’existe pas</span><span class="sxs-lookup"><span data-stu-id="de833-344">Fixed an unexpected error when certificate file does not exist</span></span>
* <span data-ttu-id="de833-345">Résolution de `az keyvault recover/purge` qui ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="de833-345">Fixed `az keyvault recover/purge` not working</span></span>

### <a name="netappfiles"></a><span data-ttu-id="de833-346">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="de833-346">NetAppFiles</span></span>

* <span data-ttu-id="de833-347">Mise à niveau d’azure-mgmt-netapp vers 0.6.0 pour utiliser la version d’API 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="de833-347">Upgraded azure-mgmt-netapp to 0.6.0 to use API version 2019-07-01.</span></span> <span data-ttu-id="de833-348">Cette nouvelle version d’API comprend les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="de833-348">This new API version includes:</span></span>

    - <span data-ttu-id="de833-349">La création de volume `--protocol-types` accepte maintenant « NFSv4.1 » et non « NFSv4 »</span><span class="sxs-lookup"><span data-stu-id="de833-349">Volume creation `--protocol-types` accepts now "NFSv4.1" not "NFSv4"</span></span>
    - <span data-ttu-id="de833-350">La propriété de stratégie d’exportation de volume est maintenant nommée « nfsv41 » et non « nfsv4 »</span><span class="sxs-lookup"><span data-stu-id="de833-350">Volume export policy property now named 'nfsv41' not 'nfsv4'</span></span>
    - <span data-ttu-id="de833-351">Le volume `--creation-token` est renommé en `--file-path`</span><span class="sxs-lookup"><span data-stu-id="de833-351">Volume `--creation-token` renamed to `--file-path`</span></span>
    - <span data-ttu-id="de833-352">La date de création de l’instantané porte maintenant juste le nom « créé »</span><span class="sxs-lookup"><span data-stu-id="de833-352">Snapshot creation date now named just 'created'</span></span>

### <a name="network"></a><span data-ttu-id="de833-353">Réseau</span><span class="sxs-lookup"><span data-stu-id="de833-353">Network</span></span>

* <span data-ttu-id="de833-354">`az network private-dns link vnet create/update`: Prise en charge de la liaison de réseau virtuel entre locataires.</span><span class="sxs-lookup"><span data-stu-id="de833-354">`az network private-dns link vnet create/update`: Support cross-tenant virtual network linking.</span></span>
* <span data-ttu-id="de833-355">[CHANGEMENT CASSANT] `az network vnet subnet list` : Modification de `--resource-group` et `--vnet-name` pour être maintenant nécessaires.</span><span class="sxs-lookup"><span data-stu-id="de833-355">[BREAKING CHANGE] `az network vnet subnet list`: Changed `--resource-group` and `--vnet-name` to be required now.</span></span>
* <span data-ttu-id="de833-356">`az network public-ip prefix create`: Ajout de la prise en charge de la spécification de la version d’adresse IP (IPv4, IPv6) lors de la création</span><span class="sxs-lookup"><span data-stu-id="de833-356">`az network public-ip prefix create`: Added support to specify IP address version (IPv4, IPv6) when creation</span></span>
* <span data-ttu-id="de833-357">Passage d’azure-mgmt-network à 7.0.0 et d’api-version à 2019-09-01</span><span class="sxs-lookup"><span data-stu-id="de833-357">Bumped azure-mgmt-network to 7.0.0 and api-version to 2019-09-01</span></span>
* <span data-ttu-id="de833-358">`az network vrouter`: Ajout de la prise en charge du nouveau routeur virtuel de service et de l’appairage de routeur virtuel</span><span class="sxs-lookup"><span data-stu-id="de833-358">`az network vrouter`: Added support for new service virtual router and virtual router peering</span></span>
* <span data-ttu-id="de833-359">`az network express-route gateway connection`: Ajout de la prise en charge de `--internet-security`</span><span class="sxs-lookup"><span data-stu-id="de833-359">`az network express-route gateway connection`: Added support for `--internet-security`</span></span>

### <a name="profile"></a><span data-ttu-id="de833-360">Profil</span><span class="sxs-lookup"><span data-stu-id="de833-360">Profile</span></span>

* <span data-ttu-id="de833-361">Résolution de `az account get-access-token --resource-type ms-graph` qui ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="de833-361">Fixed `az account get-access-token --resource-type ms-graph` not working</span></span>
* <span data-ttu-id="de833-362">Suppression de l’avertissement de `az login`</span><span class="sxs-lookup"><span data-stu-id="de833-362">Removed warning from `az login`</span></span>

### <a name="rbac"></a><span data-ttu-id="de833-363">RBAC</span><span class="sxs-lookup"><span data-stu-id="de833-363">RBAC</span></span>

* <span data-ttu-id="de833-364">Résolution de `az ad app update --id {} --display-name {}` qui ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="de833-364">Fixed `az ad app update --id {} --display-name {}` doesn't work</span></span>

### <a name="servicefabric"></a><span data-ttu-id="de833-365">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="de833-365">ServiceFabric</span></span>

* <span data-ttu-id="de833-366">`az sf cluster create`: Résolution d’un problème en modifiant le groupe identique de machines virtuelles de calcul template.json Service Fabric Linux et Windows de disques standard en disques managés</span><span class="sxs-lookup"><span data-stu-id="de833-366">`az sf cluster create`: Fixed an issue by modifying service fabric linux and windows template.json compute vmss from standard to managed disks</span></span>

### <a name="sql"></a><span data-ttu-id="de833-367">SQL</span><span class="sxs-lookup"><span data-stu-id="de833-367">SQL</span></span>

* <span data-ttu-id="de833-368">Ajout de paramètres `--compute-model`, `--auto-pause-delay` et `--min-capacity` afin de prendre en charge les opérations CRUD pour la nouvelle offre SQL Database : Modèle de calcul serverless.</span><span class="sxs-lookup"><span data-stu-id="de833-368">Added `--compute-model`, `--auto-pause-delay`, and `--min-capacity` parameters to support CRUD operations for new SQL Database offering: Serverless compute model.</span></span>

### <a name="storage"></a><span data-ttu-id="de833-369">Stockage</span><span class="sxs-lookup"><span data-stu-id="de833-369">Storage</span></span>

* <span data-ttu-id="de833-370">`az storage account create/update`: Ajout du paramètre --enable-files-adds et du groupe d’arguments de propriétés Azure Active Directory pour prendre en charge l’authentification de service de domaine Azure Files Active Directory</span><span class="sxs-lookup"><span data-stu-id="de833-370">`az storage account create/update`: Added --enable-files-adds parameter and Azure Active Directory Properties Argument group to support Azure Files Active Directory Domain Service Authentication</span></span>
* <span data-ttu-id="de833-371">Développement de `az storage account keys list/renew` pour prendre en charge le listing ou la regénération des clés Kerberos du compte de stockage.</span><span class="sxs-lookup"><span data-stu-id="de833-371">Expanded `az storage account keys list/renew` to support listing or regenerating Kerberos keys of storage account.</span></span>

## <a name="october-15-2019"></a><span data-ttu-id="de833-372">15 octobre 2019</span><span class="sxs-lookup"><span data-stu-id="de833-372">October 15, 2019</span></span>

<span data-ttu-id="de833-373">Version 2.0.75</span><span class="sxs-lookup"><span data-stu-id="de833-373">Version 2.0.75</span></span>

### <a name="aks"></a><span data-ttu-id="de833-374">AKS</span><span class="sxs-lookup"><span data-stu-id="de833-374">AKS</span></span>

* <span data-ttu-id="de833-375">Remplacement de la valeur par défaut `--load-balancer-sku` par `standard` si elle est prise en charge par la version kubernetes</span><span class="sxs-lookup"><span data-stu-id="de833-375">Changed `--load-balancer-sku` default value to `standard` if supported by the kubernetes version</span></span>
* <span data-ttu-id="de833-376">Remplacement de la valeur par défaut `--vm-set-type` par `virtualmachinescalesets` si elle est prise en charge par la version kubernetes</span><span class="sxs-lookup"><span data-stu-id="de833-376">Changed `--vm-set-type` default value to `virtualmachinescalesets` if supported by the kubernetes version</span></span>

### <a name="ams"></a><span data-ttu-id="de833-377">AMS</span><span class="sxs-lookup"><span data-stu-id="de833-377">AMS</span></span>

* <span data-ttu-id="de833-378">[CHANGEMENT CASSANT] Remplacement du nom `job start` par `job create`</span><span class="sxs-lookup"><span data-stu-id="de833-378">[BREAKING CHANGE] Changed the name of `job start` to `job create`</span></span>
* <span data-ttu-id="de833-379">[CHANGEMENT CASSANT] Changement du paramètre `--ask` de `content-key-policy create` pour utiliser une chaîne hexadécimale de 32 caractères au lieu d’UTF8</span><span class="sxs-lookup"><span data-stu-id="de833-379">[BREAKING CHANGE] Changed the `--ask` parameter of `content-key-policy create` to use a 32-character hex string instead of UTF8</span></span>

### <a name="appservice"></a><span data-ttu-id="de833-380">AppService</span><span class="sxs-lookup"><span data-stu-id="de833-380">AppService</span></span>

* <span data-ttu-id="de833-381">Ajout des commandes `webapp config access-restriction show|set|add|remove`</span><span class="sxs-lookup"><span data-stu-id="de833-381">Added commands `webapp config access-restriction show|set|add|remove`</span></span>
* <span data-ttu-id="de833-382">Ajout d’une meilleure gestion des erreurs à `webapp up`</span><span class="sxs-lookup"><span data-stu-id="de833-382">Added better error handling to `webapp up`</span></span>
* <span data-ttu-id="de833-383">Ajout de la prise en charge de la référence SKU `Isolated` pour `appservice plan update`</span><span class="sxs-lookup"><span data-stu-id="de833-383">Added support for `Isolated` SKU to `appservice plan update`</span></span>

### <a name="arm"></a><span data-ttu-id="de833-384">ARM</span><span class="sxs-lookup"><span data-stu-id="de833-384">ARM</span></span>

* <span data-ttu-id="de833-385">Ajout du paramètre `--handle-extended-json-format` à `deployment create` pour prendre en charge le format multiligne et les commentaires dans le modèle json</span><span class="sxs-lookup"><span data-stu-id="de833-385">Added `--handle-extended-json-format` parameter `deployment create` to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="de833-386">Calcul</span><span class="sxs-lookup"><span data-stu-id="de833-386">Compute</span></span>

* <span data-ttu-id="de833-387">Ajout du paramètre `--enable-agent` pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="de833-387">Added `--enable-agent` parameter to `vm create`</span></span>
* <span data-ttu-id="de833-388">Changement de `vm create` pour utiliser automatiquement la référence SKU d’adresse IP publique standard lors de l’utilisation de zones</span><span class="sxs-lookup"><span data-stu-id="de833-388">Changed `vm create` to use standard public IP SKU automatically when using zones</span></span>
* <span data-ttu-id="de833-389">Changement de `vm create` pour créer automatiquement un nom d’ordinateur valide pour une machine virtuelle si aucun n’est fourni</span><span class="sxs-lookup"><span data-stu-id="de833-389">Changed `vm create` to automatically create a valid computer name for a VM if none is provided</span></span>
* <span data-ttu-id="de833-390">Ajout du paramètre `--computer-name-prefix` à `vmss create` pour prendre en charge le préfixe de nom d’ordinateur personnalisé des machines virtuelles dans VMSS</span><span class="sxs-lookup"><span data-stu-id="de833-390">Added `--computer-name-prefix` parameter to `vmss create` to support custom computer name prefix of virtual machines in the VMSS</span></span>
* <span data-ttu-id="de833-391">Ajout du paramètre `--workspace` à `vm create` pour activer automatiquement l’espace de travail Log Analytics</span><span class="sxs-lookup"><span data-stu-id="de833-391">Add `--workspace` parameter to `vm create` to enable log analytics workspace automatically</span></span>
* <span data-ttu-id="de833-392">Mise à jour de la version de l’API des galeries vers 2019-07-01</span><span class="sxs-lookup"><span data-stu-id="de833-392">Updated galleries API version to 2019-07-01</span></span>

### <a name="core"></a><span data-ttu-id="de833-393">Core</span><span class="sxs-lookup"><span data-stu-id="de833-393">Core</span></span>

* <span data-ttu-id="de833-394">Ajout de la vérification de la syntaxe pour le paramètre `--set` dans la commande de mise à jour générique</span><span class="sxs-lookup"><span data-stu-id="de833-394">Added syntax check for `--set` parameter in generic update command</span></span>

### <a name="iot"></a><span data-ttu-id="de833-395">IoT</span><span class="sxs-lookup"><span data-stu-id="de833-395">IoT</span></span>

* <span data-ttu-id="de833-396">Résolution d’un problème où `iot hub show` entraînait une erreur incorrecte « ressource introuvable »</span><span class="sxs-lookup"><span data-stu-id="de833-396">Fixed an issue where `iot hub show` would incorrectly error with "resource not found"</span></span>

### <a name="monitor"></a><span data-ttu-id="de833-397">Moniteur</span><span class="sxs-lookup"><span data-stu-id="de833-397">Monitor</span></span>

* <span data-ttu-id="de833-398">Ajout de la prise en charge de CRUD dans `monitor log-analytics workspace`</span><span class="sxs-lookup"><span data-stu-id="de833-398">Added support for CRUD to `monitor log-analytics workspace`</span></span>

### <a name="network"></a><span data-ttu-id="de833-399">Réseau</span><span class="sxs-lookup"><span data-stu-id="de833-399">Network</span></span>

* <span data-ttu-id="de833-400">Ajout de la prise en charge de la liaison virtuelle interlocataire dans `network private-dns link vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="de833-400">Added support for cross-tenant virtual linking to `network private-dns link vnet [create|update]`</span></span>
* <span data-ttu-id="de833-401">[CHANGEMENT CASSANT] Changement de `network vnet subnet list` pour exiger les paramètres `--resource-group` et `--vnet-name`</span><span class="sxs-lookup"><span data-stu-id="de833-401">[BREAKING CHANGE] Changed `network vnet subnet list` to require `--resource-group` and `--vnet-name` parameters</span></span>

### <a name="sql"></a><span data-ttu-id="de833-402">SQL</span><span class="sxs-lookup"><span data-stu-id="de833-402">SQL</span></span>

* <span data-ttu-id="de833-403">Ajout de commandes à `sql mi ad-admin` qui prennent en charge la définition d’un administrateur AAD sur des instances managées</span><span class="sxs-lookup"><span data-stu-id="de833-403">Added commands to `sql mi ad-admin` that support setting an AAD administrator on managed instances</span></span>

### <a name="storage"></a><span data-ttu-id="de833-404">Stockage</span><span class="sxs-lookup"><span data-stu-id="de833-404">Storage</span></span>

* <span data-ttu-id="de833-405">Ajout du paramètre `--preserve-s2s-access-tier` à `storage copy` pour préserver le niveau d’accès lors d’une copie de service à service</span><span class="sxs-lookup"><span data-stu-id="de833-405">Added `--preserve-s2s-access-tier` parameter `storage copy` to preserve access tier during service to service copy</span></span>
* <span data-ttu-id="de833-406">Ajout du paramètre `--enable-large-file-share` à `storage account [create|update]` afin de prendre en charge les gros partages de fichiers pour le compte de stockage</span><span class="sxs-lookup"><span data-stu-id="de833-406">Added `--enable-large-file-share` parameter to `storage account [create|update]` to support large file shares for storage account</span></span>

## <a name="september-24-2019"></a><span data-ttu-id="de833-407">24 septembre 2019</span><span class="sxs-lookup"><span data-stu-id="de833-407">September 24, 2019</span></span>

<span data-ttu-id="de833-408">Version 2.0.74</span><span class="sxs-lookup"><span data-stu-id="de833-408">Version 2.0.74</span></span>

### <a name="acr"></a><span data-ttu-id="de833-409">ACR</span><span class="sxs-lookup"><span data-stu-id="de833-409">ACR</span></span>

* <span data-ttu-id="de833-410">Ajout d’un paramètre `--type` obligatoire à `acr config retention update`</span><span class="sxs-lookup"><span data-stu-id="de833-410">Added a required `--type` parameter to `acr config retention update`</span></span>
* <span data-ttu-id="de833-411">[CHANGEMENT CASSANT] Remplacement du paramètre `--name -n` par `--registry -r ` pour le groupe de commandes `acr config`</span><span class="sxs-lookup"><span data-stu-id="de833-411">[BREAKING CHNAGE] Renamed parameter `--name -n` changed to `--registry -r ` for `acr config` command group</span></span>

### <a name="aks"></a><span data-ttu-id="de833-412">AKS</span><span class="sxs-lookup"><span data-stu-id="de833-412">AKS</span></span>

* <span data-ttu-id="de833-413">Ajout du paramètre `--load-balancer-sku` à la commande `aks create`, ce qui permet de créer un cluster AKS avec SLB</span><span class="sxs-lookup"><span data-stu-id="de833-413">Added `--load-balancer-sku` parameter to `aks create` command, which allows for creating AKS cluster with SLB</span></span>
* <span data-ttu-id="de833-414">Ajout des paramètres `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` et `--load-balancer-outbound-ip-prefixes` aux commandes `aks [create|update]`, ce qui permet de mettre à jour le profil d’équilibreur de charge d’un cluster AKS avec SLB</span><span class="sxs-lookup"><span data-stu-id="de833-414">Added `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` and `--load-balancer-outbound-ip-prefixes` parameters to `aks [create|update]` commands, which allow for updating load balancer profile of an AKS cluster with SLB</span></span>
* <span data-ttu-id="de833-415">Ajout du paramètre `--vm-set-type` à la commande `aks create`, ce qui permet de spécifier les types de machines virtuelles d’un cluster AKS (vmas ou vmss)</span><span class="sxs-lookup"><span data-stu-id="de833-415">Added `--vm-set-type` parameter to `aks create` command, which allows to specify vm types of an AKS Cluster (vmas or vmss)</span></span>

### <a name="arm"></a><span data-ttu-id="de833-416">ARM</span><span class="sxs-lookup"><span data-stu-id="de833-416">ARM</span></span>

* <span data-ttu-id="de833-417">Ajout du paramètre `--handle-extended-json-format` à la commande `group deployment create` pour prendre en charge les lignes multiples et les commentaires dans le modèle JSON</span><span class="sxs-lookup"><span data-stu-id="de833-417">Added `--handle-extended-json-format` parameter to `group deployment create` command to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="de833-418">Calcul</span><span class="sxs-lookup"><span data-stu-id="de833-418">Compute</span></span>

* <span data-ttu-id="de833-419">Ajout du paramètre `--terminate-notification-time` aux commandes `vmss [create|update]` pour prendre en charge la configuration de l’événement planifié d’arrêt</span><span class="sxs-lookup"><span data-stu-id="de833-419">Added `--terminate-notification-time` parameter to `vmss [create|update]` commands to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="de833-420">Ajout du paramètre `--enable-terminate-notification` à la commande `vmss update` pour prendre en charge la configuration de l’événement planifié d’arrêt</span><span class="sxs-lookup"><span data-stu-id="de833-420">Added `--enable-terminate-notification` parameter to `vmss update` command to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="de833-421">Ajout des paramètres `--priority,``--eviction-policy,``--max-billing` aux commandes `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="de833-421">Added `--priority,` `--eviction-policy,` `--max-billing` parameters to `[vm|vmss] create` commands</span></span>
* <span data-ttu-id="de833-422">Modification de `disk create` pour autoriser la spécification de la taille exacte du chargement de disque</span><span class="sxs-lookup"><span data-stu-id="de833-422">Changed `disk create` to allow specifying the exact size of the disk upload</span></span>
* <span data-ttu-id="de833-423">Ajout de la prise en charge des instantanés incrémentiels pour les disques managés à `snapshot create`</span><span class="sxs-lookup"><span data-stu-id="de833-423">Added support for incremental snapshots for managed disks to `snapshot create`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="de833-424">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="de833-424">Cosmos DB</span></span>

* <span data-ttu-id="de833-425">Ajout du paramètre `--type <key-type>` à la commande `cosmosdb keys list` pour afficher la clé, les clés en lecture seule ou les chaînes de connexion</span><span class="sxs-lookup"><span data-stu-id="de833-425">Added `--type <key-type>` parameter to `cosmosdb keys list` command to show key, read only keys or connection strings</span></span>
* <span data-ttu-id="de833-426">Ajout de la commande `cosmosdb keys regenerate`</span><span class="sxs-lookup"><span data-stu-id="de833-426">Added `cosmosdb keys regenerate` command</span></span>
* <span data-ttu-id="de833-427">[DÉPRÉCIATION] Dépréciation des commandes `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` et `cosmosdb list-read-only-keys`</span><span class="sxs-lookup"><span data-stu-id="de833-427">[DEPRECATED] Deprecated `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` and `cosmosdb list-read-only-keys` commands</span></span>

### <a name="eventgrid"></a><span data-ttu-id="de833-428">EventGrid</span><span class="sxs-lookup"><span data-stu-id="de833-428">EventGrid</span></span>

* <span data-ttu-id="de833-429">Correction du texte d’aide du point de terminaison de manière à faire référence au bon paramètre</span><span class="sxs-lookup"><span data-stu-id="de833-429">Fixed the endpoint help text to refer to the right parameter</span></span>

### <a name="key-vault"></a><span data-ttu-id="de833-430">Key Vault</span><span class="sxs-lookup"><span data-stu-id="de833-430">Key Vault</span></span>

* <span data-ttu-id="de833-431">Résolution d’un problème de connexion avec un locataire (`login -t`) qui pouvait provoquer l’échec de `keyvault create`</span><span class="sxs-lookup"><span data-stu-id="de833-431">Fixed issue where logging in with a tenant (`login -t`) could cause `keyvault create` to fail</span></span>

### <a name="monitor"></a><span data-ttu-id="de833-432">Moniteur</span><span class="sxs-lookup"><span data-stu-id="de833-432">Monitor</span></span>

* <span data-ttu-id="de833-433">Résolution d’un problème où le caractère `:` n’était pas autorisé dans l’argument `--condition` de `monitor metrics alert create`</span><span class="sxs-lookup"><span data-stu-id="de833-433">Fixed issue where `:` character was not allowed in `--condition` argument to `monitor metrics alert create`</span></span>

### <a name="policy"></a><span data-ttu-id="de833-434">Stratégie</span><span class="sxs-lookup"><span data-stu-id="de833-434">Policy</span></span>

* <span data-ttu-id="de833-435">Ajout de la prise en charge de l’API Policy version 2019-06-01</span><span class="sxs-lookup"><span data-stu-id="de833-435">Added support for Policy API version 2019-06-01</span></span>
* <span data-ttu-id="de833-436">Ajout du paramètre `--enforcement-mode` à la commande `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="de833-436">Added `--enforcement-mode` parameter to `policy assignment create` command</span></span>

### <a name="storage"></a><span data-ttu-id="de833-437">Stockage</span><span class="sxs-lookup"><span data-stu-id="de833-437">Storage</span></span>

* <span data-ttu-id="de833-438">Ajout du paramètre `--blob-type` à la commande `az storage copy`</span><span class="sxs-lookup"><span data-stu-id="de833-438">Added `--blob-type` parameter to `az storage copy` command</span></span>

## <a name="september-10-2019"></a><span data-ttu-id="de833-439">10 septembre 2019</span><span class="sxs-lookup"><span data-stu-id="de833-439">September 10, 2019</span></span>

### <a name="acr"></a><span data-ttu-id="de833-440">ACR</span><span class="sxs-lookup"><span data-stu-id="de833-440">ACR</span></span>

* <span data-ttu-id="de833-441">Ajout du groupe de commandes `acr config retention` pour configurer une stratégie de conservation</span><span class="sxs-lookup"><span data-stu-id="de833-441">Added command group `acr config retention` to configure retention policy</span></span>

### <a name="aks"></a><span data-ttu-id="de833-442">AKS</span><span class="sxs-lookup"><span data-stu-id="de833-442">AKS</span></span>

* <span data-ttu-id="de833-443">Ajout de la prise en charge de l’intégration ACR avec les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="de833-443">Added support for ACR integration with the following commands:</span></span>
  * <span data-ttu-id="de833-444">Ajout du paramètre `--attach-acr` à `aks [create|update]` pour attacher un ACR à un cluster AKS</span><span class="sxs-lookup"><span data-stu-id="de833-444">Added `--attach-acr` parameter to `aks [create|update]` to attach an ACR to an AKS cluster</span></span>
  * <span data-ttu-id="de833-445">Ajout du paramètre `--detach-acr` à `aks update` pour détacher l’ACR d’un cluster AKS</span><span class="sxs-lookup"><span data-stu-id="de833-445">Added `--detach-acr` parameter to `aks update` to detach the ACR from an AKS cluster</span></span>

### <a name="arm"></a><span data-ttu-id="de833-446">ARM</span><span class="sxs-lookup"><span data-stu-id="de833-446">ARM</span></span>

* <span data-ttu-id="de833-447">Mis à jour pour utiliser la version d’API 2019-05-10</span><span class="sxs-lookup"><span data-stu-id="de833-447">Updated to use API version 2019-05-10</span></span>

### <a name="batch"></a><span data-ttu-id="de833-448">Batch</span><span class="sxs-lookup"><span data-stu-id="de833-448">Batch</span></span>

* <span data-ttu-id="de833-449">Ajout de nouveaux paramètres de configuration JSON à `--json-file` pour `batch pool create` :</span><span class="sxs-lookup"><span data-stu-id="de833-449">Added new JSON configuration settings to `--json-file` for `batch pool create`:</span></span>
  * <span data-ttu-id="de833-450">Ajout de `MountConfigurations` pour les montages de système de fichiers (voir https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body pour les détails)</span><span class="sxs-lookup"><span data-stu-id="de833-450">Added `MountConfigurations` for file system mounts (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
  * <span data-ttu-id="de833-451">Ajout de la propriété facultative `publicIPs` sur `NetworkConfiguration` pour les adresses IP publiques sur les pools (voir https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body pour les détails)</span><span class="sxs-lookup"><span data-stu-id="de833-451">Added optional property `publicIPs` on `NetworkConfiguration` for public IPs on pools (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
* <span data-ttu-id="de833-452">Ajout de la prise en charge des galeries d’images partagées à `--image`</span><span class="sxs-lookup"><span data-stu-id="de833-452">Added support for shared image galleries to `--image`</span></span>
* <span data-ttu-id="de833-453">[CHANGEMENT CASSANT] Changement de la valeur par défaut `--start-task-wait-for-success` sur `batch pool create` qui devient `true`</span><span class="sxs-lookup"><span data-stu-id="de833-453">[BREAKING CHANGE] Changed default value of `--start-task-wait-for-success` on `batch pool create` to be `true`</span></span>
* <span data-ttu-id="de833-454">[CHANGEMENT CASSANT] Changement de la valeur par défaut pour `Scope` sur `AutoUserSpecification` pour qu’elle soit toujours Pool (était `Task` sur les nœuds Windows, `Pool` sur les nœuds Linux)</span><span class="sxs-lookup"><span data-stu-id="de833-454">[BREAKING CHANGE] Changed default value for `Scope` on `AutoUserSpecification` to always be Pool (was `Task` on Windows nodes, `Pool` on Linux nodes)</span></span>
  * <span data-ttu-id="de833-455">Cet argument ne peut être défini qu’à partir d’une configuration JSON avec `--json-file`</span><span class="sxs-lookup"><span data-stu-id="de833-455">This argument can only be set from a JSON configuration with `--json-file`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="de833-456">HDInsight</span><span class="sxs-lookup"><span data-stu-id="de833-456">HDInsight</span></span>

* <span data-ttu-id="de833-457">Version mise à la disposition générale</span><span class="sxs-lookup"><span data-stu-id="de833-457">GA release</span></span>
* <span data-ttu-id="de833-458">[CHANGEMENT CASSANT] Changement du paramètre `--workernode-count/-c` de `az hdinsight resize` pour le rendre obligatoire.</span><span class="sxs-lookup"><span data-stu-id="de833-458">[BREAKING CHANGE] Changed parameter `--workernode-count/-c` of `az hdinsight resize` to be required.</span></span>

### <a name="key-vault"></a><span data-ttu-id="de833-459">Key Vault</span><span class="sxs-lookup"><span data-stu-id="de833-459">Key Vault</span></span>

* <span data-ttu-id="de833-460">Résolution d’un problème où les sous-réseaux ne pouvaient pas être supprimés des règles réseau</span><span class="sxs-lookup"><span data-stu-id="de833-460">Fixed issue where subnets couldn't be deleted from network rules</span></span>
* <span data-ttu-id="de833-461">Résolution d’un problème où des sous-réseaux et des adresses IP dupliqués pouvaient être ajoutés aux règles réseau</span><span class="sxs-lookup"><span data-stu-id="de833-461">Fixed issue where duplicated subnets and IP addresses could be added to network rules</span></span>

### <a name="network"></a><span data-ttu-id="de833-462">Réseau</span><span class="sxs-lookup"><span data-stu-id="de833-462">Network</span></span>

* <span data-ttu-id="de833-463">Ajout du paramètre `--interval` à `network watcher flow-log` pour définir la valeur d’intervalle de l’analyse du trafic</span><span class="sxs-lookup"><span data-stu-id="de833-463">Added `--interval` parameter to `network watcher flow-log` to set traffic analysis interval value</span></span>
* <span data-ttu-id="de833-464">Ajout de `network application-gateway identity` pour gérer l’identité de la passerelle</span><span class="sxs-lookup"><span data-stu-id="de833-464">Added `network application-gateway identity` to manage gateway identity</span></span>
* <span data-ttu-id="de833-465">Ajout de la prise en charge de la définition de l’ID Key Vault sur `network application-gateway ssl-cert`</span><span class="sxs-lookup"><span data-stu-id="de833-465">Added support for setting Key Vault ID to `network application-gateway ssl-cert`</span></span>
* <span data-ttu-id="de833-466">Ajout de `network express-route peering peer-connection [show|list]`</span><span class="sxs-lookup"><span data-stu-id="de833-466">Added `network express-route peering peer-connection [show|list]`</span></span>

### <a name="policy"></a><span data-ttu-id="de833-467">Stratégie</span><span class="sxs-lookup"><span data-stu-id="de833-467">Policy</span></span>

* <span data-ttu-id="de833-468">Mis à jour pour utiliser la version d’API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="de833-468">Updated to use API version 2019-01-01</span></span>

## <a name="august-27-2019"></a><span data-ttu-id="de833-469">27 août 2019</span><span class="sxs-lookup"><span data-stu-id="de833-469">August 27, 2019</span></span>

<span data-ttu-id="de833-470">Version 2.0.72</span><span class="sxs-lookup"><span data-stu-id="de833-470">Version 2.0.72</span></span>

### <a name="acr"></a><span data-ttu-id="de833-471">ACR</span><span class="sxs-lookup"><span data-stu-id="de833-471">ACR</span></span>

* <span data-ttu-id="de833-472">[CHANGEMENT CASSANT] Suppression de la prise en charge de la référence SKU `classic`</span><span class="sxs-lookup"><span data-stu-id="de833-472">[BREAKING CHANGE] Removed support for the `classic` SKU</span></span>

### <a name="api-management"></a><span data-ttu-id="de833-473">Gestion des API</span><span class="sxs-lookup"><span data-stu-id="de833-473">API Management</span></span>

* <span data-ttu-id="de833-474">[PRÉVERSION] Ajout du groupe de commandes `apim`</span><span class="sxs-lookup"><span data-stu-id="de833-474">[PREVIEW] Added `apim` command group</span></span>

### <a name="appservice"></a><span data-ttu-id="de833-475">AppService</span><span class="sxs-lookup"><span data-stu-id="de833-475">AppService</span></span>

* <span data-ttu-id="de833-476">Résolution du problème avec la commande `webapp webjob continuous start` lors de la spécification d’un emplacement</span><span class="sxs-lookup"><span data-stu-id="de833-476">Fixed issue with `webapp webjob continuous start` command when specifying a slot</span></span>
* <span data-ttu-id="de833-477">Modification de `webapp up` pour détecter le dossier `env` et le supprimer du fichier utilisé pour le déploiement</span><span class="sxs-lookup"><span data-stu-id="de833-477">Changed `webapp up` to detect `env` folder and remove it from the file used for deployment</span></span>

### <a name="keyvault"></a><span data-ttu-id="de833-478">KeyVault</span><span class="sxs-lookup"><span data-stu-id="de833-478">Keyvault</span></span>

* <span data-ttu-id="de833-479">Correction d’un bogue dans `keyvault secret set` qui ignorait l’argument `--expires`</span><span class="sxs-lookup"><span data-stu-id="de833-479">Fixed a bug in `keyvault secret set` that igored the `--expires` argument</span></span>

### <a name="network"></a><span data-ttu-id="de833-480">Réseau</span><span class="sxs-lookup"><span data-stu-id="de833-480">Network</span></span>

* <span data-ttu-id="de833-481">Ajout de la prise en charge des adresses IPv6 pour les arguments `--private-ip-address-version`</span><span class="sxs-lookup"><span data-stu-id="de833-481">Added support for IPv6 addresses to `--private-ip-address-version` arguments</span></span>
* <span data-ttu-id="de833-482">Ajout des nouvelles commandes `network private-endpoint [create|update|list-types]` pour la gestion des points de terminaison privés</span><span class="sxs-lookup"><span data-stu-id="de833-482">Added new commands `network private-endpoint [create|update|list-types]` for private endpoint management</span></span>
* <span data-ttu-id="de833-483">Ajout du groupe de commandes `network private-link-service`</span><span class="sxs-lookup"><span data-stu-id="de833-483">Added command group `network private-link-service`</span></span>
* <span data-ttu-id="de833-484">Ajout des arguments `--private-endpoint-network-policies` et `--private-link-service-network-policies` à `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="de833-484">Added `--private-endpoint-network-policies` and `--private-link-service-network-policies` arguments to `network vnet subnet update`</span></span>

### <a name="rbac"></a><span data-ttu-id="de833-485">RBAC</span><span class="sxs-lookup"><span data-stu-id="de833-485">RBAC</span></span>

* <span data-ttu-id="de833-486">Correction du problème `ad app update --homepage` où la page d’accueil ne se mettait pas à jour</span><span class="sxs-lookup"><span data-stu-id="de833-486">Fixed issue with `ad app update --homepage` where homepage would not be updated</span></span>

### <a name="servicefabric"></a><span data-ttu-id="de833-487">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="de833-487">ServiceFabric</span></span>

* <span data-ttu-id="de833-488">Ajout de la prise en charge pour les noms Key Vault en casse mixte</span><span class="sxs-lookup"><span data-stu-id="de833-488">Added support for mixed-case Key Vault names</span></span>
* <span data-ttu-id="de833-489">Résolution du problème lors de l’utilisation de certificats dans Key Vault</span><span class="sxs-lookup"><span data-stu-id="de833-489">Fixed issue when using certificates in Key Vault</span></span>
* <span data-ttu-id="de833-490">Résolution du problème lors de l’utilisation des fichiers de certificat PFX</span><span class="sxs-lookup"><span data-stu-id="de833-490">Fixed issue with using PFX certificate files</span></span>
* <span data-ttu-id="de833-491">Correction du problème avec `sf cluster certificate add` quand le groupe de ressources Key Vault n’était pas spécifié</span><span class="sxs-lookup"><span data-stu-id="de833-491">Fixed issue with `sf cluster certificate add` when Key Vault resource group wasn't specified</span></span>
* <span data-ttu-id="de833-492">Correction du problème où `sf cluster set` ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="de833-492">Fixed issue with `sf cluster set` not working</span></span>

### <a name="signalr"></a><span data-ttu-id="de833-493">SignalR</span><span class="sxs-lookup"><span data-stu-id="de833-493">SignalR</span></span>

* <span data-ttu-id="de833-494">Ajout de nouvelles commandes :</span><span class="sxs-lookup"><span data-stu-id="de833-494">Added new commands:</span></span>
  * <span data-ttu-id="de833-495">`signalr cors`: Gérer SignalR CORS</span><span class="sxs-lookup"><span data-stu-id="de833-495">`signalr cors`: Manage SignalR CORS</span></span>
  * <span data-ttu-id="de833-496">`signalr restart`: Redémarrer un service SignalR</span><span class="sxs-lookup"><span data-stu-id="de833-496">`signalr restart`: Restart a SignalR service</span></span>
  * <span data-ttu-id="de833-497">`signalr update`: Mettre à jour un service SignalR</span><span class="sxs-lookup"><span data-stu-id="de833-497">`signalr update`: Update a SignalR service</span></span>
* <span data-ttu-id="de833-498">Ajout de l’argument `--service-mode` à `signalr create`</span><span class="sxs-lookup"><span data-stu-id="de833-498">Added `--service-mode` argument to `signalr create`</span></span>

### <a name="storage"></a><span data-ttu-id="de833-499">Stockage</span><span class="sxs-lookup"><span data-stu-id="de833-499">Storage</span></span>

* <span data-ttu-id="de833-500">Ajout de la commande `storage account revoke-delegation-keys`</span><span class="sxs-lookup"><span data-stu-id="de833-500">Added `storage account revoke-delegation-keys` command</span></span>

## <a name="august-13-2019"></a><span data-ttu-id="de833-501">13 août 2019</span><span class="sxs-lookup"><span data-stu-id="de833-501">August 13, 2019</span></span>

<span data-ttu-id="de833-502">Version 2.0.71</span><span class="sxs-lookup"><span data-stu-id="de833-502">Version 2.0.71</span></span>

### <a name="appservice"></a><span data-ttu-id="de833-503">AppService</span><span class="sxs-lookup"><span data-stu-id="de833-503">AppService</span></span>

* <span data-ttu-id="de833-504">Correction d’un problème entraînant l’échec des commandes `webapp webjob continuous` pour les emplacements</span><span class="sxs-lookup"><span data-stu-id="de833-504">Fixed issue where `webapp webjob continuous` commands were failing for slots</span></span>

### <a name="botservice"></a><span data-ttu-id="de833-505">BotService</span><span class="sxs-lookup"><span data-stu-id="de833-505">BotService</span></span>

* <span data-ttu-id="de833-506">[CHANGEMENT CASSANT] Suppression de la prise en charge de la création de bots SDK v3</span><span class="sxs-lookup"><span data-stu-id="de833-506">[BREAKING CHANGE] Removed support for creating v3 SDK bots</span></span>

### <a name="cognitiveservices"></a><span data-ttu-id="de833-507">CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="de833-507">CognitiveServices</span></span>

* <span data-ttu-id="de833-508">Ajout des commandes `cognitiveservices account network-rule`</span><span class="sxs-lookup"><span data-stu-id="de833-508">Added `cognitiveservices account network-rule` commands</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="de833-509">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="de833-509">Cosmos DB</span></span>

* <span data-ttu-id="de833-510">Suppression de l’avertissement lors de la mise à jour de plusieurs emplacements d’écriture</span><span class="sxs-lookup"><span data-stu-id="de833-510">Removed warning when updating multiple write locations</span></span>
* <span data-ttu-id="de833-511">Ajout de commandes CRUD pour les ressources CosmosDB SQL, MongoDB, Cassandra, Gremlin et Table et le débit de la ressource</span><span class="sxs-lookup"><span data-stu-id="de833-511">Added CRUD commands for CosmosDB SQL, MongoDB, Cassandra, Gremlin and Table resources and resource's throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="de833-512">HDInsight</span><span class="sxs-lookup"><span data-stu-id="de833-512">HDInsight</span></span>

<span data-ttu-id="de833-513">Cette version contient un grand nombre de modifications conséquentes.</span><span class="sxs-lookup"><span data-stu-id="de833-513">This release contains a large number of breaking changes.</span></span>

* <span data-ttu-id="de833-514">[CHANGEMENT CASSANT] Renommage des paramètres pour `hdinsight create` :</span><span class="sxs-lookup"><span data-stu-id="de833-514">[BREAKING CHANGE] Renamed parameters for `hdinsight create`:</span></span>
  * <span data-ttu-id="de833-515">`--storage-default-container` renommé en `--storage-container`</span><span class="sxs-lookup"><span data-stu-id="de833-515">Renamed `--storage-default-container` to `--storage-container`</span></span>
  * <span data-ttu-id="de833-516">`--storage-default-filesystem` renommé en `--storage-filesystem`</span><span class="sxs-lookup"><span data-stu-id="de833-516">Renamed `--storage-default-filesystem` to `--storage-filesystem`</span></span>
* <span data-ttu-id="de833-517">[CHANGEMENT CASSANT] Modification de l’argument `--name` de `application create` pour représenter le nom de l’application à la place du nom du cluster</span><span class="sxs-lookup"><span data-stu-id="de833-517">[BREAKING CHANGE] Changed the `--name` argument of `application create` to represent the application name instead of the cluster name</span></span>
* <span data-ttu-id="de833-518">Ajout d’un argument `--cluster-name` à `application create` pour remplacer l’ancienne fonctionnalité `--name`</span><span class="sxs-lookup"><span data-stu-id="de833-518">Added `--cluster-name` argument to `application create` to replace old `--name` functionality</span></span>
* <span data-ttu-id="de833-519">[CHANGEMENT CASSANT] Renommage des paramètres pour `application create` :</span><span class="sxs-lookup"><span data-stu-id="de833-519">[BREAKING CHANGE] Renamed parameters for `application create`:</span></span>
  * <span data-ttu-id="de833-520">`--application-type` renommé en `--type`</span><span class="sxs-lookup"><span data-stu-id="de833-520">Renamed `--application-type` to `--type`</span></span>
  * <span data-ttu-id="de833-521">`--marketplace-identifier` renommé en `--marketplace-id`</span><span class="sxs-lookup"><span data-stu-id="de833-521">Renamed `--marketplace-identifier` to `--marketplace-id`</span></span>
  * <span data-ttu-id="de833-522">`--https-endpoint-access-mode` renommé en `--access-mode`</span><span class="sxs-lookup"><span data-stu-id="de833-522">Renamed `--https-endpoint-access-mode` to `--access-mode`</span></span>
  * <span data-ttu-id="de833-523">`--https-endpoint-destination-port` renommé en `--destination-port`</span><span class="sxs-lookup"><span data-stu-id="de833-523">Renamed  `--https-endpoint-destination-port` to `--destination-port`</span></span>
* <span data-ttu-id="de833-524">[CHANGEMENT CASSANT] Suppression des paramètres pour `application create` :</span><span class="sxs-lookup"><span data-stu-id="de833-524">[BREAKING CHANGE] Removed parameters for `application create`:</span></span>
  * `--https-endpoint-location`
  * `--https-endpoint-public-port`
  * `--ssh-endpoint-destination-port`
  * `--ssh-endpoint-location`
  * `--ssh-endpoint-public-port`
* <span data-ttu-id="de833-525">MODIFICATION CONSÉQUENTE Renommage de `--target-instance-count` en `--workernode-count` pour `hdinsight resize`</span><span class="sxs-lookup"><span data-stu-id="de833-525">[BREAKING CHNAGE] Renamed `--target-instance-count` to `--workernode-count` for `hdinsight resize`</span></span>
* <span data-ttu-id="de833-526">[CHANGEMENT CASSANT] Modification de toutes les commandes du groupe `hdinsight script-action` pour utiliser le paramètre `--name` comme nom de l’action de script.</span><span class="sxs-lookup"><span data-stu-id="de833-526">[BREAKING CHANGE] Changed all commands in the `hdinsight script-action` group to use the `--name` parameter as the name of the script action.</span></span>
* <span data-ttu-id="de833-527">Ajout d’un argument `--cluster-name` à toutes les commandes `hdinsight script-action` pour remplacer l’ancienne fonctionnalité `--name`</span><span class="sxs-lookup"><span data-stu-id="de833-527">Added `--cluster-name` argument to all `hdinsight script-action` commands to replace old `--name` functionality</span></span>
* <span data-ttu-id="de833-528">[CHANGEMENT CASSANT] Renommage de l’option `--script-execution-id` en `--execution-id` pour toutes les commandes `hdinsight script-action`</span><span class="sxs-lookup"><span data-stu-id="de833-528">[BREAKING CHANGE] Renamed `--script-execution-id` to `--execution-id` for all `hdinsight script-action` commands</span></span>
* <span data-ttu-id="de833-529">[CHANGEMENT CASSANT] Renommage de `hdinsight script-action show` en `hdinsight script-action show-execution-details`</span><span class="sxs-lookup"><span data-stu-id="de833-529">[BREAKING CHANGE] Renamed `hdinsight script-action show` to `hdinsight script-action show-execution-details`</span></span>
* <span data-ttu-id="de833-530">[MODIFICATION CONSÉQUENTE] Modification des paramètres sur `hdinsight script-action execute --roles` pour qu’ils soient séparés par des espaces et non par des virgules</span><span class="sxs-lookup"><span data-stu-id="de833-530">[BREAKING CHNAGE] Changed parameters to `hdinsight script-action execute --roles` to be space-separated instead of comma-separated</span></span>
* <span data-ttu-id="de833-531">[CHANGEMENT CASSANT] Suppression du paramètre `--persisted` de `hdinsight script-action list`</span><span class="sxs-lookup"><span data-stu-id="de833-531">[BREAKING CHANGE] Removed the `--persisted` parameter of `hdinsight script-action list`</span></span>
* <span data-ttu-id="de833-532">Modification du paramètre `hdinsight create --cluster-configurations` pour qu’il accepte un chemin d’accès à un fichier JSON local ou une chaîne JSON</span><span class="sxs-lookup"><span data-stu-id="de833-532">Changed the `hdinsight create --cluster-configurations` parameter to accept a path to a local JSON file or a JSON string</span></span>
* <span data-ttu-id="de833-533">Ajout de la commande `hdinsight script-action list-execution-history`</span><span class="sxs-lookup"><span data-stu-id="de833-533">Added command `hdinsight script-action list-execution-history`</span></span>
* <span data-ttu-id="de833-534">Modification de `hdinsight monitor enable --workspace` pour qu’il accepte un ID ou un nom d’espace de travail Log Analytics</span><span class="sxs-lookup"><span data-stu-id="de833-534">Changed `hdinsight monitor enable --workspace` to accept a Log Analytics workspace ID or workspace name</span></span>
* <span data-ttu-id="de833-535">Ajout de l’argument `hdinsight monitor enable --primary-key`, qui est nécessaire si un ID d’espace de travail est fourni en tant que paramètre</span><span class="sxs-lookup"><span data-stu-id="de833-535">Added the `hdinsight monitor enable --primary-key` argument, which is needed if a workspace ID is provided as the parameter</span></span>
* <span data-ttu-id="de833-536">Ajout de plus d’exemples et mise à jour des descriptions des messages d’aide</span><span class="sxs-lookup"><span data-stu-id="de833-536">Added more examples and updated descriptions for help messages</span></span>

### <a name="interactive"></a><span data-ttu-id="de833-537">Interactive</span><span class="sxs-lookup"><span data-stu-id="de833-537">Interactive</span></span>

* <span data-ttu-id="de833-538">Résolution d’une erreur de chargement</span><span class="sxs-lookup"><span data-stu-id="de833-538">Fixed a loading error</span></span>

### <a name="kubernetes"></a><span data-ttu-id="de833-539">Kubernetes</span><span class="sxs-lookup"><span data-stu-id="de833-539">Kubernetes</span></span>

* <span data-ttu-id="de833-540">Modification pour utiliser `https` si le port du conteneur du tableau de bord utilise `https`</span><span class="sxs-lookup"><span data-stu-id="de833-540">Changed to use `https` if dashboard container port is using `https`</span></span>

### <a name="network"></a><span data-ttu-id="de833-541">Réseau</span><span class="sxs-lookup"><span data-stu-id="de833-541">Network</span></span>

* <span data-ttu-id="de833-542">Ajout de l’argument `--yes``network dns record-set cname delete`</span><span class="sxs-lookup"><span data-stu-id="de833-542">Added `--yes` argument `network dns record-set cname delete`</span></span>

### <a name="profile"></a><span data-ttu-id="de833-543">Profil</span><span class="sxs-lookup"><span data-stu-id="de833-543">Profile</span></span>

* <span data-ttu-id="de833-544">Ajout de l’argument `--resource-type` à `account get-access-token` pour obtenir des jetons d’accès aux ressources</span><span class="sxs-lookup"><span data-stu-id="de833-544">Added `--resource-type` argument to `account get-access-token` to get resource access tokens</span></span>

### <a name="servicefabric"></a><span data-ttu-id="de833-545">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="de833-545">ServiceFabric</span></span>

* <span data-ttu-id="de833-546">Ajout de toutes les versions de système d’exploitation prises en charge pour sf cluster create</span><span class="sxs-lookup"><span data-stu-id="de833-546">Added all supported os version for sf cluster create</span></span>
* <span data-ttu-id="de833-547">Résolution d’un bogue principal de validation de certificat</span><span class="sxs-lookup"><span data-stu-id="de833-547">Fixed primary certificate validation bug</span></span>

### <a name="storage"></a><span data-ttu-id="de833-548">Stockage</span><span class="sxs-lookup"><span data-stu-id="de833-548">Storage</span></span>

* <span data-ttu-id="de833-549">Ajout de la commande `storage copy`</span><span class="sxs-lookup"><span data-stu-id="de833-549">Added command `storage copy`</span></span>

## <a name="july-30-2019"></a><span data-ttu-id="de833-550">30 juillet 2019</span><span class="sxs-lookup"><span data-stu-id="de833-550">July 30, 2019</span></span>

<span data-ttu-id="de833-551">Version 2.0.70</span><span class="sxs-lookup"><span data-stu-id="de833-551">Version 2.0.70</span></span>

### <a name="acr"></a><span data-ttu-id="de833-552">ACR</span><span class="sxs-lookup"><span data-stu-id="de833-552">ACR</span></span>

* <span data-ttu-id="de833-553">Correction du problème #9952 (régression dans la commande `acr pack build`)</span><span class="sxs-lookup"><span data-stu-id="de833-553">Fixed issue #9952 (a regression in the `acr pack build` command)</span></span>
* <span data-ttu-id="de833-554">Suppression du nom de l’image du générateur par défaut dans `acr pack build`</span><span class="sxs-lookup"><span data-stu-id="de833-554">Removed the default builder image name in `acr pack build`</span></span>

### <a name="appservice"></a><span data-ttu-id="de833-555">AppService</span><span class="sxs-lookup"><span data-stu-id="de833-555">Appservice</span></span>

* <span data-ttu-id="de833-556">Modification de `webapp config ssl` pour afficher un message si une ressource est introuvable</span><span class="sxs-lookup"><span data-stu-id="de833-556">Changed `webapp config ssl` to show a message if a resource is not found</span></span>
* <span data-ttu-id="de833-557">Correction du problème où `functionapp create` n’acceptait pas le type de compte de stockage `Standard_RAGRS`</span><span class="sxs-lookup"><span data-stu-id="de833-557">Fixed issue where `functionapp create` does not accept `Standard_RAGRS` storage account type</span></span>
* <span data-ttu-id="de833-558">Correction d’un problème où `webapp up` échouait s’il était exécuté avec des versions antérieures de Python</span><span class="sxs-lookup"><span data-stu-id="de833-558">Fixed an issue where `webapp up` would fail if run using older versions of python</span></span>

### <a name="network"></a><span data-ttu-id="de833-559">Réseau</span><span class="sxs-lookup"><span data-stu-id="de833-559">Network</span></span>

* <span data-ttu-id="de833-560">Suppression du paramètre non valide `--ids` de `network nic ip-config add` (correctifs #9861)</span><span class="sxs-lookup"><span data-stu-id="de833-560">Removed invalid parameter `--ids` from `network nic ip-config add` (fixes #9861)</span></span>
* <span data-ttu-id="de833-561">Correctifs #9604.</span><span class="sxs-lookup"><span data-stu-id="de833-561">Fixes #9604.</span></span> <span data-ttu-id="de833-562">Ajout du paramètre `--root-certs` à `network application-gateway http-settings [create|update]` pour prendre en charge les certificats racines approuvés associés à l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="de833-562">Added `--root-certs` parameter to `network application-gateway http-settings [create|update]` to support user associate trusted root certificates.</span></span>
* <span data-ttu-id="de833-563">Correction de l’argument `--subscription` pour `network dns record-set ns create` (#9965)</span><span class="sxs-lookup"><span data-stu-id="de833-563">Fixed arguent `--subscription` for `network dns record-set ns create` (#9965)</span></span>

### <a name="rbac"></a><span data-ttu-id="de833-564">RBAC</span><span class="sxs-lookup"><span data-stu-id="de833-564">RBAC</span></span>

* <span data-ttu-id="de833-565">Ajout de la commande `user update`</span><span class="sxs-lookup"><span data-stu-id="de833-565">Added `user update` command</span></span>
* <span data-ttu-id="de833-566">[DÉPRÉCIATION] Dépréciation de `--upn-or-object-id` des commandes associées à l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="de833-566">[DEPRECATED] Deprecated `--upn-or-object-id` from user-related commands</span></span>
    * <span data-ttu-id="de833-567">Utiliser l’argument de remplacement `--id`</span><span class="sxs-lookup"><span data-stu-id="de833-567">Use replacement argument `--id`</span></span>
* <span data-ttu-id="de833-568">Ajout de l’argument `--id` aux commandes associées à l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="de833-568">Added `--id` argument to user-related commands</span></span>

### <a name="sql"></a><span data-ttu-id="de833-569">SQL</span><span class="sxs-lookup"><span data-stu-id="de833-569">SQL</span></span>

* <span data-ttu-id="de833-570">Ajout de commandes de gestion pour les clés d’instance managée et le protecteur TDE</span><span class="sxs-lookup"><span data-stu-id="de833-570">Added management commands for managed instance keys and TDE protector</span></span>

### <a name="storage"></a><span data-ttu-id="de833-571">Stockage</span><span class="sxs-lookup"><span data-stu-id="de833-571">Storage</span></span>

* <span data-ttu-id="de833-572">Ajout de la commande `storage remove`</span><span class="sxs-lookup"><span data-stu-id="de833-572">Added `storage remove` command</span></span>
* <span data-ttu-id="de833-573">Correction d’un problème avec `storage blob update`</span><span class="sxs-lookup"><span data-stu-id="de833-573">Fixed an issue with `storage blob update`</span></span>

### <a name="vm"></a><span data-ttu-id="de833-574">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="de833-574">VM</span></span>

* <span data-ttu-id="de833-575">Changement de `list-skus` pour utiliser une version API plus récente dans les détails de la zone de sortie</span><span class="sxs-lookup"><span data-stu-id="de833-575">Changed `list-skus` to use newer api-version to output zone details</span></span>
* <span data-ttu-id="de833-576">Remplacement de la valeur par défaut `--single-placement-group` par `false` pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="de833-576">Changed default of `--single-placement-group` to `false` for `vmss create`</span></span>
* <span data-ttu-id="de833-577">Ajout de la possibilité de sélectionner des références SKU de stockage ZRS pour `[snapshot|disk] create`</span><span class="sxs-lookup"><span data-stu-id="de833-577">Added ability to select ZRS storage SKUs for `[snapshot|disk] create`</span></span>
* <span data-ttu-id="de833-578">Ajout d’un nouveau groupe de commandes `vm host` pour prendre en charge des hôtes dédiés</span><span class="sxs-lookup"><span data-stu-id="de833-578">Added new command group `vm host` to support dedicated hosts</span></span>
* <span data-ttu-id="de833-579">Ajout des paramètres `--host` et `--host-group` sur `vm create` pour définir l’hôte dédié à la machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="de833-579">Added parameters `--host` and `--host-group` on `vm create` to set VM dedicated host</span></span>

## <a name="july-16-2019"></a><span data-ttu-id="de833-580">16 juillet 2019</span><span class="sxs-lookup"><span data-stu-id="de833-580">July 16, 2019</span></span>

<span data-ttu-id="de833-581">Version 2.0.69</span><span class="sxs-lookup"><span data-stu-id="de833-581">Version 2.0.69</span></span>

### <a name="appservice"></a><span data-ttu-id="de833-582">AppService</span><span class="sxs-lookup"><span data-stu-id="de833-582">Appservice</span></span>

* <span data-ttu-id="de833-583">Changement des commandes `webapp identity` pour retourner un message d’erreur approprié si le nom de ResourceGroupName ou de l’application n’est pas valide</span><span class="sxs-lookup"><span data-stu-id="de833-583">Changed `webapp identity` commands to return a proper error message if ResourceGroupName or App name are invalid</span></span>
* <span data-ttu-id="de833-584">Correction de `webapp list` pour retourner la valeur correcte pour le nombre de sites si aucun groupe de ressources n’a été fourni</span><span class="sxs-lookup"><span data-stu-id="de833-584">Fixed `webapp list` to return the correct value for numberOfSites if no ResourceGroup was provided</span></span>
* <span data-ttu-id="de833-585">Correction des effets secondaires de `appservice plan create` et de `webapp create`</span><span class="sxs-lookup"><span data-stu-id="de833-585">Fixed side-effects of `appservice plan create` and `webapp create`</span></span>

### <a name="core"></a><span data-ttu-id="de833-586">Core</span><span class="sxs-lookup"><span data-stu-id="de833-586">Core</span></span>

* <span data-ttu-id="de833-587">Résolution du problème où `--subscription` s’affichait alors qu’il ne devait pas</span><span class="sxs-lookup"><span data-stu-id="de833-587">Fixed issue where `--subscription` would appear despite being not applicable</span></span>

### <a name="batch"></a><span data-ttu-id="de833-588">Batch</span><span class="sxs-lookup"><span data-stu-id="de833-588">Batch</span></span>

* <span data-ttu-id="de833-589">[CHANGEMENT CASSANT] Remplacement de `batch pool node-agent-skus list` par `batch pool supported-images list`</span><span class="sxs-lookup"><span data-stu-id="de833-589">[BREAKING CHANGE] Replaced `batch pool node-agent-skus list` with `batch pool supported-images list`</span></span>
* <span data-ttu-id="de833-590">Ajout de la prise en charge des règles de sécurité bloquant l’accès réseau à un pool basé sur le port source du trafic lors de l’utilisation de l’option `--json-file` de `batch pool create network`</span><span class="sxs-lookup"><span data-stu-id="de833-590">Added support for security rules blocking network access to a pool based on the source port of the traffic when using the `--json-file` option of `batch pool create network`</span></span>
* <span data-ttu-id="de833-591">Ajout de la prise en charge de l’exécution de la tâche dans le répertoire de travail du conteneur ou dans le répertoire de travail de la tâche Batch lors de l’utilisation de l’option `--json-file` de `batch task create`</span><span class="sxs-lookup"><span data-stu-id="de833-591">Added support for executing the task in the container working directory or in the Batch task working directory when using the `--json-file` option of `batch task create`</span></span>
* <span data-ttu-id="de833-592">Correction d’une erreur dans l’option `--application-package-references` de `batch pool create` où elle fonctionnait uniquement avec les valeurs par défaut</span><span class="sxs-lookup"><span data-stu-id="de833-592">Fixed error in `--application-package-references` option of `batch pool create` where it would only work with defaults</span></span>

### <a name="eventhubs"></a><span data-ttu-id="de833-593">Eventhubs</span><span class="sxs-lookup"><span data-stu-id="de833-593">Eventhubs</span></span>

* <span data-ttu-id="de833-594">Ajout d’une validation pour le paramètre `--rights` des commandes `authorizationrule`</span><span class="sxs-lookup"><span data-stu-id="de833-594">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="rdbms"></a><span data-ttu-id="de833-595">SGBDR</span><span class="sxs-lookup"><span data-stu-id="de833-595">RDBMS</span></span>

* <span data-ttu-id="de833-596">Ajout d’un paramètre facultatif pour spécifier la référence SKU de réplica pour la commande de création de réplica</span><span class="sxs-lookup"><span data-stu-id="de833-596">Added optional parameter to specify replica SKU for create replica command</span></span>
* <span data-ttu-id="de833-597">Correction d’un problème d’échec des tests CI lors de la création du réplica MySQL</span><span class="sxs-lookup"><span data-stu-id="de833-597">Fixed the issue with CI test failure with creating MySQL replica</span></span>

### <a name="relay"></a><span data-ttu-id="de833-598">Relais</span><span class="sxs-lookup"><span data-stu-id="de833-598">Relay</span></span>

* <span data-ttu-id="de833-599">Correction d’un problème de connexion hybride quand l’autorisation du client est désactivée [#8775](https://github.com/azure/azure-cli/issues/8775)</span><span class="sxs-lookup"><span data-stu-id="de833-599">Fixed issue with hybrid connection when client authroization disabled [#8775](https://github.com/azure/azure-cli/issues/8775)</span></span>
* <span data-ttu-id="de833-600">Ajout du paramètre `--requires-transport-security` à `relay wcfrelay create`</span><span class="sxs-lookup"><span data-stu-id="de833-600">Added parameter `--requires-transport-security` to `relay wcfrelay create`</span></span>

### <a name="servicebus"></a><span data-ttu-id="de833-601">Servicebus</span><span class="sxs-lookup"><span data-stu-id="de833-601">Servicebus</span></span>

* <span data-ttu-id="de833-602">Ajout d’une validation pour le paramètre `--rights` des commandes `authorizationrule`</span><span class="sxs-lookup"><span data-stu-id="de833-602">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="storage"></a><span data-ttu-id="de833-603">Stockage</span><span class="sxs-lookup"><span data-stu-id="de833-603">Storage</span></span>

* <span data-ttu-id="de833-604">Activation des fichiers AADDS pour la mise à jour du compte de stockage</span><span class="sxs-lookup"><span data-stu-id="de833-604">Enable Files AADDS for storage account update</span></span>
* <span data-ttu-id="de833-605">Problème résolu `storage blob service-properties update --set`</span><span class="sxs-lookup"><span data-stu-id="de833-605">Fixed issue `storage blob service-properties update --set`</span></span>

## <a name="july-2-2019"></a><span data-ttu-id="de833-606">2 juillet 2019</span><span class="sxs-lookup"><span data-stu-id="de833-606">July 2, 2019</span></span>

<span data-ttu-id="de833-607">Version 2.0.68</span><span class="sxs-lookup"><span data-stu-id="de833-607">Version 2.0.68</span></span>

### <a name="core"></a><span data-ttu-id="de833-608">Core</span><span class="sxs-lookup"><span data-stu-id="de833-608">Core</span></span>

* <span data-ttu-id="de833-609">Les modules de commande sont désormais consolidés en un seul distribuable Python.</span><span class="sxs-lookup"><span data-stu-id="de833-609">Command modules are now consolidated into a single Python distributable.</span></span> <span data-ttu-id="de833-610">L’utilisation directe de nombreux packages `azure-cli-` sur PyPI est donc dépréciée.</span><span class="sxs-lookup"><span data-stu-id="de833-610">This deprecates direct use of many `azure-cli-` packages on PyPI.</span></span>
  <span data-ttu-id="de833-611">Cela doit réduire la taille de l’installation et affecter uniquement les utilisateurs ayant procédé à une installation directe par le biais de `pip`.</span><span class="sxs-lookup"><span data-stu-id="de833-611">This should reduce install size and only affect users who have directly installed via `pip`.</span></span>

### <a name="acr"></a><span data-ttu-id="de833-612">ACR</span><span class="sxs-lookup"><span data-stu-id="de833-612">ACR</span></span>

* <span data-ttu-id="de833-613">Ajout de la prise en charge des déclencheurs de minuteur à la tâche</span><span class="sxs-lookup"><span data-stu-id="de833-613">Added support for Timer Triggers to Task</span></span>

### <a name="appservice"></a><span data-ttu-id="de833-614">AppService</span><span class="sxs-lookup"><span data-stu-id="de833-614">Appservice</span></span>

* <span data-ttu-id="de833-615">Modification de `functionapp create` pour activer Application Insights par défaut</span><span class="sxs-lookup"><span data-stu-id="de833-615">Changed `functionapp create` to enable application insights by default</span></span>
* <span data-ttu-id="de833-616">[CHANGEMENT CASSANT] Suppression de la commande `functionapp devops-build` dépréciée.</span><span class="sxs-lookup"><span data-stu-id="de833-616">[BREAKING CHANGE] Removed deprecated `functionapp devops-build` command.</span></span>
  *  <span data-ttu-id="de833-617">Utilisez la nouvelle commande `az functionapp devops-pipeline` à la place</span><span class="sxs-lookup"><span data-stu-id="de833-617">Use the new command `az functionapp devops-pipeline` instead</span></span>
* <span data-ttu-id="de833-618">Ajout de la prise en charge du plan d’application de fonction Consommation Linux à `functionapp deployment config-zip`</span><span class="sxs-lookup"><span data-stu-id="de833-618">Added Linux Consumption function app plan support to `functionapp deployment config-zip`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="de833-619">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="de833-619">Cosmos DB</span></span>

* <span data-ttu-id="de833-620">Ajout de la prise en charge de la désactivation de TTL</span><span class="sxs-lookup"><span data-stu-id="de833-620">Added support for disabling TTL</span></span>

### <a name="dls"></a><span data-ttu-id="de833-621">DLS</span><span class="sxs-lookup"><span data-stu-id="de833-621">DLS</span></span>

* <span data-ttu-id="de833-622">Mise à jour de la version d’ADLS (0.0.45)</span><span class="sxs-lookup"><span data-stu-id="de833-622">Updated ADLS version (0.0.45)</span></span>

### <a name="feedback"></a><span data-ttu-id="de833-623">Commentaires</span><span class="sxs-lookup"><span data-stu-id="de833-623">Feedback</span></span>

* <span data-ttu-id="de833-624">Lors du signalement d’une commande d’extension ayant échoué, `az feedback` tente à présent d’ouvrir le navigateur à l’URL du projet/dépôt de l’extension à partir de l’index</span><span class="sxs-lookup"><span data-stu-id="de833-624">When reporting a failed extension command, `az feedback` now attempts to open the browser to the project/repo url of the extension from the index</span></span>

### <a name="hdinsight"></a><span data-ttu-id="de833-625">HDInsight</span><span class="sxs-lookup"><span data-stu-id="de833-625">HDInsight</span></span>

* <span data-ttu-id="de833-626">[CHANGEMENT CASSANT] Remplacement du nom du groupe de commandes `oms` par `monitor`</span><span class="sxs-lookup"><span data-stu-id="de833-626">[BREAKING CHANGE] Changed `oms` command group name to `monitor`</span></span>
* <span data-ttu-id="de833-627">[CHANGEMENT CASSANT] Paramètre `--http-password/-p` désormais obligatoire</span><span class="sxs-lookup"><span data-stu-id="de833-627">[BREAKING CHANGE] Made `--http-password/-p` a required parameter</span></span> 
* <span data-ttu-id="de833-628">Ajout de compléteurs pour le compléteur des paramètres `--cluster-admin-account` et `cluster-users-group-dns`</span><span class="sxs-lookup"><span data-stu-id="de833-628">Added completers for `--cluster-admin-account` and `cluster-users-group-dns` parameters completer</span></span> 
* <span data-ttu-id="de833-629">Paramètre `cluster-users-group-dns` désormais obligatoire quand `—esp` est présent</span><span class="sxs-lookup"><span data-stu-id="de833-629">Changed `cluster-users-group-dns` parameter to be required when `—esp` is present</span></span>
* <span data-ttu-id="de833-630">Ajout d’un délai d’expiration pour tous les compléteurs automatiques d’arguments existants</span><span class="sxs-lookup"><span data-stu-id="de833-630">Added a timeout for all existing argument auto-completers</span></span>
* <span data-ttu-id="de833-631">Ajout d’un délai d’expiration pour la transformation d’un nom de ressource en ID de ressource</span><span class="sxs-lookup"><span data-stu-id="de833-631">Added a timeout for transforming resource name to resource id</span></span>
* <span data-ttu-id="de833-632">Modification des compléteurs automatiques pour sélectionner des ressources à partir de n’importe quel groupe de ressources.</span><span class="sxs-lookup"><span data-stu-id="de833-632">Changed Auto-completers to select resources from any resource group.</span></span> <span data-ttu-id="de833-633">Le groupe de ressources peut être différent de celui spécifié avec `-g`</span><span class="sxs-lookup"><span data-stu-id="de833-633">It can be a different resource group than the one specified with `-g`</span></span>
* <span data-ttu-id="de833-634">Ajout de la prise en charge des paramètres `--sub-domain-suffix` et `--disable_gateway_auth` dans la commande `hdinsight application create`</span><span class="sxs-lookup"><span data-stu-id="de833-634">Added support for `--sub-domain-suffix` and `--disable_gateway_auth` parameters in the `hdinsight application create` command</span></span>

### <a name="managed-services"></a><span data-ttu-id="de833-635">Services gérés</span><span class="sxs-lookup"><span data-stu-id="de833-635">Managed Services</span></span>

* <span data-ttu-id="de833-636">Introduction du module de commande des services gérés en préversion</span><span class="sxs-lookup"><span data-stu-id="de833-636">Introducing managed service command module in preview</span></span>

### <a name="profile"></a><span data-ttu-id="de833-637">Profil</span><span class="sxs-lookup"><span data-stu-id="de833-637">Profile</span></span>
* <span data-ttu-id="de833-638">Suppression de l’argument `--subscription` pour la commande de déconnexion</span><span class="sxs-lookup"><span data-stu-id="de833-638">Suppress `--subscription` argument for logout command</span></span>

### <a name="rbac"></a><span data-ttu-id="de833-639">RBAC</span><span class="sxs-lookup"><span data-stu-id="de833-639">RBAC</span></span>

* <span data-ttu-id="de833-640">[CHANGEMENT CASSANT] Suppression de l’argument `--password` pour `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="de833-640">[BREAKING CHANGE] Removed `--password` argument for `create-for-rbac`</span></span>
* <span data-ttu-id="de833-641">Ajout du paramètre `--assignee-principal-type` à la commande `create` pour éviter les défaillances intermittentes dues à la latence de réplication du serveur de graphique AAD</span><span class="sxs-lookup"><span data-stu-id="de833-641">Added `--assignee-principal-type` parameter to `create` command to avoid intermittent failures caused by AAD graph server replication latency</span></span>
* <span data-ttu-id="de833-642">Correction d’un incident dans `ad signed-in-user` lors de l’énumération des objets détenus</span><span class="sxs-lookup"><span data-stu-id="de833-642">Fixed a crash in `ad signed-in-user` when listing owned objects</span></span>
* <span data-ttu-id="de833-643">Correction d’un incident lié au fait que `ad sp` ne trouve pas la bonne application à partir d’un principal de service</span><span class="sxs-lookup"><span data-stu-id="de833-643">Fixed issue where `ad sp` would not find the right application from a service principal</span></span>

### <a name="rdbms"></a><span data-ttu-id="de833-644">SGBDR</span><span class="sxs-lookup"><span data-stu-id="de833-644">RDBMS</span></span>

* <span data-ttu-id="de833-645">Ajout de la prise en charge de la réplication pour MariaDB</span><span class="sxs-lookup"><span data-stu-id="de833-645">Added support for replication for MariaDB</span></span>

### <a name="sql"></a><span data-ttu-id="de833-646">SQL</span><span class="sxs-lookup"><span data-stu-id="de833-646">SQL</span></span>

* <span data-ttu-id="de833-647">Valeurs autorisées documentées pour `sql db create --sample-name`</span><span class="sxs-lookup"><span data-stu-id="de833-647">Documented allowed values for `sql db create --sample-name`</span></span>

### <a name="storage"></a><span data-ttu-id="de833-648">Stockage</span><span class="sxs-lookup"><span data-stu-id="de833-648">Storage</span></span>

* <span data-ttu-id="de833-649">Ajout de la prise en charge des jetons SAS de délégation d’utilisateur avec `--as-user` à `storage blob generate-sas`</span><span class="sxs-lookup"><span data-stu-id="de833-649">Added user delegation SAS token support with `--as-user` to `storage blob generate-sas`</span></span> 
* <span data-ttu-id="de833-650">Ajout de la prise en charge des jetons SAS de délégation d’utilisateur avec `--as-user` à `storage container generate-sas`</span><span class="sxs-lookup"><span data-stu-id="de833-650">Added user delegation SAS token support with `--as-user` to `storage container generate-sas`</span></span> 

### <a name="vm"></a><span data-ttu-id="de833-651">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="de833-651">VM</span></span>

* <span data-ttu-id="de833-652">Correction d’un bogue contraignant `vmss create` à retourner un message d’erreur en cas d’exécution avec `--no-wait`</span><span class="sxs-lookup"><span data-stu-id="de833-652">Fixed bug where `vmss create` returns an error message when run with `--no-wait`</span></span>
* <span data-ttu-id="de833-653">Suppression de la validation côté client pour `vmss create --single-placement-group`.</span><span class="sxs-lookup"><span data-stu-id="de833-653">Removed client-side validation for `vmss create --single-placement-group`.</span></span> <span data-ttu-id="de833-654">N’échoue pas si `--single-placement-group` a la valeur `true` et si `--instance-count` est supérieur à 100 ou si des zones de disponibilité sont spécifiées, mais laisse cette validation au service de calcul</span><span class="sxs-lookup"><span data-stu-id="de833-654">Does not fail if `--single-placement-group` is set to `true` and`--instance-count` is greater than 100 or availability zones are specified, but leaves this validation to the compute service</span></span>
* <span data-ttu-id="de833-655">Correction d’un bogue entraînant l’échec de `[vm|vmss] extension image list` en cas d’utilisation avec `--latest`</span><span class="sxs-lookup"><span data-stu-id="de833-655">Fixed bug where `[vm|vmss] extension image list` fails when used with `--latest`</span></span>


## <a name="june-18-2019"></a><span data-ttu-id="de833-656">18 juin 2019</span><span class="sxs-lookup"><span data-stu-id="de833-656">June 18, 2019</span></span>

<span data-ttu-id="de833-657">Version 2.0.67</span><span class="sxs-lookup"><span data-stu-id="de833-657">Version 2.0.67</span></span>

### <a name="core"></a><span data-ttu-id="de833-658">Core</span><span class="sxs-lookup"><span data-stu-id="de833-658">Core</span></span>

<span data-ttu-id="de833-659">Cette version introduit une nouvelle étiquette [Préversion] qui permet d’indiquer plus clairement aux clients la présence d’un groupe de commandes, d’une commande ou d’un argument en préversion.</span><span class="sxs-lookup"><span data-stu-id="de833-659">This release introduces a new [Preview] tag to more clearly communicate to customers when a command group, command or argument is in preview status.</span></span> <span data-ttu-id="de833-660">Auparavant, cet état était mentionné dans le texte de l’aide ou communiqué implicitement par le numéro de version du module de commande.</span><span class="sxs-lookup"><span data-stu-id="de833-660">This was previously called out in help text or communicated implicitly by the command module version number.</span></span>
<span data-ttu-id="de833-661">À l’avenir, l’interface CLI supprimera les numéros de version des packages individuels.</span><span class="sxs-lookup"><span data-stu-id="de833-661">The CLI will be removing version numbers for individual packages in the future.</span></span> <span data-ttu-id="de833-662">Si une commande est en préversion, tous ses arguments le sont également.</span><span class="sxs-lookup"><span data-stu-id="de833-662">If a command is in preview, all of its arguments are as well.</span></span> <span data-ttu-id="de833-663">Si un groupe de commandes est étiqueté comme étant en préversion, toutes les commandes et tous les arguments sont également considérés comme étant en préversion.</span><span class="sxs-lookup"><span data-stu-id="de833-663">If a command group is labeled as being in preview, then all commands and arguments are considered to be in preview as well.</span></span>

<span data-ttu-id="de833-664">Conséquence de ce changement, plusieurs groupes de commandes peuvent « soudainement » apparaître comme étant en préversion avec cette version.</span><span class="sxs-lookup"><span data-stu-id="de833-664">As a result of this change, several command groups may seem to "suddenly" appear to be in a preview status with this release.</span></span> <span data-ttu-id="de833-665">En fait, la plupart des packages étaient en préversion, mais ils sont considérés comme étant dans un état de disponibilité générale avec cette version.</span><span class="sxs-lookup"><span data-stu-id="de833-665">What actually happened is that most packages were in a preview status, but are being deemed GA with this release</span></span>

### <a name="acr"></a><span data-ttu-id="de833-666">ACR</span><span class="sxs-lookup"><span data-stu-id="de833-666">ACR</span></span>
* <span data-ttu-id="de833-667">Ajout de la commande « acr check-health »</span><span class="sxs-lookup"><span data-stu-id="de833-667">Added 'acr check-health' command</span></span>
* <span data-ttu-id="de833-668">Amélioration de la gestion des erreurs pour les jetons AAD et pour la récupération des commandes externes</span><span class="sxs-lookup"><span data-stu-id="de833-668">Improved error handling for AAD tokens and for retrieving external commands</span></span>

### <a name="acs"></a><span data-ttu-id="de833-669">ACS</span><span class="sxs-lookup"><span data-stu-id="de833-669">ACS</span></span>
* <span data-ttu-id="de833-670">Les commandes ACS dépréciées sont désormais masquées de l’affichage de l’aide</span><span class="sxs-lookup"><span data-stu-id="de833-670">Deprecated ACS commands are now hidden from help view</span></span>

### <a name="ams"></a><span data-ttu-id="de833-671">AMS</span><span class="sxs-lookup"><span data-stu-id="de833-671">AMS</span></span>
* <span data-ttu-id="de833-672">[CHANGEMENT CASSANT] Changement apporté pour retourner les chaînes de temps ISO 8601 pour archive-window-length et key-frame-interval-duration</span><span class="sxs-lookup"><span data-stu-id="de833-672">[BREAKING CHANGE] Changed to return ISO 8601 time strings for archive-window-length and key-frame-interval-duration</span></span>

### <a name="appservice"></a><span data-ttu-id="de833-673">AppService</span><span class="sxs-lookup"><span data-stu-id="de833-673">AppService</span></span>
* <span data-ttu-id="de833-674">Ajout du routage basé sur l’emplacement pour `webapp deleted list` et `webapp deleted restore`</span><span class="sxs-lookup"><span data-stu-id="de833-674">Added location based routing for `webapp deleted list` and `webapp deleted restore`</span></span>
* <span data-ttu-id="de833-675">Correction d’un problème lié à l’impossibilité de cliquer sur l’URL cible journalisée d’une application web (« Vous pouvez lancer l’application... ») dans Azure Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="de833-675">Fixed issue where webapp up logged target URL ("You can launch the app at...") was not clickable in Azure Cloud Shell</span></span>
* <span data-ttu-id="de833-676">Correction d’un problème entraînant l’échec de la création d’applications avec certaines références SKU (erreur AlwaysOn)</span><span class="sxs-lookup"><span data-stu-id="de833-676">Fixed an issue where creating apps with the some SKUs was failing with an AlwaysOn error</span></span>
* <span data-ttu-id="de833-677">Ajout d’une fonction de prévalidation à `[appservice|webapp] create`</span><span class="sxs-lookup"><span data-stu-id="de833-677">Added pre-validation to `[appservice|webapp] create`</span></span>
* <span data-ttu-id="de833-678">Correction de `[webapp|functionapp] traffic-routing` de manière à utiliser le bon actionHostName</span><span class="sxs-lookup"><span data-stu-id="de833-678">Fixed `[webapp|functionapp] traffic-routing` to use the correct actionHostName</span></span>
* <span data-ttu-id="de833-679">Ajout de la prise en charge de l’emplacement aux commandes `functionapp`</span><span class="sxs-lookup"><span data-stu-id="de833-679">Added slot support to `functionapp` commands</span></span>

### <a name="batch"></a><span data-ttu-id="de833-680">Batch</span><span class="sxs-lookup"><span data-stu-id="de833-680">Batch</span></span>
* <span data-ttu-id="de833-681">Correction de la régression d’authentification AAD provoquée par un rapport d’erreur trop agressif pour l’authentification par clé partagée</span><span class="sxs-lookup"><span data-stu-id="de833-681">Fixed AAD auth regression caused by over-aggressive error reporting for Shared Key Auth</span></span>

### <a name="batchai"></a><span data-ttu-id="de833-682">Batch AI</span><span class="sxs-lookup"><span data-stu-id="de833-682">BatchAI</span></span>
* <span data-ttu-id="de833-683">Les commandes BatchAI sont maintenant dépréciées et masquées</span><span class="sxs-lookup"><span data-stu-id="de833-683">BatchAI commands are now deprecated and hidden</span></span>

### <a name="botservice"></a><span data-ttu-id="de833-684">BotService</span><span class="sxs-lookup"><span data-stu-id="de833-684">BotService</span></span>
* <span data-ttu-id="de833-685">Ajout de messages d’avertissement « support interrompu »/« mode maintenance » pour les commandes prenant en charge le SDK v3</span><span class="sxs-lookup"><span data-stu-id="de833-685">Added "discontinued support"/"maintenance mode" warning messages for commands that support the v3 SDK</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="de833-686">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="de833-686">CosmosDB</span></span>
* <span data-ttu-id="de833-687">[DÉPRÉCIATION] Dépréciation de la commande `cosmosdb list-keys`</span><span class="sxs-lookup"><span data-stu-id="de833-687">[DEPRECATED] Deprecated the `cosmosdb list-keys` command</span></span>
* <span data-ttu-id="de833-688">Ajout de la commande `cosmosdb keys list` (remplace `cosmosdb list-keys`)</span><span class="sxs-lookup"><span data-stu-id="de833-688">Added the `cosmosdb keys list` command - replaces `cosmosdb list-keys`</span></span>
* <span data-ttu-id="de833-689">`cosmsodb create/update`: Ajout d’un nouveau format pour --location afin d’autoriser la définition de la propriété « isZoneRedundant ».</span><span class="sxs-lookup"><span data-stu-id="de833-689">`cosmsodb create/update`: Added new format for --location to allow setting "isZoneRedundant" property.</span></span> <span data-ttu-id="de833-690">Ancien format déprécié</span><span class="sxs-lookup"><span data-stu-id="de833-690">Deprecated old format</span></span>

### <a name="eventgrid"></a><span data-ttu-id="de833-691">EventGrid</span><span class="sxs-lookup"><span data-stu-id="de833-691">EventGrid</span></span>
* <span data-ttu-id="de833-692">Ajout de commandes `eventgrid domain` pour les opérations CRUD liées aux domaines</span><span class="sxs-lookup"><span data-stu-id="de833-692">Added `eventgrid domain` commands for domain CRUD operations</span></span>
* <span data-ttu-id="de833-693">Ajout de commandes `eventgrid domain topic` pour les opérations CRUD liées aux rubriques de domaine</span><span class="sxs-lookup"><span data-stu-id="de833-693">Added `eventgrid domain topic` commands for domain topics CRUD operations</span></span>
* <span data-ttu-id="de833-694">Ajout de l’argument `--odata-query` à `eventgrid [topic|event-subscription] list` pour filtrer les résultats à l’aide de la syntaxe OData</span><span class="sxs-lookup"><span data-stu-id="de833-694">Added `--odata-query` argument to `eventgrid [topic|event-subscription] list` for filtering results using OData syntax</span></span>
* <span data-ttu-id="de833-695">`event-subscription create/update`: Ajout de servicebusqueue comme nouvelle valeur pour le paramètre `--endpoint-type`</span><span class="sxs-lookup"><span data-stu-id="de833-695">`event-subscription create/update`: Added servicebusqueue as new values for the `--endpoint-type` parameter</span></span>
* <span data-ttu-id="de833-696">[CHANGEMENT CASSANT] Suppression de la prise en charge de `--included-event-types All` avec `eventgrid event-subscription [create|update]`</span><span class="sxs-lookup"><span data-stu-id="de833-696">[BREAKING CHANGE] Removed support for `--included-event-types All` with `eventgrid event-subscription [create|update]`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="de833-697">HDInsight</span><span class="sxs-lookup"><span data-stu-id="de833-697">HDInsight</span></span>
* <span data-ttu-id="de833-698">Ajout de la prise en charge du paramètre `--ssh-public-key` dans la commande `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="de833-698">Added support for `--ssh-public-key` parameter in `hdinsight create` command</span></span>

### <a name="iot"></a><span data-ttu-id="de833-699">IoT</span><span class="sxs-lookup"><span data-stu-id="de833-699">IoT</span></span>
* <span data-ttu-id="de833-700">Ajout de la prise en charge pour régénérer les clés de stratégie d’autorisation</span><span class="sxs-lookup"><span data-stu-id="de833-700">Added support to regenerate authorization policy keys</span></span>
* <span data-ttu-id="de833-701">Ajout du SDK et de la prise en charge du service de provisionnement de dépôt DigitalTwin</span><span class="sxs-lookup"><span data-stu-id="de833-701">Added SDK and support for DigitalTwin Repository Provisioning Service</span></span>

### <a name="network"></a><span data-ttu-id="de833-702">Réseau</span><span class="sxs-lookup"><span data-stu-id="de833-702">Network</span></span>
* <span data-ttu-id="de833-703">Ajout de la prise en charge de la zone pour NAT Gateway</span><span class="sxs-lookup"><span data-stu-id="de833-703">Added Zone support for Nat Gateway</span></span>
* <span data-ttu-id="de833-704">Ajout de la commande `network list-service-tags`</span><span class="sxs-lookup"><span data-stu-id="de833-704">Added command `network list-service-tags`</span></span>
* <span data-ttu-id="de833-705">Correction d’un problème avec `dns zone import` empêchant les utilisateurs d’importer les enregistrements A génériques</span><span class="sxs-lookup"><span data-stu-id="de833-705">Fixed issue with `dns zone import` where users could not import wildcard A records</span></span>
* <span data-ttu-id="de833-706">Correction d’un problème avec `watcher flow-log configure` empêchant l’activation de la journalisation de flux dans certaines régions</span><span class="sxs-lookup"><span data-stu-id="de833-706">Fixed issue with `watcher flow-log configure` where flow logging could not be enabled in certain regions</span></span>

### <a name="resource"></a><span data-ttu-id="de833-707">Ressource</span><span class="sxs-lookup"><span data-stu-id="de833-707">Resource</span></span>
* <span data-ttu-id="de833-708">Ajout de la commande `az rest` pour passer des appels REST</span><span class="sxs-lookup"><span data-stu-id="de833-708">Added `az rest` command for making REST calls</span></span>
* <span data-ttu-id="de833-709">Correction d’une erreur liée à l’utilisation de `policy assignment list` avec un groupe de ressources ou un niveau d’abonnement `--scope`</span><span class="sxs-lookup"><span data-stu-id="de833-709">Fixed error when using `policy assignment list` with a resource group or subscription level `--scope`</span></span>

### <a name="servicebus"></a><span data-ttu-id="de833-710">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="de833-710">ServiceBus</span></span>
* <span data-ttu-id="de833-711">Résolution d’un problème lié à `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span><span class="sxs-lookup"><span data-stu-id="de833-711">Fixed issue with `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span></span>

### <a name="sql"></a><span data-ttu-id="de833-712">SQL</span><span class="sxs-lookup"><span data-stu-id="de833-712">SQL</span></span>
* <span data-ttu-id="de833-713">Modification apportée à `--location` pour le rendre facultatif pour `sql [server|mi] create` : utilise l’emplacement du groupe de ressources s’il n’est pas spécifié</span><span class="sxs-lookup"><span data-stu-id="de833-713">Changed `--location` to be optional for `sql [server|mi] create` - uses resource group location if not specified</span></span>
* <span data-ttu-id="de833-714">Correction de l’erreur « L’objet 'NoneType' n’est pas itérable » pour `sql db list-editions --available`</span><span class="sxs-lookup"><span data-stu-id="de833-714">Fixed "'NoneType' object is not iterable" error for `sql db list-editions --available`</span></span>

### <a name="sqlvm"></a><span data-ttu-id="de833-715">SQLVm</span><span class="sxs-lookup"><span data-stu-id="de833-715">SQLVm</span></span>
* <span data-ttu-id="de833-716">[CHANGEMENT CASSANT] Modification de `sql vm create` pour exiger le paramètre `--license-type`</span><span class="sxs-lookup"><span data-stu-id="de833-716">[BREAKING CHNAGE] Changed `sql vm create` to require `--license-type` parameter</span></span>
* <span data-ttu-id="de833-717">Modification apportée pour autoriser la définition d’une référence SKU d’image SQL lors de la création ou de la mise à jour d’une machine virtuelle SQL</span><span class="sxs-lookup"><span data-stu-id="de833-717">Changed to allow setting SQL image SKU when creating or updating a sql vm</span></span>

### <a name="storage"></a><span data-ttu-id="de833-718">Stockage</span><span class="sxs-lookup"><span data-stu-id="de833-718">Storage</span></span>
* <span data-ttu-id="de833-719">Correction d’un problème lié à une clé de compte manquante pour `storage container generate-sas`</span><span class="sxs-lookup"><span data-stu-id="de833-719">Fixed issue with missing account key for `storage container generate-sas`</span></span>
* <span data-ttu-id="de833-720">Correction d’un problème lié à `storage blob sync` sur Linux</span><span class="sxs-lookup"><span data-stu-id="de833-720">Fixed issue with `storage blob sync` on Linux</span></span>

### <a name="vm"></a><span data-ttu-id="de833-721">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="de833-721">VM</span></span>
* <span data-ttu-id="de833-722">[PRÉVERSION] Ajout de commandes `vm image template` pour générer des images de machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="de833-722">[PREVIEW] Added `vm image template` commands to build VM images</span></span>

## <a name="june-4-2019"></a><span data-ttu-id="de833-723">4 juin 2019</span><span class="sxs-lookup"><span data-stu-id="de833-723">June 4, 2019</span></span>

<span data-ttu-id="de833-724">Version 2.0.66</span><span class="sxs-lookup"><span data-stu-id="de833-724">Version 2.0.66</span></span>

### <a name="core"></a><span data-ttu-id="de833-725">Core</span><span class="sxs-lookup"><span data-stu-id="de833-725">Core</span></span>
* <span data-ttu-id="de833-726">Correction du bogue où des commandes échouent si `--output yaml` est utilisé avec `--query`</span><span class="sxs-lookup"><span data-stu-id="de833-726">Fixed bug where commands fail if `--output yaml` is used with `--query`</span></span>

### <a name="acr"></a><span data-ttu-id="de833-727">ACR</span><span class="sxs-lookup"><span data-stu-id="de833-727">ACR</span></span>
* <span data-ttu-id="de833-728">Ajout du groupe de commandes « acr pack » pour la création de tâches de génération rapide à l’aide de Buildpacks.</span><span class="sxs-lookup"><span data-stu-id="de833-728">Added 'acr pack' command group for creating quick build Tasks using Buildpacks.</span></span>

### <a name="acs"></a><span data-ttu-id="de833-729">ACS</span><span class="sxs-lookup"><span data-stu-id="de833-729">ACS</span></span>
* <span data-ttu-id="de833-730">Autoriser l’activation/la désactivation du module complémentaire kube-dashboard AKS</span><span class="sxs-lookup"><span data-stu-id="de833-730">Allow enabling/disabling AKS kube-dashboard addon</span></span>
* <span data-ttu-id="de833-731">Afficher un message convivial lorsque l’abonnement n’est pas autorisé à utiliser Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="de833-731">Print a friendly message when the subscription is not whitelisted to use Azure Red Hat OpenShift</span></span>

### <a name="batch"></a><span data-ttu-id="de833-732">Batch</span><span class="sxs-lookup"><span data-stu-id="de833-732">Batch</span></span>
* <span data-ttu-id="de833-733">Amélioration de la gestion des erreurs en l’absence de connexion à un compte \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span><span class="sxs-lookup"><span data-stu-id="de833-733">Improved error handling when not logged in to an account \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span></span>

### <a name="iot"></a><span data-ttu-id="de833-734">IoT</span><span class="sxs-lookup"><span data-stu-id="de833-734">IoT</span></span>
* <span data-ttu-id="de833-735">Ajout de la prise en charge du basculement manuel</span><span class="sxs-lookup"><span data-stu-id="de833-735">Added support for manual failover</span></span>

### <a name="network"></a><span data-ttu-id="de833-736">Réseau</span><span class="sxs-lookup"><span data-stu-id="de833-736">Network</span></span>
* <span data-ttu-id="de833-737">Ajout de commandes `network application-gateway waf-policy` pour prendre en charge des règles de pare-feu d’applications web personnalisées.</span><span class="sxs-lookup"><span data-stu-id="de833-737">Added `network application-gateway waf-policy` commands to support custom WAF rules.</span></span>
* <span data-ttu-id="de833-738">Ajout des arguments `--waf-policy` et `--max-capacity` à `network application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="de833-738">Added `--waf-policy` and `--max-capacity` arguments to `network application-gateway [create|update]`</span></span> 

### <a name="resource"></a><span data-ttu-id="de833-739">Ressource</span><span class="sxs-lookup"><span data-stu-id="de833-739">Resource</span></span>
* <span data-ttu-id="de833-740">Amélioration du message d’erreur émis par la commande `deployment create` quand aucun appareil TTY n’est disponible</span><span class="sxs-lookup"><span data-stu-id="de833-740">Improved error message from `deployment create` when there is no TTY available</span></span>

### <a name="role"></a><span data-ttu-id="de833-741">Role</span><span class="sxs-lookup"><span data-stu-id="de833-741">Role</span></span>
* <span data-ttu-id="de833-742">Mise à jour du texte d’aide</span><span class="sxs-lookup"><span data-stu-id="de833-742">Updated help text.</span></span>

### <a name="compute"></a><span data-ttu-id="de833-743">Calcul</span><span class="sxs-lookup"><span data-stu-id="de833-743">Compute</span></span>
* <span data-ttu-id="de833-744">Ajout de la prise en charge dans `vm create` des machines virtuelles à partir d’une image managée avec des LUN de disque de données qui ne démarrent pas de 0 ou qui ignorent des nombres</span><span class="sxs-lookup"><span data-stu-id="de833-744">Added support to `vm create` for VMs from a managed image with data-disk luns that do not start from 0 or that skip numbers</span></span>

## <a name="may-21-2019"></a><span data-ttu-id="de833-745">21 mai 2019</span><span class="sxs-lookup"><span data-stu-id="de833-745">May 21, 2019</span></span>

<span data-ttu-id="de833-746">Version 2.0.65</span><span class="sxs-lookup"><span data-stu-id="de833-746">Version 2.0.65</span></span>

### <a name="core"></a><span data-ttu-id="de833-747">Core</span><span class="sxs-lookup"><span data-stu-id="de833-747">Core</span></span>
* <span data-ttu-id="de833-748">Ajout de meilleurs commentaires pour les erreurs d’authentification</span><span class="sxs-lookup"><span data-stu-id="de833-748">Added better feedback for authentication errors</span></span>
* <span data-ttu-id="de833-749">Correction d’un problème où l’interface CLI chargeait des extensions qui n’étaient pas compatibles avec sa version principale</span><span class="sxs-lookup"><span data-stu-id="de833-749">Fixed issue where the CLI would load extensions that were not compatible with its core version</span></span>
* <span data-ttu-id="de833-750">Correction d’un problème lié au lancement lorsque `clouds.config` est endommagé</span><span class="sxs-lookup"><span data-stu-id="de833-750">Fixed issue with launching when `clouds.config` is corrupted</span></span>

### <a name="acr"></a><span data-ttu-id="de833-751">ACR</span><span class="sxs-lookup"><span data-stu-id="de833-751">ACR</span></span>
* <span data-ttu-id="de833-752">Ajout de la prise en charge des identités managées aux tâches</span><span class="sxs-lookup"><span data-stu-id="de833-752">Added support for Managed Identities to Tasks</span></span>

### <a name="acs"></a><span data-ttu-id="de833-753">ACS</span><span class="sxs-lookup"><span data-stu-id="de833-753">ACS</span></span>
* <span data-ttu-id="de833-754">Correction de la commande `openshift create` lorsqu’elle est utilisée avec le client AAD du client</span><span class="sxs-lookup"><span data-stu-id="de833-754">Fixed `openshift create` command when used with customer AAD client</span></span>

### <a name="appservice"></a><span data-ttu-id="de833-755">AppService</span><span class="sxs-lookup"><span data-stu-id="de833-755">AppService</span></span>
* <span data-ttu-id="de833-756">[DÉPRÉCIATION] Commande `functionapp devops-build` dépréciée (Elle sera supprimée de la prochaine version)</span><span class="sxs-lookup"><span data-stu-id="de833-756">[DEPRECATED] Deprecated `functionapp devops-build` command - will be removed in next release</span></span>
* <span data-ttu-id="de833-757">Changement apporté à `functionapp devops-pipeline` pour extraire un journal de génération d’Azure DevOps en mode détaillé</span><span class="sxs-lookup"><span data-stu-id="de833-757">Changed `functionapp devops-pipeline` to fetch build log from Azure DevOps in verbose mode</span></span>
* <span data-ttu-id="de833-758">[CHANGEMENT CASSANT] Suppression de l’indicateur `--use_local_settings` de la commande `functionapp devops-pipeline` (aucune opération)</span><span class="sxs-lookup"><span data-stu-id="de833-758">[BREAKING CHANGE] Removed `--use_local_settings` flag from `functionapp devops-pipeline` command - was a no-op</span></span>
* <span data-ttu-id="de833-759">Changement apporté à `webapp up` pour retourner une sortie JSON si `--logs` n’est pas utilisé</span><span class="sxs-lookup"><span data-stu-id="de833-759">Changed `webapp up` to return JSON output if `--logs` is not used</span></span>
* <span data-ttu-id="de833-760">Ajout de la prise en charge de l’écriture de ressources par défaut à la configuration locale pour `webapp up`</span><span class="sxs-lookup"><span data-stu-id="de833-760">Added support for writing default resources to local config for `webapp up`</span></span>
* <span data-ttu-id="de833-761">Ajout de la prise en charge à `webapp up` pour redéployer une application sans utiliser l’argument `--location`</span><span class="sxs-lookup"><span data-stu-id="de833-761">Added support to `webapp up` for redeploying an app without using the `--location` argument</span></span>
* <span data-ttu-id="de833-762">Résolution d’un problème où, lors de la création ASP de la référence SKU Gratuite, la valeur de référence Gratuit ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="de833-762">Fixed an issue where for Linux Free SKU ASP creation use Free as SKU value was not working</span></span>

### <a name="botservice"></a><span data-ttu-id="de833-763">BotService</span><span class="sxs-lookup"><span data-stu-id="de833-763">BotService</span></span>
* <span data-ttu-id="de833-764">Modification autorisant toutes les casses pour les paramètres `--lang` des commandes</span><span class="sxs-lookup"><span data-stu-id="de833-764">Changed to allow all casing for `--lang` parameters for commands</span></span>
* <span data-ttu-id="de833-765">Mise à jour de la description du module de commande</span><span class="sxs-lookup"><span data-stu-id="de833-765">Updated description for command module</span></span>

### <a name="consumption"></a><span data-ttu-id="de833-766">Consommation</span><span class="sxs-lookup"><span data-stu-id="de833-766">Consumption</span></span>
* <span data-ttu-id="de833-767">Ajout du paramètre obligatoire manquant lors de l’exécution de `consumption usage list --billing-period-name`</span><span class="sxs-lookup"><span data-stu-id="de833-767">Added missing required parameter when running `consumption usage list --billing-period-name`</span></span>

### <a name="iot"></a><span data-ttu-id="de833-768">IoT</span><span class="sxs-lookup"><span data-stu-id="de833-768">IoT</span></span>
* <span data-ttu-id="de833-769">Ajout de la prise en charge permettant de répertorier toutes les clés</span><span class="sxs-lookup"><span data-stu-id="de833-769">Added support to list all keys</span></span>

### <a name="network"></a><span data-ttu-id="de833-770">Réseau</span><span class="sxs-lookup"><span data-stu-id="de833-770">Network</span></span>
* [CHANGEMENT CASSANT]: Removed `network interface-endpoints` command group - use `network private-endpoints`
[BREAKING CHANGE]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* <span data-ttu-id="de833-772">Ajout de l’argument `--nat-gateway` à `network vnet subnet [create|update]` pour attacher à une passerelle NAT</span><span class="sxs-lookup"><span data-stu-id="de833-772">Added `--nat-gateway` argument to `network vnet subnet [create|update]` for attaching to a NAT gateway</span></span>
* <span data-ttu-id="de833-773">Correction d’un problème avec `dns zone import` où les noms d’enregistrement pouvaient ne pas correspondre à un type d’enregistrement</span><span class="sxs-lookup"><span data-stu-id="de833-773">Fixed issue with `dns zone import` where record names could not match a record type</span></span>

### <a name="rdbms"></a><span data-ttu-id="de833-774">SGBDR</span><span class="sxs-lookup"><span data-stu-id="de833-774">RDBMS</span></span>
* <span data-ttu-id="de833-775">Ajout de la prise en charge de MySQL et Postgres pour la géoréplication</span><span class="sxs-lookup"><span data-stu-id="de833-775">Added postgres and mysql support for geo replication</span></span>

### <a name="rbac"></a><span data-ttu-id="de833-776">RBAC</span><span class="sxs-lookup"><span data-stu-id="de833-776">RBAC</span></span>
* <span data-ttu-id="de833-777">Ajout de la prise en charge de l’étendue du groupe de gestion dans `role assignment`</span><span class="sxs-lookup"><span data-stu-id="de833-777">Added support for management group scope to `role assignment`</span></span>

### <a name="storage"></a><span data-ttu-id="de833-778">Stockage</span><span class="sxs-lookup"><span data-stu-id="de833-778">Storage</span></span>
* <span data-ttu-id="de833-779">`storage blob sync` : ajout de la commande de synchronisation pour le blob de stockage</span><span class="sxs-lookup"><span data-stu-id="de833-779">`storage blob sync`: add sync command for storage blob</span></span>

### <a name="compute"></a><span data-ttu-id="de833-780">Calcul</span><span class="sxs-lookup"><span data-stu-id="de833-780">Compute</span></span>
* <span data-ttu-id="de833-781">Ajout de `--computer-name` à `vm create` pour définir le nom d’une machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="de833-781">Added `--computer-name` to `vm create` for setting a VM's computer name</span></span>
* <span data-ttu-id="de833-782">`--ssh-key-value` renommé en `--ssh-key-values` pour `[vm|vmss] create` - peut maintenant accepter plusieurs chemins d’accès ou valeurs de clé publique SSH</span><span class="sxs-lookup"><span data-stu-id="de833-782">Renamed `--ssh-key-value` renamed to `--ssh-key-values` for `[vm|vmss] create` - can now accept multiple ssh public key values or paths</span></span>
  * <span data-ttu-id="de833-783">__Remarque__ : il ne s’agit **pas** d’un changement cassant - `--ssh-key-value` sera analysé correctement, car il correspond uniquement à `--ssh-key-values`</span><span class="sxs-lookup"><span data-stu-id="de833-783">__Note__: This is **not** a breaking change - `--ssh-key-value` will be parsed correctly as it matches only `--ssh-key-values`</span></span>
* <span data-ttu-id="de833-784">Modification de l’argument `--type` qui devient facultatif dans `ppg create`</span><span class="sxs-lookup"><span data-stu-id="de833-784">Changed the `--type` argument of `ppg create` to be optional</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="de833-785">6 mai 2019</span><span class="sxs-lookup"><span data-stu-id="de833-785">May 6, 2019</span></span>

<span data-ttu-id="de833-786">Version 2.0.64</span><span class="sxs-lookup"><span data-stu-id="de833-786">Version 2.0.64</span></span>

### <a name="acs"></a><span data-ttu-id="de833-787">ACS</span><span class="sxs-lookup"><span data-stu-id="de833-787">ACS</span></span>
* <span data-ttu-id="de833-788">[CHANGEMENT CASSANT] Suppression de l’indicateur `--fqdn` sur les commandes `openshift`</span><span class="sxs-lookup"><span data-stu-id="de833-788">[BREAKING CHANGE] Removed `--fqdn` flag on `openshift` commands</span></span>
* <span data-ttu-id="de833-789">Modification permettant d’utiliser la version d’API en disponibilité générale d’Azure Red Hat Openshift</span><span class="sxs-lookup"><span data-stu-id="de833-789">Changed to use Azure Red Hat Openshift GA API Version</span></span>
* <span data-ttu-id="de833-790">Ajout de l’indicateur `customer-admin-group-id` à `openshift create`</span><span class="sxs-lookup"><span data-stu-id="de833-790">Added `customer-admin-group-id` flag to `openshift create`</span></span>
* <span data-ttu-id="de833-791">[Mise à la disposition générale] Suppression de `(PREVIEW)` de l’option `aks create``--network-policy`</span><span class="sxs-lookup"><span data-stu-id="de833-791">[GA] Removed `(PREVIEW)` from `aks create` option `--network-policy`</span></span>

### <a name="appservice"></a><span data-ttu-id="de833-792">AppService</span><span class="sxs-lookup"><span data-stu-id="de833-792">Appservice</span></span>
* <span data-ttu-id="de833-793">[DÉPRÉCIATION] Commande `functionapp devops-build` dépréciée</span><span class="sxs-lookup"><span data-stu-id="de833-793">[DEPRECATED] Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="de833-794">Renommée `functionapp devops-pipeline`</span><span class="sxs-lookup"><span data-stu-id="de833-794">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="de833-795">Correction du processus d’obtention du nom d’utilisateur pour Cloud Shell qui provoquait l’échec de `webapp up`</span><span class="sxs-lookup"><span data-stu-id="de833-795">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="de833-796">Mise à jour de la documentation `appservice plan --sku` pour refléter les plans App Service pris en charge</span><span class="sxs-lookup"><span data-stu-id="de833-796">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="de833-797">Ajout d’arguments facultatifs pour le groupe et le plan de ressources à `webapp up`</span><span class="sxs-lookup"><span data-stu-id="de833-797">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="de833-798">Ajout de dispositifs de prise en charge à `webapp ssh` pour respecter la variable d’environnement `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`</span><span class="sxs-lookup"><span data-stu-id="de833-798">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="de833-799">Ajout de la prise en charge de `appserviceplan create` pour la référence SKU Linux gratuite</span><span class="sxs-lookup"><span data-stu-id="de833-799">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="de833-800">Mise en veille de 30 s de `webapp up` après la définition de `SCM_DO_BUILD_DURING_DEPLOYMENT=true` pour gérer le démarrage à froid de kudu</span><span class="sxs-lookup"><span data-stu-id="de833-800">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="de833-801">Ajout de la prise en charge du runtime `powershell` à `functionapp create` sur Windows</span><span class="sxs-lookup"><span data-stu-id="de833-801">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="de833-802">Ajout de la commande `create-remote-connection`</span><span class="sxs-lookup"><span data-stu-id="de833-802">Added `create-remote-connection` command</span></span>

### <a name="batch"></a><span data-ttu-id="de833-803">Batch</span><span class="sxs-lookup"><span data-stu-id="de833-803">Batch</span></span>
* <span data-ttu-id="de833-804">Correction du bogue dans le validateur pour les options `--application-package-references`</span><span class="sxs-lookup"><span data-stu-id="de833-804">Fixed bug in validator for `--application-package-references` options</span></span>

### <a name="botservice"></a><span data-ttu-id="de833-805">Botservice</span><span class="sxs-lookup"><span data-stu-id="de833-805">Botservice</span></span>
* <span data-ttu-id="de833-806">[CHANGEMENT CASSANT] Modification apportée à `bot create -v v4 -k webapp` pour créer un bot d’application web vide par défaut (autrement dit, aucun bot n’est déployé sur App Service)</span><span class="sxs-lookup"><span data-stu-id="de833-806">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to create an empty Web App Bot by default (i.e. no bot is deployed to the App Service)</span></span>
* <span data-ttu-id="de833-807">Ajout de l’indicateur `--echo` à `bot create` pour utiliser l’ancien comportement avec `-v v4`</span><span class="sxs-lookup"><span data-stu-id="de833-807">Added `--echo` flag to `bot create` to use the old behavior with `-v v4`</span></span>
* <span data-ttu-id="de833-808">[CHANGEMENT CASSANT] Modification de la valeur par défaut de `--version` qui devient `v4`</span><span class="sxs-lookup"><span data-stu-id="de833-808">[BREAKING CHANGE] Changed the default value of  `--version` to `v4`</span></span>
  * <span data-ttu-id="de833-809">__REMARQUE :__ `bot prepare-publish` utilise toujours son ancienne valeur par défaut</span><span class="sxs-lookup"><span data-stu-id="de833-809">__NOTE:__ `bot prepare-publish` still uses the its old default</span></span>
* <span data-ttu-id="de833-810">[CHANGEMENT CASSANT] Modification de `--lang` qui n’a plus la valeur par défaut `Csharp`.</span><span class="sxs-lookup"><span data-stu-id="de833-810">[BREAKING CHANGE] Changed `--lang` to no longer default to `Csharp`.</span></span> <span data-ttu-id="de833-811">Si la commande nécessite `--lang` et que celui-ci n’est pas fourni, la commande génère à présent une erreur</span><span class="sxs-lookup"><span data-stu-id="de833-811">If the command requires `--lang` and it is not provided, the command will now error out</span></span>
* <span data-ttu-id="de833-812">[CHANGEMENT CASSANT] Modification des arguments `--appid` et `--password` de `bot create` afin que ceux-ci soient requis et puisse maintenant être créés via `ad app create`</span><span class="sxs-lookup"><span data-stu-id="de833-812">[BREAKING CHANGE] Changed the `--appid` and `--password` args for `bot create` to be required and can now be created via `ad app create`</span></span>
* <span data-ttu-id="de833-813">Ajout de la validation `--appid` et `--password`</span><span class="sxs-lookup"><span data-stu-id="de833-813">Added `--appid` and `--password` validation</span></span>
* <span data-ttu-id="de833-814">[CHANGEMENT CASSANT] Modification apportée à la commande `bot create -v v4` afin qu’elle ne crée ni n’utilise un compte de stockage ou Application Insights</span><span class="sxs-lookup"><span data-stu-id="de833-814">[BREAKING CHANGE] Changed `bot create -v v4` to not create or use a Storage Account or Application Insights</span></span>
* <span data-ttu-id="de833-815">[CHANGEMENT CASSANT] Modification de `bot create -v v3` pour exiger une région où Application Insights est disponible</span><span class="sxs-lookup"><span data-stu-id="de833-815">[BREAKING CHANGE] Changed `bot create -v v3` to require a region where Application Insights is available</span></span>
* <span data-ttu-id="de833-816">[CHANGEMENT CASSANT] Modification de `bot update` qui affecte maintenant uniquement les propriétés spécifiques d’un bot</span><span class="sxs-lookup"><span data-stu-id="de833-816">[BREAKING CHANGE] Changed `bot update` to now affect only specific properties of a bot</span></span>
* <span data-ttu-id="de833-817">[CHANGEMENT CASSANT] Modification des indicateurs `--lang` qui acceptent `Javascript` au lieu de `Node`</span><span class="sxs-lookup"><span data-stu-id="de833-817">[BREAKING CHANGE] Changed `--lang` flags to accept `Javascript` instead of `Node`</span></span>
* <span data-ttu-id="de833-818">[CHANGEMENT CASSANT] Suppression de `Node` comme valeur `--lang` autorisée</span><span class="sxs-lookup"><span data-stu-id="de833-818">[BREAKING CHANGE] Removed `Node` as an allowed `--lang` value</span></span>
* <span data-ttu-id="de833-819">[CHANGEMENT CASSANT] Modification de `bot create -v v4 -k webapp` afin que `SCM_DO_BUILD_DURING_DEPLOYMENT` ne soit plus défini sur True.</span><span class="sxs-lookup"><span data-stu-id="de833-819">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to no longer set `SCM_DO_BUILD_DURING_DEPLOYMENT` to true.</span></span> <span data-ttu-id="de833-820">Tous les déploiements via Kudu agissent conformément à leur comportement par défaut</span><span class="sxs-lookup"><span data-stu-id="de833-820">All deployments through Kudu will act according to their default behavior</span></span>
* <span data-ttu-id="de833-821">Modification de la commande `bot download` pour des bots sans fichiers `.bot` afin de créer le fichier de configuration spécifique à une langue avec des valeurs de paramètres d’application pour le bot</span><span class="sxs-lookup"><span data-stu-id="de833-821">Changed `bot download` for bots without `.bot` files to create the language-specific configuration file with values from the Application Settings for the bot</span></span>
* <span data-ttu-id="de833-822">Ajout de la prise en charge de `Typescript` pour `bot prepare-deploy`</span><span class="sxs-lookup"><span data-stu-id="de833-822">Added `Typescript` support to `bot prepare-deploy`</span></span>
* <span data-ttu-id="de833-823">Ajout du message d’avertissement à `bot prepare-deploy` pour les bots `Javascript` et `Typescript` quand `--code-dir` ne contient pas `package.json`</span><span class="sxs-lookup"><span data-stu-id="de833-823">Added warning message to `bot prepare-deploy` for `Javascript` and `Typescript` bots for when `--code-dir` does not contain `package.json`</span></span>
* <span data-ttu-id="de833-824">Modification de `bot prepare-deploy` qui retourne `true` en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="de833-824">Changed `bot prepare-deploy` to return `true` if successful</span></span>
* <span data-ttu-id="de833-825">Ajout de la journalisation commentée à `bot prepare-deploy`</span><span class="sxs-lookup"><span data-stu-id="de833-825">Added verbose logging to `bot prepare-deploy`</span></span>
* <span data-ttu-id="de833-826">Ajout d’un plus grand nombre de régions Application Insights disponibles dans `az bot create -v v3`</span><span class="sxs-lookup"><span data-stu-id="de833-826">Added more available Application Insights regions to `az bot create -v v3`</span></span>

### <a name="configure"></a><span data-ttu-id="de833-827">Configurer</span><span class="sxs-lookup"><span data-stu-id="de833-827">Configure</span></span>
* <span data-ttu-id="de833-828">Ajout de la prise en charge des configurations de valeur par défaut d’argument en fonction d’un dossier</span><span class="sxs-lookup"><span data-stu-id="de833-828">Added support for folder based argument default value configurations</span></span>

### <a name="eventhubs"></a><span data-ttu-id="de833-829">Eventhubs</span><span class="sxs-lookup"><span data-stu-id="de833-829">Eventhubs</span></span>
* <span data-ttu-id="de833-830">Ajout des commandes `namespace network-rule`</span><span class="sxs-lookup"><span data-stu-id="de833-830">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="de833-831">Ajout de l’argument `--default-action` pour les règles réseau à `namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="de833-831">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="de833-832">Réseau</span><span class="sxs-lookup"><span data-stu-id="de833-832">Network</span></span>
* <span data-ttu-id="de833-833">[CHANGEMENT CASSANT] Remplacement de l’argument `--cache` par `--defer` pour `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="de833-833">[BREAKING CHANGE] Replaced `--cache` arugment with `--defer` for `vnet [create|update]`</span></span> 

### <a name="policy-insights"></a><span data-ttu-id="de833-834">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="de833-834">Policy Insights</span></span>
* <span data-ttu-id="de833-835">Ajout de la prise en charge pour `--expand PolicyEvaluationDetails` pour interroger les détails de l’évaluation de stratégie sur la ressource</span><span class="sxs-lookup"><span data-stu-id="de833-835">Added support for `--expand PolicyEvaluationDetails` to query policy evaluation details on the resource</span></span>

### <a name="role"></a><span data-ttu-id="de833-836">Role</span><span class="sxs-lookup"><span data-stu-id="de833-836">Role</span></span>
* <span data-ttu-id="de833-837">[DÉPRÉCIATION] Changement apporté à `create-for-rbac` concernant le masquage de l’argument '--password' - Fin de la prise en charge en mai 2019</span><span class="sxs-lookup"><span data-stu-id="de833-837">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

### <a name="service-bus"></a><span data-ttu-id="de833-838">Service Bus</span><span class="sxs-lookup"><span data-stu-id="de833-838">Service Bus</span></span>
* <span data-ttu-id="de833-839">Ajout des commandes `namespace network-rule`</span><span class="sxs-lookup"><span data-stu-id="de833-839">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="de833-840">Ajout de l’argument `--default-action` pour les règles réseau à `namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="de833-840">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>
* <span data-ttu-id="de833-841">Correction de `topic [create|update]` qui autorise `--max-size` à prendre en charge les valeurs 10, 20, 40 et 80 Go avec la référence SKU Premium</span><span class="sxs-lookup"><span data-stu-id="de833-841">Fixed `topic [create|update]` to allow `--max-size` support for 10, 20, 40 and 80GB values with premium SKU</span></span>

### <a name="sql"></a><span data-ttu-id="de833-842">SQL</span><span class="sxs-lookup"><span data-stu-id="de833-842">SQL</span></span>
* <span data-ttu-id="de833-843">Ajout des commandes `sql virtual-cluster [list|show|delete]`</span><span class="sxs-lookup"><span data-stu-id="de833-843">Added `sql virtual-cluster [list|show|delete]` commands</span></span>

### <a name="vm"></a><span data-ttu-id="de833-844">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="de833-844">VM</span></span>
* <span data-ttu-id="de833-845">Ajout de `--protect-from-scale-in` et `--protect-from-scale-set-actions` à `vmss update` pour activer les mises à jour de la stratégie de protection des instances de machine virtuelle VMSS</span><span class="sxs-lookup"><span data-stu-id="de833-845">Added `--protect-from-scale-in` and `--protect-from-scale-set-actions` to `vmss update` to enable updates to the protection policy of VMSS VM instances</span></span>
* <span data-ttu-id="de833-846">Ajout de `--instance-id` à `vmss update` pour activer la mise à jour générique des instances de machine virtuelle VMSS</span><span class="sxs-lookup"><span data-stu-id="de833-846">Added `--instance-id` to `vmss update` to enable generic update of VMSS VM instances</span></span>
* <span data-ttu-id="de833-847">Ajout de `--instance-id` à `vmss wait`</span><span class="sxs-lookup"><span data-stu-id="de833-847">Added `--instance-id` to `vmss wait`</span></span>
* <span data-ttu-id="de833-848">Ajout du nouveau groupe de commandes `ppg` pour gérer les groupes de placements de proximité</span><span class="sxs-lookup"><span data-stu-id="de833-848">Added new `ppg` command group for managing Proximity Placement Groups</span></span>
* <span data-ttu-id="de833-849">Ajout de `--ppg` à `[vm|vmss] create` et `vm availability-set create` pour la gestion des groupes de placements de proximité</span><span class="sxs-lookup"><span data-stu-id="de833-849">Added `--ppg` to `[vm|vmss] create` and `vm availability-set create` for managing PPGs</span></span>
* <span data-ttu-id="de833-850">Ajout du paramètre `--hyper-v-generation` pour `image create`</span><span class="sxs-lookup"><span data-stu-id="de833-850">Added `--hyper-v-generation` parameter to `image create`</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="de833-851">23 avril 2019</span><span class="sxs-lookup"><span data-stu-id="de833-851">April 23, 2019</span></span>

<span data-ttu-id="de833-852">Version 2.0.63</span><span class="sxs-lookup"><span data-stu-id="de833-852">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="de833-853">ACS</span><span class="sxs-lookup"><span data-stu-id="de833-853">ACS</span></span>
* <span data-ttu-id="de833-854">Changement apporté à `aks get-credentials` pour demander confirmation en cas de remplacement de valeurs dupliquées</span><span class="sxs-lookup"><span data-stu-id="de833-854">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="de833-855">Suppression de `(PREVIEW)` des commandes Dev Spaces « aks use-dev-spaces » et « aks remove-dev-spaces »</span><span class="sxs-lookup"><span data-stu-id="de833-855">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="de833-856">AMS</span><span class="sxs-lookup"><span data-stu-id="de833-856">AMS</span></span>
* <span data-ttu-id="de833-857">Correction d’un bogue lié à la mise à jour des filtres de composant et de compte</span><span class="sxs-lookup"><span data-stu-id="de833-857">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="de833-858">AppService</span><span class="sxs-lookup"><span data-stu-id="de833-858">AppService</span></span>
* <span data-ttu-id="de833-859">Ajout de la prise en charge d’ASE et de délais d’expiration à `webapp ssh`</span><span class="sxs-lookup"><span data-stu-id="de833-859">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="de833-860">Ajout de la prise en charge de l’établissement de CI/CD dans un pipeline Azure DevOps entre un dépôt Github et des applications de fonction</span><span class="sxs-lookup"><span data-stu-id="de833-860">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="de833-861">Ajout de l’argument `--github-pat` à `functionapp devops-build create` pour accepter un jeton d’accès personnel Github</span><span class="sxs-lookup"><span data-stu-id="de833-861">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="de833-862">Ajout de l’argument `--github-repository` à `functionapp devops-build create` pour accepter un dépôt Github contenant le code source d’une application de fonction</span><span class="sxs-lookup"><span data-stu-id="de833-862">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="de833-863">Résolution d’un problème provoquant l’échec de `az webapp up --logs` avec une erreur et la mise à jour de la version par défaut NETCORE avec la version 2.1</span><span class="sxs-lookup"><span data-stu-id="de833-863">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="de833-864">Suppression des paramètres d’application de fonction inutiles lors de la création d’une telle application avec un plan de consommation</span><span class="sxs-lookup"><span data-stu-id="de833-864">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="de833-865">Changement apporté à `webapp up` pour ajouter un numéro à la fin de la chaîne asp par défaut afin de créer un ASP basé sur les options de la référence SKU</span><span class="sxs-lookup"><span data-stu-id="de833-865">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="de833-866">Ajout de `-b` en tant qu’option à `webapp up` pour lancer l’application dans le navigateur</span><span class="sxs-lookup"><span data-stu-id="de833-866">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="de833-867">Changement apporté à `webapp deployment source config zip` pour gérer la variable d’environnement `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`</span><span class="sxs-lookup"><span data-stu-id="de833-867">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="de833-868">Gestionnaire de déploiement</span><span class="sxs-lookup"><span data-stu-id="de833-868">Deployment Manager</span></span>
* <span data-ttu-id="de833-869">[PRÉVERSION] Création et gestion d’artefacts prenant en charge les lancements</span><span class="sxs-lookup"><span data-stu-id="de833-869">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="de833-870">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="de833-870">Lab</span></span>
* <span data-ttu-id="de833-871">Correction d’un bogue provoquant une sortie anticipée</span><span class="sxs-lookup"><span data-stu-id="de833-871">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="de833-872">Réseau</span><span class="sxs-lookup"><span data-stu-id="de833-872">Network</span></span>
* <span data-ttu-id="de833-873">Ajout d’une délégation de serveurs nommés automatiquement à `dns zone create` dans le parent durant la création d’une zone enfant</span><span class="sxs-lookup"><span data-stu-id="de833-873">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="de833-874">Ressource</span><span class="sxs-lookup"><span data-stu-id="de833-874">Resource</span></span>
* <span data-ttu-id="de833-875">[DÉPRÉCIATION] Dépréciation des arguments `--link-id`, `--target-id` et `--filter-string` de `resource link`</span><span class="sxs-lookup"><span data-stu-id="de833-875">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="de833-876">Arguments remplacés par `--link`, `--target` et `--filter`</span><span class="sxs-lookup"><span data-stu-id="de833-876">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="de833-877">Correction d’un problème empêchant le fonctionnement des commandes `resource link [create|update]`</span><span class="sxs-lookup"><span data-stu-id="de833-877">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="de833-878">Correction d’un problème où une suppression effectuée à l’aide d’un ID de ressource pouvait entraîner un plantage en cas d’erreur</span><span class="sxs-lookup"><span data-stu-id="de833-878">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="de833-879">SQL</span><span class="sxs-lookup"><span data-stu-id="de833-879">SQL</span></span>
* <span data-ttu-id="de833-880">Ajout de la prise en charge d’un fuseau horaire personnalisé sur les instances managées</span><span class="sxs-lookup"><span data-stu-id="de833-880">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="de833-881">Changement apporté pour autoriser l’utilisation d’un nom de pool élastique avec `sql db update`</span><span class="sxs-lookup"><span data-stu-id="de833-881">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="de833-882">Ajout de la prise en charge de `--no-wait` pour `sql server [create|update]`</span><span class="sxs-lookup"><span data-stu-id="de833-882">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="de833-883">Ajout de la commande `sql server wait`</span><span class="sxs-lookup"><span data-stu-id="de833-883">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="de833-884">Stockage</span><span class="sxs-lookup"><span data-stu-id="de833-884">Storage</span></span>
* <span data-ttu-id="de833-885">Résolution du problème lié aux jetons SAS à double encodage dans `storage blob generate-sas`</span><span class="sxs-lookup"><span data-stu-id="de833-885">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="de833-886">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="de833-886">VM</span></span>
* <span data-ttu-id="de833-887">Ajout de l’indicateur `--skip-shutdown` à `vm|vmss stop` pour mettre hors tension les machines virtuelles sans les arrêter</span><span class="sxs-lookup"><span data-stu-id="de833-887">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="de833-888">Ajout de l’argument `--storage-account-type` à `sig image-version create` pour définir le type de compte du profil de publication</span><span class="sxs-lookup"><span data-stu-id="de833-888">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="de833-889">Ajout de l’argument `--target-regions` à `sig image-version create` pour autoriser la définition de types de comptes de stockage spécifiques à une région</span><span class="sxs-lookup"><span data-stu-id="de833-889">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="de833-890">9 avril 2019</span><span class="sxs-lookup"><span data-stu-id="de833-890">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="de833-891">Core</span><span class="sxs-lookup"><span data-stu-id="de833-891">Core</span></span>
* <span data-ttu-id="de833-892">Correction du problème où certaines extensions affichaient une version `Unknown` et ne pouvaient pas être mises à jour</span><span class="sxs-lookup"><span data-stu-id="de833-892">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="de833-893">ACR</span><span class="sxs-lookup"><span data-stu-id="de833-893">ACR</span></span>
* <span data-ttu-id="de833-894">Ajout de la prise en charge de l’exécution d’une image sans contexte</span><span class="sxs-lookup"><span data-stu-id="de833-894">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="de833-895">AMS</span><span class="sxs-lookup"><span data-stu-id="de833-895">AMS</span></span>
* [DÉPRÉCIATION]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [CHANGEMENT CASSANT]: Renamed the `--bitrate` parameter to `--first-quality`
[BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="de833-898">Ajout de la prise en charge de nouveaux paramètres de chiffrement dans `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="de833-898">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="de833-899">Ajout du nouveau paramètre `--filters` à `ams streaming-locator create`</span><span class="sxs-lookup"><span data-stu-id="de833-899">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="de833-900">AppService</span><span class="sxs-lookup"><span data-stu-id="de833-900">AppService</span></span>
* <span data-ttu-id="de833-901">Ajout de la prise en charge de `--logs` pour `webapp up`</span><span class="sxs-lookup"><span data-stu-id="de833-901">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="de833-902">Correction des problèmes de génération de `azure-pipelines.yml` avec la commande `functionapp devops-build create`</span><span class="sxs-lookup"><span data-stu-id="de833-902">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="de833-903">Amélioration des indicateurs et de la gestion des erreurs `unctionapp devops-build create`</span><span class="sxs-lookup"><span data-stu-id="de833-903">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="de833-904">[CHANGEMENT CASSANT] Suppression de l’indicateur `--local-git` pour la commande `devops-build` ; la détection et la gestion d’un Git local sont obligatoires pour créer des pipelines Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="de833-904">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="de833-905">Ajout de la prise en charge de la création de plan de fonction pour Linux</span><span class="sxs-lookup"><span data-stu-id="de833-905">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="de833-906">Ajout de la possibilité de changer de plan sous une application de fonction avec `functionapp update --plan`</span><span class="sxs-lookup"><span data-stu-id="de833-906">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="de833-907">Ajout de la prise en charge de paramètres de scale-out pour le plan Azure Functions Premium</span><span class="sxs-lookup"><span data-stu-id="de833-907">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="de833-908">CDN</span><span class="sxs-lookup"><span data-stu-id="de833-908">CDN</span></span>
* <span data-ttu-id="de833-909">Ajout de la prise en charge de `Microsoft_Standard` et de `Standard_ChinaCdn`</span><span class="sxs-lookup"><span data-stu-id="de833-909">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="de833-910">Commentaires</span><span class="sxs-lookup"><span data-stu-id="de833-910">Feedback</span></span>
* <span data-ttu-id="de833-911">Changement apporté à `feedback` pour afficher les métadonnées sur les commandes exécutées récemment</span><span class="sxs-lookup"><span data-stu-id="de833-911">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="de833-912">Changement apporté à `feedback` pour inviter l’utilisateur à ouvrir un navigateur et à utiliser un modèle de message de problème afin de faciliter le processus de création du ticket</span><span class="sxs-lookup"><span data-stu-id="de833-912">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="de833-913">Changement apporté à `feedback` pour afficher le corps du message du problème quand la commande est exécutée avec '--verbose'</span><span class="sxs-lookup"><span data-stu-id="de833-913">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="de833-914">Moniteur</span><span class="sxs-lookup"><span data-stu-id="de833-914">Monitor</span></span>
* <span data-ttu-id="de833-915">Correction du problème où « count » n’était pas une valeur autorisée avec `metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="de833-915">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="de833-916">Réseau</span><span class="sxs-lookup"><span data-stu-id="de833-916">Network</span></span>
* <span data-ttu-id="de833-917">Correction du problème empêchant l’affichage du format de table avec `vnet-gateway list-bgp-peer-status`</span><span class="sxs-lookup"><span data-stu-id="de833-917">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="de833-918">Ajout des commandes `list-request-headers` et `list-response-headers` à `application-gateway rewrite-rule`</span><span class="sxs-lookup"><span data-stu-id="de833-918">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="de833-919">Ajout de la commande `list-server-variables` à `application-gateway rewrite-rule condition`</span><span class="sxs-lookup"><span data-stu-id="de833-919">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="de833-920">Correction du problème où la mise à jour de l’état d’une liaison sur un port express-route levait une exception d’attribut inconnu `express-route port update`</span><span class="sxs-lookup"><span data-stu-id="de833-920">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="de833-921">PrivateDNS</span><span class="sxs-lookup"><span data-stu-id="de833-921">PrivateDNS</span></span>
* <span data-ttu-id="de833-922">Ajout de `network private-dns` pour les zones de DNS privé</span><span class="sxs-lookup"><span data-stu-id="de833-922">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="de833-923">Ressource</span><span class="sxs-lookup"><span data-stu-id="de833-923">Resource</span></span>
* <span data-ttu-id="de833-924">Correction du problème avec `deployment create` et `group deployment create` où un fichier de paramètres avec un ensemble de paramètres vide ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="de833-924">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="de833-925">Role</span><span class="sxs-lookup"><span data-stu-id="de833-925">Role</span></span>
* <span data-ttu-id="de833-926">Correction de `create-for-rbac` pour gérer `--years` correctement</span><span class="sxs-lookup"><span data-stu-id="de833-926">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="de833-927">[CHANGEMENT CASSANT] Changement apporté à `role assignment delete` pour afficher une invite lors d’une suppression sans condition de toutes les attributions sous l’abonnement</span><span class="sxs-lookup"><span data-stu-id="de833-927">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="de833-928">SQL</span><span class="sxs-lookup"><span data-stu-id="de833-928">SQL</span></span>
* <span data-ttu-id="de833-929">Mise à jour de `sql mi [create|update]` avec les propriétés proxyOverride et publicDataEndpointEnabledd</span><span class="sxs-lookup"><span data-stu-id="de833-929">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="de833-930">Stockage</span><span class="sxs-lookup"><span data-stu-id="de833-930">Storage</span></span>
* <span data-ttu-id="de833-931">[CHANGEMENT CASSANT] Suppression du résultat de `storage blob delete`</span><span class="sxs-lookup"><span data-stu-id="de833-931">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="de833-932">Ajout de `--full-uri` à `storage blob generate-sas` pour créer l’URI complet pour l’objet blob avec SAS</span><span class="sxs-lookup"><span data-stu-id="de833-932">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="de833-933">Ajout de `--file-snapshot` à `storage file copy start` pour copier le fichier à partir de l’instantané</span><span class="sxs-lookup"><span data-stu-id="de833-933">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="de833-934">Changement apporté à `storage blob copy cancel` pour afficher uniquement l’erreur au lieu de l’exception pour NoPendingCopyOperation</span><span class="sxs-lookup"><span data-stu-id="de833-934">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="de833-935">26 mars 2019</span><span class="sxs-lookup"><span data-stu-id="de833-935">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="de833-936">Core</span><span class="sxs-lookup"><span data-stu-id="de833-936">Core</span></span>
* <span data-ttu-id="de833-937">Résolution des problèmes d’incompatibilité des extensions de développement</span><span class="sxs-lookup"><span data-stu-id="de833-937">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="de833-938">La gestion des erreurs redirige les clients vers la page des problèmes</span><span class="sxs-lookup"><span data-stu-id="de833-938">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="de833-939">Cloud</span><span class="sxs-lookup"><span data-stu-id="de833-939">Cloud</span></span>
* <span data-ttu-id="de833-940">Correction d’une erreur « abonnement introuvable » dans `cloud set`</span><span class="sxs-lookup"><span data-stu-id="de833-940">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="de833-941">ACR</span><span class="sxs-lookup"><span data-stu-id="de833-941">ACR</span></span>
* <span data-ttu-id="de833-942">Correction d’un problème concernant des sources redondantes lors de l’importation d’images</span><span class="sxs-lookup"><span data-stu-id="de833-942">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="de833-943">Ajout de `--auth-mode` aux commandes `acr build`, `acr run`, `acr task create` et `acr task update`</span><span class="sxs-lookup"><span data-stu-id="de833-943">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="de833-944">Ajout du groupe de commandes 'acr task credential' pour la gestion des informations d’identification pour une tâche</span><span class="sxs-lookup"><span data-stu-id="de833-944">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="de833-945">Ajout de '--no-wait' à la commande `acr build`</span><span class="sxs-lookup"><span data-stu-id="de833-945">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="de833-946">AppService</span><span class="sxs-lookup"><span data-stu-id="de833-946">AppService</span></span>
* <span data-ttu-id="de833-947">Correction du bogue où `webapp up` ne gérait pas correctement l’exécution dans un scénario de répertoire vide ou de code inconnu</span><span class="sxs-lookup"><span data-stu-id="de833-947">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="de833-948">Correction du bogue où les emplacements ne fonctionnaient pas pour `[webapp|functionapp] config ssl bind`</span><span class="sxs-lookup"><span data-stu-id="de833-948">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="de833-949">Service BOT</span><span class="sxs-lookup"><span data-stu-id="de833-949">BOT Service</span></span>
* <span data-ttu-id="de833-950">Ajout de `bot prepare-deploy` pour préparer le déploiement de bots via `webapp`</span><span class="sxs-lookup"><span data-stu-id="de833-950">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="de833-951">Modification de `bot create --kind registration` pour afficher le mot de passe si celui-ci n’est pas fourni</span><span class="sxs-lookup"><span data-stu-id="de833-951">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="de833-952">[CHANGEMENT CASSANT] Changement de `--endpoint` dans `bot create --kind registration` pour qu’il soit par défaut dans une chaîne vide au lieu d’être requis</span><span class="sxs-lookup"><span data-stu-id="de833-952">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="de833-953">Ajout de `SCM_DO_BUILD_DURING_DEPLOYMENT` aux paramètres d’application du modèle ARM pour Web App Bots v4</span><span class="sxs-lookup"><span data-stu-id="de833-953">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="de833-954">CDN</span><span class="sxs-lookup"><span data-stu-id="de833-954">CDN</span></span>
* <span data-ttu-id="de833-955">Ajout de la prise en charge de `--no-wait` pour `cdn endpoint [create|update|start|stop|delete|load|purge]`</span><span class="sxs-lookup"><span data-stu-id="de833-955">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* <span data-ttu-id="de833-956">[CHANGEMENT CASSANT] : Changement du comportement de mise en cache de chaînes de requête par défaut de `cdn endpoint create`.</span><span class="sxs-lookup"><span data-stu-id="de833-956">[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour.</span></span> <span data-ttu-id="de833-957">Sa valeur par défaut n’est plus « IgnoreQueryString ».</span><span class="sxs-lookup"><span data-stu-id="de833-957">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="de833-958">Il est maintenant défini par le service</span><span class="sxs-lookup"><span data-stu-id="de833-958">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="de833-959">Cosmosdb</span><span class="sxs-lookup"><span data-stu-id="de833-959">Cosmosdb</span></span>
* <span data-ttu-id="de833-960">Ajout de la prise en charge de `--enable-multiple-write-locations` lors de la mise à jour de compte</span><span class="sxs-lookup"><span data-stu-id="de833-960">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="de833-961">Ajout du sous-groupe `network-rule` avec les commandes `add`, `remove` et `list` pour gérer les règles de réseau virtuel d’un compte Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="de833-961">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="de833-962">Interactive</span><span class="sxs-lookup"><span data-stu-id="de833-962">Interactive</span></span>
* <span data-ttu-id="de833-963">Correction d’une incompatibilité avec l’extension Interactive installée via azdev</span><span class="sxs-lookup"><span data-stu-id="de833-963">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="de833-964">Moniteur</span><span class="sxs-lookup"><span data-stu-id="de833-964">Monitor</span></span>
* <span data-ttu-id="de833-965">Changement visant à autoriser la valeur de dimension `*` pour `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="de833-965">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="de833-966">Réseau</span><span class="sxs-lookup"><span data-stu-id="de833-966">Network</span></span>
* <span data-ttu-id="de833-967">Ajout du groupe de commandes `rewrite-rule` à `application-gateway`</span><span class="sxs-lookup"><span data-stu-id="de833-967">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="de833-968">Profil</span><span class="sxs-lookup"><span data-stu-id="de833-968">Profile</span></span>
* <span data-ttu-id="de833-969">Ajout de la prise en charge du compte de niveau locataire pour Managed Service Identity dans `login`</span><span class="sxs-lookup"><span data-stu-id="de833-969">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="de833-970">Postgres</span><span class="sxs-lookup"><span data-stu-id="de833-970">Postgres</span></span> 
* <span data-ttu-id="de833-971">Ajout des commandes `replica` et de la commande `restart server` postgresql</span><span class="sxs-lookup"><span data-stu-id="de833-971">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="de833-972">Changement permettant d’obtenir l’emplacement par défaut du groupe de ressources lorsqu’il n’a pas été fourni, pour la création de serveurs et l’ajout d’une validation pour les jours de conservation</span><span class="sxs-lookup"><span data-stu-id="de833-972">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="de833-973">Ressource</span><span class="sxs-lookup"><span data-stu-id="de833-973">Resource</span></span>
* <span data-ttu-id="de833-974">Amélioration de la sortie de table pour `deployment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="de833-974">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="de833-975">Correction du problème avec `deployment [create|validate]` où le secureObject de type n’était pas reconnu</span><span class="sxs-lookup"><span data-stu-id="de833-975">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="de833-976">Graph</span><span class="sxs-lookup"><span data-stu-id="de833-976">Graph</span></span>
* <span data-ttu-id="de833-977">Ajout de la prise en charge de `--end-date` pour `ad [app|sp] credential reset`</span><span class="sxs-lookup"><span data-stu-id="de833-977">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="de833-978">Ajout de la prise en charge permettant d’ajouter des autorisations avec `ad app permission add`</span><span class="sxs-lookup"><span data-stu-id="de833-978">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="de833-979">Correction d’un bogue avec `ad app permission list` où il n’existait aucune autorisation</span><span class="sxs-lookup"><span data-stu-id="de833-979">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="de833-980">Modification de `ad sp delete` pour ignorer la suppression d’attribution de rôle si le compte actuel n’a aucun abonnement</span><span class="sxs-lookup"><span data-stu-id="de833-980">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="de833-981">Modification de `ad app create` pour avoir `--identifier-uris` par défaut dans une liste vide si non fourni</span><span class="sxs-lookup"><span data-stu-id="de833-981">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="de833-982">storage</span><span class="sxs-lookup"><span data-stu-id="de833-982">storage</span></span>
* <span data-ttu-id="de833-983">Ajout de `--snapshot` à `storage file download-batch` pour télécharger depuis un instantané de partage</span><span class="sxs-lookup"><span data-stu-id="de833-983">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="de833-984">Modification de la barre de progression `storage blob [download-batch|upload-batch]` pour qu’elle soit moins détaillée et qu’elle indique les objets blob actuels</span><span class="sxs-lookup"><span data-stu-id="de833-984">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="de833-985">Correction du problème avec `storage account update` lors de la mise à jour des paramètres de chiffrement</span><span class="sxs-lookup"><span data-stu-id="de833-985">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="de833-986">Correction d’un problème où `storage blob show` échouait quand oauth était utilisé (`--auth-mode=login`)</span><span class="sxs-lookup"><span data-stu-id="de833-986">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="de833-987">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="de833-987">VM</span></span>
* <span data-ttu-id="de833-988">Ajout de la commande `image update`</span><span class="sxs-lookup"><span data-stu-id="de833-988">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="de833-989">12 mars 2019</span><span class="sxs-lookup"><span data-stu-id="de833-989">March 12, 2019</span></span>

<span data-ttu-id="de833-990">Version 2.0.60</span><span class="sxs-lookup"><span data-stu-id="de833-990">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="de833-991">Core</span><span class="sxs-lookup"><span data-stu-id="de833-991">Core</span></span>

* <span data-ttu-id="de833-992">Correction d’une erreur dans `cloud set` concernant un abonnement introuvable</span><span class="sxs-lookup"><span data-stu-id="de833-992">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="de833-993">ACR</span><span class="sxs-lookup"><span data-stu-id="de833-993">ACR</span></span>

* <span data-ttu-id="de833-994">Correction d’un problème concernant des sources redondantes lors de l’importation d’images</span><span class="sxs-lookup"><span data-stu-id="de833-994">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="de833-995">ACS</span><span class="sxs-lookup"><span data-stu-id="de833-995">ACS</span></span>

* <span data-ttu-id="de833-996">Changement apporté pour que le paramètre `--listen-address` dans `aks browse` soit ignoré s’il n’est pas pris en charge par kubectl</span><span class="sxs-lookup"><span data-stu-id="de833-996">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="de833-997">AppService</span><span class="sxs-lookup"><span data-stu-id="de833-997">AppService</span></span>

* <span data-ttu-id="de833-998">Ajout de `[webapp|functionapp] deployment list-publishing-credentials` pour obtenir l’URL de publication Kudu et ses informations d’identification</span><span class="sxs-lookup"><span data-stu-id="de833-998">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="de833-999">Suppression d’une instruction print erronée pour `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="de833-999">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="de833-1000">Correction de `functionapp` pour définir la bonne image runtime dans les plans App Service Linux</span><span class="sxs-lookup"><span data-stu-id="de833-1000">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="de833-1001">Suppression de l’étiquette de préversion pour `webapp up` et ajout d’améliorations à la commande</span><span class="sxs-lookup"><span data-stu-id="de833-1001">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="de833-1002">Botservice</span><span class="sxs-lookup"><span data-stu-id="de833-1002">Botservice</span></span>

* <span data-ttu-id="de833-1003">Ajout de `SCM_DO_BUILD_DURING_DEPLOYMENT` aux paramètres d’application du modèle ARM pour Web App Bots v4</span><span class="sxs-lookup"><span data-stu-id="de833-1003">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="de833-1004">Ajout de `Microsoft-BotFramework-AppId` et de `Microsoft-BotFramework-AppPassword` aux paramètres d’application du modèle ARM pour Web App Bots v4</span><span class="sxs-lookup"><span data-stu-id="de833-1004">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="de833-1005">Suppression des guillemets simples dans la sortie de la commande `bot publish`, à la fin de `bot create`</span><span class="sxs-lookup"><span data-stu-id="de833-1005">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="de833-1006">Modification de `bot publish` pour le rendre asynchrone</span><span class="sxs-lookup"><span data-stu-id="de833-1006">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="de833-1007">Conteneur</span><span class="sxs-lookup"><span data-stu-id="de833-1007">Container</span></span>

* <span data-ttu-id="de833-1008">Ajout de l’argument `--no-wait` à `container [start|restart]`</span><span class="sxs-lookup"><span data-stu-id="de833-1008">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="de833-1009">Event Hub</span><span class="sxs-lookup"><span data-stu-id="de833-1009">EventHub</span></span>

* <span data-ttu-id="de833-1010">Ajout de l’indicateur `--skip-empty-archives` à `eventhub create|update` pour prendre en charge les archives vides dans les captures</span><span class="sxs-lookup"><span data-stu-id="de833-1010">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="de833-1011">Rechercher</span><span class="sxs-lookup"><span data-stu-id="de833-1011">Find</span></span>

* <span data-ttu-id="de833-1012">Mise à jour importante de fonctionnalités</span><span class="sxs-lookup"><span data-stu-id="de833-1012">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="de833-1013">HDInsight</span><span class="sxs-lookup"><span data-stu-id="de833-1013">HDInsight</span></span>

* <span data-ttu-id="de833-1014">Ajout du paramètre `--storage-account-managed-identity` à `hdinsight create` pour prendre en charge le MSI ADLS Gen2</span><span class="sxs-lookup"><span data-stu-id="de833-1014">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="de833-1015">Réseau</span><span class="sxs-lookup"><span data-stu-id="de833-1015">Network</span></span>

* <span data-ttu-id="de833-1016">Correction d’un problème concernant `vpn-connection update`, qui provoquait l’échec de la mise à jour d’une connexion VPN établie entre deux passerelles appartenant à des abonnements différents</span><span class="sxs-lookup"><span data-stu-id="de833-1016">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="de833-1017">Rdbms</span><span class="sxs-lookup"><span data-stu-id="de833-1017">Rdbms</span></span>

* <span data-ttu-id="de833-1018">Correctifs mineurs permettant d’obtenir l’emplacement par défaut du groupe de ressources lorsqu’il n’a pas été fourni, pour la création de serveurs et l’ajout d’une validation pour les jours de rétention</span><span class="sxs-lookup"><span data-stu-id="de833-1018">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="de833-1019">Role</span><span class="sxs-lookup"><span data-stu-id="de833-1019">Role</span></span>

* <span data-ttu-id="de833-1020">Correction de `role definition update` pour utiliser l’ID afin de résoudre correctement les définitions</span><span class="sxs-lookup"><span data-stu-id="de833-1020">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="de833-1021">Modification de `ad app credential reset` pour ne plus partir du principe que le principal de service de l’application existe toujours</span><span class="sxs-lookup"><span data-stu-id="de833-1021">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="de833-1022">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="de833-1022">Service Fabric</span></span>

* <span data-ttu-id="de833-1023">Correction du problème où `sf cluster list` n’était pas itérable</span><span class="sxs-lookup"><span data-stu-id="de833-1023">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="de833-1024">26 février 2019</span><span class="sxs-lookup"><span data-stu-id="de833-1024">February 26, 2019</span></span>

<span data-ttu-id="de833-1025">Version 2.0.59</span><span class="sxs-lookup"><span data-stu-id="de833-1025">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="de833-1026">Core</span><span class="sxs-lookup"><span data-stu-id="de833-1026">Core</span></span>

* <span data-ttu-id="de833-1027">Correction du problème où l’utilisation de `--subscription NAME` levait une exception dans certains cas</span><span class="sxs-lookup"><span data-stu-id="de833-1027">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="de833-1028">ACR</span><span class="sxs-lookup"><span data-stu-id="de833-1028">ACR</span></span>

* <span data-ttu-id="de833-1029">Ajout du paramètre `--target` pour les commandes `acr build`, `acr task create` et `acr task update`</span><span class="sxs-lookup"><span data-stu-id="de833-1029">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="de833-1030">Amélioration de la gestion des erreurs pour les commandes de runtime quand vous n’êtes pas connecté à Azure</span><span class="sxs-lookup"><span data-stu-id="de833-1030">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="de833-1031">ACS</span><span class="sxs-lookup"><span data-stu-id="de833-1031">ACS</span></span>

* <span data-ttu-id="de833-1032">Ajout de l’option `--listen-address` à `aks port-forward`</span><span class="sxs-lookup"><span data-stu-id="de833-1032">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="de833-1033">AppService</span><span class="sxs-lookup"><span data-stu-id="de833-1033">AppService</span></span>

* <span data-ttu-id="de833-1034">Ajout de la commande `functionapp devops-build`</span><span class="sxs-lookup"><span data-stu-id="de833-1034">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="de833-1035">Batch</span><span class="sxs-lookup"><span data-stu-id="de833-1035">Batch</span></span>
* <span data-ttu-id="de833-1036">[CHANGEMENT CASSANT] Suppression de la commande `batch pool upgrade os`</span><span class="sxs-lookup"><span data-stu-id="de833-1036">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="de833-1037">[CHANGEMENT CASSANT] Suppression de la propriété `Pacakges` des réponses `Application`</span><span class="sxs-lookup"><span data-stu-id="de833-1037">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="de833-1038">Ajout de la commande `batch application package list` pour lister les packages d’une application</span><span class="sxs-lookup"><span data-stu-id="de833-1038">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="de833-1039">[CHANGEMENT CASSANT] Remplacement de `--application-id` par `--application-name` dans toutes les commandes `batch application`</span><span class="sxs-lookup"><span data-stu-id="de833-1039">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="de833-1040">Ajout de l’argument `--json-file` aux commandes permettant de demander la réponse d’API brute</span><span class="sxs-lookup"><span data-stu-id="de833-1040">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="de833-1041">Mise à jour de la validation pour inclure automatiquement `https://` dans tous les points de terminaison si manquant</span><span class="sxs-lookup"><span data-stu-id="de833-1041">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="de833-1042">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="de833-1042">CosmosDB</span></span>

* <span data-ttu-id="de833-1043">Ajout du sous-groupe `network-rule` avec les commandes `add`, `remove` et `list` pour gérer les règles de réseau virtuel d’un compte Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="de833-1043">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="de833-1044">Kusto</span><span class="sxs-lookup"><span data-stu-id="de833-1044">Kusto</span></span>

* <span data-ttu-id="de833-1045">[CHANGEMENT CASSANT] Changement des types `hot_cache_period` et `soft_delete_period` de la base de données en format de durée ISO8601</span><span class="sxs-lookup"><span data-stu-id="de833-1045">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="de833-1046">Réseau</span><span class="sxs-lookup"><span data-stu-id="de833-1046">Network</span></span>

* <span data-ttu-id="de833-1047">Ajout de l’argument `--express-route-gateway-bypass` à `vpn-connection [create|update]`</span><span class="sxs-lookup"><span data-stu-id="de833-1047">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="de833-1048">Ajout de groupes de commandes à partir des extensions `express-route`</span><span class="sxs-lookup"><span data-stu-id="de833-1048">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="de833-1049">Ajout des groupes de commandes `express-route gateway` et `express-route port`</span><span class="sxs-lookup"><span data-stu-id="de833-1049">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="de833-1050">Ajout d’un argument `--legacy-mode` à `express-route peering [create|update]`</span><span class="sxs-lookup"><span data-stu-id="de833-1050">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="de833-1051">Ajout des arguments `--allow-classic-operations` et `--express-route-port` à `express-route [create|update]`</span><span class="sxs-lookup"><span data-stu-id="de833-1051">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="de833-1052">Ajout de l’argument `--gateway-default-site` à `vnet-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="de833-1052">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="de833-1053">Ajout des commandes `ipsec-policy` à `vnet-gateway`</span><span class="sxs-lookup"><span data-stu-id="de833-1053">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="de833-1054">Ressource</span><span class="sxs-lookup"><span data-stu-id="de833-1054">Resource</span></span>

* <span data-ttu-id="de833-1055">Correction du problème de `deployment create` où le champ de type n’était pas sensible à la casse</span><span class="sxs-lookup"><span data-stu-id="de833-1055">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="de833-1056">Ajout de la prise en charge du fichier de paramètres basé sur l’URI sur `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="de833-1056">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="de833-1057">Ajout de la prise en charge des définitions et des paramètres basés sur l’URI sur `policy set-definition update`</span><span class="sxs-lookup"><span data-stu-id="de833-1057">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="de833-1058">Correction de la gestion des paramètres et des règles pour `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="de833-1058">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="de833-1059">Correction du problème avec `resource show/update/delete/tag/invoke-action` où les ID inter-abonnements n’honoraient pas correctement l’ID d’abonnement</span><span class="sxs-lookup"><span data-stu-id="de833-1059">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="de833-1060">Role</span><span class="sxs-lookup"><span data-stu-id="de833-1060">Role</span></span>

* <span data-ttu-id="de833-1061">Ajout de la prise en charge des rôles d’application sur `ad app [create|update]`</span><span class="sxs-lookup"><span data-stu-id="de833-1061">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="de833-1062">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="de833-1062">VM</span></span>

* <span data-ttu-id="de833-1063">Correction du problème avec `vm create where `--accelerated-networking\` qui n’était pas activé par défaut pour Ubuntu 18.0</span><span class="sxs-lookup"><span data-stu-id="de833-1063">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="de833-1064">12 février 2019</span><span class="sxs-lookup"><span data-stu-id="de833-1064">February 12, 2019</span></span>

<span data-ttu-id="de833-1065">Version 2.0.58</span><span class="sxs-lookup"><span data-stu-id="de833-1065">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="de833-1066">Core</span><span class="sxs-lookup"><span data-stu-id="de833-1066">Core</span></span>

* <span data-ttu-id="de833-1067">`az --version` affiche désormais une notification si vous avez des packages qui peuvent être mis à jour</span><span class="sxs-lookup"><span data-stu-id="de833-1067">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="de833-1068">Correction de la régression où `--ids` ne pouvait plus être utilisé avec une sortie JSON</span><span class="sxs-lookup"><span data-stu-id="de833-1068">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="de833-1069">ACR</span><span class="sxs-lookup"><span data-stu-id="de833-1069">ACR</span></span>
* <span data-ttu-id="de833-1070">[CHANGEMENT CASSANT] Suppression du groupe de commandes `acr build-task`</span><span class="sxs-lookup"><span data-stu-id="de833-1070">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="de833-1071">[CHANGEMENT CASSANT] Suppression des options `--tag` et `--manifest` dans `acr repository delete`</span><span class="sxs-lookup"><span data-stu-id="de833-1071">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="de833-1072">ACS</span><span class="sxs-lookup"><span data-stu-id="de833-1072">ACS</span></span>
* <span data-ttu-id="de833-1073">Ajout de la prise en charge des noms qui ne respectent pas la casse à `aks [enable-addons|disable-addons]`</span><span class="sxs-lookup"><span data-stu-id="de833-1073">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="de833-1074">Ajout de la prise en charge de l’opération de mise à jour d’Azure Active Directory à l’aide de `aks update-credentials --reset-aad`</span><span class="sxs-lookup"><span data-stu-id="de833-1074">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="de833-1075">Ajout d’une clarification indiquant que `--output` est ignoré pour `aks get-credentials`</span><span class="sxs-lookup"><span data-stu-id="de833-1075">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="de833-1076">AMS</span><span class="sxs-lookup"><span data-stu-id="de833-1076">AMS</span></span>
* <span data-ttu-id="de833-1077">Ajout des commandes `ams streaming-endpoint [start | stop | create | update] wait`</span><span class="sxs-lookup"><span data-stu-id="de833-1077">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="de833-1078">Ajout des commandes `ams live-event [create | start | stop | reset] wait`</span><span class="sxs-lookup"><span data-stu-id="de833-1078">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="de833-1079">AppService</span><span class="sxs-lookup"><span data-stu-id="de833-1079">Appservice</span></span>
* <span data-ttu-id="de833-1080">Ajout des possibilités de création et de configuration de fonctions à l’aide de conteneurs ACR</span><span class="sxs-lookup"><span data-stu-id="de833-1080">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="de833-1081">Ajout de la prise en charge de la mise à jour des configurations d’applications web via JSON</span><span class="sxs-lookup"><span data-stu-id="de833-1081">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="de833-1082">Amélioration de l’aide pour `appservice-plan-update`</span><span class="sxs-lookup"><span data-stu-id="de833-1082">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="de833-1083">Ajout de la prise en charge d’Application Insights sur functionapp create</span><span class="sxs-lookup"><span data-stu-id="de833-1083">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="de833-1084">Résolution des problèmes liés à webapp SSH</span><span class="sxs-lookup"><span data-stu-id="de833-1084">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="de833-1085">Botservice</span><span class="sxs-lookup"><span data-stu-id="de833-1085">Botservice</span></span>
* <span data-ttu-id="de833-1086">Amélioration de l’expérience utilisateur pour `bot publish`</span><span class="sxs-lookup"><span data-stu-id="de833-1086">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="de833-1087">Ajout d’un avertissement pour les délais d’expiration au moment de l’exécution de `npm install` durant `az bot publish`</span><span class="sxs-lookup"><span data-stu-id="de833-1087">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="de833-1088">Suppression du caractère non valide `.` de `--name` dans `az bot create`</span><span class="sxs-lookup"><span data-stu-id="de833-1088">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="de833-1089">Changement apporté pour mettre fin aux noms de ressources aléatoires durant la création du Stockage Azure, du plan App Service, de Function App/Web App et d’Application Insights</span><span class="sxs-lookup"><span data-stu-id="de833-1089">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="de833-1090">[DÉPRÉCIATION] Dépréciation de l’argument `--proj-name` en faveur de `--proj-file-path`</span><span class="sxs-lookup"><span data-stu-id="de833-1090">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="de833-1091">Changement apporté à `az bot publish` pour supprimer les fichiers de déploiements IIS Node.js récupérés (fetch), s’ils n’existent pas déjà</span><span class="sxs-lookup"><span data-stu-id="de833-1091">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="de833-1092">Ajout de l’argument `--keep-node-modules` à `az bot publish` pour éviter la suppression du dossier `node_modules` dans App Service</span><span class="sxs-lookup"><span data-stu-id="de833-1092">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="de833-1093">Ajout de la paire clé/valeur `"publishCommand"` à la sortie de `az bot create` au moment de la création d’une fonction Azure ou d’un bot Web App</span><span class="sxs-lookup"><span data-stu-id="de833-1093">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="de833-1094">La valeur de `"publishCommand"` est une commande `az bot publish` préremplie avec les paramètres obligatoires pour publier le bot venant d’être créé</span><span class="sxs-lookup"><span data-stu-id="de833-1094">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="de833-1095">Mise à jour de `"WEBSITE_NODE_DEFAULT_VERSION"` dans le modèle ARM pour permettre aux bots du kit SDK v4 d’utiliser la version 10.14.1 au lieu de la version 8.9.4</span><span class="sxs-lookup"><span data-stu-id="de833-1095">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="de833-1096">Key Vault</span><span class="sxs-lookup"><span data-stu-id="de833-1096">Key Vault</span></span>
* <span data-ttu-id="de833-1097">Correction du problème lié à `keyvault secret backup`, où certains utilisateurs recevaient une erreur `unexpected_keyword` quand ils utilisaient `--id`</span><span class="sxs-lookup"><span data-stu-id="de833-1097">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="de833-1098">Moniteur</span><span class="sxs-lookup"><span data-stu-id="de833-1098">Monitor</span></span>
* <span data-ttu-id="de833-1099">Changement apporté à `monitor metrics alert [create|update]` pour autoriser la valeur de dimension `*`</span><span class="sxs-lookup"><span data-stu-id="de833-1099">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="de833-1100">Réseau</span><span class="sxs-lookup"><span data-stu-id="de833-1100">Network</span></span>
* <span data-ttu-id="de833-1101">Changement apporté à `dns zone export` pour que les enregistrements CNAME exportés soient des noms de domaine complets</span><span class="sxs-lookup"><span data-stu-id="de833-1101">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="de833-1102">Ajout du paramètre `--gateway-name` à `nic ip-config address-pool [add|remove]` pour permettre la prise en charge des pools d’adresses back-end d’Application Gateway</span><span class="sxs-lookup"><span data-stu-id="de833-1102">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="de833-1103">Ajout des arguments `--traffic-analytics` et `--workspace` à `network watcher flow-log configure` pour permettre la prise en charge de l’analyse du trafic via un espace de travail Log Analytics</span><span class="sxs-lookup"><span data-stu-id="de833-1103">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="de833-1104">Ajout de `--idle-timeout` et `--floating-ip` à `lb inbound-nat-pool [create|update]`</span><span class="sxs-lookup"><span data-stu-id="de833-1104">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="de833-1105">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="de833-1105">Policy Insights</span></span>
* <span data-ttu-id="de833-1106">Ajout des commandes `policy remediation` pour permettre la prise en charge des fonctionnalités de correction des stratégies de ressources</span><span class="sxs-lookup"><span data-stu-id="de833-1106">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="de833-1107">SGBDR</span><span class="sxs-lookup"><span data-stu-id="de833-1107">RDBMS</span></span>
* <span data-ttu-id="de833-1108">Amélioration du message d’aide et des paramètres de commande</span><span class="sxs-lookup"><span data-stu-id="de833-1108">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="de833-1109">Redis</span><span class="sxs-lookup"><span data-stu-id="de833-1109">Redis</span></span>
* <span data-ttu-id="de833-1110">Ajout de commandes pour la gestion des règles de pare-feu (create, update, delete, show, list)</span><span class="sxs-lookup"><span data-stu-id="de833-1110">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="de833-1111">Ajout de commandes pour la gestion de la liaison avec le serveur (create, delete, show, list)</span><span class="sxs-lookup"><span data-stu-id="de833-1111">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="de833-1112">Ajout de commandes pour la gestion de la planification des correctifs (create, update, delete, show)</span><span class="sxs-lookup"><span data-stu-id="de833-1112">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="de833-1113">Ajout de la prise en charge des zones de disponibilité et de la version minimale de TLS dans redis create</span><span class="sxs-lookup"><span data-stu-id="de833-1113">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="de833-1114">[CHANGEMENT CASSANT] Suppression des commandes `redis update-settings` et `redis list-all`</span><span class="sxs-lookup"><span data-stu-id="de833-1114">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="de833-1115">[CHANGEMENT CASSANT] Le paramètre de `redis create` : « paramètres du locataire » n’est pas accepté au format clé[=valeur]</span><span class="sxs-lookup"><span data-stu-id="de833-1115">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="de833-1116">[DÉPRÉCIATION] Ajout d’un message d’avertissement concernant la dépréciation de la commande `redis import-method`</span><span class="sxs-lookup"><span data-stu-id="de833-1116">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="de833-1117">Role</span><span class="sxs-lookup"><span data-stu-id="de833-1117">Role</span></span>
* <span data-ttu-id="de833-1118">[CHANGEMENT CASSANT] Déplacement de la commande `az identity` ici à partir des commandes `vm`</span><span class="sxs-lookup"><span data-stu-id="de833-1118">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="de833-1119">Machine virtuelle SQL</span><span class="sxs-lookup"><span data-stu-id="de833-1119">SQL VM</span></span>
* <span data-ttu-id="de833-1120">[DÉPRÉCIATION] Dépréciation de l’argument `--boostrap-acc-pwd` en raison d’une faute de frappe</span><span class="sxs-lookup"><span data-stu-id="de833-1120">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="de833-1121">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="de833-1121">VM</span></span>
* <span data-ttu-id="de833-1122">Changement de `vm list-skus` pour autoriser l’utilisation de `--all` à la place de `--all true`</span><span class="sxs-lookup"><span data-stu-id="de833-1122">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="de833-1123">Ajout de `vmss run-command [invoke | list | show]`</span><span class="sxs-lookup"><span data-stu-id="de833-1123">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="de833-1124">Correction d’un bogue qui entraînait l’échec de `vmss encryption enable`, s’il était exécuté</span><span class="sxs-lookup"><span data-stu-id="de833-1124">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="de833-1125">[CHANGEMENT CASSANT] Déplacement de la commande `az identity` vers les commandes `role`</span><span class="sxs-lookup"><span data-stu-id="de833-1125">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="de833-1126">31 janvier 2019</span><span class="sxs-lookup"><span data-stu-id="de833-1126">January 31, 2019</span></span>

<span data-ttu-id="de833-1127">Version 2.0.57</span><span class="sxs-lookup"><span data-stu-id="de833-1127">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="de833-1128">Core</span><span class="sxs-lookup"><span data-stu-id="de833-1128">Core</span></span>

* <span data-ttu-id="de833-1129">Correctif pour le [problème 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="de833-1129">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="de833-1130">28 janvier 2019</span><span class="sxs-lookup"><span data-stu-id="de833-1130">January 28, 2019</span></span>

<span data-ttu-id="de833-1131">Version 2.0.56</span><span class="sxs-lookup"><span data-stu-id="de833-1131">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="de833-1132">ACR</span><span class="sxs-lookup"><span data-stu-id="de833-1132">ACR</span></span>
* <span data-ttu-id="de833-1133">Ajout de la prise en charge des règles de réseau virtuel (VNet)/d’adresses IP</span><span class="sxs-lookup"><span data-stu-id="de833-1133">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="de833-1134">ACS</span><span class="sxs-lookup"><span data-stu-id="de833-1134">ACS</span></span>
* <span data-ttu-id="de833-1135">Ajout de l’aperçu des nœuds virtuels</span><span class="sxs-lookup"><span data-stu-id="de833-1135">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="de833-1136">Ajout des commandes d’OpenShift managé</span><span class="sxs-lookup"><span data-stu-id="de833-1136">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="de833-1137">Ajout de la prise en charge des mises à jour du principal de service avec `aks update-credentials -reset-service-principal`</span><span class="sxs-lookup"><span data-stu-id="de833-1137">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="de833-1138">AMS</span><span class="sxs-lookup"><span data-stu-id="de833-1138">AMS</span></span>
* <span data-ttu-id="de833-1139">[CHANGEMENT CASSANT] Renommage de `ams asset get-streaming-locators` en `ams asset list-streaming-locators`</span><span class="sxs-lookup"><span data-stu-id="de833-1139">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="de833-1140">[CHANGEMENT CASSANT] Renommage de `ams streaming-locator get-content-keys` en `ams streaming-locator list-content-keys`</span><span class="sxs-lookup"><span data-stu-id="de833-1140">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="de833-1141">AppService</span><span class="sxs-lookup"><span data-stu-id="de833-1141">Appservice</span></span>
* <span data-ttu-id="de833-1142">Ajout de la prise en charge d’Application Insights sur `functionapp create`</span><span class="sxs-lookup"><span data-stu-id="de833-1142">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="de833-1143">Ajout de la prise en charge de la création de plans App Service (notamment Elastic Premium) à Function App</span><span class="sxs-lookup"><span data-stu-id="de833-1143">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="de833-1144">Correction de problèmes de configuration des applications avec les plans Elastic Premium</span><span class="sxs-lookup"><span data-stu-id="de833-1144">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="de833-1145">Conteneur</span><span class="sxs-lookup"><span data-stu-id="de833-1145">Container</span></span>
* <span data-ttu-id="de833-1146">Ajout de la commande `container start`</span><span class="sxs-lookup"><span data-stu-id="de833-1146">Added `container start` command</span></span>
* <span data-ttu-id="de833-1147">Changements apportés afin de permettre l’utilisation de valeurs décimales pour le processeur durant la création d’un conteneur</span><span class="sxs-lookup"><span data-stu-id="de833-1147">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="de833-1148">EventGrid</span><span class="sxs-lookup"><span data-stu-id="de833-1148">EventGrid</span></span>
* <span data-ttu-id="de833-1149">Ajout du paramètre `--deadletter-endpoint` pour `event-subscription [create|update]`</span><span class="sxs-lookup"><span data-stu-id="de833-1149">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="de833-1150">Ajout de storagequeue et hybridconnection en tant que nouvelles valeurs pour « event-subscription [create|update] --endpoint-type »</span><span class="sxs-lookup"><span data-stu-id="de833-1150">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="de833-1151">Ajout des paramètres `--max-delivery-attempts` et `--event-ttl` à `event-subscription create` pour spécifier la stratégie de nouvelles tentatives des événements</span><span class="sxs-lookup"><span data-stu-id="de833-1151">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="de833-1152">Ajout d’un message d’avertissement à `event-subscription [create|update]` en cas d’utilisation de Webhook en tant que destination pour un abonnement à un événement</span><span class="sxs-lookup"><span data-stu-id="de833-1152">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="de833-1153">Ajout du paramètre source-resource-id pour toutes les commandes relatives à un abonnement aux événements et marquage de tous les autres paramètres relatifs aux ressources sources comme étant dépréciés</span><span class="sxs-lookup"><span data-stu-id="de833-1153">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="de833-1154">HDInsight</span><span class="sxs-lookup"><span data-stu-id="de833-1154">HDInsight</span></span>
* <span data-ttu-id="de833-1155">[CHANGEMENT CASSANT] Suppression des paramètres `--virtual-network` et `--subnet-name` dans `hdinsight [application] create`</span><span class="sxs-lookup"><span data-stu-id="de833-1155">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="de833-1156">[CHANGEMENT CASSANT] Changement apporté à `hdinsight create --storage-account` pour accepter le nom ou l’ID du compte de stockage à la place des points de terminaison d’objet blob</span><span class="sxs-lookup"><span data-stu-id="de833-1156">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="de833-1157">Ajout des paramètres `--vnet-name` et `--subnet-name` à `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="de833-1157">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="de833-1158">Ajout de la prise en charge du Pack Sécurité Entreprise et du chiffrement de disque à `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="de833-1158">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="de833-1159">Ajout de la commande `hdinsight rotate-disk-encryption-key`</span><span class="sxs-lookup"><span data-stu-id="de833-1159">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="de833-1160">Ajout de la commande `hdinsight update`</span><span class="sxs-lookup"><span data-stu-id="de833-1160">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="de833-1161">IoT</span><span class="sxs-lookup"><span data-stu-id="de833-1161">IoT</span></span>
* <span data-ttu-id="de833-1162">Ajout du format d’encodage à la commande routing-endpoint</span><span class="sxs-lookup"><span data-stu-id="de833-1162">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="de833-1163">Kusto</span><span class="sxs-lookup"><span data-stu-id="de833-1163">Kusto</span></span>
* <span data-ttu-id="de833-1164">Préversion</span><span class="sxs-lookup"><span data-stu-id="de833-1164">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="de833-1165">Moniteur</span><span class="sxs-lookup"><span data-stu-id="de833-1165">Monitor</span></span>
* <span data-ttu-id="de833-1166">Changement apporté à la comparaison d’ID pour qu’elle ne respecte pas la casse</span><span class="sxs-lookup"><span data-stu-id="de833-1166">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="de833-1167">Profil</span><span class="sxs-lookup"><span data-stu-id="de833-1167">Profile</span></span>
* <span data-ttu-id="de833-1168">Activation du compte de niveau locataire pour la fonctionnalité Managed Service Identity pour `login`</span><span class="sxs-lookup"><span data-stu-id="de833-1168">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="de833-1169">Réseau</span><span class="sxs-lookup"><span data-stu-id="de833-1169">Network</span></span>
* <span data-ttu-id="de833-1170">Correction d’un problème lié à `express-route update` où l’argument `--bandwidth` était ignoré</span><span class="sxs-lookup"><span data-stu-id="de833-1170">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="de833-1171">Correction d’un problème lié à `ddos-protection update` où set comprehension entraînait la génération d’un rapport des appels de procédure</span><span class="sxs-lookup"><span data-stu-id="de833-1171">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="de833-1172">Ressource</span><span class="sxs-lookup"><span data-stu-id="de833-1172">Resource</span></span>
* <span data-ttu-id="de833-1173">Ajout de la prise en charge du fichier de paramètres d’URI à `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="de833-1173">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="de833-1174">Ajout de la prise en charge de l’identité managée à `policy assignment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="de833-1174">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="de833-1175">Machine virtuelle SQL</span><span class="sxs-lookup"><span data-stu-id="de833-1175">SQL Virtual Machine</span></span>
* <span data-ttu-id="de833-1176">Préversion</span><span class="sxs-lookup"><span data-stu-id="de833-1176">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="de833-1177">Stockage</span><span class="sxs-lookup"><span data-stu-id="de833-1177">Storage</span></span>
* <span data-ttu-id="de833-1178">Changement d’une correction pour mettre à jour uniquement les propriétés modifiées sur le même objet</span><span class="sxs-lookup"><span data-stu-id="de833-1178">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="de833-1179">Correction (n° 8021). Les données binaires sont encodées au format base 64 quand elles sont retournées</span><span class="sxs-lookup"><span data-stu-id="de833-1179">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="de833-1180">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="de833-1180">VM</span></span>
* <span data-ttu-id="de833-1181">Changement apporté à `vm encryption enable` pour valider le coffre de clés de chiffrement de disque et vérifier l’existence du coffre de clés de chiffrement à clé</span><span class="sxs-lookup"><span data-stu-id="de833-1181">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="de833-1182">Ajout de l’indicateur `--force` à `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="de833-1182">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="de833-1183">15 janvier 2019</span><span class="sxs-lookup"><span data-stu-id="de833-1183">January 15, 2019</span></span>

<span data-ttu-id="de833-1184">Version 2.0.55</span><span class="sxs-lookup"><span data-stu-id="de833-1184">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="de833-1185">ACR</span><span class="sxs-lookup"><span data-stu-id="de833-1185">ACR</span></span>
* <span data-ttu-id="de833-1186">Changement apporté pour forcer l’envoi (push) d’un chart Helm qui n’existe pas</span><span class="sxs-lookup"><span data-stu-id="de833-1186">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="de833-1187">changement apporté pour autoriser les opérations de runtime sans requêtes ARM</span><span class="sxs-lookup"><span data-stu-id="de833-1187">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="de833-1188">[DÉPRÉCIATION] Dépréciation du paramètre `--resource-group` dans les commandes :</span><span class="sxs-lookup"><span data-stu-id="de833-1188">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="de833-1189">ACS</span><span class="sxs-lookup"><span data-stu-id="de833-1189">ACS</span></span>
* <span data-ttu-id="de833-1190">Ajout de la prise en charge des nouvelles régions ACI</span><span class="sxs-lookup"><span data-stu-id="de833-1190">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="de833-1191">AppService</span><span class="sxs-lookup"><span data-stu-id="de833-1191">Appservice</span></span>
* <span data-ttu-id="de833-1192">Correction d’un problème lié au chargement des certificats des applications hébergées sur un ASE, où ASE RG et App RG sont différents</span><span class="sxs-lookup"><span data-stu-id="de833-1192">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="de833-1193">Changement apporté à `webapp up` pour utiliser la référence (SKU) P1V1 en tant que valeur par défaut pour Linux</span><span class="sxs-lookup"><span data-stu-id="de833-1193">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="de833-1194">Correction apporté à `[webapp|functionapp] deployment source config-zip` pour afficher le message d’erreur approprié en cas d’échec d’un déploiement</span><span class="sxs-lookup"><span data-stu-id="de833-1194">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="de833-1195">Ajout de la commande `webapp ssh`</span><span class="sxs-lookup"><span data-stu-id="de833-1195">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="de833-1196">Botservice</span><span class="sxs-lookup"><span data-stu-id="de833-1196">Botservice</span></span>
* <span data-ttu-id="de833-1197">Ajout de mises à jour de l’état de déploiement à `bot create`</span><span class="sxs-lookup"><span data-stu-id="de833-1197">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="de833-1198">Configurer</span><span class="sxs-lookup"><span data-stu-id="de833-1198">Configure</span></span>
* <span data-ttu-id="de833-1199">Ajout de `none` en tant que format de sortie configurable</span><span class="sxs-lookup"><span data-stu-id="de833-1199">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="de833-1200">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="de833-1200">CosmosDB</span></span>
* <span data-ttu-id="de833-1201">Ajout de la prise en charge de la création d’une base de données avec débit partagé</span><span class="sxs-lookup"><span data-stu-id="de833-1201">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="de833-1202">HDInsight</span><span class="sxs-lookup"><span data-stu-id="de833-1202">HDInsight</span></span>
* <span data-ttu-id="de833-1203">Ajout de commandes pour la gestion des applications</span><span class="sxs-lookup"><span data-stu-id="de833-1203">Added commands for managing applications</span></span>
* <span data-ttu-id="de833-1204">Ajout de commandes pour la gestion des actions de script</span><span class="sxs-lookup"><span data-stu-id="de833-1204">Added commands for managing script actions</span></span>
* <span data-ttu-id="de833-1205">Ajout de commandes pour la gestion d’OMS (Operations Management Suite)</span><span class="sxs-lookup"><span data-stu-id="de833-1205">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="de833-1206">Ajout de la prise en charge permettant de lister l’utilisation régionale à `hdinsight list-usage`</span><span class="sxs-lookup"><span data-stu-id="de833-1206">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="de833-1207">[CHANGEMENT CASSANT] Suppression du type de cluster par défaut dans `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="de833-1207">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="de833-1208">Réseau</span><span class="sxs-lookup"><span data-stu-id="de833-1208">Network</span></span>
* <span data-ttu-id="de833-1209">Ajout des arguments `--custom-headers` et `--status-code-ranges` à `traffic-manager profile [create|update]`</span><span class="sxs-lookup"><span data-stu-id="de833-1209">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="de833-1210">Ajout de nouveaux types de routage : Sous-réseau et valeurs multiples</span><span class="sxs-lookup"><span data-stu-id="de833-1210">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="de833-1211">Ajout des arguments `--custom-headers` et `--subnets` à `traffic-manager endpoint [create|update]`</span><span class="sxs-lookup"><span data-stu-id="de833-1211">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="de833-1212">Correction du problème où la fourniture de `--vnets ""` à `ddos-protection update` provoquait une erreur</span><span class="sxs-lookup"><span data-stu-id="de833-1212">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="de833-1213">Role</span><span class="sxs-lookup"><span data-stu-id="de833-1213">Role</span></span>
* <span data-ttu-id="de833-1214">[DÉPRÉCIATION] Dépréciation de l’argument `--password` pour `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="de833-1214">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="de833-1215">Utilisation de mots de passe sécurisés générés par l’interface CLI à la place</span><span class="sxs-lookup"><span data-stu-id="de833-1215">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="de833-1216">Sécurité</span><span class="sxs-lookup"><span data-stu-id="de833-1216">Security</span></span>
* <span data-ttu-id="de833-1217">Version initiale</span><span class="sxs-lookup"><span data-stu-id="de833-1217">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="de833-1218">Stockage</span><span class="sxs-lookup"><span data-stu-id="de833-1218">Storage</span></span>
* <span data-ttu-id="de833-1219">[CHANGEMENT CASSANT] Changement apporté à `storage [blob|file|container|share] list` pour que le nombre par défaut de résultats soit de 5 000.</span><span class="sxs-lookup"><span data-stu-id="de833-1219">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="de833-1220">Utilisation de `--num-results *` pour que le comportement d’origine permette de retourner tous les résultats</span><span class="sxs-lookup"><span data-stu-id="de833-1220">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="de833-1221">Ajout du paramètre `--marker` pour `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="de833-1221">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="de833-1222">Ajout du marqueur de journal de la page suivante à STDERR pour `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="de833-1222">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="de833-1223">Ajout de la commande `storage blob service-properties update` avec prise en charge des sites web statiques</span><span class="sxs-lookup"><span data-stu-id="de833-1223">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="de833-1224">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="de833-1224">VM</span></span>
* <span data-ttu-id="de833-1225">Changement apporté à `vm [disk|unmanaged-disk]` et `vmss disk` pour avoir des paramètres plus cohérents</span><span class="sxs-lookup"><span data-stu-id="de833-1225">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="de833-1226">Ajout de la prise en charge du référencement d’images entre locataires à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="de833-1226">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="de833-1227">Résolution d’un bogue lié à la configuration par défaut dans `vm diagnostics get-default-config --windows-os`</span><span class="sxs-lookup"><span data-stu-id="de833-1227">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="de833-1228">Ajout de l’argument `--provision-after-extensions` à `vmss extension set` pour définir les extensions à provisionner avant de définir l’extension</span><span class="sxs-lookup"><span data-stu-id="de833-1228">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="de833-1229">Ajout de l’argument `--replica-count` à `sig image-version update` pour définir le nombre de réplications par défaut</span><span class="sxs-lookup"><span data-stu-id="de833-1229">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="de833-1230">Résolution d’un bogue lié à `image create --source` où le disque d’OS source est confondu avec une machine virtuelle portant le même nom, même si l’ID de ressource complet est fourni</span><span class="sxs-lookup"><span data-stu-id="de833-1230">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="de833-1231">20 décembre 2018</span><span class="sxs-lookup"><span data-stu-id="de833-1231">December 20, 2018</span></span>

<span data-ttu-id="de833-1232">Version 2.0.54</span><span class="sxs-lookup"><span data-stu-id="de833-1232">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="de833-1233">AppService</span><span class="sxs-lookup"><span data-stu-id="de833-1233">Appservice</span></span>
* <span data-ttu-id="de833-1234">Correction d’un problème qui causait l’échec du redéploiement pour `webapp up`</span><span class="sxs-lookup"><span data-stu-id="de833-1234">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="de833-1235">Ajout de la prise en charge du référencement et de la restauration des instantanés d’applications web</span><span class="sxs-lookup"><span data-stu-id="de833-1235">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="de833-1236">Ajout de la prise en charge pour l’indicateur `--runtime` aux applications de fonction Windows</span><span class="sxs-lookup"><span data-stu-id="de833-1236">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="de833-1237">IotCentral</span><span class="sxs-lookup"><span data-stu-id="de833-1237">IoTCentral</span></span>
* <span data-ttu-id="de833-1238">Correction de l’appel d’API des commandes de mise à jour</span><span class="sxs-lookup"><span data-stu-id="de833-1238">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="de833-1239">Role</span><span class="sxs-lookup"><span data-stu-id="de833-1239">Role</span></span>
* <span data-ttu-id="de833-1240">[CHANGEMENT CASSANT] Remplacement de `ad [app|sp] list` par une liste des 100 premiers objets par défaut uniquement</span><span class="sxs-lookup"><span data-stu-id="de833-1240">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="de833-1241">SQL</span><span class="sxs-lookup"><span data-stu-id="de833-1241">SQL</span></span>
* <span data-ttu-id="de833-1242">Ajout de la prise en charge du classement personnalisé sur les instances managées</span><span class="sxs-lookup"><span data-stu-id="de833-1242">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="de833-1243">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="de833-1243">VM</span></span>
* <span data-ttu-id="de833-1244">Ajout du paramètre `---os-type` pour `disk create`</span><span class="sxs-lookup"><span data-stu-id="de833-1244">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="de833-1245">18 décembre 2018</span><span class="sxs-lookup"><span data-stu-id="de833-1245">December 18, 2018</span></span>

<span data-ttu-id="de833-1246">Version 2.0.53</span><span class="sxs-lookup"><span data-stu-id="de833-1246">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="de833-1247">ACR</span><span class="sxs-lookup"><span data-stu-id="de833-1247">ACR</span></span>
* <span data-ttu-id="de833-1248">Ajout de la prise en charge de l’importation d’image à partir des registres de conteneurs externes</span><span class="sxs-lookup"><span data-stu-id="de833-1248">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="de833-1249">Condensé de la disposition du tableau pour la liste des tâches</span><span class="sxs-lookup"><span data-stu-id="de833-1249">Condensed the table layout for task list</span></span>
* <span data-ttu-id="de833-1250">Ajout de la prise en charge des URL Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="de833-1250">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="de833-1251">ACS</span><span class="sxs-lookup"><span data-stu-id="de833-1251">ACS</span></span>
* <span data-ttu-id="de833-1252">Ajout de l’aperçu des nœuds virtuels</span><span class="sxs-lookup"><span data-stu-id="de833-1252">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="de833-1253">Suppression du mot « (PRÉVERSION) » des arguments AAD pour `aks create`</span><span class="sxs-lookup"><span data-stu-id="de833-1253">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="de833-1254">[DÉPRÉCIATION] Dépréciation des commandes `az acs`.</span><span class="sxs-lookup"><span data-stu-id="de833-1254">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="de833-1255">Le service ACS sera mis hors service le 31 janvier 2020.</span><span class="sxs-lookup"><span data-stu-id="de833-1255">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="de833-1256">Ajout de la prise en charge de la stratégie de réseau lors de la création de clusters AKS</span><span class="sxs-lookup"><span data-stu-id="de833-1256">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="de833-1257">Suppression du caractère obligatoire de l’argument `--nodepool-name` pour `aks scale` s’il n’existe qu’un seul pool de nœuds</span><span class="sxs-lookup"><span data-stu-id="de833-1257">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="de833-1258">AppService</span><span class="sxs-lookup"><span data-stu-id="de833-1258">Appservice</span></span>
* <span data-ttu-id="de833-1259">Problème résolu quand `webapp config container` n’honore pas le paramètre `--slot`</span><span class="sxs-lookup"><span data-stu-id="de833-1259">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="de833-1260">Botservice</span><span class="sxs-lookup"><span data-stu-id="de833-1260">Botservice</span></span>
* <span data-ttu-id="de833-1261">Ajout de la prise en charge de l’analyse de fichier `.bot` lors de l’appel de `bot show`</span><span class="sxs-lookup"><span data-stu-id="de833-1261">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="de833-1262">Correction du bogue d’approvisionnement AppInsights</span><span class="sxs-lookup"><span data-stu-id="de833-1262">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="de833-1263">Correction du bogue d’espace blanc lors du traitement de chemins d’accès de fichier</span><span class="sxs-lookup"><span data-stu-id="de833-1263">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="de833-1264">Réduction des appels réseau Kudu</span><span class="sxs-lookup"><span data-stu-id="de833-1264">Reduced Kudu network calls</span></span>
* <span data-ttu-id="de833-1265">Amélioration de l’expérience utilisateur des commandes générales</span><span class="sxs-lookup"><span data-stu-id="de833-1265">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="de833-1266">Consommation</span><span class="sxs-lookup"><span data-stu-id="de833-1266">Consumption</span></span>
* <span data-ttu-id="de833-1267">Correction des bogues dans l’API de budget pour afficher les notifications</span><span class="sxs-lookup"><span data-stu-id="de833-1267">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="de833-1268">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="de833-1268">CosmosDB</span></span>
* <span data-ttu-id="de833-1269">Ajout de la prise en charge de la mise à jour de compte (multimaître vers maître unique)</span><span class="sxs-lookup"><span data-stu-id="de833-1269">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="de833-1270">Cartes</span><span class="sxs-lookup"><span data-stu-id="de833-1270">Maps</span></span>
* <span data-ttu-id="de833-1271">Ajout de la prise en charge de la référence (SKU) S1 pour `maps account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="de833-1271">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="de833-1272">Réseau</span><span class="sxs-lookup"><span data-stu-id="de833-1272">Network</span></span>
* <span data-ttu-id="de833-1273">Ajout de la prise en charge de `--format`, `--log-version` et `watcher flow-log configure`</span><span class="sxs-lookup"><span data-stu-id="de833-1273">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="de833-1274">Correction du problème avec `dns zone update`, où l’utilisation de "" pour effacer les réseaux virtuels de résolution d’inscription ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="de833-1274">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="de833-1275">Ressource</span><span class="sxs-lookup"><span data-stu-id="de833-1275">Resource</span></span>
* <span data-ttu-id="de833-1276">Correction de la gestion du paramètre d’étendue pour les groupes d’administration dans `policy assignment [create|list|delete|show|update]`</span><span class="sxs-lookup"><span data-stu-id="de833-1276">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="de833-1277">Ajout de la commande `resource wait`</span><span class="sxs-lookup"><span data-stu-id="de833-1277">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="de833-1278">Stockage</span><span class="sxs-lookup"><span data-stu-id="de833-1278">Storage</span></span>
*  <span data-ttu-id="de833-1279">Possibilité de mettre à jour la version de schéma de journal pour les services de stockage dans `storage logging update`</span><span class="sxs-lookup"><span data-stu-id="de833-1279">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="de833-1280">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="de833-1280">VM</span></span>
* <span data-ttu-id="de833-1281">Correction d’incident dans `vm identity remove`, lorsque la machine virtuelle spécifiée n’a aucune identité de service managé affectée</span><span class="sxs-lookup"><span data-stu-id="de833-1281">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="de833-1282">4 décembre 2018</span><span class="sxs-lookup"><span data-stu-id="de833-1282">December 4, 2018</span></span>

<span data-ttu-id="de833-1283">Version 2.0.52</span><span class="sxs-lookup"><span data-stu-id="de833-1283">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="de833-1284">Core</span><span class="sxs-lookup"><span data-stu-id="de833-1284">Core</span></span>
* <span data-ttu-id="de833-1285">L’approvisionnement des ressources entre locataires est désormais pris en charge pour le principal du service multi-locataire.</span><span class="sxs-lookup"><span data-stu-id="de833-1285">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="de833-1286">Les ID d’une commande avec sortie TSV n’étaient pas analysés correctement. Ce bogue a été corrigé.</span><span class="sxs-lookup"><span data-stu-id="de833-1286">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="de833-1287">AppService</span><span class="sxs-lookup"><span data-stu-id="de833-1287">Appservice</span></span>
* <span data-ttu-id="de833-1288">[APERÇU] Une commande `webapp up` a été ajoutée pour faciliter la création et le déploiement de contenu dans l’application.</span><span class="sxs-lookup"><span data-stu-id="de833-1288">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="de833-1289">Le bogue qui survenait sur les applications Windows basées sur des conteneurs en raison du changement de serveur principal a été corrigé.</span><span class="sxs-lookup"><span data-stu-id="de833-1289">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="de833-1290">Réseau</span><span class="sxs-lookup"><span data-stu-id="de833-1290">Network</span></span>
* <span data-ttu-id="de833-1291">L’argument `--exclusion` a été ajouté à `application-gateway waf-config set` pour prendre en charge les exclusions WAF</span><span class="sxs-lookup"><span data-stu-id="de833-1291">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="de833-1292">Role</span><span class="sxs-lookup"><span data-stu-id="de833-1292">Role</span></span>
* <span data-ttu-id="de833-1293">Les identificateurs personnalisés sont désormais pris en charge pour l’authentification par mot de passe.</span><span class="sxs-lookup"><span data-stu-id="de833-1293">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="de833-1294">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="de833-1294">VM</span></span>
* <span data-ttu-id="de833-1295">[DÉPRÉCIATION] Dépréciation du paramètre `vm extension [show|wait] --expand`</span><span class="sxs-lookup"><span data-stu-id="de833-1295">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="de833-1296">Le paramètre `--force` a été ajouté à `vm restart` pour redéployer les machines virtuelles qui ne répondent pas.</span><span class="sxs-lookup"><span data-stu-id="de833-1296">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="de833-1297">Le paramètre `[vm|vmss] create --authentication-type` a été modifié pour accepter la valeur « all » pour créer une machine virtuelle avec à la fois un mot de passe et une authentification SSH.</span><span class="sxs-lookup"><span data-stu-id="de833-1297">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="de833-1298">Le paramètre `image create --os-disk-caching` a été ajouté pour définir la mise en cache du disque du système d’exploitation pour une image.</span><span class="sxs-lookup"><span data-stu-id="de833-1298">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="de833-1299">20 novembre 2018</span><span class="sxs-lookup"><span data-stu-id="de833-1299">November 20, 2018</span></span>

<span data-ttu-id="de833-1300">Version 2.0.51</span><span class="sxs-lookup"><span data-stu-id="de833-1300">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="de833-1301">Core</span><span class="sxs-lookup"><span data-stu-id="de833-1301">Core</span></span>
* <span data-ttu-id="de833-1302">Modification du nom de connexion MSI pour ne pas réutiliser le nom d’abonnement dans une identité</span><span class="sxs-lookup"><span data-stu-id="de833-1302">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="de833-1303">ACR</span><span class="sxs-lookup"><span data-stu-id="de833-1303">ACR</span></span>
* <span data-ttu-id="de833-1304">Ajout d’un jeton de contexte à l’étape de tâche</span><span class="sxs-lookup"><span data-stu-id="de833-1304">Added context token to task step</span></span>
* <span data-ttu-id="de833-1305">Ajout de prise en charge pour la configuration des secrets dans acr run pour refléter acr task</span><span class="sxs-lookup"><span data-stu-id="de833-1305">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="de833-1306">Amélioration de la prise en charge de `--top` et `--orderby` pour les commandes `show-tags` et `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="de833-1306">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="de833-1307">AppService</span><span class="sxs-lookup"><span data-stu-id="de833-1307">Appservice</span></span>
* <span data-ttu-id="de833-1308">Augmentation du délai d’expiration par défaut du déploiement zip pour interroger l’état à 5 min, ce qui ajoute également une propriété de délai d’expiration pour personnaliser cette valeur</span><span class="sxs-lookup"><span data-stu-id="de833-1308">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="de833-1309">Mise à jour de la valeur par défaut `node_version`.</span><span class="sxs-lookup"><span data-stu-id="de833-1309">Updated the default `node_version`.</span></span> <span data-ttu-id="de833-1310">La réinitialisation d’une action d’échange d’emplacements pendant un échange en deux phases conserve toutes les chaînes de connexion et paramètres d’application</span><span class="sxs-lookup"><span data-stu-id="de833-1310">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="de833-1311">Suppression de la vérification de référence SKU côté client pour app service plan create de Linux</span><span class="sxs-lookup"><span data-stu-id="de833-1311">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="de833-1312">Correction de l’erreur qui survenait lors de tentatives d’obtention de l’état zipdeploy</span><span class="sxs-lookup"><span data-stu-id="de833-1312">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="de833-1313">IotCentral</span><span class="sxs-lookup"><span data-stu-id="de833-1313">IotCentral</span></span>
* <span data-ttu-id="de833-1314">Ajouter de la vérification de disponibilité du sous-domaine lors de la création d’une application IoT Central</span><span class="sxs-lookup"><span data-stu-id="de833-1314">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="de833-1315">KeyVault</span><span class="sxs-lookup"><span data-stu-id="de833-1315">KeyVault</span></span>
* <span data-ttu-id="de833-1316">Correction du bogue dans lequel des erreurs pouvaient avoir été ignorées</span><span class="sxs-lookup"><span data-stu-id="de833-1316">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="de833-1317">Réseau</span><span class="sxs-lookup"><span data-stu-id="de833-1317">Network</span></span>
* <span data-ttu-id="de833-1318">Ajout de sous-commandes `root-cert` à `application-gateway` pour traiter les certificats racine de confiance</span><span class="sxs-lookup"><span data-stu-id="de833-1318">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="de833-1319">Ajout des options `--min-capacity` et `--custom-error-pages` à `application-gateway [create|update]` :</span><span class="sxs-lookup"><span data-stu-id="de833-1319">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="de833-1320">Ajout de `--zones` pour la prise en charge de zone de disponibilité à `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="de833-1320">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="de833-1321">Ajout des arguments `--file-upload-limit`, `--max-request-body-size` et `--request-body-check` à `application-gateway waf-config set`</span><span class="sxs-lookup"><span data-stu-id="de833-1321">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="de833-1322">Rdbms</span><span class="sxs-lookup"><span data-stu-id="de833-1322">Rdbms</span></span>
* <span data-ttu-id="de833-1323">Ajouts de commandes mariadb vnet</span><span class="sxs-lookup"><span data-stu-id="de833-1323">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="de833-1324">Contrôle d’accès en fonction du rôle (RBAC)</span><span class="sxs-lookup"><span data-stu-id="de833-1324">Rbac</span></span>
* <span data-ttu-id="de833-1325">Résolution d’un problème qui survenait lors de tentatives de mise à jour d’informations d’identification immuables dans `ad app update`</span><span class="sxs-lookup"><span data-stu-id="de833-1325">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="de833-1326">Ajout d’avertissements de sortie pour indiquer des changements cassants dans un futur proche pour `ad [app|sp] list`</span><span class="sxs-lookup"><span data-stu-id="de833-1326">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="de833-1327">Stockage</span><span class="sxs-lookup"><span data-stu-id="de833-1327">Storage</span></span>
* <span data-ttu-id="de833-1328">Amélioration du traitement des « corner cases » pour les commandes de copie de stockage</span><span class="sxs-lookup"><span data-stu-id="de833-1328">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="de833-1329">Résolution d’un problème où `storage blob copy start-batch` n’utilisait pas les informations d’identification de connexion lorsque les comptes source et de destination étaient identiques</span><span class="sxs-lookup"><span data-stu-id="de833-1329">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="de833-1330">Correction du bogue avec `storage [blob|file] url` où `sas_token` n’était pas intégré dans l’URL</span><span class="sxs-lookup"><span data-stu-id="de833-1330">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="de833-1331">Ajout d’un avertissement de changement cassant à `[blob|container] list` : bientôt, seuls les 5 000 premiers résultats seront affichés par défaut dans la sortie</span><span class="sxs-lookup"><span data-stu-id="de833-1331">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="de833-1332">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="de833-1332">VM</span></span>
* <span data-ttu-id="de833-1333">Ajout de la prise en charge de `[vm|vmss] create --storage-sku` pour spécifier la référence SKU de compte de stockage pour les disques de données et de système d’exploitation managés de façon distincte</span><span class="sxs-lookup"><span data-stu-id="de833-1333">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="de833-1334">Remplacement des paramètres de nom de version `sig image-version` par `--image-version -e`</span><span class="sxs-lookup"><span data-stu-id="de833-1334">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="de833-1335">Version déconseillée de la valeur `--image-version-name` d’argument `sig image-version` remplacée par `--image-version`</span><span class="sxs-lookup"><span data-stu-id="de833-1335">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="de833-1336">Ajout de la prise en charge pour utiliser le disque de système d’exploitation local pour `[vm|vmss] create --ephemeral-os-disk`</span><span class="sxs-lookup"><span data-stu-id="de833-1336">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="de833-1337">Ajout de la prise en charge de `--no-wait` pour `snapshot create/update`</span><span class="sxs-lookup"><span data-stu-id="de833-1337">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="de833-1338">Ajout de la commande `snapshot wait`</span><span class="sxs-lookup"><span data-stu-id="de833-1338">Added `snapshot wait` command</span></span>
* <span data-ttu-id="de833-1339">Ajout de la prise en charge pour utiliser le nom d’instance avec `[vm|vmss] extension set --extension-instance-name`</span><span class="sxs-lookup"><span data-stu-id="de833-1339">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="de833-1340">6 novembre 2018</span><span class="sxs-lookup"><span data-stu-id="de833-1340">November 6, 2018</span></span>

<span data-ttu-id="de833-1341">Version 2.0.50</span><span class="sxs-lookup"><span data-stu-id="de833-1341">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="de833-1342">Core</span><span class="sxs-lookup"><span data-stu-id="de833-1342">Core</span></span>
* <span data-ttu-id="de833-1343">Ajout de la prise en charge pour le principal de service sn+issuer auth</span><span class="sxs-lookup"><span data-stu-id="de833-1343">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="de833-1344">ACR</span><span class="sxs-lookup"><span data-stu-id="de833-1344">ACR</span></span>
* <span data-ttu-id="de833-1345">Ajout de la prise en charge pour les événements git de demande d’envoi et de tirage pour le déclencheur de tâche source</span><span class="sxs-lookup"><span data-stu-id="de833-1345">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="de833-1346">Modification de l’utilisation de fichiers Dockerfile par défaut s’il n’est pas spécifié dans la commande build</span><span class="sxs-lookup"><span data-stu-id="de833-1346">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="de833-1347">ACS</span><span class="sxs-lookup"><span data-stu-id="de833-1347">ACS</span></span>
* <span data-ttu-id="de833-1348">[Changement cassant] : `enable_cloud_console_aks_browse` supprimé pour activer « az aks browse » par défaut</span><span class="sxs-lookup"><span data-stu-id="de833-1348">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="de833-1349">Advisor</span><span class="sxs-lookup"><span data-stu-id="de833-1349">Advisor</span></span>
* <span data-ttu-id="de833-1350">Version mise à la disposition générale</span><span class="sxs-lookup"><span data-stu-id="de833-1350">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="de833-1351">AMS</span><span class="sxs-lookup"><span data-stu-id="de833-1351">AMS</span></span>
* <span data-ttu-id="de833-1352">Ajout de nouveaux groupes de commandes :</span><span class="sxs-lookup"><span data-stu-id="de833-1352">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="de833-1353">Ajout de nouvelles commandes :</span><span class="sxs-lookup"><span data-stu-id="de833-1353">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="de833-1354">Ajout de la prise en charge des paramètres de chiffrement de `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="de833-1354">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="de833-1355">Ajout de la prise en charge de `ams transform output remove` qui peut désormais être effectuée en transmettant le chemin de l’index pour le supprimer</span><span class="sxs-lookup"><span data-stu-id="de833-1355">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="de833-1356">Ajout des arguments `--correlation-data` et `--label` au groupe de commandes `ams job`</span><span class="sxs-lookup"><span data-stu-id="de833-1356">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="de833-1357">Ajout des arguments `--storage-account` et `--container` au groupe de commandes `ams asset`</span><span class="sxs-lookup"><span data-stu-id="de833-1357">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="de833-1358">Ajout des valeurs par défaut pour le délai d’expiration (présent + 23h) et les autorisations (lecture) dans la commande `ams asset get-sas-url`</span><span class="sxs-lookup"><span data-stu-id="de833-1358">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="de833-1359">[Changement cassant] : commande `ams streaming locator` remplacée par `ams streaming-locator`</span><span class="sxs-lookup"><span data-stu-id="de833-1359">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="de833-1360">[Changement cassant] : mise à jour de l’argument `--content-keys` de `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="de833-1360">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="de833-1361">[Changement cassant] : `--content-policy-name` renommé en `--content-key-policy-name` dans la commande `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="de833-1361">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="de833-1362">[Changement cassant] : commande `ams streaming policy` remplacée par `ams streaming-policy`</span><span class="sxs-lookup"><span data-stu-id="de833-1362">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="de833-1363">[Changement cassant] : argument `--preset-names` remplacé par `--preset` dans le groupe de commandes `ams transform`.</span><span class="sxs-lookup"><span data-stu-id="de833-1363">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="de833-1364">À présent vous ne pouvez définir qu’une sortie/présélection à la fois (pour en ajouter d’autres, vous devez exécuter `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="de833-1364">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="de833-1365">En outre, vous pouvez définir StandardEncoderPreset de façon personnalisée en transmettant le chemin à votre JSON personnalisé</span><span class="sxs-lookup"><span data-stu-id="de833-1365">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="de833-1366">[Changement cassant] : `--output-asset-names ` renommé en `--output-assets` dans la commande `ams job start`.</span><span class="sxs-lookup"><span data-stu-id="de833-1366">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="de833-1367">Il accepte désormais une liste de ressources séparée par des espaces au format « assetName=label ».</span><span class="sxs-lookup"><span data-stu-id="de833-1367">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="de833-1368">Une ressource sans étiquette peut être envoyée comme ceci : « assetName= »</span><span class="sxs-lookup"><span data-stu-id="de833-1368">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="de833-1369">AppService</span><span class="sxs-lookup"><span data-stu-id="de833-1369">AppService</span></span>
* <span data-ttu-id="de833-1370">Correction d’un bogue dans `az webapp config backup update` qui empêche de définir une planification de sauvegarde si elle n’est pas déjà définie</span><span class="sxs-lookup"><span data-stu-id="de833-1370">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="de833-1371">Configurer</span><span class="sxs-lookup"><span data-stu-id="de833-1371">Configure</span></span>
* <span data-ttu-id="de833-1372">Ajout de YAML aux options de format de sortie</span><span class="sxs-lookup"><span data-stu-id="de833-1372">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="de833-1373">Conteneur</span><span class="sxs-lookup"><span data-stu-id="de833-1373">Container</span></span>
* <span data-ttu-id="de833-1374">Modification pour afficher l’identité lors de l’exportation d’un groupe de conteneurs vers yaml</span><span class="sxs-lookup"><span data-stu-id="de833-1374">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="de833-1375">Event Hub</span><span class="sxs-lookup"><span data-stu-id="de833-1375">EventHub</span></span>
* <span data-ttu-id="de833-1376">Ajout d’un indicateur `--enable-kafka` pour prendre en charge Kafka dans `eventhub namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="de833-1376">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="de833-1377">Interactive</span><span class="sxs-lookup"><span data-stu-id="de833-1377">Interactive</span></span>
* <span data-ttu-id="de833-1378">Interactive installe maintenant l’extension `interactive`, ce qui permettra des mises à jour et prises en charge plus rapides</span><span class="sxs-lookup"><span data-stu-id="de833-1378">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="de833-1379">Moniteur</span><span class="sxs-lookup"><span data-stu-id="de833-1379">Monitor</span></span>
* <span data-ttu-id="de833-1380">Ajout de la prise en charge pour les noms de métriques qui incluent les caractères barre oblique (/) et point (.) à `--condition` dans `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="de833-1380">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="de833-1381">Réseau</span><span class="sxs-lookup"><span data-stu-id="de833-1381">Network</span></span>
* <span data-ttu-id="de833-1382">Noms de commande `network interface-endpoint` déconseillés en faveur de `network private-endpoint`</span><span class="sxs-lookup"><span data-stu-id="de833-1382">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="de833-1383">Problème résolu à l’endroit où l’argument `--peer-circuit` n’accepte pas d’ID dans `express-route peering connection create`</span><span class="sxs-lookup"><span data-stu-id="de833-1383">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="de833-1384">Problème résolu à l’endroit où `--ip-tags` ne fonctionnait pas correctement avec `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="de833-1384">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="de833-1385">Profil</span><span class="sxs-lookup"><span data-stu-id="de833-1385">Profile</span></span>
* <span data-ttu-id="de833-1386">Ajout de `--use-cert-sn-issuer` à `az login` pour la connexion principale du service à l’aide du certificat de déploiement automatique</span><span class="sxs-lookup"><span data-stu-id="de833-1386">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="de833-1387">SGBDR</span><span class="sxs-lookup"><span data-stu-id="de833-1387">RDBMS</span></span>
* <span data-ttu-id="de833-1388">Ajout de commandes de réplica mysql</span><span class="sxs-lookup"><span data-stu-id="de833-1388">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="de833-1389">Ressource</span><span class="sxs-lookup"><span data-stu-id="de833-1389">Resource</span></span>
* <span data-ttu-id="de833-1390">Ajout de la prise en charge pour les groupes d’administration et les abonnements aux commandes `policy definition|set-definition`</span><span class="sxs-lookup"><span data-stu-id="de833-1390">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="de833-1391">Role</span><span class="sxs-lookup"><span data-stu-id="de833-1391">Role</span></span>
* <span data-ttu-id="de833-1392">Ajout de la prise en charge pour la gestion d’autorisation API, les utilisateurs connectés ainsi que la gestion des mots de passe et informations d’identification des certificats de l’application</span><span class="sxs-lookup"><span data-stu-id="de833-1392">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="de833-1393">Modification de `ad sp create-for-rbac` pour clarifier la confusion entre displayName et le nom de principal du service</span><span class="sxs-lookup"><span data-stu-id="de833-1393">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="de833-1394">Ajout de la prise en charge pour attribuer les autorisations aux applications AAD</span><span class="sxs-lookup"><span data-stu-id="de833-1394">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="de833-1395">Stockage</span><span class="sxs-lookup"><span data-stu-id="de833-1395">Storage</span></span>
* <span data-ttu-id="de833-1396">Ajout de la prise en charge pour vous connecter aux services de stockage uniquement avec les signatures d’accès partagé et les points de terminaison (sans nom de compte ou clé), comme décrit dans `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span><span class="sxs-lookup"><span data-stu-id="de833-1396">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="de833-1397">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="de833-1397">VM</span></span>
* <span data-ttu-id="de833-1398">Ajout de l’argument `storage-sku` à `image create` pour définir le type de compte de stockage par défaut de l’image</span><span class="sxs-lookup"><span data-stu-id="de833-1398">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="de833-1399">Correction du bogue avec `vm resize` à l’endroit où l’option `--no-wait` a entraîné un incident avec la commande</span><span class="sxs-lookup"><span data-stu-id="de833-1399">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="de833-1400">Modification du format de sortie de la table `vm encryption show` pour afficher l’état</span><span class="sxs-lookup"><span data-stu-id="de833-1400">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="de833-1401">Modification de `vm secret format` pour exiger la sortie json/jsonc</span><span class="sxs-lookup"><span data-stu-id="de833-1401">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="de833-1402">Avertit l’utilisateur et les valeurs par défaut à la sortie json si un format de sortie indésirable est sélectionné</span><span class="sxs-lookup"><span data-stu-id="de833-1402">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="de833-1403">Amélioration de la validation de l’argument pour `vm create --image`</span><span class="sxs-lookup"><span data-stu-id="de833-1403">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="de833-1404">23 octobre 2018</span><span class="sxs-lookup"><span data-stu-id="de833-1404">October 23, 2018</span></span>

<span data-ttu-id="de833-1405">Version 2.0.49</span><span class="sxs-lookup"><span data-stu-id="de833-1405">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="de833-1406">Core</span><span class="sxs-lookup"><span data-stu-id="de833-1406">Core</span></span>
* <span data-ttu-id="de833-1407">Correction du problème avec `--ids` où `--subscription` serait prioritaire sur l’abonnement dans `--ids`</span><span class="sxs-lookup"><span data-stu-id="de833-1407">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="de833-1408">Ajout d’avertissements explicites lorsque les paramètres sont ignorés par `--ids`</span><span class="sxs-lookup"><span data-stu-id="de833-1408">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="de833-1409">ACR</span><span class="sxs-lookup"><span data-stu-id="de833-1409">ACR</span></span>
* <span data-ttu-id="de833-1410">Correction d’un problème de codage ACR Build dans Python2</span><span class="sxs-lookup"><span data-stu-id="de833-1410">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="de833-1411">CDN</span><span class="sxs-lookup"><span data-stu-id="de833-1411">CDN</span></span>
* <span data-ttu-id="de833-1412">[CHANGEMENT CASSANT] Modification du comportement de mise en cache de chaîne de requête par défaut de `cdn endpoint create` afin que ce ne soit plus « IgnoreQueryString » par défaut.</span><span class="sxs-lookup"><span data-stu-id="de833-1412">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="de833-1413">Il est maintenant défini par le service</span><span class="sxs-lookup"><span data-stu-id="de833-1413">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="de833-1414">Conteneur</span><span class="sxs-lookup"><span data-stu-id="de833-1414">Container</span></span>
* <span data-ttu-id="de833-1415">Ajout de `Private` comme un type valide pour passer à «--ip-address»</span><span class="sxs-lookup"><span data-stu-id="de833-1415">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="de833-1416">Modification pour permettre l’utilisation d’un seul ID de sous-réseau pour configurer un réseau virtuel pour le groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="de833-1416">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="de833-1417">Modification pour permettre l’utilisation d’un nom de réseau virtuel ou d’un ID de ressource pour permettre l’utilisation de réseaux virtuels à partir de groupes de ressources différents</span><span class="sxs-lookup"><span data-stu-id="de833-1417">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="de833-1418">Ajout de `--assign-identity` pour ajouter une identité MSI à un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="de833-1418">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="de833-1419">Ajout de `--scope` pour créer une attribution de rôle pour l’identité MSI attribuée par le système</span><span class="sxs-lookup"><span data-stu-id="de833-1419">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="de833-1420">Ajout d’un avertissement lors de la création d’un groupe de conteneurs avec une image sans processus à long terme</span><span class="sxs-lookup"><span data-stu-id="de833-1420">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="de833-1421">Correction de problèmes de sortie de table pour les commandes `list` et `show`</span><span class="sxs-lookup"><span data-stu-id="de833-1421">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="de833-1422">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="de833-1422">CosmosDB</span></span>
* <span data-ttu-id="de833-1423">Ajout de la prise en charge de `--enable-multiple-write-locations` pour `cosmosdb create`</span><span class="sxs-lookup"><span data-stu-id="de833-1423">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="de833-1424">Interactive</span><span class="sxs-lookup"><span data-stu-id="de833-1424">Interactive</span></span>
* <span data-ttu-id="de833-1425">Modifié pour assurer l’apparition du paramètre d’abonnement global dans les paramètres</span><span class="sxs-lookup"><span data-stu-id="de833-1425">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="de833-1426">IoT Central</span><span class="sxs-lookup"><span data-stu-id="de833-1426">IoT Central</span></span>
* <span data-ttu-id="de833-1427">Ajout d’options de modèle et de nom d’affichage pour la création de l’application IoT central</span><span class="sxs-lookup"><span data-stu-id="de833-1427">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="de833-1428">[CHANGEMENT CASSANT] Suppression de la prise en charge de la référence SKU F1, utilisez la référence SKU S1 à la place</span><span class="sxs-lookup"><span data-stu-id="de833-1428">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="de833-1429">Moniteur</span><span class="sxs-lookup"><span data-stu-id="de833-1429">Monitor</span></span>
* <span data-ttu-id="de833-1430">Change en `monitor activity-log list` :</span><span class="sxs-lookup"><span data-stu-id="de833-1430">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="de833-1431">Prise en charge ajoutée pour répertorier tous les événements au niveau de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="de833-1431">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="de833-1432">Ajout du paramètre `--offset` pour créer plus facilement des requêtes de temps</span><span class="sxs-lookup"><span data-stu-id="de833-1432">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="de833-1433">Amélioration de la validation pour `--start-time` et `--end-time` pour utiliser des plages de formats ISO8601 plus larges et des formats dateHeure plus conviviaux</span><span class="sxs-lookup"><span data-stu-id="de833-1433">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="de833-1434">Ajout de `--namespace` comme alias pour l’option déconseillée `--resource-provider`</span><span class="sxs-lookup"><span data-stu-id="de833-1434">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="de833-1435">`--filters` déconseillé, car aucune valeur autre que celles avec des options fortement typées ne sont prises en charge par le service</span><span class="sxs-lookup"><span data-stu-id="de833-1435">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="de833-1436">Change en `monitor metrics list` :</span><span class="sxs-lookup"><span data-stu-id="de833-1436">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="de833-1437">Ajout du paramètre `--offset` pour créer plus facilement des requêtes de temps</span><span class="sxs-lookup"><span data-stu-id="de833-1437">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="de833-1438">Amélioration de la validation pour `--start-time` et `--end-time` pour utiliser des plages de formats ISO8601 plus larges et des formats dateHeure plus conviviaux</span><span class="sxs-lookup"><span data-stu-id="de833-1438">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="de833-1439">Amélioration de la validation pour les arguments `--event-hub` et `--event-hub-rule` à `monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="de833-1439">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="de833-1440">Réseau</span><span class="sxs-lookup"><span data-stu-id="de833-1440">Network</span></span>
* <span data-ttu-id="de833-1441">Ajout des arguments `--app-gateway-address-pools` et `--gateway-name` à `nic create`, pour prendre en charge l’ajout de pools d’adresses principaux Application Gateway à une carte réseau</span><span class="sxs-lookup"><span data-stu-id="de833-1441">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="de833-1442">Ajout des arguments `--app-gateway-address-pools` et `--gateway-name` à `nic ip-config create/update`, pour prendre en charge l’ajout de pools d’adresses principaux Application Gateway à une carte réseau</span><span class="sxs-lookup"><span data-stu-id="de833-1442">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="de833-1443">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="de833-1443">ServiceBus</span></span>
* <span data-ttu-id="de833-1444">Ajout de `migration_state` en lecture seule à MigrationConfigProperties pour afficher l’état actuel de migration d’espace de noms Standard à Premium de Service Bus</span><span class="sxs-lookup"><span data-stu-id="de833-1444">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="de833-1445">SQL</span><span class="sxs-lookup"><span data-stu-id="de833-1445">SQL</span></span>
* <span data-ttu-id="de833-1446">`sql failover-group create` et `sql failover-group update` corrigés pour fonctionner avec la stratégie de basculement manuel</span><span class="sxs-lookup"><span data-stu-id="de833-1446">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="de833-1447">Stockage</span><span class="sxs-lookup"><span data-stu-id="de833-1447">Storage</span></span>
* <span data-ttu-id="de833-1448">Formatage de sortie de `az storage cors list` corrigé, tous les éléments affichent une clé de « Service » correcte</span><span class="sxs-lookup"><span data-stu-id="de833-1448">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="de833-1449">Ajout du paramètre `--bypass-immutability-policy` pour la suppression du conteneur de stratégie d’immuabilité bloquée</span><span class="sxs-lookup"><span data-stu-id="de833-1449">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="de833-1450">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="de833-1450">VM</span></span>
* <span data-ttu-id="de833-1451">Mode de mise en cache configuré sur `None` pour la série de machines Lv/Lv2 dans `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="de833-1451">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="de833-1452">Mise à jour de la liste des tailles prises en charge, prenant en charge l’accélérateur de mise en réseau pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="de833-1452">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="de833-1453">Ajout des arguments fortement typés pour les configurations d’E/S et Mbits/s Ultrassd pour `disk create`</span><span class="sxs-lookup"><span data-stu-id="de833-1453">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="de833-1454">16 octobre 2018</span><span class="sxs-lookup"><span data-stu-id="de833-1454">October 16, 2018</span></span>

<span data-ttu-id="de833-1455">Version 2.0.48</span><span class="sxs-lookup"><span data-stu-id="de833-1455">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="de833-1456">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="de833-1456">VM</span></span>
* <span data-ttu-id="de833-1457">Résolution du problème de kit de développement logiciel qui a provoqué l’échec d’installation de Homebrew</span><span class="sxs-lookup"><span data-stu-id="de833-1457">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="de833-1458">9 octobre 2018</span><span class="sxs-lookup"><span data-stu-id="de833-1458">October 9, 2018</span></span>

<span data-ttu-id="de833-1459">Version 2.0.47</span><span class="sxs-lookup"><span data-stu-id="de833-1459">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="de833-1460">Core</span><span class="sxs-lookup"><span data-stu-id="de833-1460">Core</span></span>
* <span data-ttu-id="de833-1461">Gestion améliorée des erreurs « Demande incorrecte »</span><span class="sxs-lookup"><span data-stu-id="de833-1461">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="de833-1462">ACR</span><span class="sxs-lookup"><span data-stu-id="de833-1462">ACR</span></span>
* <span data-ttu-id="de833-1463">Prise en charge de format de tableau similaire, comme le client helm</span><span class="sxs-lookup"><span data-stu-id="de833-1463">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="de833-1464">ACS</span><span class="sxs-lookup"><span data-stu-id="de833-1464">ACS</span></span>
* <span data-ttu-id="de833-1465">Ajout de `aks [create|scale] --nodepool-name` pour configurer le nom du pool de nœuds, tronqué à 12 caractères, par défaut : nodepool1</span><span class="sxs-lookup"><span data-stu-id="de833-1465">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="de833-1466">Correction d’une erreur pour revenir à « scp » lorsque Parimiko échoue</span><span class="sxs-lookup"><span data-stu-id="de833-1466">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="de833-1467">Modification de `aks create` pour ne plus nécessiter `--aad-tenant-id`</span><span class="sxs-lookup"><span data-stu-id="de833-1467">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="de833-1468">Fusion améliorée des informations d'identification Kubernetes lorsque des entrées dupliquées sont présentes</span><span class="sxs-lookup"><span data-stu-id="de833-1468">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="de833-1469">Conteneur</span><span class="sxs-lookup"><span data-stu-id="de833-1469">Container</span></span>
* <span data-ttu-id="de833-1470">Modification de `functionapp create` pour prendre en charge la création d’un type de plan de consommation Linux avec un runtime spécifique</span><span class="sxs-lookup"><span data-stu-id="de833-1470">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="de833-1471">[PRÉVERSION] Prise en charge de l’hébergement d’applications web sur les conteneurs Windows</span><span class="sxs-lookup"><span data-stu-id="de833-1471">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="de833-1472">Event Hub</span><span class="sxs-lookup"><span data-stu-id="de833-1472">Event Hub</span></span>
* <span data-ttu-id="de833-1473">Correction de la commande `eventhub update`</span><span class="sxs-lookup"><span data-stu-id="de833-1473">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="de833-1474">[CHANGEMENT CASSANT] Modification des commandes `list` pour gérer des erreurs resource(s) NotFound(404) d’une manière habituelle au lieu d’afficher une liste vide</span><span class="sxs-lookup"><span data-stu-id="de833-1474">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="de833-1475">Extensions</span><span class="sxs-lookup"><span data-stu-id="de833-1475">Extensions</span></span>
* <span data-ttu-id="de833-1476">Correction d’une erreur de tentative d’ajout d’une extension déjà installée</span><span class="sxs-lookup"><span data-stu-id="de833-1476">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="de833-1477">HDInsight</span><span class="sxs-lookup"><span data-stu-id="de833-1477">HDInsight</span></span>
* <span data-ttu-id="de833-1478">Version initiale</span><span class="sxs-lookup"><span data-stu-id="de833-1478">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="de833-1479">IoT</span><span class="sxs-lookup"><span data-stu-id="de833-1479">IoT</span></span>
* <span data-ttu-id="de833-1480">Ajout de la commande d’installation de l’extension à une bannière pour la première exécution</span><span class="sxs-lookup"><span data-stu-id="de833-1480">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="de833-1481">KeyVault</span><span class="sxs-lookup"><span data-stu-id="de833-1481">KeyVault</span></span>
* <span data-ttu-id="de833-1482">Modification pour restreindre les commandes de stockage keyvault au dernier profil API</span><span class="sxs-lookup"><span data-stu-id="de833-1482">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="de833-1483">Réseau</span><span class="sxs-lookup"><span data-stu-id="de833-1483">Network</span></span>
* <span data-ttu-id="de833-1484">Correction de `network dns zone create` : la commande réussit même si l’utilisateur a configuré un emplacement par défaut.</span><span class="sxs-lookup"><span data-stu-id="de833-1484">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="de833-1485">Voir #6052</span><span class="sxs-lookup"><span data-stu-id="de833-1485">See #6052</span></span>
* <span data-ttu-id="de833-1486">Remplacement de `--remote-vnet-id` pour `network vnet peering create`</span><span class="sxs-lookup"><span data-stu-id="de833-1486">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="de833-1487">Ajout de `--remote-vnet` à `network vnet peering create`, qui accepte un nom ou ID</span><span class="sxs-lookup"><span data-stu-id="de833-1487">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="de833-1488">Prise en charge de multiples préfixes de sous-réseau pour `network vnet create` avec `--subnet-prefixes`</span><span class="sxs-lookup"><span data-stu-id="de833-1488">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="de833-1489">Prise en charge de multiples préfixes de sous-réseau pour `network vnet subnet [create|update]` avec `--address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="de833-1489">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="de833-1490">Correction d’une erreur relative à `network application-gateway create` qui empêchait la création de passerelles avec les références SKU `WAF_v2` ou `Standard_v2`</span><span class="sxs-lookup"><span data-stu-id="de833-1490">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="de833-1491">Ajout de l’argument d’usage `--service-endpoint-policy` à `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="de833-1491">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="de833-1492">Role</span><span class="sxs-lookup"><span data-stu-id="de833-1492">Role</span></span>
* <span data-ttu-id="de833-1493">Prise en charge du listing des propriétaires d’applications Azure AD à `ad app owner`</span><span class="sxs-lookup"><span data-stu-id="de833-1493">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="de833-1494">Prise en charge du listing des propriétaires de principaux de service Azure AD à `ad sp owner`</span><span class="sxs-lookup"><span data-stu-id="de833-1494">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="de833-1495">Modification pour garantir que les commandes de mise à jour et de création de définition de rôle acceptent les configurations à autorisations multiples</span><span class="sxs-lookup"><span data-stu-id="de833-1495">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="de833-1496">Modification de `ad sp create-for-rbac` pour garantir que l’URI de la page d’accueil est toujours « https »</span><span class="sxs-lookup"><span data-stu-id="de833-1496">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="de833-1497">Service Bus</span><span class="sxs-lookup"><span data-stu-id="de833-1497">Service Bus</span></span>
* <span data-ttu-id="de833-1498">[CHANGEMENT CASSANT] Modification des commandes `list` pour gérer des erreurs resource(s) NotFound(404) d’une manière habituelle au lieu d’afficher une liste vide</span><span class="sxs-lookup"><span data-stu-id="de833-1498">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="de833-1499">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="de833-1499">VM</span></span>
* <span data-ttu-id="de833-1500">Correction du champ vide `accessSas` dans `disk grant-access`</span><span class="sxs-lookup"><span data-stu-id="de833-1500">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="de833-1501">Modification de `vmss create` pour réserver une plage de port de frontend assez large pour gérer le surprovisionnement</span><span class="sxs-lookup"><span data-stu-id="de833-1501">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="de833-1502">Correction des commandes de mise à jour pour `sig`</span><span class="sxs-lookup"><span data-stu-id="de833-1502">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="de833-1503">Prise en charge `--no-wait` de la gestion de versions d’images dans `sig`</span><span class="sxs-lookup"><span data-stu-id="de833-1503">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="de833-1504">Modification de `vm list-ip-addresses` pour afficher la zone de disponibilité des adresses IP publiques</span><span class="sxs-lookup"><span data-stu-id="de833-1504">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="de833-1505">Modification de `[vm|vmss] disk attach` pour définir le numéro d’identité logique (LUN) par défaut du disque sur le premier emplacement disponible</span><span class="sxs-lookup"><span data-stu-id="de833-1505">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="de833-1506">21 septembre 2018</span><span class="sxs-lookup"><span data-stu-id="de833-1506">September 21, 2018</span></span>

<span data-ttu-id="de833-1507">Version 2.0.46</span><span class="sxs-lookup"><span data-stu-id="de833-1507">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="de833-1508">ACR</span><span class="sxs-lookup"><span data-stu-id="de833-1508">ACR</span></span>
* <span data-ttu-id="de833-1509">Ajout de commandes de tâche ACR</span><span class="sxs-lookup"><span data-stu-id="de833-1509">Added ACR Task commands</span></span>
* <span data-ttu-id="de833-1510">Ajout de la commande d’exécution rapide</span><span class="sxs-lookup"><span data-stu-id="de833-1510">Added quick run command</span></span>
* <span data-ttu-id="de833-1511">Groupe de commandes `build-task` déconseillé</span><span class="sxs-lookup"><span data-stu-id="de833-1511">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="de833-1512">Ajout du groupe de commandes `helm` pour prendre en charge la gestion des graphiques Helm avec ACR</span><span class="sxs-lookup"><span data-stu-id="de833-1512">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="de833-1513">Ajout de la prise en charge de la création idempotent pour les registres managés</span><span class="sxs-lookup"><span data-stu-id="de833-1513">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="de833-1514">Ajout d’un indicateur de non-format pour l’affichage des journaux d’activité de génération</span><span class="sxs-lookup"><span data-stu-id="de833-1514">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="de833-1515">ACS</span><span class="sxs-lookup"><span data-stu-id="de833-1515">ACS</span></span>
* <span data-ttu-id="de833-1516">Modification de la commande `install-connector` pour configurer le nom de domaine complet maître AKS</span><span class="sxs-lookup"><span data-stu-id="de833-1516">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="de833-1517">Correction de la création d’attribution de rôle pour vnet-subnet-id lorsque le principal de service n’est pas spécifié, et pour skip-role-assignemnt</span><span class="sxs-lookup"><span data-stu-id="de833-1517">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="de833-1518">AppService</span><span class="sxs-lookup"><span data-stu-id="de833-1518">AppService</span></span>

* <span data-ttu-id="de833-1519">Ajout de la prise en charge de la gestion des opérations (continues et déclenchées) des Webjobs</span><span class="sxs-lookup"><span data-stu-id="de833-1519">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="de833-1520">az webapp config set prend en charge la propriété FTS-state. Aussi ajout de la prise en charge de az functionapp config set & show</span><span class="sxs-lookup"><span data-stu-id="de833-1520">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="de833-1521">Ajout de la prise en charge de Bring Your Own Storage pour les applications web</span><span class="sxs-lookup"><span data-stu-id="de833-1521">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="de833-1522">Ajout de la prise en charge du référencement et de la restauration des applications web supprimées</span><span class="sxs-lookup"><span data-stu-id="de833-1522">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="de833-1523">Batch</span><span class="sxs-lookup"><span data-stu-id="de833-1523">Batch</span></span>
* <span data-ttu-id="de833-1524">Modification de l’ajout des tâches via `--json-file` pour prendre en charge la syntaxe AddTaskCollectionParameter</span><span class="sxs-lookup"><span data-stu-id="de833-1524">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="de833-1525">Mise à jour de la documentation des formats `--json-file` acceptés</span><span class="sxs-lookup"><span data-stu-id="de833-1525">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="de833-1526">Ajout de `--max-tasks-per-node-option` à `batch pool create`</span><span class="sxs-lookup"><span data-stu-id="de833-1526">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="de833-1527">Modification du comportement de `batch account` pour afficher la connexion au compte si aucune option n’est spécifiée</span><span class="sxs-lookup"><span data-stu-id="de833-1527">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="de833-1528">Batch AI</span><span class="sxs-lookup"><span data-stu-id="de833-1528">Batch AI</span></span> 
* <span data-ttu-id="de833-1529">Correction de l’échec de création de compte de stockage automatique dans la commande `batchai cluster create`</span><span class="sxs-lookup"><span data-stu-id="de833-1529">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="de833-1530">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="de833-1530">Cognitive Services</span></span>
* <span data-ttu-id="de833-1531">Ajout de Completer pour les arguments `--sku`, `--kind` et `--location`</span><span class="sxs-lookup"><span data-stu-id="de833-1531">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="de833-1532">Ajout de la commande `cognitiveservices account list-usage`</span><span class="sxs-lookup"><span data-stu-id="de833-1532">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="de833-1533">Ajout de la commande `cognitiveservices account list-kinds`</span><span class="sxs-lookup"><span data-stu-id="de833-1533">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="de833-1534">Ajout de la commande `cognitiveservices account list`</span><span class="sxs-lookup"><span data-stu-id="de833-1534">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="de833-1535">`cognitiveservices list` déconseillé</span><span class="sxs-lookup"><span data-stu-id="de833-1535">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="de833-1536">Modification de `--name` afin de le rendre facultatif pour `cognitiveservices account list-skus`</span><span class="sxs-lookup"><span data-stu-id="de833-1536">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="de833-1537">Conteneur</span><span class="sxs-lookup"><span data-stu-id="de833-1537">Container</span></span>
* <span data-ttu-id="de833-1538">Ajout de la possibilité de redémarrer et d’arrêter un groupe de conteneurs en cours d’exécution</span><span class="sxs-lookup"><span data-stu-id="de833-1538">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="de833-1539">Ajout de `--network-profile` pour autoriser le passage dans un profil réseau</span><span class="sxs-lookup"><span data-stu-id="de833-1539">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="de833-1540">Ajout de `--subnet` et `--vnet_name` pour autoriser la création de groupes de conteneurs dans un réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="de833-1540">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="de833-1541">Modification de la sortie de table pour afficher l’état du groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="de833-1541">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="de833-1542">DataLake</span><span class="sxs-lookup"><span data-stu-id="de833-1542">Datalake</span></span>
* <span data-ttu-id="de833-1543">Ajout de commandes pour les règles de réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="de833-1543">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="de833-1544">Shell interactif</span><span class="sxs-lookup"><span data-stu-id="de833-1544">Interactive Shell</span></span>
* <span data-ttu-id="de833-1545">Correction des erreurs sur Windows où les commandes ne s’exécutent pas correctement</span><span class="sxs-lookup"><span data-stu-id="de833-1545">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="de833-1546">Correction du problème de chargement de commande dans le Shell interactif provoqué par les objets déconseillés</span><span class="sxs-lookup"><span data-stu-id="de833-1546">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="de833-1547">IoT</span><span class="sxs-lookup"><span data-stu-id="de833-1547">IoT</span></span>
* <span data-ttu-id="de833-1548">Ajout de la prise en charge du routage des hubs IoT</span><span class="sxs-lookup"><span data-stu-id="de833-1548">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="de833-1549">Key Vault</span><span class="sxs-lookup"><span data-stu-id="de833-1549">Key Vault</span></span>
* <span data-ttu-id="de833-1550">Correction de l’importation de la clé Key Vault pour les clés RSA</span><span class="sxs-lookup"><span data-stu-id="de833-1550">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="de833-1551">Réseau</span><span class="sxs-lookup"><span data-stu-id="de833-1551">Network</span></span>
* <span data-ttu-id="de833-1552">Ajout des commandes `network public-ip prefix` pour prendre en charge les fonctionnalités de préfixes d’adresses IP publiques</span><span class="sxs-lookup"><span data-stu-id="de833-1552">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="de833-1553">Ajout des commandes `network service-endpoint` pour prendre en charge les fonctionnalités de stratégie de point de terminaison de service</span><span class="sxs-lookup"><span data-stu-id="de833-1553">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="de833-1554">Ajout des commandes `network lb outbound-rule` pour prendre en charge la création de règles de trafic sortant d’un équilibreur de charge standard</span><span class="sxs-lookup"><span data-stu-id="de833-1554">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="de833-1555">Ajout de `--public-ip-prefix` à `network lb frontend-ip create/update` pour prendre en charge les configurations IP frontales à l’aide de préfixes d’adresses IP publiques</span><span class="sxs-lookup"><span data-stu-id="de833-1555">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="de833-1556">Ajout de `--enable-tcp-reset` à `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span><span class="sxs-lookup"><span data-stu-id="de833-1556">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="de833-1557">Ajout de `--disable-outbound-snat` à `network lb rule create/update`</span><span class="sxs-lookup"><span data-stu-id="de833-1557">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="de833-1558">Autoriser `network watcher flow-log show/configure` à être utilisé avec des groupes de sécurité réseau classiques</span><span class="sxs-lookup"><span data-stu-id="de833-1558">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="de833-1559">Ajouter la commande `network watcher run-configuration-diagnostic`</span><span class="sxs-lookup"><span data-stu-id="de833-1559">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="de833-1560">Correction de la commande `network watcher test-connectivity` et ajout des propriétés `--method`, `--valid-status-codes` et `--headers`</span><span class="sxs-lookup"><span data-stu-id="de833-1560">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="de833-1561">`network express-route create/update`: ajout de l’indicateur `--allow-global-reach`</span><span class="sxs-lookup"><span data-stu-id="de833-1561">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="de833-1562">`network vnet subnet create/update`: ajout de la prise en charge de `--delegation`</span><span class="sxs-lookup"><span data-stu-id="de833-1562">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="de833-1563">Ajout de la commande `network vnet subnet list-available-delegations`</span><span class="sxs-lookup"><span data-stu-id="de833-1563">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="de833-1564">`network traffic-manager profile create/update`: ajout de la prise en charge de `--interval`, `--timeout` et `--max-failures` pour les options Deprecated de configuration du moniteur `--monitor-path`, `--monitor-port` et `--monitor-protocol` en faveur de `--path`, `--port`, `--protocol`</span><span class="sxs-lookup"><span data-stu-id="de833-1564">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="de833-1565">`network lb frontend-ip create/update`: correction de la logique de réglage de la méthode d’allocation d’adresses IP privées. Si une adresse IP privée est fournie, l’allocation sera statique. Si aucune adresse IP privée n’est fournie, ou qu’une chaîne vide est fournie pour l’adresse IP privée, l’allocation est dynamique.</span><span class="sxs-lookup"><span data-stu-id="de833-1565">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="de833-1566">`dns record-set * create/update`: ajout de la prise en charge de `--target-resource`</span><span class="sxs-lookup"><span data-stu-id="de833-1566">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="de833-1567">Ajout des commandes `network interface-endpoint` pour interroger les objets de point de terminaison de l’interface</span><span class="sxs-lookup"><span data-stu-id="de833-1567">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="de833-1568">Ajout de `network profile show/list/delete` pour la gestion partielle des profils de réseau</span><span class="sxs-lookup"><span data-stu-id="de833-1568">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="de833-1569">Ajout des commandes `network express-route peering connection` pour gérer les connexions de peering entre les routes ExpressRoutes</span><span class="sxs-lookup"><span data-stu-id="de833-1569">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="de833-1570">SGBDR</span><span class="sxs-lookup"><span data-stu-id="de833-1570">RDBMS</span></span>
* <span data-ttu-id="de833-1571">Ajout de la prise en charge du service MariaDB</span><span class="sxs-lookup"><span data-stu-id="de833-1571">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="de833-1572">Réservation</span><span class="sxs-lookup"><span data-stu-id="de833-1572">Reservation</span></span>
* <span data-ttu-id="de833-1573">Ajout de CosmosDb dans le type d’énumération des ressources réservées</span><span class="sxs-lookup"><span data-stu-id="de833-1573">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="de833-1574">Ajout de la propriété de nom dans un modèle Patch</span><span class="sxs-lookup"><span data-stu-id="de833-1574">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="de833-1575">Gérer l’application</span><span class="sxs-lookup"><span data-stu-id="de833-1575">Manage App</span></span>
* <span data-ttu-id="de833-1576">Correction du bogue dans `managedapp create --kind MarketPlace` à l’origine du blocage de la création d’instance d’une application Marketplace gérée</span><span class="sxs-lookup"><span data-stu-id="de833-1576">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="de833-1577">Modification des commandes `feature` afin qu’elles soient limitées aux profils pris en charge</span><span class="sxs-lookup"><span data-stu-id="de833-1577">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="de833-1578">Role</span><span class="sxs-lookup"><span data-stu-id="de833-1578">Role</span></span>
* <span data-ttu-id="de833-1579">Ajout de la prise en charge pour répertorier les appartenances de l’utilisateur à des groupes</span><span class="sxs-lookup"><span data-stu-id="de833-1579">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="de833-1580">SignalR</span><span class="sxs-lookup"><span data-stu-id="de833-1580">SignalR</span></span>
* <span data-ttu-id="de833-1581">Première version</span><span class="sxs-lookup"><span data-stu-id="de833-1581">First release</span></span>

### <a name="storage"></a><span data-ttu-id="de833-1582">Stockage</span><span class="sxs-lookup"><span data-stu-id="de833-1582">Storage</span></span>
* <span data-ttu-id="de833-1583">Ajout du paramètre `--auth-mode login` pour l’utilisation des informations d’identification de l’utilisateur pour autoriser les objets blob et les files d’attente</span><span class="sxs-lookup"><span data-stu-id="de833-1583">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="de833-1584">Ajout de `storage container immutability-policy/legal-hold` pour gérer le stockage immuable</span><span class="sxs-lookup"><span data-stu-id="de833-1584">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="de833-1585">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="de833-1585">VM</span></span>
* <span data-ttu-id="de833-1586">Correction d’un problème `vm create --generate-ssh-keys` qui remplace le fichier de clé privée si le fichier de clé publique est manquant (#4725, #6780)</span><span class="sxs-lookup"><span data-stu-id="de833-1586">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="de833-1587">Ajout de la prise en charge pour la galerie d’images partagée via `az sig`</span><span class="sxs-lookup"><span data-stu-id="de833-1587">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="de833-1588">28 Août 2018</span><span class="sxs-lookup"><span data-stu-id="de833-1588">August 28, 2018</span></span>

<span data-ttu-id="de833-1589">Version 2.0.45</span><span class="sxs-lookup"><span data-stu-id="de833-1589">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="de833-1590">Core</span><span class="sxs-lookup"><span data-stu-id="de833-1590">Core</span></span>

* <span data-ttu-id="de833-1591">Résolution du problème de chargement de fichier de configuration vide</span><span class="sxs-lookup"><span data-stu-id="de833-1591">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="de833-1592">Ajout de la prise en charge du profil `2018-03-01-hybrid` pour Azure Stack</span><span class="sxs-lookup"><span data-stu-id="de833-1592">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="de833-1593">ACR</span><span class="sxs-lookup"><span data-stu-id="de833-1593">ACR</span></span>

* <span data-ttu-id="de833-1594">Ajout d’une solution pour les opérations d’exécution sans les requêtes ARM</span><span class="sxs-lookup"><span data-stu-id="de833-1594">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="de833-1595">Exclusion des fichiers de contrôle de version (par exemple, .git, .gitignore) chargés par défaut dans les fichiers tar dans la commande `build`</span><span class="sxs-lookup"><span data-stu-id="de833-1595">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="de833-1596">ACS</span><span class="sxs-lookup"><span data-stu-id="de833-1596">ACS</span></span>

* <span data-ttu-id="de833-1597">Modification de `aks create` à la valeur par défaut sur les machines virtuelles `Standard_DS2_v2`</span><span class="sxs-lookup"><span data-stu-id="de833-1597">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="de833-1598">Modification de `aks get-credentials` afin d’appeler de nouvelles API pour l’obtention des informations d’identification des clusters</span><span class="sxs-lookup"><span data-stu-id="de833-1598">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="de833-1599">AppService</span><span class="sxs-lookup"><span data-stu-id="de833-1599">AppService</span></span>

* <span data-ttu-id="de833-1600">Prise en charge de CORS sur functionapp et webapp</span><span class="sxs-lookup"><span data-stu-id="de833-1600">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="de833-1601">Ajout de la prise en charge de la balise ARM sur les commandes de création</span><span class="sxs-lookup"><span data-stu-id="de833-1601">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="de833-1602">Modification de `[webapp|functionapp] identity show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="de833-1602">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="de833-1603">Backup</span><span class="sxs-lookup"><span data-stu-id="de833-1603">Backup</span></span>

* <span data-ttu-id="de833-1604">Modification de `backup vault backup-properties show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="de833-1604">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="de833-1605">Service de robot</span><span class="sxs-lookup"><span data-stu-id="de833-1605">Bot Service</span></span>

* <span data-ttu-id="de833-1606">Version initiale de l’interface CLI de Bot Service</span><span class="sxs-lookup"><span data-stu-id="de833-1606">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="de833-1607">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="de833-1607">Cognitive Services</span></span>

* <span data-ttu-id="de833-1608">Ajout du nouveau paramètre `--api-properties,` requis pour la création de certains services</span><span class="sxs-lookup"><span data-stu-id="de833-1608">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="de833-1609">IoT</span><span class="sxs-lookup"><span data-stu-id="de833-1609">IoT</span></span>

* <span data-ttu-id="de833-1610">Résolution du problème relatif à l’association de hubs liés</span><span class="sxs-lookup"><span data-stu-id="de833-1610">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="de833-1611">Moniteur</span><span class="sxs-lookup"><span data-stu-id="de833-1611">Monitor</span></span>

* <span data-ttu-id="de833-1612">Ajout des commandes `monitor metrics alert` permettant de recevoir des alertes sur les métriques quasiment en temps réel</span><span class="sxs-lookup"><span data-stu-id="de833-1612">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="de833-1613">Commandes `monitor alert` déconseillées</span><span class="sxs-lookup"><span data-stu-id="de833-1613">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="de833-1614">Réseau</span><span class="sxs-lookup"><span data-stu-id="de833-1614">Network</span></span>

* <span data-ttu-id="de833-1615">Modification de `network application-gateway ssl-policy predefined show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="de833-1615">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="de833-1616">Ressource</span><span class="sxs-lookup"><span data-stu-id="de833-1616">Resource</span></span>

* <span data-ttu-id="de833-1617">Modification de `provider operation show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="de833-1617">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="de833-1618">Stockage</span><span class="sxs-lookup"><span data-stu-id="de833-1618">Storage</span></span>

* <span data-ttu-id="de833-1619">Modification de `storage share policy show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="de833-1619">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="de833-1620">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="de833-1620">VM</span></span>

* <span data-ttu-id="de833-1621">Modification de `vm/vmss identity show` permettant de quitter avec le code 3 en cas de ressource manquante</span><span class="sxs-lookup"><span data-stu-id="de833-1621">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="de833-1622">Remplacement de `--storage-caching` pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="de833-1622">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="de833-1623">14 août 2018</span><span class="sxs-lookup"><span data-stu-id="de833-1623">Auguest 14, 2018</span></span>

<span data-ttu-id="de833-1624">Version 2.0.44</span><span class="sxs-lookup"><span data-stu-id="de833-1624">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="de833-1625">Core</span><span class="sxs-lookup"><span data-stu-id="de833-1625">Core</span></span>

* <span data-ttu-id="de833-1626">Correction de l’affichage numérique dans la sortie `table`</span><span class="sxs-lookup"><span data-stu-id="de833-1626">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="de833-1627">Ajout du format de sortie YAML</span><span class="sxs-lookup"><span data-stu-id="de833-1627">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="de833-1628">Télémétrie</span><span class="sxs-lookup"><span data-stu-id="de833-1628">Telemetry</span></span>

* <span data-ttu-id="de833-1629">Amélioration des rapports de télémétrie</span><span class="sxs-lookup"><span data-stu-id="de833-1629">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="de833-1630">ACR</span><span class="sxs-lookup"><span data-stu-id="de833-1630">ACR</span></span>

* <span data-ttu-id="de833-1631">Ajout des commandes `content-trust policy`</span><span class="sxs-lookup"><span data-stu-id="de833-1631">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="de833-1632">Résolution du problème où `.dockerignore` n’était pas honorée</span><span class="sxs-lookup"><span data-stu-id="de833-1632">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="de833-1633">ACS</span><span class="sxs-lookup"><span data-stu-id="de833-1633">ACS</span></span>

* <span data-ttu-id="de833-1634">Modification de `az acs/aks install-cli` afin d’effectuer l’installation sous `%USERPROFILE%\.azure-kubectl` sur Windows</span><span class="sxs-lookup"><span data-stu-id="de833-1634">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="de833-1635">Modification de `az aks install-connector` afin de détecter si le cluster dispose du contrôle RBAC et de configurer le connecteur ACI correctement</span><span class="sxs-lookup"><span data-stu-id="de833-1635">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="de833-1636">Remplacement par l’attribution de rôle au sous-réseau lorsque l’attribution est fournie</span><span class="sxs-lookup"><span data-stu-id="de833-1636">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="de833-1637">Ajout de l’option nouveau « ignorer attribution de rôle » pour le sous-réseau lorsque l’attribution est fournie</span><span class="sxs-lookup"><span data-stu-id="de833-1637">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="de833-1638">Modification ignorant l’attribution de rôle au sous-réseau lorsque l’attribution existe déjà</span><span class="sxs-lookup"><span data-stu-id="de833-1638">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="de833-1639">AppService</span><span class="sxs-lookup"><span data-stu-id="de833-1639">AppService</span></span>

* <span data-ttu-id="de833-1640">Correction d’un bogue empêchant de créer une application de fonction à l’aide de comptes de stockage dans les groupes de ressources externes</span><span class="sxs-lookup"><span data-stu-id="de833-1640">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="de833-1641">Correction d’un incident lors du déploiement de dossier zip</span><span class="sxs-lookup"><span data-stu-id="de833-1641">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="de833-1642">Batch AI</span><span class="sxs-lookup"><span data-stu-id="de833-1642">BatchAI</span></span>

* <span data-ttu-id="de833-1643">Modification de la sortie de l’enregistreur d’événements pour la création du compte de stockage automatique afin de spécifier l’information « ressource *groupe*».</span><span class="sxs-lookup"><span data-stu-id="de833-1643">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="de833-1644">Conteneur</span><span class="sxs-lookup"><span data-stu-id="de833-1644">Container</span></span>

* <span data-ttu-id="de833-1645">Ajout de `--secure-environment-variables` pour transmettre des variables d’environnement sécurisées vers un conteneur</span><span class="sxs-lookup"><span data-stu-id="de833-1645">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="de833-1646">IoT</span><span class="sxs-lookup"><span data-stu-id="de833-1646">IoT</span></span>

* <span data-ttu-id="de833-1647">[CHANGEMENT CASSANT] Suppression des commandes obsolètes déplacées vers l’extension iot</span><span class="sxs-lookup"><span data-stu-id="de833-1647">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="de833-1648">Mise à jour des éléments afin de ne pas prendre en compte le domaine `azure-devices.net`</span><span class="sxs-lookup"><span data-stu-id="de833-1648">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="de833-1649">Iot Central</span><span class="sxs-lookup"><span data-stu-id="de833-1649">Iot Central</span></span>

* <span data-ttu-id="de833-1650">Version initiale du module IoT Central</span><span class="sxs-lookup"><span data-stu-id="de833-1650">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="de833-1651">KeyVault</span><span class="sxs-lookup"><span data-stu-id="de833-1651">KeyVault</span></span>


* <span data-ttu-id="de833-1652">Ajout des commandes pour la gestion des comptes de stockage et les définitions SAS</span><span class="sxs-lookup"><span data-stu-id="de833-1652">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="de833-1653">Ajout de commandes pour les règles réseau</span><span class="sxs-lookup"><span data-stu-id="de833-1653">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="de833-1654">Ajout du paramètre `--id` aux opérations relatives au mots de passe confidentiels, clés et certificats</span><span class="sxs-lookup"><span data-stu-id="de833-1654">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="de833-1655">Ajout de la prise en charge pour la version multi-api avec gestion des coffres de clés</span><span class="sxs-lookup"><span data-stu-id="de833-1655">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="de833-1656">Ajout de la prise en charge pour la version multi-api avec plan de données des coffres de clés</span><span class="sxs-lookup"><span data-stu-id="de833-1656">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="de833-1657">Relais</span><span class="sxs-lookup"><span data-stu-id="de833-1657">Relay</span></span>

* <span data-ttu-id="de833-1658">Version initiale</span><span class="sxs-lookup"><span data-stu-id="de833-1658">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="de833-1659">SQL</span><span class="sxs-lookup"><span data-stu-id="de833-1659">Sql</span></span>

* <span data-ttu-id="de833-1660">Ajout des commandes `sql failover-group`</span><span class="sxs-lookup"><span data-stu-id="de833-1660">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="de833-1661">Stockage</span><span class="sxs-lookup"><span data-stu-id="de833-1661">Storage</span></span>

* <span data-ttu-id="de833-1662">[CHANGEMENT CASSANT] Modification de `storage account show-usage` afin d’exiger le paramètre `--location` et de répertorier par région</span><span class="sxs-lookup"><span data-stu-id="de833-1662">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="de833-1663">Modification du paramètre `--resource-group` afin de le rendre facultatif pour les commandes `storage account`</span><span class="sxs-lookup"><span data-stu-id="de833-1663">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="de833-1664">Suppression des avertissements concernant l’échec de la condition préalable pour les défaillances isolées dans les commandes batch pour les messages agrégés uniques</span><span class="sxs-lookup"><span data-stu-id="de833-1664">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="de833-1665">Modification des commandes `[blob|file] delete-batch` afin de ne plus produire des tableaux ayant la valeur null</span><span class="sxs-lookup"><span data-stu-id="de833-1665">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="de833-1666">Modification des commandes `blob [download|upload|delete-batch]` afin de lire le jeton de SAS à partir de l’url du conteneur</span><span class="sxs-lookup"><span data-stu-id="de833-1666">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="de833-1667">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="de833-1667">VM</span></span>

* <span data-ttu-id="de833-1668">Ajout des filtres courants à `vm list-skus` pour une plus grande simplicité d’utilisation</span><span class="sxs-lookup"><span data-stu-id="de833-1668">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="de833-1669">31 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="de833-1669">July 31, 2018</span></span>

<span data-ttu-id="de833-1670">Version 2.0.43</span><span class="sxs-lookup"><span data-stu-id="de833-1670">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="de833-1671">ACR</span><span class="sxs-lookup"><span data-stu-id="de833-1671">ACR</span></span>

* <span data-ttu-id="de833-1672">Ajout de l’indicateur `--with-secure-properties` à la commande `acr build-task show`</span><span class="sxs-lookup"><span data-stu-id="de833-1672">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="de833-1673">Ajout de la commande `acr build-task update-build`</span><span class="sxs-lookup"><span data-stu-id="de833-1673">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="de833-1674">ACS</span><span class="sxs-lookup"><span data-stu-id="de833-1674">ACS</span></span>

* <span data-ttu-id="de833-1675">Retour au return 0 (réussite) à la fin de `az aks browse` en appuyant sur [Ctrl + C]</span><span class="sxs-lookup"><span data-stu-id="de833-1675">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="de833-1676">Batch</span><span class="sxs-lookup"><span data-stu-id="de833-1676">Batch</span></span>

* <span data-ttu-id="de833-1677">Correction du bug lors de l’affichage des jetons AAD dans le Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="de833-1677">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="de833-1678">Conteneur</span><span class="sxs-lookup"><span data-stu-id="de833-1678">Container</span></span>

* <span data-ttu-id="de833-1679">Suppression de l’exigence pour `--log-analytics-workspace-key` pour le nom ou l’identifiant lors de l’abonnement standard</span><span class="sxs-lookup"><span data-stu-id="de833-1679">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="de833-1680">Réseau</span><span class="sxs-lookup"><span data-stu-id="de833-1680">Network</span></span>

* <span data-ttu-id="de833-1681">Ajout du serveur DNS au profil du 09/03/2017 pour Azure Stack</span><span class="sxs-lookup"><span data-stu-id="de833-1681">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="de833-1682">Ressource</span><span class="sxs-lookup"><span data-stu-id="de833-1682">Resource</span></span>

* <span data-ttu-id="de833-1683">Ajout de `--rollback-on-error` à `group deployment create` pour exécuter un déploiement correct et connu en cas d’erreur</span><span class="sxs-lookup"><span data-stu-id="de833-1683">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="de833-1684">Correction d’un problème où `--parameters {}` avec `group deployment create` entraînait une erreur</span><span class="sxs-lookup"><span data-stu-id="de833-1684">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="de833-1685">Role</span><span class="sxs-lookup"><span data-stu-id="de833-1685">Role</span></span>

* <span data-ttu-id="de833-1686">Ajout de la prise en charge du profil stack du 09/03/2017</span><span class="sxs-lookup"><span data-stu-id="de833-1686">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="de833-1687">Correction d’un problème où les paramètres de mise à jour génériques à `app update` ne fonctionnaient pas correctement</span><span class="sxs-lookup"><span data-stu-id="de833-1687">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="de833-1688">Recherche</span><span class="sxs-lookup"><span data-stu-id="de833-1688">Search</span></span>

* <span data-ttu-id="de833-1689">Ajout de commandes pour le service de recherches d’Azure</span><span class="sxs-lookup"><span data-stu-id="de833-1689">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="de833-1690">Service Bus</span><span class="sxs-lookup"><span data-stu-id="de833-1690">Service Bus</span></span>

* <span data-ttu-id="de833-1691">Ajout d’un groupe de commandes de migration pour migrer un espace de noms d’un Service Bus Standard à un Premium</span><span class="sxs-lookup"><span data-stu-id="de833-1691">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="de833-1692">Ajout de nouvelles propriétés facultatives à la file d’attente du Service Bus et à l’abonnement</span><span class="sxs-lookup"><span data-stu-id="de833-1692">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="de833-1693">`--enable-batched-operations` et `--enable-dead-lettering-on-message-expiration` dans `queue`</span><span class="sxs-lookup"><span data-stu-id="de833-1693">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="de833-1694">`--dead-letter-on-filter-exceptions` dans `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="de833-1694">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="de833-1695">Stockage</span><span class="sxs-lookup"><span data-stu-id="de833-1695">Storage</span></span>

* <span data-ttu-id="de833-1696">Ajout de la prise en charge du téléchargement de fichiers volumineux à l’aide d’une connexion unique</span><span class="sxs-lookup"><span data-stu-id="de833-1696">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="de833-1697">Conversion des commandes `show` qui manquaient d’échouer avec le code de sortie 3 sur une ressource manquante</span><span class="sxs-lookup"><span data-stu-id="de833-1697">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="de833-1698">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="de833-1698">VM</span></span>

* <span data-ttu-id="de833-1699">Ajout d’une prise en charge pour lister les groupes disponibles par abonnement</span><span class="sxs-lookup"><span data-stu-id="de833-1699">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="de833-1700">Ajout de la prise en charge de `StandardSSD_LRS`</span><span class="sxs-lookup"><span data-stu-id="de833-1700">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="de833-1701">Ajout d’une prise en charge des groupes de sécurité d’application dans la création du groupe identique de machines virtuelles</span><span class="sxs-lookup"><span data-stu-id="de833-1701">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="de833-1702">[CHANGEMENT CASSANT] Changement de `[vm|vmss] create`, `[vm|vmss] identity assign`, et `[vm|vmss] identity remove` pour sortir les identités des utilisateurs au format de dictionnaire</span><span class="sxs-lookup"><span data-stu-id="de833-1702">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="de833-1703">18 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="de833-1703">July 18, 2018</span></span>

<span data-ttu-id="de833-1704">Version 2.0.42</span><span class="sxs-lookup"><span data-stu-id="de833-1704">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="de833-1705">Core</span><span class="sxs-lookup"><span data-stu-id="de833-1705">Core</span></span>

* <span data-ttu-id="de833-1706">Ajout de la prise en charge de la connexion basée sur le navigateur dans la fenêtre d’interpréteur de commandes Windows pour Linux</span><span class="sxs-lookup"><span data-stu-id="de833-1706">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="de833-1707">Ajout de l’indicateur `--force-string` pour toutes les commandes de mise à jour générique</span><span class="sxs-lookup"><span data-stu-id="de833-1707">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="de833-1708">[CHANGEMENT CASSANT] Modification des commandes « d’affichage » pour connecter le message d’erreur et échec avec un code de sortie de 3 sur une ressource manquante</span><span class="sxs-lookup"><span data-stu-id="de833-1708">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="de833-1709">ACR</span><span class="sxs-lookup"><span data-stu-id="de833-1709">ACR</span></span>

* <span data-ttu-id="de833-1710">[CHANGEMENT CASSANT] Mise à jour de « --no-push » vers un indicateur pur dans la commande « ACR Build »</span><span class="sxs-lookup"><span data-stu-id="de833-1710">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="de833-1711">Ajout des commandes `show` et `update` sous le groupe `acr repository`</span><span class="sxs-lookup"><span data-stu-id="de833-1711">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="de833-1712">Ajout de l’indicateur `--detail` à `show-manifests` et `show-tags` pour afficher des informations plus détaillées</span><span class="sxs-lookup"><span data-stu-id="de833-1712">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="de833-1713">Ajout du paramètre `--image` pour prendre en charge l’obtention des détails de build ou des journaux d’activité par une image</span><span class="sxs-lookup"><span data-stu-id="de833-1713">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="de833-1714">ACS</span><span class="sxs-lookup"><span data-stu-id="de833-1714">ACS</span></span>

* <span data-ttu-id="de833-1715">Modification de `az aks create` en sortie d’erreur si `--max-pods` est inférieur à 5</span><span class="sxs-lookup"><span data-stu-id="de833-1715">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="de833-1716">AppService</span><span class="sxs-lookup"><span data-stu-id="de833-1716">AppService</span></span>

* <span data-ttu-id="de833-1717">Ajout de la prise en charge pour les références (SKU) PremiumV2</span><span class="sxs-lookup"><span data-stu-id="de833-1717">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="de833-1718">Batch</span><span class="sxs-lookup"><span data-stu-id="de833-1718">Batch</span></span>

* <span data-ttu-id="de833-1719">Correction d’un bogue relatif à l’utilisation des informations d’identification de jeton dans le mode Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="de833-1719">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="de833-1720">Modification de l’entrée JSON pour respecter la casse</span><span class="sxs-lookup"><span data-stu-id="de833-1720">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="de833-1721">Batch AI</span><span class="sxs-lookup"><span data-stu-id="de833-1721">Batch AI</span></span>

* <span data-ttu-id="de833-1722">Correction de la commande `az batchai job exec`</span><span class="sxs-lookup"><span data-stu-id="de833-1722">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="de833-1723">Conteneur</span><span class="sxs-lookup"><span data-stu-id="de833-1723">Container</span></span>

* <span data-ttu-id="de833-1724">Suppression des exigences pour le nom d’utilisateur et le mot de passe pour les registres non dockerhub</span><span class="sxs-lookup"><span data-stu-id="de833-1724">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="de833-1725">Correction de l’erreur lors de la création de groupes de conteneur à partir du fichier yaml</span><span class="sxs-lookup"><span data-stu-id="de833-1725">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="de833-1726">Réseau</span><span class="sxs-lookup"><span data-stu-id="de833-1726">Network</span></span>

* <span data-ttu-id="de833-1727">Ajout de la prise en charge de `--no-wait` pour `network nic [create|update|delete]`</span><span class="sxs-lookup"><span data-stu-id="de833-1727">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="de833-1728">Ajout de `network nic wait`</span><span class="sxs-lookup"><span data-stu-id="de833-1728">Added `network nic wait`</span></span>
* <span data-ttu-id="de833-1729">Argument `--ids` déconseillé pour `network vnet [subnet|peering] list`</span><span class="sxs-lookup"><span data-stu-id="de833-1729">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="de833-1730">Ajout de l’indicateur `--include-default` pour inclure les règles de sécurité par défaut dans la sortie de `network nsg rule list`</span><span class="sxs-lookup"><span data-stu-id="de833-1730">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="de833-1731">Ressource</span><span class="sxs-lookup"><span data-stu-id="de833-1731">Resource</span></span>

* <span data-ttu-id="de833-1732">Ajout de la prise en charge de `--no-wait` pour `group deployment delete`</span><span class="sxs-lookup"><span data-stu-id="de833-1732">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="de833-1733">Ajout de la prise en charge de `--no-wait` pour `deployment delete`</span><span class="sxs-lookup"><span data-stu-id="de833-1733">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="de833-1734">Ajout de la commande `deployment wait`</span><span class="sxs-lookup"><span data-stu-id="de833-1734">Added `deployment wait` command</span></span>
* <span data-ttu-id="de833-1735">Résolution du problème qui causait l’affichage par erreur des commandes `az deployment` du niveau de l’abonnement pour le profil 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="de833-1735">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="de833-1736">SQL</span><span class="sxs-lookup"><span data-stu-id="de833-1736">SQL</span></span>

* <span data-ttu-id="de833-1737">Résolution de l’erreur « Le nom du groupe de ressources fourni ne correspond pas au nom de l’URL » lors de la spécification du nom du pool élastique pour les commandes `sql db copy` et `sql db replica create`</span><span class="sxs-lookup"><span data-stu-id="de833-1737">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="de833-1738">Autoriser la configuration de SQL Server par défaut en exécutant `az configure --defaults sql-server=<name>`</span><span class="sxs-lookup"><span data-stu-id="de833-1738">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="de833-1739">Implémentation de formateurs de table pour les commandes `sql server`, `sql server firewall-rule`, `sql list-usages` et `sql show-usage`</span><span class="sxs-lookup"><span data-stu-id="de833-1739">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="de833-1740">Stockage</span><span class="sxs-lookup"><span data-stu-id="de833-1740">Storage</span></span>

* <span data-ttu-id="de833-1741">Ajout de la propriété `pageRanges` à la sortie `storage blob show` qui sera renseignée pour les objets blob de pages</span><span class="sxs-lookup"><span data-stu-id="de833-1741">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="de833-1742">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="de833-1742">VM</span></span>

* <span data-ttu-id="de833-1743">[CHANGEMENT CASSANT] Modification de `vmss create` pour utiliser `Standard_DS1_v2` comme taille d’instance par défaut</span><span class="sxs-lookup"><span data-stu-id="de833-1743">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="de833-1744">Ajout de la prise en charge de `--no-wait` pour `vm extension [set|delete]` et `vmss extension [set|delete]`</span><span class="sxs-lookup"><span data-stu-id="de833-1744">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="de833-1745">Ajout de `vm extension wait`</span><span class="sxs-lookup"><span data-stu-id="de833-1745">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="de833-1746">3 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="de833-1746">July 3, 2018</span></span>

<span data-ttu-id="de833-1747">Version 2.0.41</span><span class="sxs-lookup"><span data-stu-id="de833-1747">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="de833-1748">AKS</span><span class="sxs-lookup"><span data-stu-id="de833-1748">AKS</span></span>

* <span data-ttu-id="de833-1749">Modification de la surveillance pour utiliser l’ID d’abonnement</span><span class="sxs-lookup"><span data-stu-id="de833-1749">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="de833-1750">3 juillet 2018</span><span class="sxs-lookup"><span data-stu-id="de833-1750">July 3, 2018</span></span>

<span data-ttu-id="de833-1751">Version 2.0.40</span><span class="sxs-lookup"><span data-stu-id="de833-1751">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="de833-1752">Core</span><span class="sxs-lookup"><span data-stu-id="de833-1752">Core</span></span>

* <span data-ttu-id="de833-1753">Ajout d’un nouveau flux de code d’autorisation pour une connexion interactive</span><span class="sxs-lookup"><span data-stu-id="de833-1753">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="de833-1754">ACR</span><span class="sxs-lookup"><span data-stu-id="de833-1754">ACR</span></span>

* <span data-ttu-id="de833-1755">Ajout de l’interrogation de l’état du build</span><span class="sxs-lookup"><span data-stu-id="de833-1755">Added polling build status</span></span>
* <span data-ttu-id="de833-1756">Ajout de la prise en charge des valeurs d’énumération ne respectant pas la casse</span><span class="sxs-lookup"><span data-stu-id="de833-1756">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="de833-1757">Ajout des paramètres `--top` et `--orderby` pour `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="de833-1757">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="de833-1758">ACS</span><span class="sxs-lookup"><span data-stu-id="de833-1758">ACS</span></span>

* <span data-ttu-id="de833-1759">[CHANGEMENT CASSANT] Active le contrôle d’accès en fonction du rôle Kubernetes par défaut</span><span class="sxs-lookup"><span data-stu-id="de833-1759">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="de833-1760">Ajout de l’argument `--disable-rbac` et dépréciation de `--enable-rbac` dans la mesure où il s’agit actuellement de la valeur par défaut</span><span class="sxs-lookup"><span data-stu-id="de833-1760">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="de833-1761">Mise à jour des options de la commande `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="de833-1761">Updated options for `aks browse` command.</span></span> <span data-ttu-id="de833-1762">Ajout de la prise en charge de `--listen-port`</span><span class="sxs-lookup"><span data-stu-id="de833-1762">Added `--listen-port` support</span></span>
* <span data-ttu-id="de833-1763">Mise à jour du package de graphique Helm par défaut pour la commande `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="de833-1763">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="de833-1764">Use virtual-kubelet-for-aks-latest.tgz</span><span class="sxs-lookup"><span data-stu-id="de833-1764">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="de833-1765">Ajout des commandes `aks enable-addons` et `aks disable-addons` pour mettre à jour un cluster existant</span><span class="sxs-lookup"><span data-stu-id="de833-1765">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="de833-1766">AppService</span><span class="sxs-lookup"><span data-stu-id="de833-1766">AppService</span></span>

* <span data-ttu-id="de833-1767">Ajout de la prise en charge de la désactivation d’identité via `webapp identity remove`</span><span class="sxs-lookup"><span data-stu-id="de833-1767">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="de833-1768">Suppression de la balise `preview` pour la fonctionnalité Identité</span><span class="sxs-lookup"><span data-stu-id="de833-1768">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="de833-1769">Backup</span><span class="sxs-lookup"><span data-stu-id="de833-1769">Backup</span></span>

* <span data-ttu-id="de833-1770">Mise à jour de la définition du module</span><span class="sxs-lookup"><span data-stu-id="de833-1770">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="de833-1771">Batch AI</span><span class="sxs-lookup"><span data-stu-id="de833-1771">BatchAI</span></span>

* <span data-ttu-id="de833-1772">Correction de la sortie de table pour les commandes `batchai cluster node list` et `batchai job node list`</span><span class="sxs-lookup"><span data-stu-id="de833-1772">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="de833-1773">Cloud</span><span class="sxs-lookup"><span data-stu-id="de833-1773">Cloud</span></span>

* <span data-ttu-id="de833-1774">Ajout du suffixe de serveur `acr login` à la configuration du cloud</span><span class="sxs-lookup"><span data-stu-id="de833-1774">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="de833-1775">Conteneur</span><span class="sxs-lookup"><span data-stu-id="de833-1775">Container</span></span>

* <span data-ttu-id="de833-1776">Modification de `container create` sur valeur par défaut en opération à long terme</span><span class="sxs-lookup"><span data-stu-id="de833-1776">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="de833-1777">Ajout des paramètres Log Analytics `--log-analytics-workspace` et `--log-analytics-workspace-key`</span><span class="sxs-lookup"><span data-stu-id="de833-1777">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="de833-1778">Ajout du paramètre `--protocol` pour spécifier le protocole réseau à utiliser</span><span class="sxs-lookup"><span data-stu-id="de833-1778">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="de833-1779">Extension</span><span class="sxs-lookup"><span data-stu-id="de833-1779">Extension</span></span>

* <span data-ttu-id="de833-1780">Modification de `extension list-available` pour afficher uniquement les extensions compatibles avec la version CLI</span><span class="sxs-lookup"><span data-stu-id="de833-1780">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="de833-1781">Réseau</span><span class="sxs-lookup"><span data-stu-id="de833-1781">Network</span></span>

* <span data-ttu-id="de833-1782">Résolution du problème où les types d’enregistrement étaient sensibles à la casse pour ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="de833-1782">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="de833-1783">Rdbms</span><span class="sxs-lookup"><span data-stu-id="de833-1783">Rdbms</span></span>

* <span data-ttu-id="de833-1784">Ajout des commandes `[postgres|myql] server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="de833-1784">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="de833-1785">Ressource</span><span class="sxs-lookup"><span data-stu-id="de833-1785">Resource</span></span>

* <span data-ttu-id="de833-1786">Ajout d’un nouveau groupe d’opérations `deployment`</span><span class="sxs-lookup"><span data-stu-id="de833-1786">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="de833-1787">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="de833-1787">VM</span></span>

* <span data-ttu-id="de833-1788">Ajout de la prise en charge de la suppression de l’identité affectée au système</span><span class="sxs-lookup"><span data-stu-id="de833-1788">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="de833-1789">25 juin 2018</span><span class="sxs-lookup"><span data-stu-id="de833-1789">June 25, 2018</span></span>

<span data-ttu-id="de833-1790">Version 2.0.39</span><span class="sxs-lookup"><span data-stu-id="de833-1790">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="de833-1791">Interface de ligne de commande</span><span class="sxs-lookup"><span data-stu-id="de833-1791">CLI</span></span>

* <span data-ttu-id="de833-1792">Mise à jour de la suppression du fichier dans le programme d’installation MSI pour résoudre le problème d’installation de l’extension</span><span class="sxs-lookup"><span data-stu-id="de833-1792">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="de833-1793">19 juin 2018</span><span class="sxs-lookup"><span data-stu-id="de833-1793">June 19, 2018</span></span>

<span data-ttu-id="de833-1794">Version 2.0.38</span><span class="sxs-lookup"><span data-stu-id="de833-1794">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="de833-1795">Core</span><span class="sxs-lookup"><span data-stu-id="de833-1795">Core</span></span>

* <span data-ttu-id="de833-1796">Ajout de la prise en charge globale de `--subscription` pour la plupart des commandes</span><span class="sxs-lookup"><span data-stu-id="de833-1796">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="de833-1797">ACR</span><span class="sxs-lookup"><span data-stu-id="de833-1797">ACR</span></span>

* <span data-ttu-id="de833-1798">Ajout de `azure-storage-blob` comme dépendance</span><span class="sxs-lookup"><span data-stu-id="de833-1798">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="de833-1799">Modification de la configuration de l’UC par défaut avec `acr build-task create` pour utiliser 2 cœurs</span><span class="sxs-lookup"><span data-stu-id="de833-1799">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="de833-1800">ACS</span><span class="sxs-lookup"><span data-stu-id="de833-1800">ACS</span></span>

* <span data-ttu-id="de833-1801">Mise à jour des options de la commande `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="de833-1801">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="de833-1802">Ajout de la prise en charge de `--update`</span><span class="sxs-lookup"><span data-stu-id="de833-1802">Added `--update` support</span></span>
* <span data-ttu-id="de833-1803">Modification de `aks get-credentials --admin` pour ne pas remplacer le contexte utilisateur dans `$HOME/.kube/config`</span><span class="sxs-lookup"><span data-stu-id="de833-1803">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="de833-1804">Exposition de la propriété en lecture seule `nodeResourceGroup` sur les clusters managés</span><span class="sxs-lookup"><span data-stu-id="de833-1804">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="de833-1805">Correction de l’erreur de commande `acs browse`</span><span class="sxs-lookup"><span data-stu-id="de833-1805">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="de833-1806">`--connector-name` rendu facultatif pour `aks install-connector`, `aks upgrade-connector` et `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="de833-1806">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="de833-1807">Ajout de nouvelles régions Azure Container Instance pour `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="de833-1807">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="de833-1808">Ajout de l’emplacement normalisé dans le nom de mise en production Helm et le nom du nœud pour `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="de833-1808">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="de833-1809">AppService</span><span class="sxs-lookup"><span data-stu-id="de833-1809">AppService</span></span>

* <span data-ttu-id="de833-1810">Ajout de la prise en charge des versions urllib plus récentes</span><span class="sxs-lookup"><span data-stu-id="de833-1810">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="de833-1811">Ajout de la prise en charge pour `functionapp create` pour utiliser un plan App Service à partir de groupes de ressources externes</span><span class="sxs-lookup"><span data-stu-id="de833-1811">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="de833-1812">Batch</span><span class="sxs-lookup"><span data-stu-id="de833-1812">Batch</span></span>

* <span data-ttu-id="de833-1813">Suppression de la dépendance `azure-batch-extensions`</span><span class="sxs-lookup"><span data-stu-id="de833-1813">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="de833-1814">Batch AI</span><span class="sxs-lookup"><span data-stu-id="de833-1814">Batch AI</span></span>

* <span data-ttu-id="de833-1815">Ajout de la prise en charge des espaces de travail.</span><span class="sxs-lookup"><span data-stu-id="de833-1815">Added support for workspaces.</span></span> <span data-ttu-id="de833-1816">Les espaces de travail permettent de regrouper les clusters, serveurs de fichiers et expériences, supprimant la limitation du nombre de ressources qui peuvent être créées</span><span class="sxs-lookup"><span data-stu-id="de833-1816">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="de833-1817">Ajout de la prise en charge des expériences.</span><span class="sxs-lookup"><span data-stu-id="de833-1817">Added support for experiments.</span></span> <span data-ttu-id="de833-1818">Les expériences permettent de regrouper les tâches dans des collections, supprimant la limitation du nombre de tâches créées</span><span class="sxs-lookup"><span data-stu-id="de833-1818">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="de833-1819">Ajout de la prise en charge pour configurer `/dev/shm` pour les travaux en cours d’exécution dans un conteneur docker</span><span class="sxs-lookup"><span data-stu-id="de833-1819">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="de833-1820">Ajout des commandes `batchai cluster node exec` et `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="de833-1820">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="de833-1821">Ces commandes permettent d’exécuter des commandes directement sur les nœuds et fournissent la fonctionnalité de réacheminement de port.</span><span class="sxs-lookup"><span data-stu-id="de833-1821">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="de833-1822">Ajout de la prise en charge des commandes `--ids` et `batchai`</span><span class="sxs-lookup"><span data-stu-id="de833-1822">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="de833-1823">[CHANGEMENT CASSANT] Tous les clusters et serveurs de fichiers doivent être créés dans des espaces de travail</span><span class="sxs-lookup"><span data-stu-id="de833-1823">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="de833-1824">[CHANGEMENT CASSANT] Les travaux doivent être créés dans des expériences</span><span class="sxs-lookup"><span data-stu-id="de833-1824">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="de833-1825">[CHANGEMENT CASSANT] Suppression de `--nfs-resource-group` des commandes `cluster create` et `job create`.</span><span class="sxs-lookup"><span data-stu-id="de833-1825">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="de833-1826">Pour monter un NFS appartenant à un autre espace de travail/groupe de ressources, indiquez l’ID ARM du serveur de fichiers via l’option `--nfs`</span><span class="sxs-lookup"><span data-stu-id="de833-1826">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="de833-1827">[CHANGEMENT CASSANT] Suppression de `--cluster-resource-group` de la commande `job create`.</span><span class="sxs-lookup"><span data-stu-id="de833-1827">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="de833-1828">Pour soumettre un travail sur un cluster appartenant à un autre espace de travail/groupe de ressources, indiquez l’ID ARM du cluster via l’option `--cluster`</span><span class="sxs-lookup"><span data-stu-id="de833-1828">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="de833-1829">[CHANGEMENT CASSANT] Suppression de l’attribut `location` des travaux, clusters et serveurs de fichiers.</span><span class="sxs-lookup"><span data-stu-id="de833-1829">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="de833-1830">L’emplacement est maintenant un attribut d’espace de travail.</span><span class="sxs-lookup"><span data-stu-id="de833-1830">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="de833-1831">[CHANGEMENT CASSANT] Suppression de `--location` des commandes `job create`, `cluster create` et `file-server create`</span><span class="sxs-lookup"><span data-stu-id="de833-1831">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="de833-1832">[CHANGEMENT CASSANT] Modification des noms des options courtes pour rendre l’interface plus cohérente :</span><span class="sxs-lookup"><span data-stu-id="de833-1832">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="de833-1833">[`--config`, `-c`] renommé en [`--config-file`, `-f`]</span><span class="sxs-lookup"><span data-stu-id="de833-1833">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="de833-1834">[`--cluster`, `-r`] renommé en [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="de833-1834">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="de833-1835">[`--cluster`, `-n`] renommé en [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="de833-1835">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="de833-1836">[`--job`, `-n`] renommé en [`--job`, `-j`]</span><span class="sxs-lookup"><span data-stu-id="de833-1836">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="de833-1837">Cartes</span><span class="sxs-lookup"><span data-stu-id="de833-1837">Maps</span></span>

* <span data-ttu-id="de833-1838">[CHANGEMENT CASSANT] Modification de `maps account create` pour accepter les Conditions d’utilisation, soit par l’invite interactive ou par l’indicateur `--accept-tos`</span><span class="sxs-lookup"><span data-stu-id="de833-1838">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="de833-1839">Réseau</span><span class="sxs-lookup"><span data-stu-id="de833-1839">Network</span></span>

* <span data-ttu-id="de833-1840">Ajout de la prise en charge de `https` à `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="de833-1840">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="de833-1841">Correction d’un problème où `--endpoint-status` était sensible à la casse.</span><span class="sxs-lookup"><span data-stu-id="de833-1841">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="de833-1842">#6502</span><span class="sxs-lookup"><span data-stu-id="de833-1842">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="de833-1843">Réservations</span><span class="sxs-lookup"><span data-stu-id="de833-1843">Reservations</span></span>

* <span data-ttu-id="de833-1844">[CHANGEMENT CASSANT] Ajout du paramètre obligatoire `ReservedResourceType` à `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="de833-1844">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="de833-1845">Ajout du paramètre `Location` à `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="de833-1845">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="de833-1846">[CHANGEMENT CASSANT] Suppression de `kind` de `ReservationProperties`</span><span class="sxs-lookup"><span data-stu-id="de833-1846">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="de833-1847">[CHANGEMENT CASSANT]`capabilities` renommé en `sku_properties` dans `Catalog`</span><span class="sxs-lookup"><span data-stu-id="de833-1847">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="de833-1848">[CHANGEMENT CASSANT] Suppression des propriétés `size` et `tier` de `Catalog`</span><span class="sxs-lookup"><span data-stu-id="de833-1848">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="de833-1849">Ajout du paramètre `InstanceFlexibility` à `reservations reservation update`</span><span class="sxs-lookup"><span data-stu-id="de833-1849">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="de833-1850">Role</span><span class="sxs-lookup"><span data-stu-id="de833-1850">Role</span></span>

* <span data-ttu-id="de833-1851">Amélioration de la gestion des erreurs</span><span class="sxs-lookup"><span data-stu-id="de833-1851">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="de833-1852">SQL</span><span class="sxs-lookup"><span data-stu-id="de833-1852">SQL</span></span>

* <span data-ttu-id="de833-1853">Correction de l’erreur déroutante lors de l’exécution de `az sql db list-editions` pour un emplacement qui n’est pas disponible pour votre abonnement</span><span class="sxs-lookup"><span data-stu-id="de833-1853">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="de833-1854">Stockage</span><span class="sxs-lookup"><span data-stu-id="de833-1854">Storage</span></span>

* <span data-ttu-id="de833-1855">Modification de la sortie de table pour que `storage blob download` soit plus lisible</span><span class="sxs-lookup"><span data-stu-id="de833-1855">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="de833-1856">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="de833-1856">VM</span></span>

* <span data-ttu-id="de833-1857">Amélioration de la vérification de la taille de la machine virtuelle pour la prise en charge de la mise en réseau accélérée dans `vm create`</span><span class="sxs-lookup"><span data-stu-id="de833-1857">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="de833-1858">Ajout d’un avertissement pour `vmss create` indiquant que la taille de la machine virtuelle par défaut va passer de `Standard_D1_v2` à `Standard_DS1_v2`</span><span class="sxs-lookup"><span data-stu-id="de833-1858">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="de833-1859">Ajout de `--force-update` à `[vm|vmss] extension set` pour mettre à jour l’extension, même lorsque la configuration n’a pas changé</span><span class="sxs-lookup"><span data-stu-id="de833-1859">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="de833-1860">13 juin 2018</span><span class="sxs-lookup"><span data-stu-id="de833-1860">June 13, 2018</span></span>

<span data-ttu-id="de833-1861">Version 2.0.37</span><span class="sxs-lookup"><span data-stu-id="de833-1861">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="de833-1862">Core</span><span class="sxs-lookup"><span data-stu-id="de833-1862">Core</span></span>

* <span data-ttu-id="de833-1863">Amélioration de la télémétrie interactive</span><span class="sxs-lookup"><span data-stu-id="de833-1863">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="de833-1864">13 juin 2018</span><span class="sxs-lookup"><span data-stu-id="de833-1864">June 13, 2018</span></span>

<span data-ttu-id="de833-1865">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="de833-1865">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="de833-1866">AKS</span><span class="sxs-lookup"><span data-stu-id="de833-1866">AKS</span></span>

* <span data-ttu-id="de833-1867">Ajout d’options réseau avancées à `aks create`</span><span class="sxs-lookup"><span data-stu-id="de833-1867">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="de833-1868">Ajout d’arguments à `aks create` pour permettre la surveillance et le routage HTTP</span><span class="sxs-lookup"><span data-stu-id="de833-1868">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="de833-1869">Ajout de l’argument `--no-ssh-key` à `aks create`</span><span class="sxs-lookup"><span data-stu-id="de833-1869">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="de833-1870">Ajout de l’argument `--enable-rbac` à `aks create`</span><span class="sxs-lookup"><span data-stu-id="de833-1870">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="de833-1871">[PRÉVERSION] Ajout de la prise en charge pour l’authentification basée sur Azure Active Directory à `aks create`</span><span class="sxs-lookup"><span data-stu-id="de833-1871">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="de833-1872">AppService</span><span class="sxs-lookup"><span data-stu-id="de833-1872">AppService</span></span>

* <span data-ttu-id="de833-1873">Résolution d’un problème lié à des versions urllib incompatibles</span><span class="sxs-lookup"><span data-stu-id="de833-1873">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="de833-1874">5 juin 2018</span><span class="sxs-lookup"><span data-stu-id="de833-1874">June 5, 2018</span></span>

<span data-ttu-id="de833-1875">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="de833-1875">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="de833-1876">Interactive</span><span class="sxs-lookup"><span data-stu-id="de833-1876">Interactive</span></span>

* <span data-ttu-id="de833-1877">Ajout de limites aux dépendances du mode interactif</span><span class="sxs-lookup"><span data-stu-id="de833-1877">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="de833-1878">5 juin 2018</span><span class="sxs-lookup"><span data-stu-id="de833-1878">June 5, 2018</span></span>

<span data-ttu-id="de833-1879">Version 2.0.34</span><span class="sxs-lookup"><span data-stu-id="de833-1879">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="de833-1880">Core</span><span class="sxs-lookup"><span data-stu-id="de833-1880">Core</span></span>

* <span data-ttu-id="de833-1881">Prise en charge supplémentaire pour les références de ressources inter-client</span><span class="sxs-lookup"><span data-stu-id="de833-1881">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="de833-1882">Amélioration de la fiabilité de téléchargement des données de télémétrie</span><span class="sxs-lookup"><span data-stu-id="de833-1882">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="de833-1883">ACR</span><span class="sxs-lookup"><span data-stu-id="de833-1883">ACR</span></span>

* <span data-ttu-id="de833-1884">Prise en charge supplémentaire pour VSTS en tant qu’emplacement source distant</span><span class="sxs-lookup"><span data-stu-id="de833-1884">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="de833-1885">Ajout de la commande `acr import`</span><span class="sxs-lookup"><span data-stu-id="de833-1885">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="de833-1886">AKS</span><span class="sxs-lookup"><span data-stu-id="de833-1886">AKS</span></span>

* <span data-ttu-id="de833-1887">`aks get-credentials` a été modifié pour créer le fichier de configuration kube avec des autorisations de système de fichiers plus sécurisées</span><span class="sxs-lookup"><span data-stu-id="de833-1887">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="de833-1888">Batch</span><span class="sxs-lookup"><span data-stu-id="de833-1888">Batch</span></span>

* <span data-ttu-id="de833-1889">Résolution du bogue concernant la mise en forme dans la table de liste de pool [[problème #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="de833-1889">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="de833-1890">IOT</span><span class="sxs-lookup"><span data-stu-id="de833-1890">IOT</span></span>

* <span data-ttu-id="de833-1891">Prise en charge ajoutée pour la création de IoT Hubs de niveau de base</span><span class="sxs-lookup"><span data-stu-id="de833-1891">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="de833-1892">Réseau</span><span class="sxs-lookup"><span data-stu-id="de833-1892">Network</span></span>

* <span data-ttu-id="de833-1893">`network vnet peering` amélioré</span><span class="sxs-lookup"><span data-stu-id="de833-1893">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="de833-1894">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="de833-1894">Policy Insights</span></span>

* <span data-ttu-id="de833-1895">Version initiale</span><span class="sxs-lookup"><span data-stu-id="de833-1895">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="de833-1896">ARM</span><span class="sxs-lookup"><span data-stu-id="de833-1896">ARM</span></span>

* <span data-ttu-id="de833-1897">Ajout des commandes `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="de833-1897">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="de833-1898">SQL</span><span class="sxs-lookup"><span data-stu-id="de833-1898">SQL</span></span>

* <span data-ttu-id="de833-1899">Ajout de nouvelles commandes d’instance gérée :</span><span class="sxs-lookup"><span data-stu-id="de833-1899">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="de833-1900">Ajout de nouvelles commandes de base de données gérée :</span><span class="sxs-lookup"><span data-stu-id="de833-1900">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="de833-1901">Stockage</span><span class="sxs-lookup"><span data-stu-id="de833-1901">Storage</span></span>

* <span data-ttu-id="de833-1902">Ajout de types MimeTypes supplémentaires pour les formats json et javascript pour être déduit à partir des extensions de fichier</span><span class="sxs-lookup"><span data-stu-id="de833-1902">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="de833-1903">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="de833-1903">VM</span></span>

* <span data-ttu-id="de833-1904">`vm list-skus` a été modifié pour utiliser des colonnes corrigées et ajouter l’avertissement que `Tier` et `Size` seront supprimés</span><span class="sxs-lookup"><span data-stu-id="de833-1904">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="de833-1905">Ajout de l’option `--accelerated-networking` à `vm create`</span><span class="sxs-lookup"><span data-stu-id="de833-1905">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="de833-1906">Ajout de `--tags` à `identity create`</span><span class="sxs-lookup"><span data-stu-id="de833-1906">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="de833-1907">22 mai 2018</span><span class="sxs-lookup"><span data-stu-id="de833-1907">May 22, 2018</span></span>

<span data-ttu-id="de833-1908">Version 2.0.33</span><span class="sxs-lookup"><span data-stu-id="de833-1908">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="de833-1909">Core</span><span class="sxs-lookup"><span data-stu-id="de833-1909">Core</span></span>

* <span data-ttu-id="de833-1910">Ajout de la prise en charge pour le développement de `@` dans les noms de fichiers</span><span class="sxs-lookup"><span data-stu-id="de833-1910">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="de833-1911">ACS</span><span class="sxs-lookup"><span data-stu-id="de833-1911">ACS</span></span>

* <span data-ttu-id="de833-1912">Ajout de nouvelles commandes Dev Spaces `aks use-dev-spaces` et `aks remove-dev-spaces`</span><span class="sxs-lookup"><span data-stu-id="de833-1912">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="de833-1913">Faute de frappe corrigée dans un message d’aide</span><span class="sxs-lookup"><span data-stu-id="de833-1913">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="de833-1914">AppService</span><span class="sxs-lookup"><span data-stu-id="de833-1914">AppService</span></span>

* <span data-ttu-id="de833-1915">Amélioration des commandes de mise à jour générique</span><span class="sxs-lookup"><span data-stu-id="de833-1915">Improved generic update commands</span></span>
* <span data-ttu-id="de833-1916">Ajout de la prise en charge asynchrone pour `webapp deployment source config-zip`</span><span class="sxs-lookup"><span data-stu-id="de833-1916">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="de833-1917">Conteneur</span><span class="sxs-lookup"><span data-stu-id="de833-1917">Container</span></span>

* <span data-ttu-id="de833-1918">Prise en charge ajoutée pour l’exportation d’un groupe de conteneurs au format yaml</span><span class="sxs-lookup"><span data-stu-id="de833-1918">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="de833-1919">Prise en charge ajoutée pour l’utilisation d’un fichier yaml afin de créer/mettre à jour un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="de833-1919">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="de833-1920">Extension</span><span class="sxs-lookup"><span data-stu-id="de833-1920">Extension</span></span>

* <span data-ttu-id="de833-1921">Amélioration de la suppression des extensions</span><span class="sxs-lookup"><span data-stu-id="de833-1921">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="de833-1922">Interactive</span><span class="sxs-lookup"><span data-stu-id="de833-1922">Interactive</span></span>

* <span data-ttu-id="de833-1923">La journalisation a été modifiée pour désactiver l’analyseur pour les saisies semi-automatiques</span><span class="sxs-lookup"><span data-stu-id="de833-1923">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="de833-1924">Gestion améliorée des caches d’aide incorrects</span><span class="sxs-lookup"><span data-stu-id="de833-1924">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="de833-1925">KeyVault</span><span class="sxs-lookup"><span data-stu-id="de833-1925">KeyVault</span></span>

* <span data-ttu-id="de833-1926">Commandes keyvault corrigées afin de fonctionner dans Cloud Shell ou dans des machines virtuelles avec l’identité</span><span class="sxs-lookup"><span data-stu-id="de833-1926">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="de833-1927">Réseau</span><span class="sxs-lookup"><span data-stu-id="de833-1927">Network</span></span>

* <span data-ttu-id="de833-1928">Résolution d’un problème où `network watcher show-topology` ne fonctionnait pas avec le nom de réseau virtuel et/ou de sous-réseau [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="de833-1928">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="de833-1929">Correction d’un problème où certaines commandes `network watcher` revendiquaient que Network Watcher n’était pas activé pour certaines régions alors qu’il l’était [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="de833-1929">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="de833-1930">SQL</span><span class="sxs-lookup"><span data-stu-id="de833-1930">SQL</span></span>

* <span data-ttu-id="de833-1931">[CHANGEMENT CASSANT] Objets de réponse retournés modifiés à partir des commandes `db` et `dw`</span><span class="sxs-lookup"><span data-stu-id="de833-1931">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="de833-1932">Propriété `serviceLevelObjective` renommée en `currentServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="de833-1932">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="de833-1933">Suppression des propriétés `currentServiceObjectiveId` et `requestedServiceObjectiveId`</span><span class="sxs-lookup"><span data-stu-id="de833-1933">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="de833-1934">Propriété `maxSizeBytes` modifiée en valeur entière au lieu d’une chaîne</span><span class="sxs-lookup"><span data-stu-id="de833-1934">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="de833-1935">[CHANGEMENT CASSANT] Les propriétés `db` et `dw` suivantes ont été modifiées pour être en lecture seule :</span><span class="sxs-lookup"><span data-stu-id="de833-1935">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="de833-1936">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="de833-1936">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="de833-1937">Pour mettre à jour, utilisez le paramètre `--service-objective` ou définissez la propriété `sku.name`</span><span class="sxs-lookup"><span data-stu-id="de833-1937">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="de833-1938">`edition`.</span><span class="sxs-lookup"><span data-stu-id="de833-1938">`edition`.</span></span> <span data-ttu-id="de833-1939">Pour mettre à jour, utilisez le paramètre `--edition` ou définissez la propriété `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="de833-1939">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="de833-1940">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="de833-1940">`elasticPoolName`.</span></span> <span data-ttu-id="de833-1941">Pour mettre à jour, utilisez le paramètre `--elastic-pool` ou définissez la propriété `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="de833-1941">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="de833-1942">[CHANGEMENT CASSANT] Les propriétés `elastic-pool` suivantes ont été modifiées pour être en lecture seule :</span><span class="sxs-lookup"><span data-stu-id="de833-1942">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="de833-1943">`edition`.</span><span class="sxs-lookup"><span data-stu-id="de833-1943">`edition`.</span></span> <span data-ttu-id="de833-1944">Pour mettre à jour, utilisez le paramètre `--edition`</span><span class="sxs-lookup"><span data-stu-id="de833-1944">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="de833-1945">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="de833-1945">`dtu`.</span></span> <span data-ttu-id="de833-1946">Pour mettre à jour, utilisez le paramètre `--capacity`</span><span class="sxs-lookup"><span data-stu-id="de833-1946">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="de833-1947">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="de833-1947">`databaseDtuMin`.</span></span> <span data-ttu-id="de833-1948">Pour mettre à jour, utilisez le paramètre `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="de833-1948">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="de833-1949">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="de833-1949">`databaseDtuMax`.</span></span> <span data-ttu-id="de833-1950">Pour mettre à jour, utilisez le paramètre `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="de833-1950">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="de833-1951">Ajout des paramètres `--family` et `--capacity` aux commandes `db`, `dw` et `elastic-pool`</span><span class="sxs-lookup"><span data-stu-id="de833-1951">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="de833-1952">Ajout de formateurs de table aux commandes `db`, `dw` et `elastic-pool`</span><span class="sxs-lookup"><span data-stu-id="de833-1952">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="de833-1953">Stockage</span><span class="sxs-lookup"><span data-stu-id="de833-1953">Storage</span></span>

* <span data-ttu-id="de833-1954">Ajout d’un compléteur pour l’argument `--account-name`</span><span class="sxs-lookup"><span data-stu-id="de833-1954">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="de833-1955">Correction d’un problème avec `storage entity query`</span><span class="sxs-lookup"><span data-stu-id="de833-1955">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="de833-1956">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="de833-1956">VM</span></span>

* <span data-ttu-id="de833-1957">[CHANGEMENT CASSANT] Suppression de `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="de833-1957">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="de833-1958">La même prise en charge est accessible via `vm update` ou `vm disk attach`</span><span class="sxs-lookup"><span data-stu-id="de833-1958">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="de833-1959">Correction de l’image de l’extension efficace dans `[vm|vmss] extension`</span><span class="sxs-lookup"><span data-stu-id="de833-1959">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="de833-1960">Ajout de`--boot-diagnostics-storage` à `vm create` pour capturer le journal de démarrage</span><span class="sxs-lookup"><span data-stu-id="de833-1960">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="de833-1961">Ajout de `--license-type` à `[vm|vmss] update`</span><span class="sxs-lookup"><span data-stu-id="de833-1961">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="de833-1962">7 mai 2018</span><span class="sxs-lookup"><span data-stu-id="de833-1962">May 7, 2018</span></span>

<span data-ttu-id="de833-1963">Version 2.0.32</span><span class="sxs-lookup"><span data-stu-id="de833-1963">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="de833-1964">Core</span><span class="sxs-lookup"><span data-stu-id="de833-1964">Core</span></span>

* <span data-ttu-id="de833-1965">Correction d’une exception non gérée lors de la récupération des clés secrètes à partir d’un compte de principal de service avec certificat</span><span class="sxs-lookup"><span data-stu-id="de833-1965">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="de833-1966">Nouvelle prise en charge limitée pour les arguments positionnels</span><span class="sxs-lookup"><span data-stu-id="de833-1966">Added limited support for positional arguments</span></span>
* <span data-ttu-id="de833-1967">Correction d’un problème où `--query` ne pouvait pas être utilisé avec `--ids`.</span><span class="sxs-lookup"><span data-stu-id="de833-1967">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="de833-1968">#5591</span><span class="sxs-lookup"><span data-stu-id="de833-1968">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="de833-1969">Amélioration des scénarios de redirection à partir des commandes en utilisant `--ids`.</span><span class="sxs-lookup"><span data-stu-id="de833-1969">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="de833-1970">Prend en charge `-o tsv` avec une requête spécifiée ou `-o json` sans spécification de requête</span><span class="sxs-lookup"><span data-stu-id="de833-1970">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="de833-1971">Ajout de suggestions de commande en cas d’erreur engendrées par des fautes de frappe des utilisateurs dans les commandes</span><span class="sxs-lookup"><span data-stu-id="de833-1971">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="de833-1972">Amélioration de l’erreur lorsque les utilisateurs entrent `az ''`</span><span class="sxs-lookup"><span data-stu-id="de833-1972">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="de833-1973">Ajout de la prise en charge des types de ressources personnalisés pour les modules et les extensions de commande</span><span class="sxs-lookup"><span data-stu-id="de833-1973">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="de833-1974">ACR</span><span class="sxs-lookup"><span data-stu-id="de833-1974">ACR</span></span>

* <span data-ttu-id="de833-1975">Ajout de commandes de build de l’ACR</span><span class="sxs-lookup"><span data-stu-id="de833-1975">Added ACR Build commands</span></span>
* <span data-ttu-id="de833-1976">Améliorations des messages d’erreur dus aux ressources introuvables</span><span class="sxs-lookup"><span data-stu-id="de833-1976">Improved resource not found error messages</span></span>
* <span data-ttu-id="de833-1977">Amélioration des performances de création de ressources et de la gestion des erreurs</span><span class="sxs-lookup"><span data-stu-id="de833-1977">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="de833-1978">Amélioration de la connexion ACR dans des consoles non standards et des WSL</span><span class="sxs-lookup"><span data-stu-id="de833-1978">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="de833-1979">Amélioration des messages d’erreur dus aux commandes de dépôt</span><span class="sxs-lookup"><span data-stu-id="de833-1979">Improved repository commands error messages</span></span>
* <span data-ttu-id="de833-1980">Mise à jour des colonnes de la table et du classement</span><span class="sxs-lookup"><span data-stu-id="de833-1980">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="de833-1981">ACS</span><span class="sxs-lookup"><span data-stu-id="de833-1981">ACS</span></span>

* <span data-ttu-id="de833-1982">Ajout d’un avertissement indiquant que `az aks` est un service en préversion</span><span class="sxs-lookup"><span data-stu-id="de833-1982">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="de833-1983">Résolution du problème d’autorisation dans `aks install-connector` lorsque `--aci-resource-group` n’est pas spécifié</span><span class="sxs-lookup"><span data-stu-id="de833-1983">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="de833-1984">AMS</span><span class="sxs-lookup"><span data-stu-id="de833-1984">AMS</span></span>

* <span data-ttu-id="de833-1985">Version initiale - Gérer des ressources Azure Media Services</span><span class="sxs-lookup"><span data-stu-id="de833-1985">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="de833-1986">AppService</span><span class="sxs-lookup"><span data-stu-id="de833-1986">Appservice</span></span>

* <span data-ttu-id="de833-1987">Correction d’un bogue dans `webapp delete` lorsque `--slot` est fourni</span><span class="sxs-lookup"><span data-stu-id="de833-1987">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="de833-1988">`--runtime-version` retiré de `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="de833-1988">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="de833-1989">Ajout de la prise en charge de min\_tls\_version & https2.0</span><span class="sxs-lookup"><span data-stu-id="de833-1989">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="de833-1990">Ajout de la prise en charge pour les multiconteneurs</span><span class="sxs-lookup"><span data-stu-id="de833-1990">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="de833-1991">Batch AI</span><span class="sxs-lookup"><span data-stu-id="de833-1991">Batch AI</span></span>

* <span data-ttu-id="de833-1992">`batchai create cluster` modifié pour respecter la priorité de machine virtuelle configurée dans le fichier de configuration du cluster</span><span class="sxs-lookup"><span data-stu-id="de833-1992">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="de833-1993">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="de833-1993">Cognitive Services</span></span>

* <span data-ttu-id="de833-1994">Faute de frappe corrigée dans l’exemple de `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="de833-1994">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="de833-1995">Consommation</span><span class="sxs-lookup"><span data-stu-id="de833-1995">Consumption</span></span>

* <span data-ttu-id="de833-1996">Ajout de nouvelles commandes pour l’API Budget</span><span class="sxs-lookup"><span data-stu-id="de833-1996">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="de833-1997">Conteneur</span><span class="sxs-lookup"><span data-stu-id="de833-1997">Container</span></span>

* <span data-ttu-id="de833-1998">Suppression de l’exigence pour `--registry-server` pour `container create` lorsqu’un serveur de registre est inclus dans le nom de l’image</span><span class="sxs-lookup"><span data-stu-id="de833-1998">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="de833-1999">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="de833-1999">Cosmos DB</span></span>

* <span data-ttu-id="de833-2000">Présentation de la prise en charge d’un réseau virtuel pour Azure CLI - Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="de833-2000">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="de833-2001">DMS</span><span class="sxs-lookup"><span data-stu-id="de833-2001">DMS</span></span>

* <span data-ttu-id="de833-2002">Version initiale - Ajoute la prise en charge de l’instruction SQL pour le scénario de migration de SQL Azure</span><span class="sxs-lookup"><span data-stu-id="de833-2002">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="de833-2003">Extension</span><span class="sxs-lookup"><span data-stu-id="de833-2003">Extension</span></span>

* <span data-ttu-id="de833-2004">Correction d’un bogue où les métadonnées d’extension cessaient d’être affichées</span><span class="sxs-lookup"><span data-stu-id="de833-2004">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="de833-2005">Interactive</span><span class="sxs-lookup"><span data-stu-id="de833-2005">Interactive</span></span>

* <span data-ttu-id="de833-2006">Autorise le fonctionnement de compléments interactifs avec des arguments positionnel</span><span class="sxs-lookup"><span data-stu-id="de833-2006">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="de833-2007">Sortie plus conviviale lorsque les utilisateurs entrent \'</span><span class="sxs-lookup"><span data-stu-id="de833-2007">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="de833-2008">Achèvements corrigés pour les paramètres sans aide</span><span class="sxs-lookup"><span data-stu-id="de833-2008">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="de833-2009">Descriptions corrigées pour les groupes de commandes</span><span class="sxs-lookup"><span data-stu-id="de833-2009">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="de833-2010">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="de833-2010">Lab</span></span>

* <span data-ttu-id="de833-2011">Régressions corrigées de conversion Knack</span><span class="sxs-lookup"><span data-stu-id="de833-2011">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="de833-2012">Réseau</span><span class="sxs-lookup"><span data-stu-id="de833-2012">Network</span></span>

* <span data-ttu-id="de833-2013">[CHANGEMENT CASSANT] Suppression du paramètre `--ids` pour :</span><span class="sxs-lookup"><span data-stu-id="de833-2013">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="de833-2014">Profil</span><span class="sxs-lookup"><span data-stu-id="de833-2014">Profile</span></span>

* <span data-ttu-id="de833-2015">Correction de la détection de source `disk create`</span><span class="sxs-lookup"><span data-stu-id="de833-2015">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="de833-2016">[CHANGEMENT CASSANT] Suppression de `--msi-port` et `--identity-port` car ils ne sont plus utilisés</span><span class="sxs-lookup"><span data-stu-id="de833-2016">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="de833-2017">Correction d’une faute de frappe dans le bref résumé de `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="de833-2017">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="de833-2018">Redis</span><span class="sxs-lookup"><span data-stu-id="de833-2018">Redis</span></span>

* <span data-ttu-id="de833-2019">`redis patch-schedule patch-schedule show` déconseillé en faveur de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="de833-2019">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="de833-2020">`redis list-all` déconseillé.</span><span class="sxs-lookup"><span data-stu-id="de833-2020">Deprecated `redis list-all`.</span></span> <span data-ttu-id="de833-2021">Cette fonctionnalité a été pliée dans `redis list`</span><span class="sxs-lookup"><span data-stu-id="de833-2021">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="de833-2022">`redis import-method` déconseillé en faveur de `redis import`</span><span class="sxs-lookup"><span data-stu-id="de833-2022">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="de833-2023">Ajout de la prise en charge de `--ids` pour diverses commandes</span><span class="sxs-lookup"><span data-stu-id="de833-2023">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="de833-2024">Role</span><span class="sxs-lookup"><span data-stu-id="de833-2024">Role</span></span>

* <span data-ttu-id="de833-2025">[CHANGEMENT CASSANT] Suppression de `ad sp reset-credentials` déconseillé</span><span class="sxs-lookup"><span data-stu-id="de833-2025">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="de833-2026">Stockage</span><span class="sxs-lookup"><span data-stu-id="de833-2026">Storage</span></span>

* <span data-ttu-id="de833-2027">Autorise l’application du jeton SAS de destination pour une copie d’objets blob si le SAS source et la clé de compte ne sont pas spécifiés</span><span class="sxs-lookup"><span data-stu-id="de833-2027">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="de833-2028">Exposé--délai d’expiration de socket pour les chargements et téléchargements d’objets blob</span><span class="sxs-lookup"><span data-stu-id="de833-2028">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="de833-2029">Traite les noms d’objets blob commençant par des séparateurs de chemin d’accès comme des chemins d’accès relatifs</span><span class="sxs-lookup"><span data-stu-id="de833-2029">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="de833-2030">Autorise `storage blob copy --source-sas` avec le caractère de démarrage de requête, « ? »</span><span class="sxs-lookup"><span data-stu-id="de833-2030">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="de833-2031">`storage entity query --marker` corrigé pour accepter une liste de clé =valeurs</span><span class="sxs-lookup"><span data-stu-id="de833-2031">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="de833-2032">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="de833-2032">VM</span></span>

* <span data-ttu-id="de833-2033">Correction d’une logique de détection invalide sur l’URI de l’objet blob non gérée</span><span class="sxs-lookup"><span data-stu-id="de833-2033">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="de833-2034">Ajout de la prise en charge du chiffrement de disque sans principaux de service fournis par l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="de833-2034">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="de833-2035">[CHANGEMENT CASSANT] Ne pas utiliser « ManagedIdentityExtension » de machine virtuelle pour la prise en charge de MSI</span><span class="sxs-lookup"><span data-stu-id="de833-2035">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="de833-2036">Ajout de la prise en charge pour la stratégie d’éviction vers `vmss`</span><span class="sxs-lookup"><span data-stu-id="de833-2036">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="de833-2037">[CHANGEMENT CASSANT] Suppression de `--ids` de :</span><span class="sxs-lookup"><span data-stu-id="de833-2037">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="de833-2038">Ajout de la prise en charge des accélérateurs d’écriture</span><span class="sxs-lookup"><span data-stu-id="de833-2038">Added write accelerator support</span></span>
* <span data-ttu-id="de833-2039">Ajout de `vmss perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="de833-2039">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="de833-2040">Correction de `vm diagnostics set` pour détecter la fiabilité du type de système d’exploitation de la machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="de833-2040">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="de833-2041">Modification de `vm resize` pour vérifier si la taille demandée est différente de celle actuellement définie et pour mettre à jour uniquement en cas de modifications</span><span class="sxs-lookup"><span data-stu-id="de833-2041">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="de833-2042">10 avril 2018</span><span class="sxs-lookup"><span data-stu-id="de833-2042">April 10, 2018</span></span>

<span data-ttu-id="de833-2043">Version 2.0.31</span><span class="sxs-lookup"><span data-stu-id="de833-2043">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="de833-2044">ACR</span><span class="sxs-lookup"><span data-stu-id="de833-2044">ACR</span></span>

* <span data-ttu-id="de833-2045">Gestion améliorée des erreurs de secours wincred</span><span class="sxs-lookup"><span data-stu-id="de833-2045">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="de833-2046">ACS</span><span class="sxs-lookup"><span data-stu-id="de833-2046">ACS</span></span>

* <span data-ttu-id="de833-2047">Modification de la durée de validité des SPN créés par AKS à 5 ans</span><span class="sxs-lookup"><span data-stu-id="de833-2047">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="de833-2048">AppService</span><span class="sxs-lookup"><span data-stu-id="de833-2048">Appservice</span></span>

* [CHANGEMENT CASSANT]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="de833-2050">Correction d’une exception non interceptée pour les plans webapp inexistants</span><span class="sxs-lookup"><span data-stu-id="de833-2050">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="de833-2051">Batch AI</span><span class="sxs-lookup"><span data-stu-id="de833-2051">BatchAI</span></span>

* <span data-ttu-id="de833-2052">Ajout de la prise en charge de l’API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="de833-2052">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="de833-2053">Montage au niveau du travail</span><span class="sxs-lookup"><span data-stu-id="de833-2053">Job level mounting</span></span>
  - <span data-ttu-id="de833-2054">Variables d’environnement avec les valeurs des secrets</span><span class="sxs-lookup"><span data-stu-id="de833-2054">Environment variables with secret values</span></span>
  - <span data-ttu-id="de833-2055">Paramètres des compteurs de performances</span><span class="sxs-lookup"><span data-stu-id="de833-2055">Performance counters settings</span></span>
  - <span data-ttu-id="de833-2056">Création de rapports de segments de ligne spécifiques à un travail</span><span class="sxs-lookup"><span data-stu-id="de833-2056">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="de833-2057">Prise en charge des sous-dossiers dans les listes de fichiers de l’API</span><span class="sxs-lookup"><span data-stu-id="de833-2057">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="de833-2058">Création de rapports d’utilisation et de limites</span><span class="sxs-lookup"><span data-stu-id="de833-2058">Usage and limits reporting</span></span>
  - <span data-ttu-id="de833-2059">Autorisation de la spécification du type de mise en cache pour les serveurs NFS</span><span class="sxs-lookup"><span data-stu-id="de833-2059">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="de833-2060">Prise en charge des images personnalisées</span><span class="sxs-lookup"><span data-stu-id="de833-2060">Support for custom images</span></span>
  - <span data-ttu-id="de833-2061">Ajout de la prise en charge de la boîte à outils pyTorch</span><span class="sxs-lookup"><span data-stu-id="de833-2061">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="de833-2062">Ajout de la commande `job wait` qui permet d’attendre la fin du travail et d’obtenir le code de sortie du travail</span><span class="sxs-lookup"><span data-stu-id="de833-2062">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="de833-2063">Ajout de la commande `usage show` pour répertorier l’utilisation actuelle des ressources Batch AI et les limites pour les différentes régions</span><span class="sxs-lookup"><span data-stu-id="de833-2063">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="de833-2064">Prise en charge des clouds nationaux</span><span class="sxs-lookup"><span data-stu-id="de833-2064">National clouds are supported</span></span>
* <span data-ttu-id="de833-2065">Ajout d’arguments de ligne de commande de travail pour monter des systèmes de fichiers au niveau du travail en plus des fichiers de configuration</span><span class="sxs-lookup"><span data-stu-id="de833-2065">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="de833-2066">Ajout de plus d’options pour personnaliser les clusters : priorité des machines virtuelles, sous-réseau, nombre de nœuds initial pour les clusters avec mise à l’échelle automatique, spécification d’une image personnalisée</span><span class="sxs-lookup"><span data-stu-id="de833-2066">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="de833-2067">Ajout d’une option de ligne de commande pour spécifier le type de mise en cache pour les NFS gérés par Batch AI</span><span class="sxs-lookup"><span data-stu-id="de833-2067">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="de833-2068">Simplification de la spécification du montage du système de fichiers dans les fichiers config.</span><span class="sxs-lookup"><span data-stu-id="de833-2068">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="de833-2069">Il est désormais possible d’omettre les informations d’identification pour les partages de fichiers Azure et les conteneurs d’objets blob Azure : CLI remplira les informations d’identification manquantes à l’aide de la clé du compte de stockage fournie par le biais des paramètres de ligne de commande ou spécifiée via la variable d’environnement, ou interrogera la clé à partir du stockage Azure (si le compte de stockage appartient à l’abonnement actuel)</span><span class="sxs-lookup"><span data-stu-id="de833-2069">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="de833-2070">La commande de flux de fichiers de travail se remplit désormais automatiquement lorsque le travail est terminé (réussite, échec, terminé ou supprimé)</span><span class="sxs-lookup"><span data-stu-id="de833-2070">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="de833-2071">Amélioration de la sortie `table` pour les opérations `show`</span><span class="sxs-lookup"><span data-stu-id="de833-2071">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="de833-2072">Ajout de l’option `--use-auto-storage` pour la création du cluster.</span><span class="sxs-lookup"><span data-stu-id="de833-2072">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="de833-2073">Cette option simplifie la gestion des comptes de stockage et le montage de partages de fichiers Azure et de conteneurs d’objets blob Azure vers des clusters</span><span class="sxs-lookup"><span data-stu-id="de833-2073">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="de833-2074">Ajout de l’option `--generate-ssh-keys` à `cluster create` et `file-server create`</span><span class="sxs-lookup"><span data-stu-id="de833-2074">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="de833-2075">Ajout de la possibilité de fournir la tâche de configuration de nœud via la ligne de commande</span><span class="sxs-lookup"><span data-stu-id="de833-2075">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="de833-2076">[CHANGEMENT CASSANT] Déplacement des commandes `job stream-file` et `job list-files` sous le groupe `job file`</span><span class="sxs-lookup"><span data-stu-id="de833-2076">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="de833-2077">[CHANGEMENT CASSANT] Renommage de `--admin-user-name` en `--user-name` dans la commande `file-server create` pour être cohérent avec la commande `cluster create`</span><span class="sxs-lookup"><span data-stu-id="de833-2077">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="de833-2078">Facturation</span><span class="sxs-lookup"><span data-stu-id="de833-2078">Billing</span></span>

* <span data-ttu-id="de833-2079">Ajout de commandes d’inscription de compte</span><span class="sxs-lookup"><span data-stu-id="de833-2079">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="de833-2080">Consommation</span><span class="sxs-lookup"><span data-stu-id="de833-2080">Consumption</span></span>

* <span data-ttu-id="de833-2081">Ajout des commandes `marketplace`</span><span class="sxs-lookup"><span data-stu-id="de833-2081">Added `marketplace` commands</span></span>
* <span data-ttu-id="de833-2082">[CHANGEMENT CASSANT] Renommage de `reservations summaries` en `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="de833-2082">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="de833-2083">[CHANGEMENT CASSANT] Renommage de `reservations details` en `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="de833-2083">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="de833-2084">[CHANGEMENT CASSANT] Suppression des options abrégées de `--reservation-order-id` et `--reservation-id` pour les commandes `reservation`</span><span class="sxs-lookup"><span data-stu-id="de833-2084">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="de833-2085">[CHANGEMENT CASSANT] Suppression des options abrégées de `--grain` pour les commandes `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="de833-2085">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="de833-2086">[CHANGEMENT CASSANT] Suppression des options abrégées de `--include-meter-details` pour les commandes `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="de833-2086">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="de833-2087">Conteneur</span><span class="sxs-lookup"><span data-stu-id="de833-2087">Container</span></span>

* <span data-ttu-id="de833-2088">Ajout des paramètres de montage de volume de dépôt Git `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` et `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="de833-2088">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="de833-2089">Résolution de [#5926](https://github.com/Azure/azure-cli/issues/5926) : `az container exec` échoue lorsque le nom du conteneur -- est spécifié</span><span class="sxs-lookup"><span data-stu-id="de833-2089">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="de833-2090">Extension</span><span class="sxs-lookup"><span data-stu-id="de833-2090">Extension</span></span>

* <span data-ttu-id="de833-2091">Modification du message de vérification de distribution pour qu’il soit au niveau du débogage</span><span class="sxs-lookup"><span data-stu-id="de833-2091">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="de833-2092">Interactive</span><span class="sxs-lookup"><span data-stu-id="de833-2092">Interactive</span></span>

* <span data-ttu-id="de833-2093">Modification pour arrêter la saisie semi-automatique sur les commandes non reconnues</span><span class="sxs-lookup"><span data-stu-id="de833-2093">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="de833-2094">Ajout d’événements de raccordement avant et après la création du sous-arbre de commande</span><span class="sxs-lookup"><span data-stu-id="de833-2094">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="de833-2095">Ajout de la saisie semi-automatique pour les paramètres `--ids`</span><span class="sxs-lookup"><span data-stu-id="de833-2095">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="de833-2096">Réseau</span><span class="sxs-lookup"><span data-stu-id="de833-2096">Network</span></span>

* <span data-ttu-id="de833-2097">Résolution de [#5936](https://github.com/Azure/azure-cli/issues/5936) : les balises `application-gateway create` n’ont pas pu déterminer l’ensemble</span><span class="sxs-lookup"><span data-stu-id="de833-2097">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="de833-2098">Ajout de l’argument `--auth-certs` pour joindre des certificats d’authentification pour `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="de833-2098">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="de833-2099">#4910</span><span class="sxs-lookup"><span data-stu-id="de833-2099">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="de833-2100">Ajout de commandes `ddos-protection` pour créer des plans de protection DDoS</span><span class="sxs-lookup"><span data-stu-id="de833-2100">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="de833-2101">Prise en charge de `--ddos-protection-plan` pour `vnet [create|update]` pour associer un réseau virtuel à un plan de protection DDoS</span><span class="sxs-lookup"><span data-stu-id="de833-2101">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="de833-2102">Résolution du problème avec l’ indicateur `--disable-bgp-route-propagation` dans `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="de833-2102">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="de833-2103">Suppression des arguments factices `--public-ip-address-type` et `--subnet-type` pour `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="de833-2103">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="de833-2104">Ajout de la prise en charge des enregistrements TXT avec les séquences d’échappement RFC 1035 à `network dns zone [import|export]` et `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="de833-2104">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="de833-2105">Profil</span><span class="sxs-lookup"><span data-stu-id="de833-2105">Profile</span></span>

* <span data-ttu-id="de833-2106">Ajout de la prise en charge des comptes Azure Classic dans `account list`</span><span class="sxs-lookup"><span data-stu-id="de833-2106">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="de833-2107">[CHANGEMENT CASSANT] Suppression des arguments `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="de833-2107">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="de833-2108">SGBDR</span><span class="sxs-lookup"><span data-stu-id="de833-2108">RDBMS</span></span>

* <span data-ttu-id="de833-2109">Ajout de la commande `georestore`</span><span class="sxs-lookup"><span data-stu-id="de833-2109">Added `georestore` command</span></span>
* <span data-ttu-id="de833-2110">Suppression de la restriction de taille de stockage de la commande `create`</span><span class="sxs-lookup"><span data-stu-id="de833-2110">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="de833-2111">Ressource</span><span class="sxs-lookup"><span data-stu-id="de833-2111">Resource</span></span>

* <span data-ttu-id="de833-2112">Ajout de la prise en charge de `--metadata` pour `policy definition create`</span><span class="sxs-lookup"><span data-stu-id="de833-2112">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="de833-2113">Ajout de la prise en charge de `--metadata`, `--set`, `--add` et `--remove` à `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="de833-2113">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="de833-2114">SQL</span><span class="sxs-lookup"><span data-stu-id="de833-2114">SQL</span></span>

* <span data-ttu-id="de833-2115">Ajout de `sql elastic-pool op list` et `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="de833-2115">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="de833-2116">Stockage</span><span class="sxs-lookup"><span data-stu-id="de833-2116">Storage</span></span>

* <span data-ttu-id="de833-2117">Amélioration des messages d’erreur pour les chaînes de connexion incorrectes</span><span class="sxs-lookup"><span data-stu-id="de833-2117">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="de833-2118">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="de833-2118">VM</span></span>

* <span data-ttu-id="de833-2119">Ajout de la prise en charge pour configurer le nombre de domaines d’erreur de plateforme sur `vmss create`</span><span class="sxs-lookup"><span data-stu-id="de833-2119">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="de833-2120">Modification de `vmss create` sur la valeur par défaut de l’équilibreur de charge Standard pour les groupes identiques désactivés zonaux, grands ou avec un seul groupe de placement</span><span class="sxs-lookup"><span data-stu-id="de833-2120">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [CHANGEMENT CASSANT]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="de833-2122">Ajout de la prise en charge des références SKU d’IP public à `vm create`</span><span class="sxs-lookup"><span data-stu-id="de833-2122">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="de833-2123">Ajout des arguments `--keyvault` et `--resource-group` à `vm secret format` pour prendre en charge des scénarios où la commande ne parvient pas à résoudre l’ID de coffre.</span><span class="sxs-lookup"><span data-stu-id="de833-2123">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="de833-2124">#5718</span><span class="sxs-lookup"><span data-stu-id="de833-2124">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="de833-2125">Amélioration des erreurs pour `[vm|vmss create]` lorsque l’emplacement d’un groupe de ressources ne possède aucune prise en charge de zone</span><span class="sxs-lookup"><span data-stu-id="de833-2125">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="de833-2126">27 mars 2018</span><span class="sxs-lookup"><span data-stu-id="de833-2126">March 27, 2018</span></span>

<span data-ttu-id="de833-2127">Version 2.0.30</span><span class="sxs-lookup"><span data-stu-id="de833-2127">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="de833-2128">Core</span><span class="sxs-lookup"><span data-stu-id="de833-2128">Core</span></span>

* <span data-ttu-id="de833-2129">Afficher le message pour les extensions marquées en tant que préversions dans l’aide</span><span class="sxs-lookup"><span data-stu-id="de833-2129">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="de833-2130">ACS</span><span class="sxs-lookup"><span data-stu-id="de833-2130">ACS</span></span>

* <span data-ttu-id="de833-2131">Corriger l’erreur de vérification de certificat SSL pour `aks install-cli` dans Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="de833-2131">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="de833-2132">AppService</span><span class="sxs-lookup"><span data-stu-id="de833-2132">Appservice</span></span>

* <span data-ttu-id="de833-2133">Ajout de la prise en charge HTTPS exclusive à `webapp update`</span><span class="sxs-lookup"><span data-stu-id="de833-2133">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="de833-2134">Ajout de la prise en charge des emplacements à `az webapp identity [assign|show]` et `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="de833-2134">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="de833-2135">Backup</span><span class="sxs-lookup"><span data-stu-id="de833-2135">Backup</span></span>

* <span data-ttu-id="de833-2136">Ajout de la commande `az backup protection isenabled-for-vm`</span><span class="sxs-lookup"><span data-stu-id="de833-2136">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="de833-2137">Cette commande peut être utilisée pour vérifier si une machine virtuelle est sauvegardée par un coffre dans l’abonnement</span><span class="sxs-lookup"><span data-stu-id="de833-2137">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="de833-2138">Activation des ID d’objet Azure pour les paramètres `--resource-group` et `--vault-name`, pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="de833-2138">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="de833-2139">Modification des paramètres `--name` pour accepter le format de sortie des commandes `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="de833-2139">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="de833-2140">Conteneur</span><span class="sxs-lookup"><span data-stu-id="de833-2140">Container</span></span>

* <span data-ttu-id="de833-2141">Ajout de la commande `container exec`</span><span class="sxs-lookup"><span data-stu-id="de833-2141">Added `container exec` command.</span></span> <span data-ttu-id="de833-2142">Exécute les commandes dans un conteneur, pour un groupe de conteneurs en exécution.</span><span class="sxs-lookup"><span data-stu-id="de833-2142">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="de833-2143">Autoriser la sortie de table pour la création et la mise à jour d’un groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="de833-2143">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="de833-2144">Extension</span><span class="sxs-lookup"><span data-stu-id="de833-2144">Extension</span></span>

* <span data-ttu-id="de833-2145">Ajout d’un message pour `extension add` si l’extension est en préversion</span><span class="sxs-lookup"><span data-stu-id="de833-2145">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="de833-2146">Modification de `extension list-available` afin d’afficher les données complètes d’extension avec `--show-details`</span><span class="sxs-lookup"><span data-stu-id="de833-2146">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="de833-2147">[CHANGEMENT CASSANT] Modification de `extension list-available` afin d’afficher les données simplifiées d’extension par défaut</span><span class="sxs-lookup"><span data-stu-id="de833-2147">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="de833-2148">Interactive</span><span class="sxs-lookup"><span data-stu-id="de833-2148">Interactive</span></span>

* <span data-ttu-id="de833-2149">Modification des saisies semi-automatiques pour procéder à l’activation dès le chargement de la table de commande</span><span class="sxs-lookup"><span data-stu-id="de833-2149">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="de833-2150">Correction du bogue par l’exécution du paramètre `--style`</span><span class="sxs-lookup"><span data-stu-id="de833-2150">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="de833-2151">Analyseur lexical interactif instancié après le vidage de la table de commande, si manquant</span><span class="sxs-lookup"><span data-stu-id="de833-2151">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="de833-2152">Amélioration de la prise en charge de Completer</span><span class="sxs-lookup"><span data-stu-id="de833-2152">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="de833-2153">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="de833-2153">Lab</span></span>

* <span data-ttu-id="de833-2154">Correction des bogues avec la commande `create environment`</span><span class="sxs-lookup"><span data-stu-id="de833-2154">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="de833-2155">Moniteur</span><span class="sxs-lookup"><span data-stu-id="de833-2155">Monitor</span></span>

* <span data-ttu-id="de833-2156">Ajout de la prise en charge de `--top`, `--orderby` et `--namespace` à `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="de833-2156">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="de833-2157">Résolution de [#4529](https://github.com/Azure/azure-cli/issues/5785) : `metrics list` accepte une liste de mesures séparées par des espaces pour la récupération</span><span class="sxs-lookup"><span data-stu-id="de833-2157">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="de833-2158">Ajout de la prise en charge de `--namespace` à `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="de833-2158">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="de833-2159">Réseau</span><span class="sxs-lookup"><span data-stu-id="de833-2159">Network</span></span>

* <span data-ttu-id="de833-2160">Ajout de la prise en charge des zones de DNS privé</span><span class="sxs-lookup"><span data-stu-id="de833-2160">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="de833-2161">Profil</span><span class="sxs-lookup"><span data-stu-id="de833-2161">Profile</span></span>

* <span data-ttu-id="de833-2162">Ajout d’un avertissement pour `--identity-port` et `--msi-port` à `login`</span><span class="sxs-lookup"><span data-stu-id="de833-2162">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="de833-2163">SGBDR</span><span class="sxs-lookup"><span data-stu-id="de833-2163">RDBMS</span></span>

* <span data-ttu-id="de833-2164">Ajout de la version d’API mise à la disposition générale du modèle d’entreprise 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="de833-2164">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="de833-2165">Ressource</span><span class="sxs-lookup"><span data-stu-id="de833-2165">Resource</span></span>

* [CHANGEMENT CASSANT]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="de833-2167">Role</span><span class="sxs-lookup"><span data-stu-id="de833-2167">Role</span></span>

* <span data-ttu-id="de833-2168">Ajout de la prise en charge des configurations d’accès et des clients natifs requis à `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="de833-2168">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="de833-2169">Modification des commandes `rbac` afin de renvoyer moins de 1 000 ID sur la résolution d’objet</span><span class="sxs-lookup"><span data-stu-id="de833-2169">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="de833-2170">Ajout des commandes de gestion des informations d’identification `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="de833-2170">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="de833-2171">[CHANGEMENT CASSANT] Suppression des propriétés de la sortie `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="de833-2171">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="de833-2172">Ajout de la prise en charge des autorisations `dataActions` et `notDataActions` à `role definition`</span><span class="sxs-lookup"><span data-stu-id="de833-2172">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="de833-2173">Stockage</span><span class="sxs-lookup"><span data-stu-id="de833-2173">Storage</span></span>

* <span data-ttu-id="de833-2174">Résolution du problème lié au chargement des fichiers présentant une taille comprise entre 195 Go et 200 Go</span><span class="sxs-lookup"><span data-stu-id="de833-2174">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="de833-2175">Résolution de [#4049](https://github.com/Azure/azure-cli/issues/4049) : problèmes avec les chargements d’objets blob d’ajout ignorant les paramètres de condition</span><span class="sxs-lookup"><span data-stu-id="de833-2175">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="de833-2176">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="de833-2176">VM</span></span>

* <span data-ttu-id="de833-2177">Ajout d’un avertissement à `vmss create` concernant les changements cassants à venir pour les ensembles comprenant plus de 100 instances</span><span class="sxs-lookup"><span data-stu-id="de833-2177">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="de833-2178">Ajout de la prise en charge de la résilience dans la zone à `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="de833-2178">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="de833-2179">Modification de la vue d’instance de disque pour signaler un meilleur état de chiffrement</span><span class="sxs-lookup"><span data-stu-id="de833-2179">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="de833-2180">[CHANGEMENT CASSANT] Modification de `vm extension delete` afin d’annuler la capacité de génération de sortie</span><span class="sxs-lookup"><span data-stu-id="de833-2180">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="de833-2181">13 mars 2018</span><span class="sxs-lookup"><span data-stu-id="de833-2181">March 13, 2018</span></span>

<span data-ttu-id="de833-2182">Version 2.0.29</span><span class="sxs-lookup"><span data-stu-id="de833-2182">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="de833-2183">ACR</span><span class="sxs-lookup"><span data-stu-id="de833-2183">ACR</span></span>

* <span data-ttu-id="de833-2184">Ajout de la prise en charge du paramètre `--image` pour `repository delete`</span><span class="sxs-lookup"><span data-stu-id="de833-2184">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="de833-2185">Paramètres `--manifest` et `--tag` de la commande `repository delete` déconseillés</span><span class="sxs-lookup"><span data-stu-id="de833-2185">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="de833-2186">Ajout de la commande `repository untag` pour supprimer une balise sans supprimer les données</span><span class="sxs-lookup"><span data-stu-id="de833-2186">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="de833-2187">ACS</span><span class="sxs-lookup"><span data-stu-id="de833-2187">ACS</span></span>

* <span data-ttu-id="de833-2188">Ajout de la commande `aks upgrade-connector` pour mettre à niveau un connecteur existant</span><span class="sxs-lookup"><span data-stu-id="de833-2188">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="de833-2189">Modification des fichiers de configuration `kubectl` pour utiliser un YAML de style bloc plus lisible</span><span class="sxs-lookup"><span data-stu-id="de833-2189">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="de833-2190">Advisor</span><span class="sxs-lookup"><span data-stu-id="de833-2190">Advisor</span></span>

* <span data-ttu-id="de833-2191">[CHANGEMENT CASSANT] Renommage de `advisor configuration get` en `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="de833-2191">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="de833-2192">[CHANGEMENT CASSANT] Renommage de `advisor configuration set` en `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="de833-2192">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="de833-2193">[CHANGEMENT CASSANT] Suppression de `advisor recommendation generate`</span><span class="sxs-lookup"><span data-stu-id="de833-2193">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="de833-2194">Ajout du paramètre `--refresh` pour `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="de833-2194">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="de833-2195">Ajout de la commande `advisor recommendation show`</span><span class="sxs-lookup"><span data-stu-id="de833-2195">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="de833-2196">AppService</span><span class="sxs-lookup"><span data-stu-id="de833-2196">Appservice</span></span>

* <span data-ttu-id="de833-2197">`[webapp|functionapp] assign-identity` déconseillé</span><span class="sxs-lookup"><span data-stu-id="de833-2197">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="de833-2198">Ajout des commandes d’identité gérée `webapp identity [assign|show]` et `functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="de833-2198">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="de833-2199">Eventhubs</span><span class="sxs-lookup"><span data-stu-id="de833-2199">Eventhubs</span></span>

* <span data-ttu-id="de833-2200">Version initiale</span><span class="sxs-lookup"><span data-stu-id="de833-2200">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="de833-2201">Extension</span><span class="sxs-lookup"><span data-stu-id="de833-2201">Extension</span></span>

* <span data-ttu-id="de833-2202">Ajout d’un contrôle supplémentaire pour avertir l’utilisateur si le distributeur utilisé est différent de celui stocké dans le fichier source du package, car cela peut entraîner des erreurs</span><span class="sxs-lookup"><span data-stu-id="de833-2202">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="de833-2203">Interactive</span><span class="sxs-lookup"><span data-stu-id="de833-2203">Interactive</span></span>

* <span data-ttu-id="de833-2204">Résolution de [#5625](https://github.com/Azure/azure-cli/issues/5625) : conservation de l’historique entre différentes sessions</span><span class="sxs-lookup"><span data-stu-id="de833-2204">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="de833-2205">Résolution de [#3016](https://github.com/Azure/azure-cli/issues/3016) : historique non enregistré alors qu’il était dans la portée</span><span class="sxs-lookup"><span data-stu-id="de833-2205">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="de833-2206">Résolution de [#5688](https://github.com/Azure/azure-cli/issues/5688) : la saisie automatique n’apparaît pas si le chargement de la table de commande a rencontré une exception</span><span class="sxs-lookup"><span data-stu-id="de833-2206">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="de833-2207">Résolu : indicateur de progression pour les opérations à long terme</span><span class="sxs-lookup"><span data-stu-id="de833-2207">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="de833-2208">Moniteur</span><span class="sxs-lookup"><span data-stu-id="de833-2208">Monitor</span></span>

* <span data-ttu-id="de833-2209">Les commandes `monitor autoscale-settings` ont été déconseillées</span><span class="sxs-lookup"><span data-stu-id="de833-2209">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="de833-2210">Ajout des commandes `monitor autoscale`</span><span class="sxs-lookup"><span data-stu-id="de833-2210">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="de833-2211">Ajout des commandes `monitor autoscale profile`</span><span class="sxs-lookup"><span data-stu-id="de833-2211">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="de833-2212">Ajout des commandes `monitor autoscale rule`</span><span class="sxs-lookup"><span data-stu-id="de833-2212">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="de833-2213">Réseau</span><span class="sxs-lookup"><span data-stu-id="de833-2213">Network</span></span>

* <span data-ttu-id="de833-2214">[CHANGEMENT CASSANT] Suppression du paramètre `--tags` de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="de833-2214">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="de833-2215">Suppression de certaines valeurs par défaut erronées pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="de833-2215">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="de833-2216">Ajout des commandes `network watcher connection-monitor`</span><span class="sxs-lookup"><span data-stu-id="de833-2216">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="de833-2217">Ajout des paramètres `--vnet` et `--subnet` à `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="de833-2217">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="de833-2218">Profil</span><span class="sxs-lookup"><span data-stu-id="de833-2218">Profile</span></span>

* <span data-ttu-id="de833-2219">Paramètre `--msi` déconseillé pour `az login`</span><span class="sxs-lookup"><span data-stu-id="de833-2219">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="de833-2220">Ajout du paramètre `--identity` pour `az login` afin de remplacer `--msi`</span><span class="sxs-lookup"><span data-stu-id="de833-2220">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="de833-2221">SGBDR</span><span class="sxs-lookup"><span data-stu-id="de833-2221">RDBMS</span></span>

* <span data-ttu-id="de833-2222">[PRÉVERSION] Modifiée pour utiliser l’API 2017-12-01-préversion</span><span class="sxs-lookup"><span data-stu-id="de833-2222">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="de833-2223">Service Bus</span><span class="sxs-lookup"><span data-stu-id="de833-2223">Service Bus</span></span>

* <span data-ttu-id="de833-2224">Version initiale</span><span class="sxs-lookup"><span data-stu-id="de833-2224">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="de833-2225">Stockage</span><span class="sxs-lookup"><span data-stu-id="de833-2225">Storage</span></span>

* <span data-ttu-id="de833-2226">Résolution de [#4971](https://github.com/Azure/azure-cli/issues/4971) : `storage blob copy` prend désormais en charge les autres clouds Azure</span><span class="sxs-lookup"><span data-stu-id="de833-2226">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="de833-2227">Résolution de [#5286](https://github.com/Azure/azure-cli/issues/5286) : les commandes batch `storage blob [delete-batch|download-batch|upload-batch]` ne génèrent plus d’erreur lors d’échecs de la condition préalable</span><span class="sxs-lookup"><span data-stu-id="de833-2227">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="de833-2228">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="de833-2228">VM</span></span>

* <span data-ttu-id="de833-2229">Ajout de prise en charge de `[vm|vmss] create` pour attacher des disques de données non gérées et configurer la mise en cache</span><span class="sxs-lookup"><span data-stu-id="de833-2229">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="de833-2230">`[vm|vmss] assign-identity` et `[vm|vmss] remove-identity` sont déconseillés</span><span class="sxs-lookup"><span data-stu-id="de833-2230">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="de833-2231">Ajout des commandes `vm identity [assign|remove|show]` et `vmss identity [assign|remove|show]` pour remplacer des commandes déconseillées</span><span class="sxs-lookup"><span data-stu-id="de833-2231">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="de833-2232">Modification de la priorité par défaut dans `vmss create` à None</span><span class="sxs-lookup"><span data-stu-id="de833-2232">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="de833-2233">27 février 2018</span><span class="sxs-lookup"><span data-stu-id="de833-2233">February 27, 2018</span></span>

<span data-ttu-id="de833-2234">Version 2.0.28</span><span class="sxs-lookup"><span data-stu-id="de833-2234">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="de833-2235">Core</span><span class="sxs-lookup"><span data-stu-id="de833-2235">Core</span></span>

* <span data-ttu-id="de833-2236">Résolution de [#5184](https://github.com/Azure/azure-cli/issues/5184) : problème d’installation d’Homebrew</span><span class="sxs-lookup"><span data-stu-id="de833-2236">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="de833-2237">Ajout de la prise en charge de télémétrie d’extension avec des clés personnalisées</span><span class="sxs-lookup"><span data-stu-id="de833-2237">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="de833-2238">Ajout de la connexion HTTP à `--debug`</span><span class="sxs-lookup"><span data-stu-id="de833-2238">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="de833-2239">ACS</span><span class="sxs-lookup"><span data-stu-id="de833-2239">ACS</span></span>

* <span data-ttu-id="de833-2240">Modification pour utiliser le graphique Helm `virtual-kubelet-for-aks` pour `aks install-connector` par défaut</span><span class="sxs-lookup"><span data-stu-id="de833-2240">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="de833-2241">Résolution de #7161 : autorisation insuffisante des principaux de service pour la création de groupe de conteneurs ACI</span><span class="sxs-lookup"><span data-stu-id="de833-2241">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="de833-2242">Ajout des paramètres `--aci-container-group`, `--location` et `--image-tag` à `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="de833-2242">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="de833-2243">Suppression de l’avis de désapprobation de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="de833-2243">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="de833-2244">AppService</span><span class="sxs-lookup"><span data-stu-id="de833-2244">Appservice</span></span>

* <span data-ttu-id="de833-2245">Mises à jour pour la nouvelle version du kit de développement logiciel (SDK) (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="de833-2245">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="de833-2246">Résolu [#5538](https://github.com/Azure/azure-cli/issues/5538) : `Free` défini comme une SKU invalide</span><span class="sxs-lookup"><span data-stu-id="de833-2246">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="de833-2247">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="de833-2247">Cognitive Services</span></span>

* <span data-ttu-id="de833-2248">Mise à jour de l’avis lors de la création d’un compte Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="de833-2248">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="de833-2249">Consommation</span><span class="sxs-lookup"><span data-stu-id="de833-2249">Consumption</span></span>

* <span data-ttu-id="de833-2250">Ajout de nouvelles commandes pour l’API priceSheet</span><span class="sxs-lookup"><span data-stu-id="de833-2250">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="de833-2251">Mise à jour des formats existants Détails d’utilisations et Détails de la réservation</span><span class="sxs-lookup"><span data-stu-id="de833-2251">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="de833-2252">Conteneur</span><span class="sxs-lookup"><span data-stu-id="de833-2252">Container</span></span>

* <span data-ttu-id="de833-2253">Ajout des arguments `--secrets` et `--secrets-mount-path` à `container create` pour utiliser des secrets dans ACI</span><span class="sxs-lookup"><span data-stu-id="de833-2253">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="de833-2254">Réseau</span><span class="sxs-lookup"><span data-stu-id="de833-2254">Network</span></span>

* <span data-ttu-id="de833-2255">Résolution de [#5559](https://github.com/Azure/azure-cli/issues/5559) : client manquant dans `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="de833-2255">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="de833-2256">Ressource</span><span class="sxs-lookup"><span data-stu-id="de833-2256">Resource</span></span>

* <span data-ttu-id="de833-2257">Modification de `group deployment export` pour afficher un modèle et des erreurs partiels sur échec</span><span class="sxs-lookup"><span data-stu-id="de833-2257">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="de833-2258">Role</span><span class="sxs-lookup"><span data-stu-id="de833-2258">Role</span></span>

* <span data-ttu-id="de833-2259">Ajout de `role assignment list-changelogs` pour permettre l’audit des rôles du principal de service</span><span class="sxs-lookup"><span data-stu-id="de833-2259">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="de833-2260">SQL</span><span class="sxs-lookup"><span data-stu-id="de833-2260">SQL</span></span>

* <span data-ttu-id="de833-2261">Ajout de la prise en charge de la redondance de zone pour les bases de données et les pools élastiques lors de création et mise à jour</span><span class="sxs-lookup"><span data-stu-id="de833-2261">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="de833-2262">Stockage</span><span class="sxs-lookup"><span data-stu-id="de833-2262">Storage</span></span>

* <span data-ttu-id="de833-2263">Activation de la spécification de préfixe/destination pour `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="de833-2263">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="de833-2264">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="de833-2264">VM</span></span>

* <span data-ttu-id="de833-2265">Ajout de prise en charge de jonction / séparation de disques sur une instance de groupe de machines virtuelles identiques uniques</span><span class="sxs-lookup"><span data-stu-id="de833-2265">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="de833-2266">13 février 2018</span><span class="sxs-lookup"><span data-stu-id="de833-2266">February 13, 2018</span></span>

<span data-ttu-id="de833-2267">Version 2.0.27</span><span class="sxs-lookup"><span data-stu-id="de833-2267">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="de833-2268">Core</span><span class="sxs-lookup"><span data-stu-id="de833-2268">Core</span></span>

* <span data-ttu-id="de833-2269">Modification de l’authentification pour passer au système de clé sur l’ID d’abonnement et le nom sur la connexion MSI</span><span class="sxs-lookup"><span data-stu-id="de833-2269">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="de833-2270">ACS</span><span class="sxs-lookup"><span data-stu-id="de833-2270">ACS</span></span>

* <span data-ttu-id="de833-2271">[CHANGEMENT CASSANT] Renommage de `aks get-versions` en `aks get-upgrades` pour des raisons de précision</span><span class="sxs-lookup"><span data-stu-id="de833-2271">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="de833-2272">Modification de `aks get-versions` pour afficher les versions Kubernetes disponibles pour `aks create`</span><span class="sxs-lookup"><span data-stu-id="de833-2272">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="de833-2273">Modification des valeurs par défaut de `aks create` de manière à laisser le serveur choisir la version de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="de833-2273">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="de833-2274">Mise à jour des messages d’aide faisant référence au principal du service généré par AKS</span><span class="sxs-lookup"><span data-stu-id="de833-2274">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="de833-2275">Modification des tailles de nœud par défaut pour `aks create` pour passer de « Standard\_D1\_v2 » à « Standard\_DS1\_v2 »</span><span class="sxs-lookup"><span data-stu-id="de833-2275">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="de833-2276">Meilleure fiabilité lors de la localisation du pod de tableau de bord pour `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="de833-2276">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="de833-2277">Correction de `aks get-credentials` pour gérer les erreurs Unicode lors du chargement des fichiers de configuration Kubernetes</span><span class="sxs-lookup"><span data-stu-id="de833-2277">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="de833-2278">Ajout d’un message à `az aks install-cli` pour aider à l’obtention de `kubectl` dans `$PATH`</span><span class="sxs-lookup"><span data-stu-id="de833-2278">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="de833-2279">AppService</span><span class="sxs-lookup"><span data-stu-id="de833-2279">Appservice</span></span>

* <span data-ttu-id="de833-2280">Résolution du problème dans lequel `webapp [backup|restore]` a échoué en raison d’une référence null</span><span class="sxs-lookup"><span data-stu-id="de833-2280">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="de833-2281">Ajout de la prise en charge supplémentaire des plans App Service par défaut via `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="de833-2281">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="de833-2282">CDN</span><span class="sxs-lookup"><span data-stu-id="de833-2282">CDN</span></span>

* <span data-ttu-id="de833-2283">Ajout des commandes `cdn custom-domain [enable-https|disable-https]`</span><span class="sxs-lookup"><span data-stu-id="de833-2283">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="de833-2284">Conteneur</span><span class="sxs-lookup"><span data-stu-id="de833-2284">Container</span></span>

* <span data-ttu-id="de833-2285">Ajout de l’option `--follow` à `az container logs` pour les journaux d’activité de diffusion en continu</span><span class="sxs-lookup"><span data-stu-id="de833-2285">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="de833-2286">Ajout de la commande `container attach` qui associe les flux d’erreur et de sortie standard locaux à un conteneur d’un groupe de conteneur</span><span class="sxs-lookup"><span data-stu-id="de833-2286">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="de833-2287">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="de833-2287">CosmosDB</span></span>

* <span data-ttu-id="de833-2288">Ajout de la prise en charge de la définition de fonctionnalités</span><span class="sxs-lookup"><span data-stu-id="de833-2288">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="de833-2289">Extension</span><span class="sxs-lookup"><span data-stu-id="de833-2289">Extension</span></span>

* <span data-ttu-id="de833-2290">Ajout de la prise en charge du paramètre `--pip-proxy` pour les commandes `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="de833-2290">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="de833-2291">Ajout de la prise en charge de l’argument `--pip-extra-index-urls` pour les commandes `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="de833-2291">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="de833-2292">Commentaires</span><span class="sxs-lookup"><span data-stu-id="de833-2292">Feedback</span></span>

* <span data-ttu-id="de833-2293">Ajout d’informations d’extension aux données de télémétrie</span><span class="sxs-lookup"><span data-stu-id="de833-2293">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="de833-2294">Interactive</span><span class="sxs-lookup"><span data-stu-id="de833-2294">Interactive</span></span>

* <span data-ttu-id="de833-2295">Résolution du problème dans lequel l’utilisateur est invité à se connecter à l’aide du mode interactif dans Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="de833-2295">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="de833-2296">Correction de la régression avec les listes de saisie semi-automatique des paramètres manquants</span><span class="sxs-lookup"><span data-stu-id="de833-2296">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="de833-2297">IoT</span><span class="sxs-lookup"><span data-stu-id="de833-2297">IoT</span></span>

* <span data-ttu-id="de833-2298">Résolution du problème dans lequel `iot dps access policy [create|update]` renvoie une erreur « introuvable » en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="de833-2298">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="de833-2299">Résolution du problème dans lequel `iot dps linked-hub [create|update]` renvoie une erreur « introuvable » en cas de réussite</span><span class="sxs-lookup"><span data-stu-id="de833-2299">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="de833-2300">Ajout de la prise en charge de `--no-wait` pour `iot dps access policy [create|update]` et `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="de833-2300">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="de833-2301">Modification de `iot hub create` pour autoriser la spécification du nombre de partitions</span><span class="sxs-lookup"><span data-stu-id="de833-2301">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="de833-2302">Moniteur</span><span class="sxs-lookup"><span data-stu-id="de833-2302">Monitor</span></span>

* <span data-ttu-id="de833-2303">Correction de la commande `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="de833-2303">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="de833-2304">Réseau</span><span class="sxs-lookup"><span data-stu-id="de833-2304">Network</span></span>

* <span data-ttu-id="de833-2305">Correction de l’option `--tags` pour les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="de833-2305">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="de833-2306">Profil</span><span class="sxs-lookup"><span data-stu-id="de833-2306">Profile</span></span>

* <span data-ttu-id="de833-2307">Activation `az login` à partir du mode interactif</span><span class="sxs-lookup"><span data-stu-id="de833-2307">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="de833-2308">Ressource</span><span class="sxs-lookup"><span data-stu-id="de833-2308">Resource</span></span>

* <span data-ttu-id="de833-2309">Rajout de `feature show`</span><span class="sxs-lookup"><span data-stu-id="de833-2309">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="de833-2310">Role</span><span class="sxs-lookup"><span data-stu-id="de833-2310">Role</span></span>

* <span data-ttu-id="de833-2311">Ajout de l’argument `--available-to-other-tenants` à `ad app update`</span><span class="sxs-lookup"><span data-stu-id="de833-2311">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="de833-2312">SQL</span><span class="sxs-lookup"><span data-stu-id="de833-2312">SQL</span></span>

* <span data-ttu-id="de833-2313">Ajout des commandes `sql server dns-alias`</span><span class="sxs-lookup"><span data-stu-id="de833-2313">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="de833-2314">Ajout de `sql db rename`</span><span class="sxs-lookup"><span data-stu-id="de833-2314">Added `sql db rename`</span></span>
* <span data-ttu-id="de833-2315">Ajout de la prise en charge de l’argument `--ids` pour toutes les commandes sql</span><span class="sxs-lookup"><span data-stu-id="de833-2315">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="de833-2316">Stockage</span><span class="sxs-lookup"><span data-stu-id="de833-2316">Storage</span></span>

* <span data-ttu-id="de833-2317">Ajout des commandes `storage blob service-properties delete-policy` et `storage blob undelete` pour permettre une suppression réversible</span><span class="sxs-lookup"><span data-stu-id="de833-2317">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="de833-2318">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="de833-2318">VM</span></span>

* <span data-ttu-id="de833-2319">Correction d’un incident lorsque le chiffrement de la machine virtuelle ne peut pas être initialisé entièrement</span><span class="sxs-lookup"><span data-stu-id="de833-2319">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="de833-2320">Ajout de la sortie d’ID du principal lors de l’activation de MSI</span><span class="sxs-lookup"><span data-stu-id="de833-2320">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="de833-2321">`vm boot-diagnostics get-boot-log` fixe</span><span class="sxs-lookup"><span data-stu-id="de833-2321">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="de833-2322">31 janvier 2018</span><span class="sxs-lookup"><span data-stu-id="de833-2322">January 31, 2018</span></span>

<span data-ttu-id="de833-2323">Version 2.0.26</span><span class="sxs-lookup"><span data-stu-id="de833-2323">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="de833-2324">Core</span><span class="sxs-lookup"><span data-stu-id="de833-2324">Core</span></span>

* <span data-ttu-id="de833-2325">Ajout de la prise en charge de la récupération du jeton brut dans le contexte MSI</span><span class="sxs-lookup"><span data-stu-id="de833-2325">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="de833-2326">Suppression de la chaîne de l’indicateur d’interrogation après la fin de LRO sur le fichier cmd.exe de Windows</span><span class="sxs-lookup"><span data-stu-id="de833-2326">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="de833-2327">Ajout d’un avertissement qui s’affiche lorsque l’utilisation d’une valeur par défaut configurée a été remplacée par une entrée de niveau INFO.</span><span class="sxs-lookup"><span data-stu-id="de833-2327">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="de833-2328">Utilisation de `--verbose` pour voir</span><span class="sxs-lookup"><span data-stu-id="de833-2328">Use `--verbose` to see</span></span>
* <span data-ttu-id="de833-2329">Ajouter un indicateur de progression pour les commandes wait</span><span class="sxs-lookup"><span data-stu-id="de833-2329">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="de833-2330">ACS</span><span class="sxs-lookup"><span data-stu-id="de833-2330">ACS</span></span>

* <span data-ttu-id="de833-2331">Clarification de l’argument `--disable-browser`</span><span class="sxs-lookup"><span data-stu-id="de833-2331">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="de833-2332">Amélioration de la touche TAB pour les arguments `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="de833-2332">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="de833-2333">AppService</span><span class="sxs-lookup"><span data-stu-id="de833-2333">Appservice</span></span>

* <span data-ttu-id="de833-2334">`webapp log [tail|download]` fixe</span><span class="sxs-lookup"><span data-stu-id="de833-2334">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="de833-2335">Suppression de la vérification de `kind` sur les fonctions et les applications web</span><span class="sxs-lookup"><span data-stu-id="de833-2335">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="de833-2336">CDN</span><span class="sxs-lookup"><span data-stu-id="de833-2336">CDN</span></span>

* <span data-ttu-id="de833-2337">Résolution du problème de client manquant avec `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="de833-2337">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="de833-2338">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="de833-2338">CosmosDB</span></span>

* <span data-ttu-id="de833-2339">Correction de la description du paramètre pour les stratégies de basculement</span><span class="sxs-lookup"><span data-stu-id="de833-2339">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="de833-2340">Interactive</span><span class="sxs-lookup"><span data-stu-id="de833-2340">Interactive</span></span>

* <span data-ttu-id="de833-2341">Résolution du problème dans lequel les listes de saisie semi-automatique d’option de commande ne s’affichent plus</span><span class="sxs-lookup"><span data-stu-id="de833-2341">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="de833-2342">Réseau</span><span class="sxs-lookup"><span data-stu-id="de833-2342">Network</span></span>

* <span data-ttu-id="de833-2343">Ajout de la protection pour `--cert-password` à `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="de833-2343">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="de833-2344">Résolution du problème lié à `application-gateway update` où `--sku` a appliqué par erreur une valeur par défaut</span><span class="sxs-lookup"><span data-stu-id="de833-2344">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="de833-2345">Ajout de la protection pour `--shared-key` et `--authorization-key` à `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="de833-2345">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="de833-2346">Résolution du problème de client manquant avec `asg create`</span><span class="sxs-lookup"><span data-stu-id="de833-2346">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="de833-2347">Ajout du paramètre `--file-name / -f` pour les noms exportés à `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="de833-2347">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="de833-2348">Les problèmes suivants liés à `dns zone export` ont été résolus :</span><span class="sxs-lookup"><span data-stu-id="de833-2348">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="de833-2349">Résolution du problème dans lequel des enregistrements TXT longs ont été mal exportés</span><span class="sxs-lookup"><span data-stu-id="de833-2349">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="de833-2350">Résolution du problème dans lequel des enregistrements TXT entre guillemets ont été mal exportés sans guillemets placés dans une séquence d’échappement.</span><span class="sxs-lookup"><span data-stu-id="de833-2350">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="de833-2351">Résolution du problème où certains enregistrements ont été importés à deux reprises avec `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="de833-2351">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="de833-2352">Restauration des commandes `vnet-gateway root-cert` et `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="de833-2352">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="de833-2353">Profil</span><span class="sxs-lookup"><span data-stu-id="de833-2353">Profile</span></span>

* <span data-ttu-id="de833-2354">Correction de `get-access-token` pour qu’il fonctionne à l’intérieur d’une machine virtuelle avec l’identité</span><span class="sxs-lookup"><span data-stu-id="de833-2354">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="de833-2355">Ressource</span><span class="sxs-lookup"><span data-stu-id="de833-2355">Resource</span></span>

* <span data-ttu-id="de833-2356">Correction du bogue lié à `deployment [create|validate]` où un avertissement ne s’est pas affiché correctement quand un champ ’type’ du modèle contient des valeurs en majuscules</span><span class="sxs-lookup"><span data-stu-id="de833-2356">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="de833-2357">Stockage</span><span class="sxs-lookup"><span data-stu-id="de833-2357">Storage</span></span>

* <span data-ttu-id="de833-2358">Résolution du problème lié à la migration des comptes Storage V1 vers Storage V2</span><span class="sxs-lookup"><span data-stu-id="de833-2358">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="de833-2359">Ajout de la création progressive de rapports pour toutes les commandes de chargement/téléchargement</span><span class="sxs-lookup"><span data-stu-id="de833-2359">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="de833-2360">Résolution du bogue empêchant l’option d’argument « -n » avec `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="de833-2360">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="de833-2361">Ajout de la colonne de « snapshot » ajouté à la sortie de table pour `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="de833-2361">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="de833-2362">Résolution des bogues dans lesquels différents paramètres devaient être analysés en tant qu’entiers</span><span class="sxs-lookup"><span data-stu-id="de833-2362">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="de833-2363">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="de833-2363">VM</span></span>

* <span data-ttu-id="de833-2364">Ajout de la commande `vm image accept-terms` pour autoriser la création de machines virtuelles à partir d’images moyennant des frais supplémentaires</span><span class="sxs-lookup"><span data-stu-id="de833-2364">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="de833-2365">Correction de `[vm|vmss create]` pour garantir l’exécution des commandes sous un proxy avec des certificats non signés</span><span class="sxs-lookup"><span data-stu-id="de833-2365">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="de833-2366">[APERÇU] Ajout de la prise en charge de la priorité « faible» au groupe de machines virtuelles identiques</span><span class="sxs-lookup"><span data-stu-id="de833-2366">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="de833-2367">Ajout de la protection pour `--admin-password` à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="de833-2367">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="de833-2368">17 janvier 2018</span><span class="sxs-lookup"><span data-stu-id="de833-2368">January 17, 2018</span></span>

<span data-ttu-id="de833-2369">Version 2.0.25</span><span class="sxs-lookup"><span data-stu-id="de833-2369">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="de833-2370">ACR</span><span class="sxs-lookup"><span data-stu-id="de833-2370">ACR</span></span>

* <span data-ttu-id="de833-2371">Ajout d’une connexion acr de secours en cas d’erreurs d’informations d’identification Windows</span><span class="sxs-lookup"><span data-stu-id="de833-2371">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="de833-2372">Activation des journaux d’activité du Registre</span><span class="sxs-lookup"><span data-stu-id="de833-2372">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="de833-2373">ACS</span><span class="sxs-lookup"><span data-stu-id="de833-2373">ACS</span></span>

* <span data-ttu-id="de833-2374">Correction de la commande `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="de833-2374">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="de833-2375">Suppression de l’exigence de rôle SPN</span><span class="sxs-lookup"><span data-stu-id="de833-2375">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="de833-2376">AppService</span><span class="sxs-lookup"><span data-stu-id="de833-2376">Appservice</span></span>

* <span data-ttu-id="de833-2377">Correction du bogue avec `config ssl upload` où `hosting_environment_profile` avait la valeur null</span><span class="sxs-lookup"><span data-stu-id="de833-2377">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="de833-2378">Ajout de la prise en charge des URL personnalisées pour `browse`</span><span class="sxs-lookup"><span data-stu-id="de833-2378">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="de833-2379">Prise en charge de l’emplacement fixe pour `log tail`</span><span class="sxs-lookup"><span data-stu-id="de833-2379">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="de833-2380">Backup</span><span class="sxs-lookup"><span data-stu-id="de833-2380">Backup</span></span>

* <span data-ttu-id="de833-2381">Modification de l’option `--container-name` de `backup item list` désormais facultative</span><span class="sxs-lookup"><span data-stu-id="de833-2381">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="de833-2382">Ajout d’options de compte de stockage à `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="de833-2382">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="de833-2383">Correction de la vérification de l’emplacement dans `backup protection enable-for-vm`, ne tient désormais plus compte de la casse</span><span class="sxs-lookup"><span data-stu-id="de833-2383">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="de833-2384">Correction d’un problème qui causait l’échec des commandes avec un nom de conteneur non valide</span><span class="sxs-lookup"><span data-stu-id="de833-2384">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="de833-2385">Modification de `backup item list` pour inclure « État d’intégrité » par défaut</span><span class="sxs-lookup"><span data-stu-id="de833-2385">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="de833-2386">Batch</span><span class="sxs-lookup"><span data-stu-id="de833-2386">Batch</span></span>

* <span data-ttu-id="de833-2387">Modification de `batch login` pour retourner des détails d’authentification</span><span class="sxs-lookup"><span data-stu-id="de833-2387">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="de833-2388">Cloud</span><span class="sxs-lookup"><span data-stu-id="de833-2388">Cloud</span></span>

* <span data-ttu-id="de833-2389">Ne requiert plus de points de terminaison lors de la définition de `--profile` sur un cloud</span><span class="sxs-lookup"><span data-stu-id="de833-2389">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="de833-2390">Consommation</span><span class="sxs-lookup"><span data-stu-id="de833-2390">Consumption</span></span>

* <span data-ttu-id="de833-2391">Ajout de nouvelles commandes pour les réservations : `consumption reservations summaries` et `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="de833-2391">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="de833-2392">Event Grid</span><span class="sxs-lookup"><span data-stu-id="de833-2392">Event Grid</span></span>

* <span data-ttu-id="de833-2393">[CHANGEMENT CASSANT] Déplacement des commandes `az eventgrid topic event-subscription` vers `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="de833-2393">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="de833-2394">[CHANGEMENT CASSANT] Déplacement des commandes `az eventgrid resource event-subscription` vers `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="de833-2394">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="de833-2395">[CHANGEMENT CASSANT] Suppression de la commande `eventgrid event-subscription show-endpoint-url`</span><span class="sxs-lookup"><span data-stu-id="de833-2395">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="de833-2396">Utilisation de `eventgrid event-subscription show --include-full-endpoint-url` à la place</span><span class="sxs-lookup"><span data-stu-id="de833-2396">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="de833-2397">Ajout de la commande `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="de833-2397">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="de833-2398">Ajout de la commande `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="de833-2398">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="de833-2399">Ajout du paramètre `--ids` pour les commandes `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="de833-2399">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="de833-2400">Ajout de la prise en charge de la saisie semi-automatique via la touche TAB pour les noms de rubrique</span><span class="sxs-lookup"><span data-stu-id="de833-2400">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="de833-2401">Interactive</span><span class="sxs-lookup"><span data-stu-id="de833-2401">Interactive</span></span>

* <span data-ttu-id="de833-2402">Correction d’un problème qui empêchait le fonctionnement du mode interactif avec Python 2.x</span><span class="sxs-lookup"><span data-stu-id="de833-2402">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="de833-2403">Corrections d’erreurs au démarrage</span><span class="sxs-lookup"><span data-stu-id="de833-2403">Fixed errors on startup</span></span>
* <span data-ttu-id="de833-2404">Correction du problème de commandes ne s’exécutant pas en mode interactif</span><span class="sxs-lookup"><span data-stu-id="de833-2404">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="de833-2405">IoT</span><span class="sxs-lookup"><span data-stu-id="de833-2405">IoT</span></span>

* <span data-ttu-id="de833-2406">Ajout de la prise en charge du service de provisionnement des appareils</span><span class="sxs-lookup"><span data-stu-id="de833-2406">Added support for device provisioning service</span></span>
* <span data-ttu-id="de833-2407">Ajout de messages de désapprobation dans les commandes et l’aide relative aux commandes</span><span class="sxs-lookup"><span data-stu-id="de833-2407">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="de833-2408">Ajout de la vérification IoT pour informer les utilisateurs de l’extension IoT</span><span class="sxs-lookup"><span data-stu-id="de833-2408">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="de833-2409">Moniteur</span><span class="sxs-lookup"><span data-stu-id="de833-2409">Monitor</span></span>

* <span data-ttu-id="de833-2410">Ajout de la prise en charge des paramètres multi diagnostic.</span><span class="sxs-lookup"><span data-stu-id="de833-2410">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="de833-2411">Le paramètre `--name` est désormais requis pour `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="de833-2411">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="de833-2412">Ajout de la commande `monitor diagnostic-settings categories` pour obtenir la catégorie des paramètres de diagnostic</span><span class="sxs-lookup"><span data-stu-id="de833-2412">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="de833-2413">Réseau</span><span class="sxs-lookup"><span data-stu-id="de833-2413">Network</span></span>

* <span data-ttu-id="de833-2414">Résolution du problème se produisant lors de la tentative de passage au mode actif-passif, ou depuis ce dernier, avec `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="de833-2414">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="de833-2415">Ajout de la prise en charge de HTTP2 vers `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="de833-2415">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="de833-2416">Profil</span><span class="sxs-lookup"><span data-stu-id="de833-2416">Profile</span></span>

* <span data-ttu-id="de833-2417">Ajout de la prise en charge pour la connexion à l’aide d’identités affectées aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="de833-2417">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="de833-2418">Role</span><span class="sxs-lookup"><span data-stu-id="de833-2418">Role</span></span>

* <span data-ttu-id="de833-2419">Ajout de l’argument `--assignee-object-id` à `role assignment create` pour ignorer les requêtes de graphique</span><span class="sxs-lookup"><span data-stu-id="de833-2419">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="de833-2420">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="de833-2420">Service Fabric</span></span>

* <span data-ttu-id="de833-2421">Ajout d’erreurs détaillées à la réponse de validation lors de la création du cluster</span><span class="sxs-lookup"><span data-stu-id="de833-2421">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="de833-2422">Résolution du problème concernant le client manquant avec plusieurs commandes</span><span class="sxs-lookup"><span data-stu-id="de833-2422">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="de833-2423">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="de833-2423">VM</span></span>

* <span data-ttu-id="de833-2424">[PRÉVERSION] Prise en charge interzone pour `vmss`</span><span class="sxs-lookup"><span data-stu-id="de833-2424">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="de833-2425">[CHANGEMENT CASSANT] Modification de la valeur par défaut `vmss` de zone unique en équilibreur de charge « Standard »</span><span class="sxs-lookup"><span data-stu-id="de833-2425">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="de833-2426">[CHANGEMENT CASSANT] Modification de `externalIdentities` en `userAssignedIdentities` pour EMSI</span><span class="sxs-lookup"><span data-stu-id="de833-2426">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="de833-2427">[PRÉVERSION] Ajout de la prise en charge de l’échange de disque du système d’exploitation</span><span class="sxs-lookup"><span data-stu-id="de833-2427">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="de833-2428">Ajout de la prise en charge de l’utilisation des images de machine virtuelle à partir d’autres abonnements</span><span class="sxs-lookup"><span data-stu-id="de833-2428">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="de833-2429">Ajout des arguments `--plan-name`, `--plan-product`, `--plan-promotion-code` et `--plan-publisher` à `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="de833-2429">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="de833-2430">Correction des problèmes d’erreur avec `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="de833-2430">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="de833-2431">Correction de l’utilisation excessive des ressources due à `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="de833-2431">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="de833-2432">19 décembre 2017</span><span class="sxs-lookup"><span data-stu-id="de833-2432">December 19, 2017</span></span>

<span data-ttu-id="de833-2433">Version 2.0.23</span><span class="sxs-lookup"><span data-stu-id="de833-2433">Version 2.0.23</span></span>

* <span data-ttu-id="de833-2434">Ajout de la prise en charge pour la connexion à l’aide d’identités affectées aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="de833-2434">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="de833-2435">Conteneur</span><span class="sxs-lookup"><span data-stu-id="de833-2435">Container</span></span>

* <span data-ttu-id="de833-2436">Correction de l’ordre incorrect des paramètres pour les journaux d’activité du conteneur</span><span class="sxs-lookup"><span data-stu-id="de833-2436">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="de833-2437">Réseau</span><span class="sxs-lookup"><span data-stu-id="de833-2437">Network</span></span>

* <span data-ttu-id="de833-2438">Ajout de l’argument `--disable-bgp-route-propagation` à `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="de833-2438">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="de833-2439">Ajout de l’argument `--ip-tags` à `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="de833-2439">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="de833-2440">Stockage</span><span class="sxs-lookup"><span data-stu-id="de833-2440">Storage</span></span>

* <span data-ttu-id="de833-2441">Ajout de la prise en charge du stockage V2</span><span class="sxs-lookup"><span data-stu-id="de833-2441">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="de833-2442">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="de833-2442">VM</span></span>

* <span data-ttu-id="de833-2443">[APERÇU] Ajout de la prise en charge des identités affectées aux utilisateurs pour les machines virtuelles et les VMSS</span><span class="sxs-lookup"><span data-stu-id="de833-2443">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="de833-2444">5 décembre 2017</span><span class="sxs-lookup"><span data-stu-id="de833-2444">December 5, 2017</span></span>

<span data-ttu-id="de833-2445">Version 2.0.22</span><span class="sxs-lookup"><span data-stu-id="de833-2445">Version 2.0.22</span></span>

* <span data-ttu-id="de833-2446">Suppression des commandes `az component`.</span><span class="sxs-lookup"><span data-stu-id="de833-2446">Removed `az component` commands.</span></span> <span data-ttu-id="de833-2447">Utilisation de `az extension` à la place</span><span class="sxs-lookup"><span data-stu-id="de833-2447">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="de833-2448">Core</span><span class="sxs-lookup"><span data-stu-id="de833-2448">Core</span></span>
* <span data-ttu-id="de833-2449">Modification du point de terminaison de l’autorité AAD `AZURE_US_GOV_CLOUD` pour le faire passer de login.microsoftonline.com à login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="de833-2449">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="de833-2450">Résolution du problème au cours duquel les données de télémétrie étaient constamment renvoyées</span><span class="sxs-lookup"><span data-stu-id="de833-2450">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="de833-2451">ACS</span><span class="sxs-lookup"><span data-stu-id="de833-2451">ACS</span></span>

* <span data-ttu-id="de833-2452">Ajout des commandes `aks install-connector` et `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="de833-2452">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="de833-2453">Amélioration des rapports d’erreurs pour `acs create`</span><span class="sxs-lookup"><span data-stu-id="de833-2453">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="de833-2454">Correction de l’utilisation de `aks get-credentials -f` sans chemin d’accès complet</span><span class="sxs-lookup"><span data-stu-id="de833-2454">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="de833-2455">Advisor</span><span class="sxs-lookup"><span data-stu-id="de833-2455">Advisor</span></span>

* <span data-ttu-id="de833-2456">Version initiale</span><span class="sxs-lookup"><span data-stu-id="de833-2456">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="de833-2457">AppService</span><span class="sxs-lookup"><span data-stu-id="de833-2457">Appservice</span></span>

* <span data-ttu-id="de833-2458">Correction de la génération du nom de certificat avec `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="de833-2458">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="de833-2459">Correction de `webapp [list|show]` et `functionapp [list|show]` de manière à afficher les applications correctes</span><span class="sxs-lookup"><span data-stu-id="de833-2459">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="de833-2460">Ajout de la valeur par défaut pour `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="de833-2460">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="de833-2461">Consommation</span><span class="sxs-lookup"><span data-stu-id="de833-2461">Consumption</span></span>

* <span data-ttu-id="de833-2462">Ajout de la prise en charge de l’API version 2017-11-30</span><span class="sxs-lookup"><span data-stu-id="de833-2462">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="de833-2463">Conteneur</span><span class="sxs-lookup"><span data-stu-id="de833-2463">Container</span></span>

* <span data-ttu-id="de833-2464">Correction de la régression des ports par défaut</span><span class="sxs-lookup"><span data-stu-id="de833-2464">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="de833-2465">Moniteur</span><span class="sxs-lookup"><span data-stu-id="de833-2465">Monitor</span></span>

* <span data-ttu-id="de833-2466">Ajout de la prise en charge de plusieurs dimensions à la commande des mesures</span><span class="sxs-lookup"><span data-stu-id="de833-2466">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="de833-2467">Ressource</span><span class="sxs-lookup"><span data-stu-id="de833-2467">Resource</span></span>

* <span data-ttu-id="de833-2468">Ajout de l’argument `--include-response-body` à `resource show`</span><span class="sxs-lookup"><span data-stu-id="de833-2468">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="de833-2469">Role</span><span class="sxs-lookup"><span data-stu-id="de833-2469">Role</span></span>

* <span data-ttu-id="de833-2470">Ajout de l’affichage des affectations par défaut pour les administrateurs « classiques » à `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="de833-2470">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="de833-2471">Ajout de la prise en charge à `ad sp reset-credentials` pour l’ajout d’informations d’identification au lieu de leur remplacement</span><span class="sxs-lookup"><span data-stu-id="de833-2471">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="de833-2472">Amélioration des rapports d’erreurs pour `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="de833-2472">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="de833-2473">SQL</span><span class="sxs-lookup"><span data-stu-id="de833-2473">SQL</span></span>

* <span data-ttu-id="de833-2474">Ajout des commandes `sql db list-usages` et `sql db show-usage`</span><span class="sxs-lookup"><span data-stu-id="de833-2474">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="de833-2475">Ajout des commandes `sql server conn-policy show` et `sql server conn-policy update`</span><span class="sxs-lookup"><span data-stu-id="de833-2475">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="de833-2476">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="de833-2476">VM</span></span>

* <span data-ttu-id="de833-2477">Ajout des informations de zone à `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="de833-2477">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="de833-2478">14 novembre 2017</span><span class="sxs-lookup"><span data-stu-id="de833-2478">November 14, 2017</span></span>

<span data-ttu-id="de833-2479">Version 2.0.21</span><span class="sxs-lookup"><span data-stu-id="de833-2479">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="de833-2480">ACR</span><span class="sxs-lookup"><span data-stu-id="de833-2480">ACR</span></span>

* <span data-ttu-id="de833-2481">Ajout de la prise en charge pour la création de webhooks dans les régions de réplication</span><span class="sxs-lookup"><span data-stu-id="de833-2481">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="de833-2482">ACS</span><span class="sxs-lookup"><span data-stu-id="de833-2482">ACS</span></span>

* <span data-ttu-id="de833-2483">Modification de toutes les mentions « agent » en « nœud » dans AKS</span><span class="sxs-lookup"><span data-stu-id="de833-2483">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="de833-2484">Option `--orchestrator-release` déconseillée pour `acs create`</span><span class="sxs-lookup"><span data-stu-id="de833-2484">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="de833-2485">Changement de la taille de machine virtuelle par défaut pour AKS à `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="de833-2485">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="de833-2486">Résolution de `az aks browse` sur Windows</span><span class="sxs-lookup"><span data-stu-id="de833-2486">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="de833-2487">Résolution de `az aks get-credentials` sur Windows</span><span class="sxs-lookup"><span data-stu-id="de833-2487">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="de833-2488">AppService</span><span class="sxs-lookup"><span data-stu-id="de833-2488">Appservice</span></span>

* <span data-ttu-id="de833-2489">Ajout de la source de déploiement `config-zip` pour les applications Web et de fonction</span><span class="sxs-lookup"><span data-stu-id="de833-2489">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="de833-2490">Ajout de l’option `--docker-container-logging` à `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="de833-2490">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="de833-2491">Suppression de l’option `storage` du paramètre `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="de833-2491">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="de833-2492">Amélioration des messages d’erreur pour `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="de833-2492">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="de833-2493">Ajout de la prise en charge pour la création d’applications de fonction Linux</span><span class="sxs-lookup"><span data-stu-id="de833-2493">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="de833-2494">`list-locations` fixe</span><span class="sxs-lookup"><span data-stu-id="de833-2494">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="de833-2495">Batch</span><span class="sxs-lookup"><span data-stu-id="de833-2495">Batch</span></span>

* <span data-ttu-id="de833-2496">Correction du bogue dans la commande de création de pool lorsqu’un ID ressource a été utilisé avec l’indicateur `--image`</span><span class="sxs-lookup"><span data-stu-id="de833-2496">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="de833-2497">Batchai</span><span class="sxs-lookup"><span data-stu-id="de833-2497">Batchai</span></span>

* <span data-ttu-id="de833-2498">Ajout de l’option courte, `-s`, pour `--vm-size` quand la taille de machine virtuelle est fournie dans la commande `file-server create`</span><span class="sxs-lookup"><span data-stu-id="de833-2498">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="de833-2499">Ajout du nom de compte de stockage et des arguments de clé dans les paramètres `cluster create`</span><span class="sxs-lookup"><span data-stu-id="de833-2499">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="de833-2500">Résolution de la documentation pour `job list-files` et `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="de833-2500">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="de833-2501">Ajout de l’option courte, `-r`, pour `--cluster-name` quand le nom du cluster est fourni dans la commande `job create`</span><span class="sxs-lookup"><span data-stu-id="de833-2501">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="de833-2502">Cloud</span><span class="sxs-lookup"><span data-stu-id="de833-2502">Cloud</span></span>

* <span data-ttu-id="de833-2503">Modification de `cloud [register|update]` pour empêcher l’inscription des clouds qui ne disposent pas de tous les points de terminaison requis</span><span class="sxs-lookup"><span data-stu-id="de833-2503">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="de833-2504">Conteneur</span><span class="sxs-lookup"><span data-stu-id="de833-2504">Container</span></span>

* <span data-ttu-id="de833-2505">Ajout de la prise en charge pour ouvrir plusieurs ports</span><span class="sxs-lookup"><span data-stu-id="de833-2505">Added support to open multiple ports</span></span>
* <span data-ttu-id="de833-2506">Ajout de la stratégie de redémarrage du groupe de conteneurs</span><span class="sxs-lookup"><span data-stu-id="de833-2506">Added container group restart policy</span></span>
* <span data-ttu-id="de833-2507">Ajout de la prise en charge pour monter le partage de fichier Azure en tant que volume</span><span class="sxs-lookup"><span data-stu-id="de833-2507">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="de833-2508">Mise à jour des documents d’assistance</span><span class="sxs-lookup"><span data-stu-id="de833-2508">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="de833-2509">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="de833-2509">Data Lake Analytics</span></span>

* <span data-ttu-id="de833-2510">Modification de `[job|account] list` pour retourner des informations plus concises</span><span class="sxs-lookup"><span data-stu-id="de833-2510">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="de833-2511">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="de833-2511">Data Lake Store</span></span>

* <span data-ttu-id="de833-2512">Modification de `account list` pour retourner des informations plus concises</span><span class="sxs-lookup"><span data-stu-id="de833-2512">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="de833-2513">Extension</span><span class="sxs-lookup"><span data-stu-id="de833-2513">Extension</span></span>

* <span data-ttu-id="de833-2514">Ajout de `extension list-available` pour permettre l’affichage de la liste des extensions officielles Microsoft</span><span class="sxs-lookup"><span data-stu-id="de833-2514">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="de833-2515">Ajout de `--name` à `extension [add|update]` pour permettre l’installation des extensions par nom</span><span class="sxs-lookup"><span data-stu-id="de833-2515">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="de833-2516">IoT</span><span class="sxs-lookup"><span data-stu-id="de833-2516">IoT</span></span>

* <span data-ttu-id="de833-2517">Ajout de la prise en charge pour les autorités de certification (CA) et les chaînes d’approbation</span><span class="sxs-lookup"><span data-stu-id="de833-2517">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="de833-2518">Moniteur</span><span class="sxs-lookup"><span data-stu-id="de833-2518">Monitor</span></span>

* <span data-ttu-id="de833-2519">Ajout des commandes `activity-log alert`</span><span class="sxs-lookup"><span data-stu-id="de833-2519">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="de833-2520">Réseau</span><span class="sxs-lookup"><span data-stu-id="de833-2520">Network</span></span>

* <span data-ttu-id="de833-2521">Ajout de la prise en charge pour les enregistrements DNS CAA</span><span class="sxs-lookup"><span data-stu-id="de833-2521">Added support for CAA DNS records</span></span>
* <span data-ttu-id="de833-2522">Résolution d’un problème empêchant la mise à jour des points de terminaison avec `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="de833-2522">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="de833-2523">Résolution d’un problème où `vnet update --dns-servers` ne fonctionnait pas, en fonction de la façon dont avait été créé le réseau virtuel</span><span class="sxs-lookup"><span data-stu-id="de833-2523">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="de833-2524">Résolution d’un problème où les noms DNS relatifs n’étaient pas importés correctement par `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="de833-2524">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="de833-2525">Réservations</span><span class="sxs-lookup"><span data-stu-id="de833-2525">Reservations</span></span>

* <span data-ttu-id="de833-2526">Version préliminaire initiale</span><span class="sxs-lookup"><span data-stu-id="de833-2526">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="de833-2527">Ressource</span><span class="sxs-lookup"><span data-stu-id="de833-2527">Resource</span></span>

* <span data-ttu-id="de833-2528">Ajout de la prise en charge pour les ID de ressource au paramètre `--resource` et pour les verrous au niveau des ressources</span><span class="sxs-lookup"><span data-stu-id="de833-2528">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="de833-2529">SQL</span><span class="sxs-lookup"><span data-stu-id="de833-2529">SQL</span></span>

* <span data-ttu-id="de833-2530">Ajout du paramètre `--ignore-missing-vnet-service-endpoint` pour `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="de833-2530">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="de833-2531">Stockage</span><span class="sxs-lookup"><span data-stu-id="de833-2531">Storage</span></span>

* <span data-ttu-id="de833-2532">Modification de `storage account create` pour utiliser la référence SKU `Standard_RAGRS` par défaut</span><span class="sxs-lookup"><span data-stu-id="de833-2532">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="de833-2533">Correction du bogue lors du traitement des noms d’objets blob/de fichier qui incluent des caractères non-ascii</span><span class="sxs-lookup"><span data-stu-id="de833-2533">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="de833-2534">Correction du bogue qui empêchait l’utilisation de `--source-uri` avec `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="de833-2534">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="de833-2535">Ajout de commandes pour paramétrer et supprimer plusieurs objets avec `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="de833-2535">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="de833-2536">Résolution du problème de l’activation des métriques avec `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="de833-2536">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="de833-2537">Résolution du problème des fichiers de plus de 200 Go lors de l’utilisation de `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="de833-2537">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="de833-2538">Résolution du problème où `--bypass` et `--default-action` étaient ignorés par `storage account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="de833-2538">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="de833-2539">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="de833-2539">VM</span></span>

* <span data-ttu-id="de833-2540">Correction d’un bogue avec `vmss create` qui empêchait l’utilisation du niveau de taille `Basic`</span><span class="sxs-lookup"><span data-stu-id="de833-2540">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="de833-2541">Ajout d’arguments `--plan` à `[vm|vmss] create` pour les images personnalisées avec des informations de facturation</span><span class="sxs-lookup"><span data-stu-id="de833-2541">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="de833-2542">Ajout des commandes `vm secret `[add|remove|list]</span><span class="sxs-lookup"><span data-stu-id="de833-2542">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="de833-2543">`vm format-secret` renommé en `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="de833-2543">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="de833-2544">Ajout de l’argument `--encrypt format` à `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="de833-2544">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="de833-2545">24 octobre 2017</span><span class="sxs-lookup"><span data-stu-id="de833-2545">October 24, 2017</span></span>

<span data-ttu-id="de833-2546">Version 2.0.20</span><span class="sxs-lookup"><span data-stu-id="de833-2546">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="de833-2547">Core</span><span class="sxs-lookup"><span data-stu-id="de833-2547">Core</span></span>

* <span data-ttu-id="de833-2548">Mise à jour de `2017-03-09-profile` pour consommer l’API `MGMT_STORAGE` version `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="de833-2548">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="de833-2549">ACR</span><span class="sxs-lookup"><span data-stu-id="de833-2549">ACR</span></span>

* <span data-ttu-id="de833-2550">Mise à jour de la gestion des ressources pour pointer vers la version d’API `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="de833-2550">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="de833-2551">Modification de la référence SKU « Bring Your Own Storage » en Classique</span><span class="sxs-lookup"><span data-stu-id="de833-2551">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="de833-2552">Changement des noms des références SKU de registre en De base, Standard, et Premium</span><span class="sxs-lookup"><span data-stu-id="de833-2552">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="de833-2553">ACS</span><span class="sxs-lookup"><span data-stu-id="de833-2553">ACS</span></span>

* <span data-ttu-id="de833-2554">[PRÉVERSION] Ajout des commandes `az aks`</span><span class="sxs-lookup"><span data-stu-id="de833-2554">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="de833-2555">Réparation de Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="de833-2555">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="de833-2556">AppService</span><span class="sxs-lookup"><span data-stu-id="de833-2556">Appservice</span></span>

* <span data-ttu-id="de833-2557">Résolution d’une erreur où le téléchargement des journaux d’activité `webapp` était incorrect</span><span class="sxs-lookup"><span data-stu-id="de833-2557">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="de833-2558">Composant</span><span class="sxs-lookup"><span data-stu-id="de833-2558">Component</span></span>

* <span data-ttu-id="de833-2559">Ajout de clarté dans les messages visant à déconseiller de tous les programmes d’installation et des invites de confirmation</span><span class="sxs-lookup"><span data-stu-id="de833-2559">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="de833-2560">Moniteur</span><span class="sxs-lookup"><span data-stu-id="de833-2560">Monitor</span></span>

* <span data-ttu-id="de833-2561">Ajout des commandes `action-group`</span><span class="sxs-lookup"><span data-stu-id="de833-2561">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="de833-2562">Ressource</span><span class="sxs-lookup"><span data-stu-id="de833-2562">Resource</span></span>

* <span data-ttu-id="de833-2563">Résolution d’une incompatibilité de la dépendance msrest dans `group export` avec les versions les plus récentes</span><span class="sxs-lookup"><span data-stu-id="de833-2563">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="de833-2564">Résolution de `policy assignment create` pour qu’il fonctionne avec les définitions de stratégie et les définitions d’ensemble de stratégie intégrées</span><span class="sxs-lookup"><span data-stu-id="de833-2564">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="de833-2565">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="de833-2565">VM</span></span>

* <span data-ttu-id="de833-2566">Ajout de l’argument `--accelerated-networking` à `vmss create`</span><span class="sxs-lookup"><span data-stu-id="de833-2566">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="de833-2567">9 octobre 2017</span><span class="sxs-lookup"><span data-stu-id="de833-2567">October 9, 2017</span></span>

<span data-ttu-id="de833-2568">Version 2.0.19</span><span class="sxs-lookup"><span data-stu-id="de833-2568">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="de833-2569">Core</span><span class="sxs-lookup"><span data-stu-id="de833-2569">Core</span></span>

* <span data-ttu-id="de833-2570">Ajout de la gestion des URL d’autorisation AD FS avec une barre oblique à Azure Stack</span><span class="sxs-lookup"><span data-stu-id="de833-2570">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="de833-2571">AppService</span><span class="sxs-lookup"><span data-stu-id="de833-2571">Appservice</span></span>

* <span data-ttu-id="de833-2572">Ajout de la mise à jour générique avec la nouvelle commande `webapp update`</span><span class="sxs-lookup"><span data-stu-id="de833-2572">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="de833-2573">Batch</span><span class="sxs-lookup"><span data-stu-id="de833-2573">Batch</span></span>

* <span data-ttu-id="de833-2574">Mis à jour du kit de développement logiciel (SDK) à la version 4.0.0</span><span class="sxs-lookup"><span data-stu-id="de833-2574">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="de833-2575">Mise à jour de l’option `--image` de VirtualMachineConfiguration pour prendre en charge les références d’image ARM en plus de publish:offre:sku:version</span><span class="sxs-lookup"><span data-stu-id="de833-2575">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="de833-2576">Ajout de la prise en charge du nouveau modèle d’extension CLI pour les commandes d’extension Batch</span><span class="sxs-lookup"><span data-stu-id="de833-2576">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="de833-2577">Suppression de la prise en charge Batch des modèles de composants</span><span class="sxs-lookup"><span data-stu-id="de833-2577">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="de833-2578">Batchai</span><span class="sxs-lookup"><span data-stu-id="de833-2578">Batchai</span></span>

* <span data-ttu-id="de833-2579">Version initiale du module Batch AI</span><span class="sxs-lookup"><span data-stu-id="de833-2579">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="de833-2580">KeyVault</span><span class="sxs-lookup"><span data-stu-id="de833-2580">Keyvault</span></span>

* <span data-ttu-id="de833-2581">Résolution du problème d’authentification Key Vault lors de l’utilisation d’AD FS sur Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="de833-2581">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="de833-2582">(#4448)</span><span class="sxs-lookup"><span data-stu-id="de833-2582">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="de833-2583">Réseau</span><span class="sxs-lookup"><span data-stu-id="de833-2583">Network</span></span>

* <span data-ttu-id="de833-2584">La modification de l’argument `--server` de `application-gateway address-pool create` devient facultative, permettant les pools d’adresses vides</span><span class="sxs-lookup"><span data-stu-id="de833-2584">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="de833-2585">Mise à jour de `traffic-manager` pour prendre en charge les fonctionnalités les plus récentes</span><span class="sxs-lookup"><span data-stu-id="de833-2585">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="de833-2586">Ressource</span><span class="sxs-lookup"><span data-stu-id="de833-2586">Resource</span></span>

* <span data-ttu-id="de833-2587">Ajout de la prise en charge des options `--resource-group/-g` pour le nom du groupe de ressources dans `group`</span><span class="sxs-lookup"><span data-stu-id="de833-2587">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="de833-2588">Ajout des commandes à `account lock` pour travailler avec des verrous au niveau de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="de833-2588">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="de833-2589">Ajout des commandes à `group lock` pour travailler avec des verrous au niveau du groupe</span><span class="sxs-lookup"><span data-stu-id="de833-2589">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="de833-2590">Ajout des commandes à `resource lock` pour travailler avec des verrous au niveau des ressources</span><span class="sxs-lookup"><span data-stu-id="de833-2590">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="de833-2591">SQL</span><span class="sxs-lookup"><span data-stu-id="de833-2591">Sql</span></span>

* <span data-ttu-id="de833-2592">Ajout de la prise en charge pour le Chiffrement transparent des données (TDE) SQL et le chiffrement transparent des données avec Bring Your Own Key</span><span class="sxs-lookup"><span data-stu-id="de833-2592">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="de833-2593">Ajout de la commande `db list-deleted` et du paramètre `db restore --deleted-time`, ce qui offre la possibilité de rechercher et de restaurer les bases de données supprimées</span><span class="sxs-lookup"><span data-stu-id="de833-2593">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="de833-2594">Ajout de `db op list` et `db op cancel`, ce qui offre la capacité de répertorier et d’annuler des opérations en cours sur la base de données</span><span class="sxs-lookup"><span data-stu-id="de833-2594">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="de833-2595">Stockage</span><span class="sxs-lookup"><span data-stu-id="de833-2595">Storage</span></span>

* <span data-ttu-id="de833-2596">Ajout de la prise en charge d’instantané de partage de fichiers</span><span class="sxs-lookup"><span data-stu-id="de833-2596">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="de833-2597">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="de833-2597">Vm</span></span>

* <span data-ttu-id="de833-2598">Correction d’un bogue dans `vm show` où l’utilisation de `-d` a provoqué un incident dans les adresses IP privées manquantes</span><span class="sxs-lookup"><span data-stu-id="de833-2598">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="de833-2599">[VERSION PRÉLIMINAIRE] Ajout de la prise en charge de la mise à niveau propagée pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="de833-2599">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="de833-2600">Ajout de la prise en charge de la mise à jour des paramètres de chiffrement avec `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="de833-2600">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="de833-2601">Ajout du paramètre `--os-disk-size-gb` pour `vm create`</span><span class="sxs-lookup"><span data-stu-id="de833-2601">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="de833-2602">Ajout du paramètre `--license-type` de Windows pour `vmss create`</span><span class="sxs-lookup"><span data-stu-id="de833-2602">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="de833-2603">22 septembre 2017</span><span class="sxs-lookup"><span data-stu-id="de833-2603">September 22, 2017</span></span>

<span data-ttu-id="de833-2604">Version 2.0.18</span><span class="sxs-lookup"><span data-stu-id="de833-2604">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="de833-2605">Ressource</span><span class="sxs-lookup"><span data-stu-id="de833-2605">Resource</span></span>

* <span data-ttu-id="de833-2606">Ajout de la prise en charge de l’affichage des définitions de stratégie intégrée</span><span class="sxs-lookup"><span data-stu-id="de833-2606">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="de833-2607">Ajout de la prise en charge du paramètre de mode pour la création de définitions de stratégie</span><span class="sxs-lookup"><span data-stu-id="de833-2607">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="de833-2608">Ajout de la prise en charge des définitions d’interface utilisateur et des modèles pour `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="de833-2608">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="de833-2609">[CHANGEMENT CASSANT] Modification du type de ressource `managedapp` de `appliances` en `applications` et de `applianceDefinitions` en `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="de833-2609">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="de833-2610">Réseau</span><span class="sxs-lookup"><span data-stu-id="de833-2610">Network</span></span>

* <span data-ttu-id="de833-2611">Ajout de la prise en charge de la zone de disponibilité aux sous-commandes `network lb` et `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="de833-2611">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="de833-2612">Ajout de la prise en charge du peering Microsoft IPv6 pour `express-route`</span><span class="sxs-lookup"><span data-stu-id="de833-2612">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="de833-2613">Ajout des commandes du groupe de sécurité d’application `asg`</span><span class="sxs-lookup"><span data-stu-id="de833-2613">Added `asg` application security group commands</span></span>
* <span data-ttu-id="de833-2614">Ajout de l’argument `--application-security-groups` à `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="de833-2614">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="de833-2615">Ajout des arguments `--source-asgs` et `--destination-asgs` à `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="de833-2615">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="de833-2616">Ajout des arguments `--ddos-protection` et `--vm-protection` à `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="de833-2616">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="de833-2617">Ajout des commandes `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="de833-2617">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="de833-2618">Stockage</span><span class="sxs-lookup"><span data-stu-id="de833-2618">Storage</span></span>

* <span data-ttu-id="de833-2619">Résolution d’un problème qui pouvait causer l’échec des commandes `storage account network-rule` après la mise à jour du Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="de833-2619">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="de833-2620">Événement</span><span class="sxs-lookup"><span data-stu-id="de833-2620">Eventgrid</span></span>

* <span data-ttu-id="de833-2621">Mise à jour du Kit de développement logiciel (SDK) Python Azure Event Grid afin d’utiliser une version plus récente de l’API « 2017-09-15-preview »</span><span class="sxs-lookup"><span data-stu-id="de833-2621">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="de833-2622">SQL</span><span class="sxs-lookup"><span data-stu-id="de833-2622">SQL</span></span>

* <span data-ttu-id="de833-2623">La modification de l’`sql server list`argument`--resource-group` devient facultative.</span><span class="sxs-lookup"><span data-stu-id="de833-2623">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="de833-2624">En l’absence de précisions, tous les serveurs SQL dans l’abonnement seront retournés</span><span class="sxs-lookup"><span data-stu-id="de833-2624">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="de833-2625">Ajout du paramètre `--no-wait` à `db [create|copy|restore|update|replica create|create|update]` et `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="de833-2625">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="de833-2626">KeyVault</span><span class="sxs-lookup"><span data-stu-id="de833-2626">Keyvault</span></span>

* <span data-ttu-id="de833-2627">Ajout de la prise en charge des commandes Keyvault derrière un proxy</span><span class="sxs-lookup"><span data-stu-id="de833-2627">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="de833-2628">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="de833-2628">VM</span></span>

* <span data-ttu-id="de833-2629">Ajout de la prise en charge de zone de disponibilité pour `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="de833-2629">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="de833-2630">Résolution d’un problème à cause duquel l’utilisation de `--app-gateway ID` avec `vmss create` entraînait un échec</span><span class="sxs-lookup"><span data-stu-id="de833-2630">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="de833-2631">Ajout de l’argument `--asgs` à `vm create`</span><span class="sxs-lookup"><span data-stu-id="de833-2631">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="de833-2632">Ajout de la prise en charge des commandes en cours d’exécution sur des machines virtuelles avec `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="de833-2632">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="de833-2633">[PRÉVERSION] Ajout de la prise en charge du chiffrement de disque VMSS avec `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="de833-2633">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="de833-2634">Ajout de la prise en charge de la réalisation de la maintenance sur des machines virtuelles avec `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="de833-2634">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="de833-2635">ACS</span><span class="sxs-lookup"><span data-stu-id="de833-2635">ACS</span></span>

* <span data-ttu-id="de833-2636">[PRÉVERSION] Ajout de l’argument `--orchestrator-release` à `acs create` pour les régions ACS en préversion</span><span class="sxs-lookup"><span data-stu-id="de833-2636">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="de833-2637">AppService</span><span class="sxs-lookup"><span data-stu-id="de833-2637">Appservice</span></span>

* <span data-ttu-id="de833-2638">Ajout de la capacité à mettre à jour et à afficher les paramètres d’authentification avec `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="de833-2638">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="de833-2639">Backup</span><span class="sxs-lookup"><span data-stu-id="de833-2639">Backup</span></span>

* <span data-ttu-id="de833-2640">Préversion</span><span class="sxs-lookup"><span data-stu-id="de833-2640">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="de833-2641">11 septembre 2017</span><span class="sxs-lookup"><span data-stu-id="de833-2641">September 11, 2017</span></span>

<span data-ttu-id="de833-2642">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="de833-2642">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="de833-2643">Core</span><span class="sxs-lookup"><span data-stu-id="de833-2643">Core</span></span>

* <span data-ttu-id="de833-2644">Module de commande activé pour définir son propre ID de corrélation dans la télémétrie</span><span class="sxs-lookup"><span data-stu-id="de833-2644">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="de833-2645">Résolution du problème de vidage JSON lorsque la télémétrie est définie en mode diagnostics</span><span class="sxs-lookup"><span data-stu-id="de833-2645">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="de833-2646">Acs</span><span class="sxs-lookup"><span data-stu-id="de833-2646">Acs</span></span>

* <span data-ttu-id="de833-2647">Ajout de la commande `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="de833-2647">Added `acs list-locations` command</span></span>
* <span data-ttu-id="de833-2648">Faire en sorte que `ssh-key-file` soit fourni avec la valeur par défaut attendu</span><span class="sxs-lookup"><span data-stu-id="de833-2648">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="de833-2649">AppService</span><span class="sxs-lookup"><span data-stu-id="de833-2649">Appservice</span></span>

* <span data-ttu-id="de833-2650">Ajout de la possibilité de créer une application web dans un groupe de ressources autre que celui du plan de service actif</span><span class="sxs-lookup"><span data-stu-id="de833-2650">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="de833-2651">CDN</span><span class="sxs-lookup"><span data-stu-id="de833-2651">CDN</span></span>

* <span data-ttu-id="de833-2652">Correction du bogue « CustomDomain n’est pas itérable » pour `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="de833-2652">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="de833-2653">Extension</span><span class="sxs-lookup"><span data-stu-id="de833-2653">Extension</span></span>

* <span data-ttu-id="de833-2654">Version initiale</span><span class="sxs-lookup"><span data-stu-id="de833-2654">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="de833-2655">KeyVault</span><span class="sxs-lookup"><span data-stu-id="de833-2655">Keyvault</span></span>

* <span data-ttu-id="de833-2656">Résolution du problème où les autorisations étaient sensibles à la casse pour `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="de833-2656">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="de833-2657">Réseau</span><span class="sxs-lookup"><span data-stu-id="de833-2657">Network</span></span>

* <span data-ttu-id="de833-2658">`vnet list-private-access-services` renommé en `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="de833-2658">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="de833-2659">Argument `--private-access-services` renommé en `--service-endpoints` pour`vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="de833-2659">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="de833-2660">Ajout de la prise en charge de plusieurs plages IP et de ports à `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="de833-2660">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="de833-2661">Ajout de la prise en charge de la référence (SKU) pour `lb create`</span><span class="sxs-lookup"><span data-stu-id="de833-2661">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="de833-2662">Ajout de la prise en charge de la référence (SKU) pour `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="de833-2662">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="de833-2663">Ressource</span><span class="sxs-lookup"><span data-stu-id="de833-2663">Resource</span></span>

* <span data-ttu-id="de833-2664">Autoriser le passages dans les définitions de paramètres de stratégie de ressource dans `policy definition create`, et`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="de833-2664">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="de833-2665">Autoriser le passage dans les valeurs de paramètres pour `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="de833-2665">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="de833-2666">Autoriser le passage de JSON ou d’un fichier pour tous les paramètres</span><span class="sxs-lookup"><span data-stu-id="de833-2666">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="de833-2667">Incrémentation de la version de l’API</span><span class="sxs-lookup"><span data-stu-id="de833-2667">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="de833-2668">SQL</span><span class="sxs-lookup"><span data-stu-id="de833-2668">SQL</span></span>

* <span data-ttu-id="de833-2669">Ajout des commandes `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="de833-2669">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="de833-2670">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="de833-2670">VM</span></span>

* <span data-ttu-id="de833-2671">Résolu : n’affecte aucun accès tant que `--scope` n’est pas indiqué</span><span class="sxs-lookup"><span data-stu-id="de833-2671">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="de833-2672">Résolu : utilisation de la même dénomination d’extension que celle du portail</span><span class="sxs-lookup"><span data-stu-id="de833-2672">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="de833-2673">Suppression de `subscription` de la sortie `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="de833-2673">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="de833-2674">Résolu : la référence SKU de stockage `[vm|vmss] create` n’est pas appliquée sur les disques de données avec une image</span><span class="sxs-lookup"><span data-stu-id="de833-2674">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="de833-2675">Résolu : `vm format-secret --secrets` n’accepte pas d’ID séparés par un saut de ligne</span><span class="sxs-lookup"><span data-stu-id="de833-2675">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="de833-2676">31 août 2017</span><span class="sxs-lookup"><span data-stu-id="de833-2676">August 31, 2017</span></span>

<span data-ttu-id="de833-2677">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="de833-2677">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="de833-2678">KeyVault</span><span class="sxs-lookup"><span data-stu-id="de833-2678">Keyvault</span></span>

* <span data-ttu-id="de833-2679">Correction d’un bogue à cause duquel vous tentez de résoudre automatiquement l’encodage secret avec `secret download`</span><span class="sxs-lookup"><span data-stu-id="de833-2679">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="de833-2680">Sf</span><span class="sxs-lookup"><span data-stu-id="de833-2680">Sf</span></span>

* <span data-ttu-id="de833-2681">Déconseiller toutes les commandes en faveur de Service Fabric CLI (sfctl)</span><span class="sxs-lookup"><span data-stu-id="de833-2681">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="de833-2682">Stockage</span><span class="sxs-lookup"><span data-stu-id="de833-2682">Storage</span></span>

* <span data-ttu-id="de833-2683">Résolution du problème dans lequel la création de comptes de stockage dans les régions ne prenant pas en charge la fonctionnalité NetworkACLs était impossible</span><span class="sxs-lookup"><span data-stu-id="de833-2683">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="de833-2684">Déterminer le type de contenu et l’encodage du contenu lors du chargement d’objets blob et de fichiers si aucun type de contenu et d’encodage n’est spécifié.</span><span class="sxs-lookup"><span data-stu-id="de833-2684">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="de833-2685">28 août 2017</span><span class="sxs-lookup"><span data-stu-id="de833-2685">August 28, 2017</span></span>

<span data-ttu-id="de833-2686">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="de833-2686">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="de833-2687">Interface de ligne de commande</span><span class="sxs-lookup"><span data-stu-id="de833-2687">CLI</span></span>

* <span data-ttu-id="de833-2688">Ajout d’une remarque juridique pour `--version`</span><span class="sxs-lookup"><span data-stu-id="de833-2688">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="de833-2689">ACS</span><span class="sxs-lookup"><span data-stu-id="de833-2689">ACS</span></span>

* <span data-ttu-id="de833-2690">Correction des régions d’aperçu</span><span class="sxs-lookup"><span data-stu-id="de833-2690">Corrected preview regions</span></span>
* <span data-ttu-id="de833-2691">Mise en forme par défaut `dns_name_prefix` correctement</span><span class="sxs-lookup"><span data-stu-id="de833-2691">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="de833-2692">Optimisation de la sortie de commande des services ACS</span><span class="sxs-lookup"><span data-stu-id="de833-2692">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="de833-2693">AppService</span><span class="sxs-lookup"><span data-stu-id="de833-2693">Appservice</span></span>

* <span data-ttu-id="de833-2694">[CHANGEMENT CASSANT] Fixation des incohérences dans la sortie de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="de833-2694">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="de833-2695">Ajout d’un nouvel alias de `-i` pour `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="de833-2695">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="de833-2696">Exposé `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="de833-2696">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="de833-2697">Exposition de nouveaux arguments à partir de `az webapp delete` pour conserver le plan de service d'application, les métriques ou l’inscription DNS</span><span class="sxs-lookup"><span data-stu-id="de833-2697">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="de833-2698">Résolu : détecter les paramètres d’emplacement correctement</span><span class="sxs-lookup"><span data-stu-id="de833-2698">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="de833-2699">IoT</span><span class="sxs-lookup"><span data-stu-id="de833-2699">IoT</span></span>

* <span data-ttu-id="de833-2700">Résolution de #3934 : la création de la stratégie n’efface plus les stratégies existantes</span><span class="sxs-lookup"><span data-stu-id="de833-2700">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="de833-2701">Réseau</span><span class="sxs-lookup"><span data-stu-id="de833-2701">Network</span></span>

* <span data-ttu-id="de833-2702">[CHANGEMENT CASSANT] Renommage de `vnet list-private-access-services` en `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="de833-2702">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="de833-2703">[CHANGEMENT CASSANT] Renommage de l’option `--private-access-services` en `--service-endpoints` pour `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="de833-2703">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="de833-2704">Ajout de la prise en charge de plusieurs IP et de plusieurs pages de port pour `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="de833-2704">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="de833-2705">Ajout de la prise en charge de la référence (SKU) pour `lb create`</span><span class="sxs-lookup"><span data-stu-id="de833-2705">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="de833-2706">Ajout de la prise en charge de la référence (SKU) pour `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="de833-2706">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="de833-2707">Profil</span><span class="sxs-lookup"><span data-stu-id="de833-2707">Profile</span></span>

* <span data-ttu-id="de833-2708">exposés `--msi` et `--msi-port` pour vous connecter à l’aide d’une identité de machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="de833-2708">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="de833-2709">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="de833-2709">Service Fabric</span></span>

* <span data-ttu-id="de833-2710">Préversion</span><span class="sxs-lookup"><span data-stu-id="de833-2710">Preview release</span></span>
* <span data-ttu-id="de833-2711">Règles d’utilisateur du Registre/de mot de passe simplifiées pour la commande</span><span class="sxs-lookup"><span data-stu-id="de833-2711">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="de833-2712">Invite de mot de passe fixe pour l’utilisateur, même après le passage de paramètre</span><span class="sxs-lookup"><span data-stu-id="de833-2712">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="de833-2713">Ajout de la prise en charge de vide `registry_cred`</span><span class="sxs-lookup"><span data-stu-id="de833-2713">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="de833-2714">Stockage</span><span class="sxs-lookup"><span data-stu-id="de833-2714">Storage</span></span>

* <span data-ttu-id="de833-2715">Paramétrage du niveau blob activé</span><span class="sxs-lookup"><span data-stu-id="de833-2715">Enabled setting blob tier</span></span>
* <span data-ttu-id="de833-2716">Ajout des arguments `--bypass` et `--default-action` à `storage account [create|update]` pour la prise en charge du tunneling de service</span><span class="sxs-lookup"><span data-stu-id="de833-2716">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="de833-2717">Ajout de commandes permettant d’ajouter des règles de réseau virtuel et des règles basées sur IP à `storage account network-rule`</span><span class="sxs-lookup"><span data-stu-id="de833-2717">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="de833-2718">Activation du chiffrement du service par la clé gérée du client</span><span class="sxs-lookup"><span data-stu-id="de833-2718">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="de833-2719">[CHANGEMENT CASSANT] Renommage de l’option `--encryption` en `--encryption-services` pour la commande `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="de833-2719">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="de833-2720">Problème résolu #4220 : `az storage account update encryption` - incompatibilité de syntaxe</span><span class="sxs-lookup"><span data-stu-id="de833-2720">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="de833-2721">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="de833-2721">VM</span></span>

* <span data-ttu-id="de833-2722">Correction d’un problème qui entraînait l’affichage d’informations supplémentaires erronées pour `vmss get-instance-view` lors de l’utilisation `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="de833-2722">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="de833-2723">Ajout de la prise en charge de `--lb-sku` pour `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="de833-2723">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="de833-2724">Suppression des noms humains de la liste rouge du nom de l’administrateur pour `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="de833-2724">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="de833-2725">Correction d’un problème qui entraînait `[vm|vmss] create` la levée d’une erreur si la commande ne parvenait pas à extraire des informations de plan à partir d’une image</span><span class="sxs-lookup"><span data-stu-id="de833-2725">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="de833-2726">Correction d’un incident qui se produisait lors de la création d’un groupe identique VMMD avec un équilibrage de charge (LB) interne</span><span class="sxs-lookup"><span data-stu-id="de833-2726">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="de833-2727">Correction d’un problème qui empêchait `--no-wait` le fonctionnement d’un argument avec `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="de833-2727">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="de833-2728">15 août 2017</span><span class="sxs-lookup"><span data-stu-id="de833-2728">August 15, 2017</span></span>

<span data-ttu-id="de833-2729">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="de833-2729">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="de833-2730">ACS</span><span class="sxs-lookup"><span data-stu-id="de833-2730">ACS</span></span>

* <span data-ttu-id="de833-2731">Correction du numéro de port sshMaster0 pour kubernetes</span><span class="sxs-lookup"><span data-stu-id="de833-2731">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="de833-2732">AppService</span><span class="sxs-lookup"><span data-stu-id="de833-2732">Appservice</span></span>

* <span data-ttu-id="de833-2733">Correction d’une exception qui se produisait lors de la création d’une nouvelle application web Linux basée sur git</span><span class="sxs-lookup"><span data-stu-id="de833-2733">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="de833-2734">Event Grid</span><span class="sxs-lookup"><span data-stu-id="de833-2734">Event Grid</span></span>

* <span data-ttu-id="de833-2735">Ajout de dépendances du kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="de833-2735">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="de833-2736">11 août 2017</span><span class="sxs-lookup"><span data-stu-id="de833-2736">August 11, 2017</span></span>

<span data-ttu-id="de833-2737">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="de833-2737">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="de833-2738">ACS</span><span class="sxs-lookup"><span data-stu-id="de833-2738">ACS</span></span>

* <span data-ttu-id="de833-2739">Ajout de nouvelles régions d’aperçu</span><span class="sxs-lookup"><span data-stu-id="de833-2739">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="de833-2740">Batch</span><span class="sxs-lookup"><span data-stu-id="de833-2740">Batch</span></span>

* <span data-ttu-id="de833-2741">Mise à jour vers Kit de développement logiciel (DSK) de lot 3.1.0 et Kit de développement logiciel (SDK) de gestion de lot 4.1.0</span><span class="sxs-lookup"><span data-stu-id="de833-2741">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="de833-2742">Ajout d'une nouvelle commande affichant le nombre de tâches d’un travail</span><span class="sxs-lookup"><span data-stu-id="de833-2742">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="de833-2743">Correction du bogue dans le traitement de l’URL de la signature d'accès partagé du fichier de ressources</span><span class="sxs-lookup"><span data-stu-id="de833-2743">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="de833-2744">Point de terminaison de compte Batch prend désormais en charge le préfixe « https:// » facultatif</span><span class="sxs-lookup"><span data-stu-id="de833-2744">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="de833-2745">Prise en charge de l’ajout des listes de plus de 100 tâches à un travail</span><span class="sxs-lookup"><span data-stu-id="de833-2745">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="de833-2746">Ajout de l’enregistrement de débogage pour le chargement du module de commande Extensions</span><span class="sxs-lookup"><span data-stu-id="de833-2746">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="de833-2747">Composant</span><span class="sxs-lookup"><span data-stu-id="de833-2747">Component</span></span>

* <span data-ttu-id="de833-2748">Ajout d’un avertissement de désapprobation aux commandes « az component »</span><span class="sxs-lookup"><span data-stu-id="de833-2748">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="de833-2749">Conteneur</span><span class="sxs-lookup"><span data-stu-id="de833-2749">Container</span></span>

* <span data-ttu-id="de833-2750">`create`: correction d’un problème qui empêchait l’utilisation du signe égal à l’intérieur d’une variable d’environnement</span><span class="sxs-lookup"><span data-stu-id="de833-2750">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="de833-2751">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="de833-2751">Data Lake Store</span></span>

* <span data-ttu-id="de833-2752">Contrôle de progression activé</span><span class="sxs-lookup"><span data-stu-id="de833-2752">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="de833-2753">Event Grid</span><span class="sxs-lookup"><span data-stu-id="de833-2753">Event Grid</span></span>

* <span data-ttu-id="de833-2754">Version initiale</span><span class="sxs-lookup"><span data-stu-id="de833-2754">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="de833-2755">Réseau</span><span class="sxs-lookup"><span data-stu-id="de833-2755">Network</span></span>

* <span data-ttu-id="de833-2756">`lb`: correction d’un problème qui empêchait certains noms de ressources enfant d’être résolus correctement lorsqu’ils étaient omis</span><span class="sxs-lookup"><span data-stu-id="de833-2756">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="de833-2757">`application-gateway {subresource} delete`: correction d’un problème en raison duquel `--no-wait` n’était pas honorée</span><span class="sxs-lookup"><span data-stu-id="de833-2757">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="de833-2758">`application-gateway http-settings update`: correction d’un problème qui empêchait la désactivation de `--connection-draining-timeout`</span><span class="sxs-lookup"><span data-stu-id="de833-2758">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="de833-2759">Correction de erreur argument du mot-clé inattendu `sa_data_size_kilobyes` avec`az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="de833-2759">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="de833-2760">Profil</span><span class="sxs-lookup"><span data-stu-id="de833-2760">Profile</span></span>

* <span data-ttu-id="de833-2761">`account list`: ajout de `--refresh` pour synchroniser les derniers abonnements à partir du serveur</span><span class="sxs-lookup"><span data-stu-id="de833-2761">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="de833-2762">Stockage</span><span class="sxs-lookup"><span data-stu-id="de833-2762">Storage</span></span>

* <span data-ttu-id="de833-2763">Activer le compte de stockage de mise à jour avec l’identité attribuée par le système</span><span class="sxs-lookup"><span data-stu-id="de833-2763">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="de833-2764">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="de833-2764">VM</span></span>

* <span data-ttu-id="de833-2765">`availability-set`: nombre de domaines d’erreur exposés lors de la conversion</span><span class="sxs-lookup"><span data-stu-id="de833-2765">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="de833-2766">Commande `list-skus` exposée</span><span class="sxs-lookup"><span data-stu-id="de833-2766">Exposed `list-skus` command</span></span>
* <span data-ttu-id="de833-2767">Prise en charge pour affecter l’identité avec ou sans création d’attributions de rôle</span><span class="sxs-lookup"><span data-stu-id="de833-2767">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="de833-2768">Appliquer la référence (SKU) de stockage lors de l’attachement de disques de données</span><span class="sxs-lookup"><span data-stu-id="de833-2768">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="de833-2769">Suppression du nom du disque du système d’exploitation par défaut et de la référence (SKU) de stockage lors de l’utilisation des disques managés</span><span class="sxs-lookup"><span data-stu-id="de833-2769">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="de833-2770">28 juillet 2017</span><span class="sxs-lookup"><span data-stu-id="de833-2770">July 28, 2017</span></span>

<span data-ttu-id="de833-2771">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="de833-2771">Version 2.0.12</span></span>

* <span data-ttu-id="de833-2772">Ajout de commandes de conteneur</span><span class="sxs-lookup"><span data-stu-id="de833-2772">Added container commands</span></span>
* <span data-ttu-id="de833-2773">Ajout de modules de facturation et de consommation</span><span class="sxs-lookup"><span data-stu-id="de833-2773">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="de833-2774">Core</span><span class="sxs-lookup"><span data-stu-id="de833-2774">Core</span></span>

* <span data-ttu-id="de833-2775">Informations d’authentification du Kit de développement logiciel (SDK) de sortie pour les principaux de service avec des certificats</span><span class="sxs-lookup"><span data-stu-id="de833-2775">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="de833-2776">Correction des exceptions de progression de déploiement</span><span class="sxs-lookup"><span data-stu-id="de833-2776">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="de833-2777">Utiliser le point de terminaison ARM à partir du cloud actuel pour créer le client de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="de833-2777">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="de833-2778">Amélioration de la gestion simultanée de fichiers clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="de833-2778">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="de833-2779">Actualiser l’ID de la demande client pour chaque exécution de la commande</span><span class="sxs-lookup"><span data-stu-id="de833-2779">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="de833-2780">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel ( SDK) (#3635)</span><span class="sxs-lookup"><span data-stu-id="de833-2780">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="de833-2781">Rapports de progression pour les déploiements de modèle (#3510)</span><span class="sxs-lookup"><span data-stu-id="de833-2781">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="de833-2782">Ajout de la prise en charge des champs de sortie de la table de prélèvement via la requête jmespath (#3581)</span><span class="sxs-lookup"><span data-stu-id="de833-2782">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="de833-2783">Amélioration de la désactivation des arguments d’analyse et de l’historique Ajout avec des mouvements (#3434)</span><span class="sxs-lookup"><span data-stu-id="de833-2783">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="de833-2784">Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="de833-2784">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="de833-2785">Déplacer tous les fichiers d’enregistrement existant vers le dernier dossier</span><span class="sxs-lookup"><span data-stu-id="de833-2785">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="de833-2786">Correction de l’idempotence pour VM/VMSS create (#3586)</span><span class="sxs-lookup"><span data-stu-id="de833-2786">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="de833-2787">Les chemins d’accès de la commande ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="de833-2787">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="de833-2788">Certains paramètres de type booléen ne sont plus sensibles à la casse</span><span class="sxs-lookup"><span data-stu-id="de833-2788">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="de833-2789">Prise en charge de la connexion à ADFS sur le serveur local de manière identique à Azure Stack</span><span class="sxs-lookup"><span data-stu-id="de833-2789">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="de833-2790">Correction des écritures simultanées dans clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="de833-2790">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="de833-2791">ACR</span><span class="sxs-lookup"><span data-stu-id="de833-2791">ACR</span></span>

* <span data-ttu-id="de833-2792">Ajout de la commande `show-usage` pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="de833-2792">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="de833-2793">Prise en charge de la mise à jour de la référence (SKU) pour les registres gérés</span><span class="sxs-lookup"><span data-stu-id="de833-2793">Support SKU update for managed registries</span></span>
* <span data-ttu-id="de833-2794">Ajout de registres gérés avec la référence (SKU) gérée</span><span class="sxs-lookup"><span data-stu-id="de833-2794">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="de833-2795">Ajout de webhooks pour les registres gérés avec le module de commande acr webhook</span><span class="sxs-lookup"><span data-stu-id="de833-2795">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="de833-2796">Ajout de l’authentification AAD avec la commande de connexion acr</span><span class="sxs-lookup"><span data-stu-id="de833-2796">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="de833-2797">Ajout de la commande de suppression pour les référentiels docker, les manifestes et les balises</span><span class="sxs-lookup"><span data-stu-id="de833-2797">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="de833-2798">ACS</span><span class="sxs-lookup"><span data-stu-id="de833-2798">ACS</span></span>

* <span data-ttu-id="de833-2799">Prise en charge des API version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="de833-2799">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="de833-2800">AppService</span><span class="sxs-lookup"><span data-stu-id="de833-2800">Appservice</span></span>

* <span data-ttu-id="de833-2801">Correction d’un bogue à cause duquel l’énumération d’une application Linux ne retournait absolument rien</span><span class="sxs-lookup"><span data-stu-id="de833-2801">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="de833-2802">Prise en charge de la récupération de références depuis ACR</span><span class="sxs-lookup"><span data-stu-id="de833-2802">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="de833-2803">Supprimer toutes les commandes sous `appservice web`</span><span class="sxs-lookup"><span data-stu-id="de833-2803">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="de833-2804">Masquer les mots de passe du registre docker de la commande de sortie (#3656)</span><span class="sxs-lookup"><span data-stu-id="de833-2804">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="de833-2805">Vérifier que le navigateur par défaut est utilisé sur macOs sans erreurs (#3623)</span><span class="sxs-lookup"><span data-stu-id="de833-2805">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="de833-2806">Améliorer l’aide de `webapp log tail` et `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="de833-2806">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="de833-2807">Commandes `traffic-routing` exposées pour configurer le routage statique (#3566)</span><span class="sxs-lookup"><span data-stu-id="de833-2807">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="de833-2808">Ajout de correctifs de fiabilité pour la configuration du contrôle de code source (#3245)</span><span class="sxs-lookup"><span data-stu-id="de833-2808">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="de833-2809">Suppression d’un argument non pris en charge `--node-version` de `webapp config update` pour les applications Web de Windows.</span><span class="sxs-lookup"><span data-stu-id="de833-2809">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="de833-2810">Utilisez à la place `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="de833-2810">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="de833-2811">Batch</span><span class="sxs-lookup"><span data-stu-id="de833-2811">Batch</span></span>

* <span data-ttu-id="de833-2812">Mise à jour vers kit de développement logiciel (SDK) de lot 3.0.0 avec prise en charge pour les machines virtuelles de faible priorité dans des pools</span><span class="sxs-lookup"><span data-stu-id="de833-2812">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="de833-2813">Renommage `pool create` option `--target-dedicated` en `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="de833-2813">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="de833-2814">Ajout des options `pool create`, `--target-low-priority-nodes` et `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="de833-2814">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="de833-2815">CDN</span><span class="sxs-lookup"><span data-stu-id="de833-2815">CDN</span></span>

* <span data-ttu-id="de833-2816">Fourniture d’un meilleur message d’erreur pour `cdn endpoint list` quand le profil spécifié par `--profile-name` n’existe pas</span><span class="sxs-lookup"><span data-stu-id="de833-2816">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="de833-2817">Cloud</span><span class="sxs-lookup"><span data-stu-id="de833-2817">Cloud</span></span>

* <span data-ttu-id="de833-2818">Modification de la version de l’API du point de terminaison de métadonnées du cloud au format AAAA-MM-JJ</span><span class="sxs-lookup"><span data-stu-id="de833-2818">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="de833-2819">Le point de terminaison de la galerie n’est pas nécessaire</span><span class="sxs-lookup"><span data-stu-id="de833-2819">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="de833-2820">Prise en charge de l’inscription du cloud, avec le point de terminaison ARM resource manager</span><span class="sxs-lookup"><span data-stu-id="de833-2820">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="de833-2821">Ajout d’une option pour `cloud set` permettant de choisir le profil lors de la sélection du cloud actuel</span><span class="sxs-lookup"><span data-stu-id="de833-2821">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="de833-2822">Exposé `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="de833-2822">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="de833-2823">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="de833-2823">CosmosDB</span></span>

* <span data-ttu-id="de833-2824">Correction relative à la permission de la création de collection avec une clé de partition personnalisée</span><span class="sxs-lookup"><span data-stu-id="de833-2824">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="de833-2825">Ajout de la prise en charge de la durée de vie par défaut de la collection</span><span class="sxs-lookup"><span data-stu-id="de833-2825">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="de833-2826">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="de833-2826">Data Lake Analytics</span></span>

* <span data-ttu-id="de833-2827">Ajout de commandes pour la gestion de la stratégie de calcul sous le titre `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="de833-2827">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="de833-2828">Ajout de `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="de833-2828">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="de833-2829">Ajout de `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="de833-2829">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="de833-2830">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="de833-2830">Data Lake Store</span></span>

* <span data-ttu-id="de833-2831">Ajout de la prise en charge pour la rotation de coffre de clés gérés par l’utilisateur dans `dls account update`</span><span class="sxs-lookup"><span data-stu-id="de833-2831">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="de833-2832">Mise à jour de la version du kit de développement logiciel (SDK) du système de fichiers Data Lake Store sous-jacente, réglant un problème de performance</span><span class="sxs-lookup"><span data-stu-id="de833-2832">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="de833-2833">Ajout de la commande `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="de833-2833">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="de833-2834">Cette commande tente d’activer un utilisateur de coffre de clés fourni par l’utilisateur pour utiliser le chiffrement des données dans un compte Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="de833-2834">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="de833-2835">Interactive</span><span class="sxs-lookup"><span data-stu-id="de833-2835">Interactive</span></span>

* <span data-ttu-id="de833-2836">Amélioration du temps de démarrage à l’aide des commandes en cache</span><span class="sxs-lookup"><span data-stu-id="de833-2836">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="de833-2837">Couverture de test accrue</span><span class="sxs-lookup"><span data-stu-id="de833-2837">Increased test coverage</span></span>
* <span data-ttu-id="de833-2838">Amélioration du mouvement « ? » pour injecter également dans la commande suivante</span><span class="sxs-lookup"><span data-stu-id="de833-2838">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="de833-2839">Correction d’erreurs interactives avec le profil 2017-03-09-profil-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="de833-2839">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="de833-2840">Autorisé `--version` en tant que paramètre pour le mode interactif (#3645)</span><span class="sxs-lookup"><span data-stu-id="de833-2840">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="de833-2841">Empêche le mode interactif de lever des erreurs à partir des listes de saisie semi-automatique de validation (#3570)</span><span class="sxs-lookup"><span data-stu-id="de833-2841">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="de833-2842">Rapports de progression pour les déploiements de modèles (#3510)</span><span class="sxs-lookup"><span data-stu-id="de833-2842">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="de833-2843">Ajout de l’indicateur `--progress`</span><span class="sxs-lookup"><span data-stu-id="de833-2843">Added `--progress` flag</span></span>
* <span data-ttu-id="de833-2844">Suppression `--debug` et `--verbose` des listes de saisie semi-automatique</span><span class="sxs-lookup"><span data-stu-id="de833-2844">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="de833-2845">Suppression `interactive` des listes de saisie semi-automatique (#3324)</span><span class="sxs-lookup"><span data-stu-id="de833-2845">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="de833-2846">IoT</span><span class="sxs-lookup"><span data-stu-id="de833-2846">IoT</span></span>

* <span data-ttu-id="de833-2847">La création de la stratégie n’efface plus les stratégies existantes.</span><span class="sxs-lookup"><span data-stu-id="de833-2847">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="de833-2848">(#3934)</span><span class="sxs-lookup"><span data-stu-id="de833-2848">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="de833-2849">Coffre de clés</span><span class="sxs-lookup"><span data-stu-id="de833-2849">Key vault</span></span>

* <span data-ttu-id="de833-2850">Ajout de commandes pour les fonctionnalités de récupération de coffre de clés :</span><span class="sxs-lookup"><span data-stu-id="de833-2850">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="de833-2851">`keyvault`sous-commandes `purge`, `recover`,`keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="de833-2851">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="de833-2852">`keyvault secret`sous-commandes `backup`, `restore`, `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="de833-2852">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="de833-2853">`keyvault certificate`sous-commandes `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="de833-2853">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="de833-2854">`keyvault key`sous-commandes `purge`, `recover`,`list-deleted`</span><span class="sxs-lookup"><span data-stu-id="de833-2854">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="de833-2855">Ajout de l’intégration du coffre de clés du principal du service (#3133)</span><span class="sxs-lookup"><span data-stu-id="de833-2855">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="de833-2856">Mise à jour du plan de données du coffre de clés vers 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="de833-2856">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="de833-2857">(#3307)</span><span class="sxs-lookup"><span data-stu-id="de833-2857">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="de833-2858">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="de833-2858">Lab</span></span>

* <span data-ttu-id="de833-2859">Ajout de la prise en charge de la revendication de toutes les machines virtuelles dans le laboratoire via `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="de833-2859">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="de833-2860">Ajout du formateur de sortie de tableau pour `az lab vm list` et `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="de833-2860">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="de833-2861">Moniteur</span><span class="sxs-lookup"><span data-stu-id="de833-2861">Monitor</span></span>

* <span data-ttu-id="de833-2862">Correctif pour le fichier de modèle avec `monitor autoscale-settings get-parameters-template` commande (#3349)</span><span class="sxs-lookup"><span data-stu-id="de833-2862">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="de833-2863">`monitor alert-rule-incidents list` renommé en `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="de833-2863">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="de833-2864">`monitor alert-rule-incidents show` renommé en `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="de833-2864">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="de833-2865">`monitor metric-defintions list` renommé en `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="de833-2865">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="de833-2866">`monitor alert-rules` renommé en `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="de833-2866">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="de833-2867">Modifié `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="de833-2867">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="de833-2868">sous-commandes`condition` et `action` n’acceptent plus JSON</span><span class="sxs-lookup"><span data-stu-id="de833-2868">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="de833-2869">Ajout de nombreux paramètres simplifiant le processus de création de règle</span><span class="sxs-lookup"><span data-stu-id="de833-2869">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="de833-2870">`location` n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="de833-2870">`location` no longer required</span></span>
  * <span data-ttu-id="de833-2871">Ajout d’un nom et de la prise en charge de l’ID de la cible</span><span class="sxs-lookup"><span data-stu-id="de833-2871">Add name and ID support for target</span></span>
  * <span data-ttu-id="de833-2872">Suppression de `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="de833-2872">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="de833-2873">Le renommage de `is-enabled` en `enabled`n’est plus nécessaire</span><span class="sxs-lookup"><span data-stu-id="de833-2873">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="de833-2874">`description` par défaut sont désormais basées sur la condition fournie</span><span class="sxs-lookup"><span data-stu-id="de833-2874">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="de833-2875">Ajout d’exemples aidant à clarifier le nouveau format</span><span class="sxs-lookup"><span data-stu-id="de833-2875">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="de833-2876">Prise en charge des noms ou des ID pour les commandes `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="de833-2876">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="de833-2877">Ajout d’arguments d’usage et d’exemples pour `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="de833-2877">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="de833-2878">Réseau</span><span class="sxs-lookup"><span data-stu-id="de833-2878">Network</span></span>

* <span data-ttu-id="de833-2879">Ajout de la commande `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="de833-2879">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="de833-2880">Ajout de l’argument `--private-access-services` à `vnet subnet create` et `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="de833-2880">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="de833-2881">Correction d’un problème `application-gateway redirect-config create` qui causait l’échec de</span><span class="sxs-lookup"><span data-stu-id="de833-2881">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="de833-2882">Correction d’un problème `application-gateway redirect-config update` qui `--no-wait` empêchait le fonctionnement de</span><span class="sxs-lookup"><span data-stu-id="de833-2882">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="de833-2883">Correction d’un bogue lié à l’utilisation d’un `--servers` argument avec `application-gateway address-pool create` et `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="de833-2883">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="de833-2884">Ajout des commandes `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="de833-2884">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="de833-2885">Ajout de commandes à `application-gateway ssl-policy` : `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="de833-2885">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="de833-2886">Ajout d’arguments à `application-gateway ssl-policy set` : `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="de833-2886">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="de833-2887">Ajout d’arguments à `application-gateway http-settings create` et `application-gateway http-settings update` : `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="de833-2887">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="de833-2888">Ajout d’arguments à `application-gateway url-path-map create` et `application-gateway url-path-map update`, `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="de833-2888">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="de833-2889">Ajout d’un argument `--redirect-config` à `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="de833-2889">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="de833-2890">Ajout de la prise en charge de `--no-wait` pour `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="de833-2890">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="de833-2891">Ajout d’arguments à `application-gateway probe create` et `application-gateway probe update` : `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="de833-2891">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="de833-2892">Ajout d’un argument `--redirect-config` à `application-gateway rule create` et `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="de833-2892">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="de833-2893">Ajout de la prise en charge de `--accelerated-networking` pour `nic create` et `nic update`</span><span class="sxs-lookup"><span data-stu-id="de833-2893">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="de833-2894">Suppression de l’ `--internal-dns-name-suffix` argument à partir de `nic create`</span><span class="sxs-lookup"><span data-stu-id="de833-2894">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="de833-2895">Ajout de la prise en charge de `--dns-servers` pour `nic update` et `nic create` : ajout de la prise en charge de --dns-servers</span><span class="sxs-lookup"><span data-stu-id="de833-2895">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="de833-2896">Correction d’un bogue qui faisait `local-gateway create` ignorer `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="de833-2896">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="de833-2897">Ajout de la prise en charge de `--dns-servers` pour `vnet update`</span><span class="sxs-lookup"><span data-stu-id="de833-2897">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="de833-2898">Correction d’un bogue lors de la création d’un peering sans filtrage de l’itinéraire avec `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="de833-2898">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="de833-2899">Correction d’un bogue qui empêchait le fonctionnement des arguments `--provider` et `--bandwidth` avec `express-route update`</span><span class="sxs-lookup"><span data-stu-id="de833-2899">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="de833-2900">Correction d’un bogue avec `network watcher show-topology` une logique de valeurs par défaut</span><span class="sxs-lookup"><span data-stu-id="de833-2900">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="de833-2901">Amélioration de la mise en forme de sortie pour `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="de833-2901">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="de833-2902">Utilisation de l’IP frontale par défaut pour `application-gateway http-listener create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="de833-2902">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="de833-2903">Utilisation d’un pool d’adresses par défaut, des paramètres HTTP et de l’écouteur HTTP pour `application-gateway rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="de833-2903">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="de833-2904">Utilisation de l’IP frontale par défaut et du pool principal `lb rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="de833-2904">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="de833-2905">Utilisation de l’IP frontale par défaut pour `lb inbound-nat-rule create` s’il n’en existe qu’une seule</span><span class="sxs-lookup"><span data-stu-id="de833-2905">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="de833-2906">Profil</span><span class="sxs-lookup"><span data-stu-id="de833-2906">Profile</span></span>

* <span data-ttu-id="de833-2907">Prise en charge de la connexion à l’intérieur d’une machine virtuelle avec une identité gérée</span><span class="sxs-lookup"><span data-stu-id="de833-2907">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="de833-2908">Prise en charge de la sortie pour `account show` au format de fichier d’authentification du Kit de développement logiciel (SDK)</span><span class="sxs-lookup"><span data-stu-id="de833-2908">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="de833-2909">Affichage des avertissements de désapprobation lors de l’utilisation de '--expanded-view'</span><span class="sxs-lookup"><span data-stu-id="de833-2909">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="de833-2910">Ajout de la commande `get-access-token` permettant de fournir un jeton AAD brut</span><span class="sxs-lookup"><span data-stu-id="de833-2910">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="de833-2911">Prise en charge de la connexion avec un compte d’utilisateur sans abonnements associés</span><span class="sxs-lookup"><span data-stu-id="de833-2911">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="de833-2912">SGBDR</span><span class="sxs-lookup"><span data-stu-id="de833-2912">RDBMS</span></span>

* <span data-ttu-id="de833-2913">Prise en charge de l’énumération de serveurs à travers un abonnement (#3417)</span><span class="sxs-lookup"><span data-stu-id="de833-2913">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="de833-2914">Correction de `%s` non traité car il manque `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="de833-2914">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="de833-2915">Correction du mappage de la source du document et ajout de la tâche CI permettant la vérification de (#3361)</span><span class="sxs-lookup"><span data-stu-id="de833-2915">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="de833-2916">Correction concernant l’aide relative à MySQL et PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="de833-2916">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="de833-2917">Ressource</span><span class="sxs-lookup"><span data-stu-id="de833-2917">Resource</span></span>

* <span data-ttu-id="de833-2918">Amélioration des invites pour les paramètres manquants de `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="de833-2918">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="de833-2919">Amélioration de l’analyse de `--parameters KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="de833-2919">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="de833-2920">Correction des problèmes à cause desquels `group deployment create` les fichiers de paramètres n’étaient plus reconnus à l’aide de la `@<file>` syntaxe</span><span class="sxs-lookup"><span data-stu-id="de833-2920">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="de833-2921">Prise en charge de l’ `--ids` argument pour `resource` et `managedapp` les commandes</span><span class="sxs-lookup"><span data-stu-id="de833-2921">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="de833-2922">Correction de certains messages d’analyse et d’erreur (#3584)</span><span class="sxs-lookup"><span data-stu-id="de833-2922">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="de833-2923">Correction de l’analyse `--resource-type` permettant à la `lock` commande d’accepter `<resource-namespace>` et `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="de833-2923">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="de833-2924">Ajout de la vérification de paramètre des modèles de liaison de modèle (#3629)</span><span class="sxs-lookup"><span data-stu-id="de833-2924">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="de833-2925">Ajout de la prise en charge de la spécification des paramètres de déploiement à l’aide de la `KEY=VALUE` syntaxe</span><span class="sxs-lookup"><span data-stu-id="de833-2925">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="de833-2926">Role</span><span class="sxs-lookup"><span data-stu-id="de833-2926">Role</span></span>

* <span data-ttu-id="de833-2927">Prise en charge de la sortie au format de fichier d’authentification du Kit de développement logiciel (SDK) pour `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="de833-2927">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="de833-2928">Nettoyage des attributions de rôles et de l’application AAD liée lors de la suppression d’un principal de service (#3610)</span><span class="sxs-lookup"><span data-stu-id="de833-2928">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="de833-2929">Inclusion du format d’heure dans `app create` args `--start-date` et `--end-date` descriptions</span><span class="sxs-lookup"><span data-stu-id="de833-2929">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="de833-2930">Affichage des avertissements de désapprobation lors de l’utilisation de `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="de833-2930">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="de833-2931">Ajout de l’intégration du coffre de clés pour les commandes `create-for-rbac` et `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="de833-2931">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="de833-2932">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="de833-2932">Service Fabric</span></span>
* <span data-ttu-id="de833-2933">Correction d’un problème avec les fichiers volumineux dans les applications tronquées sur le chargement (#3666)</span><span class="sxs-lookup"><span data-stu-id="de833-2933">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="de833-2934">Ajout de tests pour les commandes Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="de833-2934">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="de833-2935">Correction de nombreuses commandes Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="de833-2935">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="de833-2936">SQL</span><span class="sxs-lookup"><span data-stu-id="de833-2936">SQL</span></span>

* <span data-ttu-id="de833-2937">Suppression du paramètre `sql server create` `--identity` rompu</span><span class="sxs-lookup"><span data-stu-id="de833-2937">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="de833-2938">Suppression des valeurs de mot de passe à partir de la sortie de commande `sql server create` et `sql server update`</span><span class="sxs-lookup"><span data-stu-id="de833-2938">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="de833-2939">Ajout des commandes `sql db list-editions` et `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="de833-2939">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="de833-2940">Stockage</span><span class="sxs-lookup"><span data-stu-id="de833-2940">Storage</span></span>

* <span data-ttu-id="de833-2941">Suppression d’une `--marker` option à partir des commandes `storage blob list`, `storage container list`et `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="de833-2941">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="de833-2942">Activation de la création d’un compte de stockage https-only</span><span class="sxs-lookup"><span data-stu-id="de833-2942">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="de833-2943">Mise à jour des métriques de stockage, de la journalisation et des commandes cors (#3495)</span><span class="sxs-lookup"><span data-stu-id="de833-2943">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="de833-2944">Reformulation d’un message d’exception de l’ajout CORS (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="de833-2944">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="de833-2945">Conversion du générateur à une liste en mode exécution d’essai de la commande de téléchargement de lot (#3592)</span><span class="sxs-lookup"><span data-stu-id="de833-2945">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="de833-2946">Correction du problème d’essai associé au lot de téléchargement du blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="de833-2946">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="de833-2947">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="de833-2947">VM</span></span>

* <span data-ttu-id="de833-2948">Prise en charge de la configuration du groupe de sécurité réseau</span><span class="sxs-lookup"><span data-stu-id="de833-2948">Support configuring nsg</span></span>
* <span data-ttu-id="de833-2949">Correction d’un bogue qui entraînait une configuration incorrecte du serveur DNS</span><span class="sxs-lookup"><span data-stu-id="de833-2949">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="de833-2950">Prise en charge des identités de service géré</span><span class="sxs-lookup"><span data-stu-id="de833-2950">Support managed service identities</span></span>
* <span data-ttu-id="de833-2951">Correction d’un problème à cause duquel `cmss create` avec un équilibreur de charge existant exigeait `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="de833-2951">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="de833-2952">Les disques de données créés avec le numéro d’unité logique `vm image create` commencent à 0</span><span class="sxs-lookup"><span data-stu-id="de833-2952">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="de833-2953">10 mai 2017</span><span class="sxs-lookup"><span data-stu-id="de833-2953">May 10, 2017</span></span>

<span data-ttu-id="de833-2954">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="de833-2954">Version 2.0.6</span></span>

* <span data-ttu-id="de833-2955">documentdb renommé en cosmosdb</span><span class="sxs-lookup"><span data-stu-id="de833-2955">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="de833-2956">Ajouter rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="de833-2956">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="de833-2957">Inclure les modules Data Lake Analytics et Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="de833-2957">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="de833-2958">Inclure le module Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="de833-2958">Include Cognitive Services module</span></span>
* <span data-ttu-id="de833-2959">Inclure le module Service Fabric</span><span class="sxs-lookup"><span data-stu-id="de833-2959">Include Service Fabric module</span></span>
* <span data-ttu-id="de833-2960">Inclure le module Interactive (az-shell renommé)</span><span class="sxs-lookup"><span data-stu-id="de833-2960">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="de833-2961">Ajouter la prise en charge des commandes CDN</span><span class="sxs-lookup"><span data-stu-id="de833-2961">Add support for CDN commands</span></span>
* <span data-ttu-id="de833-2962">Supprimer le module Container</span><span class="sxs-lookup"><span data-stu-id="de833-2962">Remove Container module</span></span>
* <span data-ttu-id="de833-2963">Ajouter « az -v » comme raccourci pour « az --version » ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="de833-2963">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="de833-2964">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="de833-2964">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="de833-2965">Core</span><span class="sxs-lookup"><span data-stu-id="de833-2965">Core</span></span>

* <span data-ttu-id="de833-2966">principal : capturer les exceptions provoquées par un fournisseur non enregistré et l’enregistrer automatiquement</span><span class="sxs-lookup"><span data-stu-id="de833-2966">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="de833-2967">performance : conserver le cache de jeton adal en mémoire jusqu’à la fin du processus ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="de833-2967">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="de833-2968">Corriger les octets retournés par l’empreinte digitale hex -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="de833-2968">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="de833-2969">Téléchargement du certificat Key Vault et intégration AAD SP améliorés ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="de833-2969">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="de833-2970">Ajouter l’emplacement de Python à « az —version » ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="de833-2970">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="de833-2971">connexion : prise en charge de la connexion lorsqu’il n’y a aucun abonnement ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="de833-2971">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="de833-2972">principal : corriger une erreur lors de la connexion à l’aide d’un principal de service deux fois ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="de833-2972">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="de833-2973">principal : autoriser la configuration du chemin d’accès d’accessTokens.json via une variable d’environnement ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="de833-2973">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="de833-2974">principal : autoriser l’application des valeurs par défaut configurées sur les arguments facultatifs ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="de833-2974">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="de833-2975">principal : performances améliorées</span><span class="sxs-lookup"><span data-stu-id="de833-2975">core: Improved performance</span></span>
* <span data-ttu-id="de833-2976">principal : certificats d’autorité de certification personnalisés, prise en charge de la définition de la variable d’environnement REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="de833-2976">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="de833-2977">principal : configuration du cloud, utiliser le point de terminaison « resource manager » si le point de terminaison « management » n’est pas défini</span><span class="sxs-lookup"><span data-stu-id="de833-2977">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="de833-2978">ACS</span><span class="sxs-lookup"><span data-stu-id="de833-2978">ACS</span></span>

* <span data-ttu-id="de833-2979">corriger le nombre de maîtres et d’agents sur un nombre entier au lieu d’une chaîne</span><span class="sxs-lookup"><span data-stu-id="de833-2979">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="de833-2980">exposer « az acs create --no-wait » et « az acs wait » pour la création asynchrone</span><span class="sxs-lookup"><span data-stu-id="de833-2980">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="de833-2981">exposer « az acs create --validate » pour les validations de test</span><span class="sxs-lookup"><span data-stu-id="de833-2981">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="de833-2982">supprimer le profil Windows avant l’appel PUT pour la commande de mise à l’échelle ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="de833-2982">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="de833-2983">AppService</span><span class="sxs-lookup"><span data-stu-id="de833-2983">AppService</span></span>

* <span data-ttu-id="de833-2984">functionapp : ajouter la prise en charge complète de functionapp, notamment créer, afficher, liste, supprimer, nom d’hôte, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="de833-2984">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="de833-2985">Ajout de Team Services (vsts) comme option de livraison continue à « config contrôle source web appservice »</span><span class="sxs-lookup"><span data-stu-id="de833-2985">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="de833-2986">Créer « az webapp » pour remplacer « az appservice web » (pour la rétrocompatibilité, « az appservice web » sera conservé dans les 2 prochaines versions)</span><span class="sxs-lookup"><span data-stu-id="de833-2986">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="de833-2987">Exposer des arguments pour configurer le déploiement et des « piles d’exécution » sur webapp create</span><span class="sxs-lookup"><span data-stu-id="de833-2987">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="de833-2988">Exposer « webapp list-runtimes »</span><span class="sxs-lookup"><span data-stu-id="de833-2988">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="de833-2989">prendre en charge la configuration des chaînes de connexion ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="de833-2989">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="de833-2990">prendre en charge le basculement d’emplacement avec aperçu</span><span class="sxs-lookup"><span data-stu-id="de833-2990">support slot swap with preview</span></span>
* <span data-ttu-id="de833-2991">Supprimer les erreurs des commandes appservice ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="de833-2991">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="de833-2992">Utiliser le groupe de ressources du plan app service pour les opérations de certificat ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="de833-2992">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="de833-2993">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="de833-2993">CosmosDB</span></span>

* <span data-ttu-id="de833-2994">Renommer le module documentdb en cosmosdb</span><span class="sxs-lookup"><span data-stu-id="de833-2994">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="de833-2995">Prise en charge ajoutée pour les API de plan de données documentdb : gestion de base de données et de collecte</span><span class="sxs-lookup"><span data-stu-id="de833-2995">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="de833-2996">Prise en charge ajoutée pour activer le basculement automatique sur les comptes de base de données</span><span class="sxs-lookup"><span data-stu-id="de833-2996">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="de833-2997">Prise en charge ajoutée pour la nouvelle stratégie de cohérence ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="de833-2997">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="de833-2998">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="de833-2998">Data Lake Analytics</span></span>

* <span data-ttu-id="de833-2999">Corriger un bogue dans lequel le filtrage sur le résultat et l’état des listes de travaux lève une erreur</span><span class="sxs-lookup"><span data-stu-id="de833-2999">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="de833-3000">Ajouter la prise en charge d’un nouveau type d’élément de catalogue : paquet.</span><span class="sxs-lookup"><span data-stu-id="de833-3000">Add support for new catalog item type: package.</span></span> <span data-ttu-id="de833-3001">accessible via : `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="de833-3001">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="de833-3002">A rendu possible le fait de répertorier les éléments de catalogue suivants à partir d’une base de données (aucune spécification de schéma requise) :</span><span class="sxs-lookup"><span data-stu-id="de833-3002">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="de833-3003">Table de charge de travail</span><span class="sxs-lookup"><span data-stu-id="de833-3003">Table</span></span>
  * <span data-ttu-id="de833-3004">Fonction table</span><span class="sxs-lookup"><span data-stu-id="de833-3004">Table valued function</span></span>
  * <span data-ttu-id="de833-3005">Affichage</span><span class="sxs-lookup"><span data-stu-id="de833-3005">View</span></span>
  * <span data-ttu-id="de833-3006">Statistiques de table.</span><span class="sxs-lookup"><span data-stu-id="de833-3006">Table Statistics.</span></span> <span data-ttu-id="de833-3007">Cela peut également être répertorié avec un schéma, mais sans spécifier un nom de table</span><span class="sxs-lookup"><span data-stu-id="de833-3007">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="de833-3008">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="de833-3008">Data Lake Store</span></span>

* <span data-ttu-id="de833-3009">Mettre à jour la version du Kit de développement logiciel (SDK) du système de fichiers sous-jacent, qui offre une meilleure prise en charge pour gérer les scénarios de limitation côté serveur</span><span class="sxs-lookup"><span data-stu-id="de833-3009">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="de833-3010">Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="de833-3010">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="de833-3011">aide manquante pour afficher l’accès.</span><span class="sxs-lookup"><span data-stu-id="de833-3011">missed help for access show.</span></span> <span data-ttu-id="de833-3012">ajout en cours.</span><span class="sxs-lookup"><span data-stu-id="de833-3012">adding it.</span></span> <span data-ttu-id="de833-3013">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="de833-3013">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="de833-3014">Rechercher</span><span class="sxs-lookup"><span data-stu-id="de833-3014">Find</span></span>

* <span data-ttu-id="de833-3015">résultats de la recherche améliorés et autorisation du contrôle de version de l’index de recherche</span><span class="sxs-lookup"><span data-stu-id="de833-3015">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="de833-3016">KeyVault</span><span class="sxs-lookup"><span data-stu-id="de833-3016">KeyVault</span></span>

* <span data-ttu-id="de833-3017">BC : `az keyvault certificate download` remplacer -e dans chaîne ou élément binaire par PEM ou DER afin de mieux représenter les options</span><span class="sxs-lookup"><span data-stu-id="de833-3017">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="de833-3018">BC : supprimer --expires et --not-before dans `keyvault certificate create`, car ces paramètres ne sont pas pris en charge par le service</span><span class="sxs-lookup"><span data-stu-id="de833-3018">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="de833-3019">Ajoute le paramètre --validity à `keyvault certificate create` pour substituer de manière sélective la valeur dans --policy</span><span class="sxs-lookup"><span data-stu-id="de833-3019">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="de833-3020">Résout le problème dans `keyvault certificate get-default-policy` où « expires » et « not_before » étaient exposés mais « validity_in_months » ne l’était pas</span><span class="sxs-lookup"><span data-stu-id="de833-3020">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="de833-3021">correction de keyvault pour l’importation de pem et pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="de833-3021">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="de833-3022">Laboratoire</span><span class="sxs-lookup"><span data-stu-id="de833-3022">Lab</span></span>

* <span data-ttu-id="de833-3023">Ajout des commandes créer, afficher, supprimer et liste pour l’environnement dans le laboratoire</span><span class="sxs-lookup"><span data-stu-id="de833-3023">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="de833-3024">Ajout des commandes afficher et liste pour afficher les modèles ARM dans le laboratoire</span><span class="sxs-lookup"><span data-stu-id="de833-3024">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="de833-3025">Ajout de l’indicateur --environment dans `az lab vm list` pour filtrer les machines virtuelles selon l’environnement du laboratoire</span><span class="sxs-lookup"><span data-stu-id="de833-3025">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="de833-3026">Ajout de la commande pratique `az lab formula export-artifacts` pour exporter une structure d’artefact dans une formule de laboratoire</span><span class="sxs-lookup"><span data-stu-id="de833-3026">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="de833-3027">Ajout de commandes pour gérer les secrets dans un laboratoire</span><span class="sxs-lookup"><span data-stu-id="de833-3027">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="de833-3028">Moniteur</span><span class="sxs-lookup"><span data-stu-id="de833-3028">Monitor</span></span>

* <span data-ttu-id="de833-3029">Résolution de bogue : modélisation de `--actions` de `az alert-rules create` pour consommer la chaîne JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="de833-3029">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="de833-3030">Correction de bogue : la création de paramètres de diagnostic n’accepte pas les métriques/journaux à partir des commandes d’affichage ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="de833-3030">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="de833-3031">Réseau</span><span class="sxs-lookup"><span data-stu-id="de833-3031">Network</span></span>

* <span data-ttu-id="de833-3032">Ajouter la commande `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="de833-3032">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="de833-3033">Ajouter la prise en charge du paramètre `--filters` pour `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="de833-3033">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="de833-3034">Ajouter la prise en charge pour le drainage de connexion Application Gateway</span><span class="sxs-lookup"><span data-stu-id="de833-3034">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="de833-3035">Ajouter la prise en charge pour la configuration du jeu de règles WAF d’Application Gateway</span><span class="sxs-lookup"><span data-stu-id="de833-3035">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="de833-3036">Ajouter la prise en charge des règles et des filtres de routage ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="de833-3036">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="de833-3037">Ajouter la prise en charge pour le routage géographique TrafficManager</span><span class="sxs-lookup"><span data-stu-id="de833-3037">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="de833-3038">Ajouter la prise en charge des sélecteurs de trafic basés sur la stratégie de connexion VPN</span><span class="sxs-lookup"><span data-stu-id="de833-3038">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="de833-3039">Ajouter la prise en charge pour les stratégies IPSec de la connexion VPN</span><span class="sxs-lookup"><span data-stu-id="de833-3039">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="de833-3040">Corriger le bogue avec `vpn-connection create` lors de l’utilisation des paramètres `--no-wait` ou `--validate`</span><span class="sxs-lookup"><span data-stu-id="de833-3040">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="de833-3041">Ajouter la prise en charge des passerelles de réseau virtuel actif-actif</span><span class="sxs-lookup"><span data-stu-id="de833-3041">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="de833-3042">Supprimer les valeurs NULL de la sortie des commandes `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="de833-3042">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="de833-3043">BC : résoudre un bogue dans la sortie de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="de833-3043">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="de833-3044">Corriger le bogue où l’argument « --key-length » de « vpn-connection create » n’était pas analysé correctement</span><span class="sxs-lookup"><span data-stu-id="de833-3044">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="de833-3045">Corriger le bogue dans `dns zone import` où les enregistrements n’étaient pas été importés correctement</span><span class="sxs-lookup"><span data-stu-id="de833-3045">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="de833-3046">Corriger le bogue où `traffic-manager endpoint update` ne fonctionnait pas</span><span class="sxs-lookup"><span data-stu-id="de833-3046">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="de833-3047">Ajouter des commandes d’aperçu « network watcher »</span><span class="sxs-lookup"><span data-stu-id="de833-3047">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="de833-3048">Profil</span><span class="sxs-lookup"><span data-stu-id="de833-3048">Profile</span></span>

* <span data-ttu-id="de833-3049">Prendre en charge la connexion lorsqu’il n’y a aucun abonnement trouvé ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="de833-3049">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="de833-3050">Prendre en charge un nom de paramètre court dans le jeu de comptes az --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="de833-3050">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="de833-3051">Redis</span><span class="sxs-lookup"><span data-stu-id="de833-3051">Redis</span></span>

* <span data-ttu-id="de833-3052">Ajout d’une commande de mise à jour qui ajoute également la possibilité de mettre à l’échelle pour le cache redis</span><span class="sxs-lookup"><span data-stu-id="de833-3052">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="de833-3053">Commande « update-settings » déconseillée</span><span class="sxs-lookup"><span data-stu-id="de833-3053">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="de833-3054">Ressource</span><span class="sxs-lookup"><span data-stu-id="de833-3054">Resource</span></span>

* <span data-ttu-id="de833-3055">Ajouter managedapp et les commandes de définition managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="de833-3055">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="de833-3056">Prendre en charge les commandes « provider operation » ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="de833-3056">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="de833-3057">Prendre en charge la création de ressource générique ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="de833-3057">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="de833-3058">Corriger l’analyse de ressource et la recherche de version d’API.</span><span class="sxs-lookup"><span data-stu-id="de833-3058">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="de833-3059">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="de833-3059">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="de833-3060">Ajouter des documents pour mise à jour du verrou az.</span><span class="sxs-lookup"><span data-stu-id="de833-3060">Add docs for az lock update.</span></span> <span data-ttu-id="de833-3061">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="de833-3061">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="de833-3062">Sortie d’erreur si vous essayez de lister des ressources pour un groupe qui n’existe pas.</span><span class="sxs-lookup"><span data-stu-id="de833-3062">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="de833-3063">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="de833-3063">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="de833-3064">[Compute] Résoudre les problèmes de mise à jour de VMSS et du groupe à haute disponibilité de machines virtuelles.</span><span class="sxs-lookup"><span data-stu-id="de833-3064">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="de833-3065">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="de833-3065">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="de833-3066">Corriger le verrouillage des commandes créer et supprimer si parent-resource-path est None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="de833-3066">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="de833-3067">Role</span><span class="sxs-lookup"><span data-stu-id="de833-3067">Role</span></span>

* <span data-ttu-id="de833-3068">create-for-rbac : vérifier que la date de fin du SP ne dépassera pas la date d’expiration du certificat ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="de833-3068">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="de833-3069">RBAC : ajouter la prise en charge complète de « ad group » ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="de833-3069">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="de833-3070">rôle : résoudre les problèmes de mise à jour de définition de rôle ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="de833-3070">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="de833-3071">create-for-rbac : vérifier que le mot de passe fourni par l’utilisateur est accepté</span><span class="sxs-lookup"><span data-stu-id="de833-3071">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="de833-3072">SQL</span><span class="sxs-lookup"><span data-stu-id="de833-3072">SQL</span></span>

* <span data-ttu-id="de833-3073">Ajout des commandes az sql server list-usages et az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="de833-3073">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="de833-3074">SQL : possibilité de se connecter directement au fournisseur de ressources ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="de833-3074">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="de833-3075">Stockage</span><span class="sxs-lookup"><span data-stu-id="de833-3075">Storage</span></span>

* <span data-ttu-id="de833-3076">Définir l’emplacement par défaut sur l’emplacement du groupe de ressources pour `storage account create`</span><span class="sxs-lookup"><span data-stu-id="de833-3076">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="de833-3077">Ajouter la prise en charge de la copie incrémentielle d’objet blob</span><span class="sxs-lookup"><span data-stu-id="de833-3077">Add support for incremental blob copy</span></span>
* <span data-ttu-id="de833-3078">Ajouter la prise en charge du chargement d’objet blob de blocs volumineux</span><span class="sxs-lookup"><span data-stu-id="de833-3078">Add support for large block blob upload</span></span>
* <span data-ttu-id="de833-3079">Modifier la taille de bloc à 100 Mo lorsque le fichier à charger est supérieur à 200 Go</span><span class="sxs-lookup"><span data-stu-id="de833-3079">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="de833-3080">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="de833-3080">VM</span></span>

* <span data-ttu-id="de833-3081">avail-set : rendre le compte de domaine UD&FD facultatif</span><span class="sxs-lookup"><span data-stu-id="de833-3081">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="de833-3082">Remarque : commandes de machine virtuelle dans clouds souverains. Veuillez éviter les fonctionnalités liées au disque managé, notamment :</span><span class="sxs-lookup"><span data-stu-id="de833-3082">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="de833-3083">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="de833-3083">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="de833-3084">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="de833-3084">az vm/vmss disk</span></span>
  3. <span data-ttu-id="de833-3085">Dans « az vm/vmss create », utiliser « —use-unmanaged-disk » pour éviter le disque managé Les autres commandes devraient fonctionner</span><span class="sxs-lookup"><span data-stu-id="de833-3085">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="de833-3086">vm/vmss : améliorer le texte d’avertissement lors de la génération de paires de clés ssh</span><span class="sxs-lookup"><span data-stu-id="de833-3086">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="de833-3087">vm/vmss : prendre en charge la création à partir d’une image de la Place de marché qui requiert des informations sur le plan ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="de833-3087">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="de833-3088">3 avril 2017</span><span class="sxs-lookup"><span data-stu-id="de833-3088">April 3, 2017</span></span>

<span data-ttu-id="de833-3089">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="de833-3089">Version 2.0.2</span></span>

<span data-ttu-id="de833-3090">Nous avons publié les composants ACR, Batch, KeyVault et SQL dans cette version</span><span class="sxs-lookup"><span data-stu-id="de833-3090">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="de833-3091">Core</span><span class="sxs-lookup"><span data-stu-id="de833-3091">Core</span></span>

* <span data-ttu-id="de833-3092">Ajout des modules acr, lab, monitor et find à la liste par défaut</span><span class="sxs-lookup"><span data-stu-id="de833-3092">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="de833-3093">Connexion : ignorer les locataires erronés ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="de833-3093">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="de833-3094">login : définition de l’abonnement par défaut à la valeur « un » avec l’état « Activé » ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="de833-3094">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="de833-3095">Ajout de la prise en charge des commandes wait et de --no-wait à davantage de commandes ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="de833-3095">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="de833-3096">core : prise en charge de la connexion à l’aide du principal du service avec un certificat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="de833-3096">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="de833-3097">Ajout d’une invite pour les paramètres de modèle manquants.</span><span class="sxs-lookup"><span data-stu-id="de833-3097">Add prompting for missing template parameters.</span></span> <span data-ttu-id="de833-3098">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="de833-3098">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="de833-3099">Prise en charge de la définition de valeurs par défaut pour des arguments courants tels que le groupe de ressources par défaut, le site web par défaut et la machine virtuelle par défaut</span><span class="sxs-lookup"><span data-stu-id="de833-3099">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="de833-3100">Prise en charge de la connexion à un locataire spécifique</span><span class="sxs-lookup"><span data-stu-id="de833-3100">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="de833-3101">ACS</span><span class="sxs-lookup"><span data-stu-id="de833-3101">ACS</span></span>

* <span data-ttu-id="de833-3102">[ACS] Ajout de la prise en charge de la configuration d’un cluster ACS par défaut ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="de833-3102">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="de833-3103">Ajout de la prise en charge de l’invite de mot de passe de clé ssh.</span><span class="sxs-lookup"><span data-stu-id="de833-3103">Add support for ssh key password prompting.</span></span> <span data-ttu-id="de833-3104">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="de833-3104">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="de833-3105">Ajout de la prise en charge des clusters Windows.</span><span class="sxs-lookup"><span data-stu-id="de833-3105">Add support for windows clusters.</span></span> <span data-ttu-id="de833-3106">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="de833-3106">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="de833-3107">Basculement du rôle Propriétaire au rôle Contributeur.</span><span class="sxs-lookup"><span data-stu-id="de833-3107">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="de833-3108">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="de833-3108">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="de833-3109">AppService</span><span class="sxs-lookup"><span data-stu-id="de833-3109">AppService</span></span>

* <span data-ttu-id="de833-3110">appservice : prise en charge de l’obtention de l’adresse IP externe utilisée pour les enregistrements A DNS ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="de833-3110">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="de833-3111">appservice : prise en charge de la liaison des certificats avec caractères génériques ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="de833-3111">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="de833-3112">appservice : prise en charge des profils de publication de liste ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="de833-3112">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="de833-3113">AppService : déclenchement de la synchronisation de contrôle de code source après la configuration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="de833-3113">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="de833-3114">DataLake</span><span class="sxs-lookup"><span data-stu-id="de833-3114">DataLake</span></span>

* <span data-ttu-id="de833-3115">Version initiale du module Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="de833-3115">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="de833-3116">Version initiale du module Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="de833-3116">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="de833-3117">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="de833-3117">DocuemntDB</span></span>

* <span data-ttu-id="de833-3118">DocumentDB : ajout de la prise en charge de l’énumération des chaînes de connexion ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="de833-3118">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="de833-3119">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="de833-3119">VM</span></span>

* <span data-ttu-id="de833-3120">[Compute] Ajout de la prise en charge d’AppGateway à la création de groupe de machines virtuelles identiques ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="de833-3120">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="de833-3121">[VM/VMSS] Amélioration de la prise en charge de la mise en cache de disque ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="de833-3121">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="de833-3122">VM/VMSS : intégration de la logique de validation des informations d’identification utilisée par le portail ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="de833-3122">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="de833-3123">Ajout de la prise en charge des commandes wait et de --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="de833-3123">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="de833-3124">Groupe de machines virtuelles identiques : prise en charge de \* pour énumérer les vues d’instance parmi les machines virtuelles ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="de833-3124">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="de833-3125">Ajout --secrets pour machine virtuelle et groupe de machines virtuelles identiques ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="de833-3125">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="de833-3126">Autorisation de la création de machines virtuelles avec un disque dur virtuel spécialisé ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="de833-3126">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="de833-3127">27 février 2017</span><span class="sxs-lookup"><span data-stu-id="de833-3127">February 27, 2017</span></span>

<span data-ttu-id="de833-3128">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="de833-3128">Version 2.0.0</span></span>

<span data-ttu-id="de833-3129">Cette version d’Azure CLI 2.0 est la première instance mise à la disposition générale. La disponibilité générale s’applique à ces modules de commande :</span><span class="sxs-lookup"><span data-stu-id="de833-3129">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="de833-3130">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="de833-3130">Container Service (acs)</span></span>
- <span data-ttu-id="de833-3131">Compute (notamment Resource Manager, machine virtuelle, groupes de machines virtuelles identiques, Disques managés)</span><span class="sxs-lookup"><span data-stu-id="de833-3131">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="de833-3132">Mise en réseau</span><span class="sxs-lookup"><span data-stu-id="de833-3132">Networking</span></span>
- <span data-ttu-id="de833-3133">Stockage</span><span class="sxs-lookup"><span data-stu-id="de833-3133">Storage</span></span>

<span data-ttu-id="de833-3134">Ces modules de commande, pouvant être utilisés en production, sont pris en charge par le contrat de niveau de service (SLA) Microsoft standard. Vous pouvez ouvrir des incidents directement auprès du support technique Microsoft ou dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/). Vous pouvez poser des questions sur [StackOverflow à l’aide du mot-clé azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), ou contacter l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Vous pouvez fournir des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="de833-3134">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="de833-3135">Les commandes de ces modules sont stables et il n’est pas prévu que la syntaxe change dans les mises à jour ultérieures de cette version d’Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="de833-3135">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="de833-3136">Pour vérifier la version de l’interface CLI, utilisez `az --version`. La sortie indique la version de l’interface CLI proprement dite (2.0.0 dans cette version), les différents modules de commande et les versions de Python et de GCC que vous utilisez.</span><span class="sxs-lookup"><span data-stu-id="de833-3136">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="de833-3137">Certains de ces modules de commande présentent un suffixe « b*n* » ou « rc*n* ». Ces modules de commande, encore en préversion, seront mis à la disposition générale à l’avenir.</span><span class="sxs-lookup"><span data-stu-id="de833-3137">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="de833-3138">Nous avons également des versions d’évaluation nocturnes de l’interface CLI. Pour plus d’informations, consultez ces instructions sur l’[obtention des builds nocturnes](https://github.com/Azure/azure-cli#nightly-builds), ainsi que ces instructions sur [la contribution au code et la configuration d’un environnement de développement](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="de833-3138">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="de833-3139">Vous pouvez signaler des problèmes liés aux versions d’évaluation nocturnes comme suit :</span><span class="sxs-lookup"><span data-stu-id="de833-3139">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="de833-3140">Signalez des problèmes dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="de833-3140">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="de833-3141">Contactez l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="de833-3141">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="de833-3142">Fournissez des commentaires à partir de la ligne de commande avec la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="de833-3142">Provide feedback from the command line with the `az feedback` command</span></span>

