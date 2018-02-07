---
title: Installer manuellement Azure CLI 2.0 pour Linux
description: "Installation manuelle d’Azure CLI 2.0 pour Linux"
keywords: "Azure CLI, Installation d’Azure CLI, Azure Linux, installation Azure Linux"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 01/29/18
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: d8c88d111c50a3cbb6b643a14dcd2a9773699657
ms.sourcegitcommit: 8606f36963e8daa6448d637393d1e4ef2c9859a0
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/01/2018
---
# <a name="install-azure-cli-20-on-linux-manually"></a><span data-ttu-id="f4534-104">Installer manuellement Azure CLI 2.0 sur Linux</span><span class="sxs-lookup"><span data-stu-id="f4534-104">Install Azure CLI 2.0 on Linux manually</span></span>

<span data-ttu-id="f4534-105">Si vous n’avez pas de package disponible sur votre distribution pour l’interface de ligne de commande Azure, vous pouvez toujours installer l’interface de ligne de commande manuellement en exécutant un script d’installation.</span><span class="sxs-lookup"><span data-stu-id="f4534-105">If you do not have a package for the Azure CLI available on your distribution, you can always install the CLI manually by running an installation script.</span></span>

> [!NOTE]
> <span data-ttu-id="f4534-106">Il est fortement recommandé d’utiliser un gestionnaire de package pour l’interface CLI.</span><span class="sxs-lookup"><span data-stu-id="f4534-106">It's strongly recommend that you use a package manager for the CLI.</span></span> <span data-ttu-id="f4534-107">Un gestionnaire de package permet de s’assurer que vous obtenez toujours les dernières mises à jour et garantit la stabilité des composants de l’interface CLI.</span><span class="sxs-lookup"><span data-stu-id="f4534-107">A package manager makes sure you always get the latest updates, and guarantees the stability of CLI components.</span></span> <span data-ttu-id="f4534-108">Vérifiez s’il existe un package pour votre distribution avant d’installer manuellement.</span><span class="sxs-lookup"><span data-stu-id="f4534-108">Check and see if there is a package for your distribution before installing manually.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f4534-109">configuration requise</span><span class="sxs-lookup"><span data-stu-id="f4534-109">Prerequisites</span></span>

<span data-ttu-id="f4534-110">Pour installer l’interface de ligne de commande, vous avez besoin des logiciels suivants sur votre système :</span><span class="sxs-lookup"><span data-stu-id="f4534-110">In order to install the CLI, you need the following software available on your system:</span></span>

* [<span data-ttu-id="f4534-111">Python 2.7 ou Python 3.x</span><span class="sxs-lookup"><span data-stu-id="f4534-111">Python 2.7 or Python 3.x</span></span>](https://www.python.org/downloads/)
* [<span data-ttu-id="f4534-112">libffi</span><span class="sxs-lookup"><span data-stu-id="f4534-112">libffi</span></span>](https://sourceware.org/libffi/)
* [<span data-ttu-id="f4534-113">OpenSSL 1.0.2</span><span class="sxs-lookup"><span data-stu-id="f4534-113">OpenSSL 1.0.2</span></span>](https://www.openssl.org/source/)

## <a name="install-or-update"></a><span data-ttu-id="f4534-114">Installation ou mise à jour</span><span class="sxs-lookup"><span data-stu-id="f4534-114">Install or update</span></span> 

<span data-ttu-id="f4534-115">Que vous installiez ou que vous mettiez à jour l’interface de ligne de commande, vous devez effectuer une installation complète.</span><span class="sxs-lookup"><span data-stu-id="f4534-115">Whether you are installing or updating the CLI, you need to perform a full installation.</span></span> <span data-ttu-id="f4534-116">Une fois que vous disposez de la configuration requise, vous pouvez installer l’interface de ligne de commande en exécutant `curl`.</span><span class="sxs-lookup"><span data-stu-id="f4534-116">Once you have the prerequisites, you can install the CLI by running `curl`.</span></span>

```bash
curl -L https://aka.ms/InstallAzureCli | bash
```

<span data-ttu-id="f4534-117">Au lieu de cela, vous pouvez également télécharger le script et l’exécuter localement.</span><span class="sxs-lookup"><span data-stu-id="f4534-117">You can also download the script and run it locally instead.</span></span> <span data-ttu-id="f4534-118">Vous devrez peut-être redémarrer votre interpréteur de commandes pour que certaines modifications soient prises en compte.</span><span class="sxs-lookup"><span data-stu-id="f4534-118">You may have to restart your shell in order for changes to take effect.</span></span> <span data-ttu-id="f4534-119">Après l’installation, exécutez l’interface de ligne de commande avec la commande `az`.</span><span class="sxs-lookup"><span data-stu-id="f4534-119">After installation, run the CLI with the `az` command.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="f4534-120">Résolution de problèmes</span><span class="sxs-lookup"><span data-stu-id="f4534-120">Troubleshooting</span></span>

<span data-ttu-id="f4534-121">Voici certains problèmes courants rencontrés pendant une installation manuelle.</span><span class="sxs-lookup"><span data-stu-id="f4534-121">Here are some common problems seen during a manual installation.</span></span> <span data-ttu-id="f4534-122">Si votre problème ne figure pas ici, veuillez [signaler le problème sur Github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="f4534-122">If your issue is not listed here, please [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>
### <a name="curl-object-moved-error"></a><span data-ttu-id="f4534-123">erreur curl « Objet déplacé »</span><span class="sxs-lookup"><span data-stu-id="f4534-123">curl "Object Moved" error</span></span>

<span data-ttu-id="f4534-124">Si la commande `curl` renvoie une erreur concernant le `-L` paramètre ou un message d’erreur indiquant « Objet déplacé », essayez d’utiliser l’URL complète plutôt que la `aka.ms` redirection :</span><span class="sxs-lookup"><span data-stu-id="f4534-124">If you get an error from `curl` related to the `-L` parameter, or an error message including the text "Object Moved", try using the full URL instead of the `aka.ms` redirect:</span></span>

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

### <a name="az-command-not-found"></a><span data-ttu-id="f4534-125">`az` commande introuvable</span><span class="sxs-lookup"><span data-stu-id="f4534-125">`az` command not found</span></span>

<span data-ttu-id="f4534-126">Si vous ne pouvez pas exécuter la commande après l’installation et après avoir utilisé `bash` et `zsh`, effacez le cache de hachage de commande de votre interpréteur de commandes.</span><span class="sxs-lookup"><span data-stu-id="f4534-126">If you can't run the command after installation and using `bash` or `zsh`, clear your shell's command hash cache.</span></span> <span data-ttu-id="f4534-127">Exécuter</span><span class="sxs-lookup"><span data-stu-id="f4534-127">Run</span></span>

```bash
hash -r
```

<span data-ttu-id="f4534-128">et vérifiez si le problème est résolu.</span><span class="sxs-lookup"><span data-stu-id="f4534-128">and check if the problem is resolved.</span></span>

<span data-ttu-id="f4534-129">Le problème peut également se produire si vous n’avez pas redémarré votre interpréteur de commandes après l’installation.</span><span class="sxs-lookup"><span data-stu-id="f4534-129">The issue can also occur if you did not restart your shell after installation.</span></span> <span data-ttu-id="f4534-130">Assurez-vous que l’emplacement de la commande `az` se trouve dans votre `$PATH`.</span><span class="sxs-lookup"><span data-stu-id="f4534-130">Make sure that the location of the `az` command is in your `$PATH`.</span></span> <span data-ttu-id="f4534-131">L’emplacement de la commande `az` est</span><span class="sxs-lookup"><span data-stu-id="f4534-131">The location of the `az` command is</span></span>

```bash
<install path>/bin
```

## <a name="uninstall"></a><span data-ttu-id="f4534-132">Désinstaller l’interface</span><span class="sxs-lookup"><span data-stu-id="f4534-132">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="f4534-133">Désinstallez l’interface de ligne de commande en supprimant directement les fichiers de l’emplacement spécifié lors de l’installation.</span><span class="sxs-lookup"><span data-stu-id="f4534-133">Uninstall the CLI by directly deleting the files from the location chosen at the time of installation.</span></span> <span data-ttu-id="f4534-134">L’emplacement d’installation par défaut est `$HOME`.</span><span class="sxs-lookup"><span data-stu-id="f4534-134">The default install location is `$HOME`.</span></span>

1. <span data-ttu-id="f4534-135">Supprimez les fichiers CLI installés.</span><span class="sxs-lookup"><span data-stu-id="f4534-135">Remove the installed CLI files.</span></span>
  
  ```bash
  rm -r <install location>/lib/azure-cli
  rm <install location>/bin/az
  ```
2. <span data-ttu-id="f4534-136">Modifiez votre fichier `$HOME/.bash_profile` pour supprimer la ligne suivante :</span><span class="sxs-lookup"><span data-stu-id="f4534-136">Modify your `$HOME/.bash_profile` file to remove the following line:</span></span>
  
  ```
  <install location>/lib/azure-cli/az.completion
  ```

3. <span data-ttu-id="f4534-137">Si vous utilisez `bash` ou `zsh`, rechargez le cache de commande de l’interpréteur de commandes.</span><span class="sxs-lookup"><span data-stu-id="f4534-137">If using `bash` or `zsh`, reload your shell's command cache.</span></span>
  
  ```bash
  hash -r
  ```
