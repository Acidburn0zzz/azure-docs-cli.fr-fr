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
ms.custom: devx-track-azurecli
ms.openlocfilehash: 0d1c117274d4e363c921d9161fbbf1051d0b078b
ms.sourcegitcommit: 5d29362589078b66d15f5cd494fe903a5195658d
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/25/2020
ms.locfileid: "91225454"
---
# <a name="azure-cli-for-azure-iot"></a>Azure CLI pour Azure IoT

L'interface de ligne de commande Azure ([Azure CLI](./what-is-azure-cli.md)) est un ensemble de commandes utilisées pour créer et gérer des ressources Azure.  Elle est disponible sur de nombreux services Azure, notamment Azure IoT.  Il existe plus de 100 références pour Azure IoT vous donnant la possibilité de travailler efficacement avec les services IoT à partir d’une ligne de commande.

## <a name="references-for-iot"></a>Références pour IoT

L’expérience CLI d’Azure IoT est composée de deux parties : Azure CLI (communément appelée **noyau** CLI) et l’**extension** Azure IoT CLI.

La fonctionnalité IoT dans le **noyau** Azure CLI est axée sur la gestion et la configuration de l’infrastructure. Les opérations CRUD IoT Hub, ou la configuration des routes de messages IoT Hub, sont des cas d’usage typiques pour les commandes de noyau.

L’**extension** IoT introduit des fonctions en enrichies pour gérer, manipuler et interagir avec les données, les entités et les objets de l’infrastructure elle-même. Par exemple, la gestion des flottes d’appareils, la supervision des événements appareil-à-cloud et l’appel de méthodes cloud-à-appareil sont toutes activées par le biais de l’extension IoT. L’extension Azure IoT pour Azure CLI déverrouille l’utilisation de technologies expérimentales ou en préversion qui contribuent à sa polyvalence dans divers scénarios et cas d’usage.

### <a name="core-reference-commands"></a>Informations de référence sur le noyau

| Informations de référence | A une extension | Description
|-|-|-|
| [az iot](/cli/azure/iot) | Oui  | Toutes les commandes de noyau Azure CLI disponibles pour Azure IoT.
| [az iot central](/cli/azure/iot/central) | Oui | Gérer les ressources IoT Central.
| [az iot dps](/cli/azure/iot/dps) | Oui | Gérer le service IoT Hub Device Provisioning.
| [az iot hub](/cli/azure/iot/hub) | Oui | Gérer l’infrastructure Azure IoT Hub.

### <a name="extension-reference-commands"></a>Commandes de référence des extensions

| Informations de référence | A un noyau | Description
|-|-|-|
| [az iot](/cli/azure/ext/azure-iot/iot) | Oui | Toutes les commandes d’extension Azure CLI disponibles pour Azure IoT.
| [az iot central](/cli/azure/ext/azure-iot/iot/central) | Oui | Gérer les solutions et l’infrastructure Azure Central (IoT Central).
| [az iot device](/cli/azure/ext/azure-iot/iot/device) | | Tirer parti des fonctionnalités de messagerie appareil-à-cloud et cloud-à-appareil.
| [az dt](/cli/azure/ext/azure-iot/dt) | | Gérer les solutions et l’infrastructure Azure Digital Twins.
| [az iot dps](/cli/azure/ext/azure-iot/iot/dps) | Oui | Gérer les entités dans un service Azure IoT Hub Device Provisioning.
| [az iot edge](/cli/azure/ext/azure-iot/iot/edge) | | Gérer les solutions IoT en périphérie.
| [az iot hub](/cli/azure/ext/azure-iot/iot/hub) | Oui | Gérer les entités dans un hub IoT Azure.
| [az iot pnp](/cli/azure/ext/azure-iot/iot/pnp) | | Gérer les entités d’un référentiel de modèle IoT Plug-and-Play.

### <a name="additional-cli-commands-for-azure-services-used-by-iot"></a>Commandes CLI supplémentaires pour les services Azure utilisés par IoT

| Informations de référence | Type | Description
|-|-|-|
| [az maps](/cli/azure/maps) | core | Gérer Azure Maps.
| [az timeseriesinsights](/cli/azure/ext/timeseriesinsights/timeseriesinsights) | extension | Gérer Azure Time Series Insights.

### <a name="extension-reference-installation"></a>Installation de référence des extensions

Les références d’extension Azure CLI doivent être installées avant d’être utilisées.  Utilisez la commande [az extension add](./azure-cli-extensions-overview.md) pour installer une référence d’extension par nom.  Découvrez-en plus sur les références des extensions dans [Utiliser des extensions avec Azure CLI](./azure-cli-extensions-overview.md).

```azurecli
# install the Azure CLI extension reference for Azure IoT
az extension add --name azure-iot
```

## <a name="popular-iot-articles-using-the-azure-cli"></a>Articles IoT populaires utilisant Azure CLI

- [Créer un hub IoT](/azure/iot-hub/iot-hub-create-using-cli)
- [Gérer IoT Central](/azure/iot-central/core/howto-manage-iot-central-from-cli)
- [Tutoriels sur les appareils basés sur l’interface CLI utilisant Azure RTOS](/azure/rtos/getting-started?branch=master)
- [Utiliser l’extension IoT pour la gestion des appareils Azure IoT Hub](/azure/iot-hub/iot-hub-device-management-iot-extension-azure-cli-2-0)
- [Déployer et superviser des modules IoT Edge à grande échelle avec l’extension Azure CLI pour IoT](/azure/iot-edge/how-to-deploy-cli-at-scale)
- [Envoyer des données de télémétrie à un appareil et les superviser avec l’extension Azure CLI pour IoT](/azure/iot-hub/quickstart-send-telemetry-cli)
- [Utiliser Azure CLI pour configurer le routage des messages IoT Hub](/azure/iot-hub/tutorial-routing-config-message-routing-cli)
- [Gérer les interfaces dans un référentiel de modèles Plug-and-Play](/azure/iot-pnp/howto-install-pnp-cli#manage-interfaces-in-a-model-repository)

## <a name="azure-cli-reference-examples"></a>Exemples de référence Azure CLI

Des exemples sont fournis avec chaque référence Azure CLI. Vous pouvez également effectuer ces tâches via le portail Azure, mais l'utilisation d'Azure CLI ne nécessite qu'une seule ligne de commande.  Les blocs de code suivants vous donneront une idée de la facilité d'utilisation d'Azure CLI.

Pour utiliser Azure IoT, vous devrez d’abord disposer d’un groupe de ressources.  Les groupes de ressources Azure sont faciles à créer et à gérer avec Azure CLI.  

```azurecli
#create a resource group
az group create -location westus -name MyResourceGroup
```

```azurecli
#get a list of resource groups for a subscription
az group list --subscription MySubscription --output table
```

Il est aussi simple de créer un hub IoT Azure dans la région « westus » au niveau tarifaire standard.

```azurecli
#create an Azure IoT hub
az iot hub create --resource-group MyResourceGroup --name MyIotHub --location westus
```

## <a name="see-also"></a>Voir aussi

- [Prise en main d'Azure CLI](./get-started-with-azure-cli.md) pour en savoir plus sur l'installation et la connexion.

- Découvrez des références [publiées](/cli/azure/reference-index) et [d’extension](./azure-cli-extensions-list.md) supplémentaires dans la documentation Azure CLI.