---
title: Azure CLI 2.0
description: Vue d’ensemble d’Azure CLI 2.0.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/16/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 9b6f7a5c79033c0b0bec2bf8b56eb40831484f1a
ms.sourcegitcommit: 8b4629a42ceecf30c1efbc6fdddf512f4dddfab0
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/18/2018
ms.locfileid: "34306248"
---
# <a name="azure-cli-20"></a>Azure CLI 2.0

Azure CLI 2.0 est l’interface de ligne commande multiplateforme de Microsoft pour la gestion des ressources Azure.
Vous pouvez l’utiliser dans votre navigateur avec [Azure Cloud Shell](/azure/cloud-shell/overview) ou l’[installer](install-azure-cli.md) sur macOS, Linux ou Windows et l’exécuter à partir de la ligne de commande.

Azure CLI 2.0 est optimisé pour la gestion et l’administration des ressources Azure à partir de la ligne de commande, et pour la création de scripts d’automatisation qui opèrent sur Azure Resource Manager. Pour créer des machines virtuelles dans Azure avec Azure CLI 2.0, il vous suffit de taper la commande suivante :

```azurecli-interactive
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS
```

Utilisez [Cloud Shell](/azure/cloud-shell/overview) pour exécuter l’interface CLI dans votre navigateur ou [l’installer](install-azure-cli.md) sur macOS, Linux ou Windows.
Lisez l’article [Bien démarrer](get-started-with-azure-cli.md) pour commencer à utiliser l’interface de ligne de commande.
Pour plus d’informations sur la version la plus récente, consultez les [Notes de publication](release-notes-azure-cli.md).

Les exemples suivants vous aideront à vous familiariser avec les tâches courantes dans Azure CLI 2.0 :
- [Machines virtuelles Linux](/azure/virtual-machines/virtual-machines-linux-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- Interactif : [Créer des machines virtuelles Linux](https://docs.microsoft.com/learn/azure-cli-2-0/index)
- [Machines virtuelles Windows](/azure/virtual-machines/virtual-machines-windows-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [Web Apps](/azure/app-service-web/app-service-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [Base de données SQL](/azure/sql-database/sql-database-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)

Une [référence](/cli/azure/reference-index) détaillée est également disponible. Elle explique comment utiliser chacune des commandes Azure CLI 2.0.

[Bien démarrer avec Azure CLI 2.0](get-started-with-azure-cli.md).

> [!NOTE]
> Si vous utilisez la version précédente de l’interface de ligne de commande (Azure CLI 1.0), vous pouvez continuer à l’utiliser.
> Cependant, nous vous recommandons de la mettre à jour pour utiliser la dernière version (Azure CLI 2.0) afin de bénéficier d’une expérience optimale.
> Si vous utilisez les deux interfaces de ligne de commande, n’oubliez pas que `azure` est l’ancienne interface CLI (Azure CLI) et que `az` est la nouvelle interface CLI (Azure CLI 2.0).
