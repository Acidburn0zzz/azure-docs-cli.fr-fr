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
ms.openlocfilehash: e8103b8b235c7ac003b2434c72e69839a39f4a9f
ms.sourcegitcommit: e672284b83a9dbb46cbc54be17f5cd8512310e0a
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/20/2021
ms.locfileid: "98594187"
---
# <a name="install-azure-cli-on-windows"></a><span data-ttu-id="507d3-103">Installer Azure CLI sur Windows</span><span class="sxs-lookup"><span data-stu-id="507d3-103">Install Azure CLI on Windows</span></span>

<span data-ttu-id="507d3-104">Pour Windows, Azure CLI est installée à l’aide d’un fichier MSI, ce qui vous donne accès à l’interface CLI via l’Invite de commande Windows (CMD) ou PowerShell.</span><span class="sxs-lookup"><span data-stu-id="507d3-104">For Windows, the Azure CLI is installed via a MSI, which gives you access to the CLI through the Windows Command Prompt (CMD) or PowerShell.</span></span>
<span data-ttu-id="507d3-105">Lors de son installation sur le sous-système Windows pour Linux (WSL), des packages sont disponibles pour votre distribution Linux.</span><span class="sxs-lookup"><span data-stu-id="507d3-105">When installing for Windows Subsystem for Linux (WSL), packages are available for your Linux distribution.</span></span> <span data-ttu-id="507d3-106">Consultez la [page d’installation principale](install-azure-cli.md) pour obtenir la liste des gestionnaires de packages pris en charge ou pour savoir comment installer manuellement avec le sous-système Windows pour Linux.</span><span class="sxs-lookup"><span data-stu-id="507d3-106">See the [main install page](install-azure-cli.md) for the list of supported package managers or how to install manually under WSL.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

## <a name="install-or-update"></a><span data-ttu-id="507d3-107">Installation ou mise à jour</span><span class="sxs-lookup"><span data-stu-id="507d3-107">Install or update</span></span>

<span data-ttu-id="507d3-108">Le fichier MSI distribuable est utilisé pour l’installation ou la mise à jour d’Azure CLI sur Windows.</span><span class="sxs-lookup"><span data-stu-id="507d3-108">The MSI distributable is used for installing or updating the Azure CLI on Windows.</span></span> <span data-ttu-id="507d3-109">Vous n’avez pas besoin de désinstaller les versions actuelles avant d’utiliser le programme d’installation MSI, car celui-ci met à jour toute version existante.</span><span class="sxs-lookup"><span data-stu-id="507d3-109">You don't need to uninstall current versions before using the MSI installer because the MSI will update any existing version.</span></span>

# <a name="microsoft-installer-msi"></a>[<span data-ttu-id="507d3-110">Microsoft Installer (MSI)</span><span class="sxs-lookup"><span data-stu-id="507d3-110">Microsoft Installer (MSI)</span></span>](#tab/azure-cli)

<span data-ttu-id="507d3-111">Lorsque le programme d’installation vous demande s’il peut apporter des modifications à votre ordinateur, cliquez sur la case « Oui ».</span><span class="sxs-lookup"><span data-stu-id="507d3-111">When the installer asks if it can make changes to your computer, click the "Yes" box.</span></span>

### <a name="azure-cli-current-version"></a><span data-ttu-id="507d3-112">Version actuelle d’Azure CLI</span><span class="sxs-lookup"><span data-stu-id="507d3-112">Azure CLI current version</span></span>

<span data-ttu-id="507d3-113">Téléchargez et installez la version actuelle d’Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="507d3-113">Download and install the current release of the Azure CLI.</span></span>  

> [!div class="nextstepaction"]
> [<span data-ttu-id="507d3-114">Version actuelle d’Azure CLI</span><span class="sxs-lookup"><span data-stu-id="507d3-114">Current release of the Azure CLI</span></span>](https://aka.ms/installazurecliwindows)

### <a name="azure-cli-beta-version"></a><span data-ttu-id="507d3-115">Version bêta d’Azure CLI</span><span class="sxs-lookup"><span data-stu-id="507d3-115">Azure CLI beta version</span></span>

<span data-ttu-id="507d3-116">La version bêta d’Azure CLI prend en charge toutes les commandes CLI disponibles dans la version finale actuelle.</span><span class="sxs-lookup"><span data-stu-id="507d3-116">The beta version of the Azure CLI supports all CLI commands that you will find in the current released version.</span></span> <span data-ttu-id="507d3-117">La version bêta est une migration de la version publiée d’Azure CLI, car la plateforme d’authentification AAD (v1.0) est sur le point d’être dépréciée.</span><span class="sxs-lookup"><span data-stu-id="507d3-117">The beta version is a migration from the released Azure CLI as the AAD authentication platform (v1.0) is being deprecated.</span></span>  <span data-ttu-id="507d3-118">La [Plateforme d’identité Microsoft (v2.0)](/azure/active-directory/develop/v2-overview) est la nouvelle méthode d’authentification utilisée par version bêta d’Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="507d3-118">[Microsoft Identity platform (v2.0)](/azure/active-directory/develop/v2-overview) is the new authentication method and is used by Azure CLI beta.</span></span>  <span data-ttu-id="507d3-119">Nous vous recommandons d’essayer la version bêta à l’avance.</span><span class="sxs-lookup"><span data-stu-id="507d3-119">We recommend that you try the beta version in advance.</span></span>  

<span data-ttu-id="507d3-120">Pour plus d’informations sur la version bêta d’Azure CLI, consultez les [notes de publication](./release-notes-azure-cli.md?tabs=azure-cli-beta).</span><span class="sxs-lookup"><span data-stu-id="507d3-120">For more information about Azure CLI beta, please see [release notes](./release-notes-azure-cli.md?tabs=azure-cli-beta).</span></span>

> [!IMPORTANT]
>
> <span data-ttu-id="507d3-121">La version bêta ne garantit pas la qualité du produit. Ne l’utilisez pas dans votre environnement de production.</span><span class="sxs-lookup"><span data-stu-id="507d3-121">The beta version does not guarantee product level quality so it should not be used in your production environment.</span></span>

<span data-ttu-id="507d3-122">Téléchargez et installez la version bêta d’Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="507d3-122">Download and install the beta version of the Azure CLI.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="507d3-123">Version bêta d’Azure CLI</span><span class="sxs-lookup"><span data-stu-id="507d3-123">Beta release of the Azure CLI</span></span>](https://aka.ms/installazurecliwindowsbeta)

# <a name="microsoft-installer-msi-with-command"></a>[<span data-ttu-id="507d3-124">Microsoft Installer (MSI) avec commande</span><span class="sxs-lookup"><span data-stu-id="507d3-124">Microsoft Installer (MSI) with Command</span></span>](#tab/azure-powershell)

### <a name="powershell-command"></a><span data-ttu-id="507d3-125">Commande PowerShell</span><span class="sxs-lookup"><span data-stu-id="507d3-125">Powershell Command</span></span>

<span data-ttu-id="507d3-126">Vous pouvez également installer Azure CLI en utilisant PowerShell.</span><span class="sxs-lookup"><span data-stu-id="507d3-126">You can also install the Azure CLI using PowerShell.</span></span> <span data-ttu-id="507d3-127">Démarrez PowerShell en tant qu’administrateur et exécutez la commande suivante :</span><span class="sxs-lookup"><span data-stu-id="507d3-127">Start PowerShell as administrator and run the following command:</span></span>

   ```PowerShell
   Invoke-WebRequest -Uri https://aka.ms/installazurecliwindows -OutFile .\AzureCLI.msi; Start-Process msiexec.exe -Wait -ArgumentList '/I AzureCLI.msi /quiet'; rm .\AzureCLI.msi
   ```

<span data-ttu-id="507d3-128">Cette opération télécharge et installe la dernière version d’Azure CLI pour Windows.</span><span class="sxs-lookup"><span data-stu-id="507d3-128">This will download and install the latest version of the Azure CLI for Windows.</span></span> <span data-ttu-id="507d3-129">Si une version est déjà installée, le programme d’installation met à jour la version existante.</span><span class="sxs-lookup"><span data-stu-id="507d3-129">If you already have a version installed, the installer will update the existing version.</span></span> <span data-ttu-id="507d3-130">Une fois l’installation terminée, vous devez rouvrir PowerShell pour utiliser Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="507d3-130">After the installation is complete, you will need to reopen PowerShell to use the Azure CLI.</span></span>

### <a name="azure-cli-command-for-update-only"></a><span data-ttu-id="507d3-131">Commande Azure CLI (pour mise à jour uniquement)</span><span class="sxs-lookup"><span data-stu-id="507d3-131">Azure CLI Command (for update only)</span></span>
[!INCLUDE [az-upgrade](includes/az-upgrade.md)]

---

## <a name="run-the-azure-cli"></a><span data-ttu-id="507d3-132">Exécuter Azure CLI</span><span class="sxs-lookup"><span data-stu-id="507d3-132">Run the Azure CLI</span></span>

<span data-ttu-id="507d3-133">Vous pouvez désormais exécuter l’interface de ligne de commande Azure avec la commande `az` à partir de l’invite de commandes Windows ou PowerShell.</span><span class="sxs-lookup"><span data-stu-id="507d3-133">You can now run the Azure CLI with the `az` command from either Windows Command Prompt or PowerShell.</span></span> <span data-ttu-id="507d3-134">PowerShell offre des fonctionnalités de saisie semi-automatique via la touche TAB non disponibles à partir de l’invite de commandes Windows.</span><span class="sxs-lookup"><span data-stu-id="507d3-134">PowerShell offers some tab completion features not available from Windows Command Prompt.</span></span> <span data-ttu-id="507d3-135">Pour vous connecter, exécutez la commande [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="507d3-135">To sign in, run the [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="507d3-136">Pour en savoir plus sur les différentes méthodes d’authentification, consultez [Se connecter avec Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="507d3-136">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="507d3-137">Dépannage</span><span class="sxs-lookup"><span data-stu-id="507d3-137">Troubleshooting</span></span>

<span data-ttu-id="507d3-138">Voici certains problèmes courants lors de l’installation sur Windows.</span><span class="sxs-lookup"><span data-stu-id="507d3-138">Here are some common problems seen when installing on Windows.</span></span> <span data-ttu-id="507d3-139">Si vous rencontrez un problème qui n’est pas traité ici, [signalez ce problème sur GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="507d3-139">If you experience a problem not covered here, [file an issue on GitHub](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="proxy-blocks-connection"></a><span data-ttu-id="507d3-140">Le proxy bloque la connexion</span><span class="sxs-lookup"><span data-stu-id="507d3-140">Proxy blocks connection</span></span>

<span data-ttu-id="507d3-141">Si vous ne pouvez pas télécharger le programme d’installation MSI car votre serveur proxy bloque la connexion, vérifiez que votre proxy est configuré correctement.</span><span class="sxs-lookup"><span data-stu-id="507d3-141">If you can't download the MSI installer because your proxy is blocking the connection, make sure that you have your proxy properly configured.</span></span> <span data-ttu-id="507d3-142">Pour Windows 10, ces paramètres sont gérés dans le volet `Settings > Network & Internet > Proxy`.</span><span class="sxs-lookup"><span data-stu-id="507d3-142">For Windows 10, these settings are managed in the `Settings > Network & Internet > Proxy` pane.</span></span> <span data-ttu-id="507d3-143">Contactez votre administrateur système pour connaître les paramètres requis, ou les situations où votre ordinateur peut être géré par configuration ou nécessiter une configuration avancée.</span><span class="sxs-lookup"><span data-stu-id="507d3-143">Contact your system administrator for the required settings, or for situations where your machine may be configuration-managed or require advanced setup.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="507d3-144">Ces paramètres sont également requis pour l’accès aux services Azure avec l’interface CLI, PowerShell ou l’invite de commandes.</span><span class="sxs-lookup"><span data-stu-id="507d3-144">These settings are also required to be able to access Azure services with the CLI, from both PowerShell or the Command Prompt.</span></span> <span data-ttu-id="507d3-145">Dans PowerShell, pour ce faire, utilisez la commande suivante :</span><span class="sxs-lookup"><span data-stu-id="507d3-145">In PowerShell, you do this with the following command:</span></span>
>
> ```powershell
> (New-Object System.Net.WebClient).Proxy.Credentials = `
>   [System.Net.CredentialCache]::DefaultNetworkCredentials
> ```

<span data-ttu-id="507d3-146">Pour obtenir le fichier MSI, votre proxy doit autoriser les connexions HTTPS aux adresses suivantes :</span><span class="sxs-lookup"><span data-stu-id="507d3-146">In order to get the MSI, your proxy needs to allow HTTPS connections to the following addresses:</span></span>

* `https://aka.ms/`
* `https://azcliprod.blob.core.windows.net/`

## <a name="uninstall"></a><span data-ttu-id="507d3-147">Désinstaller l’interface</span><span class="sxs-lookup"><span data-stu-id="507d3-147">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="507d3-148">La désinstallation d’Azure CLI s’effectue à partir de la liste « Applications et fonctionnalités » dans Windows.</span><span class="sxs-lookup"><span data-stu-id="507d3-148">You uninstall the Azure CLI from the Windows "Apps and Features" list.</span></span> <span data-ttu-id="507d3-149">Pour désinstaller :</span><span class="sxs-lookup"><span data-stu-id="507d3-149">To uninstall:</span></span>

| <span data-ttu-id="507d3-150">Plateforme</span><span class="sxs-lookup"><span data-stu-id="507d3-150">Platform</span></span> | <span data-ttu-id="507d3-151">Instructions</span><span class="sxs-lookup"><span data-stu-id="507d3-151">Instructions</span></span> |
|---|---|
| <span data-ttu-id="507d3-152">Windows 10</span><span class="sxs-lookup"><span data-stu-id="507d3-152">Windows 10</span></span> | <span data-ttu-id="507d3-153">Démarrer > Paramètres > Applications</span><span class="sxs-lookup"><span data-stu-id="507d3-153">Start > Settings > Apps</span></span> |
| <span data-ttu-id="507d3-154">Windows 8 et Windows 7</span><span class="sxs-lookup"><span data-stu-id="507d3-154">Windows 8 and Windows 7</span></span> | <span data-ttu-id="507d3-155">Démarrer > Panneau de configuration > Programmes > Désinstaller un programme</span><span class="sxs-lookup"><span data-stu-id="507d3-155">Start > Control Panel > Programs > Uninstall a program</span></span> |

<span data-ttu-id="507d3-156">Une fois sur cet écran, tapez __Azure CLI__ dans la barre de recherche du programme.</span><span class="sxs-lookup"><span data-stu-id="507d3-156">Once on this screen type __Azure CLI__ into the program search bar.</span></span> <span data-ttu-id="507d3-157">Le programme à désinstaller est listé sous le nom __Microsoft CLI 2.0 pour Azure__.</span><span class="sxs-lookup"><span data-stu-id="507d3-157">The program to uninstall is listed as __Microsoft CLI 2.0 for Azure__.</span></span> <span data-ttu-id="507d3-158">Sélectionnez cette application, puis cliquez sur le bouton `Uninstall`.</span><span class="sxs-lookup"><span data-stu-id="507d3-158">Select this application, then click the `Uninstall` button.</span></span>

## <a name="next-steps"></a><span data-ttu-id="507d3-159">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="507d3-159">Next Steps</span></span>

<span data-ttu-id="507d3-160">Maintenant que vous avez installé l’interface CLI, découvrez ses fonctionnalités et ses commandes courantes.</span><span class="sxs-lookup"><span data-stu-id="507d3-160">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="507d3-161">Prise en main de l’interface Azure CLI</span><span class="sxs-lookup"><span data-stu-id="507d3-161">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)