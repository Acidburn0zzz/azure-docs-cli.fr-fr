---
title: Installer manuellement Azure CLI 2.0 pour Linux
description: "Installation manuelle d’Azure CLI 2.0 pour Linux"
keywords: "Azure CLI, Installation d’Azure CLI, Azure Linux, installation Azure Linux"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 11/01/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ROBOTS: NOINDEX,NOFOLLOW
ms.openlocfilehash: f792d3fc84eedade52ddfb3f351e48689e474d53
ms.sourcegitcommit: 905939cc44764b4d1cc79a9b36c0793f7055a686
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/20/2017
---
# <a name="install-azure-cli-20-on-linux-manually"></a><span data-ttu-id="acd9f-104">Installer manuellement Azure CLI 2.0 sur Linux</span><span class="sxs-lookup"><span data-stu-id="acd9f-104">Install Azure CLI 2.0 on Linux manually</span></span>

<span data-ttu-id="acd9f-105">Si vous n’avez pas de package disponible sur votre distribution pour l’interface de ligne de commande Azure, vous pouvez toujours installer l’interface de ligne de commande manuellement en exécutant un script d’installation.</span><span class="sxs-lookup"><span data-stu-id="acd9f-105">If you do not have a package for the Azure CLI available on your distribution, you can always install the CLI manualy by running an installation script.</span></span> <span data-ttu-id="acd9f-106">Si vous disposez d’un package disponible, il s’agit toujours de la méthode d’installation recommandée.</span><span class="sxs-lookup"><span data-stu-id="acd9f-106">If you do have a package available, that is always the recommended installation method.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="acd9f-107">Composants requis</span><span class="sxs-lookup"><span data-stu-id="acd9f-107">Prerequisites</span></span>

<span data-ttu-id="acd9f-108">Pour installer l’interface de ligne de commande, vous devrez disposer des logiciels suivants sur votre système :</span><span class="sxs-lookup"><span data-stu-id="acd9f-108">In order to install the CLI, you will need the following software available on your system:</span></span>

* [<span data-ttu-id="acd9f-109">Python 2.7 ou Python 3.x</span><span class="sxs-lookup"><span data-stu-id="acd9f-109">Python 2.7 or Python 3.x</span></span>](https://www.python.org/downloads/)
* [<span data-ttu-id="acd9f-110">libffi</span><span class="sxs-lookup"><span data-stu-id="acd9f-110">libffi</span></span>](https://sourceware.org/libffi/)
* [<span data-ttu-id="acd9f-111">OpenSSL</span><span class="sxs-lookup"><span data-stu-id="acd9f-111">OpenSSL</span></span>](https://www.openssl.org/source/)

## <a name="install-or-update-manually"></a><span data-ttu-id="acd9f-112">Installation ou mise à jour manuelle</span><span class="sxs-lookup"><span data-stu-id="acd9f-112">Install or update manually</span></span>

<span data-ttu-id="acd9f-113">Que vous installiez ou que vous mettiez à jour l’interface de ligne de commande, vous devrez effectuer une installation complète.</span><span class="sxs-lookup"><span data-stu-id="acd9f-113">Whether you are installing or updating the CLI, you will need to perform a full installation.</span></span> <span data-ttu-id="acd9f-114">Une fois que vous disposez de la configuration requise, vous pouvez installer l’interface de ligne de commande en exécutant `curl`.</span><span class="sxs-lookup"><span data-stu-id="acd9f-114">Once you have the prerequisites, you can install the CLI by running `curl`.</span></span>

```bash
curl -L https://aka.ms/InstallAzureCli | bash
```

<span data-ttu-id="acd9f-115">Si vous préférez, ou si vous n’avez pas `curl` sur votre système, vous pouvez télécharger le script et l’exécuter localement à la place.</span><span class="sxs-lookup"><span data-stu-id="acd9f-115">If you would prefer, or do not have `curl` on your system, you can download the script and run it locally instead.</span></span> <span data-ttu-id="acd9f-116">Vous devrez peut-être redémarrer votre interpréteur de commandes pour que certaines modifications soient prises en compte.</span><span class="sxs-lookup"><span data-stu-id="acd9f-116">You may have to restart your shell in order for changes to take effect.</span></span> <span data-ttu-id="acd9f-117">Après l’installation, exécutez l’interface de ligne de commande avec la commande `az`.</span><span class="sxs-lookup"><span data-stu-id="acd9f-117">After installation, run the CLI with the `az` command.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="acd9f-118">Résolution des problèmes</span><span class="sxs-lookup"><span data-stu-id="acd9f-118">Troubleshooting</span></span>

### <a name="curl-object-moved-error"></a><span data-ttu-id="acd9f-119">erreur curl « Objet déplacé »</span><span class="sxs-lookup"><span data-stu-id="acd9f-119">curl "Object Moved" error</span></span>

<span data-ttu-id="acd9f-120">Si la commande `curl` renvoie une erreur concernant le `-L` paramètre ou un message d’erreur indiquant « Objet déplacé », essayez d’utiliser l’URL complète plutôt que la `aka.ms` redirection :</span><span class="sxs-lookup"><span data-stu-id="acd9f-120">If you get an error from `curl` related to the `-L` parameter, or an error message including the text "Object Moved", try using the full URL instead of the `aka.ms` redirect:</span></span>

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

### <a name="az-command-not-found"></a><span data-ttu-id="acd9f-121">`az` commande introuvable</span><span class="sxs-lookup"><span data-stu-id="acd9f-121">`az` command not found</span></span>

<span data-ttu-id="acd9f-122">Après l’installation, si vous ne pouvez pas exécuter la commande, vous devrez peut-être effacer le cache de hachage de commande de l’interpréteur de commandes.</span><span class="sxs-lookup"><span data-stu-id="acd9f-122">After installation if you can't run the command, you may need to clear your shell's command hash cache.</span></span> <span data-ttu-id="acd9f-123">Exécuter</span><span class="sxs-lookup"><span data-stu-id="acd9f-123">Run</span></span>

```bash
hash -r
```

<span data-ttu-id="acd9f-124">et vérifier si le problème est résolu.</span><span class="sxs-lookup"><span data-stu-id="acd9f-124">and see if the problem is resolved.</span></span> 

<span data-ttu-id="acd9f-125">Cela peut également se produire si vous n’avez pas redémarré votre interpréteur de commandes après l’installation.</span><span class="sxs-lookup"><span data-stu-id="acd9f-125">This can also occur if you did not restart your shell after installation.</span></span> <span data-ttu-id="acd9f-126">Assurez-vous que l’emplacement de la commande `az` se trouve dans votre `$PATH`.</span><span class="sxs-lookup"><span data-stu-id="acd9f-126">Make sure that the location of the `az` command is in your `$PATH`.</span></span>

<span data-ttu-id="acd9f-127">Si vous avez exécuté le script d’installation, il s’agira de :</span><span class="sxs-lookup"><span data-stu-id="acd9f-127">If you ran the installation script, this will be:</span></span>

```bash
<install path>/bin
```

## <a name="unstinall-manually"></a><span data-ttu-id="acd9f-128">Désinstaller manuellement</span><span class="sxs-lookup"><span data-stu-id="acd9f-128">Unstinall manually</span></span>

<span data-ttu-id="acd9f-129">Si jamais vous décidez de désinstaller l’interface de ligne de commande Azure, nous sommes désolés de vous voir partir.</span><span class="sxs-lookup"><span data-stu-id="acd9f-129">If you ever decide to uninstall the Azure CLI, we're sorry to see you go.</span></span> <span data-ttu-id="acd9f-130">Avant de désinstaller, utilisez la commande `az feedback`, afin de nous donner quelques raisons pour lesquelles vous avez choisi de désinstaller et nous aider à améliorer l’expérience CLI.</span><span class="sxs-lookup"><span data-stu-id="acd9f-130">Before you uninstall, use the `az feedback` command to give us some reasons why you chose to uninstall and how we could improve the CLI experience.</span></span> <span data-ttu-id="acd9f-131">Nous souhaitons nous assurer que l’interface de ligne de commande Azure est aussi conviviale et exempte de bogues que possible.</span><span class="sxs-lookup"><span data-stu-id="acd9f-131">We want to make sure that the Azure CLI is as bug-free and user-friendly as we can make it.</span></span> <span data-ttu-id="acd9f-132">Vous pouvez également [signaler un problème lié à GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="acd9f-132">You can also [file a github issue](https://github.com/Azure/azure-cli/issues).</span></span>

<span data-ttu-id="acd9f-133">Vous pouvez désinstaller l’interface de ligne de commande en supprimant directement les fichiers de l’emplacement d’installation.</span><span class="sxs-lookup"><span data-stu-id="acd9f-133">You can uninstall the CLI by directly deleting the files from the install location.</span></span> <span data-ttu-id="acd9f-134">Votre emplacement d’installation doit être spécifié au moment de l’installation, si vous avez installé via le script `https://aka.ms/InstallAzureCLI`.</span><span class="sxs-lookup"><span data-stu-id="acd9f-134">Your install location should have been chosen at the time of install, if you installed via the `https://aka.ms/InstallAzureCLI` script.</span></span> <span data-ttu-id="acd9f-135">L’emplacement d’installation par défaut est `$HOME`.</span><span class="sxs-lookup"><span data-stu-id="acd9f-135">The default installation location is `$HOME`.</span></span>

<span data-ttu-id="acd9f-136">Tout d’abord, supprimez les fichiers CLI installés :</span><span class="sxs-lookup"><span data-stu-id="acd9f-136">First, remove the installed CLI files:</span></span>

```bash
rm -r <install location>/lib/azure-cli
rm <install location>/bin/az
```

<span data-ttu-id="acd9f-137">Modifiez ensuite votre fichier `$HOME/.bash_profile` pour supprimer la ligne :</span><span class="sxs-lookup"><span data-stu-id="acd9f-137">Then modify your `$HOME/.bash_profile` file to remove the line:</span></span>

```
<install location>/lib/azure-cli/az.completion
```

<span data-ttu-id="acd9f-138">Enfin, rechargez le cache de commande de l’interpréteur de commandes s’il en utilise un.</span><span class="sxs-lookup"><span data-stu-id="acd9f-138">And finally, reload your shell's command cache if it uses one.</span></span> <span data-ttu-id="acd9f-139">Les utilisateurs `bash`et `zsh` devront effectuer cette étape :</span><span class="sxs-lookup"><span data-stu-id="acd9f-139">`bash` and `zsh` users will need to perform this step:</span></span>

```bash
hash -r
```
