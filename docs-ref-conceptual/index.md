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
ms.openlocfilehash: 047a953a0ab8ccaf145d56e4d774d2bf9852ed6f
ms.sourcegitcommit: c4462456dfb17993f098d47c37bc19f4d78b8179
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/25/2018
ms.locfileid: "47177723"
---
# <a name="azure-cli"></a><span data-ttu-id="b9966-103">Azure CLI</span><span class="sxs-lookup"><span data-stu-id="b9966-103">Azure CLI</span></span>

<span data-ttu-id="b9966-104">Azure CLI est l’interface de ligne de commande multiplateforme de Microsoft pour la gestion de ressources Azure.</span><span class="sxs-lookup"><span data-stu-id="b9966-104">The Azure CLI is Microsoft's cross-platform command-line experience for managing Azure resources.</span></span>
<span data-ttu-id="b9966-105">Vous pouvez l’utiliser dans votre navigateur avec [Azure Cloud Shell](/azure/cloud-shell/overview) ou l’[installer](install-azure-cli.md) sur macOS, Linux ou Windows et l’exécuter à partir de la ligne de commande.</span><span class="sxs-lookup"><span data-stu-id="b9966-105">You can use it in your browser with [Azure Cloud Shell](/azure/cloud-shell/overview), or [install](install-azure-cli.md) it on macOS, Linux, or Windows and run it from the command line.</span></span>

<span data-ttu-id="b9966-106">Azure CLI est simple à prendre en main et convient parfaitement pour la création de scripts d’automatisation qui fonctionnent sur Azure Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="b9966-106">The Azure CLI is simple to get started with, and best used for building automation scripts that work against the Azure Resource Manager.</span></span> <span data-ttu-id="b9966-107">Pour créer des machines virtuelles dans Azure, avec Azure CLI, il vous suffit de taper la commande suivante :</span><span class="sxs-lookup"><span data-stu-id="b9966-107">Using the Azure CLI, you can create VMs within Azure as easily as typing the following command:</span></span>

```azurecli-interactive
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS
```

## <a name="run-or-install"></a><span data-ttu-id="b9966-108">Exécuter ou installer</span><span class="sxs-lookup"><span data-stu-id="b9966-108">Run or Install</span></span>

<span data-ttu-id="b9966-109">Vous pouvez installer l’interface CLI localement, et l’exécuter dans le navigateur avec Azure Cloud Shell, ou bien de l’exécuter dans un conteneur Docker.</span><span class="sxs-lookup"><span data-stu-id="b9966-109">You can install the CLI locally, run it in the browser with Azure Cloud Shell, or run in a Docker container.</span></span>

* <span data-ttu-id="b9966-110">Pour l’exécuter dans votre navigateur avec Azure Cloud Shell, consultez le [démarrage rapide de Bash dans Azure Cloud Shell](/azure/cloud-shell/quickstart) ou le [démarrage rapide de PowerShell dans Azure Cloud Shell](/azure/cloud-shell/quickstart-powershell).</span><span class="sxs-lookup"><span data-stu-id="b9966-110">To run in your browser with Azure Cloud Shell, see [Quickstart for Bash in Azure Cloud Shell](/azure/cloud-shell/quickstart) or [Quickstart for PowerShell in Azure Cloud Shell](/azure/cloud-shell/quickstart-powershell).</span></span>
* <span data-ttu-id="b9966-111">Pour installer l’interface de ligne de commande, consultez la section [Installer Azure CLI](install-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="b9966-111">To install the CLI, see [Install the Azure CLI](install-azure-cli.md).</span></span>
* <span data-ttu-id="b9966-112">Pour exécuter cette interface comme un conteneur Docker, consultez [Exécuter Azure CLI dans un conteneur Docker](run-azure-cli-docker.md)</span><span class="sxs-lookup"><span data-stu-id="b9966-112">To run as a Docker container, see [Run Azure CLI in a Docker Container](run-azure-cli-docker.md)</span></span>

## <a name="build-your-skills-with-microsoft-learn"></a><span data-ttu-id="b9966-113">Développer vos compétences avec Microsoft Learn</span><span class="sxs-lookup"><span data-stu-id="b9966-113">Build your skills with Microsoft Learn</span></span>

- [<span data-ttu-id="b9966-114">Gérer des machines virtuelles avec Azure CLI</span><span class="sxs-lookup"><span data-stu-id="b9966-114">Manage virtual machines with the Azure CLI</span></span>](/learn/modules/manage-virtual-machines-with-azure-cli/)
- [<span data-ttu-id="b9966-115">Contrôler des services Azure avec l’interface CLI</span><span class="sxs-lookup"><span data-stu-id="b9966-115">Control Azure services with the CLI</span></span>](/learn/modules/control-azure-services-with-cli/)
- [<span data-ttu-id="b9966-116">Plus de formations interactives...</span><span class="sxs-lookup"><span data-stu-id="b9966-116">More interactive learning...</span></span>](/learn/browse/?products=azure-clis)

## <a name="get-started"></a><span data-ttu-id="b9966-117">Prise en main</span><span class="sxs-lookup"><span data-stu-id="b9966-117">Get started</span></span>

<span data-ttu-id="b9966-118">Lisez l’article [Bien démarrer](get-started-with-azure-cli.md) pour apprendre les bases de l’interface CLI.</span><span class="sxs-lookup"><span data-stu-id="b9966-118">Read the [Get Started](get-started-with-azure-cli.md) article to learn the CLI basics.</span></span> <span data-ttu-id="b9966-119">Les exemples suivants illustrent quelques cas d’utilisations courantes :</span><span class="sxs-lookup"><span data-stu-id="b9966-119">The following samples demonstrate some common uses cases:</span></span>

- [<span data-ttu-id="b9966-120">Machines virtuelles Linux</span><span class="sxs-lookup"><span data-stu-id="b9966-120">Linux Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-linux-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="b9966-121">Machines virtuelles Windows</span><span class="sxs-lookup"><span data-stu-id="b9966-121">Windows Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-windows-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="b9966-122">Web Apps</span><span class="sxs-lookup"><span data-stu-id="b9966-122">Web Apps</span></span>](/azure/app-service-web/app-service-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="b9966-123">Base de données SQL</span><span class="sxs-lookup"><span data-stu-id="b9966-123">SQL Database</span></span>](/azure/sql-database/sql-database-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)

<span data-ttu-id="b9966-124">Une [référence](/cli/azure/reference-index) détaillée est également disponible. Elle explique comment utiliser chacune des commandes Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="b9966-124">A detailed [reference](/cli/azure/reference-index) is also available that documents how to use each individual Azure CLI command.</span></span>

> [!NOTE]
> <span data-ttu-id="b9966-125">Si vous utilisez la version précédente de l’interface de ligne de commande (Azure CLI Classic), vous pouvez continuer à l’utiliser.</span><span class="sxs-lookup"><span data-stu-id="b9966-125">If you use the previous version of the CLI (Azure classic CLI), you can continue to use it.</span></span>
> <span data-ttu-id="b9966-126">Cependant, nous vous recommandons de la mettre à jour pour utiliser la dernière version d’Azure CLI afin de bénéficier d’une expérience optimale.</span><span class="sxs-lookup"><span data-stu-id="b9966-126">However, we recommend updating to use the latest version of the Azure CLI for the best experience.</span></span>
> <span data-ttu-id="b9966-127">Si vous utilisez les deux interfaces de ligne de commande, n’oubliez pas que `azure` correspond à l’interface CLI classique et que `az` correspond l’interface CLI la plus récente.</span><span class="sxs-lookup"><span data-stu-id="b9966-127">If you use both CLIs, remember that `azure` is the classic CLI and that `az` is the most recent CLI.</span></span>
