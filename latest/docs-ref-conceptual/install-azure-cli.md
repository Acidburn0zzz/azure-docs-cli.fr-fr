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
ms.openlocfilehash: 1b47bd5603f5214dd11d772caaebe8cf380df5c0
ms.sourcegitcommit: 5e862fd0a93cf668fa76a74ae1c7505d3c8c45f2
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/09/2017
---
# <a name="install-azure-cli-20"></a><span data-ttu-id="adf1e-104">Installer Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="adf1e-104">Install Azure CLI 2.0</span></span>

<span data-ttu-id="adf1e-105">Installez la nouvelle version de l’interface de ligne de commande Azure dès aujourd’hui.</span><span class="sxs-lookup"><span data-stu-id="adf1e-105">Install the new version of the Azure CLI today!</span></span>
<span data-ttu-id="adf1e-106">Nous avons amélioré et mis à jour cette interface afin d’offrir une expérience de ligne de commande native d’exception pour la gestion des ressources Azure.</span><span class="sxs-lookup"><span data-stu-id="adf1e-106">We've improved and updated it to provide a great native command-line experience for managing Azure resources.</span></span>
<span data-ttu-id="adf1e-107">Elle peut être utilisée sur macOS, Linux et Windows.</span><span class="sxs-lookup"><span data-stu-id="adf1e-107">It can be used on macOS, Linux, and Windows.</span></span>
<span data-ttu-id="adf1e-108">Pour plus d’informations sur la version la plus récente, consultez les [Notes de publication](release-notes-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="adf1e-108">For information about the latest release, see the [release notes](release-notes-azure-cli.md).</span></span>

> [!NOTE]
> <span data-ttu-id="adf1e-109">Si vous devez utiliser la version précédente d’Azure CLI, voici comment [installer Azure 1.0](/azure/cli-install-nodejs).</span><span class="sxs-lookup"><span data-stu-id="adf1e-109">If you need the previous version of the Azure CLI, here's how to [install Azure CLI 1.0](/azure/cli-install-nodejs).</span></span>

## <a name="a-namemacosinstall-on-macos"></a><span data-ttu-id="adf1e-110"><a name="macOS"/>Installer sur macOS</span><span class="sxs-lookup"><span data-stu-id="adf1e-110"><a name="macOS"/>Install on macOS</span></span>

<span data-ttu-id="adf1e-111">Sur macOS, vous avez le choix de procéder à l’installation avec [Homebrew](https://brew.sh/) ou manuellement.</span><span class="sxs-lookup"><span data-stu-id="adf1e-111">On macOS, you are able to install either with [Homebrew](https://brew.sh/) or manually.</span></span>

### <a name="install-with-homebrew"></a><span data-ttu-id="adf1e-112">Désinstaller avec Homebrew</span><span class="sxs-lookup"><span data-stu-id="adf1e-112">Install with Homebrew</span></span>

1. <span data-ttu-id="adf1e-113">Si vous ne l’avez pas encore, installez Homebrew en suivant les [instructions d’installation pour Homebrew](https://docs.brew.sh/Installation.html).</span><span class="sxs-lookup"><span data-stu-id="adf1e-113">If you don't have it already, install Homebrew by following the [Homebrew installation instructions](https://docs.brew.sh/Installation.html).</span></span>

2. <span data-ttu-id="adf1e-114">Si vous avez précédemment installé CLI manuellement, suivez les instructions du [manuel de désinstallation](#UninstallManually).</span><span class="sxs-lookup"><span data-stu-id="adf1e-114">If you have previously installed the CLI manually, follow the [manual uninstall](#UninstallManually) instructions.</span></span>

3. <span data-ttu-id="adf1e-115">Mettez à jour vos référentiels Homebrew locaux.</span><span class="sxs-lookup"><span data-stu-id="adf1e-115">Update your local Homebrew repositories.</span></span>

   ```bash
   brew update
   ```

4. <span data-ttu-id="adf1e-116">Installez le package `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="adf1e-116">Install the `azure-cli` package.</span></span>

  ```bash
  brew install azure-cli
  ```

> [!NOTE]
> <span data-ttu-id="adf1e-117">Si vous avez installé Azure CLI 1.0 avec Homebrew au préalable, au lieu d’installer le package, vous pouvez obtenir CLI 2.0 grâce au processus normal de mise à niveau Homebrew.</span><span class="sxs-lookup"><span data-stu-id="adf1e-117">If you previously installed the Azure CLI 1.0 with Homebrew, instead of installing the package you can get CLI 2.0 through the regular Homebrew upgrade process.</span></span>
>
> ```bash
> brew upgrade
> ```

### <a name="install-manually"></a><span data-ttu-id="adf1e-118">Installer manuellement</span><span class="sxs-lookup"><span data-stu-id="adf1e-118">Install manually</span></span>

1. <span data-ttu-id="adf1e-119">Installer l’interface de ligne de commande Azure 2.0 avec `curl`.</span><span class="sxs-lookup"><span data-stu-id="adf1e-119">Install Azure CLI 2.0 with `curl`.</span></span>

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

2. <span data-ttu-id="adf1e-120">Vous devrez peut-être redémarrer votre interpréteur de commandes pour que certaines modifications soient prises en compte.</span><span class="sxs-lookup"><span data-stu-id="adf1e-120">You may have to restart your shell for some changes to take effect.</span></span>

   ```bash
   exec -l $SHELL
   ```
   
3. <span data-ttu-id="adf1e-121">Exécutez l’interface de ligne de commande Azure 2.0 à partir de l’invite de commandes avec la commande `az` .</span><span class="sxs-lookup"><span data-stu-id="adf1e-121">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-on-windows"></a><span data-ttu-id="adf1e-122">Installer sur Windows</span><span class="sxs-lookup"><span data-stu-id="adf1e-122">Install on Windows</span></span>

### <a name="install-with-msi-for-the-windows-command-line"></a><span data-ttu-id="adf1e-123">Installer avec MSI pour la ligne de commande Windows</span><span class="sxs-lookup"><span data-stu-id="adf1e-123">Install with MSI for the Windows command-line</span></span> 

<span data-ttu-id="adf1e-124">Pour installer CLI sur Windows et l’utiliser dans la ligne de commande, téléchargez et exécutez le [Programme d’installation d’Azure CLI (MSI)](https://aka.ms/InstallAzureCliWindows).</span><span class="sxs-lookup"><span data-stu-id="adf1e-124">To install the CLI on Windows and use it in the Windows command-line, download and run the [Azure CLI Installer (MSI)](https://aka.ms/InstallAzureCliWindows).</span></span>

### <a name="install-with-apt-get-for-bash-on-ubuntu-on-windows"></a><span data-ttu-id="adf1e-125">Installer avec apt-get pour Bash sous Ubuntu ou Windows</span><span class="sxs-lookup"><span data-stu-id="adf1e-125">Install with apt-get for Bash on Ubuntu on Windows</span></span>

1. <span data-ttu-id="adf1e-126">Si vous ne disposez pas de Bash sur Windows, [installez-le](https://msdn.microsoft.com/commandline/wsl/install_guide).</span><span class="sxs-lookup"><span data-stu-id="adf1e-126">If you don't have Bash on Windows, [install it](https://msdn.microsoft.com/commandline/wsl/install_guide).</span></span>

2. <span data-ttu-id="adf1e-127">Ouvrez l’interpréteur de commandes Bash.</span><span class="sxs-lookup"><span data-stu-id="adf1e-127">Open the Bash shell.</span></span>

3. <span data-ttu-id="adf1e-128">Modifiez votre liste de sources.</span><span class="sxs-lookup"><span data-stu-id="adf1e-128">Modify your sources list.</span></span>

   ```bash
   echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
   ```

4. <span data-ttu-id="adf1e-129">Exécutez les commandes sudo suivantes :</span><span class="sxs-lookup"><span data-stu-id="adf1e-129">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

5.  <span data-ttu-id="adf1e-130">Exécutez l’interface de ligne de commande Azure 2.0 à partir de l’invite de commandes avec la commande `az` .</span><span class="sxs-lookup"><span data-stu-id="adf1e-130">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-on-debianubuntu-with-apt-get"></a><span data-ttu-id="adf1e-131">Installer sous Debian/Ubuntu avec apt-get</span><span class="sxs-lookup"><span data-stu-id="adf1e-131">Install on Debian/Ubuntu with apt-get</span></span>

<span data-ttu-id="adf1e-132">Pour les distributions qui utilisent le gestionnaire de package `apt`, vous pouvez installer Azure CLI 2.0 via `apt-get`.</span><span class="sxs-lookup"><span data-stu-id="adf1e-132">For distributions using the `apt` package manager, you can install Azure CLI 2.0 via `apt-get`.</span></span>

> [!NOTE]
> <span data-ttu-id="adf1e-133">Votre distribution doit prendre en charge Python 2.7.x ou Python 3.x pour utiliser l’interface CLI.</span><span class="sxs-lookup"><span data-stu-id="adf1e-133">Your distribution must have support for Python 2.7.x or Python 3.x in order to use the CLI.</span></span>

1. <span data-ttu-id="adf1e-134">Modifiez votre liste de sources :</span><span class="sxs-lookup"><span data-stu-id="adf1e-134">Modify your sources list:</span></span>
 
   - <span data-ttu-id="adf1e-135">Système 32 bits</span><span class="sxs-lookup"><span data-stu-id="adf1e-135">32-bit system</span></span>

     ```bash
     echo "deb https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

   - <span data-ttu-id="adf1e-136">Système 64 bits</span><span class="sxs-lookup"><span data-stu-id="adf1e-136">64-bit system</span></span>

     ```bash
     echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

2. <span data-ttu-id="adf1e-137">Exécutez les commandes sudo suivantes :</span><span class="sxs-lookup"><span data-stu-id="adf1e-137">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

3.  <span data-ttu-id="adf1e-138">Exécutez l’interface de ligne de commande Azure 2.0 à partir de l’invite de commandes avec la commande `az` .</span><span class="sxs-lookup"><span data-stu-id="adf1e-138">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-on-rhel-fedora-and-centos-with-yum"></a><span data-ttu-id="adf1e-139">Installer sur RHEL, Fedora et CentOS avec yum</span><span class="sxs-lookup"><span data-stu-id="adf1e-139">Install on RHEL, Fedora, and CentOS with yum</span></span>

<span data-ttu-id="adf1e-140">Pour les distributions qui utilisent le gestionnaire de package `yum`, vous pouvez installer Azure CLI 2.0 via `yum`.</span><span class="sxs-lookup"><span data-stu-id="adf1e-140">For distributions which use the `yum` package manager, you can install Azure CLI 2.0 via `yum`.</span></span>

> [!NOTE]
> <span data-ttu-id="adf1e-141">Votre distribution doit prendre en charge Python 2.7.x ou Python 3.x pour utiliser l’interface CLI.</span><span class="sxs-lookup"><span data-stu-id="adf1e-141">Your distribution must have support for Python 2.7.x or Python 3.x in order to use the CLI.</span></span>

1. <span data-ttu-id="adf1e-142">Importer la clé de référentiel Microsoft :</span><span class="sxs-lookup"><span data-stu-id="adf1e-142">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. <span data-ttu-id="adf1e-143">Créer des informations de référentiel `azure-cli` locales :</span><span class="sxs-lookup"><span data-stu-id="adf1e-143">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/azure-cli.repo'
   ```

3. <span data-ttu-id="adf1e-144">Mettre à jour l’index de package `yum` et l’installer :</span><span class="sxs-lookup"><span data-stu-id="adf1e-144">Update the `yum` package index and install:</span></span>

   ```bash
   yum check-update
   sudo yum install azure-cli
   ```

4. <span data-ttu-id="adf1e-145">Exécutez l’interface de ligne de commande Azure 2.0 à partir de l’invite de commandes avec la commande `az` .</span><span class="sxs-lookup"><span data-stu-id="adf1e-145">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-on-opensuse-and-sle-with-zypper"></a><span data-ttu-id="adf1e-146">Installer sur openSUSE et SLE avec zypper</span><span class="sxs-lookup"><span data-stu-id="adf1e-146">Install on openSUSE and SLE with zypper</span></span>

<span data-ttu-id="adf1e-147">Pour les distributions qui utilisent le gestionnaire de package `zypper`, vous pouvez installer Azure CLI 2.0 via `zypper`.</span><span class="sxs-lookup"><span data-stu-id="adf1e-147">For distributions which use the `zypper` package manager, you can install Azure CLI 2.0 via `zypper`.</span></span>

> [!NOTE]
> <span data-ttu-id="adf1e-148">Votre distribution doit prendre en charge Python 2.7.x ou Python 3.x pour utiliser l’interface CLI.</span><span class="sxs-lookup"><span data-stu-id="adf1e-148">Your distribution must have support for Python 2.7.x or Python 3.x in order to use the CLI.</span></span>

1. <span data-ttu-id="adf1e-149">Importer la clé de référentiel Microsoft :</span><span class="sxs-lookup"><span data-stu-id="adf1e-149">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. <span data-ttu-id="adf1e-150">Créer des informations de référentiel `azure-cli` locales :</span><span class="sxs-lookup"><span data-stu-id="adf1e-150">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ntype=rpm-md\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/zypp/repos.d/azure-cli.repo'
   ```

3. <span data-ttu-id="adf1e-151">Mettre à jour l’index de package `zypper` et l’installer :</span><span class="sxs-lookup"><span data-stu-id="adf1e-151">Update the `zypper` package index and install:</span></span>

   ```bash
   sudo zypper refresh
   sudo zypper install azure-cli
   ```

4. <span data-ttu-id="adf1e-152">Exécutez l’interface de ligne de commande Azure 2.0 à partir de l’invite de commandes avec la commande `az` .</span><span class="sxs-lookup"><span data-stu-id="adf1e-152">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-with-docker"></a><span data-ttu-id="adf1e-153">Installer avec Docker</span><span class="sxs-lookup"><span data-stu-id="adf1e-153">Install with Docker</span></span>

<span data-ttu-id="adf1e-154">Nous fournissons une image Docker pré-configurée avec l’interface de ligne de commande Azure 2.0.</span><span class="sxs-lookup"><span data-stu-id="adf1e-154">We maintain a Docker image preconfigured with the Azure CLI 2.0.</span></span>

<span data-ttu-id="adf1e-155">Installez l’interface de ligne de commande à l’aide de `docker run`.</span><span class="sxs-lookup"><span data-stu-id="adf1e-155">Install the CLI using `docker run`.</span></span>

   ```bash
   docker run azuresdk/azure-cli-python:<version>
   ```

<span data-ttu-id="adf1e-156">Consultez nos [balises Docker](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/) pour connaître les versions disponibles.</span><span class="sxs-lookup"><span data-stu-id="adf1e-156">See our [Docker tags](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/) for available versions.</span></span>

<span data-ttu-id="adf1e-157">L’interface de ligne de commande est installé sur l’image en tant que commande `az` dans `/usr/local/bin`.</span><span class="sxs-lookup"><span data-stu-id="adf1e-157">The CLI is installed on the image as the `az` command in `/usr/local/bin`.</span></span>

> [!NOTE]
> <span data-ttu-id="adf1e-158">Si vous souhaitez sélectionner les clés SSH à partir de votre environnement utilisateur, vous pouvez utiliser `-v ${HOME}:/root` pour monter $HOME en tant que `/root`.</span><span class="sxs-lookup"><span data-stu-id="adf1e-158">If you want to pick up the SSH keys from your user environment, you can use `-v ${HOME}:/root` to mount $HOME as `/root`.</span></span>

> ```bash
> docker run -v ${HOME}:/root azuresdk/azure-cli-python:<version>
> ```

## <a name="a-namelinuxinstall-on-linux-without-a-package-manager"></a><span data-ttu-id="adf1e-159"><a name="Linux"/>Installer sous Linux sans gestionnaire de package</span><span class="sxs-lookup"><span data-stu-id="adf1e-159"><a name="Linux"/>Install on Linux without a package manager</span></span>

<span data-ttu-id="adf1e-160">Il est recommandé d’installer l’interface de ligne de commande avec un gestionnaire de package si possible.</span><span class="sxs-lookup"><span data-stu-id="adf1e-160">It is recommended that you install the CLI with a package manager if you are able to.</span></span> <span data-ttu-id="adf1e-161">Si vous ne voulez pas ajouter les référentiels Microsoft, ou que vous travaillez avec une distribution qui ne dispose pas d’un package fourni, vous pouvez installer l’interface CLI manuellement.</span><span class="sxs-lookup"><span data-stu-id="adf1e-161">If you do not want to add Microsoft's repositories, or are working with a distribution which does not have a provided package, you can manually install the CLI.</span></span>

1. <span data-ttu-id="adf1e-162">Installez les composants requis en fonction de votre distribution Linux.</span><span class="sxs-lookup"><span data-stu-id="adf1e-162">Install the prerequisites based on your Linux distribution.</span></span>

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

<span data-ttu-id="adf1e-163">Si votre distribution n’est pas répertoriée ci-dessus, vous devez installer [Python 2.7 ou version ultérieure](https://www.python.org/downloads/), [libffi](https://sourceware.org/libffi/), et [OpenSSL](https://www.openssl.org/source/).</span><span class="sxs-lookup"><span data-stu-id="adf1e-163">If your distribution is not listed above, you will need to install [Python 2.7 or later](https://www.python.org/downloads/), [libffi](https://sourceware.org/libffi/), and [OpenSSL](https://www.openssl.org/source/).</span></span>

2. <span data-ttu-id="adf1e-164">Installez l’interface de ligne de commande à l’aide de `curl`.</span><span class="sxs-lookup"><span data-stu-id="adf1e-164">Install the CLI with  `curl`.</span></span>

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

3. <span data-ttu-id="adf1e-165">Vous devrez peut-être redémarrer votre interpréteur de commandes pour que certaines modifications soient prises en compte.</span><span class="sxs-lookup"><span data-stu-id="adf1e-165">You may have to restart your shell for some changes to take effect.</span></span>

   ```bash
   exec -l $SHELL
   ```

4. <span data-ttu-id="adf1e-166">Exécutez l’interface de ligne de commande Azure 2.0 à partir de l’invite de commandes avec la commande `az` .</span><span class="sxs-lookup"><span data-stu-id="adf1e-166">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="adf1e-167">Résolution des problèmes</span><span class="sxs-lookup"><span data-stu-id="adf1e-167">Troubleshooting</span></span>

<span data-ttu-id="adf1e-168">Si vous rencontrez un problème lors de l’installation de l’interface de ligne de commande, consultez cette section pour savoir si votre cas particulier est couvert.</span><span class="sxs-lookup"><span data-stu-id="adf1e-168">If you encounter an issue during CLI install, check this section to see if your particular case is covered.</span></span> <span data-ttu-id="adf1e-169">Si votre problème n’est pas ici, veuillez [signaler le problème lié à Github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="adf1e-169">If your issue is not here, please [file a Github issue](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="curl-object-moved-error"></a><span data-ttu-id="adf1e-170">erreur curl « Objet déplacé »</span><span class="sxs-lookup"><span data-stu-id="adf1e-170">curl "Object Moved" error</span></span>

<span data-ttu-id="adf1e-171">Si la commande `curl` renvoie une erreur concernant le `-L` paramètre ou un message d’erreur indiquant « Objet déplacé », essayez d’utiliser l’URL complète plutôt que la `aka.ms` redirection :</span><span class="sxs-lookup"><span data-stu-id="adf1e-171">If you get an error from `curl` related to the `-L` parameter, or an error message including the text "Object Moved", try using the full URL instead of the `aka.ms` redirect:</span></span>

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

### <a name="az-command-not-found"></a><span data-ttu-id="adf1e-172">`az` commande introuvable</span><span class="sxs-lookup"><span data-stu-id="adf1e-172">`az` command not found</span></span>

<span data-ttu-id="adf1e-173">Vous devrez peut-être effacer le cache de hachage de commande de l’interpréteur de commandes</span><span class="sxs-lookup"><span data-stu-id="adf1e-173">You may need to clear your shell's command hash cache.</span></span> <span data-ttu-id="adf1e-174">Exécuter</span><span class="sxs-lookup"><span data-stu-id="adf1e-174">Run</span></span>

```bash
hash -r
```

<span data-ttu-id="adf1e-175">et vérifier si le problème est résolu.</span><span class="sxs-lookup"><span data-stu-id="adf1e-175">and see if the problem is resolved.</span></span>

## <a name="uninstall-cli-1x-versions"></a><span data-ttu-id="adf1e-176">Désinstaller les versions 1.x de l’interface de ligne de commande</span><span class="sxs-lookup"><span data-stu-id="adf1e-176">Uninstall CLI 1.x versions</span></span>

<span data-ttu-id="adf1e-177">Si vous votre système dispose d’une version 1.x antérieure de l’interface de ligne de commande, vous pouvez la désinstaller en fonction du type d’installation utilisé.</span><span class="sxs-lookup"><span data-stu-id="adf1e-177">If you have an earlier CLI 1.x version available on your system, you can uninstall it based upon the type of install used.</span></span>

### <a name="uninstall-with-npm"></a><span data-ttu-id="adf1e-178">Désinstaller avec npm</span><span class="sxs-lookup"><span data-stu-id="adf1e-178">Uninstall with npm</span></span>

<span data-ttu-id="adf1e-179">Supprimez l’ancienne interface de ligne de commande avec `npm uninstall`.</span><span class="sxs-lookup"><span data-stu-id="adf1e-179">Remove the older CLI with `npm uninstall`.</span></span>

  ```bash
  npm uninstall -g azure-cli
  ```

### <a name="uninstall-with-distributable"></a><span data-ttu-id="adf1e-180">Désinstaller avec distribuable</span><span class="sxs-lookup"><span data-stu-id="adf1e-180">Uninstall with distributable</span></span>

<span data-ttu-id="adf1e-181">Si vous avez effectué l’installation via le [Programme d’installation d’Azure CLI (MSI)](http://aka.ms/webpi-azure-cli) ou un [package macOS](http://aka.ms/mac-azure-cli), utilisez le même outil pour supprimer votre installation.</span><span class="sxs-lookup"><span data-stu-id="adf1e-181">If you installed via the [Azure CLI Installer (MSI)](http://aka.ms/webpi-azure-cli) or a [macOS package](http://aka.ms/mac-azure-cli), use the same tool to remove your install.</span></span>

### <a name="uninstall-with-docker"></a><span data-ttu-id="adf1e-182">Désinstaller avec Docker</span><span class="sxs-lookup"><span data-stu-id="adf1e-182">Uninstall with Docker</span></span>

<span data-ttu-id="adf1e-183">Si vous avez installé une image Docker pour utiliser la version antérieure de l’interface de ligne de commande, supprimez cette image et tous les conteneurs associés.</span><span class="sxs-lookup"><span data-stu-id="adf1e-183">If you installed a Docker image to use the earlier CLI version, remove that image and any associated containers.</span></span> <span data-ttu-id="adf1e-184">Vous pouvez ensuite recréer les conteneurs après l’installation de la nouvelle image Docker comme décrit dans les instructions d’installation.</span><span class="sxs-lookup"><span data-stu-id="adf1e-184">You can then re-create the containers after installing the new Docker image as described in the install instructions.</span></span>

  ```bash
  docker rmi -f microsoft/azure-cli
  ```

## <a name="update-the-cli"></a><span data-ttu-id="adf1e-185">Mise à jour de l’interface CLI</span><span class="sxs-lookup"><span data-stu-id="adf1e-185">Update the CLI</span></span>

<span data-ttu-id="adf1e-186">Pour mettre à jour l’interface de ligne de commande Azure, utilisez la même méthode que vous avez utilisée pour l’installer.</span><span class="sxs-lookup"><span data-stu-id="adf1e-186">To update the Azure CLI, use the same method that you used to install it.</span></span>

### <a name="update-with-homebrew"></a><span data-ttu-id="adf1e-187">Mettre à jour avec Homebrew</span><span class="sxs-lookup"><span data-stu-id="adf1e-187">Update with Homebrew</span></span>

1. <span data-ttu-id="adf1e-188">Si vous avez précédemment effectué l’installation manuellement, suivez les instructions relatives à l’[installation avec Homebrew](#macOS).</span><span class="sxs-lookup"><span data-stu-id="adf1e-188">If you previously installed manually, follow the [install with Homebrew](#macOS) instructions.</span></span>

2. <span data-ttu-id="adf1e-189">Mettez à jour vos informations de référentiel Homebrew locales.</span><span class="sxs-lookup"><span data-stu-id="adf1e-189">Update your local Homebrew repository information.</span></span>

   ```bash
   brew update
   ```

3. <span data-ttu-id="adf1e-190">Mettez à niveau les packages installés.</span><span class="sxs-lookup"><span data-stu-id="adf1e-190">Upgrade your installed packages.</span></span>

   ```bash
   brew upgrade
   ```

### <a name="update-with-msi"></a><span data-ttu-id="adf1e-191">Mettre à jour avec MSI</span><span class="sxs-lookup"><span data-stu-id="adf1e-191">Update with MSI</span></span>

<span data-ttu-id="adf1e-192">Exécutez de nouveau le [Programme d’installation d’Azure CLI (MSI)](https://aka.ms/InstallAzureCliWindows).</span><span class="sxs-lookup"><span data-stu-id="adf1e-192">Run the [Azure CLI Installer (MSI)](https://aka.ms/InstallAzureCliWindows) again.</span></span>

### <a name="update-with-apt-get"></a><span data-ttu-id="adf1e-193">Mettre à jour avec apt-get</span><span class="sxs-lookup"><span data-stu-id="adf1e-193">Update with apt-get</span></span>

<span data-ttu-id="adf1e-194">Utilisez `apt-get upgrade` pour mettre à jour le package de l’interface de ligne de commande.</span><span class="sxs-lookup"><span data-stu-id="adf1e-194">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> <span data-ttu-id="adf1e-195">Cela met à niveau tous les packages installés sur votre système n’ayant pas de modification de dépendance.</span><span class="sxs-lookup"><span data-stu-id="adf1e-195">This will upgrade all of the installed packages on your system which have not had a dependency change.</span></span>
> <span data-ttu-id="adf1e-196">Pour ne mettre à niveau que l’interface de ligne de commande, utilisez `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="adf1e-196">To upgrade only the CLI, use `apt-get install`.</span></span>
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

### <a name="update-with-docker"></a><span data-ttu-id="adf1e-197">Mettre à jour avec Docker</span><span class="sxs-lookup"><span data-stu-id="adf1e-197">Update with Docker</span></span>

1. <span data-ttu-id="adf1e-198">Mettre à jour votre image locale avec `docker pull`.</span><span class="sxs-lookup"><span data-stu-id="adf1e-198">Update your local image with `docker pull`.</span></span>

   ```bash
   docker pull azuresdk/azure-cli-python
   ```

2. <span data-ttu-id="adf1e-199">Obtenir les conteneurs qui utilisent actuellement l’image de l’interface de ligne de commande.</span><span class="sxs-lookup"><span data-stu-id="adf1e-199">Get the containers currently using the CLI image.</span></span>

   ```bash
   docker container ls -a --filter 'ancestor=azuresdk/azure-cli-python'
   ```

   ```output
   CONTAINER ID        IMAGE                              COMMAND             CREATED             STATUS                        PORTS               NAMES
   34a868beb2ab        azuresdk/azure-cli-python:latest      "/bin/sh -c bash"   8 minutes ago       Exited (0) 8 minutes ago                       inspiring_benz
   ```

> [!NOTE]
> <span data-ttu-id="adf1e-200">Si vous avez installé une version spécifique de l’image, vous devez ajouter `:<version>` à la fin du nom de l’image.</span><span class="sxs-lookup"><span data-stu-id="adf1e-200">If you installed a specific version of the image, you will need to add `:<version>` to the end of the image name.</span></span>

3. <span data-ttu-id="adf1e-201">Interrompre et recréer les conteneurs.</span><span class="sxs-lookup"><span data-stu-id="adf1e-201">Halt and recreate the containers.</span></span>

   ```bash
   docker stop inspiring_benz
   docker rm inspiring_benz
   docker run azuresdk/azure-cli-python
   ```

### <a name="update-manually"></a><span data-ttu-id="adf1e-202">Mettre à jour manuellement</span><span class="sxs-lookup"><span data-stu-id="adf1e-202">Update manually</span></span>

<span data-ttu-id="adf1e-203">Suivez les instructions d’installation manuelle de [macOS](#macOS) ou [Linux](#Linux) pour effectuer la mise à jour.</span><span class="sxs-lookup"><span data-stu-id="adf1e-203">Follow the manual installation instructions for [macOS](#macOS) or [Linux](#Linux) to update.</span></span>

## <a name="uninstall"></a><span data-ttu-id="adf1e-204">Désinstaller l’interface</span><span class="sxs-lookup"><span data-stu-id="adf1e-204">Uninstall</span></span>

<span data-ttu-id="adf1e-205">Si vous décidez de désinstaller l’interface de ligne de commande, nous sommes désolés de vous voir partir.</span><span class="sxs-lookup"><span data-stu-id="adf1e-205">If you decide to uninstall the CLI, we're sorry to see you go.</span></span> <span data-ttu-id="adf1e-206">Vous devez effectuer la désinstallation à l’aide de la même méthode que vous avez utilisée pour installer l’interface de ligne de commande.</span><span class="sxs-lookup"><span data-stu-id="adf1e-206">You should uninstall using the same method that you used to install the CLI.</span></span>

### <a name="uninstall-with-homebrew"></a><span data-ttu-id="adf1e-207">Désinstaller avec Homebrew</span><span class="sxs-lookup"><span data-stu-id="adf1e-207">Uninstall with Homebrew</span></span>

<span data-ttu-id="adf1e-208">Désinstallez le package `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="adf1e-208">Uninstall the `azure-cli` package.</span></span>

   ```bash
   brew uninstall azure-cli
   ```

### <a name="uninstall-with-msi"></a><span data-ttu-id="adf1e-209">Désinstaller avec MSI</span><span class="sxs-lookup"><span data-stu-id="adf1e-209">Uninstall with MSI</span></span>

<span data-ttu-id="adf1e-210">Exécutez le [MSI](https://aka.ms/InstallAzureCliWindows) de nouveau et choisissez Désinstaller.</span><span class="sxs-lookup"><span data-stu-id="adf1e-210">Run the [MSI](https://aka.ms/InstallAzureCliWindows) again and choose uninstall.</span></span>

### <a name="uninstall-with-apt-get"></a><span data-ttu-id="adf1e-211">Désinstaller avec apt-get</span><span class="sxs-lookup"><span data-stu-id="adf1e-211">Uninstall with apt-get</span></span>

<span data-ttu-id="adf1e-212">Désinstallation via `apt-get remove`:</span><span class="sxs-lookup"><span data-stu-id="adf1e-212">Uninstall via `apt-get remove`:</span></span>

  ```bash
  sudo apt-get remove -y azure-cli
  ```

### <a name="uninstall-with-docker"></a><span data-ttu-id="adf1e-213">Désinstaller avec Docker</span><span class="sxs-lookup"><span data-stu-id="adf1e-213">Uninstall with Docker</span></span>

<span data-ttu-id="adf1e-214">Si vous avez installé une image docker, vous devez supprimer tous les conteneurs qui l’exécutent avant de supprimer l’image locale.</span><span class="sxs-lookup"><span data-stu-id="adf1e-214">If you installed a docker image, you will need to remove any containers running it, and then delete the local image.</span></span>

1. <span data-ttu-id="adf1e-215">Obtenez les conteneurs qui exécutent l’image de l’interface de ligne de commande Azure.</span><span class="sxs-lookup"><span data-stu-id="adf1e-215">Get the containers which are running the azure-cli image.</span></span>

   ```bash
   docker container ls -a --filter 'ancestor=azuresdk/azure-cli-python'
   ```

   ```output
   CONTAINER ID        IMAGE                              COMMAND             CREATED             STATUS                        PORTS               NAMES
   34a868beb2ab        azuresdk/azure-cli-python:latest      "/bin/sh -c bash"   8 minutes ago       Exited (0) 8 minutes ago                       inspiring_benz
   ```

2. <span data-ttu-id="adf1e-216">Supprimez tous les conteneurs avec l’image de l’interface de ligne de commande.</span><span class="sxs-lookup"><span data-stu-id="adf1e-216">Delete any containers with the CLI image.</span></span>

   ```bash
   docker rm 34a868beb2ab
   ```

3. <span data-ttu-id="adf1e-217">Supprimez l’image de l’interface de ligne de commande installée localement.</span><span class="sxs-lookup"><span data-stu-id="adf1e-217">Remove the locally installed CLI image.</span></span>

   ```bash
   docker rmi azuresdk/azure-cli-python
   ```

> [!NOTE]
> <span data-ttu-id="adf1e-218">Si vous avez installé une version spécifique de l’image, vous devez ajouter `:<version>` à la fin du nom de l’image.</span><span class="sxs-lookup"><span data-stu-id="adf1e-218">If you installed a specific version of the image, you will need to add `:<version>` to the end of the image name.</span></span>

###<a name="a-nameuninstallmanuallyuninstall-manually"></a><span data-ttu-id="adf1e-219"><a name="UninstallManually"/>Désinstaller manuellement</span><span class="sxs-lookup"><span data-stu-id="adf1e-219"><a name="UninstallManually"/>Uninstall manually</span></span>

<span data-ttu-id="adf1e-220">Si vous avez installé l’interface de ligne de commande en utilisant le script accessible à l’adresse https://aka.ms/InstallAzureCli, vous pouvez désinstaller l’interface à l’aide de la procédure suivante.</span><span class="sxs-lookup"><span data-stu-id="adf1e-220">If you used the script at https://aka.ms/InstallAzureCli to install the CLI, you can uninstall it with these steps.</span></span>

1. <span data-ttu-id="adf1e-221">Supprimez les fichiers installés.</span><span class="sxs-lookup"><span data-stu-id="adf1e-221">Remove the installed files.</span></span>

   ```bash
   rm -r <install location>/lib/azure-cli
   rm <install location>/bin/az
   ```

2. <span data-ttu-id="adf1e-222">Supprimez la ligne `<install location>/lib/azure-cli/az.completion` de `<install location>/.bash_profile`.</span><span class="sxs-lookup"><span data-stu-id="adf1e-222">Delete the line `<install location>/lib/azure-cli/az.completion` from `<install location>/.bash_profile`.</span></span>

3. <span data-ttu-id="adf1e-223">Si votre interpréteur de commandes utilise un cache de commande, rechargez-le.</span><span class="sxs-lookup"><span data-stu-id="adf1e-223">If your shell uses a command cache, reload it.</span></span>

   ```bash
   hash -r
   ```

> [!Note]
> <span data-ttu-id="adf1e-224">L’emplacement d’installation par défaut est `/Users/<username>`.</span><span class="sxs-lookup"><span data-stu-id="adf1e-224">The default install location is `/Users/<username>`.</span></span>

## <a name="report-cli-issues-and-feedback"></a><span data-ttu-id="adf1e-225">Signaler des problèmes avec CLI et commentaires</span><span class="sxs-lookup"><span data-stu-id="adf1e-225">Report CLI issues and feedback</span></span>

<span data-ttu-id="adf1e-226">Si vous rencontrez des bogues en utilisant l’outil, signalez un problème dans la section [Problèmes](https://github.com/Azure/azure-cli/issues) de notre référentiel GitHub.</span><span class="sxs-lookup"><span data-stu-id="adf1e-226">If you encounter any bugs with the tool, file an issue in the [Issues](https://github.com/Azure/azure-cli/issues) section of our GitHub repository.</span></span>
<span data-ttu-id="adf1e-227">Pour fournir des commentaires à partir de la ligne de commande, utilisez la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="adf1e-227">To provide feedback from the command line, use the `az feedback` command.</span></span>
