---
title: Installez l’interface de ligne de commande d’Azure CLI Classic
description: Installez l’interface de ligne de commande Azure CLI Classic pour Mac, Linux et Windows afin de commencer à utiliser les services Azure
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 06/11/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 68aa728b9b9324a53856008f05d8ce30eb61c76d
ms.sourcegitcommit: c4462456dfb17993f098d47c37bc19f4d78b8179
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/25/2018
ms.locfileid: "47178163"
---
# <a name="install-the-azure-classic-cli"></a><span data-ttu-id="7026b-103">Installez l’interface de ligne de commande d’Azure CLI Classic</span><span class="sxs-lookup"><span data-stu-id="7026b-103">Install the Azure classic CLI</span></span>

> [!IMPORTANT]
> <span data-ttu-id="7026b-104">Cette rubrique décrit comment installer l’interface de ligne de commande Azure CLI Classic.</span><span class="sxs-lookup"><span data-stu-id="7026b-104">This topic describes how to install the Azure classic CLI.</span></span> <span data-ttu-id="7026b-105">L’interface de ligne de commande classique est déconseillée et doit uniquement être utilisée avec le modèle de déploiement classique.</span><span class="sxs-lookup"><span data-stu-id="7026b-105">The classic CLI is deprecated and should only be used with the classic deployment model.</span></span>
> <span data-ttu-id="7026b-106">Pour tous les autres déploiements, utilisez [Azure CLI](/cli/azure).</span><span class="sxs-lookup"><span data-stu-id="7026b-106">For all other deployments, use [the Azure CLI](/cli/azure).</span></span>

<span data-ttu-id="7026b-107">Installez rapidement l’interface de ligne de commande Azure CLI Classic pour bénéficier d’un ensemble d’interpréteurs de commandes open source permettant de créer et de gérer des ressources dans Microsoft Azure.</span><span class="sxs-lookup"><span data-stu-id="7026b-107">Quickly install the Azure classic CLI to use a set of open-source shell-based commands for creating and managing resources in Microsoft Azure.</span></span> <span data-ttu-id="7026b-108">Vous avez plusieurs options pour installer ces outils multiplateformes sur votre ordinateur :</span><span class="sxs-lookup"><span data-stu-id="7026b-108">You have several options to install these cross-platform tools on your computer:</span></span>

* <span data-ttu-id="7026b-109">**Package npm** : exécutez npm (le Gestionnaire de package pour JavaScript) afin d’installer le dernier package de l’interface de ligne de commande Azure CLI Classic sur votre système d’exploitation ou sur votre distribution Linux.</span><span class="sxs-lookup"><span data-stu-id="7026b-109">**npm package** - Run npm (the package manager for JavaScript) to install the Azure classic CLI package on your Linux distribution or OS.</span></span> <span data-ttu-id="7026b-110">Nécessite node.js et npm.</span><span class="sxs-lookup"><span data-stu-id="7026b-110">Requires node.js and npm.</span></span>
* <span data-ttu-id="7026b-111">**Programme d’installation** : téléchargez un programme d’installation pour une installation simple sur macOS ou Windows.</span><span class="sxs-lookup"><span data-stu-id="7026b-111">**Installer** - Download an installer for easy installation on macOS or Windows.</span></span>
* <span data-ttu-id="7026b-112">**Conteneur Docker** : utilisez l’interface de ligne de commande classique dans un conteneur Docker prêt à exécuter.</span><span class="sxs-lookup"><span data-stu-id="7026b-112">**Docker container** - Start using the classic CLI in a ready-to-run Docker container.</span></span> <span data-ttu-id="7026b-113">Nécessite un hôte Docker.</span><span class="sxs-lookup"><span data-stu-id="7026b-113">Requires a Docker host.</span></span>

<span data-ttu-id="7026b-114">Pour obtenir davantage d’options générales et de contexte, consultez le référentiel du projet sur [GitHub](https://github.com/azure/azure-xplat-cli).</span><span class="sxs-lookup"><span data-stu-id="7026b-114">For more options and background, see the project repository on [GitHub](https://github.com/azure/azure-xplat-cli).</span></span>

<span data-ttu-id="7026b-115">Une fois l’interface de ligne de commande Azure CLI Classic installée, connectez-vous à l’aide de `azure login` et exécutez les commandes `azure` depuis votre interface de ligne de commande (Bash, terminal, invite de commandes, etc.) pour travailler avec vos ressources Azure.</span><span class="sxs-lookup"><span data-stu-id="7026b-115">Once the Azure classic CLI is installed, connect with `azure login` and run the `azure` commands from your command-line interface (Bash, Terminal, Command prompt, and so on) to work with your Azure resources.</span></span>

## <a name="option-1-install-an-npm-package"></a><span data-ttu-id="7026b-116">Option 1 : Installer un package npm</span><span class="sxs-lookup"><span data-stu-id="7026b-116">Option 1: Install an npm package</span></span>

<span data-ttu-id="7026b-117">Pour installer l’interface de ligne de commande classique à partir d’un package npm, vérifiez que vous avez téléchargé et installé les [derniers fichiers Node.js et npm](https://nodejs.org/en/download/package-manager/).</span><span class="sxs-lookup"><span data-stu-id="7026b-117">To install the classic CLI from an npm package, make sure you have downloaded and installed the [latest Node.js and npm](https://nodejs.org/en/download/package-manager/).</span></span> <span data-ttu-id="7026b-118">Ensuite, exécutez `npm install` pour installer le package azure-cli :</span><span class="sxs-lookup"><span data-stu-id="7026b-118">Then, run `npm install` to install the azure-cli package:</span></span>

```bash
npm install -g azure-cli
```

<span data-ttu-id="7026b-119">Sur les distributions Linux, vous devrez peut-être utiliser `sudo` pour exécuter la commande `npm`, comme suit :</span><span class="sxs-lookup"><span data-stu-id="7026b-119">On Linux distributions, you might need to use `sudo` to successfully run the `npm` command, as follows:</span></span>

```bash
sudo npm install -g azure-cli
```

> [!NOTE]
> <span data-ttu-id="7026b-120">Si vous devez installer ou mettre à jour Node.js et npm sur votre système d’exploitation, nous vous recommandons d’installer la dernière version de Node.js LTS 4.x, ou une version ultérieure.</span><span class="sxs-lookup"><span data-stu-id="7026b-120">If you need to install or update Node.js and npm on your OS, we recommend that you install Node.js LTS version 4.x or later.</span></span> <span data-ttu-id="7026b-121">Si vous utilisez une version antérieure, vous pouvez obtenir des erreurs d’installation.</span><span class="sxs-lookup"><span data-stu-id="7026b-121">If you use an older version, you might get installation errors.</span></span>

<span data-ttu-id="7026b-122">Si vous préférez, vous pouvez également télécharger un fichier tar à partir des [versions GitHub](https://github.com/Azure/azure-xplat-cli/releases).</span><span class="sxs-lookup"><span data-stu-id="7026b-122">If you prefer, you may also download a tar file from the [GitHub releases](https://github.com/Azure/azure-xplat-cli/releases).</span></span> <span data-ttu-id="7026b-123">Ensuite, installez le package npm téléchargé comme suit (sur les distributions Linux, vous devrez peut-être utiliser `sudo`) :</span><span class="sxs-lookup"><span data-stu-id="7026b-123">Then, install the downloaded npm package as follows (on Linux distributions you might need to use `sudo`):</span></span>

```bash
npm install -g <path to downloaded tar file>
```

## <a name="option-2-use-an-installer"></a><span data-ttu-id="7026b-124">Option 2 : Utiliser un programme d’installation</span><span class="sxs-lookup"><span data-stu-id="7026b-124">Option 2: Use an installer</span></span>

<span data-ttu-id="7026b-125">Si vous utilisez un ordinateur Mac ou Windows, les programmes d’installation DMG et MSI sont disponibles depuis les [versions GitHub](https://github.com/Azure/azure-xplat-cli/releases).</span><span class="sxs-lookup"><span data-stu-id="7026b-125">If you use a Mac or Windows computer, DMG and MSI installers are available from [GitHub releases](https://github.com/Azure/azure-xplat-cli/releases).</span></span>

> [!TIP]
> <span data-ttu-id="7026b-126">Sous Windows, vous pouvez également télécharger [Web Platform Installer](https://go.microsoft.com/?linkid=9828653) pour installer l’interface de ligne de commande classique.</span><span class="sxs-lookup"><span data-stu-id="7026b-126">On Windows, you can also download the [Web Platform Installer](https://go.microsoft.com/?linkid=9828653) to install the classic CLI.</span></span> <span data-ttu-id="7026b-127">Ce programme d’installation vous donne la possibilité d’installer des Kits de développement logiciel (SDK) Azure et des outils de ligne de commande supplémentaires.</span><span class="sxs-lookup"><span data-stu-id="7026b-127">This installer gives you the option to install additional Azure SDK and command-line tools.</span></span>

## <a name="option-3-use-a-docker-container"></a><span data-ttu-id="7026b-128">Option 3 : Utiliser un conteneur Docker</span><span class="sxs-lookup"><span data-stu-id="7026b-128">Option 3: Use a Docker container</span></span>

<span data-ttu-id="7026b-129">Si vous avez configuré votre ordinateur comme hôte [Docker](https://docs.docker.com/engine/understanding-docker/), vous pouvez exécuter l’interface de ligne de commande Azure CLI Classic dans un conteneur Docker.</span><span class="sxs-lookup"><span data-stu-id="7026b-129">If you have set up your computer as a [Docker](https://docs.docker.com/engine/understanding-docker/) host, you can run the Azure classic CLI in a Docker container.</span></span> <span data-ttu-id="7026b-130">Exécutez la commande suivante (sur les distributions Linux, vous devrez peut-être utiliser `sudo`) :</span><span class="sxs-lookup"><span data-stu-id="7026b-130">Run the following command (on Linux distributions you might need to use `sudo`):</span></span>

```bash
docker run -it microsoft/azure-cli:0.10.17
```

## <a name="run-azure-classic-cli-commands"></a><span data-ttu-id="7026b-131">Exécutez les commandes Azure CLI Classic</span><span class="sxs-lookup"><span data-stu-id="7026b-131">Run Azure classic CLI commands</span></span>

<span data-ttu-id="7026b-132">Une fois l’interface de ligne de commande classique installée, exécutez la commande `azure` depuis l’interface utilisateur de ligne de commande (Bash, terminal, invite de commandes, etc.).</span><span class="sxs-lookup"><span data-stu-id="7026b-132">After the classic CLI is installed, run the `azure` command from your command-line user interface (Bash, Terminal, Command prompt, and so on).</span></span> <span data-ttu-id="7026b-133">Par exemple, pour exécuter la commande d’aide, saisissez ce qui suit :</span><span class="sxs-lookup"><span data-stu-id="7026b-133">For example, to run the help command, type the following:</span></span>

```azurecli
azure help
```

> [!NOTE]
> <span data-ttu-id="7026b-134">Dans certaines distributions Linux, vous pouvez recevoir une erreur similaire à `/usr/bin/env: ‘node’: No such file or directory`.</span><span class="sxs-lookup"><span data-stu-id="7026b-134">On some Linux distributions, you may receive an error similar to `/usr/bin/env: ‘node’: No such file or directory`.</span></span> <span data-ttu-id="7026b-135">Cette erreur est due à l’installation récente de Node.js sous /usr/bin/nodejs.</span><span class="sxs-lookup"><span data-stu-id="7026b-135">This error comes from recent installations of Node.js being installed at /usr/bin/nodejs.</span></span> <span data-ttu-id="7026b-136">Pour la corriger, créez un lien symbolique vers /usr/bin/node en exécutant cette commande :</span><span class="sxs-lookup"><span data-stu-id="7026b-136">To fix it, create a symbolic link to /usr/bin/node by running this command:</span></span>

```bash
sudo ln -s /usr/bin/nodejs /usr/bin/node
```

<span data-ttu-id="7026b-137">Pour afficher la version de l’interface de ligne de commande Azure CLI Classic que vous avez installée, saisissez la commande suivante :</span><span class="sxs-lookup"><span data-stu-id="7026b-137">To see the version of the Azure classic CLI installed, type the following:</span></span>

```azurecli
azure --version
```

> [!NOTE]
> <span data-ttu-id="7026b-138">Lorsque vous utilisez l’interface de ligne de commande Azure CLI Classic pour la première fois, vous voyez un message vous demandant si vous souhaitez autoriser Microsoft à recueillir des informations d’utilisation.</span><span class="sxs-lookup"><span data-stu-id="7026b-138">When you first use Azure classic CLI, you see a message asking if you want to allow Microsoft to collect usage information.</span></span> <span data-ttu-id="7026b-139">La participation se fait sur la base du volontariat.</span><span class="sxs-lookup"><span data-stu-id="7026b-139">Participation is voluntary.</span></span> <span data-ttu-id="7026b-140">Si vous choisissez de participer, vous pouvez arrêter à tout moment en exécutant `azure telemetry --disable`.</span><span class="sxs-lookup"><span data-stu-id="7026b-140">If you choose to participate, you can stop at any time by running `azure telemetry --disable`.</span></span> <span data-ttu-id="7026b-141">Pour activer la participation, exécutez `azure telemetry --enable`.</span><span class="sxs-lookup"><span data-stu-id="7026b-141">To enable participation at any time, run `azure telemetry --enable`.</span></span>

## <a name="update-the-classic-cli"></a><span data-ttu-id="7026b-142">Mettre à jour l’interface de ligne de commande classique</span><span class="sxs-lookup"><span data-stu-id="7026b-142">Update the classic CLI</span></span>

<span data-ttu-id="7026b-143">Microsoft peut publier des versions mises à jour de l’interface de ligne de commande Azure CLI Classic.</span><span class="sxs-lookup"><span data-stu-id="7026b-143">Microsoft may release updated versions of the Azure classic CLI.</span></span> <span data-ttu-id="7026b-144">Réinstallez l’interface de ligne de commande classique à l’aide du programme d’installation pour votre système d’exploitation, ou exécutez le conteneur Docker le plus récent.</span><span class="sxs-lookup"><span data-stu-id="7026b-144">Reinstall the classic CLI using the installer for your operating system, or run the latest Docker container.</span></span> <span data-ttu-id="7026b-145">Cependant, si les dernières versions de Node.js et npm sont installées, procédez à la mise à jour en saisissant ce qui suit (dans les distributions Linux, vous devrez peut-être utiliser `sudo`).</span><span class="sxs-lookup"><span data-stu-id="7026b-145">Or, if you have the latest Node.js and npm installed, update by typing the following (on Linux distributions you might need to use `sudo`).</span></span>

```bash
npm update -g azure-cli
```

## <a name="enable-tab-completion"></a><span data-ttu-id="7026b-146">Activer la saisie semi-automatique via la touche Tab</span><span class="sxs-lookup"><span data-stu-id="7026b-146">Enable tab completion</span></span>

<span data-ttu-id="7026b-147">L’autocomplétion des commandes d’interface de ligne de commande classique est prise en charge pour Mac et Linux.</span><span class="sxs-lookup"><span data-stu-id="7026b-147">Tab completion of classic CLI commands is supported for Mac and Linux.</span></span>

<span data-ttu-id="7026b-148">Pour l’activer dans zsh, exécutez :</span><span class="sxs-lookup"><span data-stu-id="7026b-148">To enable it in zsh, run:</span></span>

```bash
echo '. <(azure --completion)' >> .zshrc
```

<span data-ttu-id="7026b-149">Pour l’activer dans bash, exécutez :</span><span class="sxs-lookup"><span data-stu-id="7026b-149">To enable it in bash, run:</span></span>

```bash
azure --completion >> ~/azure.completion.sh
echo 'source ~/azure.completion.sh' >> ~/.bash_profile
```

## <a name="next-steps"></a><span data-ttu-id="7026b-150">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="7026b-150">Next steps</span></span>

* <span data-ttu-id="7026b-151">Pour plus d'informations sur l'interface de ligne de commande Azure CLI Classic, téléchargez le code source, signalez des problèmes ou contribuez au projet, en consultant le [Référentiel GitHub pour l'interface de ligne de commande Azure CLI Classic](https://github.com/azure/azure-xplat-cli).</span><span class="sxs-lookup"><span data-stu-id="7026b-151">To learn more about the Azure classic CLI, download source code, report problems, or contribute to the project, visit the [GitHub repository for the Azure classic CLI](https://github.com/azure/azure-xplat-cli).</span></span>
