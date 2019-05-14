---
title: Installer l’interface de ligne de commande Azure pour Windows
description: Comment installer Azure CLI sur Windows
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/01/2019
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: c5c499800e49dcdc536337e7655ec1ee280d48f2
ms.sourcegitcommit: 65bf8561a6e047e4eab52186e066a2e8c21f1d40
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/07/2019
ms.locfileid: "65240541"
---
# <a name="install-azure-cli-on-windows"></a><span data-ttu-id="58643-103">Installer Azure CLI sur Windows</span><span class="sxs-lookup"><span data-stu-id="58643-103">Install Azure CLI on Windows</span></span>

<span data-ttu-id="58643-104">Sur Windows, Azure CLI est installée via un fichier MSI, ce qui vous donne accès à l’interface CLI via l’Invite de commande Windows (CMD) ou PowerShell.</span><span class="sxs-lookup"><span data-stu-id="58643-104">For Windows the Azure CLI is installed via an MSI, which gives you access to the CLI through the Windows Command Prompt (CMD) or PowerShell.</span></span>
<span data-ttu-id="58643-105">Lors de son installation sur le sous-système Windows pour Linux (WSL), des packages sont disponibles pour votre distribution Linux.</span><span class="sxs-lookup"><span data-stu-id="58643-105">When installing for Windows Subsystem for Linux (WSL), packages are available for your Linux distribution.</span></span> <span data-ttu-id="58643-106">Consultez la [page d’installation principale](install-azure-cli.md) pour obtenir la liste des gestionnaires de packages pris en charge ou pour savoir comment installer manuellement avec le sous-système Windows pour Linux.</span><span class="sxs-lookup"><span data-stu-id="58643-106">See the [main install page](install-azure-cli.md) for the list of supported package managers or how to install manually under WSL.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

## <a name="install-or-update"></a><span data-ttu-id="58643-107">Installation ou mise à jour</span><span class="sxs-lookup"><span data-stu-id="58643-107">Install or update</span></span>

<span data-ttu-id="58643-108">Le fichier MSI distribuable est utilisé pour l’installation ou la mise à jour d’Azure CLI sur Windows.</span><span class="sxs-lookup"><span data-stu-id="58643-108">The MSI distributable is used for installing or updating the Azure CLI on Windows.</span></span> <span data-ttu-id="58643-109">L’utilisation du programme d’installation MSI ne nécessite pas la désinstallation des versions actuelles.</span><span class="sxs-lookup"><span data-stu-id="58643-109">You don't need to uninstall any current versions before using the MSI installer.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="58643-110">Téléchargez le programme d’installation MSI</span><span class="sxs-lookup"><span data-stu-id="58643-110">Download the MSI installer</span></span>](https://aka.ms/installazurecliwindows)

<span data-ttu-id="58643-111">Lorsque le programme d’installation vous demande s’il peut apporter des modifications à votre ordinateur, cliquez sur la case « Oui ».</span><span class="sxs-lookup"><span data-stu-id="58643-111">When the installer asks if it can make changes to your computer, click the "Yes" box.</span></span>

<span data-ttu-id="58643-112">Vous pouvez désormais exécuter l’interface de ligne de commande Azure avec la commande `az` à partir de l’invite de commandes Windows ou PowerShell.</span><span class="sxs-lookup"><span data-stu-id="58643-112">You can now run the Azure CLI with the `az` command from either Windows Command Prompt or PowerShell.</span></span> <span data-ttu-id="58643-113">PowerShell offre des fonctionnalités de saisie semi-automatique via la touche TAB non disponibles à partir de l’invite de commandes Windows.</span><span class="sxs-lookup"><span data-stu-id="58643-113">PowerShell offers some tab completion features not available from Windows Command Prompt.</span></span> <span data-ttu-id="58643-114">Pour vous connecter, exécutez la commande [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="58643-114">To sign in, run the [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="58643-115">Pour en savoir plus sur les différentes méthodes d’authentification, consultez [Se connecter avec Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="58643-115">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="uninstall"></a><span data-ttu-id="58643-116">Désinstaller l’interface</span><span class="sxs-lookup"><span data-stu-id="58643-116">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="58643-117">La désinstallation d’Azure CLI s’effectue à partir de la liste « Applications et fonctionnalités » dans Windows.</span><span class="sxs-lookup"><span data-stu-id="58643-117">You uninstall the Azure CLI from the Windows "Apps and Features" list.</span></span> <span data-ttu-id="58643-118">Pour désinstaller :</span><span class="sxs-lookup"><span data-stu-id="58643-118">To uninstall:</span></span>

| <span data-ttu-id="58643-119">Plateforme</span><span class="sxs-lookup"><span data-stu-id="58643-119">Platform</span></span> | <span data-ttu-id="58643-120">Instructions</span><span class="sxs-lookup"><span data-stu-id="58643-120">Instructions</span></span> |
|---|---|
| <span data-ttu-id="58643-121">Windows 10</span><span class="sxs-lookup"><span data-stu-id="58643-121">Windows 10</span></span> | <span data-ttu-id="58643-122">Démarrer > Paramètres > Applications</span><span class="sxs-lookup"><span data-stu-id="58643-122">Start > Settings > Apps</span></span> |
| <span data-ttu-id="58643-123">Windows 8</span><span class="sxs-lookup"><span data-stu-id="58643-123">Windows 8</span></span><br/><span data-ttu-id="58643-124">Windows 7</span><span class="sxs-lookup"><span data-stu-id="58643-124">Windows 7</span></span> | <span data-ttu-id="58643-125">Démarrer > Panneau de configuration > Programmes > Désinstaller un programme</span><span class="sxs-lookup"><span data-stu-id="58643-125">Start > Control Panel > Programs > Uninstall a program</span></span> |

<span data-ttu-id="58643-126">Une fois sur cet écran, tapez __Azure CLI__ dans la barre de recherche du programme.</span><span class="sxs-lookup"><span data-stu-id="58643-126">Once on this screen type __Azure CLI__ into the program search bar.</span></span> <span data-ttu-id="58643-127">Le programme à désinstaller est listé sous le nom __Microsoft CLI 2.0 pour Azure__.</span><span class="sxs-lookup"><span data-stu-id="58643-127">The program to uninstall is listed as __Microsoft CLI 2.0 for Azure__.</span></span> <span data-ttu-id="58643-128">Sélectionnez cette application, puis cliquez sur le bouton `Uninstall`.</span><span class="sxs-lookup"><span data-stu-id="58643-128">Select this application, then click the `Uninstall` button.</span></span>

## <a name="next-steps"></a><span data-ttu-id="58643-129">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="58643-129">Next Steps</span></span>

<span data-ttu-id="58643-130">Maintenant que vous avez installé l’interface CLI, découvrez ses fonctionnalités et ses commandes courantes.</span><span class="sxs-lookup"><span data-stu-id="58643-130">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="58643-131">Prise en main de l’interface Azure CLI</span><span class="sxs-lookup"><span data-stu-id="58643-131">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
