---
title: Installer l’interface de ligne de commande Azure CLI 1.0 | Documents Microsoft
description: Installation de l’interface de ligne de commande Azure CLI 1.0 pour Mac, Linux et Windows afin d’utiliser les services Azure
editor: ''
manager: timlt
documentationcenter: ''
author: squillace
services: virtual-machines-linux,virtual-network,storage,azure-resource-manager
tags: azure-resource-manager,azure-service-management
ms.assetid: bdb776c8-7a76-4f3a-887c-236b4fffee10
ms.service: multiple
ms.workload: multiple
ms.tgt_pltfrm: command-line-interface
ms.devlang: na
ms.topic: article
ms.date: 03/20/2017
ms.author: rasquill
ms.openlocfilehash: fa468a0b39b933b5778574a41aa29e0d60d050a8
ms.sourcegitcommit: d461e73abb09c3c85064c532b53a2efb25833b01
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/27/2018
---
# <a name="install-the-azure-cli-10"></a><span data-ttu-id="84eb4-103">Installer l’interface de ligne de commande Azure CLI 1.0</span><span class="sxs-lookup"><span data-stu-id="84eb4-103">Install the Azure CLI 1.0</span></span>

> [!IMPORTANT]
> <span data-ttu-id="84eb4-104">Cette rubrique décrit comment installer Azure CLI 1.0.</span><span class="sxs-lookup"><span data-stu-id="84eb4-104">This topic describes how to install the Azure CLI 1.0.</span></span> <span data-ttu-id="84eb4-105">Cette interface est dépréciée et doit être utilisée uniquement pour la prise en charge avec le modèle Azure Service Management (ASM) avec des ressources « classiques ».</span><span class="sxs-lookup"><span data-stu-id="84eb4-105">This CLI is deprecated and should only be used for support with the Azure Service Management (ASM) model with "classic" resources.</span></span>
> <span data-ttu-id="84eb4-106">Pour les déploiements Azure Resource Manager, utilisez [Azure CLI 2.0](/cli/azure).</span><span class="sxs-lookup"><span data-stu-id="84eb4-106">For Azure Resource Manager deployments, use [Azure CLI 2.0](/cli/azure).</span></span>

<span data-ttu-id="84eb4-107">Installez rapidement l’interface de ligne de commande Azure (Azure CLI 1.0) pour bénéficier d’un ensemble de commandes shell open source permettant de créer et de gérer les ressources dans Microsoft Azure.</span><span class="sxs-lookup"><span data-stu-id="84eb4-107">Quickly install the Azure Command-Line Interface (Azure CLI 1.0) to use a set of open-source shell-based commands for creating and managing resources in Microsoft Azure.</span></span> <span data-ttu-id="84eb4-108">Vous avez plusieurs options pour installer ces outils multiplateformes sur votre ordinateur :</span><span class="sxs-lookup"><span data-stu-id="84eb4-108">You have several options to install these cross-platform tools on your computer:</span></span>

* <span data-ttu-id="84eb4-109">**Package npm** : exécutez npm (le Gestionnaire de package de JavaScript) pour installer le dernier package de l’interface Azure CLI 1.0 sur votre système d’exploitation ou distribution Linux.</span><span class="sxs-lookup"><span data-stu-id="84eb4-109">**npm package** - Run npm (the package manager for JavaScript) to install the latest Azure CLI 1.0 package on your Linux distribution or OS.</span></span> <span data-ttu-id="84eb4-110">Requiert l’installation de node.js et npm sur votre ordinateur.</span><span class="sxs-lookup"><span data-stu-id="84eb4-110">Requires node.js and npm on your computer.</span></span>
* <span data-ttu-id="84eb4-111">**Programme d’installation** : téléchargez un programme d’installation pour une installation rapide sur Mac ou Windows.</span><span class="sxs-lookup"><span data-stu-id="84eb4-111">**Installer** - Download an installer for easy installation on Mac or Windows.</span></span>
* <span data-ttu-id="84eb4-112">**Conteneur Docker** : utilisez la dernière interface CLI dans un conteneur Docker prêt à s’exécuter.</span><span class="sxs-lookup"><span data-stu-id="84eb4-112">**Docker container** - Start using the latest CLI in a ready-to-run Docker container.</span></span> <span data-ttu-id="84eb4-113">Nécessite la présence d’un hôte Docker sur votre ordinateur.</span><span class="sxs-lookup"><span data-stu-id="84eb4-113">Requires Docker host on your computer.</span></span>

<span data-ttu-id="84eb4-114">Pour obtenir davantage d’options générales et de contexte, consultez le référentiel du projet sur [GitHub](https://github.com/azure/azure-xplat-cli).</span><span class="sxs-lookup"><span data-stu-id="84eb4-114">For more options and background, see the project repository on [GitHub](https://github.com/azure/azure-xplat-cli).</span></span>

<span data-ttu-id="84eb4-115">Une fois l’interface de ligne de commande Azure CLI 1.0 installée, [connectez-vous à l’aide de votre abonnement Azure](/cli/azure/authenticate-azure-cli) et exécutez les commandes **azure** depuis votre interface de ligne de commande (Bash, Terminal, invite de ligne de commande, etc.) pour travailler avec vos ressources Azure.</span><span class="sxs-lookup"><span data-stu-id="84eb4-115">Once the Azure CLI 1.0 is installed, [connect it with your Azure subscription](/cli/azure/authenticate-azure-cli) and run the **azure** commands from your command-line interface (Bash, Terminal, Command prompt, and so on) to work with your Azure resources.</span></span>

## <a name="option-1-install-an-npm-package"></a><span data-ttu-id="84eb4-116">Option 1 : Installer un package npm</span><span class="sxs-lookup"><span data-stu-id="84eb4-116">Option 1: Install an npm package</span></span>
<span data-ttu-id="84eb4-117">Pour installer l’interface CLI à partir d’un package npm, vérifiez que vous avez téléchargé et installé les [derniers fichiers Node.js et npm](https://nodejs.org/en/download/package-manager/).</span><span class="sxs-lookup"><span data-stu-id="84eb4-117">To install the CLI from an npm package, make sure you have downloaded and installed the [latest Node.js and npm](https://nodejs.org/en/download/package-manager/).</span></span> <span data-ttu-id="84eb4-118">Ensuite, exécutez **npm install** pour installer le package azure-cli :</span><span class="sxs-lookup"><span data-stu-id="84eb4-118">Then, run **npm install** to install the azure-cli package:</span></span>

```bash
npm install -g azure-cli
```

<span data-ttu-id="84eb4-119">Sur les distributions Linux, vous devrez peut-être utiliser **sudo** pour exécuter la commande **npm**, comme suit :</span><span class="sxs-lookup"><span data-stu-id="84eb4-119">On Linux distributions, you might need to use **sudo** to successfully run the **npm** command, as follows:</span></span>

```bash
sudo npm install -g azure-cli
```

> [!NOTE]
> <span data-ttu-id="84eb4-120">Si vous devez installer ou mettre à jour Node.js et npm sur votre distribution Linux ou votre système d’exploitation, nous vous recommandons d’installer la dernière version de Node.js LTS (4.x).</span><span class="sxs-lookup"><span data-stu-id="84eb4-120">If you need to install or update Node.js and npm on your Linux distribution or OS, we recommend that you install the most recent Node.js LTS version (4.x).</span></span> <span data-ttu-id="84eb4-121">Si vous utilisez une version antérieure, vous pouvez obtenir des erreurs d’installation.</span><span class="sxs-lookup"><span data-stu-id="84eb4-121">If you use an older version, you might get installation errors.</span></span>

<span data-ttu-id="84eb4-122">Si vous préférez, téléchargez le dernier [fichier tar][linux-installer] Linux pour le package npm en local.</span><span class="sxs-lookup"><span data-stu-id="84eb4-122">If you prefer, download the latest Linux [tar file][linux-installer] for the npm package locally.</span></span> <span data-ttu-id="84eb4-123">Ensuite, installez le package npm téléchargé comme suit (sur les distributions Linux vous devrez peut-être utiliser **sudo**) :</span><span class="sxs-lookup"><span data-stu-id="84eb4-123">Then, install the downloaded npm package as follows (on Linux distributions you might need to use **sudo**):</span></span>

```bash
npm install -g <path to downloaded tar file>
```

## <a name="option-2-use-an-installer"></a><span data-ttu-id="84eb4-124">Option 2 : Utiliser un programme d’installation</span><span class="sxs-lookup"><span data-stu-id="84eb4-124">Option 2: Use an installer</span></span>
<span data-ttu-id="84eb4-125">Si vous utilisez un ordinateur Mac ou Windows, les programmes d’installation de l’interface CLI suivants sont disponibles au téléchargement :</span><span class="sxs-lookup"><span data-stu-id="84eb4-125">If you use a Mac or Windows computer, the following CLI installers are available for download:</span></span>

* <span data-ttu-id="84eb4-126">[Programme d’installation Mac OS X][mac-installer]</span><span class="sxs-lookup"><span data-stu-id="84eb4-126">[Mac OS X installer][mac-installer]</span></span>
* <span data-ttu-id="84eb4-127">[MSI Windows][windows-installer]</span><span class="sxs-lookup"><span data-stu-id="84eb4-127">[Windows MSI][windows-installer]</span></span>

> [!TIP]
> <span data-ttu-id="84eb4-128">Sous Windows, vous pouvez également télécharger [Web Platform Installer](https://go.microsoft.com/?linkid=9828653) pour installer l’interface CLI.</span><span class="sxs-lookup"><span data-stu-id="84eb4-128">On Windows, you can also download the [Web Platform Installer](https://go.microsoft.com/?linkid=9828653) to install the CLI.</span></span> <span data-ttu-id="84eb4-129">Ce programme d’installation vous donne la possibilité d’installer des Kits de développement logiciel (SDK) Azure et des outils de ligne de commande supplémentaires après l’installation de l’interface CLI.</span><span class="sxs-lookup"><span data-stu-id="84eb4-129">This installer gives you the option to install additional Azure SDK and command-line tools after installing the CLI.</span></span>

## <a name="option-3-use-a-docker-container"></a><span data-ttu-id="84eb4-130">Option 3 : Utiliser un conteneur Docker</span><span class="sxs-lookup"><span data-stu-id="84eb4-130">Option 3: Use a Docker container</span></span>
<span data-ttu-id="84eb4-131">Si vous avez configuré votre ordinateur comme hôte [Docker](https://docs.docker.com/engine/understanding-docker/) , vous pouvez exécuter la dernière interface de ligne de commande Azure CLI 1.0 dans un conteneur Docker.</span><span class="sxs-lookup"><span data-stu-id="84eb4-131">If you have set up your computer as a [Docker](https://docs.docker.com/engine/understanding-docker/) host, you can run the latest Azure CLI 1.0 in a Docker container.</span></span> <span data-ttu-id="84eb4-132">Exécutez la commande suivante (sur les distributions Linux, vous devrez peut-être utiliser **sudo**.) :</span><span class="sxs-lookup"><span data-stu-id="84eb4-132">Run the following command (on Linux distributions you might need to use **sudo**):</span></span>

```bash
docker run -it microsoft/azure-cli:0.10.17
```

## <a name="run-azure-cli-10-commands"></a><span data-ttu-id="84eb4-133">Exécution des commandes Azure CLI 1.0</span><span class="sxs-lookup"><span data-stu-id="84eb4-133">Run Azure CLI 1.0 commands</span></span>
<span data-ttu-id="84eb4-134">Une fois l’interface de ligne de commande Azure CLI 1.0 installée, exécutez la commande **azure** depuis l’interface de ligne de commande utilisateur (Bash, Terminal, invite de ligne de commande, etc.).</span><span class="sxs-lookup"><span data-stu-id="84eb4-134">After the Azure CLI 1.0 is installed, run the **azure** command from your command-line user interface (Bash, Terminal, Command prompt, and so on).</span></span> <span data-ttu-id="84eb4-135">Par exemple, pour exécuter la commande d’aide, saisissez ce qui suit :</span><span class="sxs-lookup"><span data-stu-id="84eb4-135">For example, to run the help command, type the following:</span></span>

```azurecli
azure help
```

> [!NOTE]
> <span data-ttu-id="84eb4-136">Dans certaines distributions Linux, vous pouvez recevoir une erreur similaire à `/usr/bin/env: ‘node’: No such file or directory`.</span><span class="sxs-lookup"><span data-stu-id="84eb4-136">On some Linux distributions, you may receive an error similar to `/usr/bin/env: ‘node’: No such file or directory`.</span></span> <span data-ttu-id="84eb4-137">Cette erreur est due à l’installation récente de Node.js sous /usr/bin/nodejs.</span><span class="sxs-lookup"><span data-stu-id="84eb4-137">This error comes from recent installations of Node.js being installed at /usr/bin/nodejs.</span></span> <span data-ttu-id="84eb4-138">Pour la corriger, créez un lien symbolique vers /usr/bin/node en exécutant cette commande :</span><span class="sxs-lookup"><span data-stu-id="84eb4-138">To fix it, create a symbolic link to /usr/bin/node by running this command:</span></span>

```bash
sudo ln -s /usr/bin/nodejs /usr/bin/node
```

<span data-ttu-id="84eb4-139">Pour afficher la version de l’interface Azure CLI 1.0 que vous avez installée, saisissez la commande suivante :</span><span class="sxs-lookup"><span data-stu-id="84eb4-139">To see the version of the Azure CLI 1.0 you installed, type the following:</span></span>

```azurecli
azure --version
```

<span data-ttu-id="84eb4-140">Vous avez terminé l’installation.</span><span class="sxs-lookup"><span data-stu-id="84eb4-140">Now you are ready!</span></span> <span data-ttu-id="84eb4-141">Pour accéder à toutes les commandes de l’interface de ligne de commande et travailler avec vos propres ressources, [connectez-vous à votre abonnement Azure à partir de l’interface de ligne de commande Azure](/cli/azure/authenticate-azure-cli).</span><span class="sxs-lookup"><span data-stu-id="84eb4-141">To access all the CLI commands to work with your own resources, [connect to your Azure subscription from the Azure CLI](/cli/azure/authenticate-azure-cli).</span></span>

> [!NOTE]
> <span data-ttu-id="84eb4-142">Lorsque vous utilisez l’interface de ligne de commande Azure pour la première fois, vous voyez un message vous demandant si vous souhaitez autoriser Microsoft à recueillir des informations d’utilisation.</span><span class="sxs-lookup"><span data-stu-id="84eb4-142">When you first use Azure CLI, you see a message asking if you want to allow Microsoft to collect usage information.</span></span> <span data-ttu-id="84eb4-143">La participation se fait sur la base du volontariat.</span><span class="sxs-lookup"><span data-stu-id="84eb4-143">Participation is voluntary.</span></span> <span data-ttu-id="84eb4-144">Si vous choisissez de participer, vous pouvez arrêter à tout moment en exécutant `azure telemetry --disable`.</span><span class="sxs-lookup"><span data-stu-id="84eb4-144">If you choose to participate, you can stop at any time by running `azure telemetry --disable`.</span></span> <span data-ttu-id="84eb4-145">Pour activer la participation, exécutez `azure telemetry --enable`.</span><span class="sxs-lookup"><span data-stu-id="84eb4-145">To enable participation at any time, run `azure telemetry --enable`.</span></span>

## <a name="update-the-cli"></a><span data-ttu-id="84eb4-146">Mise à jour de l’interface CLI</span><span class="sxs-lookup"><span data-stu-id="84eb4-146">Update the CLI</span></span>
<span data-ttu-id="84eb4-147">Microsoft publie fréquemment des versions mises à jour de l’interface CLI Azure.</span><span class="sxs-lookup"><span data-stu-id="84eb4-147">Microsoft frequently releases updated versions of the Azure CLI.</span></span> <span data-ttu-id="84eb4-148">Réinstallez l’interface CLI à l’aide du programme d’installation pour votre système d’exploitation, ou exécutez le dernier conteneur Docker.</span><span class="sxs-lookup"><span data-stu-id="84eb4-148">Reinstall the CLI using the installer for your operating system, or run the latest Docker container.</span></span> <span data-ttu-id="84eb4-149">Alternativement, si les dernières versions de Node.js et npm sont installées, procédez à la mise à jour en saisissant ce qui suit (dans les distributions Linux, vous devrez peut-être utiliser **sudo**).</span><span class="sxs-lookup"><span data-stu-id="84eb4-149">Or, if you have the latest Node.js and npm installed, update by typing the following (on Linux distributions you might need to use **sudo**).</span></span>

```bash
npm update -g azure-cli
```

## <a name="enable-tab-completion"></a><span data-ttu-id="84eb4-150">Activer la saisie semi-automatique via la touche Tab</span><span class="sxs-lookup"><span data-stu-id="84eb4-150">Enable tab completion</span></span>
<span data-ttu-id="84eb4-151">La saisie semi-automatique via la touche Tab des commandes CLI est prise en charge pour Mac et Linux.</span><span class="sxs-lookup"><span data-stu-id="84eb4-151">Tab completion of CLI commands is supported for Mac and Linux.</span></span>

<span data-ttu-id="84eb4-152">Pour l’activer dans zsh, exécutez :</span><span class="sxs-lookup"><span data-stu-id="84eb4-152">To enable it in zsh, run:</span></span>

```bash
echo '. <(azure --completion)' >> .zshrc
```

<span data-ttu-id="84eb4-153">Pour l’activer dans bash, exécutez :</span><span class="sxs-lookup"><span data-stu-id="84eb4-153">To enable it in bash, run:</span></span>

```bash
azure --completion >> ~/azure.completion.sh
echo 'source ~/azure.completion.sh' >> ~/.bash_profile
```


## <a name="next-steps"></a><span data-ttu-id="84eb4-154">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="84eb4-154">Next steps</span></span>
* <span data-ttu-id="84eb4-155">[Se connecter à partir de l’interface de ligne de commande à votre abonnement Azure](/cli/azure/authenticate-azure-cli) pour créer et gérer des ressources Azure.</span><span class="sxs-lookup"><span data-stu-id="84eb4-155">[Connect from the CLI to your Azure subscription](/cli/azure/authenticate-azure-cli) to create and manage Azure resources.</span></span>
* <span data-ttu-id="84eb4-156">Pour plus d'informations sur l'interface de ligne de commande Azure, télécharger un code source, signaler des problèmes ou contribuer au projet, voir [Référentiel GitHub pour l'interface de ligne de commande Azure](https://github.com/azure/azure-xplat-cli)(en anglais).</span><span class="sxs-lookup"><span data-stu-id="84eb4-156">To learn more about the Azure CLI, download source code, report problems, or contribute to the project, visit the [GitHub repository for the Azure CLI](https://github.com/azure/azure-xplat-cli).</span></span>
* <span data-ttu-id="84eb4-157">Si vous avez des questions sur l’utilisation de l’interface de ligne de commande Azure ou sur l’utilisation d’Azure, consultez les [forums Azure](https://social.msdn.microsoft.com/Forums/en-US/home?forum=azurescripting).</span><span class="sxs-lookup"><span data-stu-id="84eb4-157">If you have questions about using the Azure CLI, or Azure, visit the [Azure Forums](https://social.msdn.microsoft.com/Forums/en-US/home?forum=azurescripting).</span></span>


[mac-installer]: http://aka.ms/mac-azure-cli
[windows-installer]: http://aka.ms/webpi-azure-cli
[linux-installer]: http://aka.ms/linux-azure-cli
[cliasm]: /cli/azure/get-started-with-az-cli2
[cliarm]: ./virtual-machines/azure-cli-arm-commands.md
