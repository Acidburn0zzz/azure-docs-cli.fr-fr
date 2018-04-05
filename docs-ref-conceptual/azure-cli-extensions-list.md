---
title: Extensions disponibles pour l’interface Azure CLI 2.0
description: Une liste complète des extensions officiellement prises en charge pour l’interface Azure CLI 2.0
author: derekbekoe
ms.author: debekoe
manager: routlaw
ms.date: 03/15/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: ceca7ed92435ab03b196e60dee37195330f6f3c7
ms.sourcegitcommit: b5a6296c006e3a44f66892729e47d7a967267d3e
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/28/2018
---
# <a name="available-extensions-for-the-azure-cli-20"></a>Extensions disponibles pour l’interface Azure CLI 2.0

Cet article comporte une liste complète des extensions disponibles pour l’interface Azure CLI 2.0 qui sont proposées et prises en charge par Microsoft.

La liste des extensions est également disponibles directement à partir de l’interface CLI. Pour l’obtenir, exécutez [az extension list-available](/cli/azure/extension?view=azure-cli-latest#az-extension-list-available) :

```azurecli
az extension list-available --output table
```

| NOM | Version | Résumé | VERSION PRÉLIMINAIRE |
|------|---------|---------|---------|
| [aem](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Gestion des extensions de surveillance Azure améliorée pour SAP. |  |
| [alias](https://github.com/Azure/azure-cli-extensions) | 0.2.0 | Prise en charge des alias de commande. |  |
| [azure-batch-cli-extensions](https://github.com/Azure/azure-batch-cli-extensions) | 2.1.0 | Commandes d’aperçu supplémentaires Azure Batch. |  |
| [azure-cli-iot-ext](https://github.com/azure/azure-iot-cli-extension) | 0.4.1 | Fourniture de la couche de commandes du plan de données pour Azure IoT Hub, IoT Edge et le service de provisionnement d’appareils IoT. |  |
| [dns](https://github.com/Azure/azure-cli-extensions) | 0.0.1 | Prise en charge de la préversion publique du DNS privé Azure. |  |
| [image-copy-extension](https://github.com/Azure/azure-cli-extensions) | 0.0.5 | Copie des images entre régions. |  |
| [managementgroups](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Prise en charge de la version préliminaire des groupes d’administration. | OUI |
| [managementpartner](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Prise en charge de la version préliminaire des groupes d’administration. | OUI |
| [rdbms](https://github.com/Azure/azure-cli-extensions) | 0.0.4 | Prise en charge d’Azure MySQL et d’Azure PostgreSQL. |  |
| [abonnement](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Prise en charge de la version préliminaire des définitions d’abonnement. | OUI |
| [webapp](https://github.com/Azure/azure-cli-extensions) | 0.2.0 | Création et déploiement des ressources appservice. | OUI |
