---
title: Installer Azure CLI 2.0
description: "Documents de référence pour l’installation de l’interface de ligne de commande Azure 2.0"
keywords: "Interface de ligne de commande Azure 2.0, Référence de l’interface de ligne de commande Azure 2.0, Installer l’interface de ligne de commande Azure 2.0, Interface de ligne de commande Azure Python, Désinstaller l’interface de ligne de commande Azure 2.0, l’interface de ligne de commande Azure, Installer l’interface de ligne de commande Azure, Référence de l’interface de ligne de commande Azure"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 08/17/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: ea5c0ee1-c530-4a1e-a83f-e1be71f6d416
ms.openlocfilehash: 00d5b555975007d7e57f04ce5d69f4f29e6d0219
ms.sourcegitcommit: f107cf927ea1ef51de181d87fc4bc078e9288e47
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/04/2017
---
# <a name="install-azure-cli-20"></a><span data-ttu-id="3d655-104">Installer Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="3d655-104">Install Azure CLI 2.0</span></span>

<span data-ttu-id="3d655-105">Installez la nouvelle version de l’interface de ligne de commande Azure dès aujourd’hui.</span><span class="sxs-lookup"><span data-stu-id="3d655-105">Install the new version of the Azure CLI today!</span></span>
<span data-ttu-id="3d655-106">Nous avons amélioré et mis à jour cette interface afin d’offrir une expérience de ligne de commande native d’exception pour la gestion des ressources Azure.</span><span class="sxs-lookup"><span data-stu-id="3d655-106">We've improved and updated it to provide a great native command-line experience for managing Azure resources.</span></span>
<span data-ttu-id="3d655-107">Elle peut être utilisée sur macOS, Linux et Windows.</span><span class="sxs-lookup"><span data-stu-id="3d655-107">It can be used on macOS, Linux, and Windows.</span></span>
<span data-ttu-id="3d655-108">Pour plus d’informations sur la version la plus récente, consultez les [Notes de publication](release-notes-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="3d655-108">For information about the latest release, see the [release notes](release-notes-azure-cli.md).</span></span>

> [!NOTE]
> <span data-ttu-id="3d655-109">Si vous devez utiliser la version précédente d’Azure CLI, voici comment [installer Azure 1.0](/azure/cli-install-nodejs).</span><span class="sxs-lookup"><span data-stu-id="3d655-109">If you need the previous version of the Azure CLI, here's how to [install Azure CLI 1.0](/azure/cli-install-nodejs).</span></span>

## <a name="a-namemacosinstall-on-macos"></a><span data-ttu-id="3d655-110"><a name="macOS"/>Installer sur macOS</span><span class="sxs-lookup"><span data-stu-id="3d655-110"><a name="macOS"/>Install on macOS</span></span>

1. <span data-ttu-id="3d655-111">Installer l’interface de ligne de commande Azure 2.0 avec `curl`.</span><span class="sxs-lookup"><span data-stu-id="3d655-111">Install Azure CLI 2.0 with `curl`.</span></span>

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

2. <span data-ttu-id="3d655-112">Vous devrez peut-être redémarrer votre interpréteur de commandes pour que certaines modifications soient prises en compte.</span><span class="sxs-lookup"><span data-stu-id="3d655-112">You may have to restart your shell for some changes to take effect.</span></span>

   ```bash
   exec -l $SHELL
   ```
   
3. <span data-ttu-id="3d655-113">Exécutez l’interface de ligne de commande Azure 2.0 à partir de l’invite de commandes avec la commande `az` .</span><span class="sxs-lookup"><span data-stu-id="3d655-113">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-on-windows"></a><span data-ttu-id="3d655-114">Installer sur Windows</span><span class="sxs-lookup"><span data-stu-id="3d655-114">Install on Windows</span></span>

<span data-ttu-id="3d655-115">Vous pouvez installer l’interface de ligne de commande Azure 2.0 avec le MSI et l’utiliser dans la ligne de commande Windows, ou vous pouvez installer la CLI avec `apt-get` sur Bash sous Ubuntu ou Windows.</span><span class="sxs-lookup"><span data-stu-id="3d655-115">You can install Azure CLI 2.0 with the MSI and use it in the Windows command-line, or you can install the CLI with `apt-get` on Bash on Ubuntu on Windows.</span></span>

### <a name="install-with-msi-for-the-windows-command-line"></a><span data-ttu-id="3d655-116">Installer avec MSI pour la ligne de commande Windows</span><span class="sxs-lookup"><span data-stu-id="3d655-116">Install with MSI for the Windows command-line</span></span> 

<span data-ttu-id="3d655-117">Pour installer l’interface de ligne de commande sous Windows et l’utiliser dans la ligne de commande Windows, téléchargez et exécutez le [MSI](https://aka.ms/InstallAzureCliWindows).</span><span class="sxs-lookup"><span data-stu-id="3d655-117">To install the CLI on Windows and use it in the Windows command-line, download and run the [MSI](https://aka.ms/InstallAzureCliWindows).</span></span>

### <a name="install-with-apt-get-for-bash-on-ubuntu-on-windows"></a><span data-ttu-id="3d655-118">Installer avec apt-get pour Bash sous Ubuntu ou Windows</span><span class="sxs-lookup"><span data-stu-id="3d655-118">Install with apt-get for Bash on Ubuntu on Windows</span></span>

1. <span data-ttu-id="3d655-119">Si vous ne disposez pas de Bash sur Windows, [installez-le](https://msdn.microsoft.com/commandline/wsl/install_guide).</span><span class="sxs-lookup"><span data-stu-id="3d655-119">If you don't have Bash on Windows, [install it](https://msdn.microsoft.com/commandline/wsl/install_guide).</span></span>

2. <span data-ttu-id="3d655-120">Ouvrez l’interpréteur de commandes Bash.</span><span class="sxs-lookup"><span data-stu-id="3d655-120">Open the Bash shell.</span></span>

3. <span data-ttu-id="3d655-121">Modifiez votre liste de sources.</span><span class="sxs-lookup"><span data-stu-id="3d655-121">Modify your sources list.</span></span>

   ```bash
   echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
   ```

4. <span data-ttu-id="3d655-122">Exécutez les commandes sudo suivantes :</span><span class="sxs-lookup"><span data-stu-id="3d655-122">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

5.  <span data-ttu-id="3d655-123">Exécutez l’interface de ligne de commande Azure 2.0 à partir de l’invite de commandes avec la commande `az` .</span><span class="sxs-lookup"><span data-stu-id="3d655-123">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-on-debianubuntu-with-apt-get"></a><span data-ttu-id="3d655-124">Installer sous Debian/Ubuntu avec apt-get</span><span class="sxs-lookup"><span data-stu-id="3d655-124">Install on Debian/Ubuntu with apt-get</span></span>

<span data-ttu-id="3d655-125">Dans le cas des systèmes Debian/Ubuntu, vous pouvez installer Azure CLI 2.0 par le biais de la commande `apt-get`.</span><span class="sxs-lookup"><span data-stu-id="3d655-125">For Debian/Ubuntu based systems, you can install Azure CLI 2.0 via `apt-get`.</span></span>

1. <span data-ttu-id="3d655-126">Modifiez votre liste de sources.</span><span class="sxs-lookup"><span data-stu-id="3d655-126">Modify your sources list.</span></span>
 
   - <span data-ttu-id="3d655-127">Système 32 bits</span><span class="sxs-lookup"><span data-stu-id="3d655-127">32-bit system</span></span>

     ```bash
     echo "deb https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

   - <span data-ttu-id="3d655-128">Système 64 bits</span><span class="sxs-lookup"><span data-stu-id="3d655-128">64-bit system</span></span>

     ```bash
     echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

2. <span data-ttu-id="3d655-129">Exécutez les commandes sudo suivantes :</span><span class="sxs-lookup"><span data-stu-id="3d655-129">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

3.  <span data-ttu-id="3d655-130">Exécutez l’interface de ligne de commande Azure 2.0 à partir de l’invite de commandes avec la commande `az` .</span><span class="sxs-lookup"><span data-stu-id="3d655-130">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-with-docker"></a><span data-ttu-id="3d655-131">Installer avec Docker</span><span class="sxs-lookup"><span data-stu-id="3d655-131">Install with Docker</span></span>

<span data-ttu-id="3d655-132">Nous fournissons une image Docker pré-configurée avec l’interface de ligne de commande Azure 2.0.</span><span class="sxs-lookup"><span data-stu-id="3d655-132">We maintain a Docker image preconfigured with the Azure CLI 2.0.</span></span>

<span data-ttu-id="3d655-133">Installez l’interface de ligne de commande à l’aide de `docker run`.</span><span class="sxs-lookup"><span data-stu-id="3d655-133">Install the CLI using `docker run`.</span></span>

  ```bash
  docker run azuresdk/azure-cli-python:<version>
  ```

<span data-ttu-id="3d655-134">Consultez nos [balises Docker](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/) pour connaître les versions disponibles.</span><span class="sxs-lookup"><span data-stu-id="3d655-134">See our [Docker tags](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/) for available versions.</span></span>

<span data-ttu-id="3d655-135">L’interface de ligne de commande est installé sur l’image en tant que commande `az` dans `/usr/local/bin`.</span><span class="sxs-lookup"><span data-stu-id="3d655-135">The CLI is installed on the image as the `az` command in `/usr/local/bin`.</span></span>

> [!NOTE]
> <span data-ttu-id="3d655-136">Si vous souhaitez sélectionner les clés SSH à partir de votre environnement utilisateur, vous pouvez utiliser `-v ${HOME}:/root` pour monter $HOME en tant que `/root`.</span><span class="sxs-lookup"><span data-stu-id="3d655-136">If you want to pick up the SSH keys from your user environment, you can use `-v ${HOME}:/root` to mount $HOME as `/root`.</span></span>

> ```bash
> docker run -v ${HOME}:/root azuresdk/azure-cli-python:<version>
> ```

## <a name="a-namelinuxinstall-on-linux-without-apt-get"></a><span data-ttu-id="3d655-137"><a name="Linux"/>Installer sous Linux sans apt-get</span><span class="sxs-lookup"><span data-stu-id="3d655-137"><a name="Linux"/>Install on Linux without apt-get</span></span>

<span data-ttu-id="3d655-138">Il est recommandé d’installer l’interface de ligne de commande avec `apt-get` si possible.</span><span class="sxs-lookup"><span data-stu-id="3d655-138">It is recommended that you install the CLI with `apt-get` if you are able to.</span></span> <span data-ttu-id="3d655-139">Pour les distributions qui n’utilisent pas le gestionnaire de package `apt`, vous pouvez installer manuellement.</span><span class="sxs-lookup"><span data-stu-id="3d655-139">For distributions which do not use the `apt` package manager, you can manually install.</span></span>

1. <span data-ttu-id="3d655-140">Installez les composants requis en fonction de votre distribution Linux.</span><span class="sxs-lookup"><span data-stu-id="3d655-140">Install the prerequisites based on your Linux distribution.</span></span>

   ```
   Platform              | Prerequisites
   ----------------------|---------------------------------------------
   Ubuntu 15.10 or 16.04 | sudo apt-get update && sudo apt-get install -y python libssl-dev libffi-dev python-dev build-essential
   Ubuntu 12.04 or 14.04 | sudo apt-get update && sudo apt-get install -y python libssl-dev libffi-dev python-dev
   Debian 8              | sudo apt-get update && sudo apt-get install -y python libssl-dev libffi-dev python-dev build-essential
   Debian 7              | sudo apt-get update && sudo apt-get install -y python libssl-dev libffi-dev python-dev
   CentOS 7.1 or 7.2     | sudo yum check-update; sudo yum install -y gcc python libffi-devel python-devel openssl-devel
   RedHat 7.2            | sudo yum check-update; sudo yum install -y gcc python libffi-devel python-devel openssl-devel
   SUSE OpenSUSE 13.2    | sudo zypper refresh && sudo zypper --non-interactive install curl gcc python python-xml libffi-devel python-devel openssl-devel
   ```

<span data-ttu-id="3d655-141">Si votre distribution ne figure pas ci-dessus, vous devez installer [Python](https://www.python.org/downloads/), [libffi](https://sourceware.org/libffi/), et [OpenSSL](https://www.openssl.org/source/).</span><span class="sxs-lookup"><span data-stu-id="3d655-141">If your distribution is not listed above, you will need to install [Python](https://www.python.org/downloads/), [libffi](https://sourceware.org/libffi/), and [OpenSSL](https://www.openssl.org/source/).</span></span>

2. <span data-ttu-id="3d655-142">Installez l’interface de ligne de commande à l’aide de `curl`.</span><span class="sxs-lookup"><span data-stu-id="3d655-142">Install the CLI with  `curl`.</span></span>

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

3. <span data-ttu-id="3d655-143">Vous devrez peut-être redémarrer votre interpréteur de commandes pour que certaines modifications soient prises en compte.</span><span class="sxs-lookup"><span data-stu-id="3d655-143">You may have to restart your shell for some changes to take effect.</span></span>

   ```bash
   exec -l $SHELL
   ```

4. <span data-ttu-id="3d655-144">Exécutez l’interface de ligne de commande Azure 2.0 à partir de l’invite de commandes avec la commande `az` .</span><span class="sxs-lookup"><span data-stu-id="3d655-144">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="3d655-145">Résolution des problèmes</span><span class="sxs-lookup"><span data-stu-id="3d655-145">Troubleshooting</span></span>

<span data-ttu-id="3d655-146">Si vous rencontrez un problème lors de l’installation de l’interface de ligne de commande, consultez cette section pour savoir si votre cas particulier est couvert.</span><span class="sxs-lookup"><span data-stu-id="3d655-146">If you encounter an issue during CLI install, check this section to see if your particular case is covered.</span></span> <span data-ttu-id="3d655-147">Si votre problème n’est pas ici, veuillez [signaler le problème lié à Github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="3d655-147">If your issue is not here, please [file a Github issue](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="curl-object-moved-error"></a><span data-ttu-id="3d655-148">erreur curl « Objet déplacé »</span><span class="sxs-lookup"><span data-stu-id="3d655-148">curl "Object Moved" error</span></span>

<span data-ttu-id="3d655-149">Si la commande `curl` renvoie une erreur concernant le `-L` paramètre ou un message d’erreur indiquant « Objet déplacé », essayez d’utiliser l’URL complète plutôt que la `aka.ms` redirection :</span><span class="sxs-lookup"><span data-stu-id="3d655-149">If you get an error from `curl` related to the `-L` parameter, or an error message including the text "Object Moved", try using the full URL instead of the `aka.ms` redirect:</span></span>

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

### <a name="homebrew-on-macos-installing-older-version"></a><span data-ttu-id="3d655-150">Installation d’une version antérieure de Homebrew sous macOS</span><span class="sxs-lookup"><span data-stu-id="3d655-150">Homebrew on macOS installing older version</span></span>

<span data-ttu-id="3d655-151">La formule de Homebrew `azure-cli` disponible pour macOS n’est pas à jour et installe une version 1.x de l’interface de ligne de commande.</span><span class="sxs-lookup"><span data-stu-id="3d655-151">The Homebrew `azure-cli` formula available for macOS is currently out of date, and will install a 1.x version of the CLI.</span></span> <span data-ttu-id="3d655-152">Vous pouvez vous tenir au courant de sa mise à jour en vérifiant `brew info azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="3d655-152">You can see when it is updated by checking `brew info azure-cli`.</span></span>

<span data-ttu-id="3d655-153">En attendant, [désinstallez l’ancienne version](#uninstall_brew) et suivez le [les instructions d’installation macOS](#macOS).</span><span class="sxs-lookup"><span data-stu-id="3d655-153">Until then, [uninstall the older version](#uninstall_brew) and follow the [macOS install instructions](#macOS).</span></span>

## <a name="uninstall-cli-1x-versions"></a><span data-ttu-id="3d655-154">Désinstaller les versions 1.x de l’interface de ligne de commande</span><span class="sxs-lookup"><span data-stu-id="3d655-154">Uninstall CLI 1.x versions</span></span>

<span data-ttu-id="3d655-155">Si vous votre système dispose d’une version 1.x antérieure de l’interface de ligne de commande, vous pouvez la désinstaller en fonction du type d’installation utilisé.</span><span class="sxs-lookup"><span data-stu-id="3d655-155">If you have an earlier CLI 1.x version available on your system, you can uninstall it based upon the type of install used.</span></span>

### <a name="uninstall-with-npm"></a><span data-ttu-id="3d655-156">Désinstaller avec npm</span><span class="sxs-lookup"><span data-stu-id="3d655-156">Uninstall with npm</span></span>

<span data-ttu-id="3d655-157">Supprimez l’ancienne interface de ligne de commande avec `npm uninstall`.</span><span class="sxs-lookup"><span data-stu-id="3d655-157">Remove the older CLI with `npm uninstall`.</span></span>

  ```bash
  npm uninstall -g azure-cli
  ```

### <a name="a-nameuninstallbrewuninstall-with-homebrew-on-macos"></a><span data-ttu-id="3d655-158"><a name="uninstall_brew"/>Désinstaller avec Homebrew sur macOS</span><span class="sxs-lookup"><span data-stu-id="3d655-158"><a name="uninstall_brew"/>Uninstall with Homebrew on macOS</span></span>

<span data-ttu-id="3d655-159">Supprimez l’ancienne interface de ligne de commande avec `brew uninstall`.</span><span class="sxs-lookup"><span data-stu-id="3d655-159">Remove the older CLI with `brew uninstall`.</span></span>

```bash
brew uninstall azure-cli
```

### <a name="uninstall-with-distributable"></a><span data-ttu-id="3d655-160">Désinstaller avec distribuable</span><span class="sxs-lookup"><span data-stu-id="3d655-160">Uninstall with distributable</span></span>

<span data-ttu-id="3d655-161">Si vous avez installé [MSI](http://aka.ms/webpi-azure-cli) ou un [package macOS](http://aka.ms/mac-azure-cli), utilisez le même outil pour supprimer votre installation.</span><span class="sxs-lookup"><span data-stu-id="3d655-161">If you installed via [MSI](http://aka.ms/webpi-azure-cli) or a [macOS package](http://aka.ms/mac-azure-cli), use the same tool to remove your install.</span></span>

### <a name="uninstall-with-docker"></a><span data-ttu-id="3d655-162">Désinstaller avec Docker</span><span class="sxs-lookup"><span data-stu-id="3d655-162">Uninstall with Docker</span></span>

<span data-ttu-id="3d655-163">Si vous avez installé une image Docker pour utiliser la version antérieure de l’interface de ligne de commande, supprimez cette image et tous les conteneurs associés.</span><span class="sxs-lookup"><span data-stu-id="3d655-163">If you installed a Docker image to use the earlier CLI version, remove that image and any associated containers.</span></span> <span data-ttu-id="3d655-164">Vous pouvez ensuite recréer les conteneurs après l’installation de la nouvelle image Docker comme décrit dans les instructions d’installation.</span><span class="sxs-lookup"><span data-stu-id="3d655-164">You can then re-create the containers after installing the new Docker image as described in the install instructions.</span></span>

  ```bash
  docker rmi -f microsoft/azure-cli
  ```

## <a name="update-the-cli"></a><span data-ttu-id="3d655-165">Mise à jour de l’interface CLI</span><span class="sxs-lookup"><span data-stu-id="3d655-165">Update the CLI</span></span>

<span data-ttu-id="3d655-166">Pour mettre à jour l’interface de ligne de commande Azure, utilisez la même méthode que vous avez utilisée pour l’installer.</span><span class="sxs-lookup"><span data-stu-id="3d655-166">To update the Azure CLI, use the same method that you used to install it.</span></span>

### <a name="update-with-msi"></a><span data-ttu-id="3d655-167">Mettre à jour avec MSI</span><span class="sxs-lookup"><span data-stu-id="3d655-167">Update with MSI</span></span>

<span data-ttu-id="3d655-168">Exécutez de nouveau le [MSI](https://aka.ms/InstallAzureCliWindows) .</span><span class="sxs-lookup"><span data-stu-id="3d655-168">Run the [MSI](https://aka.ms/InstallAzureCliWindows) again.</span></span>

### <a name="update-with-apt-get"></a><span data-ttu-id="3d655-169">Mettre à jour avec apt-get</span><span class="sxs-lookup"><span data-stu-id="3d655-169">Update with apt-get</span></span>

<span data-ttu-id="3d655-170">Utilisez `apt-get upgrade` pour mettre à jour le package de l’interface de ligne de commande.</span><span class="sxs-lookup"><span data-stu-id="3d655-170">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> <span data-ttu-id="3d655-171">Cela met à niveau tous les packages installés sur votre système n’ayant pas de modification de dépendance.</span><span class="sxs-lookup"><span data-stu-id="3d655-171">This will upgrade all of the installed packages on your system which have not had a dependency change.</span></span>
> <span data-ttu-id="3d655-172">Pour ne mettre à niveau que l’interface de ligne de commande, utilisez `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="3d655-172">To upgrade only the CLI, use `apt-get install`.</span></span>
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

### <a name="update-with-docker"></a><span data-ttu-id="3d655-173">Mettre à jour avec Docker</span><span class="sxs-lookup"><span data-stu-id="3d655-173">Update with Docker</span></span>

1. <span data-ttu-id="3d655-174">Mettre à jour votre image locale avec `docker pull`.</span><span class="sxs-lookup"><span data-stu-id="3d655-174">Update your local image with `docker pull`.</span></span>

   ```bash
   docker pull azuresdk/azure-cli-python
   ```

2. <span data-ttu-id="3d655-175">Obtenir les conteneurs qui utilisent actuellement l’image de l’interface de ligne de commande.</span><span class="sxs-lookup"><span data-stu-id="3d655-175">Get the containers currently using the CLI image.</span></span>

   ```bash
   docker container ls -a --filter 'ancestor=azuresdk/azure-cli-python'
   ```

   ```output
   CONTAINER ID        IMAGE                              COMMAND             CREATED             STATUS                        PORTS               NAMES
   34a868beb2ab        azuresdk/azure-cli-python:latest      "/bin/sh -c bash"   8 minutes ago       Exited (0) 8 minutes ago                       inspiring_benz
   ```

> [!NOTE]
> <span data-ttu-id="3d655-176">Si vous avez installé une version spécifique de l’image, vous devez ajouter `:<version>` à la fin du nom de l’image.</span><span class="sxs-lookup"><span data-stu-id="3d655-176">If you installed a specific version of the image, you will need to add `:<version>` to the end of the image name.</span></span>

3. <span data-ttu-id="3d655-177">Interrompre et recréer les conteneurs.</span><span class="sxs-lookup"><span data-stu-id="3d655-177">Halt and recreate the containers.</span></span>

   ```bash
   docker stop inspiring_benz
   docker rm inspiring_benz
   docker run azuresdk/azure-cli-python
   ```

### <a name="update-manually"></a><span data-ttu-id="3d655-178">Mettre à jour manuellement</span><span class="sxs-lookup"><span data-stu-id="3d655-178">Update manually</span></span>

<span data-ttu-id="3d655-179">Suivez les instructions d’installation manuelle de [macOS](#macOS) ou [Linux](#Linux) pour effectuer la mise à jour.</span><span class="sxs-lookup"><span data-stu-id="3d655-179">Follow the manual installation instructions for [macOS](#macOS) or [Linux](#Linux) to update.</span></span>

## <a name="uninstall"></a><span data-ttu-id="3d655-180">Désinstaller l’interface</span><span class="sxs-lookup"><span data-stu-id="3d655-180">Uninstall</span></span>

<span data-ttu-id="3d655-181">Si vous décidez de désinstaller l’interface de ligne de commande, nous sommes désolés de vous voir partir.</span><span class="sxs-lookup"><span data-stu-id="3d655-181">If you decide to uninstall the CLI, we're sorry to see you go.</span></span> <span data-ttu-id="3d655-182">Vous devez effectuer la désinstallation à l’aide de la même méthode que vous avez utilisée pour installer l’interface de ligne de commande.</span><span class="sxs-lookup"><span data-stu-id="3d655-182">You should uninstall using the same method that you used to install the CLI.</span></span>

### <a name="uninstall-with-msi"></a><span data-ttu-id="3d655-183">Désinstaller avec MSI</span><span class="sxs-lookup"><span data-stu-id="3d655-183">Uninstall with MSI</span></span>

<span data-ttu-id="3d655-184">Exécutez le [MSI](https://aka.ms/InstallAzureCliWindows) de nouveau et choisissez Désinstaller.</span><span class="sxs-lookup"><span data-stu-id="3d655-184">Run the [MSI](https://aka.ms/InstallAzureCliWindows) again and choose uninstall.</span></span>

### <a name="uninstall-with-apt-get"></a><span data-ttu-id="3d655-185">Désinstaller avec apt-get</span><span class="sxs-lookup"><span data-stu-id="3d655-185">Uninstall with apt-get</span></span>

<span data-ttu-id="3d655-186">Désinstallation via `apt-get remove`:</span><span class="sxs-lookup"><span data-stu-id="3d655-186">Uninstall via `apt-get remove`:</span></span>

  ```bash
  sudo apt-get remove -y azure-cli
  ```

### <a name="uninstall-with-docker"></a><span data-ttu-id="3d655-187">Désinstaller avec Docker</span><span class="sxs-lookup"><span data-stu-id="3d655-187">Uninstall with Docker</span></span>

<span data-ttu-id="3d655-188">Si vous avez installé une image docker, vous devez supprimer tous les conteneurs qui l’exécutent avant de supprimer l’image locale.</span><span class="sxs-lookup"><span data-stu-id="3d655-188">If you installed a docker image, you will need to remove any containers running it, and then delete the local image.</span></span>

1. <span data-ttu-id="3d655-189">Obtenez les conteneurs qui exécutent l’image de l’interface de ligne de commande Azure.</span><span class="sxs-lookup"><span data-stu-id="3d655-189">Get the containers which are running the azure-cli image.</span></span>

  ```bash
  docker container ls -a --filter 'ancestor=azuresdk/azure-cli-python'
  ```

  ```output
  CONTAINER ID        IMAGE                              COMMAND             CREATED             STATUS                        PORTS               NAMES
  34a868beb2ab        azuresdk/azure-cli-python:latest      "/bin/sh -c bash"   8 minutes ago       Exited (0) 8 minutes ago                       inspiring_benz
  ```

2. <span data-ttu-id="3d655-190">Supprimez tous les conteneurs avec l’image de l’interface de ligne de commande.</span><span class="sxs-lookup"><span data-stu-id="3d655-190">Delete any containers with the CLI image.</span></span>

  ```bash
  docker rm 34a868beb2ab
  ```

3. <span data-ttu-id="3d655-191">Supprimez l’image de l’interface de ligne de commande installée localement.</span><span class="sxs-lookup"><span data-stu-id="3d655-191">Remove the locally installed CLI image.</span></span>

  ```bash
  docker rmi azuresdk/azure-cli-python
  ```

> [!NOTE]
> <span data-ttu-id="3d655-192">Si vous avez installé une version spécifique de l’image, vous devez ajouter `:<version>` à la fin du nom de l’image.</span><span class="sxs-lookup"><span data-stu-id="3d655-192">If you installed a specific version of the image, you will need to add `:<version>` to the end of the image name.</span></span>

### <a name="uninstall-manually"></a><span data-ttu-id="3d655-193">Désinstaller manuellement</span><span class="sxs-lookup"><span data-stu-id="3d655-193">Uninstall manually</span></span>

<span data-ttu-id="3d655-194">Si vous avez installé l’interface de ligne de commande en utilisant le script accessible à l’adresse https://aka.ms/InstallAzureCli, vous pouvez désinstaller l’interface à l’aide de la procédure suivante.</span><span class="sxs-lookup"><span data-stu-id="3d655-194">If you used the script at https://aka.ms/InstallAzureCli to install the CLI, you can uninstall it with these steps.</span></span>

1. <span data-ttu-id="3d655-195">Supprimez les fichiers installés.</span><span class="sxs-lookup"><span data-stu-id="3d655-195">Remove the installed files.</span></span>

   ```bash
   rm -r <install location>/lib/azure-cli
   rm <install location>/bin/az
   ```

2. <span data-ttu-id="3d655-196">Supprimez la ligne `<install location>/lib/azure-cli/az.completion` de `<install location>/.bash_profile`.</span><span class="sxs-lookup"><span data-stu-id="3d655-196">Delete the line `<install location>/lib/azure-cli/az.completion` from `<install location>/.bash_profile`.</span></span>

> [!Note]
> <span data-ttu-id="3d655-197">L’emplacement d’installation par défaut est `/Users/<username>`.</span><span class="sxs-lookup"><span data-stu-id="3d655-197">The default install location is `/Users/<username>`.</span></span>

## <a name="report-cli-issues-and-feedback"></a><span data-ttu-id="3d655-198">Signaler des problèmes avec CLI et commentaires</span><span class="sxs-lookup"><span data-stu-id="3d655-198">Report CLI issues and feedback</span></span>

<span data-ttu-id="3d655-199">Si vous rencontrez des bogues en utilisant l’outil, signalez un problème dans la section [Problèmes](https://github.com/Azure/azure-cli/issues) de notre référentiel GitHub.</span><span class="sxs-lookup"><span data-stu-id="3d655-199">If you encounter any bugs with the tool, file an issue in the [Issues](https://github.com/Azure/azure-cli/issues) section of our GitHub repository.</span></span>
<span data-ttu-id="3d655-200">Pour fournir des commentaires à partir de la ligne de commande, utilisez la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="3d655-200">To provide feedback from the command line, use the `az feedback` command.</span></span>
