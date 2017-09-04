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
ms.openlocfilehash: 2f4f9950dd663ae85f41bf4efe114b15770ace5d
ms.sourcegitcommit: bcf93ad8ed8802072249cd8187cd4420da89b4c6
ms.translationtype: HT
ms.contentlocale: fr-FR
---
# <a name="azure-cli-20"></a><span data-ttu-id="fd055-104">Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="fd055-104">Azure CLI 2.0</span></span>

<span data-ttu-id="fd055-105">Azure CLI 2.0 est la nouvelle expérience de ligne de commande Azure pour la gestion des ressources Azure.</span><span class="sxs-lookup"><span data-stu-id="fd055-105">The Azure CLI 2.0 is Azure's new command-line experience for managing Azure resources.</span></span>  <span data-ttu-id="fd055-106">Elle peut être utilisée sur macOS, Linux et Windows.</span><span class="sxs-lookup"><span data-stu-id="fd055-106">It can be used on macOS, Linux, and Windows.</span></span> 

<span data-ttu-id="fd055-107">Azure CLI 2.0 est optimisé pour la gestion et l’administration des ressources Azure à partir de la ligne de commande, et pour la création de scripts d’automatisation qui opèrent sur Azure Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="fd055-107">Azure CLI 2.0 is optimized for managing and administering Azure resources from the command line, and for building automation scripts that work against the Azure Resource Manager.</span></span> <span data-ttu-id="fd055-108">Pour créer des machines virtuelles dans Azure avec Azure CLI 2.0, il vous suffit de taper la commande suivante :</span><span class="sxs-lookup"><span data-stu-id="fd055-108">Using the Azure CLI 2.0, you can create VMs within Azure as easily as typing the following command:</span></span>

```azurecli
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS
```

<span data-ttu-id="fd055-109">Consultez [l’article sur l’installation](install-azure-cli.md) pour savoir comment installer et exécuter Azure CLI 2.0 sur votre système.</span><span class="sxs-lookup"><span data-stu-id="fd055-109">Review the [Install article](install-azure-cli.md) to get Azure CLI 2.0 up and running on your system.</span></span> <span data-ttu-id="fd055-110">Lisez ensuite l’article [Bien démarrer](get-started-with-azure-cli.md) pour commencer à l’utiliser.</span><span class="sxs-lookup"><span data-stu-id="fd055-110">Then read the [Get Started](get-started-with-azure-cli.md) article to begin using it.</span></span>
<span data-ttu-id="fd055-111">Pour plus d’informations sur la version la plus récente, consultez les [Notes de publication](release-notes-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="fd055-111">For information about the latest release, see the [release notes](release-notes-azure-cli.md).</span></span>

<span data-ttu-id="fd055-112">Les exemples suivants peuvent vous aider à comprendre comment utiliser Azure CLI 2.0 dans certains scénarios courants :</span><span class="sxs-lookup"><span data-stu-id="fd055-112">The following samples can help you learn how to perform common scenarios with Azure CLI 2.0:</span></span>
- [<span data-ttu-id="fd055-113">Machines virtuelles Linux</span><span class="sxs-lookup"><span data-stu-id="fd055-113">Linux Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-linux-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="fd055-114">Machines virtuelles Windows</span><span class="sxs-lookup"><span data-stu-id="fd055-114">Windows Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-windows-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="fd055-115">Web Apps</span><span class="sxs-lookup"><span data-stu-id="fd055-115">Web Apps</span></span>](/azure/app-service-web/app-service-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="fd055-116">Base de données SQL</span><span class="sxs-lookup"><span data-stu-id="fd055-116">SQL Database</span></span>](/azure/sql-database/sql-database-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)

<span data-ttu-id="fd055-117">Une [référence](/cli/azure/) détaillée est également disponible. Elle explique comment utiliser chacune des commandes Azure CLI 2.0.</span><span class="sxs-lookup"><span data-stu-id="fd055-117">A detailed [reference](/cli/azure/) is also available that documents how to use each individual Azure CLI 2.0 command.</span></span>

<span data-ttu-id="fd055-118">[Bien démarrer avec Azure CLI 2.0](get-started-with-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="fd055-118">[Get started](get-started-with-azure-cli.md) with Azure CLI 2.0 now.</span></span>


> [!NOTE]
> <span data-ttu-id="fd055-119">Si vous utilisez la version précédente de l’interface de ligne de commande (Azure CLI), vous pouvez continuer à l’utiliser.</span><span class="sxs-lookup"><span data-stu-id="fd055-119">If you use the previous version of the CLI (Azure CLI), you can continue to use it.</span></span>
> <span data-ttu-id="fd055-120">Si vous utilisez les deux interfaces de ligne de commande, n’oubliez pas que `azure` est l’ancienne interface CLI (Azure CLI) et que `az` est la nouvelle interface CLI (Azure CLI 2.0).</span><span class="sxs-lookup"><span data-stu-id="fd055-120">If you use both CLIs, remember that `azure` is the old CLI - Azure CLI, and that `az` is the new CLI - Azure CLI 2.0.</span></span> 