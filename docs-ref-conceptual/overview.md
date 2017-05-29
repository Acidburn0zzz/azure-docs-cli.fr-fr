---
title: Azure CLI 2.0
description: "Vue d’ensemble d’Azure CLI 2.0."
keywords: Azure CLI 2.0, Linux, Mac, Windows, OS X, Ubuntu, Debian, CentOS, RHEL, SUSE, CoreOS, Docker, Windows, Python, PIP
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 02/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: 80ae9f6c-adb7-483c-bfb4-fbb958e075ba
ms.openlocfilehash: 2f2fe7e8643256f72ff5dd48c784b96e53c4c281
ms.sourcegitcommit: 21c42ed07c9f7679e4860013ac5647cf31213f4e
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/22/2017
---
# <a name="azure-cli-20"></a>Azure CLI 2.0

Azure CLI 2.0 est la nouvelle expérience de ligne de commande Azure pour la gestion des ressources Azure.
Vous pouvez l’utiliser dans votre navigateur avec [Azure Cloud Shell](/azure/cloud-shell/overview) ou [l’installer](install-azure-cli.md) sur macOS, Linux et Windows et l’exécuter à partir de la ligne de commande.

Azure CLI 2.0 est optimisé pour la gestion et l’administration des ressources Azure à partir de la ligne de commande, et pour la création de scripts d’automatisation qui opèrent sur Azure Resource Manager. Pour créer des machines virtuelles dans Azure avec Azure CLI 2.0, il vous suffit de taper la commande suivante :

```azurecli
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS
```

Utilisez [Cloud Shell](/azure/cloud-shell/overview) pour exécuter l’interface CLI dans votre navigateur ou [l’installer](install-azure-cli.md) sur macOS, Linux ou Windows.
Lisez l’article [Bien démarrer](get-started-with-azure-cli.md) pour commencer à utiliser l’interface de ligne de commande.
Pour plus d’informations sur la version la plus récente, consultez les [notes de publication](release-notes-azure-cli.md).

Les exemples suivants peuvent vous aider à comprendre comment utiliser Azure CLI 2.0 dans certains scénarios courants :
- [Machines virtuelles Linux](/azure/virtual-machines/virtual-machines-linux-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [Machines virtuelles Windows](/azure/virtual-machines/virtual-machines-windows-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [Web Apps](/azure/app-service-web/app-service-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [Base de données SQL](/azure/sql-database/sql-database-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)

Une [référence](/cli/azure/) détaillée est également disponible. Elle explique comment utiliser chacune des commandes Azure CLI 2.0.

[Bien démarrer avec Azure CLI 2.0](get-started-with-azure-cli.md).


> [!NOTE]
> Si vous utilisez la version précédente de l’interface de ligne de commande (Azure CLI), vous pouvez continuer à l’utiliser.
> Si vous utilisez les deux interfaces de ligne de commande, n’oubliez pas que `azure` est l’ancienne interface CLI (Azure CLI) et que `az` est la nouvelle interface CLI (Azure CLI 2.0). 