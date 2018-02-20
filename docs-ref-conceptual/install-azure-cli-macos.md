---
title: "Installer l’interface de ligne de commande Azure pour macOS"
description: "Installation d’Azure CLI 2.0 sur macOS"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 01/29/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 0295846abc2fe6091940824c6efc47b8fd64ce9f
ms.sourcegitcommit: b93a19222e116d5880bbe64c03507c64e190331e
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/15/2018
---
# <a name="install-azure-cli-20-on-macos"></a><span data-ttu-id="3a148-103">Installation d’Azure CLI 2.0 sur macOS</span><span class="sxs-lookup"><span data-stu-id="3a148-103">Install Azure CLI 2.0 on macOS</span></span>

<span data-ttu-id="3a148-104">Pour la plateforme macOS, vous pouvez installer Azure CLI avec le [Gestionnaire de package Homebrew](http://brew.sh).</span><span class="sxs-lookup"><span data-stu-id="3a148-104">For the macOS platform, you can install the Azure CLI with [homebrew package manager](http://brew.sh).</span></span> <span data-ttu-id="3a148-105">Homebrew facilite le maintien à jour de votre installation de la mise à jour de l’interface CLI.</span><span class="sxs-lookup"><span data-stu-id="3a148-105">Homebrew makes it easy to keep your installation of the CLI update to date.</span></span> <span data-ttu-id="3a148-106">Le package CLI a été testé sur macOS 10.9 et les versions ultérieures.</span><span class="sxs-lookup"><span data-stu-id="3a148-106">The CLI package has been tested on macOS versions 10.9 and later.</span></span>

## <a name="install"></a><span data-ttu-id="3a148-107">Installer</span><span class="sxs-lookup"><span data-stu-id="3a148-107">Install</span></span>

<span data-ttu-id="3a148-108">Homebrew est le moyen le plus simple pour gérer votre installation d’interface de ligne de commande.</span><span class="sxs-lookup"><span data-stu-id="3a148-108">Homebrew is the easiest way to manage your CLI install.</span></span> <span data-ttu-id="3a148-109">Il offre des moyens pratiques pour installer, mettre à jour et désinstaller.</span><span class="sxs-lookup"><span data-stu-id="3a148-109">It provides convenient ways to install, update, and uninstall.</span></span>
<span data-ttu-id="3a148-110">Si vous ne disposez pas de Homebrew sur votre système, [installez Homebrew](https://docs.brew.sh/Installation.html) avant de continuer.</span><span class="sxs-lookup"><span data-stu-id="3a148-110">If you don't have homebrew available on your system, [install homebrew](https://docs.brew.sh/Installation.html) before continuing.</span></span>

<span data-ttu-id="3a148-111">Vous pouvez installer l’interface de ligne de commande en mettant à jour vos informations de référentiel Homebrew, puis en exécutant la commande `install` :</span><span class="sxs-lookup"><span data-stu-id="3a148-111">You can install the CLI by updating your brew repository information, and then running the `install` command:</span></span>

```bash
brew update && brew install azure-cli
```

<span data-ttu-id="3a148-112">Vous pouvez ensuite exécuter l’interface de ligne de commande Azure avec la commande `az`.</span><span class="sxs-lookup"><span data-stu-id="3a148-112">You can then run the Azure CLI with the `az` command.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="3a148-113">Résolution de problèmes</span><span class="sxs-lookup"><span data-stu-id="3a148-113">Troubleshooting</span></span>

<span data-ttu-id="3a148-114">Si vous rencontrez un problème lors de l’installation de l’interface de ligne de commande via Homebrew, voici quelques erreurs courantes.</span><span class="sxs-lookup"><span data-stu-id="3a148-114">If you encounter a problem when installing the CLI through Homebrew, here are some common errors.</span></span> <span data-ttu-id="3a148-115">Si votre problème ne figure pas ici, veuillez [signaler le problème sur Github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="3a148-115">If your issue is not listed here, please [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="unable-to-find-python-or-installed-packages"></a><span data-ttu-id="3a148-116">Impossible de trouver des packages Python ou des packages installés</span><span class="sxs-lookup"><span data-stu-id="3a148-116">Unable to find Python or installed packages</span></span>

<span data-ttu-id="3a148-117">Si votre programme d’installation ne trouve pas les packages Python ou les packages installés, il se peut qu’il y ait une incompatibilité de version mineure ou un autre problème qui s’est produit lors de l’installation de Homebrew.</span><span class="sxs-lookup"><span data-stu-id="3a148-117">If your install is unable to find Python or installed packages, there may be a minor version mismatch or other issue that occurred during homebrew installation.</span></span> <span data-ttu-id="3a148-118">Étant donné que l’interface CLI n’utilise pas un environnement virtuel Python, cela dépend de sa capacité à trouver des versions appropriées de Python.</span><span class="sxs-lookup"><span data-stu-id="3a148-118">Since the CLI does not use a Python virtual environment, it relies on being able to find correct Python version.</span></span> <span data-ttu-id="3a148-119">Vous pourrez peut-être résoudre ces problèmes en liant à nouveau votre installation de Python.</span><span class="sxs-lookup"><span data-stu-id="3a148-119">You may be able to fix these issues by relinking your Python installation.</span></span>

```bash
brew link --overwrite python3
```

### <a name="cli-version-1x-is-installed"></a><span data-ttu-id="3a148-120">La version 1.x de l’interface de ligne de commande est installée</span><span class="sxs-lookup"><span data-stu-id="3a148-120">CLI version 1.x is installed</span></span>

<span data-ttu-id="3a148-121">Si une version obsolète a été installée, cela peut être dû à un cache Homebrew périmé.</span><span class="sxs-lookup"><span data-stu-id="3a148-121">If an out-of-date version was installed, it could be due to a stale homebrew cache.</span></span> <span data-ttu-id="3a148-122">Suivez les instructions de [mise à jour](#Update).</span><span class="sxs-lookup"><span data-stu-id="3a148-122">Follow the [update](#Update) instructions.</span></span>

## <a name="update"></a><span data-ttu-id="3a148-123">Mettre à jour</span><span class="sxs-lookup"><span data-stu-id="3a148-123">Update</span></span>

<span data-ttu-id="3a148-124">L’interface de ligne de commande est régulièrement mise à jour avec des correctifs de bogues, des améliorations, de nouvelles fonctions ainsi que des fonctionnalités en préversion.</span><span class="sxs-lookup"><span data-stu-id="3a148-124">The CLI is regularly updated with bug fixes, improvements, new features, and preview functionality.</span></span> <span data-ttu-id="3a148-125">Une nouvelle version est disponible à peu près toutes les deux semaines.</span><span class="sxs-lookup"><span data-stu-id="3a148-125">A new release is available roughly every two weeks.</span></span> <span data-ttu-id="3a148-126">Mettez à jour vos informations de référentiel local, puis mettez à niveau le package `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="3a148-126">Update your local repository information and then upgrade the `azure-cli` package.</span></span>

```bash
brew update && brew upgrade azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="3a148-127">Désinstaller l’interface</span><span class="sxs-lookup"><span data-stu-id="3a148-127">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="3a148-128">Utilisez homebrew pour désinstaller le package `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="3a148-128">Use homebrew to uninstall the `azure-cli` package.</span></span>

```bash
brew uninstall azure-cli
```
