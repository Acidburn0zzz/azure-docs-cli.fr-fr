---
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 12/15/2020
ms.topic: include
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: 2cba7031b3fe4c54edcb7c0dcef6f37b97d2f785
ms.sourcegitcommit: d5f026468ea20bbd7ef35bdbf9852bcb2b812d83
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/23/2020
ms.locfileid: "97744613"
---
## <a name="overview"></a><span data-ttu-id="c99a9-101">Vue d’ensemble</span><span class="sxs-lookup"><span data-stu-id="c99a9-101">Overview</span></span>

> [!NOTE]
> <span data-ttu-id="c99a9-102">Il est fortement recommandé d’installer l’interface CLI avec un gestionnaire de package.</span><span class="sxs-lookup"><span data-stu-id="c99a9-102">It's strongly recommend to install the CLI with a package manager.</span></span> <span data-ttu-id="c99a9-103">Un gestionnaire de package permet de s’assurer que vous obtenez toujours les dernières mises à jour et garantit la stabilité des composants de l’interface CLI.</span><span class="sxs-lookup"><span data-stu-id="c99a9-103">A package manager makes sure you always get the latest updates, and guarantees the stability of CLI components.</span></span> <span data-ttu-id="c99a9-104">Vérifiez s’il existe un package pour votre distribution avant d’installer manuellement.</span><span class="sxs-lookup"><span data-stu-id="c99a9-104">Check and see if there is a package for your distribution before installing manually.</span></span>

<span data-ttu-id="c99a9-105">L’interface CLI requiert les logiciels suivants :</span><span class="sxs-lookup"><span data-stu-id="c99a9-105">The CLI requires the following software:</span></span>

* <span data-ttu-id="c99a9-106">[Python 3.6.x, 3.7.x ou 3.8.x](https://www.python.org/downloads/).</span><span class="sxs-lookup"><span data-stu-id="c99a9-106">[Python 3.6.x, 3.7.x or 3.8.x](https://www.python.org/downloads/).</span></span>
* [<span data-ttu-id="c99a9-107">libffi</span><span class="sxs-lookup"><span data-stu-id="c99a9-107">libffi</span></span>](https://sourceware.org/libffi/)
* [<span data-ttu-id="c99a9-108">OpenSSL 1.0.2</span><span class="sxs-lookup"><span data-stu-id="c99a9-108">OpenSSL 1.0.2</span></span>](https://www.openssl.org/source/)

> [!IMPORTANT]
>
> <span data-ttu-id="c99a9-109">L’interface CLI a retiré la prise en charge de Python 2.7 depuis la version `2.1.0`.</span><span class="sxs-lookup"><span data-stu-id="c99a9-109">The CLI has dropped support for Python 2.7 since version `2.1.0`.</span></span> <span data-ttu-id="c99a9-110">Les nouvelles versions ne garantissent plus une exécution correcte de Python 2.7.</span><span class="sxs-lookup"><span data-stu-id="c99a9-110">New versions no longer guarantee to run with Python 2.7 correctly.</span></span>

## <a name="install-or-update"></a><span data-ttu-id="c99a9-111">Installation ou mise à jour</span><span class="sxs-lookup"><span data-stu-id="c99a9-111">Install or update</span></span>

<span data-ttu-id="c99a9-112">L’installation et la mise à jour de l’interface CLI nécessitent toutes de réexécuter le script d’installation.</span><span class="sxs-lookup"><span data-stu-id="c99a9-112">Both installing and updating the CLI requires re-running the install script.</span></span> <span data-ttu-id="c99a9-113">Installez l’interface CLI en exécutant `curl`.</span><span class="sxs-lookup"><span data-stu-id="c99a9-113">Install the CLI by running `curl`.</span></span>

```bash
curl -L https://aka.ms/InstallAzureCli | bash
```

<span data-ttu-id="c99a9-114">Le script peut également être téléchargé et exécuté localement.</span><span class="sxs-lookup"><span data-stu-id="c99a9-114">The script can also be downloaded and run locally.</span></span> <span data-ttu-id="c99a9-115">Vous devrez peut-être redémarrer votre interpréteur de commandes pour que certaines modifications soient prises en compte.</span><span class="sxs-lookup"><span data-stu-id="c99a9-115">You may have to restart your shell in order for changes to take effect.</span></span>

<span data-ttu-id="c99a9-116">Vous pouvez ensuite exécuter l’interface de ligne de commande Azure avec la commande `az`.</span><span class="sxs-lookup"><span data-stu-id="c99a9-116">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="c99a9-117">Pour vous connecter, utilisez la commande [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="c99a9-117">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](interactive-login.md)]

<span data-ttu-id="c99a9-118">Pour en savoir plus sur les différentes méthodes d’authentification, consultez [Se connecter avec Azure CLI](../authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="c99a9-118">To learn more about different authentication methods, see [Sign in with Azure CLI](../authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="c99a9-119">Dépannage</span><span class="sxs-lookup"><span data-stu-id="c99a9-119">Troubleshooting</span></span>

<span data-ttu-id="c99a9-120">Voici certains problèmes courants rencontrés pendant une installation manuelle.</span><span class="sxs-lookup"><span data-stu-id="c99a9-120">Here are some common problems seen during a manual installation.</span></span> <span data-ttu-id="c99a9-121">Si vous rencontrez un problème qui n’est pas traité ici, [signalez ce problème sur GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="c99a9-121">If you experience a problem not covered here, [file an issue on GitHub](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="curl-object-moved-error"></a><span data-ttu-id="c99a9-122">erreur curl « Objet déplacé »</span><span class="sxs-lookup"><span data-stu-id="c99a9-122">curl "Object Moved" error</span></span>

<span data-ttu-id="c99a9-123">Si la commande `curl` renvoie une erreur concernant le `-L` paramètre ou un message d’erreur indiquant « Objet déplacé », essayez d’utiliser l’URL complète plutôt que la `aka.ms` redirection :</span><span class="sxs-lookup"><span data-stu-id="c99a9-123">If you get an error from `curl` related to the `-L` parameter, or an error message including the text "Object Moved", try using the full URL instead of the `aka.ms` redirect:</span></span>

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

### <a name="az-command-not-found"></a><span data-ttu-id="c99a9-124">`az` commande introuvable</span><span class="sxs-lookup"><span data-stu-id="c99a9-124">`az` command not found</span></span>

<span data-ttu-id="c99a9-125">Si vous ne pouvez pas exécuter la commande après l’installation et après avoir utilisé `bash` et `zsh`, effacez le cache de hachage de commande de votre interpréteur de commandes.</span><span class="sxs-lookup"><span data-stu-id="c99a9-125">If you can't run the command after installation and using `bash` or `zsh`, clear your shell's command hash cache.</span></span> <span data-ttu-id="c99a9-126">Exécuter</span><span class="sxs-lookup"><span data-stu-id="c99a9-126">Run</span></span>

```bash
hash -r
```

<span data-ttu-id="c99a9-127">et vérifiez si le problème est résolu.</span><span class="sxs-lookup"><span data-stu-id="c99a9-127">and check if the problem is resolved.</span></span>

<span data-ttu-id="c99a9-128">Le problème peut également survenir si vous n’avez pas redémarré votre interpréteur de commandes après l’installation.</span><span class="sxs-lookup"><span data-stu-id="c99a9-128">The issue can also occur if you didn't restart your shell after installation.</span></span> <span data-ttu-id="c99a9-129">Assurez-vous que l’emplacement de la commande `az` se trouve dans votre `$PATH`.</span><span class="sxs-lookup"><span data-stu-id="c99a9-129">Make sure that the location of the `az` command is in your `$PATH`.</span></span> <span data-ttu-id="c99a9-130">L’emplacement de la commande `az` est</span><span class="sxs-lookup"><span data-stu-id="c99a9-130">The location of the `az` command is</span></span>

```bash
<install path>/bin
```

### <a name="proxy-blocks-connection"></a><span data-ttu-id="c99a9-131">Le proxy bloque la connexion</span><span class="sxs-lookup"><span data-stu-id="c99a9-131">Proxy blocks connection</span></span>

[!INCLUDE[configure-proxy](configure-proxy.md)]

<span data-ttu-id="c99a9-132">Pour obtenir les scripts d’installation, votre proxy doit autoriser les connexions HTTPS aux adresses suivantes :</span><span class="sxs-lookup"><span data-stu-id="c99a9-132">In order to get the installation scripts, your proxy needs to allow HTTPS connections to the following addresses:</span></span>

* `https://aka.ms/`
* `https://azurecliprod.blob.core.windows.net/`
* `https://pypi.python.org`
* <span data-ttu-id="c99a9-133">Points de terminaison utilisés par le gestionnaire de package de votre distribution (le cas échéant) pour les packages de base</span><span class="sxs-lookup"><span data-stu-id="c99a9-133">Endpoints used by your distribution's package manager (if any) for core packages</span></span>

[!INCLUDE[troubleshoot-wsl.md](troubleshoot-wsl.md)]

## <a name="uninstall"></a><span data-ttu-id="c99a9-134">Désinstaller</span><span class="sxs-lookup"><span data-stu-id="c99a9-134">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](uninstall-boilerplate.md)]

<span data-ttu-id="c99a9-135">Désinstallez l’interface de ligne de commande en supprimant directement les fichiers de l’emplacement spécifié lors de l’installation.</span><span class="sxs-lookup"><span data-stu-id="c99a9-135">Uninstall the CLI by directly deleting the files from the location chosen at the time of installation.</span></span> <span data-ttu-id="c99a9-136">L’emplacement d’installation par défaut est `$HOME`.</span><span class="sxs-lookup"><span data-stu-id="c99a9-136">The default install location is `$HOME`.</span></span>

1. <span data-ttu-id="c99a9-137">Supprimez les fichiers CLI installés.</span><span class="sxs-lookup"><span data-stu-id="c99a9-137">Remove the installed CLI files.</span></span>

   ```bash
   rm -r <install location>/lib/azure-cli
   rm <install location>/bin/az
   ```

2. <span data-ttu-id="c99a9-138">Modifiez votre fichier `$HOME/.bash_profile` pour supprimer la ligne suivante :</span><span class="sxs-lookup"><span data-stu-id="c99a9-138">Modify your `$HOME/.bash_profile` file to remove the following line:</span></span>

   ```text
   <install location>/lib/azure-cli/az.completion
   ```

3. <span data-ttu-id="c99a9-139">Si vous utilisez `bash` ou `zsh`, rechargez le cache de commande de l’interpréteur de commandes.</span><span class="sxs-lookup"><span data-stu-id="c99a9-139">If using `bash` or `zsh`, reload your shell's command cache.</span></span>

   ```bash
   hash -r
   ```