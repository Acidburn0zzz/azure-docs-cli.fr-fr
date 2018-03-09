---
title: "Azure CLI 2.0"
description: "Vue d’ensemble d’Azure CLI 2.0."
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 02/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 98f122a9b7a33bf2270664a9e5077d4cd206a6af
ms.sourcegitcommit: 29d7366a0902488f4f4d39c2cb0e89368d5186ea
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/08/2018
---
# <a name="azure-cli-20"></a><span data-ttu-id="44c0a-103">Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="44c0a-103">Azure CLI 2.0</span></span>

<span data-ttu-id="44c0a-104">Azure CLI 2.0 est la nouvelle expérience de ligne de commande Azure pour la gestion des ressources Azure.</span><span class="sxs-lookup"><span data-stu-id="44c0a-104">The Azure CLI 2.0 is Azure's new command-line experience for managing Azure resources.</span></span>
<span data-ttu-id="44c0a-105">Vous pouvez l’utiliser dans votre navigateur avec [Azure Cloud Shell](/azure/cloud-shell/overview) ou [l’installer](install-azure-cli.md) sur macOS, Linux et Windows et l’exécuter à partir de la ligne de commande.</span><span class="sxs-lookup"><span data-stu-id="44c0a-105">You can use it in your browser with [Azure Cloud Shell](/azure/cloud-shell/overview), or you can [install](install-azure-cli.md) it on macOS, Linux, and Windows and run it from the command line.</span></span>

<span data-ttu-id="44c0a-106">Azure CLI 2.0 est optimisé pour la gestion et l’administration des ressources Azure à partir de la ligne de commande, et pour la création de scripts d’automatisation qui opèrent sur Azure Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="44c0a-106">Azure CLI 2.0 is optimized for managing and administering Azure resources from the command line, and for building automation scripts that work against the Azure Resource Manager.</span></span> <span data-ttu-id="44c0a-107">Pour créer des machines virtuelles dans Azure avec Azure CLI 2.0, il vous suffit de taper la commande suivante :</span><span class="sxs-lookup"><span data-stu-id="44c0a-107">Using the Azure CLI 2.0, you can create VMs within Azure as easily as typing the following command:</span></span>

```azurecli-interactive
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS
```

<span data-ttu-id="44c0a-108">Utilisez [Cloud Shell](/azure/cloud-shell/overview) pour exécuter l’interface CLI dans votre navigateur ou [l’installer](install-azure-cli.md) sur macOS, Linux ou Windows.</span><span class="sxs-lookup"><span data-stu-id="44c0a-108">Use the [Cloud Shell](/azure/cloud-shell/overview) to run the CLI in your browser, or [install](install-azure-cli.md) it on macOS, Linux, or Windows.</span></span>
<span data-ttu-id="44c0a-109">Lisez l’article [Bien démarrer](get-started-with-azure-cli.md) pour commencer à utiliser l’interface de ligne de commande.</span><span class="sxs-lookup"><span data-stu-id="44c0a-109">Read the [Get Started](get-started-with-azure-cli.md) article to begin using the CLI.</span></span>
<span data-ttu-id="44c0a-110">Pour plus d’informations sur la version la plus récente, consultez les [notes de publication](release-notes-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="44c0a-110">For information about the latest release, see the [release notes](release-notes-azure-cli.md).</span></span>

<span data-ttu-id="44c0a-111">Les exemples suivants peuvent vous aider à comprendre comment utiliser Azure CLI 2.0 dans certains scénarios courants :</span><span class="sxs-lookup"><span data-stu-id="44c0a-111">The following samples can help you learn how to perform common scenarios with Azure CLI 2.0:</span></span>
- [<span data-ttu-id="44c0a-112">Machines virtuelles Linux</span><span class="sxs-lookup"><span data-stu-id="44c0a-112">Linux Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-linux-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="44c0a-113">Machines virtuelles Windows</span><span class="sxs-lookup"><span data-stu-id="44c0a-113">Windows Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-windows-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="44c0a-114">Web Apps</span><span class="sxs-lookup"><span data-stu-id="44c0a-114">Web Apps</span></span>](/azure/app-service-web/app-service-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="44c0a-115">Base de données SQL</span><span class="sxs-lookup"><span data-stu-id="44c0a-115">SQL Database</span></span>](/azure/sql-database/sql-database-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)

<span data-ttu-id="44c0a-116">Une [référence](/cli/azure/reference-index) détaillée est également disponible. Elle explique comment utiliser chacune des commandes Azure CLI 2.0.</span><span class="sxs-lookup"><span data-stu-id="44c0a-116">A detailed [reference](/cli/azure/reference-index) is also available that documents how to use each individual Azure CLI 2.0 command.</span></span>

<span data-ttu-id="44c0a-117">[Bien démarrer avec Azure CLI 2.0](get-started-with-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="44c0a-117">[Get started](get-started-with-azure-cli.md) with Azure CLI 2.0 now.</span></span>


> [!NOTE]
> <span data-ttu-id="44c0a-118">Si vous utilisez la version précédente de l’interface de ligne de commande (Azure CLI), vous pouvez continuer à l’utiliser.</span><span class="sxs-lookup"><span data-stu-id="44c0a-118">If you use the previous version of the CLI (Azure CLI), you can continue to use it.</span></span>
> <span data-ttu-id="44c0a-119">Si vous utilisez les deux interfaces de ligne de commande, n’oubliez pas que `azure` est l’ancienne interface CLI (Azure CLI) et que `az` est la nouvelle interface CLI (Azure CLI 2.0).</span><span class="sxs-lookup"><span data-stu-id="44c0a-119">If you use both CLIs, remember that `azure` is the old CLI - Azure CLI, and that `az` is the new CLI - Azure CLI 2.0.</span></span>
