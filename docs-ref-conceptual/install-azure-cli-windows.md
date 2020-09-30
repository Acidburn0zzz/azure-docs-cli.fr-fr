---
title: Installer l’interface de ligne de commande Azure pour Windows
description: Comment installer Azure CLI sur Windows
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.prod: azure
ms.date: 06/16/2020
ms.topic: conceptual
ms.devlang: azurecli
ms.technology: azure-cli
ms.custom: devx-track-azurecli
ms.openlocfilehash: 39668b267d3374dd1bdb5f7b1f5e0f0847d2c2fa
ms.sourcegitcommit: 5d29362589078b66d15f5cd494fe903a5195658d
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/25/2020
ms.locfileid: "91225811"
---
# <a name="install-azure-cli-on-windows"></a><span data-ttu-id="1b4d8-103">Installer Azure CLI sur Windows</span><span class="sxs-lookup"><span data-stu-id="1b4d8-103">Install Azure CLI on Windows</span></span>

<span data-ttu-id="1b4d8-104">Pour Windows, Azure CLI est installée à l’aide d’un fichier MSI, ce qui vous donne accès à l’interface CLI via l’Invite de commande Windows (CMD) ou PowerShell.</span><span class="sxs-lookup"><span data-stu-id="1b4d8-104">For Windows, the Azure CLI is installed via a MSI, which gives you access to the CLI through the Windows Command Prompt (CMD) or PowerShell.</span></span>
<span data-ttu-id="1b4d8-105">Lors de son installation sur le sous-système Windows pour Linux (WSL), des packages sont disponibles pour votre distribution Linux.</span><span class="sxs-lookup"><span data-stu-id="1b4d8-105">When installing for Windows Subsystem for Linux (WSL), packages are available for your Linux distribution.</span></span> <span data-ttu-id="1b4d8-106">Consultez la [page d’installation principale](install-azure-cli.md) pour obtenir la liste des gestionnaires de packages pris en charge ou pour savoir comment installer manuellement avec le sous-système Windows pour Linux.</span><span class="sxs-lookup"><span data-stu-id="1b4d8-106">See the [main install page](install-azure-cli.md) for the list of supported package managers or how to install manually under WSL.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

## <a name="install-or-update"></a><span data-ttu-id="1b4d8-107">Installation ou mise à jour</span><span class="sxs-lookup"><span data-stu-id="1b4d8-107">Install or update</span></span>

<span data-ttu-id="1b4d8-108">Le fichier MSI distribuable est utilisé pour l’installation ou la mise à jour d’Azure CLI sur Windows.</span><span class="sxs-lookup"><span data-stu-id="1b4d8-108">The MSI distributable is used for installing or updating the Azure CLI on Windows.</span></span> <span data-ttu-id="1b4d8-109">Vous n’avez pas besoin de désinstaller les versions actuelles avant d’utiliser le programme d’installation MSI, car celui-ci met à jour toute version existante.</span><span class="sxs-lookup"><span data-stu-id="1b4d8-109">You don't need to uninstall current versions before using the MSI installer because the MSI will update any existing version.</span></span>

# <a name="microsoft-installer-msi"></a>[<span data-ttu-id="1b4d8-110">Microsoft Installer (MSI)</span><span class="sxs-lookup"><span data-stu-id="1b4d8-110">Microsoft Installer (MSI)</span></span>](#tab/azure-cli)

<span data-ttu-id="1b4d8-111">Lorsque le programme d’installation vous demande s’il peut apporter des modifications à votre ordinateur, cliquez sur la case « Oui ».</span><span class="sxs-lookup"><span data-stu-id="1b4d8-111">When the installer asks if it can make changes to your computer, click the "Yes" box.</span></span>

### <a name="azure-cli-current-version"></a><span data-ttu-id="1b4d8-112">Version actuelle d’Azure CLI</span><span class="sxs-lookup"><span data-stu-id="1b4d8-112">Azure CLI current version</span></span>

<span data-ttu-id="1b4d8-113">Téléchargez et installez la version actuelle d’Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="1b4d8-113">Download and install the current release of the Azure CLI.</span></span>  

> [!div class="nextstepaction"]
> [<span data-ttu-id="1b4d8-114">Version actuelle d’Azure CLI</span><span class="sxs-lookup"><span data-stu-id="1b4d8-114">Current release of the Azure CLI</span></span>](https://aka.ms/installazurecliwindows)

### <a name="azure-cli-beta-version"></a><span data-ttu-id="1b4d8-115">Version bêta d’Azure CLI</span><span class="sxs-lookup"><span data-stu-id="1b4d8-115">Azure CLI beta version</span></span>

<span data-ttu-id="1b4d8-116">La version bêta d’Azure CLI prend en charge toutes les commandes CLI disponibles dans la version finale actuelle.</span><span class="sxs-lookup"><span data-stu-id="1b4d8-116">The beta version of the Azure CLI supports all CLI commands that you will find in the current released version.</span></span> <span data-ttu-id="1b4d8-117">La version bêta est une migration de la version publiée d’Azure CLI, car la plateforme d’authentification AAD (v1.0) est sur le point d’être dépréciée.</span><span class="sxs-lookup"><span data-stu-id="1b4d8-117">The beta version is a migration from the released Azure CLI as the AAD authentication platform (v1.0) is being deprecated.</span></span>  <span data-ttu-id="1b4d8-118">La [Plateforme d’identité Microsoft (v2.0)](/azure/active-directory/develop/v2-overview) est la nouvelle méthode d’authentification utilisée par version bêta d’Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="1b4d8-118">[Microsoft Identity platform (v2.0)](/azure/active-directory/develop/v2-overview) is the new authentication method and is used by Azure CLI beta.</span></span>  <span data-ttu-id="1b4d8-119">Nous vous recommandons d’essayer la version bêta à l’avance.</span><span class="sxs-lookup"><span data-stu-id="1b4d8-119">We recommend that you try the beta version in advance.</span></span>  

<span data-ttu-id="1b4d8-120">Pour plus d’informations sur la version bêta d’Azure CLI, consultez les [notes de publication](./release-notes-azure-cli.md?tabs=azure-cli-beta).</span><span class="sxs-lookup"><span data-stu-id="1b4d8-120">For more information about Azure CLI beta, please see [release notes](./release-notes-azure-cli.md?tabs=azure-cli-beta).</span></span>

> [!IMPORTANT]
>
> <span data-ttu-id="1b4d8-121">La version bêta ne garantit pas la qualité du produit. Ne l’utilisez pas dans votre environnement de production.</span><span class="sxs-lookup"><span data-stu-id="1b4d8-121">The beta version does not guarantee product level quality so it should not be used in your production environment.</span></span>

<span data-ttu-id="1b4d8-122">Téléchargez et installez la version bêta d’Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="1b4d8-122">Download and install the beta version of the Azure CLI.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="1b4d8-123">Version bêta d’Azure CLI</span><span class="sxs-lookup"><span data-stu-id="1b4d8-123">Beta release of the Azure CLI</span></span>](https://aka.ms/installazurecliwindowsbeta)

# <a name="microsoft-installer-msi-with-powershell"></a>[<span data-ttu-id="1b4d8-124">Microsoft Installer (MSI) avec PowerShell</span><span class="sxs-lookup"><span data-stu-id="1b4d8-124">Microsoft Installer (MSI) with PowerShell</span></span>](#tab/azure-powershell)

<span data-ttu-id="1b4d8-125">Vous pouvez également installer Azure CLI en utilisant PowerShell.</span><span class="sxs-lookup"><span data-stu-id="1b4d8-125">You can also install the Azure CLI using PowerShell.</span></span> <span data-ttu-id="1b4d8-126">Démarrez PowerShell en tant qu’administrateur et exécutez la commande suivante :</span><span class="sxs-lookup"><span data-stu-id="1b4d8-126">Start PowerShell as administrator and run the following command:</span></span>

   ```PowerShell
   Invoke-WebRequest -Uri https://aka.ms/installazurecliwindows -OutFile .\AzureCLI.msi; Start-Process msiexec.exe -Wait -ArgumentList '/I AzureCLI.msi /quiet'; rm .\AzureCLI.msi
   ```

<span data-ttu-id="1b4d8-127">Cette opération télécharge et installe la dernière version d’Azure CLI pour Windows.</span><span class="sxs-lookup"><span data-stu-id="1b4d8-127">This will download and install the latest version of the Azure CLI for Windows.</span></span> <span data-ttu-id="1b4d8-128">Si une version est déjà installée, le programme d’installation met à jour la version existante.</span><span class="sxs-lookup"><span data-stu-id="1b4d8-128">If you already have a version installed, the installer will update the existing version.</span></span> <span data-ttu-id="1b4d8-129">Une fois l’installation terminée, vous devez rouvrir PowerShell pour utiliser Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="1b4d8-129">After the installation is complete, you will need to reopen PowerShell to use the Azure CLI.</span></span>

---

## <a name="run-the-azure-cli"></a><span data-ttu-id="1b4d8-130">Exécuter Azure CLI</span><span class="sxs-lookup"><span data-stu-id="1b4d8-130">Run the Azure CLI</span></span>

<span data-ttu-id="1b4d8-131">Vous pouvez désormais exécuter l’interface de ligne de commande Azure avec la commande `az` à partir de l’invite de commandes Windows ou PowerShell.</span><span class="sxs-lookup"><span data-stu-id="1b4d8-131">You can now run the Azure CLI with the `az` command from either Windows Command Prompt or PowerShell.</span></span> <span data-ttu-id="1b4d8-132">PowerShell offre des fonctionnalités de saisie semi-automatique via la touche TAB non disponibles à partir de l’invite de commandes Windows.</span><span class="sxs-lookup"><span data-stu-id="1b4d8-132">PowerShell offers some tab completion features not available from Windows Command Prompt.</span></span> <span data-ttu-id="1b4d8-133">Pour vous connecter, exécutez la commande [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="1b4d8-133">To sign in, run the [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="1b4d8-134">Pour en savoir plus sur les différentes méthodes d’authentification, consultez [Se connecter avec Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="1b4d8-134">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="1b4d8-135">Dépannage</span><span class="sxs-lookup"><span data-stu-id="1b4d8-135">Troubleshooting</span></span>

<span data-ttu-id="1b4d8-136">Voici certains problèmes courants lors de l’installation sur Windows.</span><span class="sxs-lookup"><span data-stu-id="1b4d8-136">Here are some common problems seen when installing on Windows.</span></span> <span data-ttu-id="1b4d8-137">Si vous rencontrez un problème qui n’est pas traité ici, [signalez ce problème sur GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="1b4d8-137">If you experience a problem not covered here, [file an issue on GitHub](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="proxy-blocks-connection"></a><span data-ttu-id="1b4d8-138">Le proxy bloque la connexion</span><span class="sxs-lookup"><span data-stu-id="1b4d8-138">Proxy blocks connection</span></span>

<span data-ttu-id="1b4d8-139">Si vous ne pouvez pas télécharger le programme d’installation MSI car votre serveur proxy bloque la connexion, vérifiez que votre proxy est configuré correctement.</span><span class="sxs-lookup"><span data-stu-id="1b4d8-139">If you can't download the MSI installer because your proxy is blocking the connection, make sure that you have your proxy properly configured.</span></span> <span data-ttu-id="1b4d8-140">Pour Windows 10, ces paramètres sont gérés dans le volet `Settings > Network & Internet > Proxy`.</span><span class="sxs-lookup"><span data-stu-id="1b4d8-140">For Windows 10, these settings are managed in the `Settings > Network & Internet > Proxy` pane.</span></span> <span data-ttu-id="1b4d8-141">Contactez votre administrateur système pour connaître les paramètres requis, ou les situations où votre ordinateur peut être géré par configuration ou nécessiter une configuration avancée.</span><span class="sxs-lookup"><span data-stu-id="1b4d8-141">Contact your system administrator for the required settings, or for situations where your machine may be configuration-managed or require advanced setup.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="1b4d8-142">Ces paramètres sont également requis pour l’accès aux services Azure avec l’interface CLI, PowerShell ou l’invite de commandes.</span><span class="sxs-lookup"><span data-stu-id="1b4d8-142">These settings are also required to be able to access Azure services with the CLI, from both PowerShell or the Command Prompt.</span></span> <span data-ttu-id="1b4d8-143">Dans PowerShell, pour ce faire, utilisez la commande suivante :</span><span class="sxs-lookup"><span data-stu-id="1b4d8-143">In PowerShell, you do this with the following command:</span></span>
>
> ```powershell
> (New-Object System.Net.WebClient).Proxy.Credentials = `
>   [System.Net.CredentialCache]::DefaultNetworkCredentials
> ```

<span data-ttu-id="1b4d8-144">Pour obtenir le fichier MSI, votre proxy doit autoriser les connexions HTTPS aux adresses suivantes :</span><span class="sxs-lookup"><span data-stu-id="1b4d8-144">In order to get the MSI, your proxy needs to allow HTTPS connections to the following addresses:</span></span>

* `https://aka.ms/`
* `https://azurecliprod.blob.core.windows.net/`

## <a name="uninstall"></a><span data-ttu-id="1b4d8-145">Désinstaller l’interface</span><span class="sxs-lookup"><span data-stu-id="1b4d8-145">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="1b4d8-146">La désinstallation d’Azure CLI s’effectue à partir de la liste « Applications et fonctionnalités » dans Windows.</span><span class="sxs-lookup"><span data-stu-id="1b4d8-146">You uninstall the Azure CLI from the Windows "Apps and Features" list.</span></span> <span data-ttu-id="1b4d8-147">Pour désinstaller :</span><span class="sxs-lookup"><span data-stu-id="1b4d8-147">To uninstall:</span></span>

| <span data-ttu-id="1b4d8-148">Plateforme</span><span class="sxs-lookup"><span data-stu-id="1b4d8-148">Platform</span></span> | <span data-ttu-id="1b4d8-149">Instructions</span><span class="sxs-lookup"><span data-stu-id="1b4d8-149">Instructions</span></span> |
|---|---|
| <span data-ttu-id="1b4d8-150">Windows 10</span><span class="sxs-lookup"><span data-stu-id="1b4d8-150">Windows 10</span></span> | <span data-ttu-id="1b4d8-151">Démarrer > Paramètres > Applications</span><span class="sxs-lookup"><span data-stu-id="1b4d8-151">Start > Settings > Apps</span></span> |
| <span data-ttu-id="1b4d8-152">Windows 8 et Windows 7</span><span class="sxs-lookup"><span data-stu-id="1b4d8-152">Windows 8 and Windows 7</span></span> | <span data-ttu-id="1b4d8-153">Démarrer > Panneau de configuration > Programmes > Désinstaller un programme</span><span class="sxs-lookup"><span data-stu-id="1b4d8-153">Start > Control Panel > Programs > Uninstall a program</span></span> |

<span data-ttu-id="1b4d8-154">Une fois sur cet écran, tapez __Azure CLI__ dans la barre de recherche du programme.</span><span class="sxs-lookup"><span data-stu-id="1b4d8-154">Once on this screen type __Azure CLI__ into the program search bar.</span></span> <span data-ttu-id="1b4d8-155">Le programme à désinstaller est listé sous le nom __Microsoft CLI 2.0 pour Azure__.</span><span class="sxs-lookup"><span data-stu-id="1b4d8-155">The program to uninstall is listed as __Microsoft CLI 2.0 for Azure__.</span></span> <span data-ttu-id="1b4d8-156">Sélectionnez cette application, puis cliquez sur le bouton `Uninstall`.</span><span class="sxs-lookup"><span data-stu-id="1b4d8-156">Select this application, then click the `Uninstall` button.</span></span>

## <a name="next-steps"></a><span data-ttu-id="1b4d8-157">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="1b4d8-157">Next Steps</span></span>

<span data-ttu-id="1b4d8-158">Maintenant que vous avez installé l’interface CLI, découvrez ses fonctionnalités et ses commandes courantes.</span><span class="sxs-lookup"><span data-stu-id="1b4d8-158">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="1b4d8-159">Prise en main de l’interface Azure CLI</span><span class="sxs-lookup"><span data-stu-id="1b4d8-159">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)