---
title: Installer l’interface de ligne de commande Azure pour macOS
description: Comment installer Azure CLI sur macOS
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 11/05/2018
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: 826169e0792fc9a08213844468ee516f3e736f1d
ms.sourcegitcommit: bf84dfb62e910ea246586481863bb43d09d07795
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/04/2020
ms.locfileid: "87551153"
---
# <a name="install-azure-cli-on-macos"></a><span data-ttu-id="62459-103">Installer Azure CLI sur macOS</span><span class="sxs-lookup"><span data-stu-id="62459-103">Install Azure CLI on macOS</span></span>

<span data-ttu-id="62459-104">Pour la plateforme macOS, vous pouvez installer Azure CLI avec le [Gestionnaire de package Homebrew](https://brew.sh).</span><span class="sxs-lookup"><span data-stu-id="62459-104">For the macOS platform, you can install the Azure CLI with [homebrew package manager](https://brew.sh).</span></span> <span data-ttu-id="62459-105">Homebrew facilite le maintien à jour de votre installation de la mise à jour de l’interface CLI.</span><span class="sxs-lookup"><span data-stu-id="62459-105">Homebrew makes it easy to keep your installation of the CLI update to date.</span></span> <span data-ttu-id="62459-106">Le package CLI a été testé sur macOS 10.9 et les versions ultérieures.</span><span class="sxs-lookup"><span data-stu-id="62459-106">The CLI package has been tested on macOS versions 10.9 and later.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

## <a name="install-with-homebrew"></a><span data-ttu-id="62459-107">Installer avec Homebrew</span><span class="sxs-lookup"><span data-stu-id="62459-107">Install with Homebrew</span></span>

<span data-ttu-id="62459-108">Homebrew est le moyen le plus simple pour gérer votre installation d’interface de ligne de commande.</span><span class="sxs-lookup"><span data-stu-id="62459-108">Homebrew is the easiest way to manage your CLI install.</span></span> <span data-ttu-id="62459-109">Il offre des moyens pratiques pour installer, mettre à jour et désinstaller.</span><span class="sxs-lookup"><span data-stu-id="62459-109">It provides convenient ways to install, update, and uninstall.</span></span>
<span data-ttu-id="62459-110">Si vous ne disposez pas de Homebrew sur votre système, [installez Homebrew](https://docs.brew.sh/Installation.html) avant de continuer.</span><span class="sxs-lookup"><span data-stu-id="62459-110">If you don't have homebrew available on your system, [install homebrew](https://docs.brew.sh/Installation.html) before continuing.</span></span>

<span data-ttu-id="62459-111">Vous pouvez installer l’interface de ligne de commande en mettant à jour vos informations de référentiel Homebrew, puis en exécutant la commande `install` :</span><span class="sxs-lookup"><span data-stu-id="62459-111">You can install the CLI by updating your brew repository information, and then running the `install` command:</span></span>

```bash
brew update && brew install azure-cli
```

> [!IMPORTANT]
>
> <span data-ttu-id="62459-112">Azure CLI a une dépendance vis-à-vis du package Homebrew `python3` et l’installe.</span><span class="sxs-lookup"><span data-stu-id="62459-112">The Azure CLI has a dependency on the Homebrew `python3` package, and will install it.</span></span>
> <span data-ttu-id="62459-113">Azure CLI offre la garantie d’être compatible avec la dernière version de `python3` publiée sur Homebrew.</span><span class="sxs-lookup"><span data-stu-id="62459-113">The Azure CLI is guaranteed to be compatible with the latest version of `python3` published on Homebrew.</span></span>

<span data-ttu-id="62459-114">Vous pouvez ensuite exécuter l’interface de ligne de commande Azure avec la commande `az`.</span><span class="sxs-lookup"><span data-stu-id="62459-114">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="62459-115">Pour vous connecter, utilisez la commande [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="62459-115">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="62459-116">Pour en savoir plus sur les différentes méthodes d’authentification, consultez [Se connecter avec Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="62459-116">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="62459-117">Dépannage</span><span class="sxs-lookup"><span data-stu-id="62459-117">Troubleshooting</span></span>

<span data-ttu-id="62459-118">Si vous rencontrez un problème lors de l’installation de l’interface de ligne de commande via Homebrew, voici quelques erreurs courantes.</span><span class="sxs-lookup"><span data-stu-id="62459-118">If you encounter a problem when installing the CLI through Homebrew, here are some common errors.</span></span> <span data-ttu-id="62459-119">Si vous rencontrez un problème n’étant pas évoqué ici, [signalez un problème sur github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="62459-119">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="completion-is-not-working"></a><span data-ttu-id="62459-120">La complétion ne fonctionne pas</span><span class="sxs-lookup"><span data-stu-id="62459-120">Completion is not working</span></span>

<span data-ttu-id="62459-121">La formule Homebrew d’Azure CLI installe un fichier de complétion nommé `az` dans le répertoire de complétion géré par Homebrew (l’emplacement par défaut est `/usr/local/etc/bash_completion.d/`).</span><span class="sxs-lookup"><span data-stu-id="62459-121">The Homebrew formula of Azure CLI installs a completion file named `az` in the Homebrew-managed completions directory (default location is `/usr/local/etc/bash_completion.d/`).</span></span> <span data-ttu-id="62459-122">Pour permettre la complétion, suivez les [instructions](https://docs.brew.sh/Shell-Completion) fournies par Homebrew.</span><span class="sxs-lookup"><span data-stu-id="62459-122">To enable completion, please follow Homebrew's instructions [here](https://docs.brew.sh/Shell-Completion).</span></span>

### <a name="unable-to-find-python-or-installed-packages"></a><span data-ttu-id="62459-123">Impossible de trouver des packages Python ou des packages installés</span><span class="sxs-lookup"><span data-stu-id="62459-123">Unable to find Python or installed packages</span></span>

<span data-ttu-id="62459-124">Une incompatibilité de version mineure ou un autre problème a pu se produire lors de l’installation de Homebrew.</span><span class="sxs-lookup"><span data-stu-id="62459-124">There may be a minor version mismatch or other issue during homebrew installation.</span></span> <span data-ttu-id="62459-125">L’interface CLI n’utilise pas d’environnement virtuel Python, ainsi, elle s’appuie sur la recherche de la version de Python installée.</span><span class="sxs-lookup"><span data-stu-id="62459-125">The CLI doesn't use a Python virtual environment, so it relies on finding the installed Python version.</span></span> <span data-ttu-id="62459-126">Un correctif possible consiste à installer et à relier la dépendance `python3` depuis Homebrew.</span><span class="sxs-lookup"><span data-stu-id="62459-126">A possible fix is to install and relink the `python3` dependency from Homebrew.</span></span>

```bash
brew update && brew install python3 && brew upgrade python3
brew link --overwrite python3
```

### <a name="cli-version-1x-is-installed"></a><span data-ttu-id="62459-127">La version 1.x de l’interface de ligne de commande est installée</span><span class="sxs-lookup"><span data-stu-id="62459-127">CLI version 1.x is installed</span></span>

<span data-ttu-id="62459-128">Si une version obsolète a été installée, cela peut être dû à un cache Homebrew périmé.</span><span class="sxs-lookup"><span data-stu-id="62459-128">If an out-of-date version was installed, it could be because of a stale homebrew cache.</span></span> <span data-ttu-id="62459-129">Suivez les instructions de [mise à jour](#update).</span><span class="sxs-lookup"><span data-stu-id="62459-129">Follow the [update](#update) instructions.</span></span>

### <a name="proxy-blocks-connection"></a><span data-ttu-id="62459-130">Le proxy bloque la connexion</span><span class="sxs-lookup"><span data-stu-id="62459-130">Proxy blocks connection</span></span>

<span data-ttu-id="62459-131">Il se peut que vous ne puissiez pas obtenir des ressources à partir de Homebrew, sauf si vous l’avez correctement configuré pour utiliser votre proxy.</span><span class="sxs-lookup"><span data-stu-id="62459-131">You may be unable to get resources from Homebrew unless you have correctly configured it to use your proxy.</span></span> <span data-ttu-id="62459-132">Suivez les [instructions d’installation de proxy Homebrew](https://docs.brew.sh/Manpage#using-homebrew-behind-a-proxy).</span><span class="sxs-lookup"><span data-stu-id="62459-132">Follow the [Homebrew proxy configuration instructions](https://docs.brew.sh/Manpage#using-homebrew-behind-a-proxy).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="62459-133">Si vous vous trouvez derrière un proxy, `HTTP_PROXY` et `HTTPS_PROXY` doivent être définis pour se connecter aux services Azure avec l’interface CLI.</span><span class="sxs-lookup"><span data-stu-id="62459-133">If you are behind a proxy, `HTTP_PROXY` and `HTTPS_PROXY` must be set to connect to Azure services with the CLI.</span></span>
> <span data-ttu-id="62459-134">Si vous n’utilisez pas l’authentification de base, il est recommandé d’exporter ces variables dans votre fichier `.bashrc`.</span><span class="sxs-lookup"><span data-stu-id="62459-134">If you are not using basic auth, it's recommended to export these variables in your `.bashrc` file.</span></span>
> <span data-ttu-id="62459-135">Suivez toujours les stratégies de sécurité de votre entreprise et les exigences de votre administrateur système.</span><span class="sxs-lookup"><span data-stu-id="62459-135">Always follow your business' security policies and the requirements of your system administrator.</span></span>

<span data-ttu-id="62459-136">Pour obtenir les ressources Bottle de Homebrew, votre proxy doit autoriser les connexions HTTPS aux adresses suivantes :</span><span class="sxs-lookup"><span data-stu-id="62459-136">In order to get the bottle resources from Homebrew, your proxy needs to allow HTTPS connections to the following addresses:</span></span>

* `https://formulae.brew.sh`
* `https://homebrew.bintray.com`

## <a name="update"></a><span data-ttu-id="62459-137">Update</span><span class="sxs-lookup"><span data-stu-id="62459-137">Update</span></span>

<span data-ttu-id="62459-138">L’interface de ligne de commande est régulièrement mise à jour avec des correctifs de bogues, des améliorations, de nouvelles fonctions ainsi que des fonctionnalités en préversion.</span><span class="sxs-lookup"><span data-stu-id="62459-138">The CLI is regularly updated with bug fixes, improvements, new features, and preview functionality.</span></span> <span data-ttu-id="62459-139">Une nouvelle version est disponible à peu près toutes les deux semaines.</span><span class="sxs-lookup"><span data-stu-id="62459-139">A new release is available roughly every two weeks.</span></span> <span data-ttu-id="62459-140">Mettez à jour vos informations de référentiel local, puis mettez à niveau le package `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="62459-140">Update your local repository information and then upgrade the `azure-cli` package.</span></span>

```bash
brew update && brew upgrade azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="62459-141">Désinstaller l’interface</span><span class="sxs-lookup"><span data-stu-id="62459-141">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="62459-142">Utilisez homebrew pour désinstaller le package `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="62459-142">Use homebrew to uninstall the `azure-cli` package.</span></span>

```bash
brew uninstall azure-cli
```

## <a name="other-installation-methods"></a><span data-ttu-id="62459-143">Autres méthodes d’installation</span><span class="sxs-lookup"><span data-stu-id="62459-143">Other installation methods</span></span>

<span data-ttu-id="62459-144">Si vous ne pouvez pas utiliser homebrew pour installer Azure CLI dans votre environnement, il est possible d’utiliser les instructions manuelles pour Linux.</span><span class="sxs-lookup"><span data-stu-id="62459-144">If you can't use homebrew to install the Azure CLI in your environment, it's possible to use the manual instructions for Linux.</span></span> <span data-ttu-id="62459-145">Notez que ce processus n’est pas officiellement conservé pour être compatible avec macOS.</span><span class="sxs-lookup"><span data-stu-id="62459-145">Note that this process is not officially maintained to be compatible with macOS.</span></span> <span data-ttu-id="62459-146">L’utilisation d’un gestionnaire de package tel que Homebrew est toujours recommandée.</span><span class="sxs-lookup"><span data-stu-id="62459-146">Using a package manager such as Homebrew is always recommended.</span></span> <span data-ttu-id="62459-147">Utilisez uniquement la méthode d’installation manuelle si vous ne disposez d’aucune autre option disponible.</span><span class="sxs-lookup"><span data-stu-id="62459-147">Only use the manual installation method if you have no other option available.</span></span>

<span data-ttu-id="62459-148">Pour les instructions d’installation manuelle, consultez [Installer Azure CLI sur Linux manuellement](install-azure-cli-linux.md).</span><span class="sxs-lookup"><span data-stu-id="62459-148">For the manual installation instructions, see [Install Azure CLI on Linux manually](install-azure-cli-linux.md).</span></span>

## <a name="next-steps"></a><span data-ttu-id="62459-149">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="62459-149">Next Steps</span></span>

<span data-ttu-id="62459-150">Maintenant que vous avez installé l’interface CLI, découvrez ses fonctionnalités et ses commandes courantes.</span><span class="sxs-lookup"><span data-stu-id="62459-150">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="62459-151">Prise en main de l’interface Azure CLI</span><span class="sxs-lookup"><span data-stu-id="62459-151">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
