---
title: "Installer l’interface de ligne de commande Azure pour macOS"
description: "Installation d’Azure CLI 2.0 sur macOS"
keywords: "Azure CLI, Installation d’Azure CLI, Azure macOS, installation Azure macOS"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 10/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ROBOTS: NOINDEX,NOFOLLOW
ms.openlocfilehash: e615d2b3ab3b1307e982cb1d4d456633440afdf6
ms.sourcegitcommit: 905939cc44764b4d1cc79a9b36c0793f7055a686
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/20/2017
---
# <a name="install-azure-cli-20-on-macos"></a><span data-ttu-id="b18b3-104">Installation d’Azure CLI 2.0 sur macOS</span><span class="sxs-lookup"><span data-stu-id="b18b3-104">Install Azure CLI 2.0 on macOS</span></span>

<span data-ttu-id="b18b3-105">Pour la plateforme macOS, vous pouvez installer l’interface de ligne de commande Azure via le [Gestionnaire de package Homebrew](http://brew.sh) ou manuellement.</span><span class="sxs-lookup"><span data-stu-id="b18b3-105">For the macOS platform, you can install the Azure CLI either through the [homebrew package manager](http://brew.sh) or manually.</span></span> <span data-ttu-id="b18b3-106">La méthode d’installation par défaut est via Homebrew, afin de faciliter l’installation, obtenez les mises à jour et désinstallez si besoin.</span><span class="sxs-lookup"><span data-stu-id="b18b3-106">The preferred installation method is through homebrew, so that it's easier to install, get updates, and uninstall if you need to.</span></span>

## <a name="use-homebrew-to-install"></a><span data-ttu-id="b18b3-107">Utilisez Homebrew pour l’installation</span><span class="sxs-lookup"><span data-stu-id="b18b3-107">Use homebrew to install</span></span>

<span data-ttu-id="b18b3-108">Homebrew est le moyen le plus simple pour gérer votre installation d’interface de ligne de commande.</span><span class="sxs-lookup"><span data-stu-id="b18b3-108">Homebrew is the easiest way to manage your CLI install.</span></span> <span data-ttu-id="b18b3-109">Il offre des moyens pratiques pour installer, mettre à jour et désinstaller.</span><span class="sxs-lookup"><span data-stu-id="b18b3-109">It provides convenient ways to install, update, and uninstall.</span></span> <span data-ttu-id="b18b3-110">Il est semblable à d’autres gestionnaires de package comme `apt` ou `yum`.</span><span class="sxs-lookup"><span data-stu-id="b18b3-110">It's similar to other package managers such as `apt` or `yum`.</span></span>
<span data-ttu-id="b18b3-111">Si vous ne disposez pas de Homebrew sur votre système, [installez Homebrew](https://docs.brew.sh/Installation.html) avant de continuer.</span><span class="sxs-lookup"><span data-stu-id="b18b3-111">If you don't have homebrew available on your system, [install homebrew](https://docs.brew.sh/Installation.html) before continuing.</span></span>

### <a name="install-with-homebrew"></a><span data-ttu-id="b18b3-112">Installer avec Homebrew</span><span class="sxs-lookup"><span data-stu-id="b18b3-112">Install with homebrew</span></span>

<span data-ttu-id="b18b3-113">Vous pouvez installer l’interface de ligne de commande en mettant à jour vos informations de référentiel Homebrew, puis en exécutant la commande `install` :</span><span class="sxs-lookup"><span data-stu-id="b18b3-113">You can install the CLI by updating your brew repository information, and then running the `install` command:</span></span>

```bash
brew update && brew install azure-cli
```

<span data-ttu-id="b18b3-114">Vous pouvez ensuite exécuter l’interface de ligne de commande Azure avec la commande `az`.</span><span class="sxs-lookup"><span data-stu-id="b18b3-114">You can then run the Azure CLI with the `az` command.</span></span>

### <a name="update-with-homebrew"></a><span data-ttu-id="b18b3-115">Mettre à jour avec Homebrew</span><span class="sxs-lookup"><span data-stu-id="b18b3-115">Update with homebrew</span></span>

<span data-ttu-id="b18b3-116">L’interface de ligne de commande est régulièrement mise à jour avec des correctifs de bogues, des améliorations, de nouvelles fonctions ainsi que des fonctionnalités en préversion.</span><span class="sxs-lookup"><span data-stu-id="b18b3-116">The CLI is regularly updated with bug fixes, improvements, new features, and preview functionality.</span></span> <span data-ttu-id="b18b3-117">Une nouvelle version est disponible à peu près toutes les deux semaines.</span><span class="sxs-lookup"><span data-stu-id="b18b3-117">A new release is available roughly every two weeks.</span></span> <span data-ttu-id="b18b3-118">Vous devez mettre à jour vos informations de référentiel local, puis le package de l’interface de ligne de commande.</span><span class="sxs-lookup"><span data-stu-id="b18b3-118">You will need to update your local repository information, and then update the CLI package.</span></span>

```bash
brew update && brew upgrade azure-cli
```

### <a name="troubleshooting"></a><span data-ttu-id="b18b3-119">Résolution des problèmes</span><span class="sxs-lookup"><span data-stu-id="b18b3-119">Troubleshooting</span></span>

<span data-ttu-id="b18b3-120">Avez-vous rencontré un problème lors de l’installation ou la mise à jour de l’interface de ligne de commande avec Homebrew ?</span><span class="sxs-lookup"><span data-stu-id="b18b3-120">Did you encounter a problem when installing or updating the CLI with homebrew?</span></span> <span data-ttu-id="b18b3-121">Voici certaines erreurs courantes qui peuvent se produire et comment les diagnostiquer et les résoudre.</span><span class="sxs-lookup"><span data-stu-id="b18b3-121">Here are some common errors that might occur, and ways to diagnose and resolve them.</span></span>

#### <a name="unable-to-find-python-or-installed-packages"></a><span data-ttu-id="b18b3-122">Impossible de trouver des packages Python ou des packages installés</span><span class="sxs-lookup"><span data-stu-id="b18b3-122">Unable to find Python or installed packages</span></span>

<span data-ttu-id="b18b3-123">Si votre programme d’installation ne peut pas trouver les packages Python ou les packages installés, il se peut qu’il y ait une incompatibilité de version mineure ou un autre problème qui s’est produit lors de l’installation de Homebrew.</span><span class="sxs-lookup"><span data-stu-id="b18b3-123">If your install is unable to find Python or installed packages, there may be a minor version mismatch or other issue which occurred during homebrew installation.</span></span> <span data-ttu-id="b18b3-124">Étant donné que l’interface CLI n’utilise pas un virtualenv, cela dépend de sa capacité à trouver des versions appropriées de Python installées par Homebrew.</span><span class="sxs-lookup"><span data-stu-id="b18b3-124">Since the CLI does not use a virtualenv, it relies on being able to find correct versions of Python installed by homebrew.</span></span> <span data-ttu-id="b18b3-125">Vous pourrez peut-être résoudre ces problèmes en liant à nouveau votre installation de Python :</span><span class="sxs-lookup"><span data-stu-id="b18b3-125">You may be able to fix these issues by re-linking your Python installation:</span></span>

```bash
brew link --overwrite python3
```

#### <a name="the-cli-version-is-out-of-date"></a><span data-ttu-id="b18b3-126">La version de l’interface de ligne de commande est obsolète</span><span class="sxs-lookup"><span data-stu-id="b18b3-126">The CLI version is out of date</span></span>

<span data-ttu-id="b18b3-127">Si vous pensez que votre version de l’interface de ligne de commande peut être obsolète, exécutez une commande `brew update`, suivie par `brew upgrade azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="b18b3-127">If you think that your installed CLI version might be out of date, you will need to run a `brew update` command, followed by `brew upgrade azure-cli`.</span></span> <span data-ttu-id="b18b3-128">Si cela ne met pas à jour l’interface de ligne de commande, n’oubliez pas que les packages de Homebrew peuvent se déployer plus lentement que les versions générales.</span><span class="sxs-lookup"><span data-stu-id="b18b3-128">If this does not update the CLI, be aware that homebrew packages may roll out more slowly than general releases.</span></span> <span data-ttu-id="b18b3-129">Si vous avez besoin des installations les plus récentes de l’interface de ligne de commande, vous devriez [installer manuellement](#manage-the-cli-manually).</span><span class="sxs-lookup"><span data-stu-id="b18b3-129">If you require bleeding-edge installs of the CLI, then you should [install manually](#manage-the-cli-manually).</span></span>

### <a name="uninstall-with-homebrew"></a><span data-ttu-id="b18b3-130">Désinstaller avec Homebrew</span><span class="sxs-lookup"><span data-stu-id="b18b3-130">Uninstall with homebrew</span></span>

<span data-ttu-id="b18b3-131">Si jamais vous décidez de désinstaller l’interface de ligne de commande Azure, nous sommes désolés de vous voir partir.</span><span class="sxs-lookup"><span data-stu-id="b18b3-131">If you ever decide to uninstall the Azure CLI, we're sorry to see you go.</span></span> <span data-ttu-id="b18b3-132">Avant de désinstaller, utilisez la commande `az feedback`, afin de nous donner quelques raisons pour lesquelles vous avez choisi de désinstaller et nous aider à améliorer l’expérience CLI.</span><span class="sxs-lookup"><span data-stu-id="b18b3-132">Before you uninstall, use the `az feedback` command to give us some reasons why you chose to uninstall and how we could improve the CLI experience.</span></span> <span data-ttu-id="b18b3-133">Nous souhaitons nous assurer que l’interface de ligne de commande Azure est aussi conviviale et exempte de bogues que possible.</span><span class="sxs-lookup"><span data-stu-id="b18b3-133">We want to make sure that the Azure CLI is as bug-free and user-friendly as we can make it.</span></span> <span data-ttu-id="b18b3-134">Vous pouvez également [signaler un problème lié à GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="b18b3-134">You can also [file a github issue](https://github.com/Azure/azure-cli/issues).</span></span>

<span data-ttu-id="b18b3-135">Si vous avez installé avec Homebrew, vous devez également l’utiliser pour désinstaller.</span><span class="sxs-lookup"><span data-stu-id="b18b3-135">If you installed with homebrew, you should also use it to uninstall.</span></span>

```bash
brew uninstall azure-cli
```

## <a name="install-the-cli-manually"></a><span data-ttu-id="b18b3-136">Installation manuelle de l’interface de ligne de commande</span><span class="sxs-lookup"><span data-stu-id="b18b3-136">Install the CLI manually</span></span>

<span data-ttu-id="b18b3-137">Si vous ne pouvez pas ou ne souhaitez pas gérer l’installation de l’interface de ligne de commande avec Homebrew, vous pouvez installer manuellement.</span><span class="sxs-lookup"><span data-stu-id="b18b3-137">If you can't or don't want to rely on homebrew to manage the CLI install for you, then you can manually install.</span></span>

<span data-ttu-id="b18b3-138">Suivez les [instructions d’installation manuelles de Linux](install-azure-cli-linux.md) pour installer manuellement sur macOS.</span><span class="sxs-lookup"><span data-stu-id="b18b3-138">Follow the [manual Linux installation instructions](install-azure-cli-linux.md) to install manually on macOS.</span></span> <span data-ttu-id="b18b3-139">Les versions macOS 10.9 et versions ultérieures doivent inclure toutes les dépendances requises.</span><span class="sxs-lookup"><span data-stu-id="b18b3-139">macOS versions 10.9 and later should include all of the required dependencies.</span></span>
