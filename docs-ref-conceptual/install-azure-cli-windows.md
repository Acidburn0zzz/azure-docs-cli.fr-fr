---
title: Installer l’interface de ligne de commande Azure pour Windows
description: Installation d’Azure CLI 2.0 sur Windows
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 01/29/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: e614f0d108cef0702525e033d166e0498a94729f
ms.sourcegitcommit: fb3fed8701aff6c46af856e8fdc3e56ff9a678bc
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/11/2018
ms.locfileid: "38228973"
---
# <a name="install-azure-cli-20-on-windows"></a><span data-ttu-id="f1a7f-103">Installation d’Azure CLI 2.0 sur Windows</span><span class="sxs-lookup"><span data-stu-id="f1a7f-103">Install Azure CLI 2.0 on Windows</span></span>

<span data-ttu-id="f1a7f-104">Sur Windows, le fichier binaire Azure CLI est installé via un fichier MSI, qui vous donne accès à l’interface de ligne de commande via l’Invite de commandes Windows (CMD) ou PowerShell.</span><span class="sxs-lookup"><span data-stu-id="f1a7f-104">On Windows the Azure CLI binary is installed via an MSI, which gives you access to the CLI through the Windows Command Prompt (CMD) or PowerShell.</span></span>
<span data-ttu-id="f1a7f-105">Si vous exécutez le sous-système Windows pour Linux, des packages sont disponibles pour votre distribution Linux.</span><span class="sxs-lookup"><span data-stu-id="f1a7f-105">If you are running the Windows Subsystem for Linux (WSL), packages are available for your Linux distribution.</span></span> <span data-ttu-id="f1a7f-106">Consultez la [page d’installation principale](install-azure-cli.md) pour obtenir la liste des gestionnaires de packages pris en charge ou pour savoir comment installer manuellement avec le sous-système Windows pour Linux.</span><span class="sxs-lookup"><span data-stu-id="f1a7f-106">See the [main install page](install-azure-cli.md) for the list of supported package managers or how to install manually under WSL.</span></span>

## <a name="install-or-update"></a><span data-ttu-id="f1a7f-107">Installation ou mise à jour</span><span class="sxs-lookup"><span data-stu-id="f1a7f-107">Install or update</span></span>

<span data-ttu-id="f1a7f-108">Le fichier MSI distribuable est utilisé pour l’installation, la mise à jour et la désinstallation de la commande `az` sous Windows.</span><span class="sxs-lookup"><span data-stu-id="f1a7f-108">The MSI distributable is used for installing, updating, and uninstalling the `az` command on Windows.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="f1a7f-109">Téléchargez le programme d’installation MSI</span><span class="sxs-lookup"><span data-stu-id="f1a7f-109">Download the MSI installer</span></span>](https://aka.ms/installazurecliwindows)

<span data-ttu-id="f1a7f-110">Lorsque le programme d’installation vous demande s’il peut apporter des modifications à votre ordinateur, cliquez sur la case « Oui ».</span><span class="sxs-lookup"><span data-stu-id="f1a7f-110">When the installer asks if it can make changes to your computer, click the "Yes" box.</span></span>

<span data-ttu-id="f1a7f-111">Vous pouvez désormais exécuter l’interface de ligne de commande Azure avec la commande `az` à partir de l’invite de commandes Windows ou PowerShell.</span><span class="sxs-lookup"><span data-stu-id="f1a7f-111">You can now run the Azure CLI with the `az` command from either Windows Command Prompt or PowerShell.</span></span> <span data-ttu-id="f1a7f-112">PowerShell offre des fonctionnalités de saisie semi-automatique via la touche TAB non disponibles à partir de l’invite de commandes Windows.</span><span class="sxs-lookup"><span data-stu-id="f1a7f-112">PowerShell offers some tab completion features not available from Windows Command Prompt.</span></span> <span data-ttu-id="f1a7f-113">Pour vous connecter, exécutez la commande [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="f1a7f-113">To sign in, run the [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="f1a7f-114">Pour en savoir plus sur les différentes méthodes d’authentification, consultez [Se connecter avec Azure CLI 2.0](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="f1a7f-114">To learn more about different authentication methods, see [Sign in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

## <a name="uninstall"></a><span data-ttu-id="f1a7f-115">Désinstaller l’interface</span><span class="sxs-lookup"><span data-stu-id="f1a7f-115">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="f1a7f-116">La désinstallation peut être réalisée en exécutant le fichier MSI à nouveau, en choisissant l’option « Désinstaller ».</span><span class="sxs-lookup"><span data-stu-id="f1a7f-116">Uninstalling can be done by running the MSI again, and choosing the "Uninstall" option.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="f1a7f-117">Téléchargez le programme d’installation MSI</span><span class="sxs-lookup"><span data-stu-id="f1a7f-117">Download the MSI installer</span></span>](https://aka.ms/installazurecliwindows)
