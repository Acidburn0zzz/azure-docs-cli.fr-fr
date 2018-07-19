---
title: Installer manuellement Azure CLI 2.0 pour Linux
description: Installation manuelle d’Azure CLI 2.0 pour Linux
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 01/29/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 7e73ae8bbbba80bf48c6f01fc1c37a3c32c6eb31
ms.sourcegitcommit: 64f2c628e83d687d0e172c01f13d71c8c39a8040
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/11/2018
ms.locfileid: "38967552"
---
# <a name="install-azure-cli-20-on-linux-manually"></a><span data-ttu-id="5c9ce-103">Installer manuellement Azure CLI 2.0 sur Linux</span><span class="sxs-lookup"><span data-stu-id="5c9ce-103">Install Azure CLI 2.0 on Linux manually</span></span>

<span data-ttu-id="5c9ce-104">Si vous n’avez pas de package disponible sur votre distribution pour l’interface de ligne de commande Azure, vous pouvez toujours installer l’interface de ligne de commande manuellement en exécutant un script d’installation.</span><span class="sxs-lookup"><span data-stu-id="5c9ce-104">If you do not have a package for the Azure CLI available on your distribution, you can always install the CLI manually by running an installation script.</span></span>

> [!NOTE]
> <span data-ttu-id="5c9ce-105">Il est fortement recommandé d’utiliser un gestionnaire de package pour l’interface CLI.</span><span class="sxs-lookup"><span data-stu-id="5c9ce-105">It's strongly recommend that you use a package manager for the CLI.</span></span> <span data-ttu-id="5c9ce-106">Un gestionnaire de package permet de s’assurer que vous obtenez toujours les dernières mises à jour et garantit la stabilité des composants de l’interface CLI.</span><span class="sxs-lookup"><span data-stu-id="5c9ce-106">A package manager makes sure you always get the latest updates, and guarantees the stability of CLI components.</span></span> <span data-ttu-id="5c9ce-107">Vérifiez s’il existe un package pour votre distribution avant d’installer manuellement.</span><span class="sxs-lookup"><span data-stu-id="5c9ce-107">Check and see if there is a package for your distribution before installing manually.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5c9ce-108">Prérequis</span><span class="sxs-lookup"><span data-stu-id="5c9ce-108">Prerequisites</span></span>

<span data-ttu-id="5c9ce-109">Pour installer l’interface de ligne de commande, vous avez besoin des logiciels suivants sur votre système :</span><span class="sxs-lookup"><span data-stu-id="5c9ce-109">In order to install the CLI, you need the following software available on your system:</span></span>

* [<span data-ttu-id="5c9ce-110">Python 2.7 ou Python 3.x</span><span class="sxs-lookup"><span data-stu-id="5c9ce-110">Python 2.7 or Python 3.x</span></span>](https://www.python.org/downloads/)
* [<span data-ttu-id="5c9ce-111">libffi</span><span class="sxs-lookup"><span data-stu-id="5c9ce-111">libffi</span></span>](https://sourceware.org/libffi/)
* [<span data-ttu-id="5c9ce-112">OpenSSL 1.0.2</span><span class="sxs-lookup"><span data-stu-id="5c9ce-112">OpenSSL 1.0.2</span></span>](https://www.openssl.org/source/)

## <a name="install-or-update"></a><span data-ttu-id="5c9ce-113">Installation ou mise à jour</span><span class="sxs-lookup"><span data-stu-id="5c9ce-113">Install or update</span></span>

<span data-ttu-id="5c9ce-114">Que vous installiez ou que vous mettiez à jour l’interface de ligne de commande, vous devez effectuer une installation complète.</span><span class="sxs-lookup"><span data-stu-id="5c9ce-114">Whether you are installing or updating the CLI, you need to perform a full installation.</span></span> <span data-ttu-id="5c9ce-115">Une fois que vous disposez de la configuration requise, vous pouvez installer l’interface de ligne de commande en exécutant `curl`.</span><span class="sxs-lookup"><span data-stu-id="5c9ce-115">Once you have the prerequisites, you can install the CLI by running `curl`.</span></span>

```bash
curl -L https://aka.ms/InstallAzureCli | bash
```

<span data-ttu-id="5c9ce-116">Au lieu de cela, vous pouvez également télécharger le script et l’exécuter localement.</span><span class="sxs-lookup"><span data-stu-id="5c9ce-116">You can also download the script and run it locally instead.</span></span> <span data-ttu-id="5c9ce-117">Vous devrez peut-être redémarrer votre interpréteur de commandes pour que certaines modifications soient prises en compte.</span><span class="sxs-lookup"><span data-stu-id="5c9ce-117">You may have to restart your shell in order for changes to take effect.</span></span>

<span data-ttu-id="5c9ce-118">Vous pouvez ensuite exécuter l’interface de ligne de commande Azure avec la commande `az`.</span><span class="sxs-lookup"><span data-stu-id="5c9ce-118">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="5c9ce-119">Pour vous connecter, utilisez la commande [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="5c9ce-119">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="5c9ce-120">Pour en savoir plus sur les différentes méthodes d’authentification, consultez [Se connecter avec Azure CLI 2.0](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="5c9ce-120">To learn more about different authentication methods, see [Sign in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="5c9ce-121">Résolution de problèmes</span><span class="sxs-lookup"><span data-stu-id="5c9ce-121">Troubleshooting</span></span>

<span data-ttu-id="5c9ce-122">Voici certains problèmes courants rencontrés pendant une installation manuelle.</span><span class="sxs-lookup"><span data-stu-id="5c9ce-122">Here are some common problems seen during a manual installation.</span></span> <span data-ttu-id="5c9ce-123">Si votre problème ne figure pas ici, veuillez [signaler le problème sur Github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="5c9ce-123">If your issue is not listed here, please [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="curl-object-moved-error"></a><span data-ttu-id="5c9ce-124">erreur curl « Objet déplacé »</span><span class="sxs-lookup"><span data-stu-id="5c9ce-124">curl "Object Moved" error</span></span>

<span data-ttu-id="5c9ce-125">Si la commande `curl` renvoie une erreur concernant le `-L` paramètre ou un message d’erreur indiquant « Objet déplacé », essayez d’utiliser l’URL complète plutôt que la `aka.ms` redirection :</span><span class="sxs-lookup"><span data-stu-id="5c9ce-125">If you get an error from `curl` related to the `-L` parameter, or an error message including the text "Object Moved", try using the full URL instead of the `aka.ms` redirect:</span></span>

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

### <a name="az-command-not-found"></a><span data-ttu-id="5c9ce-126">`az` commande introuvable</span><span class="sxs-lookup"><span data-stu-id="5c9ce-126">`az` command not found</span></span>

<span data-ttu-id="5c9ce-127">Si vous ne pouvez pas exécuter la commande après l’installation et après avoir utilisé `bash` et `zsh`, effacez le cache de hachage de commande de votre interpréteur de commandes.</span><span class="sxs-lookup"><span data-stu-id="5c9ce-127">If you can't run the command after installation and using `bash` or `zsh`, clear your shell's command hash cache.</span></span> <span data-ttu-id="5c9ce-128">Exécuter</span><span class="sxs-lookup"><span data-stu-id="5c9ce-128">Run</span></span>

```bash
hash -r
```

<span data-ttu-id="5c9ce-129">et vérifiez si le problème est résolu.</span><span class="sxs-lookup"><span data-stu-id="5c9ce-129">and check if the problem is resolved.</span></span>

<span data-ttu-id="5c9ce-130">Le problème peut également se produire si vous n’avez pas redémarré votre interpréteur de commandes après l’installation.</span><span class="sxs-lookup"><span data-stu-id="5c9ce-130">The issue can also occur if you did not restart your shell after installation.</span></span> <span data-ttu-id="5c9ce-131">Assurez-vous que l’emplacement de la commande `az` se trouve dans votre `$PATH`.</span><span class="sxs-lookup"><span data-stu-id="5c9ce-131">Make sure that the location of the `az` command is in your `$PATH`.</span></span> <span data-ttu-id="5c9ce-132">L’emplacement de la commande `az` est</span><span class="sxs-lookup"><span data-stu-id="5c9ce-132">The location of the `az` command is</span></span>

```bash
<install path>/bin
```

## <a name="uninstall"></a><span data-ttu-id="5c9ce-133">Désinstaller l’interface</span><span class="sxs-lookup"><span data-stu-id="5c9ce-133">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="5c9ce-134">Désinstallez l’interface de ligne de commande en supprimant directement les fichiers de l’emplacement spécifié lors de l’installation.</span><span class="sxs-lookup"><span data-stu-id="5c9ce-134">Uninstall the CLI by directly deleting the files from the location chosen at the time of installation.</span></span> <span data-ttu-id="5c9ce-135">L’emplacement d’installation par défaut est `$HOME`.</span><span class="sxs-lookup"><span data-stu-id="5c9ce-135">The default install location is `$HOME`.</span></span>

1. <span data-ttu-id="5c9ce-136">Supprimez les fichiers CLI installés.</span><span class="sxs-lookup"><span data-stu-id="5c9ce-136">Remove the installed CLI files.</span></span>

  ```bash
  rm -r <install location>/lib/azure-cli
  rm <install location>/bin/az
  ```

2. <span data-ttu-id="5c9ce-137">Modifiez votre fichier `$HOME/.bash_profile` pour supprimer la ligne suivante :</span><span class="sxs-lookup"><span data-stu-id="5c9ce-137">Modify your `$HOME/.bash_profile` file to remove the following line:</span></span>

  ```text
  <install location>/lib/azure-cli/az.completion
  ```

3. <span data-ttu-id="5c9ce-138">Si vous utilisez `bash` ou `zsh`, rechargez le cache de commande de l’interpréteur de commandes.</span><span class="sxs-lookup"><span data-stu-id="5c9ce-138">If using `bash` or `zsh`, reload your shell's command cache.</span></span>

  ```bash
  hash -r
  ```
