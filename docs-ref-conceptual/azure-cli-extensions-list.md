---
title: Extensions disponibles pour Azure CLI
description: Liste complète des extensions officiellement prises en charge pour Azure CLI.
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 11/26/2019
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 60240bd73d80a2a10f82d71c36dca90a40bff83d
ms.sourcegitcommit: 18973ac471bbd12af2c8f8fa32a233b0abe5b020
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/13/2020
ms.locfileid: "75913647"
---
# <a name="available-extensions-for-the-azure-cli"></a>Extensions disponibles pour Azure CLI

Cet article comporte une liste complète des extensions disponibles pour Azure CLI qui sont prises en charge par Microsoft.

La liste des extensions est également disponible à partir de l’interface CLI. Pour l’obtenir, exécutez [az extension list-available](/cli/azure/extension?view=azure-cli-latest#az-extension-list-available) :

```azurecli-interactive
az extension list-available --output table
```

| Name | Version | Résumé | PRÉVERSION |
|------|---------|---------|---------|
| [aem](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Gestion des extensions de surveillance Azure améliorée pour SAP |  |
| [préversion ASK](https://github.com/Azure/azure-cli-extensions/tree/master/src/aks-preview) | 0.4.23 | Fournit une préversion des fonctionnalités AKS à venir | Oui |
| [alias](https://github.com/Azure/azure-cli-extensions) | 0.5.2 | Prise en charge des alias de commande | Oui |
| [appconfig](https://github.com/Azure/azure-cli-extensions) | 0.5.0 | Fournit une préversion des fonctionnalités App Configuration à venir. | Oui |
| [application-insights](https://github.com/Azure/azure-cli-extensions/tree/master/src/application-insights) | 0.1.1 | Prise en charge de la gestion des composants Application Insights et de l’interrogation des métriques, des événements et des journaux de ces composants. | Oui |
| [azure-batch-cli-extensions](https://github.com/Azure/azure-batch-cli-extensions) | 5.0.0 | Commandes supplémentaires pour travailler avec le service Azure Batch |  |
| [azure-cli-iot-ext](https://github.com/azure/azure-iot-cli-extension) | 0.8.6 | Fourniture de la couche de commandes du plan de données pour Azure IoT Hub, IoT Edge et le service de provisionnement d’appareils IoT |  |
| [azure-cli-ml](https://docs.microsoft.com/azure/machine-learning/service/) | 1.0.76 | Module de commande AzureML des outils en ligne de commande Microsoft Azure |  |
| [azure-devops](https://github.com/Microsoft/azure-devops-cli-extension) | 0.15.0 | Outils de gestion Azure DevOps. |  |
| [azure-firewall](https://github.com/Azure/azure-cli-extensions/tree/master/src/azure-firewall) | 0.1.5 | Gérez les ressources de pare-feu Azure. | Oui |
| [connectedmachine](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Extension Connectedmachine des outils en ligne de commande Microsoft Azure | Oui |
| [db-up](https://github.com/Azure/azure-cli-extensions/tree/master/src/db-up) | 0.1.13 | Commandes supplémentaires pour simplifier les workflows Azure Database. | Oui |
| [dev-spaces](https://github.com/Azure/azure-cli-extensions) | 1.0.3 | Dev Spaces offre aux équipes une expérience de développement Kubernetes rapide et itérative. |  |
| [dev-spaces-preview](https://github.com/Azure/azure-cli-extensions) | 0.1.6 | Dev Spaces offre aux équipes une expérience de développement Kubernetes rapide et itérative. | Oui |
| [dms-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/dms-preview) | 0.9.0 | Prise en charge de nouveaux scénarios de Database Migration Service. | Oui |
| [dns](https://github.com/Azure/azure-cli-extensions) | 0.0.2 | Une extension Azure CLI pour les zones DNS |  |
| [eventgrid](https://github.com/Azure/azure-cli-extensions) | 0.4.4 | Module de commande EventGrid des outils de ligne de commande Microsoft Azure. | Oui |
| [express-route](https://github.com/Azure/azure-cli-extensions/tree/master/src/express-route) | 0.1.3 | Gérez les instances ExpressRoute avec les fonctionnalités d’évaluation. | Oui |
| [express-route-cross-connexion](https://github.com/Azure/azure-cli-extensions/tree/master/src/express-route-cross-connection) | 0.1.1 | Gérez des circuits ExpressRoute de client à l’aide d’une interconnexion ExpressRoute. |  |
| [find](https://github.com/Azure/azure-cli-extensions/tree/master/src/find) | 0.3.0 | Requêtes intelligentes pour l’obtention d’informations relatives l’interface CLI. | Oui |
| [front-door](https://github.com/Azure/azure-cli-extensions/tree/master/src/front-door) | 1.0.2 | Gérez les portes d’entrée réseau. |  |
| [hack](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Extension Microsoft Azure Command-Line Tools Hack | Oui |
| [healthcareapis](https://github.com/Azure/azure-cli-extensions) | 0.1.2 | Extension HealthCareApis pour les outils en ligne de commande Microsoft Azure |  |
| [image-copy-extension](https://github.com/Azure/azure-cli-extensions) | 0.2.1 | Prise en charge de la copie d’images de machines virtuelles managées entre régions |  |
| [interactive](https://github.com/Azure/azure-cli) | 0.4.3 | Shell interactif de ligne de commande Microsoft Azure | Oui |
| [internet-analyzer](https://github.com/Azure/azure-cli-extensions) | 0.1.0rc4 | Extension Internet Analyzer des outils en ligne de commande Microsoft Azure | Oui |
| [ip-group](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Extension IpGroup des outils en ligne de commande Microsoft Azure |  |
| [keyvault-preview](https://github.com/Azure/azure-keyvault-cli-extension) | 0.1.3 | Préversion des commandes Azure Key Vault. | Oui |
| [log-analytics](https://github.com/Azure/azure-cli-extensions/tree/master/src/log-analytics) | 0.1.4 | Prise en charge des fonctionnalités de requête d’Azure Log Analytics. | Oui |
| [maintenance](https://github.com/Azure/azure-cli-extensions) | 1.0.0 | Prise en charge de la préversion de la gestion de la maintenance Azure. | Oui |
| [managementgroups](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Une extension Azure CLI pour les groupes d’administration |  |
| [managementpartner](https://github.com/Azure/azure-cli-extensions) | 0.1.2 | Prise en charge de la préversion des groupes d’administration |  |
| [mesh](https://github.com/Azure/azure-cli-extensions) | 0.10.6 | Prise en charge de Microsoft Azure Service Fabric Mesh - préversion publique | Oui |
| [mixed-reality](https://github.com/Azure/azure-cli-extensions) | 0.0.1 | Extension Mixed Reality d’Azure CLI. |  |
| [netappfiles-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/netappfiles-preview) | 0.3.2 | Fournit un aperçu des fonctionnalités Azure NetApp Files (ANF) à venir. | Oui |
| [peering](https://github.com/Azure/azure-cli-extensions) | 0.1.0rc1 | Extension Peering des outils en ligne de commande Microsoft Azure | Oui |
| [privatedns](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Commandes permettant de gérer les zones DNS privées | Oui |
| [resource-graph](https://github.com/Azure/azure-cli-extensions/tree/master/src/resource-graph) | 1.0.0 | Assistance pour interroger des ressources Azure avec Resource Graph. |  |
| [sap-hana](https://github.com/Azure/azure-hanaonazure-cli-extension) | 0.5.5 | Commandes supplémentaires pour travailler avec les instances SAP HanaOnAzure. |  |
| [spring-cloud](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Extension spring-cloud des outils en ligne de commande Microsoft Azure | Oui |
| [storage-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/storage-preview) | 0.2.10 | Fournit un aperçu des fonctionnalités de stockage à venir. | Oui |
| [subscription](https://github.com/Azure/azure-cli-extensions) | 0.1.3 | Prise en charge de la préversion des définitions d’abonnement. |  |
| [virtual-network-tap](https://github.com/Azure/azure-cli-extensions/tree/master/src/virtual-network-tap) | 0.1.0 | Gérez les taps de réseau virtuel (VTAP). | Oui |
| [virtual-wan](https://github.com/Azure/azure-cli-extensions/tree/master/src/virtual-wan) | 0.1.2 | Gérez le WAN virtuel, les hubs, les passerelles VPN et les sites VPN. | Oui |
| [vm-repair](https://github.com/Azure/azure-cli-extensions/tree/master/src/vm-repair) | 0.2.3 | Commandes de réparation automatique pour réparer les machines virtuelles. |  |
| [vmware-cs](https://github.com/Azure/az-vmware-cli) | 0.2.0 | Gérez la solution VMware Azure. | Oui |
| [webapp](https://github.com/Azure/azure-cli-extensions/tree/master/src/webapp) | 0.2.24 | Commandes supplémentaires pour Azure AppService. | Oui |