---
title: Extensions disponibles pour Azure CLI
description: Liste complète des extensions officiellement prises en charge pour Azure CLI.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 11/07/2018
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 97636487677a0f28837c474d10cffedc7a52d5a5
ms.sourcegitcommit: 2a2c87c21289cdfef3d0e5b3f07b0bea42c6c267
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/08/2018
ms.locfileid: "51273172"
---
# <a name="available-extensions-for-the-azure-cli"></a>Extensions disponibles pour Azure CLI

Cet article comporte une liste complète des extensions disponibles pour Azure CLI qui sont prises en charge par Microsoft.

La liste des extensions est également disponible à partir de l’interface CLI. Pour l’obtenir, exécutez [az extension list-available](/cli/azure/extension?view=azure-cli-latest#az-extension-list-available) :

```azurecli-interactive
az extension list-available --output table
```

| NOM | Version | Résumé | VERSION PRÉLIMINAIRE |
|------|---------|---------|---------|
| [aem](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Gestion des extensions de surveillance Azure améliorée pour SAP |  |
| [préversion ASK](https://github.com/Azure/azure-cli-extensions/tree/master/src/aks-preview) | 0.1.0 | Fournit une préversion des fonctionnalités AKS à venir | Oui |
| [alias](https://github.com/Azure/azure-cli-extensions) | 0.5.2 | Prise en charge des alias de commande | Oui |
| [azure-batch-cli-extensions](https://github.com/Azure/azure-batch-cli-extensions) | 2.5.1 | Commandes supplémentaires pour travailler avec le service Azure Batch |  |
| [azure-cli-iot-ext](https://github.com/azure/azure-iot-cli-extension) | 0.6.0 | Fourniture de la couche de commandes du plan de données pour Azure IoT Hub, IoT Edge et le service de provisionnement d’appareils IoT |  |
| [azure-firewall](https://github.com/Azure/azure-cli-extensions/tree/master/src/azure-firewall) | 0.1.0 | Gérez les ressources de pare-feu Azure. | Oui |
| [botservice](https://github.com/Azure/azure-cli-extensions) | 0.4.1 | Résolution de bogues concernant les problèmes dans le module de commande cli du botservice natif. | Oui |
| [dev-spaces-preview](https://github.com/Azure/azure-cli-extensions) | 0.1.6 | Dev Spaces offre aux équipes une expérience de développement Kubernetes rapide et itérative. | Oui |
| [dms-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/dms-preview) | 0.5.0 | Prise en charge de nouveaux scénarios de Database Migration Service. | Oui |
| [dns](https://github.com/Azure/azure-cli-extensions) | 0.0.2 | Une extension Azure CLI pour les zones DNS |  |
| [eventgrid](https://github.com/Azure/azure-cli-extensions) | 0.4.0 | Prise en charge des fonctionnalités d’évaluation d’Azure EventGrid 2018-09-15 | Oui |
| [express-route](https://github.com/Azure/azure-cli-extensions/tree/master/src/express-route) | 0.1.3 | Gérez les instances ExpressRoute avec les fonctionnalités d’évaluation. | Oui |
| [express-route-cross-connexion](https://github.com/Azure/azure-cli-extensions/tree/master/src/express-route-cross-connection) | 0.1.0 | Gérez des circuits ExpressRoute de client à l’aide d’une interconnexion ExpressRoute. |  |
| [find](https://github.com/Azure/azure-cli-extensions/tree/master/src/find) | 0.2.0 | Requêtes intelligentes pour l’obtention d’informations relatives l’interface CLI. | Oui |
| [front-door](https://github.com/Azure/azure-cli-extensions/tree/master/src/front-door) | 0.1.1 | Gérez les portes d’entrée réseau. | Oui |
| [image-copy-extension](https://github.com/Azure/azure-cli-extensions) | 0.0.8 | Prise en charge de la copie d’images de machines virtuelles managées entre régions |  |
| [interactive](https://github.com/Azure/azure-cli) | 0.4.1 | Shell interactif de ligne de commande Microsoft Azure | Oui |
| [keyvault-preview](https://github.com/Azure/azure-keyvault-cli-extension) | 0.1.3 | Préversion des commandes Azure Key Vault. | Oui |
| [log-analytics](https://github.com/Azure/azure-cli-extensions/tree/master/src/log-analytics) | 0.1.3 | Prise en charge des fonctionnalités de requête d’Azure Log Analytics. | Oui |
| [managementgroups](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Une extension Azure CLI pour les groupes d’administration |  |
| [managementpartner](https://github.com/Azure/azure-cli-extensions) | 0.1.2 | Prise en charge de la préversion des groupes d’administration |  |
| [mesh](https://github.com/Azure/azure-cli-extensions) | 0.9.3 | Prise en charge de Microsoft Azure Service Fabric Mesh - préversion publique | Oui |
| [rdbms-vnet](https://github.com/Azure/azure-cli-extensions) | 10.0.0 | Prise en charge des règles de réseau virtuel pour les ressources Azure MySQL et Azure PostgreSQL |  |
| [resource-graph](https://github.com/Azure/azure-cli-extensions/tree/master/src/resource-graph) | 0.1.8 | Assistance pour interroger des ressources Azure avec Resource Graph. | Oui |
| [sap-hana](https://github.com/Azure/azure-hanaonazure-cli-extension) | 0.1.6 | Commandes supplémentaires pour travailler avec les instances SAP HanaOnAzure. |  |
| [signalr](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Prise en charge de la préversion de gestion de signalr. | Oui |
| [storage-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/storage-preview) | 0.1.7 | Fournit un aperçu des fonctionnalités de stockage à venir. | Oui |
| [abonnement](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Prise en charge de la préversion des définitions d’abonnement. |  |
| [virtual-network-tap](https://github.com/Azure/azure-cli-extensions/tree/master/src/virtual-network-tap) | 0.1.0 | Gérez les taps de réseau virtuel (VTAP). | Oui |
| [virtual-wan](https://github.com/Azure/azure-cli-extensions/tree/master/src/virtual-wan) | 0.1.0 | Gérez le WAN virtuel, les hubs, les passerelles VPN et les sites VPN. | Oui |
| [webapp](https://github.com/Azure/azure-cli-extensions) | 0.2.14 | Commandes supplémentaires pour Azure AppService. | Oui |
