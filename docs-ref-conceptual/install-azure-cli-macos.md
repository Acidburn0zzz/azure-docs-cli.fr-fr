---
title: Installer l’interface de ligne de commande Azure pour macOS
description: Comment installer Azure CLI sur macOS
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 11/05/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 40415bc7bec056dc1564c58c8df3f7263bee348c
ms.sourcegitcommit: f40bd067ece4e6ec13e259782ed8db3e33b61a75
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/18/2018
ms.locfileid: "53593164"
---
# <a name="install-azure-cli-on-macos"></a><span data-ttu-id="1afd9-103">Installer Azure CLI sur macOS</span><span class="sxs-lookup"><span data-stu-id="1afd9-103">Install Azure CLI on macOS</span></span>

<span data-ttu-id="1afd9-104">Pour la plateforme macOS, vous pouvez installer Azure CLI avec le [Gestionnaire de package Homebrew](https://brew.sh).</span><span class="sxs-lookup"><span data-stu-id="1afd9-104">For the macOS platform, you can install the Azure CLI with [homebrew package manager](https://brew.sh).</span></span> <span data-ttu-id="1afd9-105">Homebrew facilite le maintien à jour de votre installation de la mise à jour de l’interface CLI.</span><span class="sxs-lookup"><span data-stu-id="1afd9-105">Homebrew makes it easy to keep your installation of the CLI update to date.</span></span> <span data-ttu-id="1afd9-106">Le package CLI a été testé sur macOS 10.9 et les versions ultérieures.</span><span class="sxs-lookup"><span data-stu-id="1afd9-106">The CLI package has been tested on macOS versions 10.9 and later.</span></span>

## <a name="install"></a><span data-ttu-id="1afd9-107">Installer</span><span class="sxs-lookup"><span data-stu-id="1afd9-107">Install</span></span>

<span data-ttu-id="1afd9-108">Homebrew est le moyen le plus simple pour gérer votre installation d’interface de ligne de commande.</span><span class="sxs-lookup"><span data-stu-id="1afd9-108">Homebrew is the easiest way to manage your CLI install.</span></span> <span data-ttu-id="1afd9-109">Il offre des moyens pratiques pour installer, mettre à jour et désinstaller.</span><span class="sxs-lookup"><span data-stu-id="1afd9-109">It provides convenient ways to install, update, and uninstall.</span></span>
<span data-ttu-id="1afd9-110">Si vous ne disposez pas de Homebrew sur votre système, [installez Homebrew](https://docs.brew.sh/Installation.html) avant de continuer.</span><span class="sxs-lookup"><span data-stu-id="1afd9-110">If you don't have homebrew available on your system, [install homebrew](https://docs.brew.sh/Installation.html) before continuing.</span></span>

<span data-ttu-id="1afd9-111">Vous pouvez installer l’interface de ligne de commande en mettant à jour vos informations de référentiel Homebrew, puis en exécutant la commande `install` :</span><span class="sxs-lookup"><span data-stu-id="1afd9-111">You can install the CLI by updating your brew repository information, and then running the `install` command:</span></span>

```bash
brew update && brew install azure-cli
```

<span data-ttu-id="1afd9-112">Vous pouvez ensuite exécuter l’interface de ligne de commande Azure avec la commande `az`.</span><span class="sxs-lookup"><span data-stu-id="1afd9-112">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="1afd9-113">Pour vous connecter, utilisez la commande [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="1afd9-113">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="1afd9-114">Pour en savoir plus sur les différentes méthodes d’authentification, consultez [Se connecter avec Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="1afd9-114">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="1afd9-115">Résolution de problèmes</span><span class="sxs-lookup"><span data-stu-id="1afd9-115">Troubleshooting</span></span>

<span data-ttu-id="1afd9-116">Si vous rencontrez un problème lors de l’installation de l’interface de ligne de commande via Homebrew, voici quelques erreurs courantes.</span><span class="sxs-lookup"><span data-stu-id="1afd9-116">If you encounter a problem when installing the CLI through Homebrew, here are some common errors.</span></span> <span data-ttu-id="1afd9-117">Si vous rencontrez un problème n’étant pas évoqué ici, [signalez un problème sur github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="1afd9-117">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="unable-to-find-python-or-installed-packages"></a><span data-ttu-id="1afd9-118">Impossible de trouver des packages Python ou des packages installés</span><span class="sxs-lookup"><span data-stu-id="1afd9-118">Unable to find Python or installed packages</span></span>

<span data-ttu-id="1afd9-119">Une incompatibilité de version mineure ou un autre problème a pu se produire lors de l’installation de Homebrew.</span><span class="sxs-lookup"><span data-stu-id="1afd9-119">There may be a minor version mismatch or other issue during homebrew installation.</span></span> <span data-ttu-id="1afd9-120">L’interface CLI n’utilise pas d’environnement virtuel Python, ainsi, elle s’appuie sur la recherche de la version de Python installée.</span><span class="sxs-lookup"><span data-stu-id="1afd9-120">The CLI doesn't use a Python virtual environment, so it relies on finding the installed Python version.</span></span> <span data-ttu-id="1afd9-121">Un correctif possible consiste à installer et à relier la dépendance `python3` depuis Homebrew.</span><span class="sxs-lookup"><span data-stu-id="1afd9-121">A possible fix is to install and relink the `python3` dependency from Homebrew.</span></span>

```bash
brew update && brew install python3 && brew upgrade python3
brew link --overwrite python3
```

### <a name="cli-version-1x-is-installed"></a><span data-ttu-id="1afd9-122">La version 1.x de l’interface de ligne de commande est installée</span><span class="sxs-lookup"><span data-stu-id="1afd9-122">CLI version 1.x is installed</span></span>

<span data-ttu-id="1afd9-123">Si une version obsolète a été installée, cela peut être dû à un cache Homebrew périmé.</span><span class="sxs-lookup"><span data-stu-id="1afd9-123">If an out-of-date version was installed, it could be because of a stale homebrew cache.</span></span> <span data-ttu-id="1afd9-124">Suivez les instructions de [mise à jour](#Update).</span><span class="sxs-lookup"><span data-stu-id="1afd9-124">Follow the [update](#Update) instructions.</span></span>

## <a name="update"></a><span data-ttu-id="1afd9-125">Mettre à jour</span><span class="sxs-lookup"><span data-stu-id="1afd9-125">Update</span></span>

<span data-ttu-id="1afd9-126">L’interface de ligne de commande est régulièrement mise à jour avec des correctifs de bogues, des améliorations, de nouvelles fonctions ainsi que des fonctionnalités en préversion.</span><span class="sxs-lookup"><span data-stu-id="1afd9-126">The CLI is regularly updated with bug fixes, improvements, new features, and preview functionality.</span></span> <span data-ttu-id="1afd9-127">Une nouvelle version est disponible à peu près toutes les deux semaines.</span><span class="sxs-lookup"><span data-stu-id="1afd9-127">A new release is available roughly every two weeks.</span></span> <span data-ttu-id="1afd9-128">Mettez à jour vos informations de référentiel local, puis mettez à niveau le package `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="1afd9-128">Update your local repository information and then upgrade the `azure-cli` package.</span></span>

```bash
brew update && brew upgrade azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="1afd9-129">Désinstaller l’interface</span><span class="sxs-lookup"><span data-stu-id="1afd9-129">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="1afd9-130">Utilisez homebrew pour désinstaller le package `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="1afd9-130">Use homebrew to uninstall the `azure-cli` package.</span></span>

```bash
brew uninstall azure-cli
```

## <a name="other-installation-methods"></a><span data-ttu-id="1afd9-131">Autres méthodes d’installation</span><span class="sxs-lookup"><span data-stu-id="1afd9-131">Other installation methods</span></span>

<span data-ttu-id="1afd9-132">Si vous ne pouvez pas utiliser homebrew pour installer Azure CLI dans votre environnement, il est possible d’utiliser les instructions manuelles pour Linux.</span><span class="sxs-lookup"><span data-stu-id="1afd9-132">If you can't use homebrew to install the Azure CLI in your environment, it's possible to use the manual instructions for Linux.</span></span> <span data-ttu-id="1afd9-133">Notez que ce processus n’est pas officiellement conservé pour être compatible avec macOS.</span><span class="sxs-lookup"><span data-stu-id="1afd9-133">Note that this process is not officially maintained to be compatible with macOS.</span></span> <span data-ttu-id="1afd9-134">L’utilisation d’un gestionnaire de package tel que Homebrew est toujours recommandée.</span><span class="sxs-lookup"><span data-stu-id="1afd9-134">Using a package manager such as Homebrew is always recommended.</span></span> <span data-ttu-id="1afd9-135">Utilisez uniquement la méthode d’installation manuelle si vous ne disposez d’aucune autre option disponible.</span><span class="sxs-lookup"><span data-stu-id="1afd9-135">Only use the manual installation method if you have no other option available.</span></span>

<span data-ttu-id="1afd9-136">Pour les instructions d’installation manuelle, consultez [Installer Azure CLI sur Linux manuellement](install-azure-cli-linux.md).</span><span class="sxs-lookup"><span data-stu-id="1afd9-136">For the manual installation instructions, see [Install Azure CLI on Linux manually](install-azure-cli-linux.md).</span></span>

## <a name="next-steps"></a><span data-ttu-id="1afd9-137">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="1afd9-137">Next Steps</span></span>

<span data-ttu-id="1afd9-138">Maintenant que vous avez installé l’interface CLI, découvrez ses fonctionnalités et ses commandes courantes.</span><span class="sxs-lookup"><span data-stu-id="1afd9-138">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="1afd9-139">Prise en main de l’interface Azure CLI</span><span class="sxs-lookup"><span data-stu-id="1afd9-139">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
