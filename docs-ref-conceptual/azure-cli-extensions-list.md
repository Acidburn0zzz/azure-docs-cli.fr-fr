---
title: Extensions disponibles pour Azure CLI
description: Liste complète des extensions officiellement prises en charge pour Azure CLI.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 06/30/2019
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 63d50a46a81482e260307cdc44adfea6aa4499f1
ms.sourcegitcommit: e06d34682710e77840b0c51f4718184101bd8a03
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/02/2019
ms.locfileid: "67527333"
---
# <a name="available-extensions-for-the-azure-cli"></a>Extensions disponibles pour Azure CLI

Cet article comporte une liste complète des extensions disponibles pour Azure CLI qui sont prises en charge par Microsoft.

La liste des extensions est également disponible à partir de l’interface CLI. Pour l’obtenir, exécutez [az extension list-available](/cli/azure/extension?view=azure-cli-latest#az-extension-list-available) :

```azurecli-interactive
az extension list-available --output table
```

| Nom | Version | Résumé | PRÉVERSION |
|------|---------|---------|---------|
| [aem](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Gestion des extensions de surveillance Azure améliorée pour SAP |  |
| [préversion ASK](https://github.com/Azure/azure-cli-extensions/tree/master/src/aks-preview) | 0.4.5 | Fournit une préversion des fonctionnalités AKS à venir | OUI |
| [alias](https://github.com/Azure/azure-cli-extensions) | 0.5.2 | Prise en charge des alias de commande | OUI |
| [appconfig](https://github.com/Azure/azure-cli-extensions) | 0.5.0 | Fournit une préversion des fonctionnalités App Configuration à venir. | OUI |
| [application-insights](https://github.com/Azure/azure-cli-extensions/tree/master/src/application-insights) | 0.1.1 | Prise en charge de la gestion des composants Application Insights et de l’interrogation des métriques, des événements et des journaux de ces composants. | OUI |
| [azure-batch-cli-extensions](https://github.com/Azure/azure-batch-cli-extensions) | 3.0.4 | Commandes supplémentaires pour travailler avec le service Azure Batch |  |
| [azure-cli-iot-ext](https://github.com/azure/azure-iot-cli-extension) | 0.7.1 | Fourniture de la couche de commandes du plan de données pour Azure IoT Hub, IoT Edge et le service de provisionnement d’appareils IoT |  |
| [azure-cli-ml](https://docs.microsoft.com/en-us/azure/machine-learning/service/) | 1.0.45.1 | Module de commande AzureML des outils en ligne de commande Microsoft Azure |  |
| [azure-devops](https://github.com/Microsoft/azure-devops-cli-extension) | 0.11.0 | Outils de gestion Azure DevOps. |  |
| [azure-firewall](https://github.com/Azure/azure-cli-extensions/tree/master/src/azure-firewall) | 0.1.3 | Gérez les ressources de pare-feu Azure. | OUI |
| [db-up](https://github.com/Azure/azure-cli-extensions/tree/master/src/db-up) | 0.1.13 | Commandes supplémentaires pour simplifier les workflows Azure Database. | OUI |
| [dev-spaces](https://github.com/Azure/azure-cli-extensions) | 1.0.3 | Dev Spaces offre aux équipes une expérience de développement Kubernetes rapide et itérative. |  |
| [dev-spaces-preview](https://github.com/Azure/azure-cli-extensions) | 0.1.6 | Dev Spaces offre aux équipes une expérience de développement Kubernetes rapide et itérative. | OUI |
| [dms-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/dms-preview) | 0.8.1 | Prise en charge de nouveaux scénarios de Database Migration Service. | OUI |
| [dns](https://github.com/Azure/azure-cli-extensions) | 0.0.2 | Une extension Azure CLI pour les zones DNS |  |
| [eventgrid](https://github.com/Azure/azure-cli-extensions) | 0.4.3 | Module de commande EventGrid des outils de ligne de commande Microsoft Azure. | OUI |
| [express-route](https://github.com/Azure/azure-cli-extensions/tree/master/src/express-route) | 0.1.3 | Gérez les instances ExpressRoute avec les fonctionnalités d’évaluation. | OUI |
| [express-route-cross-connexion](https://github.com/Azure/azure-cli-extensions/tree/master/src/express-route-cross-connection) | 0.1.1 | Gérez des circuits ExpressRoute de client à l’aide d’une interconnexion ExpressRoute. |  |
| [find](https://github.com/Azure/azure-cli-extensions/tree/master/src/find) | 0.3.0 | Requêtes intelligentes pour l’obtention d’informations relatives l’interface CLI. | OUI |
| [front-door](https://github.com/Azure/azure-cli-extensions/tree/master/src/front-door) | 0.1.8 | Gérez les portes d’entrée réseau. | OUI |
| [image-copy-extension](https://github.com/Azure/azure-cli-extensions) | 0.2.1 | Prise en charge de la copie d’images de machines virtuelles managées entre régions |  |
| [interactive](https://github.com/Azure/azure-cli) | 0.4.3 | Shell interactif de ligne de commande Microsoft Azure | OUI |
| [keyvault-preview](https://github.com/Azure/azure-keyvault-cli-extension) | 0.1.3 | Préversion des commandes Azure Key Vault. | OUI |
| [log-analytics](https://github.com/Azure/azure-cli-extensions/tree/master/src/log-analytics) | 0.1.3 | Prise en charge des fonctionnalités de requête d’Azure Log Analytics. | OUI |
| [managementgroups](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Une extension Azure CLI pour les groupes d’administration |  |
| [managementpartner](https://github.com/Azure/azure-cli-extensions) | 0.1.2 | Prise en charge de la préversion des groupes d’administration |  |
| [mesh](https://github.com/Azure/azure-cli-extensions) | 0.10.6 | Prise en charge de Microsoft Azure Service Fabric Mesh - préversion publique | OUI |
| [mixed-reality](https://github.com/Azure/azure-cli-extensions) | 0.0.1 | Extension Mixed Reality d’Azure CLI. |  |
| [netappfiles-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/netappfiles-preview) | 0.3.2 | Fournit un aperçu des fonctionnalités Azure NetApp Files (ANF) à venir. | OUI |
| [privatedns](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Commandes permettant de gérer les zones DNS privées | OUI |
| [resource-graph](https://github.com/Azure/azure-cli-extensions/tree/master/src/resource-graph) | 0.1.11 | Assistance pour interroger des ressources Azure avec Resource Graph. | OUI |
| [sap-hana](https://github.com/Azure/azure-hanaonazure-cli-extension) | 0.4.1 | Commandes supplémentaires pour travailler avec les instances SAP HanaOnAzure. |  |
| [storage-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/storage-preview) | 0.2.7 | Fournit un aperçu des fonctionnalités de stockage à venir. | OUI |
| [subscription](https://github.com/Azure/azure-cli-extensions) | 0.1.3 | Prise en charge de la préversion des définitions d’abonnement. |  |
| [virtual-network-tap](https://github.com/Azure/azure-cli-extensions/tree/master/src/virtual-network-tap) | 0.1.0 | Gérez les taps de réseau virtuel (VTAP). | OUI |
| [virtual-wan](https://github.com/Azure/azure-cli-extensions/tree/master/src/virtual-wan) | 0.1.0 | Gérez le WAN virtuel, les hubs, les passerelles VPN et les sites VPN. | OUI |
| [vm-repair](https://github.com/Azure/azure-cli-extensions/tree/master/src/vm-repair) | 0.1.1 | Commandes de réparation automatique pour réparer les machines virtuelles. |  |
| [webapp](https://github.com/Azure/azure-cli-extensions/tree/master/src/webapp) | 0.2.19 | Commandes supplémentaires pour Azure AppService. | OUI |