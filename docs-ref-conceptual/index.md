---
title: Vue d’ensemble d’Azure CLI
description: Vue d’ensemble d’Azure CLI.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/07/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 8ab8435f2d8337f63a73aef39472646dc8ebcd74
ms.sourcegitcommit: 0d6b08048b5b35bf0bb3d7b91ff567adbaab2a8b
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/07/2018
ms.locfileid: "51222291"
---
# <a name="azure-cli"></a><span data-ttu-id="5a92b-103">Azure CLI</span><span class="sxs-lookup"><span data-stu-id="5a92b-103">Azure CLI</span></span>

<span data-ttu-id="5a92b-104">Azure CLI est l’interface de ligne de commande multiplateforme de Microsoft pour la gestion de ressources Azure.</span><span class="sxs-lookup"><span data-stu-id="5a92b-104">The Azure CLI is Microsoft's cross-platform command-line experience for managing Azure resources.</span></span>
<span data-ttu-id="5a92b-105">Vous pouvez l’utiliser dans votre navigateur avec [Azure Cloud Shell](/azure/cloud-shell/overview) ou l’[installer](install-azure-cli.md) sur macOS, Linux ou Windows et l’exécuter à partir de la ligne de commande.</span><span class="sxs-lookup"><span data-stu-id="5a92b-105">You can use it in your browser with [Azure Cloud Shell](/azure/cloud-shell/overview), or [install](install-azure-cli.md) it on macOS, Linux, or Windows and run it from the command line.</span></span>

<span data-ttu-id="5a92b-106">Azure CLI est simple à prendre en main et convient parfaitement pour la création de scripts d’automatisation qui fonctionnent sur Azure Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="5a92b-106">The Azure CLI is simple to get started with, and best used for building automation scripts that work against the Azure Resource Manager.</span></span> <span data-ttu-id="5a92b-107">Pour créer des machines virtuelles dans Azure, avec Azure CLI, il vous suffit de taper la commande suivante :</span><span class="sxs-lookup"><span data-stu-id="5a92b-107">Using the Azure CLI, you can create VMs within Azure as easily as typing the following command:</span></span>

```azurecli-interactive
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS
```

> [!NOTE]
>
> <span data-ttu-id="5a92b-108">Dans les scripts et sur le site de documentation de Microsoft, les exemples Azure CLI sont écrits pour l’interpréteur de commandes `bash`.</span><span class="sxs-lookup"><span data-stu-id="5a92b-108">In scripts and on the Microsoft documentation site, Azure CLI examples are written for the `bash` shell.</span></span> <span data-ttu-id="5a92b-109">Les exemples d’une ligne seront exécutés sur n’importe quelle plateforme.</span><span class="sxs-lookup"><span data-stu-id="5a92b-109">One-line examples will run on any platform.</span></span> <span data-ttu-id="5a92b-110">Les exemples plus longs ou plus complexes qui se répartissent sur plusieurs lignes (`\`) ou incluent l’attribution de variables doivent être modifiés pour fonctionner sur d’autres interpréteurs de commandes, y compris PowerShell.</span><span class="sxs-lookup"><span data-stu-id="5a92b-110">Longer or more complicated examples which include line continutions (`\`) or variable assignment will need to be modified to work on other shells, including PowerShell.</span></span>

## <a name="run-or-install"></a><span data-ttu-id="5a92b-111">Exécuter ou installer</span><span class="sxs-lookup"><span data-stu-id="5a92b-111">Run or Install</span></span>

<span data-ttu-id="5a92b-112">Vous pouvez installer l’interface CLI localement, et l’exécuter dans le navigateur avec Azure Cloud Shell, ou bien de l’exécuter dans un conteneur Docker.</span><span class="sxs-lookup"><span data-stu-id="5a92b-112">You can install the CLI locally, run it in the browser with Azure Cloud Shell, or run in a Docker container.</span></span>

* <span data-ttu-id="5a92b-113">Pour l’exécuter dans votre navigateur avec Azure Cloud Shell, consultez le [démarrage rapide de Bash dans Azure Cloud Shell](/azure/cloud-shell/quickstart) ou le [démarrage rapide de PowerShell dans Azure Cloud Shell](/azure/cloud-shell/quickstart-powershell).</span><span class="sxs-lookup"><span data-stu-id="5a92b-113">To run in your browser with Azure Cloud Shell, see [Quickstart for Bash in Azure Cloud Shell](/azure/cloud-shell/quickstart) or [Quickstart for PowerShell in Azure Cloud Shell](/azure/cloud-shell/quickstart-powershell).</span></span>
* <span data-ttu-id="5a92b-114">Pour installer l’interface de ligne de commande, consultez la section [Installer Azure CLI](install-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="5a92b-114">To install the CLI, see [Install the Azure CLI](install-azure-cli.md).</span></span>
* <span data-ttu-id="5a92b-115">Pour exécuter cette interface comme un conteneur Docker, consultez [Exécuter Azure CLI dans un conteneur Docker](run-azure-cli-docker.md)</span><span class="sxs-lookup"><span data-stu-id="5a92b-115">To run as a Docker container, see [Run Azure CLI in a Docker Container](run-azure-cli-docker.md)</span></span>

## <a name="build-your-skills-with-microsoft-learn"></a><span data-ttu-id="5a92b-116">Développer vos compétences avec Microsoft Learn</span><span class="sxs-lookup"><span data-stu-id="5a92b-116">Build your skills with Microsoft Learn</span></span>

- [<span data-ttu-id="5a92b-117">Gérer des machines virtuelles avec Azure CLI</span><span class="sxs-lookup"><span data-stu-id="5a92b-117">Manage virtual machines with the Azure CLI</span></span>](/learn/modules/manage-virtual-machines-with-azure-cli/)
- [<span data-ttu-id="5a92b-118">Contrôler des services Azure avec l’interface CLI</span><span class="sxs-lookup"><span data-stu-id="5a92b-118">Control Azure services with the CLI</span></span>](/learn/modules/control-azure-services-with-cli/)
- [<span data-ttu-id="5a92b-119">Plus de formations interactives...</span><span class="sxs-lookup"><span data-stu-id="5a92b-119">More interactive learning...</span></span>](/learn/browse/?products=azure-clis)

## <a name="get-started"></a><span data-ttu-id="5a92b-120">Prise en main</span><span class="sxs-lookup"><span data-stu-id="5a92b-120">Get started</span></span>

<span data-ttu-id="5a92b-121">Lisez l’article [Bien démarrer](get-started-with-azure-cli.md) pour apprendre les bases de l’interface CLI.</span><span class="sxs-lookup"><span data-stu-id="5a92b-121">Read the [Get Started](get-started-with-azure-cli.md) article to learn the CLI basics.</span></span> <span data-ttu-id="5a92b-122">Les exemples suivants illustrent quelques cas d’utilisations courantes :</span><span class="sxs-lookup"><span data-stu-id="5a92b-122">The following samples demonstrate some common uses cases:</span></span>

- [<span data-ttu-id="5a92b-123">Machines virtuelles Linux</span><span class="sxs-lookup"><span data-stu-id="5a92b-123">Linux Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-linux-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="5a92b-124">Machines virtuelles Windows</span><span class="sxs-lookup"><span data-stu-id="5a92b-124">Windows Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-windows-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="5a92b-125">Web Apps</span><span class="sxs-lookup"><span data-stu-id="5a92b-125">Web Apps</span></span>](/azure/app-service-web/app-service-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="5a92b-126">Base de données SQL</span><span class="sxs-lookup"><span data-stu-id="5a92b-126">SQL Database</span></span>](/azure/sql-database/sql-database-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)

<span data-ttu-id="5a92b-127">Une [référence](/cli/azure/reference-index) détaillée est également disponible. Elle explique comment utiliser chacune des commandes Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="5a92b-127">A detailed [reference](/cli/azure/reference-index) is also available that documents how to use each individual Azure CLI command.</span></span>

> [!NOTE]
> <span data-ttu-id="5a92b-128">Si vous utilisez la version précédente de l’interface de ligne de commande (Azure CLI Classic), vous pouvez continuer à l’utiliser.</span><span class="sxs-lookup"><span data-stu-id="5a92b-128">If you use the previous version of the CLI (Azure classic CLI), you can continue to use it.</span></span>
> <span data-ttu-id="5a92b-129">Cependant, nous vous recommandons de la mettre à jour pour utiliser la dernière version d’Azure CLI afin de bénéficier d’une expérience optimale.</span><span class="sxs-lookup"><span data-stu-id="5a92b-129">However, we recommend updating to use the latest version of the Azure CLI for the best experience.</span></span>
> <span data-ttu-id="5a92b-130">Si vous utilisez les deux interfaces de ligne de commande, n’oubliez pas que `azure` correspond à l’interface CLI classique et que `az` correspond l’interface CLI la plus récente.</span><span class="sxs-lookup"><span data-stu-id="5a92b-130">If you use both CLIs, remember that `azure` is the classic CLI and that `az` is the most recent CLI.</span></span>
