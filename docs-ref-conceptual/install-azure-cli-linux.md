---
title: Installer manuellement Azure CLI pour Linux
description: Comment installer manuellement Azure CLI sur Linux
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 09/09/2018
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 9a98da54f397c1fd03a7cc6b581a769afe84ef88
ms.sourcegitcommit: ee64dc738cfe689a2a479e32a87bf420f96c31c8
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/06/2020
ms.locfileid: "77779582"
---
# <a name="install-azure-cli-on-linux-manually"></a><span data-ttu-id="585d7-103">Installer manuellement Azure CLI sur Linux</span><span class="sxs-lookup"><span data-stu-id="585d7-103">Install Azure CLI on Linux manually</span></span>

<span data-ttu-id="585d7-104">S’il n’existe aucun package pour l’interface Azure CLI pour vous et votre distribution, installez l’interface CLI manuellement en exécutant un script.</span><span class="sxs-lookup"><span data-stu-id="585d7-104">If there's no package for the Azure CLI for you your distribution, install the CLI manually by running a script.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

> [!NOTE]
> <span data-ttu-id="585d7-105">Il est fortement recommandé d’installer l’interface CLI avec un gestionnaire de package.</span><span class="sxs-lookup"><span data-stu-id="585d7-105">It's strongly recommend to install the CLI with a package manager.</span></span> <span data-ttu-id="585d7-106">Un gestionnaire de package permet de s’assurer que vous obtenez toujours les dernières mises à jour et garantit la stabilité des composants de l’interface CLI.</span><span class="sxs-lookup"><span data-stu-id="585d7-106">A package manager makes sure you always get the latest updates, and guarantees the stability of CLI components.</span></span> <span data-ttu-id="585d7-107">Vérifiez s’il existe un package pour votre distribution avant d’installer manuellement.</span><span class="sxs-lookup"><span data-stu-id="585d7-107">Check and see if there is a package for your distribution before installing manually.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="585d7-108">Conditions préalables requises</span><span class="sxs-lookup"><span data-stu-id="585d7-108">Prerequisites</span></span>

<span data-ttu-id="585d7-109">L’interface CLI requiert les logiciels suivants :</span><span class="sxs-lookup"><span data-stu-id="585d7-109">The CLI requires the following software:</span></span>

* <span data-ttu-id="585d7-110">[Python 3.6.x, 3.7.x ou 3.8.x](https://www.python.org/downloads/).</span><span class="sxs-lookup"><span data-stu-id="585d7-110">[Python 3.6.x, 3.7.x or 3.8.x](https://www.python.org/downloads/).</span></span> 
* [<span data-ttu-id="585d7-111">libffi</span><span class="sxs-lookup"><span data-stu-id="585d7-111">libffi</span></span>](https://sourceware.org/libffi/)
* [<span data-ttu-id="585d7-112">OpenSSL 1.0.2</span><span class="sxs-lookup"><span data-stu-id="585d7-112">OpenSSL 1.0.2</span></span>](https://www.openssl.org/source/)

> [!IMPORTANT]
>
> <span data-ttu-id="585d7-113">L’interface CLI a retiré la prise en charge de Python 2.7 depuis la version `2.1.0`.</span><span class="sxs-lookup"><span data-stu-id="585d7-113">The CLI has dropped support for Python 2.7 since version `2.1.0`.</span></span> <span data-ttu-id="585d7-114">Les nouvelles versions ne garantissent plus une exécution correcte de Python 2.7.</span><span class="sxs-lookup"><span data-stu-id="585d7-114">New versions no longer guarantee to run with Python 2.7 correctly.</span></span>

## <a name="install-or-update"></a><span data-ttu-id="585d7-115">Installation ou mise à jour</span><span class="sxs-lookup"><span data-stu-id="585d7-115">Install or update</span></span>

<span data-ttu-id="585d7-116">L’installation et la mise à jour de l’interface CLI nécessitent toutes de réexécuter le script d’installation.</span><span class="sxs-lookup"><span data-stu-id="585d7-116">Both installing and updating the CLI requires re-running the install script.</span></span> <span data-ttu-id="585d7-117">Installez l’interface CLI en exécutant `curl`.</span><span class="sxs-lookup"><span data-stu-id="585d7-117">Install the CLI by running `curl`.</span></span>

```bash
curl -L https://aka.ms/InstallAzureCli | bash
```

<span data-ttu-id="585d7-118">Le script peut également être téléchargé et exécuté localement.</span><span class="sxs-lookup"><span data-stu-id="585d7-118">The script can also be downloaded and run locally.</span></span> <span data-ttu-id="585d7-119">Vous devrez peut-être redémarrer votre interpréteur de commandes pour que certaines modifications soient prises en compte.</span><span class="sxs-lookup"><span data-stu-id="585d7-119">You may have to restart your shell in order for changes to take effect.</span></span>

<span data-ttu-id="585d7-120">Vous pouvez ensuite exécuter l’interface de ligne de commande Azure avec la commande `az`.</span><span class="sxs-lookup"><span data-stu-id="585d7-120">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="585d7-121">Pour vous connecter, utilisez la commande [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="585d7-121">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="585d7-122">Pour en savoir plus sur les différentes méthodes d’authentification, consultez [Se connecter avec Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="585d7-122">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="585d7-123">Dépannage</span><span class="sxs-lookup"><span data-stu-id="585d7-123">Troubleshooting</span></span>

<span data-ttu-id="585d7-124">Voici certains problèmes courants rencontrés pendant une installation manuelle.</span><span class="sxs-lookup"><span data-stu-id="585d7-124">Here are some common problems seen during a manual installation.</span></span> <span data-ttu-id="585d7-125">Si vous rencontrez un problème qui n’est pas traité ici, [signalez ce problème sur GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="585d7-125">If you experience a problem not covered here, [file an issue on GitHub](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="curl-object-moved-error"></a><span data-ttu-id="585d7-126">erreur curl « Objet déplacé »</span><span class="sxs-lookup"><span data-stu-id="585d7-126">curl "Object Moved" error</span></span>

<span data-ttu-id="585d7-127">Si la commande `curl` renvoie une erreur concernant le `-L` paramètre ou un message d’erreur indiquant « Objet déplacé », essayez d’utiliser l’URL complète plutôt que la `aka.ms` redirection :</span><span class="sxs-lookup"><span data-stu-id="585d7-127">If you get an error from `curl` related to the `-L` parameter, or an error message including the text "Object Moved", try using the full URL instead of the `aka.ms` redirect:</span></span>

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

### <a name="az-command-not-found"></a><span data-ttu-id="585d7-128">`az` commande introuvable</span><span class="sxs-lookup"><span data-stu-id="585d7-128">`az` command not found</span></span>

<span data-ttu-id="585d7-129">Si vous ne pouvez pas exécuter la commande après l’installation et après avoir utilisé `bash` et `zsh`, effacez le cache de hachage de commande de votre interpréteur de commandes.</span><span class="sxs-lookup"><span data-stu-id="585d7-129">If you can't run the command after installation and using `bash` or `zsh`, clear your shell's command hash cache.</span></span> <span data-ttu-id="585d7-130">Exécuter</span><span class="sxs-lookup"><span data-stu-id="585d7-130">Run</span></span>

```bash
hash -r
```

<span data-ttu-id="585d7-131">et vérifiez si le problème est résolu.</span><span class="sxs-lookup"><span data-stu-id="585d7-131">and check if the problem is resolved.</span></span>

<span data-ttu-id="585d7-132">Le problème peut également survenir si vous n’avez pas redémarré votre interpréteur de commandes après l’installation.</span><span class="sxs-lookup"><span data-stu-id="585d7-132">The issue can also occur if you didn't restart your shell after installation.</span></span> <span data-ttu-id="585d7-133">Assurez-vous que l’emplacement de la commande `az` se trouve dans votre `$PATH`.</span><span class="sxs-lookup"><span data-stu-id="585d7-133">Make sure that the location of the `az` command is in your `$PATH`.</span></span> <span data-ttu-id="585d7-134">L’emplacement de la commande `az` est</span><span class="sxs-lookup"><span data-stu-id="585d7-134">The location of the `az` command is</span></span>

```bash
<install path>/bin
```

### <a name="proxy-blocks-connection"></a><span data-ttu-id="585d7-135">Le proxy bloque la connexion</span><span class="sxs-lookup"><span data-stu-id="585d7-135">Proxy blocks connection</span></span>

[!INCLUDE[configure-proxy](includes/configure-proxy.md)]

<span data-ttu-id="585d7-136">Pour obtenir les scripts d’installation, votre proxy doit autoriser les connexions HTTPS aux adresses suivantes :</span><span class="sxs-lookup"><span data-stu-id="585d7-136">In order to get the installation scripts, your proxy needs to allow HTTPS connections to the following addresses:</span></span>

* `https://aka.ms/`
* `https://azurecliprod.blob.core.windows.net/`
* `https://pypi.python.org`
* <span data-ttu-id="585d7-137">Points de terminaison utilisés par le gestionnaire de package de votre distribution (le cas échéant) pour les packages de base</span><span class="sxs-lookup"><span data-stu-id="585d7-137">Endpoints used by your distribution's package manager (if any) for core packages</span></span>

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="uninstall"></a><span data-ttu-id="585d7-138">Désinstaller l’interface</span><span class="sxs-lookup"><span data-stu-id="585d7-138">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="585d7-139">Désinstallez l’interface de ligne de commande en supprimant directement les fichiers de l’emplacement spécifié lors de l’installation.</span><span class="sxs-lookup"><span data-stu-id="585d7-139">Uninstall the CLI by directly deleting the files from the location chosen at the time of installation.</span></span> <span data-ttu-id="585d7-140">L’emplacement d’installation par défaut est `$HOME`.</span><span class="sxs-lookup"><span data-stu-id="585d7-140">The default install location is `$HOME`.</span></span>

1. <span data-ttu-id="585d7-141">Supprimez les fichiers CLI installés.</span><span class="sxs-lookup"><span data-stu-id="585d7-141">Remove the installed CLI files.</span></span>

   ```bash
   rm -r <install location>/lib/azure-cli
   rm <install location>/bin/az
   ```

2. <span data-ttu-id="585d7-142">Modifiez votre fichier `$HOME/.bash_profile` pour supprimer la ligne suivante :</span><span class="sxs-lookup"><span data-stu-id="585d7-142">Modify your `$HOME/.bash_profile` file to remove the following line:</span></span>

   ```text
   <install location>/lib/azure-cli/az.completion
   ```

3. <span data-ttu-id="585d7-143">Si vous utilisez `bash` ou `zsh`, rechargez le cache de commande de l’interpréteur de commandes.</span><span class="sxs-lookup"><span data-stu-id="585d7-143">If using `bash` or `zsh`, reload your shell's command cache.</span></span>

   ```bash
   hash -r
   ```

## <a name="next-steps"></a><span data-ttu-id="585d7-144">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="585d7-144">Next Steps</span></span>

<span data-ttu-id="585d7-145">Maintenant que vous avez installé l’interface CLI, découvrez ses fonctionnalités et ses commandes courantes.</span><span class="sxs-lookup"><span data-stu-id="585d7-145">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="585d7-146">Prise en main de l’interface Azure CLI</span><span class="sxs-lookup"><span data-stu-id="585d7-146">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
