---
title: Installer l’interface de ligne de commande Azure pour Windows
description: Comment installer Azure CLI sur Windows
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.prod: azure
ms.date: 09/25/2020
ms.topic: conceptual
ms.devlang: azurecli
ms.technology: azure-cli
ms.custom: devx-track-azurecli
ms.openlocfilehash: e592f4e0787a8e4391e47dc45d1841ff415f24bb
ms.sourcegitcommit: 8bff8b2ce4492ab99ad39390e4c802fb4f4425c8
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/26/2021
ms.locfileid: "105581850"
---
# <a name="install-azure-cli-on-windows"></a><span data-ttu-id="e0372-103">Installer Azure CLI sur Windows</span><span class="sxs-lookup"><span data-stu-id="e0372-103">Install Azure CLI on Windows</span></span>

<span data-ttu-id="e0372-104">Pour Windows, Azure CLI est installée à l’aide d’un fichier MSI, ce qui vous donne accès à l’interface CLI via l’Invite de commande Windows (CMD) ou PowerShell.</span><span class="sxs-lookup"><span data-stu-id="e0372-104">For Windows, the Azure CLI is installed via a MSI, which gives you access to the CLI through the Windows Command Prompt (CMD) or PowerShell.</span></span>
<span data-ttu-id="e0372-105">Lors de son installation sur le sous-système Windows pour Linux (WSL), des packages sont disponibles pour votre distribution Linux.</span><span class="sxs-lookup"><span data-stu-id="e0372-105">When installing for Windows Subsystem for Linux (WSL), packages are available for your Linux distribution.</span></span> <span data-ttu-id="e0372-106">Consultez la [page d’installation principale](install-azure-cli.md) pour obtenir la liste des gestionnaires de packages pris en charge ou pour savoir comment installer manuellement avec le sous-système Windows pour Linux.</span><span class="sxs-lookup"><span data-stu-id="e0372-106">See the [main install page](install-azure-cli.md) for the list of supported package managers or how to install manually under WSL.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

## <a name="install-or-update"></a><span data-ttu-id="e0372-107">Installation ou mise à jour</span><span class="sxs-lookup"><span data-stu-id="e0372-107">Install or update</span></span>

<span data-ttu-id="e0372-108">Le fichier MSI distribuable est utilisé pour l’installation ou la mise à jour d’Azure CLI sur Windows.</span><span class="sxs-lookup"><span data-stu-id="e0372-108">The MSI distributable is used for installing or updating the Azure CLI on Windows.</span></span> <span data-ttu-id="e0372-109">Vous n’avez pas besoin de désinstaller les versions actuelles avant d’utiliser le programme d’installation MSI, car celui-ci met à jour toute version existante.</span><span class="sxs-lookup"><span data-stu-id="e0372-109">You don't need to uninstall current versions before using the MSI installer because the MSI will update any existing version.</span></span>

# <a name="microsoft-installer-msi"></a>[<span data-ttu-id="e0372-110">Microsoft Installer (MSI)</span><span class="sxs-lookup"><span data-stu-id="e0372-110">Microsoft Installer (MSI)</span></span>](#tab/azure-cli)

<span data-ttu-id="e0372-111">Lorsque le programme d’installation vous demande s’il peut apporter des modifications à votre ordinateur, cliquez sur la case « Oui ».</span><span class="sxs-lookup"><span data-stu-id="e0372-111">When the installer asks if it can make changes to your computer, click the "Yes" box.</span></span>

### <a name="azure-cli-current-version"></a><span data-ttu-id="e0372-112">Version actuelle d’Azure CLI</span><span class="sxs-lookup"><span data-stu-id="e0372-112">Azure CLI current version</span></span>

<span data-ttu-id="e0372-113">Téléchargez et installez la version actuelle d’Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="e0372-113">Download and install the current release of the Azure CLI.</span></span>  <span data-ttu-id="e0372-114">Une fois l’installation terminée, vous devez fermer et rouvrir toutes les invites de commandes Windows ou fenêtres PowerShell actives pour pouvoir utiliser Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="e0372-114">After the installation is complete, you will need to close and reopen any active Windows Command Prompt or PowerShell windows to use the Azure CLI.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="e0372-115">Version actuelle d’Azure CLI</span><span class="sxs-lookup"><span data-stu-id="e0372-115">Current release of the Azure CLI</span></span>](https://aka.ms/installazurecliwindows)

### <a name="azure-cli-beta-version"></a><span data-ttu-id="e0372-116">Version bêta d’Azure CLI</span><span class="sxs-lookup"><span data-stu-id="e0372-116">Azure CLI beta version</span></span>

<span data-ttu-id="e0372-117">La version bêta d’Azure CLI prend en charge toutes les commandes et reste synchronisée avec la version publiée actuelle.</span><span class="sxs-lookup"><span data-stu-id="e0372-117">The beta version of the Azure CLI supports all commands and will stay in sync with the current released version.</span></span>  <span data-ttu-id="e0372-118">Pour obtenir des instructions d’installation, consultez [Installer la version bêta d’Azure CLI](install-azure-cli-beta.md).</span><span class="sxs-lookup"><span data-stu-id="e0372-118">For installation instructions, see [Install Azure CLI beta version](install-azure-cli-beta.md).</span></span> 

# <a name="microsoft-installer-msi-with-command"></a>[<span data-ttu-id="e0372-119">Microsoft Installer (MSI) avec commande</span><span class="sxs-lookup"><span data-stu-id="e0372-119">Microsoft Installer (MSI) with Command</span></span>](#tab/azure-powershell)

### <a name="powershell-command"></a><span data-ttu-id="e0372-120">Commande PowerShell</span><span class="sxs-lookup"><span data-stu-id="e0372-120">Powershell Command</span></span>

<span data-ttu-id="e0372-121">Vous pouvez également installer Azure CLI en utilisant PowerShell.</span><span class="sxs-lookup"><span data-stu-id="e0372-121">You can also install the Azure CLI using PowerShell.</span></span> <span data-ttu-id="e0372-122">Démarrez PowerShell en tant qu’administrateur et exécutez la commande suivante :</span><span class="sxs-lookup"><span data-stu-id="e0372-122">Start PowerShell as administrator and run the following command:</span></span>

   ```PowerShell
   Invoke-WebRequest -Uri https://aka.ms/installazurecliwindows -OutFile .\AzureCLI.msi; Start-Process msiexec.exe -Wait -ArgumentList '/I AzureCLI.msi /quiet'; rm .\AzureCLI.msi
   ```

<span data-ttu-id="e0372-123">Cette opération télécharge et installe la dernière version d’Azure CLI pour Windows.</span><span class="sxs-lookup"><span data-stu-id="e0372-123">This will download and install the latest version of the Azure CLI for Windows.</span></span> <span data-ttu-id="e0372-124">Si une version est déjà installée, le programme d’installation met à jour la version existante.</span><span class="sxs-lookup"><span data-stu-id="e0372-124">If you already have a version installed, the installer will update the existing version.</span></span> <span data-ttu-id="e0372-125">Une fois l’installation terminée, vous devez rouvrir PowerShell pour utiliser Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="e0372-125">After the installation is complete, you will need to reopen PowerShell to use the Azure CLI.</span></span>

### <a name="azure-cli-command-for-update-only"></a><span data-ttu-id="e0372-126">Commande Azure CLI (pour mise à jour uniquement)</span><span class="sxs-lookup"><span data-stu-id="e0372-126">Azure CLI Command (for update only)</span></span>
[!INCLUDE [az upgrade](includes/az-upgrade.md)]

---

## <a name="run-the-azure-cli"></a><span data-ttu-id="e0372-127">Exécuter Azure CLI</span><span class="sxs-lookup"><span data-stu-id="e0372-127">Run the Azure CLI</span></span>

<span data-ttu-id="e0372-128">Vous pouvez désormais exécuter l’interface de ligne de commande Azure avec la commande `az` à partir de l’invite de commandes Windows ou PowerShell.</span><span class="sxs-lookup"><span data-stu-id="e0372-128">You can now run the Azure CLI with the `az` command from either Windows Command Prompt or PowerShell.</span></span> <span data-ttu-id="e0372-129">PowerShell offre des fonctionnalités de saisie semi-automatique via la touche TAB non disponibles à partir de l’invite de commandes Windows.</span><span class="sxs-lookup"><span data-stu-id="e0372-129">PowerShell offers some tab completion features not available from Windows Command Prompt.</span></span> <span data-ttu-id="e0372-130">Pour vous connecter, exécutez la commande [az login](/cli/azure/reference-index#az_login).</span><span class="sxs-lookup"><span data-stu-id="e0372-130">To sign in, run the [az login](/cli/azure/reference-index#az_login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="e0372-131">Pour en savoir plus sur les différentes méthodes d’authentification, consultez [Se connecter avec Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="e0372-131">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="e0372-132">Dépannage</span><span class="sxs-lookup"><span data-stu-id="e0372-132">Troubleshooting</span></span>

<span data-ttu-id="e0372-133">Voici certains problèmes courants lors de l’installation sur Windows.</span><span class="sxs-lookup"><span data-stu-id="e0372-133">Here are some common problems seen when installing on Windows.</span></span> <span data-ttu-id="e0372-134">Si vous rencontrez un problème qui n’est pas traité ici, [signalez ce problème sur GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="e0372-134">If you experience a problem not covered here, [file an issue on GitHub](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="proxy-blocks-connection"></a><span data-ttu-id="e0372-135">Le proxy bloque la connexion</span><span class="sxs-lookup"><span data-stu-id="e0372-135">Proxy blocks connection</span></span>

<span data-ttu-id="e0372-136">Si vous ne pouvez pas télécharger le programme d’installation MSI car votre serveur proxy bloque la connexion, vérifiez que votre proxy est configuré correctement.</span><span class="sxs-lookup"><span data-stu-id="e0372-136">If you can't download the MSI installer because your proxy is blocking the connection, make sure that you have your proxy properly configured.</span></span> <span data-ttu-id="e0372-137">Pour Windows 10, ces paramètres sont gérés dans le volet `Settings > Network & Internet > Proxy`.</span><span class="sxs-lookup"><span data-stu-id="e0372-137">For Windows 10, these settings are managed in the `Settings > Network & Internet > Proxy` pane.</span></span> <span data-ttu-id="e0372-138">Contactez votre administrateur système pour connaître les paramètres requis, ou les situations où votre ordinateur peut être géré par configuration ou nécessiter une configuration avancée.</span><span class="sxs-lookup"><span data-stu-id="e0372-138">Contact your system administrator for the required settings, or for situations where your machine may be configuration-managed or require advanced setup.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="e0372-139">Ces paramètres sont également requis pour l’accès aux services Azure avec l’interface CLI, PowerShell ou l’invite de commandes.</span><span class="sxs-lookup"><span data-stu-id="e0372-139">These settings are also required to be able to access Azure services with the CLI, from both PowerShell or the Command Prompt.</span></span> <span data-ttu-id="e0372-140">Dans PowerShell, pour ce faire, utilisez la commande suivante :</span><span class="sxs-lookup"><span data-stu-id="e0372-140">In PowerShell, you do this with the following command:</span></span>
>
> ```powershell
> (New-Object System.Net.WebClient).Proxy.Credentials = `
>   [System.Net.CredentialCache]::DefaultNetworkCredentials
> ```

<span data-ttu-id="e0372-141">Pour obtenir le fichier MSI, votre proxy doit autoriser les connexions HTTPS aux adresses suivantes :</span><span class="sxs-lookup"><span data-stu-id="e0372-141">In order to get the MSI, your proxy needs to allow HTTPS connections to the following addresses:</span></span>

* `https://aka.ms/`
* `https://azcliprod.blob.core.windows.net/`

## <a name="uninstall"></a><span data-ttu-id="e0372-142">Désinstaller l’interface</span><span class="sxs-lookup"><span data-stu-id="e0372-142">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="e0372-143">La désinstallation d’Azure CLI s’effectue à partir de la liste « Applications et fonctionnalités » dans Windows.</span><span class="sxs-lookup"><span data-stu-id="e0372-143">You uninstall the Azure CLI from the Windows "Apps and Features" list.</span></span> <span data-ttu-id="e0372-144">Pour désinstaller :</span><span class="sxs-lookup"><span data-stu-id="e0372-144">To uninstall:</span></span>

| <span data-ttu-id="e0372-145">Plateforme</span><span class="sxs-lookup"><span data-stu-id="e0372-145">Platform</span></span> | <span data-ttu-id="e0372-146">Instructions</span><span class="sxs-lookup"><span data-stu-id="e0372-146">Instructions</span></span> |
|---|---|
| <span data-ttu-id="e0372-147">Windows 10</span><span class="sxs-lookup"><span data-stu-id="e0372-147">Windows 10</span></span> | <span data-ttu-id="e0372-148">Démarrer > Paramètres > Applications</span><span class="sxs-lookup"><span data-stu-id="e0372-148">Start > Settings > Apps</span></span> |
| <span data-ttu-id="e0372-149">Windows 8 et Windows 7</span><span class="sxs-lookup"><span data-stu-id="e0372-149">Windows 8 and Windows 7</span></span> | <span data-ttu-id="e0372-150">Démarrer > Panneau de configuration > Programmes > Désinstaller un programme</span><span class="sxs-lookup"><span data-stu-id="e0372-150">Start > Control Panel > Programs > Uninstall a program</span></span> |

<span data-ttu-id="e0372-151">Une fois sur cet écran, tapez __Azure CLI__ dans la barre de recherche du programme.</span><span class="sxs-lookup"><span data-stu-id="e0372-151">Once on this screen type __Azure CLI__ into the program search bar.</span></span> <span data-ttu-id="e0372-152">Le programme à désinstaller est listé sous le nom __Microsoft CLI 2.0 pour Azure__.</span><span class="sxs-lookup"><span data-stu-id="e0372-152">The program to uninstall is listed as __Microsoft CLI 2.0 for Azure__.</span></span> <span data-ttu-id="e0372-153">Sélectionnez cette application, puis cliquez sur le bouton `Uninstall`.</span><span class="sxs-lookup"><span data-stu-id="e0372-153">Select this application, then click the `Uninstall` button.</span></span>

## <a name="next-steps"></a><span data-ttu-id="e0372-154">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="e0372-154">Next Steps</span></span>

<span data-ttu-id="e0372-155">Maintenant que vous avez installé l’interface CLI, découvrez ses fonctionnalités et ses commandes courantes.</span><span class="sxs-lookup"><span data-stu-id="e0372-155">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="e0372-156">Prise en main de l’interface Azure CLI</span><span class="sxs-lookup"><span data-stu-id="e0372-156">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
