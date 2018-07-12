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
ms.openlocfilehash: ffa435f8c6ee5aa82d2efe2e09d7bcb1f1dc434b
ms.sourcegitcommit: 64f2c628e83d687d0e172c01f13d71c8c39a8040
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/11/2018
ms.locfileid: "38967688"
---
# <a name="azure-cli-20"></a><span data-ttu-id="78707-103">Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="78707-103">Azure CLI 2.0</span></span>

<span data-ttu-id="78707-104">Azure CLI 2.0 est l’interface de ligne commande multiplateforme de Microsoft pour la gestion des ressources Azure.</span><span class="sxs-lookup"><span data-stu-id="78707-104">The Azure CLI 2.0 is Microsoft's cross-platform command line experience for managing Azure resources.</span></span>
<span data-ttu-id="78707-105">Vous pouvez l’utiliser dans votre navigateur avec [Azure Cloud Shell](/azure/cloud-shell/overview) ou l’[installer](install-azure-cli.md) sur macOS, Linux ou Windows et l’exécuter à partir de la ligne de commande.</span><span class="sxs-lookup"><span data-stu-id="78707-105">You can use it in your browser with [Azure Cloud Shell](/azure/cloud-shell/overview), or [install](install-azure-cli.md) it on macOS, Linux, or Windows and run it from the command line.</span></span>

<span data-ttu-id="78707-106">Azure CLI 2.0 est optimisé pour la gestion et l’administration des ressources Azure à partir de la ligne de commande, et pour la création de scripts d’automatisation qui opèrent sur Azure Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="78707-106">Azure CLI 2.0 is optimized for managing and administering Azure resources from the command line, and for building automation scripts that work against the Azure Resource Manager.</span></span> <span data-ttu-id="78707-107">Pour créer des machines virtuelles dans Azure avec Azure CLI 2.0, il vous suffit de taper la commande suivante :</span><span class="sxs-lookup"><span data-stu-id="78707-107">Using the Azure CLI 2.0, you can create VMs within Azure as easily as typing the following command:</span></span>

```azurecli-interactive
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS
```

<span data-ttu-id="78707-108">Utilisez [Cloud Shell](/azure/cloud-shell/overview) pour exécuter l’interface CLI dans votre navigateur ou [l’installer](install-azure-cli.md) sur macOS, Linux ou Windows.</span><span class="sxs-lookup"><span data-stu-id="78707-108">Use the [Cloud Shell](/azure/cloud-shell/overview) to run the CLI in your browser, or [install](install-azure-cli.md) it on macOS, Linux, or Windows.</span></span>
<span data-ttu-id="78707-109">Lisez l’article [Bien démarrer](get-started-with-azure-cli.md) pour commencer à utiliser l’interface de ligne de commande.</span><span class="sxs-lookup"><span data-stu-id="78707-109">Read the [Get Started](get-started-with-azure-cli.md) article to begin using the CLI.</span></span>
<span data-ttu-id="78707-110">Pour plus d’informations sur la version la plus récente, consultez les [Notes de publication](release-notes-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="78707-110">For information about the latest release, see the [release notes](release-notes-azure-cli.md).</span></span>

<span data-ttu-id="78707-111">Les exemples suivants vous aideront à vous familiariser avec les tâches courantes dans Azure CLI 2.0 :</span><span class="sxs-lookup"><span data-stu-id="78707-111">The following samples help you get started with common tasks in Azure CLI 2.0:</span></span>

- [<span data-ttu-id="78707-112">Machines virtuelles Linux</span><span class="sxs-lookup"><span data-stu-id="78707-112">Linux Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-linux-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="78707-113">Machines virtuelles Windows</span><span class="sxs-lookup"><span data-stu-id="78707-113">Windows Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-windows-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="78707-114">Web Apps</span><span class="sxs-lookup"><span data-stu-id="78707-114">Web Apps</span></span>](/azure/app-service-web/app-service-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="78707-115">Base de données SQL</span><span class="sxs-lookup"><span data-stu-id="78707-115">SQL Database</span></span>](/azure/sql-database/sql-database-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)

<span data-ttu-id="78707-116">Une [référence](/cli/azure/reference-index) détaillée est également disponible. Elle explique comment utiliser chacune des commandes Azure CLI 2.0.</span><span class="sxs-lookup"><span data-stu-id="78707-116">A detailed [reference](/cli/azure/reference-index) is also available that documents how to use each individual Azure CLI 2.0 command.</span></span>

<span data-ttu-id="78707-117">[Bien démarrer avec Azure CLI 2.0](get-started-with-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="78707-117">[Get started](get-started-with-azure-cli.md) with Azure CLI 2.0 now.</span></span>

> [!NOTE]
> <span data-ttu-id="78707-118">Si vous utilisez la version précédente de l’interface de ligne de commande (Azure CLI 1.0), vous pouvez continuer à l’utiliser.</span><span class="sxs-lookup"><span data-stu-id="78707-118">If you use the previous version of the CLI (Azure CLI 1.0), you can continue to use it.</span></span>
> <span data-ttu-id="78707-119">Cependant, nous vous recommandons de la mettre à jour pour utiliser la dernière version (Azure CLI 2.0) afin de bénéficier d’une expérience optimale.</span><span class="sxs-lookup"><span data-stu-id="78707-119">However, we recommend updating to use the latest version of Azure CLI 2.0 for the best experience.</span></span>
> <span data-ttu-id="78707-120">Si vous utilisez les deux interfaces de ligne de commande, n’oubliez pas que `azure` est l’ancienne interface CLI (Azure CLI) et que `az` est la nouvelle interface CLI (Azure CLI 2.0).</span><span class="sxs-lookup"><span data-stu-id="78707-120">If you use both CLIs, remember that `azure` is the old CLI - Azure CLI, and that `az` is the new CLI - Azure CLI 2.0.</span></span>
