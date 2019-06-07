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
ms.openlocfilehash: 40810b25bf776025c82b48ba7aa424369483ceeb
ms.sourcegitcommit: 08043c47d3ccf23522b91e6bba3932e312c04c7f
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/04/2019
ms.locfileid: "66516269"
---
# <a name="install-azure-cli-on-windows"></a><span data-ttu-id="0c55b-103">Installer Azure CLI sur Windows</span><span class="sxs-lookup"><span data-stu-id="0c55b-103">Install Azure CLI on Windows</span></span>

<span data-ttu-id="0c55b-104">Sur Windows, Azure CLI est installée via un fichier MSI, ce qui vous donne accès à l’interface CLI via l’Invite de commande Windows (CMD) ou PowerShell.</span><span class="sxs-lookup"><span data-stu-id="0c55b-104">For Windows the Azure CLI is installed via an MSI, which gives you access to the CLI through the Windows Command Prompt (CMD) or PowerShell.</span></span>
<span data-ttu-id="0c55b-105">Lors de son installation sur le sous-système Windows pour Linux (WSL), des packages sont disponibles pour votre distribution Linux.</span><span class="sxs-lookup"><span data-stu-id="0c55b-105">When installing for Windows Subsystem for Linux (WSL), packages are available for your Linux distribution.</span></span> <span data-ttu-id="0c55b-106">Consultez la [page d’installation principale](install-azure-cli.md) pour obtenir la liste des gestionnaires de packages pris en charge ou pour savoir comment installer manuellement avec le sous-système Windows pour Linux.</span><span class="sxs-lookup"><span data-stu-id="0c55b-106">See the [main install page](install-azure-cli.md) for the list of supported package managers or how to install manually under WSL.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

## <a name="install-or-update"></a><span data-ttu-id="0c55b-107">Installation ou mise à jour</span><span class="sxs-lookup"><span data-stu-id="0c55b-107">Install or update</span></span>

<span data-ttu-id="0c55b-108">Le fichier MSI distribuable est utilisé pour l’installation ou la mise à jour d’Azure CLI sur Windows.</span><span class="sxs-lookup"><span data-stu-id="0c55b-108">The MSI distributable is used for installing or updating the Azure CLI on Windows.</span></span> <span data-ttu-id="0c55b-109">L’utilisation du programme d’installation MSI ne nécessite pas la désinstallation des versions actuelles.</span><span class="sxs-lookup"><span data-stu-id="0c55b-109">You don't need to uninstall any current versions before using the MSI installer.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="0c55b-110">Téléchargez le programme d’installation MSI</span><span class="sxs-lookup"><span data-stu-id="0c55b-110">Download the MSI installer</span></span>](https://aka.ms/installazurecliwindows)

<span data-ttu-id="0c55b-111">Lorsque le programme d’installation vous demande s’il peut apporter des modifications à votre ordinateur, cliquez sur la case « Oui ».</span><span class="sxs-lookup"><span data-stu-id="0c55b-111">When the installer asks if it can make changes to your computer, click the "Yes" box.</span></span>

<span data-ttu-id="0c55b-112">Vous pouvez désormais exécuter l’interface de ligne de commande Azure avec la commande `az` à partir de l’invite de commandes Windows ou PowerShell.</span><span class="sxs-lookup"><span data-stu-id="0c55b-112">You can now run the Azure CLI with the `az` command from either Windows Command Prompt or PowerShell.</span></span> <span data-ttu-id="0c55b-113">PowerShell offre des fonctionnalités de saisie semi-automatique via la touche TAB non disponibles à partir de l’invite de commandes Windows.</span><span class="sxs-lookup"><span data-stu-id="0c55b-113">PowerShell offers some tab completion features not available from Windows Command Prompt.</span></span> <span data-ttu-id="0c55b-114">Pour vous connecter, exécutez la commande [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="0c55b-114">To sign in, run the [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="0c55b-115">Pour en savoir plus sur les différentes méthodes d’authentification, consultez [Se connecter avec Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="0c55b-115">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="0c55b-116">Résolution de problèmes</span><span class="sxs-lookup"><span data-stu-id="0c55b-116">Troubleshooting</span></span>

<span data-ttu-id="0c55b-117">Voici certains problèmes courants lors de l’installation sur Windows.</span><span class="sxs-lookup"><span data-stu-id="0c55b-117">Here are some common problems seen when installing on Windows.</span></span> <span data-ttu-id="0c55b-118">Si vous rencontrez un problème qui n’est pas traité ici, [signalez ce problème sur GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="0c55b-118">If you experience a problem not covered here, [file an issue on GitHub](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="proxy-blocks-connection"></a><span data-ttu-id="0c55b-119">Le proxy bloque la connexion</span><span class="sxs-lookup"><span data-stu-id="0c55b-119">Proxy blocks connection</span></span>

<span data-ttu-id="0c55b-120">Si vous ne pouvez pas télécharger le programme d’installation MSI car votre serveur proxy bloque la connexion, vérifiez que votre proxy est configuré correctement.</span><span class="sxs-lookup"><span data-stu-id="0c55b-120">If you can't download the MSI installer because your proxy is blocking the connection, make sure that you have your proxy properly configured.</span></span> <span data-ttu-id="0c55b-121">Pour Windows 10, ces paramètres sont gérés dans le volet `Settings > Network & Internet > Proxy`.</span><span class="sxs-lookup"><span data-stu-id="0c55b-121">For Windows 10, these settings are managed in the `Settings > Network & Internet > Proxy` pane.</span></span> <span data-ttu-id="0c55b-122">Contactez votre administrateur système pour connaître les paramètres requis, ou les situations où votre ordinateur peut être géré par configuration ou nécessiter une configuration avancée.</span><span class="sxs-lookup"><span data-stu-id="0c55b-122">Contact your system administrator for the required settings, or for situations where your machine may be configuration-managed or require advanced setup.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="0c55b-123">Ces paramètres sont également requis pour l’accès aux services Azure avec l’interface CLI, PowerShell ou l’invite de commandes.</span><span class="sxs-lookup"><span data-stu-id="0c55b-123">These settings are also required to be able to access Azure services with the CLI, from both PowerShell or the Command Prompt.</span></span> <span data-ttu-id="0c55b-124">Dans PowerShell, pour ce faire, utilisez la commande suivante :</span><span class="sxs-lookup"><span data-stu-id="0c55b-124">In PowerShell, you do this with the following command:</span></span>
>
> ```powershell
> (New-Object System.Net.WebClient).Proxy.Credentials = `
>   [System.Net.CredentialCache]::DefaultNetworkCredentials
> ```

<span data-ttu-id="0c55b-125">Pour obtenir le fichier MSI, votre proxy doit autoriser les connexions HTTPS aux adresses suivantes :</span><span class="sxs-lookup"><span data-stu-id="0c55b-125">In order to get the MSI, your proxy needs to allow HTTPS connections to the following addresses:</span></span>

* `https://aka.ms/`
* `https://azurecliprod.blob.core.windows.net/`

## <a name="uninstall"></a><span data-ttu-id="0c55b-126">Désinstaller l’interface</span><span class="sxs-lookup"><span data-stu-id="0c55b-126">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="0c55b-127">La désinstallation d’Azure CLI s’effectue à partir de la liste « Applications et fonctionnalités » dans Windows.</span><span class="sxs-lookup"><span data-stu-id="0c55b-127">You uninstall the Azure CLI from the Windows "Apps and Features" list.</span></span> <span data-ttu-id="0c55b-128">Pour désinstaller :</span><span class="sxs-lookup"><span data-stu-id="0c55b-128">To uninstall:</span></span>

| <span data-ttu-id="0c55b-129">Plateforme</span><span class="sxs-lookup"><span data-stu-id="0c55b-129">Platform</span></span> | <span data-ttu-id="0c55b-130">Instructions</span><span class="sxs-lookup"><span data-stu-id="0c55b-130">Instructions</span></span> |
|---|---|
| <span data-ttu-id="0c55b-131">Windows 10</span><span class="sxs-lookup"><span data-stu-id="0c55b-131">Windows 10</span></span> | <span data-ttu-id="0c55b-132">Démarrer > Paramètres > Applications</span><span class="sxs-lookup"><span data-stu-id="0c55b-132">Start > Settings > Apps</span></span> |
| <span data-ttu-id="0c55b-133">Windows 8</span><span class="sxs-lookup"><span data-stu-id="0c55b-133">Windows 8</span></span><br/><span data-ttu-id="0c55b-134">Windows 7</span><span class="sxs-lookup"><span data-stu-id="0c55b-134">Windows 7</span></span> | <span data-ttu-id="0c55b-135">Démarrer > Panneau de configuration > Programmes > Désinstaller un programme</span><span class="sxs-lookup"><span data-stu-id="0c55b-135">Start > Control Panel > Programs > Uninstall a program</span></span> |

<span data-ttu-id="0c55b-136">Une fois sur cet écran, tapez __Azure CLI__ dans la barre de recherche du programme.</span><span class="sxs-lookup"><span data-stu-id="0c55b-136">Once on this screen type __Azure CLI__ into the program search bar.</span></span> <span data-ttu-id="0c55b-137">Le programme à désinstaller est listé sous le nom __Microsoft CLI 2.0 pour Azure__.</span><span class="sxs-lookup"><span data-stu-id="0c55b-137">The program to uninstall is listed as __Microsoft CLI 2.0 for Azure__.</span></span> <span data-ttu-id="0c55b-138">Sélectionnez cette application, puis cliquez sur le bouton `Uninstall`.</span><span class="sxs-lookup"><span data-stu-id="0c55b-138">Select this application, then click the `Uninstall` button.</span></span>

## <a name="next-steps"></a><span data-ttu-id="0c55b-139">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="0c55b-139">Next Steps</span></span>

<span data-ttu-id="0c55b-140">Maintenant que vous avez installé l’interface CLI, découvrez ses fonctionnalités et ses commandes courantes.</span><span class="sxs-lookup"><span data-stu-id="0c55b-140">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="0c55b-141">Prise en main de l’interface Azure CLI</span><span class="sxs-lookup"><span data-stu-id="0c55b-141">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
