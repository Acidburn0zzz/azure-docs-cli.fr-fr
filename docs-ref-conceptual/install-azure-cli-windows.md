---
title: "Installer l’interface de ligne de commande Azure pour Windows"
description: "Installation d’Azure CLI 2.0 sur Windows"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 01/29/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: df1c2b33589c160525710845cc81d076082a9ecc
ms.sourcegitcommit: def1a07bfccf26a4178ba6dd836764a1df205929
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/09/2018
---
# <a name="install-azure-cli-20-on-windows"></a><span data-ttu-id="8f120-103">Installation d’Azure CLI 2.0 sur Windows</span><span class="sxs-lookup"><span data-stu-id="8f120-103">Install Azure CLI 2.0 on Windows</span></span>

<span data-ttu-id="8f120-104">Sur Windows, le fichier binaire Azure CLI est installé via un fichier MSI, qui vous donne accès à l’interface de ligne de commande via l’Invite de commandes Windows (CMD) ou PowerShell.</span><span class="sxs-lookup"><span data-stu-id="8f120-104">On Windows the Azure CLI binary is installed via an MSI, which gives you access to the CLI through the Windows Command Prompt (CMD) or PowerShell.</span></span>
<span data-ttu-id="8f120-105">Si vous exécutez le Sous-système Windows pour Linux, des packages sont disponibles pour votre distribution Linux.</span><span class="sxs-lookup"><span data-stu-id="8f120-105">If you are running Windows Subsystem for Linux (WSL), there are packages available for your Linux distribution.</span></span> <span data-ttu-id="8f120-106">Consultez la [page d’installation principale](install-azure-cli.md) pour obtenir la liste des gestionnaires de packages pris en charge ou pour savoir comment installer manuellement avec le sous-système Windows pour Linux.</span><span class="sxs-lookup"><span data-stu-id="8f120-106">See the [main install page](install-azure-cli.md) for the list of supported package managers or how to install manually under WSL.</span></span>

## <a name="install-or-update"></a><span data-ttu-id="8f120-107">Installation ou mise à jour</span><span class="sxs-lookup"><span data-stu-id="8f120-107">Install or update</span></span>

<span data-ttu-id="8f120-108">Le fichier MSI distribuable est utilisé pour l’installation, la mise à jour et la désinstallation de la commande `az` sous Windows.</span><span class="sxs-lookup"><span data-stu-id="8f120-108">The MSI distributable is used for installing, updating, and uninstalling the `az` command on Windows.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="8f120-109">Téléchargez le programme d’installation MSI</span><span class="sxs-lookup"><span data-stu-id="8f120-109">Download the MSI installer</span></span>](https://aka.ms/installazurecliwindows)

<span data-ttu-id="8f120-110">Lorsque le programme d’installation vous demande s’il peut apporter des modifications à votre ordinateur, cliquez sur la case « Oui ».</span><span class="sxs-lookup"><span data-stu-id="8f120-110">When the installer asks if it can make changes to your computer, click the "Yes" box.</span></span>

<span data-ttu-id="8f120-111">Vous pouvez désormais exécuter l’interface de ligne de commande Azure avec la commande `az` à partir de l’invite de commandes Windows ou PowerShell.</span><span class="sxs-lookup"><span data-stu-id="8f120-111">You can now run the Azure CLI with the `az` command from either Windows Command Prompt or PowerShell.</span></span> <span data-ttu-id="8f120-112">PowerShell offre des fonctionnalité de saisie semi-automatique via la touche TAB non disponibles à partir de CMD.</span><span class="sxs-lookup"><span data-stu-id="8f120-112">PowerShell offers some tab completion features not available from CMD.</span></span>

## <a name="uninstall"></a><span data-ttu-id="8f120-113">Désinstaller l’interface</span><span class="sxs-lookup"><span data-stu-id="8f120-113">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="8f120-114">La désinstallation peut être réalisée en exécutant le fichier MSI à nouveau, en choisissant l’option « Désinstaller ».</span><span class="sxs-lookup"><span data-stu-id="8f120-114">Uninstalling can be done by running the MSI again, and choosing the "Uninstall" option.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="8f120-115">Téléchargez le programme d’installation MSI</span><span class="sxs-lookup"><span data-stu-id="8f120-115">Download the MSI installer</span></span>](https://aka.ms/installazurecliwindows)
