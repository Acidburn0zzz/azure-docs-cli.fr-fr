---
title: Installer Azure CLI 2.0
description: "Documents de référence pour l’installation de l’interface de ligne de commande Azure 2.0"
keywords: "Azure CLI, Installer Azure CLI, Azure Python CLI, Référence sur Azure CLI"
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
ms.openlocfilehash: 580438bfc66f3ed0b4dad504258eab453b1b9183
ms.sourcegitcommit: c1df7794ad42adb8640b51b630e4275f4a791ac2
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/19/2017
---
# <a name="install-azure-cli-20"></a><span data-ttu-id="8cab4-104">Installer Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="8cab4-104">Install Azure CLI 2.0</span></span>

<span data-ttu-id="8cab4-105">Installez la nouvelle version de l’interface de ligne de commande Azure dès aujourd’hui.</span><span class="sxs-lookup"><span data-stu-id="8cab4-105">Install the new version of the Azure CLI today!</span></span>
<span data-ttu-id="8cab4-106">Nous avons amélioré et mis à jour cette interface afin d’offrir une expérience de ligne de commande native d’exception pour la gestion des ressources Azure.</span><span class="sxs-lookup"><span data-stu-id="8cab4-106">We've improved and updated it to provide a great native command-line experience for managing Azure resources.</span></span>
<span data-ttu-id="8cab4-107">Elle peut être utilisée sur macOS, Linux et Windows.</span><span class="sxs-lookup"><span data-stu-id="8cab4-107">It can be used on macOS, Linux, and Windows.</span></span>
<span data-ttu-id="8cab4-108">Pour plus d’informations sur la version la plus récente, consultez les [Notes de publication](release-notes-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="8cab4-108">For information about the latest release, see the [release notes](release-notes-azure-cli.md).</span></span>

> [!NOTE]
> <span data-ttu-id="8cab4-109">Si vous devez utiliser la version précédente d’Azure CLI, voici comment [installer Azure 1.0](/azure/cli-install-nodejs).</span><span class="sxs-lookup"><span data-stu-id="8cab4-109">If you need the previous version of the Azure CLI, here's how to [install Azure CLI 1.0](/azure/cli-install-nodejs).</span></span>

## <a name="a-namemacosinstall-on-macos"></a><span data-ttu-id="8cab4-110"><a name="macOS"/>Installer sur macOS</span><span class="sxs-lookup"><span data-stu-id="8cab4-110"><a name="macOS"/>Install on macOS</span></span>

<span data-ttu-id="8cab4-111">Sur macOS, vous avez le choix de procéder à l’installation avec [Homebrew](https://brew.sh/) ou manuellement.</span><span class="sxs-lookup"><span data-stu-id="8cab4-111">On macOS, you are able to install either with [Homebrew](https://brew.sh/) or manually.</span></span>

### <a name="install-with-homebrew"></a><span data-ttu-id="8cab4-112">Désinstaller avec Homebrew</span><span class="sxs-lookup"><span data-stu-id="8cab4-112">Install with Homebrew</span></span>

1. <span data-ttu-id="8cab4-113">Si vous ne l’avez pas encore, installez Homebrew en suivant les [instructions d’installation pour Homebrew](https://docs.brew.sh/Installation.html).</span><span class="sxs-lookup"><span data-stu-id="8cab4-113">If you don't have it already, install Homebrew by following the [Homebrew installation instructions](https://docs.brew.sh/Installation.html).</span></span>

2. <span data-ttu-id="8cab4-114">Mettez à jour vos référentiels Homebrew locaux.</span><span class="sxs-lookup"><span data-stu-id="8cab4-114">Update your local Homebrew repositories.</span></span>

   ```bash
   brew update
   ```

3. <span data-ttu-id="8cab4-115">Installez le package `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="8cab4-115">Install the `azure-cli` package.</span></span>

  ```bash
  brew install azure-cli
  ```

> [!NOTE]
> <span data-ttu-id="8cab4-116">Si vous avez installé Azure CLI 1.0 avec Homebrew au préalable, au lieu d’installer le package, vous pouvez obtenir CLI 2.0 grâce au processus normal de mise à niveau Homebrew.</span><span class="sxs-lookup"><span data-stu-id="8cab4-116">If you previously installed the Azure CLI 1.0 with Homebrew, instead of installing the package you can get CLI 2.0 through the regular Homebrew upgrade process.</span></span>
>
> ```bash
> brew upgrade
> ```

### <a name="install-manually"></a><span data-ttu-id="8cab4-117">Installer manuellement</span><span class="sxs-lookup"><span data-stu-id="8cab4-117">Install manually</span></span>

1. <span data-ttu-id="8cab4-118">Installer l’interface de ligne de commande Azure 2.0 avec `curl`.</span><span class="sxs-lookup"><span data-stu-id="8cab4-118">Install Azure CLI 2.0 with `curl`.</span></span>

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

2. <span data-ttu-id="8cab4-119">Vous devrez peut-être redémarrer votre interpréteur de commandes pour que certaines modifications soient prises en compte.</span><span class="sxs-lookup"><span data-stu-id="8cab4-119">You may have to restart your shell for some changes to take effect.</span></span>

   ```bash
   exec -l $SHELL
   ```
   
3. <span data-ttu-id="8cab4-120">Exécutez l’interface de ligne de commande Azure 2.0 à partir de l’invite de commandes avec la commande `az` .</span><span class="sxs-lookup"><span data-stu-id="8cab4-120">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-on-windows"></a><span data-ttu-id="8cab4-121">Installer sur Windows</span><span class="sxs-lookup"><span data-stu-id="8cab4-121">Install on Windows</span></span>

<span data-ttu-id="8cab4-122">Vous pouvez installer l’interface de ligne de commande Azure 2.0 avec le MSI et l’utiliser dans la ligne de commande Windows, ou vous pouvez installer la CLI avec `apt-get` sur Bash sous Ubuntu ou Windows.</span><span class="sxs-lookup"><span data-stu-id="8cab4-122">You can install Azure CLI 2.0 with the MSI and use it in the Windows command-line, or you can install the CLI with `apt-get` on Bash on Ubuntu on Windows.</span></span>

### <a name="install-with-msi-for-the-windows-command-line"></a><span data-ttu-id="8cab4-123">Installer avec MSI pour la ligne de commande Windows</span><span class="sxs-lookup"><span data-stu-id="8cab4-123">Install with MSI for the Windows command-line</span></span> 

<span data-ttu-id="8cab4-124">Pour installer l’interface de ligne de commande sous Windows et l’utiliser dans la ligne de commande Windows, téléchargez et exécutez le [MSI](https://aka.ms/InstallAzureCliWindows).</span><span class="sxs-lookup"><span data-stu-id="8cab4-124">To install the CLI on Windows and use it in the Windows command-line, download and run the [MSI](https://aka.ms/InstallAzureCliWindows).</span></span>

### <a name="install-with-apt-get-for-bash-on-ubuntu-on-windows"></a><span data-ttu-id="8cab4-125">Installer avec apt-get pour Bash sous Ubuntu ou Windows</span><span class="sxs-lookup"><span data-stu-id="8cab4-125">Install with apt-get for Bash on Ubuntu on Windows</span></span>

1. <span data-ttu-id="8cab4-126">Si vous ne disposez pas de Bash sur Windows, [installez-le](https://msdn.microsoft.com/commandline/wsl/install_guide).</span><span class="sxs-lookup"><span data-stu-id="8cab4-126">If you don't have Bash on Windows, [install it](https://msdn.microsoft.com/commandline/wsl/install_guide).</span></span>

2. <span data-ttu-id="8cab4-127">Ouvrez l’interpréteur de commandes Bash.</span><span class="sxs-lookup"><span data-stu-id="8cab4-127">Open the Bash shell.</span></span>

3. <span data-ttu-id="8cab4-128">Modifiez votre liste de sources.</span><span class="sxs-lookup"><span data-stu-id="8cab4-128">Modify your sources list.</span></span>

   ```bash
   echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
   ```

4. <span data-ttu-id="8cab4-129">Exécutez les commandes sudo suivantes :</span><span class="sxs-lookup"><span data-stu-id="8cab4-129">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

5.  <span data-ttu-id="8cab4-130">Exécutez l’interface de ligne de commande Azure 2.0 à partir de l’invite de commandes avec la commande `az` .</span><span class="sxs-lookup"><span data-stu-id="8cab4-130">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-on-debianubuntu-with-apt-get"></a><span data-ttu-id="8cab4-131">Installer sous Debian/Ubuntu avec apt-get</span><span class="sxs-lookup"><span data-stu-id="8cab4-131">Install on Debian/Ubuntu with apt-get</span></span>

<span data-ttu-id="8cab4-132">Dans le cas des systèmes Debian/Ubuntu, vous pouvez installer Azure CLI 2.0 par le biais de la commande `apt-get`.</span><span class="sxs-lookup"><span data-stu-id="8cab4-132">For Debian/Ubuntu based systems, you can install Azure CLI 2.0 via `apt-get`.</span></span>

1. <span data-ttu-id="8cab4-133">Modifiez votre liste de sources :</span><span class="sxs-lookup"><span data-stu-id="8cab4-133">Modify your sources list:</span></span>
 
   - <span data-ttu-id="8cab4-134">Système 32 bits</span><span class="sxs-lookup"><span data-stu-id="8cab4-134">32-bit system</span></span>

     ```bash
     echo "deb https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

   - <span data-ttu-id="8cab4-135">Système 64 bits</span><span class="sxs-lookup"><span data-stu-id="8cab4-135">64-bit system</span></span>

     ```bash
     echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

2. <span data-ttu-id="8cab4-136">Exécutez les commandes sudo suivantes :</span><span class="sxs-lookup"><span data-stu-id="8cab4-136">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

3.  <span data-ttu-id="8cab4-137">Exécutez l’interface de ligne de commande Azure 2.0 à partir de l’invite de commandes avec la commande `az` .</span><span class="sxs-lookup"><span data-stu-id="8cab4-137">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-on-rhel-fedora-and-centos-with-yum"></a><span data-ttu-id="8cab4-138">Installer sur RHEL, Fedora et CentOS avec yum</span><span class="sxs-lookup"><span data-stu-id="8cab4-138">Install on RHEL, Fedora, and CentOS with yum</span></span>

<span data-ttu-id="8cab4-139">Pour une distribution basée sur RedHat et qui contient le gestionnaire de package `yum`, vous pouvez installer Azure CLI 2.0 via `yum`.</span><span class="sxs-lookup"><span data-stu-id="8cab4-139">For any distribution which is based off of RedHat and contains the `yum` package manager, you can install Azure CLI 2.0 via `yum`.</span></span>

1. <span data-ttu-id="8cab4-140">Importer la clé de référentiel Microsoft :</span><span class="sxs-lookup"><span data-stu-id="8cab4-140">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. <span data-ttu-id="8cab4-141">Créer des informations de référentiel `azure-cli` locales :</span><span class="sxs-lookup"><span data-stu-id="8cab4-141">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/azure-cli.repo'
   ```

3. <span data-ttu-id="8cab4-142">Mettre à jour l’index de package `yum` et l’installer :</span><span class="sxs-lookup"><span data-stu-id="8cab4-142">Update the `yum` package index and install:</span></span>

   ```bash
   yum check-update
   sudo yum install azure-cli
   ```

4. <span data-ttu-id="8cab4-143">Exécutez l’interface de ligne de commande Azure 2.0 à partir de l’invite de commandes avec la commande `az` .</span><span class="sxs-lookup"><span data-stu-id="8cab4-143">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-on-opensuse-and-sle-with-zypper"></a><span data-ttu-id="8cab4-144">Installer sur openSUSE et SLE avec zypper</span><span class="sxs-lookup"><span data-stu-id="8cab4-144">Install on openSUSE and SLE with zypper</span></span>

1. <span data-ttu-id="8cab4-145">Importer la clé de référentiel Microsoft :</span><span class="sxs-lookup"><span data-stu-id="8cab4-145">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. <span data-ttu-id="8cab4-146">Créer des informations de référentiel `azure-cli` locales :</span><span class="sxs-lookup"><span data-stu-id="8cab4-146">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ntype=rpm-md\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/zypp/repos.d/azure-cli.repo'
   ```

3. <span data-ttu-id="8cab4-147">Mettre à jour l’index de package `zypper` et l’installer :</span><span class="sxs-lookup"><span data-stu-id="8cab4-147">Update the `zypper` package index and install:</span></span>

   ```bash
   sudo zypper refresh
   sudo zypper install azure-cli
   ```

4. <span data-ttu-id="8cab4-148">Exécutez l’interface de ligne de commande Azure 2.0 à partir de l’invite de commandes avec la commande `az` .</span><span class="sxs-lookup"><span data-stu-id="8cab4-148">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-with-docker"></a><span data-ttu-id="8cab4-149">Installer avec Docker</span><span class="sxs-lookup"><span data-stu-id="8cab4-149">Install with Docker</span></span>

<span data-ttu-id="8cab4-150">Nous fournissons une image Docker pré-configurée avec l’interface de ligne de commande Azure 2.0.</span><span class="sxs-lookup"><span data-stu-id="8cab4-150">We maintain a Docker image preconfigured with the Azure CLI 2.0.</span></span>

<span data-ttu-id="8cab4-151">Installez l’interface de ligne de commande à l’aide de `docker run`.</span><span class="sxs-lookup"><span data-stu-id="8cab4-151">Install the CLI using `docker run`.</span></span>

   ```bash
   docker run azuresdk/azure-cli-python:<version>
   ```

<span data-ttu-id="8cab4-152">Consultez nos [balises Docker](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/) pour connaître les versions disponibles.</span><span class="sxs-lookup"><span data-stu-id="8cab4-152">See our [Docker tags](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/) for available versions.</span></span>

<span data-ttu-id="8cab4-153">L’interface de ligne de commande est installé sur l’image en tant que commande `az` dans `/usr/local/bin`.</span><span class="sxs-lookup"><span data-stu-id="8cab4-153">The CLI is installed on the image as the `az` command in `/usr/local/bin`.</span></span>

> [!NOTE]
> <span data-ttu-id="8cab4-154">Si vous souhaitez sélectionner les clés SSH à partir de votre environnement utilisateur, vous pouvez utiliser `-v ${HOME}:/root` pour monter $HOME en tant que `/root`.</span><span class="sxs-lookup"><span data-stu-id="8cab4-154">If you want to pick up the SSH keys from your user environment, you can use `-v ${HOME}:/root` to mount $HOME as `/root`.</span></span>

> ```bash
> docker run -v ${HOME}:/root azuresdk/azure-cli-python:<version>
> ```

## <a name="a-namelinuxinstall-on-linux-without-apt-get"></a><span data-ttu-id="8cab4-155"><a name="Linux"/>Installer sous Linux sans apt-get</span><span class="sxs-lookup"><span data-stu-id="8cab4-155"><a name="Linux"/>Install on Linux without apt-get</span></span>

<span data-ttu-id="8cab4-156">Il est recommandé d’installer l’interface de ligne de commande avec un gestionnaire de package si possible.</span><span class="sxs-lookup"><span data-stu-id="8cab4-156">It is recommended that you install the CLI with a package manager if you are able to.</span></span> <span data-ttu-id="8cab4-157">Pour les distributions ne disposant pas de gestionnaire de package, vous pouvez procéder à une installation manuelle.</span><span class="sxs-lookup"><span data-stu-id="8cab4-157">For distributions which do not have a package provided for them, you can manually install.</span></span>

1. <span data-ttu-id="8cab4-158">Installez les composants requis en fonction de votre distribution Linux.</span><span class="sxs-lookup"><span data-stu-id="8cab4-158">Install the prerequisites based on your Linux distribution.</span></span>

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

<span data-ttu-id="8cab4-159">Si votre distribution ne figure pas ci-dessus, vous devez installer [Python](https://www.python.org/downloads/), [libffi](https://sourceware.org/libffi/), et [OpenSSL](https://www.openssl.org/source/).</span><span class="sxs-lookup"><span data-stu-id="8cab4-159">If your distribution is not listed above, you will need to install [Python](https://www.python.org/downloads/), [libffi](https://sourceware.org/libffi/), and [OpenSSL](https://www.openssl.org/source/).</span></span>

2. <span data-ttu-id="8cab4-160">Installez l’interface de ligne de commande à l’aide de `curl`.</span><span class="sxs-lookup"><span data-stu-id="8cab4-160">Install the CLI with  `curl`.</span></span>

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

3. <span data-ttu-id="8cab4-161">Vous devrez peut-être redémarrer votre interpréteur de commandes pour que certaines modifications soient prises en compte.</span><span class="sxs-lookup"><span data-stu-id="8cab4-161">You may have to restart your shell for some changes to take effect.</span></span>

   ```bash
   exec -l $SHELL
   ```

4. <span data-ttu-id="8cab4-162">Exécutez l’interface de ligne de commande Azure 2.0 à partir de l’invite de commandes avec la commande `az` .</span><span class="sxs-lookup"><span data-stu-id="8cab4-162">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="8cab4-163">Résolution des problèmes</span><span class="sxs-lookup"><span data-stu-id="8cab4-163">Troubleshooting</span></span>

<span data-ttu-id="8cab4-164">Si vous rencontrez un problème lors de l’installation de l’interface de ligne de commande, consultez cette section pour savoir si votre cas particulier est couvert.</span><span class="sxs-lookup"><span data-stu-id="8cab4-164">If you encounter an issue during CLI install, check this section to see if your particular case is covered.</span></span> <span data-ttu-id="8cab4-165">Si votre problème n’est pas ici, veuillez [signaler le problème lié à Github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="8cab4-165">If your issue is not here, please [file a Github issue](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="curl-object-moved-error"></a><span data-ttu-id="8cab4-166">erreur curl « Objet déplacé »</span><span class="sxs-lookup"><span data-stu-id="8cab4-166">curl "Object Moved" error</span></span>

<span data-ttu-id="8cab4-167">Si la commande `curl` renvoie une erreur concernant le `-L` paramètre ou un message d’erreur indiquant « Objet déplacé », essayez d’utiliser l’URL complète plutôt que la `aka.ms` redirection :</span><span class="sxs-lookup"><span data-stu-id="8cab4-167">If you get an error from `curl` related to the `-L` parameter, or an error message including the text "Object Moved", try using the full URL instead of the `aka.ms` redirect:</span></span>

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

## <a name="uninstall-cli-1x-versions"></a><span data-ttu-id="8cab4-168">Désinstaller les versions 1.x de l’interface de ligne de commande</span><span class="sxs-lookup"><span data-stu-id="8cab4-168">Uninstall CLI 1.x versions</span></span>

<span data-ttu-id="8cab4-169">Si vous votre système dispose d’une version 1.x antérieure de l’interface de ligne de commande, vous pouvez la désinstaller en fonction du type d’installation utilisé.</span><span class="sxs-lookup"><span data-stu-id="8cab4-169">If you have an earlier CLI 1.x version available on your system, you can uninstall it based upon the type of install used.</span></span>

### <a name="uninstall-with-npm"></a><span data-ttu-id="8cab4-170">Désinstaller avec npm</span><span class="sxs-lookup"><span data-stu-id="8cab4-170">Uninstall with npm</span></span>

<span data-ttu-id="8cab4-171">Supprimez l’ancienne interface de ligne de commande avec `npm uninstall`.</span><span class="sxs-lookup"><span data-stu-id="8cab4-171">Remove the older CLI with `npm uninstall`.</span></span>

  ```bash
  npm uninstall -g azure-cli
  ```

### <a name="uninstall-with-distributable"></a><span data-ttu-id="8cab4-172">Désinstaller avec distribuable</span><span class="sxs-lookup"><span data-stu-id="8cab4-172">Uninstall with distributable</span></span>

<span data-ttu-id="8cab4-173">Si vous avez installé [MSI](http://aka.ms/webpi-azure-cli) ou un [package macOS](http://aka.ms/mac-azure-cli), utilisez le même outil pour supprimer votre installation.</span><span class="sxs-lookup"><span data-stu-id="8cab4-173">If you installed via [MSI](http://aka.ms/webpi-azure-cli) or a [macOS package](http://aka.ms/mac-azure-cli), use the same tool to remove your install.</span></span>

### <a name="uninstall-with-docker"></a><span data-ttu-id="8cab4-174">Désinstaller avec Docker</span><span class="sxs-lookup"><span data-stu-id="8cab4-174">Uninstall with Docker</span></span>

<span data-ttu-id="8cab4-175">Si vous avez installé une image Docker pour utiliser la version antérieure de l’interface de ligne de commande, supprimez cette image et tous les conteneurs associés.</span><span class="sxs-lookup"><span data-stu-id="8cab4-175">If you installed a Docker image to use the earlier CLI version, remove that image and any associated containers.</span></span> <span data-ttu-id="8cab4-176">Vous pouvez ensuite recréer les conteneurs après l’installation de la nouvelle image Docker comme décrit dans les instructions d’installation.</span><span class="sxs-lookup"><span data-stu-id="8cab4-176">You can then re-create the containers after installing the new Docker image as described in the install instructions.</span></span>

  ```bash
  docker rmi -f microsoft/azure-cli
  ```

## <a name="update-the-cli"></a><span data-ttu-id="8cab4-177">Mise à jour de l’interface CLI</span><span class="sxs-lookup"><span data-stu-id="8cab4-177">Update the CLI</span></span>

<span data-ttu-id="8cab4-178">Pour mettre à jour l’interface de ligne de commande Azure, utilisez la même méthode que vous avez utilisée pour l’installer.</span><span class="sxs-lookup"><span data-stu-id="8cab4-178">To update the Azure CLI, use the same method that you used to install it.</span></span>

### <a name="update-with-homebrew"></a><span data-ttu-id="8cab4-179">Mettre à jour avec Homebrew</span><span class="sxs-lookup"><span data-stu-id="8cab4-179">Update with Homebrew</span></span>

1. <span data-ttu-id="8cab4-180">Mettez à jour vos informations de référentiel Homebrew locales.</span><span class="sxs-lookup"><span data-stu-id="8cab4-180">Update your local Homebrew repository information.</span></span>

   ```bash
   brew update
   ```

2. <span data-ttu-id="8cab4-181">Mettez à niveau les packages installés.</span><span class="sxs-lookup"><span data-stu-id="8cab4-181">Upgrade your installed packages.</span></span>

   ```bash
   brew upgrade
   ```

### <a name="update-with-msi"></a><span data-ttu-id="8cab4-182">Mettre à jour avec MSI</span><span class="sxs-lookup"><span data-stu-id="8cab4-182">Update with MSI</span></span>

<span data-ttu-id="8cab4-183">Exécutez de nouveau le [MSI](https://aka.ms/InstallAzureCliWindows) .</span><span class="sxs-lookup"><span data-stu-id="8cab4-183">Run the [MSI](https://aka.ms/InstallAzureCliWindows) again.</span></span>

### <a name="update-with-apt-get"></a><span data-ttu-id="8cab4-184">Mettre à jour avec apt-get</span><span class="sxs-lookup"><span data-stu-id="8cab4-184">Update with apt-get</span></span>

<span data-ttu-id="8cab4-185">Utilisez `apt-get upgrade` pour mettre à jour le package de l’interface de ligne de commande.</span><span class="sxs-lookup"><span data-stu-id="8cab4-185">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> <span data-ttu-id="8cab4-186">Cela met à niveau tous les packages installés sur votre système n’ayant pas de modification de dépendance.</span><span class="sxs-lookup"><span data-stu-id="8cab4-186">This will upgrade all of the installed packages on your system which have not had a dependency change.</span></span>
> <span data-ttu-id="8cab4-187">Pour ne mettre à niveau que l’interface de ligne de commande, utilisez `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="8cab4-187">To upgrade only the CLI, use `apt-get install`.</span></span>
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

### <a name="update-with-docker"></a><span data-ttu-id="8cab4-188">Mettre à jour avec Docker</span><span class="sxs-lookup"><span data-stu-id="8cab4-188">Update with Docker</span></span>

1. <span data-ttu-id="8cab4-189">Mettre à jour votre image locale avec `docker pull`.</span><span class="sxs-lookup"><span data-stu-id="8cab4-189">Update your local image with `docker pull`.</span></span>

   ```bash
   docker pull azuresdk/azure-cli-python
   ```

2. <span data-ttu-id="8cab4-190">Obtenir les conteneurs qui utilisent actuellement l’image de l’interface de ligne de commande.</span><span class="sxs-lookup"><span data-stu-id="8cab4-190">Get the containers currently using the CLI image.</span></span>

   ```bash
   docker container ls -a --filter 'ancestor=azuresdk/azure-cli-python'
   ```

   ```output
   CONTAINER ID        IMAGE                              COMMAND             CREATED             STATUS                        PORTS               NAMES
   34a868beb2ab        azuresdk/azure-cli-python:latest      "/bin/sh -c bash"   8 minutes ago       Exited (0) 8 minutes ago                       inspiring_benz
   ```

> [!NOTE]
> <span data-ttu-id="8cab4-191">Si vous avez installé une version spécifique de l’image, vous devez ajouter `:<version>` à la fin du nom de l’image.</span><span class="sxs-lookup"><span data-stu-id="8cab4-191">If you installed a specific version of the image, you will need to add `:<version>` to the end of the image name.</span></span>

3. <span data-ttu-id="8cab4-192">Interrompre et recréer les conteneurs.</span><span class="sxs-lookup"><span data-stu-id="8cab4-192">Halt and recreate the containers.</span></span>

   ```bash
   docker stop inspiring_benz
   docker rm inspiring_benz
   docker run azuresdk/azure-cli-python
   ```

### <a name="update-manually"></a><span data-ttu-id="8cab4-193">Mettre à jour manuellement</span><span class="sxs-lookup"><span data-stu-id="8cab4-193">Update manually</span></span>

<span data-ttu-id="8cab4-194">Suivez les instructions d’installation manuelle de [macOS](#macOS) ou [Linux](#Linux) pour effectuer la mise à jour.</span><span class="sxs-lookup"><span data-stu-id="8cab4-194">Follow the manual installation instructions for [macOS](#macOS) or [Linux](#Linux) to update.</span></span>

## <a name="uninstall"></a><span data-ttu-id="8cab4-195">Désinstaller l’interface</span><span class="sxs-lookup"><span data-stu-id="8cab4-195">Uninstall</span></span>

<span data-ttu-id="8cab4-196">Si vous décidez de désinstaller l’interface de ligne de commande, nous sommes désolés de vous voir partir.</span><span class="sxs-lookup"><span data-stu-id="8cab4-196">If you decide to uninstall the CLI, we're sorry to see you go.</span></span> <span data-ttu-id="8cab4-197">Vous devez effectuer la désinstallation à l’aide de la même méthode que vous avez utilisée pour installer l’interface de ligne de commande.</span><span class="sxs-lookup"><span data-stu-id="8cab4-197">You should uninstall using the same method that you used to install the CLI.</span></span>

### <a name="uninstall-with-homebrew"></a><span data-ttu-id="8cab4-198">Désinstaller avec Homebrew</span><span class="sxs-lookup"><span data-stu-id="8cab4-198">Uninstall with Homebrew</span></span>

<span data-ttu-id="8cab4-199">Désinstallez le package `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="8cab4-199">Uninstall the `azure-cli` package.</span></span>

   ```bash
   brew uninstall azure-cli
   ```

### <a name="uninstall-with-msi"></a><span data-ttu-id="8cab4-200">Désinstaller avec MSI</span><span class="sxs-lookup"><span data-stu-id="8cab4-200">Uninstall with MSI</span></span>

<span data-ttu-id="8cab4-201">Exécutez le [MSI](https://aka.ms/InstallAzureCliWindows) de nouveau et choisissez Désinstaller.</span><span class="sxs-lookup"><span data-stu-id="8cab4-201">Run the [MSI](https://aka.ms/InstallAzureCliWindows) again and choose uninstall.</span></span>

### <a name="uninstall-with-apt-get"></a><span data-ttu-id="8cab4-202">Désinstaller avec apt-get</span><span class="sxs-lookup"><span data-stu-id="8cab4-202">Uninstall with apt-get</span></span>

<span data-ttu-id="8cab4-203">Désinstallation via `apt-get remove`:</span><span class="sxs-lookup"><span data-stu-id="8cab4-203">Uninstall via `apt-get remove`:</span></span>

  ```bash
  sudo apt-get remove -y azure-cli
  ```

### <a name="uninstall-with-docker"></a><span data-ttu-id="8cab4-204">Désinstaller avec Docker</span><span class="sxs-lookup"><span data-stu-id="8cab4-204">Uninstall with Docker</span></span>

<span data-ttu-id="8cab4-205">Si vous avez installé une image docker, vous devez supprimer tous les conteneurs qui l’exécutent avant de supprimer l’image locale.</span><span class="sxs-lookup"><span data-stu-id="8cab4-205">If you installed a docker image, you will need to remove any containers running it, and then delete the local image.</span></span>

1. <span data-ttu-id="8cab4-206">Obtenez les conteneurs qui exécutent l’image de l’interface de ligne de commande Azure.</span><span class="sxs-lookup"><span data-stu-id="8cab4-206">Get the containers which are running the azure-cli image.</span></span>

   ```bash
   docker container ls -a --filter 'ancestor=azuresdk/azure-cli-python'
   ```

   ```output
   CONTAINER ID        IMAGE                              COMMAND             CREATED             STATUS                        PORTS               NAMES
   34a868beb2ab        azuresdk/azure-cli-python:latest      "/bin/sh -c bash"   8 minutes ago       Exited (0) 8 minutes ago                       inspiring_benz
   ```

2. <span data-ttu-id="8cab4-207">Supprimez tous les conteneurs avec l’image de l’interface de ligne de commande.</span><span class="sxs-lookup"><span data-stu-id="8cab4-207">Delete any containers with the CLI image.</span></span>

   ```bash
   docker rm 34a868beb2ab
   ```

3. <span data-ttu-id="8cab4-208">Supprimez l’image de l’interface de ligne de commande installée localement.</span><span class="sxs-lookup"><span data-stu-id="8cab4-208">Remove the locally installed CLI image.</span></span>

   ```bash
   docker rmi azuresdk/azure-cli-python
   ```

> [!NOTE]
> <span data-ttu-id="8cab4-209">Si vous avez installé une version spécifique de l’image, vous devez ajouter `:<version>` à la fin du nom de l’image.</span><span class="sxs-lookup"><span data-stu-id="8cab4-209">If you installed a specific version of the image, you will need to add `:<version>` to the end of the image name.</span></span>

### <a name="uninstall-manually"></a><span data-ttu-id="8cab4-210">Désinstaller manuellement</span><span class="sxs-lookup"><span data-stu-id="8cab4-210">Uninstall manually</span></span>

<span data-ttu-id="8cab4-211">Si vous avez installé l’interface de ligne de commande en utilisant le script accessible à l’adresse https://aka.ms/InstallAzureCli, vous pouvez désinstaller l’interface à l’aide de la procédure suivante.</span><span class="sxs-lookup"><span data-stu-id="8cab4-211">If you used the script at https://aka.ms/InstallAzureCli to install the CLI, you can uninstall it with these steps.</span></span>

1. <span data-ttu-id="8cab4-212">Supprimez les fichiers installés.</span><span class="sxs-lookup"><span data-stu-id="8cab4-212">Remove the installed files.</span></span>

   ```bash
   rm -r <install location>/lib/azure-cli
   rm <install location>/bin/az
   ```

2. <span data-ttu-id="8cab4-213">Supprimez la ligne `<install location>/lib/azure-cli/az.completion` de `<install location>/.bash_profile`.</span><span class="sxs-lookup"><span data-stu-id="8cab4-213">Delete the line `<install location>/lib/azure-cli/az.completion` from `<install location>/.bash_profile`.</span></span>

> [!Note]
> <span data-ttu-id="8cab4-214">L’emplacement d’installation par défaut est `/Users/<username>`.</span><span class="sxs-lookup"><span data-stu-id="8cab4-214">The default install location is `/Users/<username>`.</span></span>

## <a name="report-cli-issues-and-feedback"></a><span data-ttu-id="8cab4-215">Signaler des problèmes avec CLI et commentaires</span><span class="sxs-lookup"><span data-stu-id="8cab4-215">Report CLI issues and feedback</span></span>

<span data-ttu-id="8cab4-216">Si vous rencontrez des bogues en utilisant l’outil, signalez un problème dans la section [Problèmes](https://github.com/Azure/azure-cli/issues) de notre référentiel GitHub.</span><span class="sxs-lookup"><span data-stu-id="8cab4-216">If you encounter any bugs with the tool, file an issue in the [Issues](https://github.com/Azure/azure-cli/issues) section of our GitHub repository.</span></span>
<span data-ttu-id="8cab4-217">Pour fournir des commentaires à partir de la ligne de commande, utilisez la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="8cab4-217">To provide feedback from the command line, use the `az feedback` command.</span></span>
