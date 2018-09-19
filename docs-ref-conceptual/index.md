---
title: Vue d’ensemble d’Azure CLI 2.0
description: Vue d’ensemble d’Azure CLI 2.0.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/07/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 55c5ea3ad69df60d211cc076e3570e9f07040af7
ms.sourcegitcommit: 0e688704889fc88b91588bb6678a933c2d54f020
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/11/2018
ms.locfileid: "44388383"
---
# <a name="azure-cli-20"></a><span data-ttu-id="64737-103">Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="64737-103">Azure CLI 2.0</span></span>

<span data-ttu-id="64737-104">Azure CLI 2.0 est l’interface de ligne de commande multiplateforme de Microsoft pour la gestion des ressources Azure.</span><span class="sxs-lookup"><span data-stu-id="64737-104">The Azure CLI 2.0 is Microsoft's cross-platform command-line experience for managing Azure resources.</span></span>
<span data-ttu-id="64737-105">Vous pouvez l’utiliser dans votre navigateur avec [Azure Cloud Shell](/azure/cloud-shell/overview) ou l’[installer](install-azure-cli.md) sur macOS, Linux ou Windows et l’exécuter à partir de la ligne de commande.</span><span class="sxs-lookup"><span data-stu-id="64737-105">You can use it in your browser with [Azure Cloud Shell](/azure/cloud-shell/overview), or [install](install-azure-cli.md) it on macOS, Linux, or Windows and run it from the command line.</span></span>

<span data-ttu-id="64737-106">Azure CLI 2.0 est simple à prendre en main et convient parfaitement pour la création de scripts d’automatisation qui opèrent sur Azure Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="64737-106">Azure CLI 2.0 is simple to get started with, and best used for building automation scripts that work against the Azure Resource Manager.</span></span> <span data-ttu-id="64737-107">Pour créer des machines virtuelles dans Azure avec Azure CLI 2.0, il vous suffit de taper la commande suivante :</span><span class="sxs-lookup"><span data-stu-id="64737-107">Using the Azure CLI 2.0, you can create VMs within Azure as easily as typing the following command:</span></span>

```azurecli-interactive
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS
```

## <a name="run-or-install"></a><span data-ttu-id="64737-108">Exécuter ou installer</span><span class="sxs-lookup"><span data-stu-id="64737-108">Run or Install</span></span>

<span data-ttu-id="64737-109">Vous pouvez installer l’interface CLI localement, et l’exécuter dans le navigateur avec Azure Cloud Shell, ou bien de l’exécuter dans un conteneur Docker.</span><span class="sxs-lookup"><span data-stu-id="64737-109">You can install the CLI locally, run it in the browser with Azure Cloud Shell, or run in a Docker container.</span></span>

* <span data-ttu-id="64737-110">Pour l’exécuter dans votre navigateur avec Azure Cloud Shell, consultez le [démarrage rapide de Bash dans Azure Cloud Shell](/azure/cloud-shell/quickstart) ou le [démarrage rapide de PowerShell dans Azure Cloud Shell](/azure/cloud-shell/quickstart-powershell).</span><span class="sxs-lookup"><span data-stu-id="64737-110">To run in your browser with Azure Cloud Shell, see [Quickstart for Bash in Azure Cloud Shell](/azure/cloud-shell/quickstart) or [Quickstart for PowerShell in Azure Cloud Shell](/azure/cloud-shell/quickstart-powershell).</span></span>
* <span data-ttu-id="64737-111">Pour installer Azure CLI, consultez la section [Installer l’interface Azure CLI 2.0](install-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="64737-111">To install the CLI, see [Install the Azure CLI 2.0](install-azure-cli.md).</span></span>
* <span data-ttu-id="64737-112">Pour s’exécuter comme un conteneur Docker, consultez la section [Exécuter Azure CLI 2.0 dans un conteneur Docker](run-azure-cli-docker.md)</span><span class="sxs-lookup"><span data-stu-id="64737-112">To run as a Docker container, see [Run Azure CLI 2.0 in a Docker Container](run-azure-cli-docker.md)</span></span>

## <a name="get-started"></a><span data-ttu-id="64737-113">Prise en main</span><span class="sxs-lookup"><span data-stu-id="64737-113">Get started</span></span>

<span data-ttu-id="64737-114">Lisez l’article [Bien démarrer](get-started-with-azure-cli.md) pour apprendre les bases de l’interface CLI.</span><span class="sxs-lookup"><span data-stu-id="64737-114">Read the [Get Started](get-started-with-azure-cli.md) article to learn the CLI basics.</span></span> <span data-ttu-id="64737-115">Les exemples suivants illustrent quelques cas d’utilisations courantes :</span><span class="sxs-lookup"><span data-stu-id="64737-115">The following samples demonstrate some common uses cases:</span></span>

- [<span data-ttu-id="64737-116">Machines virtuelles Linux</span><span class="sxs-lookup"><span data-stu-id="64737-116">Linux Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-linux-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="64737-117">Machines virtuelles Windows</span><span class="sxs-lookup"><span data-stu-id="64737-117">Windows Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-windows-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="64737-118">Web Apps</span><span class="sxs-lookup"><span data-stu-id="64737-118">Web Apps</span></span>](/azure/app-service-web/app-service-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="64737-119">Base de données SQL</span><span class="sxs-lookup"><span data-stu-id="64737-119">SQL Database</span></span>](/azure/sql-database/sql-database-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)

<span data-ttu-id="64737-120">Une [référence](/cli/azure/reference-index) détaillée est également disponible. Elle explique comment utiliser chacune des commandes Azure CLI 2.0.</span><span class="sxs-lookup"><span data-stu-id="64737-120">A detailed [reference](/cli/azure/reference-index) is also available that documents how to use each individual Azure CLI 2.0 command.</span></span>

> [!NOTE]
> <span data-ttu-id="64737-121">Si vous utilisez la version précédente de l’interface de ligne de commande (Azure CLI 1.0), vous pouvez continuer à l’utiliser.</span><span class="sxs-lookup"><span data-stu-id="64737-121">If you use the previous version of the CLI (Azure CLI 1.0), you can continue to use it.</span></span>
> <span data-ttu-id="64737-122">Cependant, nous vous recommandons de la mettre à jour pour utiliser la dernière version (Azure CLI 2.0) afin de bénéficier d’une expérience optimale.</span><span class="sxs-lookup"><span data-stu-id="64737-122">However, we recommend updating to use the latest version of Azure CLI 2.0 for the best experience.</span></span>
> <span data-ttu-id="64737-123">Si vous utilisez les deux interfaces de ligne de commande, n’oubliez pas que `azure` est l’ancienne interface CLI (Azure CLI) et que `az` est la nouvelle interface CLI (Azure CLI 2.0).</span><span class="sxs-lookup"><span data-stu-id="64737-123">If you use both CLIs, remember that `azure` is the old CLI - Azure CLI, and that `az` is the new CLI - Azure CLI 2.0.</span></span>
