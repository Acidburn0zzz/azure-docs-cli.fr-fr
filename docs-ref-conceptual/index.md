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
ms.openlocfilehash: 285567b00d8c303af3e78a01dc80946a08e4e8f8
ms.sourcegitcommit: 614811ea63ceb0e71bd99323846dc1b754e15255
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/28/2018
ms.locfileid: "53805905"
---
# <a name="azure-command-line-interface-cli"></a><span data-ttu-id="f6c2c-103">Interface de ligne de commande Azure (CLI)</span><span class="sxs-lookup"><span data-stu-id="f6c2c-103">Azure Command-Line Interface (CLI)</span></span>

<span data-ttu-id="f6c2c-104">L’interface de ligne de commande Azure (CLI) est l’interface de ligne de commande multiplateforme de Microsoft pour la gestion de ressources Azure.</span><span class="sxs-lookup"><span data-stu-id="f6c2c-104">The Azure command-line interface (CLI) is Microsoft's cross-platform command-line experience for managing Azure resources.</span></span>
<span data-ttu-id="f6c2c-105">Vous pouvez l’utiliser dans votre navigateur avec [Azure Cloud Shell](/azure/cloud-shell/overview) ou l’[installer](install-azure-cli.md) sur macOS, Linux ou Windows et l’exécuter à partir de la ligne de commande.</span><span class="sxs-lookup"><span data-stu-id="f6c2c-105">Use it in your browser with [Azure Cloud Shell](/azure/cloud-shell/overview), or [install](install-azure-cli.md) it on macOS, Linux, or Windows and run it from the command line.</span></span>

<span data-ttu-id="f6c2c-106">L’interface Azure CLI est facile à prendre en main et convient parfaitement pour la création de scripts d’automatisation qui fonctionnent avec Azure Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="f6c2c-106">The Azure CLI is easy to get started with, and best used for building automation scripts that work with the Azure Resource Manager.</span></span>
<span data-ttu-id="f6c2c-107">Pour créer des machines virtuelles dans Azure, avec Azure CLI, il vous suffit de taper la commande suivante :</span><span class="sxs-lookup"><span data-stu-id="f6c2c-107">Using the Azure CLI, you can create VMs within Azure as easily as typing the following command:</span></span>

```azurecli-interactive
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS
```

> [!NOTE]
>
> <span data-ttu-id="f6c2c-108">Dans les scripts et sur le site de documentation de Microsoft, les exemples Azure CLI sont écrits pour l’interpréteur de commandes `bash`.</span><span class="sxs-lookup"><span data-stu-id="f6c2c-108">In scripts and on the Microsoft documentation site, Azure CLI examples are written for the `bash` shell.</span></span> <span data-ttu-id="f6c2c-109">Les exemples d’une ligne seront exécutés sur n’importe quelle plateforme.</span><span class="sxs-lookup"><span data-stu-id="f6c2c-109">One-line examples will run on any platform.</span></span> <span data-ttu-id="f6c2c-110">Les exemples plus longs qui se répartissent sur plusieurs lignes (`\`) ou incluent l’attribution de variables doivent être modifiés pour fonctionner sur d’autres interpréteurs de commandes, y compris PowerShell.</span><span class="sxs-lookup"><span data-stu-id="f6c2c-110">Longer examples which include line continutions (`\`) or variable assignment need to be modified to work on other shells, including PowerShell.</span></span>

## <a name="run-or-install"></a><span data-ttu-id="f6c2c-111">Exécuter ou installer</span><span class="sxs-lookup"><span data-stu-id="f6c2c-111">Run or Install</span></span>

<span data-ttu-id="f6c2c-112">Vous pouvez installer l’interface CLI localement, et l’exécuter dans le navigateur avec Azure Cloud Shell, ou bien de l’exécuter dans un conteneur Docker.</span><span class="sxs-lookup"><span data-stu-id="f6c2c-112">You can install the CLI locally, run it in the browser with Azure Cloud Shell, or run in a Docker container.</span></span>

* <span data-ttu-id="f6c2c-113">Pour l’exécuter dans votre navigateur avec Azure Cloud Shell, consultez le [démarrage rapide de Bash dans Azure Cloud Shell](/azure/cloud-shell/quickstart) ou le [démarrage rapide de PowerShell dans Azure Cloud Shell](/azure/cloud-shell/quickstart-powershell).</span><span class="sxs-lookup"><span data-stu-id="f6c2c-113">To run in your browser with Azure Cloud Shell, see [Quickstart for Bash in Azure Cloud Shell](/azure/cloud-shell/quickstart) or [Quickstart for PowerShell in Azure Cloud Shell](/azure/cloud-shell/quickstart-powershell).</span></span>
* <span data-ttu-id="f6c2c-114">Pour installer l’interface de ligne de commande, consultez la section [Installer Azure CLI](install-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="f6c2c-114">To install the CLI, see [Install the Azure CLI](install-azure-cli.md).</span></span>
* <span data-ttu-id="f6c2c-115">Pour exécuter cette interface comme un conteneur Docker, consultez [Exécuter Azure CLI dans un conteneur Docker](run-azure-cli-docker.md)</span><span class="sxs-lookup"><span data-stu-id="f6c2c-115">To run as a Docker container, see [Run Azure CLI in a Docker Container](run-azure-cli-docker.md)</span></span>

## <a name="build-your-skills-with-microsoft-learn"></a><span data-ttu-id="f6c2c-116">Développer vos compétences avec Microsoft Learn</span><span class="sxs-lookup"><span data-stu-id="f6c2c-116">Build your skills with Microsoft Learn</span></span>

- [<span data-ttu-id="f6c2c-117">Gérer des machines virtuelles avec Azure CLI</span><span class="sxs-lookup"><span data-stu-id="f6c2c-117">Manage virtual machines with the Azure CLI</span></span>](/learn/modules/manage-virtual-machines-with-azure-cli/)
- [<span data-ttu-id="f6c2c-118">Contrôler des services Azure avec l’interface CLI</span><span class="sxs-lookup"><span data-stu-id="f6c2c-118">Control Azure services with the CLI</span></span>](/learn/modules/control-azure-services-with-cli/)
- [<span data-ttu-id="f6c2c-119">Plus de formations interactives...</span><span class="sxs-lookup"><span data-stu-id="f6c2c-119">More interactive learning...</span></span>](/learn/browse/?products=azure-clis)

## <a name="get-started"></a><span data-ttu-id="f6c2c-120">Prise en main</span><span class="sxs-lookup"><span data-stu-id="f6c2c-120">Get started</span></span>

<span data-ttu-id="f6c2c-121">Lisez l’article [Bien démarrer](get-started-with-azure-cli.md) pour apprendre les bases de l’interface CLI.</span><span class="sxs-lookup"><span data-stu-id="f6c2c-121">Read the [Get Started](get-started-with-azure-cli.md) article to learn the CLI basics.</span></span> <span data-ttu-id="f6c2c-122">Les exemples suivants illustrent quelques cas d’utilisations courantes :</span><span class="sxs-lookup"><span data-stu-id="f6c2c-122">The following samples demonstrate some common uses cases:</span></span>

- [<span data-ttu-id="f6c2c-123">Machines virtuelles Linux</span><span class="sxs-lookup"><span data-stu-id="f6c2c-123">Linux Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-linux-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="f6c2c-124">Machines virtuelles Windows</span><span class="sxs-lookup"><span data-stu-id="f6c2c-124">Windows Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-windows-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="f6c2c-125">Web Apps</span><span class="sxs-lookup"><span data-stu-id="f6c2c-125">Web Apps</span></span>](/azure/app-service-web/app-service-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="f6c2c-126">Base de données SQL</span><span class="sxs-lookup"><span data-stu-id="f6c2c-126">SQL Database</span></span>](/azure/sql-database/sql-database-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)

<span data-ttu-id="f6c2c-127">Une [référence](/cli/azure/reference-index) détaillée est également disponible. Elle explique comment utiliser chacune des commandes Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="f6c2c-127">A detailed [reference](/cli/azure/reference-index) is also available that documents how to use each individual Azure CLI command.</span></span>

> [!NOTE]
> <span data-ttu-id="f6c2c-128">Si vous utilisez la version précédente de l’interface de ligne de commande (Azure CLI Classic), vous pouvez continuer à l’utiliser.</span><span class="sxs-lookup"><span data-stu-id="f6c2c-128">If you use the previous version of the CLI (Azure classic CLI), you can continue to use it.</span></span>
> <span data-ttu-id="f6c2c-129">Cependant, nous vous recommandons de la mettre à jour pour utiliser la dernière version d’Azure CLI afin de bénéficier d’une expérience optimale.</span><span class="sxs-lookup"><span data-stu-id="f6c2c-129">However, we recommend updating to use the latest version of the Azure CLI for the best experience.</span></span>
> <span data-ttu-id="f6c2c-130">Si vous utilisez les deux interfaces de ligne de commande, n’oubliez pas que `azure` correspond à l’interface CLI classique et que `az` correspond l’interface CLI la plus récente.</span><span class="sxs-lookup"><span data-stu-id="f6c2c-130">If you use both CLIs, remember that `azure` is the classic CLI and that `az` is the most recent CLI.</span></span>
