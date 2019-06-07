---
title: Installer manuellement Azure CLI pour Linux
description: Comment installer manuellement Azure CLI sur Linux
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 13edb9954678aca627529714aeee02062c720219
ms.sourcegitcommit: 08043c47d3ccf23522b91e6bba3932e312c04c7f
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/04/2019
ms.locfileid: "66516300"
---
# <a name="install-azure-cli-on-linux-manually"></a><span data-ttu-id="745b4-103">Installer manuellement Azure CLI sur Linux</span><span class="sxs-lookup"><span data-stu-id="745b4-103">Install Azure CLI on Linux manually</span></span>

<span data-ttu-id="745b4-104">S’il n’existe aucun package pour l’interface Azure CLI pour vous et votre distribution, installez l’interface CLI manuellement en exécutant un script.</span><span class="sxs-lookup"><span data-stu-id="745b4-104">If there's no package for the Azure CLI for you your distribution, install the CLI manually by running a script.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

> [!NOTE]
> <span data-ttu-id="745b4-105">Il est fortement recommandé d’installer l’interface CLI avec un gestionnaire de package.</span><span class="sxs-lookup"><span data-stu-id="745b4-105">It's strongly recommend to install the CLI with a package manager.</span></span> <span data-ttu-id="745b4-106">Un gestionnaire de package permet de s’assurer que vous obtenez toujours les dernières mises à jour et garantit la stabilité des composants de l’interface CLI.</span><span class="sxs-lookup"><span data-stu-id="745b4-106">A package manager makes sure you always get the latest updates, and guarantees the stability of CLI components.</span></span> <span data-ttu-id="745b4-107">Vérifiez s’il existe un package pour votre distribution avant d’installer manuellement.</span><span class="sxs-lookup"><span data-stu-id="745b4-107">Check and see if there is a package for your distribution before installing manually.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="745b4-108">Prérequis</span><span class="sxs-lookup"><span data-stu-id="745b4-108">Prerequisites</span></span>

<span data-ttu-id="745b4-109">L’interface CLI requiert les logiciels suivants :</span><span class="sxs-lookup"><span data-stu-id="745b4-109">The CLI requires the following software:</span></span>

* <span data-ttu-id="745b4-110">[Python 3.6.x ou 3.7.x](https://www.python.org/downloads/).</span><span class="sxs-lookup"><span data-stu-id="745b4-110">[Python 3.6.x or 3.7.x](https://www.python.org/downloads/).</span></span> 
* [<span data-ttu-id="745b4-111">libffi</span><span class="sxs-lookup"><span data-stu-id="745b4-111">libffi</span></span>](https://sourceware.org/libffi/)
* [<span data-ttu-id="745b4-112">OpenSSL 1.0.2</span><span class="sxs-lookup"><span data-stu-id="745b4-112">OpenSSL 1.0.2</span></span>](https://www.openssl.org/source/)

> [!IMPORTANT]
>
> <span data-ttu-id="745b4-113">L’interface CLI est également compatible avec Python 2.7.x, dont la fin de vie est prévue pour le 1er janvier 2020.</span><span class="sxs-lookup"><span data-stu-id="745b4-113">The CLI is also compatible with Python 2.7.x, which is being end-of-lifed on January 1, 2020.</span></span> <span data-ttu-id="745b4-114">C’est la raison pour laquelle nous vous recommandons d’installer Python 3 afin d’exécuter l’interface CLI.</span><span class="sxs-lookup"><span data-stu-id="745b4-114">For this reason we recommend that you install Python 3 to run the CLI.</span></span>

## <a name="install-or-update"></a><span data-ttu-id="745b4-115">Installation ou mise à jour</span><span class="sxs-lookup"><span data-stu-id="745b4-115">Install or update</span></span>

<span data-ttu-id="745b4-116">L’installation et la mise à jour de l’interface CLI nécessitent toutes de réexécuter le script d’installation.</span><span class="sxs-lookup"><span data-stu-id="745b4-116">Both installing and updating the CLI requires re-running the install script.</span></span> <span data-ttu-id="745b4-117">Installez l’interface CLI en exécutant `curl`.</span><span class="sxs-lookup"><span data-stu-id="745b4-117">Install the CLI by running `curl`.</span></span>

```bash
curl -L https://aka.ms/InstallAzureCli | bash
```

<span data-ttu-id="745b4-118">Le script peut également être téléchargé et exécuté localement.</span><span class="sxs-lookup"><span data-stu-id="745b4-118">The script can also be downloaded and run locally.</span></span> <span data-ttu-id="745b4-119">Vous devrez peut-être redémarrer votre interpréteur de commandes pour que certaines modifications soient prises en compte.</span><span class="sxs-lookup"><span data-stu-id="745b4-119">You may have to restart your shell in order for changes to take effect.</span></span>

<span data-ttu-id="745b4-120">Vous pouvez ensuite exécuter l’interface de ligne de commande Azure avec la commande `az`.</span><span class="sxs-lookup"><span data-stu-id="745b4-120">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="745b4-121">Pour vous connecter, utilisez la commande [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="745b4-121">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="745b4-122">Pour en savoir plus sur les différentes méthodes d’authentification, consultez [Se connecter avec Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="745b4-122">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="745b4-123">Résolution de problèmes</span><span class="sxs-lookup"><span data-stu-id="745b4-123">Troubleshooting</span></span>

<span data-ttu-id="745b4-124">Voici certains problèmes courants rencontrés pendant une installation manuelle.</span><span class="sxs-lookup"><span data-stu-id="745b4-124">Here are some common problems seen during a manual installation.</span></span> <span data-ttu-id="745b4-125">Si vous rencontrez un problème qui n’est pas traité ici, [signalez ce problème sur GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="745b4-125">If you experience a problem not covered here, [file an issue on GitHub](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="curl-object-moved-error"></a><span data-ttu-id="745b4-126">erreur curl « Objet déplacé »</span><span class="sxs-lookup"><span data-stu-id="745b4-126">curl "Object Moved" error</span></span>

<span data-ttu-id="745b4-127">Si la commande `curl` renvoie une erreur concernant le `-L` paramètre ou un message d’erreur indiquant « Objet déplacé », essayez d’utiliser l’URL complète plutôt que la `aka.ms` redirection :</span><span class="sxs-lookup"><span data-stu-id="745b4-127">If you get an error from `curl` related to the `-L` parameter, or an error message including the text "Object Moved", try using the full URL instead of the `aka.ms` redirect:</span></span>

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

### <a name="az-command-not-found"></a><span data-ttu-id="745b4-128">`az` commande introuvable</span><span class="sxs-lookup"><span data-stu-id="745b4-128">`az` command not found</span></span>

<span data-ttu-id="745b4-129">Si vous ne pouvez pas exécuter la commande après l’installation et après avoir utilisé `bash` et `zsh`, effacez le cache de hachage de commande de votre interpréteur de commandes.</span><span class="sxs-lookup"><span data-stu-id="745b4-129">If you can't run the command after installation and using `bash` or `zsh`, clear your shell's command hash cache.</span></span> <span data-ttu-id="745b4-130">Exécuter</span><span class="sxs-lookup"><span data-stu-id="745b4-130">Run</span></span>

```bash
hash -r
```

<span data-ttu-id="745b4-131">et vérifiez si le problème est résolu.</span><span class="sxs-lookup"><span data-stu-id="745b4-131">and check if the problem is resolved.</span></span>

<span data-ttu-id="745b4-132">Le problème peut également survenir si vous n’avez pas redémarré votre interpréteur de commandes après l’installation.</span><span class="sxs-lookup"><span data-stu-id="745b4-132">The issue can also occur if you didn't restart your shell after installation.</span></span> <span data-ttu-id="745b4-133">Assurez-vous que l’emplacement de la commande `az` se trouve dans votre `$PATH`.</span><span class="sxs-lookup"><span data-stu-id="745b4-133">Make sure that the location of the `az` command is in your `$PATH`.</span></span> <span data-ttu-id="745b4-134">L’emplacement de la commande `az` est</span><span class="sxs-lookup"><span data-stu-id="745b4-134">The location of the `az` command is</span></span>

```bash
<install path>/bin
```

### <a name="proxy-blocks-connection"></a><span data-ttu-id="745b4-135">Le proxy bloque la connexion</span><span class="sxs-lookup"><span data-stu-id="745b4-135">Proxy blocks connection</span></span>

[!INCLUDE[configure-proxy](includes/configure-proxy.md)]

<span data-ttu-id="745b4-136">Pour obtenir les scripts d’installation, votre proxy doit autoriser les connexions HTTPS aux adresses suivantes :</span><span class="sxs-lookup"><span data-stu-id="745b4-136">In order to get the installation scripts, your proxy needs to allow HTTPS connections to the following addresses:</span></span>

* `https://aka.ms/`
* `https://azurecliprod.blob.core.windows.net/`
* `https://pypi.python.org`
* <span data-ttu-id="745b4-137">Points de terminaison utilisés par le gestionnaire de package de votre distribution (le cas échéant) pour les packages de base</span><span class="sxs-lookup"><span data-stu-id="745b4-137">Endpoints used by your distribution's package manager (if any) for core packages</span></span>

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="uninstall"></a><span data-ttu-id="745b4-138">Désinstaller l’interface</span><span class="sxs-lookup"><span data-stu-id="745b4-138">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="745b4-139">Désinstallez l’interface de ligne de commande en supprimant directement les fichiers de l’emplacement spécifié lors de l’installation.</span><span class="sxs-lookup"><span data-stu-id="745b4-139">Uninstall the CLI by directly deleting the files from the location chosen at the time of installation.</span></span> <span data-ttu-id="745b4-140">L’emplacement d’installation par défaut est `$HOME`.</span><span class="sxs-lookup"><span data-stu-id="745b4-140">The default install location is `$HOME`.</span></span>

1. <span data-ttu-id="745b4-141">Supprimez les fichiers CLI installés.</span><span class="sxs-lookup"><span data-stu-id="745b4-141">Remove the installed CLI files.</span></span>

   ```bash
   rm -r <install location>/lib/azure-cli
   rm <install location>/bin/az
   ```

2. <span data-ttu-id="745b4-142">Modifiez votre fichier `$HOME/.bash_profile` pour supprimer la ligne suivante :</span><span class="sxs-lookup"><span data-stu-id="745b4-142">Modify your `$HOME/.bash_profile` file to remove the following line:</span></span>

   ```text
   <install location>/lib/azure-cli/az.completion
   ```

3. <span data-ttu-id="745b4-143">Si vous utilisez `bash` ou `zsh`, rechargez le cache de commande de l’interpréteur de commandes.</span><span class="sxs-lookup"><span data-stu-id="745b4-143">If using `bash` or `zsh`, reload your shell's command cache.</span></span>

   ```bash
   hash -r
   ```

## <a name="next-steps"></a><span data-ttu-id="745b4-144">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="745b4-144">Next Steps</span></span>

<span data-ttu-id="745b4-145">Maintenant que vous avez installé l’interface CLI, découvrez ses fonctionnalités et ses commandes courantes.</span><span class="sxs-lookup"><span data-stu-id="745b4-145">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="745b4-146">Prise en main de l’interface Azure CLI</span><span class="sxs-lookup"><span data-stu-id="745b4-146">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
