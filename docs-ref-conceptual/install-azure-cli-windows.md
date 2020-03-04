---
title: Installer l’interface de ligne de commande Azure pour Windows
description: Comment installer Azure CLI sur Windows
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 05/01/2019
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: f88e9d6650354ace9d9e03a33a6bbb2642069bbd
ms.sourcegitcommit: 7caa6673f65e61deb8d6def6386e4eb9acdac923
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/28/2020
ms.locfileid: "77779565"
---
# <a name="install-azure-cli-on-windows"></a><span data-ttu-id="a9e1f-103">Installer Azure CLI sur Windows</span><span class="sxs-lookup"><span data-stu-id="a9e1f-103">Install Azure CLI on Windows</span></span>

<span data-ttu-id="a9e1f-104">Sur Windows, Azure CLI est installée via un fichier MSI, ce qui vous donne accès à l’interface CLI via l’Invite de commande Windows (CMD) ou PowerShell.</span><span class="sxs-lookup"><span data-stu-id="a9e1f-104">For Windows the Azure CLI is installed via an MSI, which gives you access to the CLI through the Windows Command Prompt (CMD) or PowerShell.</span></span>
<span data-ttu-id="a9e1f-105">Lors de son installation sur le sous-système Windows pour Linux (WSL), des packages sont disponibles pour votre distribution Linux.</span><span class="sxs-lookup"><span data-stu-id="a9e1f-105">When installing for Windows Subsystem for Linux (WSL), packages are available for your Linux distribution.</span></span> <span data-ttu-id="a9e1f-106">Consultez la [page d’installation principale](install-azure-cli.md) pour obtenir la liste des gestionnaires de packages pris en charge ou pour savoir comment installer manuellement avec le sous-système Windows pour Linux.</span><span class="sxs-lookup"><span data-stu-id="a9e1f-106">See the [main install page](install-azure-cli.md) for the list of supported package managers or how to install manually under WSL.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

## <a name="install-or-update"></a><span data-ttu-id="a9e1f-107">Installation ou mise à jour</span><span class="sxs-lookup"><span data-stu-id="a9e1f-107">Install or update</span></span>

<span data-ttu-id="a9e1f-108">Le fichier MSI distribuable est utilisé pour l’installation ou la mise à jour d’Azure CLI sur Windows.</span><span class="sxs-lookup"><span data-stu-id="a9e1f-108">The MSI distributable is used for installing or updating the Azure CLI on Windows.</span></span> <span data-ttu-id="a9e1f-109">L’utilisation du programme d’installation MSI ne nécessite pas la désinstallation des versions actuelles.</span><span class="sxs-lookup"><span data-stu-id="a9e1f-109">You don't need to uninstall any current versions before using the MSI installer.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="a9e1f-110">Téléchargez le programme d’installation MSI</span><span class="sxs-lookup"><span data-stu-id="a9e1f-110">Download the MSI installer</span></span>](https://aka.ms/installazurecliwindows)

<span data-ttu-id="a9e1f-111">Lorsque le programme d’installation vous demande s’il peut apporter des modifications à votre ordinateur, cliquez sur la case « Oui ».</span><span class="sxs-lookup"><span data-stu-id="a9e1f-111">When the installer asks if it can make changes to your computer, click the "Yes" box.</span></span>

<span data-ttu-id="a9e1f-112">Vous pouvez également installer Azure CLI en utilisant PowerShell.</span><span class="sxs-lookup"><span data-stu-id="a9e1f-112">You can also install the Azure CLI using PowerShell.</span></span> <span data-ttu-id="a9e1f-113">Démarrez PowerShell en tant qu’administrateur et exécutez la commande suivante :</span><span class="sxs-lookup"><span data-stu-id="a9e1f-113">Start PowerShell as administrator and run the following command:</span></span>

   ```PowerShell
   Invoke-WebRequest -Uri https://aka.ms/installazurecliwindows -OutFile .\AzureCLI.msi; Start-Process msiexec.exe -Wait -ArgumentList '/I AzureCLI.msi /quiet'
   ```
<span data-ttu-id="a9e1f-114">Cette opération télécharge et installe la dernière version d’Azure CLI pour Windows.</span><span class="sxs-lookup"><span data-stu-id="a9e1f-114">This will download and install the latest version of the Azure CLI for Windows.</span></span> <span data-ttu-id="a9e1f-115">Si vous aviez déjà installé une version, celle-ci est mise à jour.</span><span class="sxs-lookup"><span data-stu-id="a9e1f-115">If you already have a version installed, it will update the existing version.</span></span> <span data-ttu-id="a9e1f-116">Une fois l’installation terminée, vous devez rouvrir PowerShell pour utiliser Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="a9e1f-116">After the installation is complete, you will need to reopen PowerShell to use the Azure CLI.</span></span>

<span data-ttu-id="a9e1f-117">Vous pouvez désormais exécuter l’interface de ligne de commande Azure avec la commande `az` à partir de l’invite de commandes Windows ou PowerShell.</span><span class="sxs-lookup"><span data-stu-id="a9e1f-117">You can now run the Azure CLI with the `az` command from either Windows Command Prompt or PowerShell.</span></span> <span data-ttu-id="a9e1f-118">PowerShell offre des fonctionnalités de saisie semi-automatique via la touche TAB non disponibles à partir de l’invite de commandes Windows.</span><span class="sxs-lookup"><span data-stu-id="a9e1f-118">PowerShell offers some tab completion features not available from Windows Command Prompt.</span></span> <span data-ttu-id="a9e1f-119">Pour vous connecter, exécutez la commande [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="a9e1f-119">To sign in, run the [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="a9e1f-120">Pour en savoir plus sur les différentes méthodes d’authentification, consultez [Se connecter avec Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="a9e1f-120">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="a9e1f-121">Dépannage</span><span class="sxs-lookup"><span data-stu-id="a9e1f-121">Troubleshooting</span></span>

<span data-ttu-id="a9e1f-122">Voici certains problèmes courants lors de l’installation sur Windows.</span><span class="sxs-lookup"><span data-stu-id="a9e1f-122">Here are some common problems seen when installing on Windows.</span></span> <span data-ttu-id="a9e1f-123">Si vous rencontrez un problème qui n’est pas traité ici, [signalez ce problème sur GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="a9e1f-123">If you experience a problem not covered here, [file an issue on GitHub](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="proxy-blocks-connection"></a><span data-ttu-id="a9e1f-124">Le proxy bloque la connexion</span><span class="sxs-lookup"><span data-stu-id="a9e1f-124">Proxy blocks connection</span></span>

<span data-ttu-id="a9e1f-125">Si vous ne pouvez pas télécharger le programme d’installation MSI car votre serveur proxy bloque la connexion, vérifiez que votre proxy est configuré correctement.</span><span class="sxs-lookup"><span data-stu-id="a9e1f-125">If you can't download the MSI installer because your proxy is blocking the connection, make sure that you have your proxy properly configured.</span></span> <span data-ttu-id="a9e1f-126">Pour Windows 10, ces paramètres sont gérés dans le volet `Settings > Network & Internet > Proxy`.</span><span class="sxs-lookup"><span data-stu-id="a9e1f-126">For Windows 10, these settings are managed in the `Settings > Network & Internet > Proxy` pane.</span></span> <span data-ttu-id="a9e1f-127">Contactez votre administrateur système pour connaître les paramètres requis, ou les situations où votre ordinateur peut être géré par configuration ou nécessiter une configuration avancée.</span><span class="sxs-lookup"><span data-stu-id="a9e1f-127">Contact your system administrator for the required settings, or for situations where your machine may be configuration-managed or require advanced setup.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="a9e1f-128">Ces paramètres sont également requis pour l’accès aux services Azure avec l’interface CLI, PowerShell ou l’invite de commandes.</span><span class="sxs-lookup"><span data-stu-id="a9e1f-128">These settings are also required to be able to access Azure services with the CLI, from both PowerShell or the Command Prompt.</span></span> <span data-ttu-id="a9e1f-129">Dans PowerShell, pour ce faire, utilisez la commande suivante :</span><span class="sxs-lookup"><span data-stu-id="a9e1f-129">In PowerShell, you do this with the following command:</span></span>
>
> ```powershell
> (New-Object System.Net.WebClient).Proxy.Credentials = `
>   [System.Net.CredentialCache]::DefaultNetworkCredentials
> ```

<span data-ttu-id="a9e1f-130">Pour obtenir le fichier MSI, votre proxy doit autoriser les connexions HTTPS aux adresses suivantes :</span><span class="sxs-lookup"><span data-stu-id="a9e1f-130">In order to get the MSI, your proxy needs to allow HTTPS connections to the following addresses:</span></span>

* `https://aka.ms/`
* `https://azurecliprod.blob.core.windows.net/`

## <a name="uninstall"></a><span data-ttu-id="a9e1f-131">Désinstaller l’interface</span><span class="sxs-lookup"><span data-stu-id="a9e1f-131">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="a9e1f-132">La désinstallation d’Azure CLI s’effectue à partir de la liste « Applications et fonctionnalités » dans Windows.</span><span class="sxs-lookup"><span data-stu-id="a9e1f-132">You uninstall the Azure CLI from the Windows "Apps and Features" list.</span></span> <span data-ttu-id="a9e1f-133">Pour désinstaller :</span><span class="sxs-lookup"><span data-stu-id="a9e1f-133">To uninstall:</span></span>

| <span data-ttu-id="a9e1f-134">Plateforme</span><span class="sxs-lookup"><span data-stu-id="a9e1f-134">Platform</span></span> | <span data-ttu-id="a9e1f-135">Instructions</span><span class="sxs-lookup"><span data-stu-id="a9e1f-135">Instructions</span></span> |
|---|---|
| <span data-ttu-id="a9e1f-136">Windows 10</span><span class="sxs-lookup"><span data-stu-id="a9e1f-136">Windows 10</span></span> | <span data-ttu-id="a9e1f-137">Démarrer > Paramètres > Applications</span><span class="sxs-lookup"><span data-stu-id="a9e1f-137">Start > Settings > Apps</span></span> |
| <span data-ttu-id="a9e1f-138">Windows 8</span><span class="sxs-lookup"><span data-stu-id="a9e1f-138">Windows 8</span></span><br/><span data-ttu-id="a9e1f-139">Windows 7</span><span class="sxs-lookup"><span data-stu-id="a9e1f-139">Windows 7</span></span> | <span data-ttu-id="a9e1f-140">Démarrer > Panneau de configuration > Programmes > Désinstaller un programme</span><span class="sxs-lookup"><span data-stu-id="a9e1f-140">Start > Control Panel > Programs > Uninstall a program</span></span> |

<span data-ttu-id="a9e1f-141">Une fois sur cet écran, tapez __Azure CLI__ dans la barre de recherche du programme.</span><span class="sxs-lookup"><span data-stu-id="a9e1f-141">Once on this screen type __Azure CLI__ into the program search bar.</span></span> <span data-ttu-id="a9e1f-142">Le programme à désinstaller est listé sous le nom __Microsoft CLI 2.0 pour Azure__.</span><span class="sxs-lookup"><span data-stu-id="a9e1f-142">The program to uninstall is listed as __Microsoft CLI 2.0 for Azure__.</span></span> <span data-ttu-id="a9e1f-143">Sélectionnez cette application, puis cliquez sur le bouton `Uninstall`.</span><span class="sxs-lookup"><span data-stu-id="a9e1f-143">Select this application, then click the `Uninstall` button.</span></span>

## <a name="next-steps"></a><span data-ttu-id="a9e1f-144">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="a9e1f-144">Next Steps</span></span>

<span data-ttu-id="a9e1f-145">Maintenant que vous avez installé l’interface CLI, découvrez ses fonctionnalités et ses commandes courantes.</span><span class="sxs-lookup"><span data-stu-id="a9e1f-145">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="a9e1f-146">Prise en main de l’interface Azure CLI</span><span class="sxs-lookup"><span data-stu-id="a9e1f-146">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
