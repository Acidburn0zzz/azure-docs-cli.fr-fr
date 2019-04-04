---
title: Vue d’ensemble d’Azure CLI
description: Vue d’ensemble de l’interface de ligne de commande Azure (CLI).
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/07/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 3b9589c769a90e82c35aa64c583dffdac4e4f063
ms.sourcegitcommit: 1987a39809f9865034b27130e56f30b2bd1eb72c
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/19/2019
ms.locfileid: "56421981"
---
# <a name="azure-command-line-interface-cli"></a>Interface de ligne de commande Azure (CLI)

L’interface de ligne de commande Azure (CLI) est l’interface de ligne de commande multiplateforme de Microsoft pour la gestion de ressources Azure.
Vous pouvez l’utiliser dans votre navigateur avec [Azure Cloud Shell](/azure/cloud-shell/overview) ou l’[installer](install-azure-cli.md) sur macOS, Linux ou Windows et l’exécuter à partir de la ligne de commande.

L’interface Azure CLI est facile à prendre en main et convient parfaitement pour la création de scripts d’automatisation qui fonctionnent avec Azure Resource Manager.
Pour créer des machines virtuelles dans Azure, avec Azure CLI, il vous suffit de taper la commande suivante :

```azurecli-interactive
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS
```

> [!NOTE]
>
> Dans les scripts et sur le site de documentation de Microsoft, les exemples Azure CLI sont écrits pour l’interpréteur de commandes `bash`. Les exemples d’une ligne seront exécutés sur n’importe quelle plateforme. Les exemples plus longs qui se répartissent sur plusieurs lignes (`\`) ou incluent l’attribution de variables doivent être modifiés pour fonctionner sur d’autres interpréteurs de commandes, y compris PowerShell.

## <a name="run-or-install"></a>Exécuter ou installer

Vous pouvez installer l’interface CLI localement, et l’exécuter dans le navigateur avec Azure Cloud Shell, ou bien de l’exécuter dans un conteneur Docker. Pour obtenir la version actuelle de l’interface CLI, exécutez `az --version`.

* Pour l’exécuter dans votre navigateur avec Azure Cloud Shell, consultez le [démarrage rapide de Bash dans Azure Cloud Shell](/azure/cloud-shell/quickstart) ou le [démarrage rapide de PowerShell dans Azure Cloud Shell](/azure/cloud-shell/quickstart-powershell).
* Pour installer l’interface de ligne de commande, consultez la section [Installer Azure CLI](install-azure-cli.md).
* Pour exécuter cette interface comme un conteneur Docker, consultez [Exécuter Azure CLI dans un conteneur Docker](run-azure-cli-docker.md)

## <a name="build-your-skills-with-microsoft-learn"></a>Développer vos compétences avec Microsoft Learn

- [Gérer des machines virtuelles avec Azure CLI](/learn/modules/manage-virtual-machines-with-azure-cli/)
- [Contrôler des services Azure avec l’interface CLI](/learn/modules/control-azure-services-with-cli/)
- [Plus de formations interactives...](/learn/browse/?products=azure-clis)

## <a name="get-started"></a>Prise en main

Lisez l’article [Bien démarrer](get-started-with-azure-cli.md) pour apprendre les bases de l’interface CLI. Les exemples suivants illustrent quelques cas d’utilisations courantes :

- [Machines virtuelles Linux](/azure/virtual-machines/virtual-machines-linux-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [Machines virtuelles Windows](/azure/virtual-machines/virtual-machines-windows-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [Web Apps](/azure/app-service-web/app-service-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [Base de données SQL](/azure/sql-database/sql-database-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)

Une [référence](/cli/azure/reference-index) détaillée est également disponible. Elle explique comment utiliser chacune des commandes Azure CLI.

> [!NOTE]
> Si vous utilisez la version précédente de l’interface de ligne de commande (Azure CLI Classic), vous pouvez continuer à l’utiliser.
> Cependant, nous vous recommandons de la mettre à jour pour utiliser la dernière version d’Azure CLI afin de bénéficier d’une expérience optimale.
> Si vous utilisez les deux interfaces de ligne de commande, n’oubliez pas que `azure` correspond à l’interface CLI classique et que `az` correspond l’interface CLI la plus récente.
