---
title: Installer l’interface de ligne de commande Azure pour Windows
description: Installation d’Azure CLI 2.0 sur Windows
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 6e57837313faf0edd95d822132ae282ed416aae7
ms.sourcegitcommit: d93b0a2bcfb0d164ef90d6d4618f0552609a8ea6
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/20/2018
ms.locfileid: "46469961"
---
# <a name="install-azure-cli-20-on-windows"></a><span data-ttu-id="6974f-103">Installation d’Azure CLI 2.0 sur Windows</span><span class="sxs-lookup"><span data-stu-id="6974f-103">Install Azure CLI 2.0 on Windows</span></span>

<span data-ttu-id="6974f-104">Sur Windows, Azure CLI est installée via un fichier MSI, ce qui vous donne accès à l’interface CLI via l’Invite de commande Windows (CMD) ou PowerShell.</span><span class="sxs-lookup"><span data-stu-id="6974f-104">For Windows the Azure CLI is installed via an MSI, which gives you access to the CLI through the Windows Command Prompt (CMD) or PowerShell.</span></span>
<span data-ttu-id="6974f-105">Lors de son installation sur le sous-système Windows pour Linux (WSL), des packages sont disponibles pour votre distribution Linux.</span><span class="sxs-lookup"><span data-stu-id="6974f-105">When installing for Windows Subsystem for Linux (WSL), packages are available for your Linux distribution.</span></span> <span data-ttu-id="6974f-106">Consultez la [page d’installation principale](install-azure-cli.md) pour obtenir la liste des gestionnaires de packages pris en charge ou pour savoir comment installer manuellement avec le sous-système Windows pour Linux.</span><span class="sxs-lookup"><span data-stu-id="6974f-106">See the [main install page](install-azure-cli.md) for the list of supported package managers or how to install manually under WSL.</span></span>

## <a name="install-or-update"></a><span data-ttu-id="6974f-107">Installation ou mise à jour</span><span class="sxs-lookup"><span data-stu-id="6974f-107">Install or update</span></span>

<span data-ttu-id="6974f-108">Le fichier MSI distribuable est utilisé pour l’installation, la mise à jour et la désinstallation de la commande `az` sous Windows.</span><span class="sxs-lookup"><span data-stu-id="6974f-108">The MSI distributable is used for installing, updating, and uninstalling the `az` command on Windows.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="6974f-109">Téléchargez le programme d’installation MSI</span><span class="sxs-lookup"><span data-stu-id="6974f-109">Download the MSI installer</span></span>](https://aka.ms/installazurecliwindows)

<span data-ttu-id="6974f-110">Lorsque le programme d’installation vous demande s’il peut apporter des modifications à votre ordinateur, cliquez sur la case « Oui ».</span><span class="sxs-lookup"><span data-stu-id="6974f-110">When the installer asks if it can make changes to your computer, click the "Yes" box.</span></span>

<span data-ttu-id="6974f-111">Vous pouvez désormais exécuter l’interface de ligne de commande Azure avec la commande `az` à partir de l’invite de commandes Windows ou PowerShell.</span><span class="sxs-lookup"><span data-stu-id="6974f-111">You can now run the Azure CLI with the `az` command from either Windows Command Prompt or PowerShell.</span></span> <span data-ttu-id="6974f-112">PowerShell offre des fonctionnalités de saisie semi-automatique via la touche TAB non disponibles à partir de l’invite de commandes Windows.</span><span class="sxs-lookup"><span data-stu-id="6974f-112">PowerShell offers some tab completion features not available from Windows Command Prompt.</span></span> <span data-ttu-id="6974f-113">Pour vous connecter, exécutez la commande [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="6974f-113">To sign in, run the [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="6974f-114">Pour en savoir plus sur les différentes méthodes d’authentification, consultez [Se connecter avec Azure CLI 2.0](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="6974f-114">To learn more about different authentication methods, see [Sign in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

## <a name="uninstall"></a><span data-ttu-id="6974f-115">Désinstaller l’interface</span><span class="sxs-lookup"><span data-stu-id="6974f-115">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="6974f-116">La désinstallation peut être réalisée en exécutant le fichier MSI à nouveau, en choisissant l’option « Désinstaller ».</span><span class="sxs-lookup"><span data-stu-id="6974f-116">Uninstalling can be done by running the MSI again, and choosing the "Uninstall" option.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="6974f-117">Téléchargez le programme d’installation MSI</span><span class="sxs-lookup"><span data-stu-id="6974f-117">Download the MSI installer</span></span>](https://aka.ms/installazurecliwindows)

## <a name="next-steps"></a><span data-ttu-id="6974f-118">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="6974f-118">Next Steps</span></span>

<span data-ttu-id="6974f-119">Maintenant que vous avez installé l’interface CLI, découvrez ses fonctionnalités et ses commandes courantes.</span><span class="sxs-lookup"><span data-stu-id="6974f-119">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="6974f-120">Prise en main de l’interface Azure CLI</span><span class="sxs-lookup"><span data-stu-id="6974f-120">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
