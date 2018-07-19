---
title: Installer l’interface de ligne de commande Azure pour macOS
description: Installation d’Azure CLI 2.0 sur macOS
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 01/29/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 76b9afec92aa3da916382b85d2261547b6877e03
ms.sourcegitcommit: fb3fed8701aff6c46af856e8fdc3e56ff9a678bc
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/11/2018
ms.locfileid: "38228918"
---
# <a name="install-azure-cli-20-on-macos"></a><span data-ttu-id="9a5e8-103">Installation d’Azure CLI 2.0 sur macOS</span><span class="sxs-lookup"><span data-stu-id="9a5e8-103">Install Azure CLI 2.0 on macOS</span></span>

<span data-ttu-id="9a5e8-104">Pour la plateforme macOS, vous pouvez installer Azure CLI avec le [Gestionnaire de package Homebrew](http://brew.sh).</span><span class="sxs-lookup"><span data-stu-id="9a5e8-104">For the macOS platform, you can install the Azure CLI with [homebrew package manager](http://brew.sh).</span></span> <span data-ttu-id="9a5e8-105">Homebrew facilite le maintien à jour de votre installation de la mise à jour de l’interface CLI.</span><span class="sxs-lookup"><span data-stu-id="9a5e8-105">Homebrew makes it easy to keep your installation of the CLI update to date.</span></span> <span data-ttu-id="9a5e8-106">Le package CLI a été testé sur macOS 10.9 et les versions ultérieures.</span><span class="sxs-lookup"><span data-stu-id="9a5e8-106">The CLI package has been tested on macOS versions 10.9 and later.</span></span>

## <a name="install"></a><span data-ttu-id="9a5e8-107">Installer</span><span class="sxs-lookup"><span data-stu-id="9a5e8-107">Install</span></span>

<span data-ttu-id="9a5e8-108">Homebrew est le moyen le plus simple pour gérer votre installation d’interface de ligne de commande.</span><span class="sxs-lookup"><span data-stu-id="9a5e8-108">Homebrew is the easiest way to manage your CLI install.</span></span> <span data-ttu-id="9a5e8-109">Il offre des moyens pratiques pour installer, mettre à jour et désinstaller.</span><span class="sxs-lookup"><span data-stu-id="9a5e8-109">It provides convenient ways to install, update, and uninstall.</span></span>
<span data-ttu-id="9a5e8-110">Si vous ne disposez pas de Homebrew sur votre système, [installez Homebrew](https://docs.brew.sh/Installation.html) avant de continuer.</span><span class="sxs-lookup"><span data-stu-id="9a5e8-110">If you don't have homebrew available on your system, [install homebrew](https://docs.brew.sh/Installation.html) before continuing.</span></span>

<span data-ttu-id="9a5e8-111">Vous pouvez installer l’interface de ligne de commande en mettant à jour vos informations de référentiel Homebrew, puis en exécutant la commande `install` :</span><span class="sxs-lookup"><span data-stu-id="9a5e8-111">You can install the CLI by updating your brew repository information, and then running the `install` command:</span></span>

```bash
brew update && brew install azure-cli
```

<span data-ttu-id="9a5e8-112">Vous pouvez ensuite exécuter l’interface de ligne de commande Azure avec la commande `az`.</span><span class="sxs-lookup"><span data-stu-id="9a5e8-112">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="9a5e8-113">Pour vous connecter, utilisez la commande [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="9a5e8-113">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="9a5e8-114">Pour en savoir plus sur les différentes méthodes d’authentification, consultez [Se connecter avec Azure CLI 2.0](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="9a5e8-114">To learn more about different authentication methods, see [Sign in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="9a5e8-115">Résolution de problèmes</span><span class="sxs-lookup"><span data-stu-id="9a5e8-115">Troubleshooting</span></span>

<span data-ttu-id="9a5e8-116">Si vous rencontrez un problème lors de l’installation de l’interface de ligne de commande via Homebrew, voici quelques erreurs courantes.</span><span class="sxs-lookup"><span data-stu-id="9a5e8-116">If you encounter a problem when installing the CLI through Homebrew, here are some common errors.</span></span> <span data-ttu-id="9a5e8-117">Si votre problème ne figure pas ici, veuillez [signaler le problème sur Github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="9a5e8-117">If your issue is not listed here, please [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="unable-to-find-python-or-installed-packages"></a><span data-ttu-id="9a5e8-118">Impossible de trouver des packages Python ou des packages installés</span><span class="sxs-lookup"><span data-stu-id="9a5e8-118">Unable to find Python or installed packages</span></span>

<span data-ttu-id="9a5e8-119">Si votre programme d’installation ne trouve pas les packages Python ou les packages installés, il se peut qu’il y ait une incompatibilité de version mineure ou un autre problème qui s’est produit lors de l’installation de Homebrew.</span><span class="sxs-lookup"><span data-stu-id="9a5e8-119">If your install is unable to find Python or installed packages, there may be a minor version mismatch or other issue that occurred during homebrew installation.</span></span> <span data-ttu-id="9a5e8-120">Étant donné que l’interface CLI n’utilise pas un environnement virtuel Python, cela dépend de sa capacité à trouver des versions appropriées de Python.</span><span class="sxs-lookup"><span data-stu-id="9a5e8-120">Since the CLI does not use a Python virtual environment, it relies on being able to find correct Python version.</span></span> <span data-ttu-id="9a5e8-121">Vous pourrez peut-être résoudre ces problèmes en liant à nouveau votre installation de Python.</span><span class="sxs-lookup"><span data-stu-id="9a5e8-121">You may be able to fix these issues by relinking your Python installation.</span></span>

```bash
brew link --overwrite python3
```

### <a name="cli-version-1x-is-installed"></a><span data-ttu-id="9a5e8-122">La version 1.x de l’interface de ligne de commande est installée</span><span class="sxs-lookup"><span data-stu-id="9a5e8-122">CLI version 1.x is installed</span></span>

<span data-ttu-id="9a5e8-123">Si une version obsolète a été installée, cela peut être dû à un cache Homebrew périmé.</span><span class="sxs-lookup"><span data-stu-id="9a5e8-123">If an out-of-date version was installed, it could be due to a stale homebrew cache.</span></span> <span data-ttu-id="9a5e8-124">Suivez les instructions de [mise à jour](#Update).</span><span class="sxs-lookup"><span data-stu-id="9a5e8-124">Follow the [update](#Update) instructions.</span></span>

## <a name="update"></a><span data-ttu-id="9a5e8-125">Mettre à jour</span><span class="sxs-lookup"><span data-stu-id="9a5e8-125">Update</span></span>

<span data-ttu-id="9a5e8-126">L’interface de ligne de commande est régulièrement mise à jour avec des correctifs de bogues, des améliorations, de nouvelles fonctions ainsi que des fonctionnalités en préversion.</span><span class="sxs-lookup"><span data-stu-id="9a5e8-126">The CLI is regularly updated with bug fixes, improvements, new features, and preview functionality.</span></span> <span data-ttu-id="9a5e8-127">Une nouvelle version est disponible à peu près toutes les deux semaines.</span><span class="sxs-lookup"><span data-stu-id="9a5e8-127">A new release is available roughly every two weeks.</span></span> <span data-ttu-id="9a5e8-128">Mettez à jour vos informations de référentiel local, puis mettez à niveau le package `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="9a5e8-128">Update your local repository information and then upgrade the `azure-cli` package.</span></span>

```bash
brew update && brew upgrade azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="9a5e8-129">Désinstaller l’interface</span><span class="sxs-lookup"><span data-stu-id="9a5e8-129">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="9a5e8-130">Utilisez homebrew pour désinstaller le package `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="9a5e8-130">Use homebrew to uninstall the `azure-cli` package.</span></span>

```bash
brew uninstall azure-cli
```
