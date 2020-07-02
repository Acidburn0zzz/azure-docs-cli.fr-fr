---
title: Références Azure CLI pour Azure IoT
description: Page de destination des références Azure CLI pour Azure IoT
author: dbradish-microsoft
manager: barbkess
ms.devlang: azurecli
ms.topic: reference
ms.date: 06/05/2020
ms.author: dbradish
ms.service: azure-cli
ms.reviewer: paymaun.heidari
ms.openlocfilehash: e3bf40eab68f09dfb94e14e59d8a746d87bb0766
ms.sourcegitcommit: 415c6ddcce1da133d96b8c700e6aa570e4746b3f
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/01/2020
ms.locfileid: "85765102"
---
# <a name="azure-cli-for-azure-iot"></a><span data-ttu-id="c0455-103">Azure CLI pour Azure IoT</span><span class="sxs-lookup"><span data-stu-id="c0455-103">Azure CLI for Azure IoT</span></span>

<span data-ttu-id="c0455-104">L'interface de ligne de commande Azure ([Azure CLI](/cli/azure/what-is-azure-cli)) est un ensemble de commandes utilisées pour créer et gérer des ressources Azure.</span><span class="sxs-lookup"><span data-stu-id="c0455-104">The Azure Command Line Interface ([Azure CLI](/cli/azure/what-is-azure-cli)) is a set of commands used to create and manage Azure resources.</span></span>  <span data-ttu-id="c0455-105">Elle est disponible sur de nombreux services Azure, notamment Azure IoT.</span><span class="sxs-lookup"><span data-stu-id="c0455-105">It is available across many Azure services including Azure IoT.</span></span>  <span data-ttu-id="c0455-106">Il existe plus de 100 références pour Azure IoT vous donnant la possibilité de travailler efficacement avec les services IoT à partir d’une ligne de commande.</span><span class="sxs-lookup"><span data-stu-id="c0455-106">There are over 100 references for Azure IoT giving you the ability to work effectively with IoT services from a command line.</span></span>

## <a name="references-for-iot"></a><span data-ttu-id="c0455-107">Références pour IoT</span><span class="sxs-lookup"><span data-stu-id="c0455-107">References for IoT</span></span>

<span data-ttu-id="c0455-108">L’expérience CLI d’Azure IoT est composée de deux parties : Azure CLI (communément appelée **noyau** CLI) et l’**extension** Azure IoT CLI.</span><span class="sxs-lookup"><span data-stu-id="c0455-108">The Azure IoT CLI experience is composed of two parts: Azure CLI (commonly referred to as CLI **core**) and the Azure IoT CLI **extension**.</span></span>

<span data-ttu-id="c0455-109">La fonctionnalité IoT dans le **noyau** Azure CLI est axée sur la gestion et la configuration de l’infrastructure.</span><span class="sxs-lookup"><span data-stu-id="c0455-109">IoT functionality in Azure CLI **core** is focused on infrastructure management and configuration.</span></span> <span data-ttu-id="c0455-110">Les opérations CRUD IoT Hub, ou la configuration des routes de messages IoT Hub, sont des cas d’usage typiques pour les commandes de noyau.</span><span class="sxs-lookup"><span data-stu-id="c0455-110">IoT Hub CRUD operations, or configuring IoT Hub message routes are typical use cases for core commands.</span></span>

<span data-ttu-id="c0455-111">L’**extension** IoT introduit des fonctions en enrichies pour gérer, manipuler et interagir avec les données, les entités et les objets de l’infrastructure elle-même.</span><span class="sxs-lookup"><span data-stu-id="c0455-111">The IoT **extension** introduces rich features and functionality to manage, manipulate and interact with the data, entities and objects on the infrastructure itself.</span></span> <span data-ttu-id="c0455-112">Par exemple, la gestion des flottes d’appareils, la supervision des événements appareil-à-cloud et l’appel de méthodes cloud-à-appareil sont toutes activées par le biais de l’extension IoT.</span><span class="sxs-lookup"><span data-stu-id="c0455-112">For example managing fleets of devices, monitoring device-to-cloud events and invoking cloud to device methods are all enabled via the IoT extension.</span></span> <span data-ttu-id="c0455-113">L’extension Azure IoT pour Azure CLI déverrouille l’utilisation de technologies expérimentales ou en préversion qui contribuent à sa polyvalence dans divers scénarios et cas d’usage.</span><span class="sxs-lookup"><span data-stu-id="c0455-113">The Azure IoT extension for Azure CLI unlocks the use of experimental or pre-release technology contributing to its versatility in a variety of scenarios and use cases.</span></span>

### <a name="core-reference-commands"></a><span data-ttu-id="c0455-114">Informations de référence sur le noyau</span><span class="sxs-lookup"><span data-stu-id="c0455-114">Core reference commands</span></span>

| <span data-ttu-id="c0455-115">Informations de référence</span><span class="sxs-lookup"><span data-stu-id="c0455-115">Reference</span></span> | <span data-ttu-id="c0455-116">A une extension</span><span class="sxs-lookup"><span data-stu-id="c0455-116">Has extension</span></span> | <span data-ttu-id="c0455-117">Description</span><span class="sxs-lookup"><span data-stu-id="c0455-117">Description</span></span>
|-|-|-|
| [<span data-ttu-id="c0455-118">az iot</span><span class="sxs-lookup"><span data-stu-id="c0455-118">az iot</span></span>](/cli/azure/iot) | <span data-ttu-id="c0455-119">Oui</span><span class="sxs-lookup"><span data-stu-id="c0455-119">yes</span></span>  | <span data-ttu-id="c0455-120">Toutes les commandes de noyau Azure CLI disponibles pour Azure IoT.</span><span class="sxs-lookup"><span data-stu-id="c0455-120">All available Azure CLI core commands for Azure IoT.</span></span>
| [<span data-ttu-id="c0455-121">az iot central</span><span class="sxs-lookup"><span data-stu-id="c0455-121">az iot central</span></span>](/cli/azure/iot/central) | <span data-ttu-id="c0455-122">Oui</span><span class="sxs-lookup"><span data-stu-id="c0455-122">yes</span></span> | <span data-ttu-id="c0455-123">Gérer les ressources IoT Central.</span><span class="sxs-lookup"><span data-stu-id="c0455-123">Manage IoT Central assets.</span></span>
| [<span data-ttu-id="c0455-124">az iot dps</span><span class="sxs-lookup"><span data-stu-id="c0455-124">az iot dps</span></span>](/en-us/cli/azure/iot/dps) | <span data-ttu-id="c0455-125">Oui</span><span class="sxs-lookup"><span data-stu-id="c0455-125">yes</span></span> | <span data-ttu-id="c0455-126">Gérer le service IoT Hub Device Provisioning.</span><span class="sxs-lookup"><span data-stu-id="c0455-126">Manage Azure IoT Hub Device Provisioning Service.</span></span>
| [<span data-ttu-id="c0455-127">az iot hub</span><span class="sxs-lookup"><span data-stu-id="c0455-127">az iot hub</span></span>](/cli/azure/iot/hub) | <span data-ttu-id="c0455-128">Oui</span><span class="sxs-lookup"><span data-stu-id="c0455-128">yes</span></span> | <span data-ttu-id="c0455-129">Gérer l’infrastructure Azure IoT Hub.</span><span class="sxs-lookup"><span data-stu-id="c0455-129">Manage Azure IoT Hub infrastructure.</span></span>
| [<span data-ttu-id="c0455-130">az iot pnp</span><span class="sxs-lookup"><span data-stu-id="c0455-130">az iot pnp</span></span>](/cli/azure/iot/pnp) | <span data-ttu-id="c0455-131">Oui</span><span class="sxs-lookup"><span data-stu-id="c0455-131">yes</span></span> | <span data-ttu-id="c0455-132">Gérer les référentiels IoT Plug-and-Play et les clés d’accès aux référentiels.</span><span class="sxs-lookup"><span data-stu-id="c0455-132">Manage IoT Plug and Play repositories and repository access keys.</span></span>

### <a name="extension-reference-commands"></a><span data-ttu-id="c0455-133">Commandes de référence des extensions</span><span class="sxs-lookup"><span data-stu-id="c0455-133">Extension reference commands</span></span>

| <span data-ttu-id="c0455-134">Informations de référence</span><span class="sxs-lookup"><span data-stu-id="c0455-134">Reference</span></span> | <span data-ttu-id="c0455-135">A un noyau</span><span class="sxs-lookup"><span data-stu-id="c0455-135">Has core</span></span> | <span data-ttu-id="c0455-136">Description</span><span class="sxs-lookup"><span data-stu-id="c0455-136">Description</span></span>
|-|-|-|
| [<span data-ttu-id="c0455-137">az iot</span><span class="sxs-lookup"><span data-stu-id="c0455-137">az iot</span></span>](/cli/azure/ext/azure-iot/iot) | <span data-ttu-id="c0455-138">Oui</span><span class="sxs-lookup"><span data-stu-id="c0455-138">yes</span></span> | <span data-ttu-id="c0455-139">Toutes les commandes d’extension Azure CLI disponibles pour Azure IoT.</span><span class="sxs-lookup"><span data-stu-id="c0455-139">All available Azure CLI extension commands for Azure IoT.</span></span>
| [<span data-ttu-id="c0455-140">az iot central</span><span class="sxs-lookup"><span data-stu-id="c0455-140">az iot central</span></span>](/cli/azure/ext/azure-iot/iot/central) | <span data-ttu-id="c0455-141">Oui</span><span class="sxs-lookup"><span data-stu-id="c0455-141">yes</span></span> | <span data-ttu-id="c0455-142">Gérer les solutions et l’infrastructure Azure Central (IoT Central).</span><span class="sxs-lookup"><span data-stu-id="c0455-142">Manage Azure Central (IoT Central) solutions & infrastructure.</span></span>
| [<span data-ttu-id="c0455-143">az iot device</span><span class="sxs-lookup"><span data-stu-id="c0455-143">az iot device</span></span>](/cli/azure/ext/azure-iot/iot/device) | | <span data-ttu-id="c0455-144">Tirer parti des fonctionnalités de messagerie appareil-à-cloud et cloud-à-appareil.</span><span class="sxs-lookup"><span data-stu-id="c0455-144">Leverage device-to-cloud and cloud-to-device messaging capabilities.</span></span>
| [<span data-ttu-id="c0455-145">az dt</span><span class="sxs-lookup"><span data-stu-id="c0455-145">az dt</span></span>](/cli/azure/ext/azure-iot/dt) | | <span data-ttu-id="c0455-146">Gérer les solutions et l’infrastructure Azure Digital Twins.</span><span class="sxs-lookup"><span data-stu-id="c0455-146">Manage Azure Digital Twins solutions & infrastructure.</span></span>
| [<span data-ttu-id="c0455-147">az iot dps</span><span class="sxs-lookup"><span data-stu-id="c0455-147">az iot dps</span></span>](/cli/azure/ext/azure-iot/iot/dps) | <span data-ttu-id="c0455-148">Oui</span><span class="sxs-lookup"><span data-stu-id="c0455-148">yes</span></span> | <span data-ttu-id="c0455-149">Gérer les entités dans un service Azure IoT Hub Device Provisioning.</span><span class="sxs-lookup"><span data-stu-id="c0455-149">Manage entities in an Azure IoT Hub Device Provisioning Service.</span></span>
| [<span data-ttu-id="c0455-150">az iot edge</span><span class="sxs-lookup"><span data-stu-id="c0455-150">az iot edge</span></span>](/cli/azure/ext/azure-iot/iot/edge) | | <span data-ttu-id="c0455-151">Gérer les solutions IoT en périphérie.</span><span class="sxs-lookup"><span data-stu-id="c0455-151">Manage IoT solutions on the Edge.</span></span>
| [<span data-ttu-id="c0455-152">az iot hub</span><span class="sxs-lookup"><span data-stu-id="c0455-152">az iot hub</span></span>](/cli/azure/ext/azure-iot/iot/hub) | <span data-ttu-id="c0455-153">Oui</span><span class="sxs-lookup"><span data-stu-id="c0455-153">yes</span></span> | <span data-ttu-id="c0455-154">Gérer les entités dans un hub IoT Azure.</span><span class="sxs-lookup"><span data-stu-id="c0455-154">Manage entities in an Azure IoT Hub.</span></span>
| [<span data-ttu-id="c0455-155">az iot pnp</span><span class="sxs-lookup"><span data-stu-id="c0455-155">az iot pnp</span></span>](/cli/azure/ext/azure-iot/iot/pnp) | <span data-ttu-id="c0455-156">Oui</span><span class="sxs-lookup"><span data-stu-id="c0455-156">yes</span></span> | <span data-ttu-id="c0455-157">Gérer les entités d’un référentiel de modèle IoT Plug-and-Play.</span><span class="sxs-lookup"><span data-stu-id="c0455-157">Manage entities of an IoT Plug and Play model repository.</span></span>

### <a name="additional-cli-commands-for-azure-services-used-by-iot"></a><span data-ttu-id="c0455-158">Commandes CLI supplémentaires pour les services Azure utilisés par IoT</span><span class="sxs-lookup"><span data-stu-id="c0455-158">Additional CLI commands for Azure services used by IoT</span></span>

| <span data-ttu-id="c0455-159">Informations de référence</span><span class="sxs-lookup"><span data-stu-id="c0455-159">Reference</span></span> | <span data-ttu-id="c0455-160">Type</span><span class="sxs-lookup"><span data-stu-id="c0455-160">Type</span></span> | <span data-ttu-id="c0455-161">Description</span><span class="sxs-lookup"><span data-stu-id="c0455-161">Description</span></span>
|-|-|-|
| [<span data-ttu-id="c0455-162">az maps</span><span class="sxs-lookup"><span data-stu-id="c0455-162">az maps</span></span>](/cli/azure/maps) | <span data-ttu-id="c0455-163">core</span><span class="sxs-lookup"><span data-stu-id="c0455-163">core</span></span> | <span data-ttu-id="c0455-164">Gérer Azure Maps.</span><span class="sxs-lookup"><span data-stu-id="c0455-164">Manage Azure Maps.</span></span>
| [<span data-ttu-id="c0455-165">az timeseriesinsights</span><span class="sxs-lookup"><span data-stu-id="c0455-165">az timeseriesinsights</span></span>](/cli/azure/ext/timeseriesinsights/timeseriesinsights) | <span data-ttu-id="c0455-166">extension</span><span class="sxs-lookup"><span data-stu-id="c0455-166">extension</span></span> | <span data-ttu-id="c0455-167">Gérer Azure Time Series Insights.</span><span class="sxs-lookup"><span data-stu-id="c0455-167">Manage Azure Time Series Insights.</span></span>

## <a name="popular-iot-articles-using-the-azure-cli"></a><span data-ttu-id="c0455-168">Articles IoT populaires utilisant Azure CLI</span><span class="sxs-lookup"><span data-stu-id="c0455-168">Popular IoT articles using the Azure CLI</span></span>

- [<span data-ttu-id="c0455-169">Créer un hub IoT</span><span class="sxs-lookup"><span data-stu-id="c0455-169">Create an IoT hub</span></span>](/azure/iot-hub/iot-hub-create-using-cli)
- [<span data-ttu-id="c0455-170">Gérer IoT Central</span><span class="sxs-lookup"><span data-stu-id="c0455-170">Manage IoT Central</span></span>](/azure/iot-central/core/howto-manage-iot-central-from-cli)
- [<span data-ttu-id="c0455-171">Tutoriels sur les appareils basés sur l’interface CLI utilisant Azure RTOS</span><span class="sxs-lookup"><span data-stu-id="c0455-171">CLI driven device tutorials using Azure RTOS</span></span>](/azure/rtos/getting-started?branch=master)
- [<span data-ttu-id="c0455-172">Utiliser l’extension IoT pour la gestion des appareils Azure IoT Hub</span><span class="sxs-lookup"><span data-stu-id="c0455-172">Use the IoT extension for Azure IoT Hub device management</span></span>](/azure/iot-hub/iot-hub-device-management-iot-extension-azure-cli-2-0)
- [<span data-ttu-id="c0455-173">Déployer et superviser des modules IoT Edge à grande échelle avec l’extension Azure CLI pour IoT</span><span class="sxs-lookup"><span data-stu-id="c0455-173">Deploy and monitor IoT Edge modules at scale with the Azure CLI extension for IoT</span></span>](/azure/iot-edge/how-to-deploy-cli-at-scale)
- [<span data-ttu-id="c0455-174">Envoyer des données de télémétrie à un appareil et les superviser avec l’extension Azure CLI pour IoT</span><span class="sxs-lookup"><span data-stu-id="c0455-174">Send Telemetry to a device and monitor it with the Azure CLI extension for IoT</span></span>](/azure/iot-hub/quickstart-send-telemetry-cli)
- [<span data-ttu-id="c0455-175">Utiliser Azure CLI pour configurer le routage des messages IoT Hub</span><span class="sxs-lookup"><span data-stu-id="c0455-175">Use the Azure CLI to configure IoT Hub message routing</span></span>](/azure/iot-hub/tutorial-routing-config-message-routing-cli)
- [<span data-ttu-id="c0455-176">Gérer les interfaces dans un référentiel de modèles Plug-and-Play</span><span class="sxs-lookup"><span data-stu-id="c0455-176">Manage interfaces in a Plug and Play model repository</span></span>](/azure/iot-pnp/howto-install-pnp-cli#manage-interfaces-in-a-model-repository)

## <a name="azure-cli-reference-examples"></a><span data-ttu-id="c0455-177">Exemples de référence Azure CLI</span><span class="sxs-lookup"><span data-stu-id="c0455-177">Azure CLI reference examples</span></span>

<span data-ttu-id="c0455-178">Des exemples sont fournis avec chaque référence Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="c0455-178">Examples are provided with every Azure CLI reference.</span></span> <span data-ttu-id="c0455-179">Vous pouvez également effectuer ces tâches via le portail Azure, mais l'utilisation d'Azure CLI ne nécessite qu'une seule ligne de commande.</span><span class="sxs-lookup"><span data-stu-id="c0455-179">Although you can also complete these tasks through the Azure portal, using the Azure CLI requires a single command line.</span></span>  <span data-ttu-id="c0455-180">Les blocs de code suivants vous donneront une idée de la facilité d'utilisation d'Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="c0455-180">Here are a few code blocks to give you an idea of how easy it is to use the Azure CLI.</span></span>

<span data-ttu-id="c0455-181">Pour utiliser Azure IoT, vous devrez d’abord disposer d’un groupe de ressources.</span><span class="sxs-lookup"><span data-stu-id="c0455-181">To work with Azure IoT, you'll first need a resource group.</span></span>  <span data-ttu-id="c0455-182">Les groupes de ressources Azure sont faciles à créer et à gérer avec Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="c0455-182">Azure resource groups are simple to create and manage with the Azure CLI.</span></span>  

```azurecli
#create a resource group
az group create -location westus -name MyResourceGroup
```

```azurecli
#get a list of resource groups for a subscription
az group list --subscription MySubscription --output table
```

<span data-ttu-id="c0455-183">Il est aussi simple de créer un hub IoT Azure dans la région « westus » au niveau tarifaire standard.</span><span class="sxs-lookup"><span data-stu-id="c0455-183">It is as straightforward to create an Azure IoT Hub in the '''westus''' region in the standard pricing tier.</span></span>

```azurecli
#create an Azure IoT hub
az iot hub create --resource-group MyResourceGroup --name MyIotHub --location westus
```

## <a name="see-also"></a><span data-ttu-id="c0455-184">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c0455-184">See also</span></span>

- <span data-ttu-id="c0455-185">[Prise en main d'Azure CLI](/cli/azure/get-started-with-azure-cli) pour en savoir plus sur l'installation et la connexion.</span><span class="sxs-lookup"><span data-stu-id="c0455-185">[Get started with Azure CLI](/cli/azure/get-started-with-azure-cli) to learn about installation and sign in.</span></span>

- <span data-ttu-id="c0455-186">Découvrez des références [publiées](/cli/azure/reference-index) et [d’extension](/cli/azure/azure-cli-extensions-list) supplémentaires dans la documentation Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="c0455-186">Discover additional [released](/cli/azure/reference-index) and [extension](/cli/azure/azure-cli-extensions-list) references in the Azure CLI documentation.</span></span>

- <span data-ttu-id="c0455-187">Découvrez-en plus sur les références des extensions dans [Utiliser des extensions avec Azure CLI](/cli/azure/azure-cli-extensions-overview).</span><span class="sxs-lookup"><span data-stu-id="c0455-187">Find out more about extension references in [Use extensions with Azure CLI](/cli/azure/azure-cli-extensions-overview).</span></span>
