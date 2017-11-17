---
title: Installer Azure CLI 2.0
description: "Documents de référence pour l’installation d’Azure CLI 2.0"
keywords: "Azure CLI 2.0, Référence Azure CLI 2.0, Installer Azure CLI 2.0, interface de ligne de commande Python Azure, Désinstaller Azure CLI 2.0"
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 08/17/2017
ms.topic: "articleå"
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: ea5c0ee1-c530-4a1e-a83f-e1be71f6d416
ms.openlocfilehash: 432edac070e238a6f1be0ccd76b9b3582b082219
ms.sourcegitcommit: 2ec80224c6b831e31038b710d912c0dbb1ddfef6
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/17/2017
---
# <a name="install-azure-cli-20"></a><span data-ttu-id="871e5-104">Installer Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="871e5-104">Install Azure CLI 2.0</span></span>

<span data-ttu-id="871e5-105">Installez la nouvelle version de l’interface de ligne de commande Azure dès aujourd’hui.</span><span class="sxs-lookup"><span data-stu-id="871e5-105">Install the new version of the Azure CLI today!</span></span>
<span data-ttu-id="871e5-106">Nous avons amélioré et mis à jour cette interface afin d’offrir une expérience de ligne de commande native d’exception pour la gestion des ressources Azure.</span><span class="sxs-lookup"><span data-stu-id="871e5-106">We've improved and updated it to provide a great native command-line experience for managing Azure resources.</span></span>
<span data-ttu-id="871e5-107">Elle peut être utilisée sur macOS, Linux et Windows.</span><span class="sxs-lookup"><span data-stu-id="871e5-107">It can be used on macOS, Linux, and Windows.</span></span>
<span data-ttu-id="871e5-108">Pour plus d’informations sur la version la plus récente, consultez les [Notes de publication](release-notes-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="871e5-108">For information about the latest release, see the [release notes](release-notes-azure-cli.md).</span></span>

> [!NOTE]
> <span data-ttu-id="871e5-109">Si vous devez utiliser la version précédente d’Azure CLI, voici comment [installer Azure 1.0](/azure/cli-install-nodejs).</span><span class="sxs-lookup"><span data-stu-id="871e5-109">If you need the previous version of the Azure CLI, here's how to [install Azure CLI 1.0](/azure/cli-install-nodejs).</span></span>

## <a name="macos"></a><span data-ttu-id="871e5-110">macOS</span><span class="sxs-lookup"><span data-stu-id="871e5-110">macOS</span></span>

> [!WARNING]
> <span data-ttu-id="871e5-111">La formule Homebrew pour Azure CLI, `azure-cli`, n’est plus à jour actuellement. Une version antérieure sera installée.</span><span class="sxs-lookup"><span data-stu-id="871e5-111">The Homebrew formula for the Azure CLI, `azure-cli`, is currently out of date and will install a previous version.</span></span>

1. <span data-ttu-id="871e5-112">Installez Azure CLI 2.0 avec une commande `curl`.</span><span class="sxs-lookup"><span data-stu-id="871e5-112">Install Azure CLI 2.0 with one `curl` command.</span></span>

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

2. <span data-ttu-id="871e5-113">Vous devrez peut-être redémarrer votre interface de commande pour que certaines modifications soient prises en compte.</span><span class="sxs-lookup"><span data-stu-id="871e5-113">You may have to restart your command shell for some changes to take effect.</span></span>

   ```bash
   exec -l $SHELL
   ```
   
3. <span data-ttu-id="871e5-114">Exécutez l’interface de ligne de commande Azure 2.0 à partir de l’invite de commandes avec la commande `az` .</span><span class="sxs-lookup"><span data-stu-id="871e5-114">Run the CLI from the command prompt with the `az` command.</span></span>

> [!Note]
> <span data-ttu-id="871e5-115">Lorsque vous effectuez l’installation avec InstallAzureCli, [`az component update`](/cli/azure/component#update) n’est pas pris en charge.</span><span class="sxs-lookup"><span data-stu-id="871e5-115">When you install with InstallAzureCli, [`az component update`](/cli/azure/component#update) isn't supported.</span></span>
> <span data-ttu-id="871e5-116">Pour mettre à jour l’interface de ligne de commande avec la dernière version, ré-exécutez `curl -L https://aka.ms/InstallAzureCli | bash`.</span><span class="sxs-lookup"><span data-stu-id="871e5-116">To update to the latest CLI, run `curl -L https://aka.ms/InstallAzureCli | bash` again.</span></span>
> 
> <span data-ttu-id="871e5-117">Pour désinstaller l’interface, reportez-vous aux [instructions de désinstallation manuelle](#uninstall).</span><span class="sxs-lookup"><span data-stu-id="871e5-117">To uninstall, see the [manual uninstall instructions](#uninstall).</span></span>

## <a name="windows"></a><span data-ttu-id="871e5-118">Windows</span><span class="sxs-lookup"><span data-stu-id="871e5-118">Windows</span></span>

<span data-ttu-id="871e5-119">Vous pouvez installer Azure CLI 2.0 avec l’identité de service administré et l’utiliser dans la ligne de commande Windows, ou vous pouvez installer l’interface CLI avec apt-get sur Bash sous Ubuntu ou Windows.</span><span class="sxs-lookup"><span data-stu-id="871e5-119">You can install Azure CLI 2.0 with the MSI and use it in the Windows command-line, or you can install the CLI with apt-get on Bash on Ubuntu on Windows.</span></span>

### <a name="msi-for-the-windows-command-line"></a><span data-ttu-id="871e5-120">MSI pour la ligne de commande Windows</span><span class="sxs-lookup"><span data-stu-id="871e5-120">MSI for the Windows command-line</span></span> 

<span data-ttu-id="871e5-121">Pour installer l’interface de ligne de commande sous Windows et l’utiliser dans la ligne de commande Windows, téléchargez et exécutez le [msi](https://aka.ms/InstallAzureCliWindows).</span><span class="sxs-lookup"><span data-stu-id="871e5-121">To install the CLI on Windows and use it in the Windows command-line, download and run the [msi](https://aka.ms/InstallAzureCliWindows).</span></span>

> [!NOTE]
> <span data-ttu-id="871e5-122">Lorsque vous installez l’identité de service administré, [`az component`](/cli/azure/component) n’est pas pris en charge.</span><span class="sxs-lookup"><span data-stu-id="871e5-122">When you install with the msi, [`az component`](/cli/azure/component) isn't supported.</span></span>
> <span data-ttu-id="871e5-123">Pour mettre à jour vers l’interface de ligne de commande la plus récente, réexécutez le [msi](https://aka.ms/InstallAzureCliWindows).</span><span class="sxs-lookup"><span data-stu-id="871e5-123">To update to the latest CLI, run the [msi](https://aka.ms/InstallAzureCliWindows) again.</span></span>
> 
> <span data-ttu-id="871e5-124">Pour désinstaller l’interface de ligne de commande, réexécutez le [msi](https://aka.ms/InstallAzureCliWindows) et choisissez Désinstaller.</span><span class="sxs-lookup"><span data-stu-id="871e5-124">To uninstall the CLI, run the [msi](https://aka.ms/InstallAzureCliWindows) again and choose uninstall.</span></span>

### <a name="apt-get-for-bash-on-ubuntu-on-windows"></a><span data-ttu-id="871e5-125">apt-get pour Bash sur Ubuntu sous Windows</span><span class="sxs-lookup"><span data-stu-id="871e5-125">apt-get for Bash on Ubuntu on Windows</span></span>

1. <span data-ttu-id="871e5-126">Si vous ne disposez pas de Bash sur Windows, [installez-le](https://msdn.microsoft.com/commandline/wsl/install_guide).</span><span class="sxs-lookup"><span data-stu-id="871e5-126">If you don't have Bash on Windows, [install it](https://msdn.microsoft.com/commandline/wsl/install_guide).</span></span>

2. <span data-ttu-id="871e5-127">Ouvrez l’interpréteur de commandes Bash.</span><span class="sxs-lookup"><span data-stu-id="871e5-127">Open the Bash shell.</span></span>

3. <span data-ttu-id="871e5-128">Modifiez votre liste de sources.</span><span class="sxs-lookup"><span data-stu-id="871e5-128">Modify your sources list.</span></span>

   ```bash
   echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
   ```

4. <span data-ttu-id="871e5-129">Exécutez les commandes sudo suivantes :</span><span class="sxs-lookup"><span data-stu-id="871e5-129">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

5.  <span data-ttu-id="871e5-130">Exécutez l’interface de ligne de commande Azure 2.0 à partir de l’invite de commandes avec la commande `az` .</span><span class="sxs-lookup"><span data-stu-id="871e5-130">Run the CLI from the command prompt with the `az` command.</span></span>

> [!NOTE]
> <span data-ttu-id="871e5-131">Lorsque vous effectuez l’installation avec apt-get, [`az component`](/cli/azure/component) n’est pas pris en charge.</span><span class="sxs-lookup"><span data-stu-id="871e5-131">When you install with apt-get, [`az component`](/cli/azure/component) isn't supported.</span></span>
> <span data-ttu-id="871e5-132">Pour mettre à jour l’interface de ligne de commande, ré-exécutez `sudo apt-get update && sudo apt-get install azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="871e5-132">To update the CLI, run `sudo apt-get update && sudo apt-get install azure-cli` again.</span></span>
> 
> <span data-ttu-id="871e5-133">Pour désinstaller l’interface, exécutez `sudo apt-get remove azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="871e5-133">To uninstall, run `sudo apt-get remove azure-cli`.</span></span>

## <a name="apt-get-for-debianubuntu"></a><span data-ttu-id="871e5-134">apt-get pour Debian/Ubuntu</span><span class="sxs-lookup"><span data-stu-id="871e5-134">apt-get for Debian/Ubuntu</span></span>

<span data-ttu-id="871e5-135">Dans le cas des systèmes Debian/Ubuntu, vous pouvez installer Azure CLI 2.0 par le biais de la commande `apt-get`.</span><span class="sxs-lookup"><span data-stu-id="871e5-135">For Debian/Ubuntu based systems, you can install Azure CLI 2.0 via `apt-get`.</span></span>

1. <span data-ttu-id="871e5-136">Modifiez votre liste de sources.</span><span class="sxs-lookup"><span data-stu-id="871e5-136">Modify your sources list.</span></span>
 
   - <span data-ttu-id="871e5-137">Système 32 bits</span><span class="sxs-lookup"><span data-stu-id="871e5-137">32-bit system</span></span>

     ```bash
     echo "deb https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

   - <span data-ttu-id="871e5-138">Système 64 bits</span><span class="sxs-lookup"><span data-stu-id="871e5-138">64-bit system</span></span>

     ```bash
     echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

2. <span data-ttu-id="871e5-139">Exécutez les commandes sudo suivantes :</span><span class="sxs-lookup"><span data-stu-id="871e5-139">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

3.  <span data-ttu-id="871e5-140">Exécutez l’interface de ligne de commande Azure 2.0 à partir de l’invite de commandes avec la commande `az` .</span><span class="sxs-lookup"><span data-stu-id="871e5-140">Run the CLI from the command prompt with the `az` command.</span></span>

> [!NOTE]
> <span data-ttu-id="871e5-141">Lorsque vous effectuez l’installation avec apt-get, [`az component`](/cli/azure/component) n’est pas pris en charge.</span><span class="sxs-lookup"><span data-stu-id="871e5-141">When you install with apt-get, [`az component`](/cli/azure/component) isn't supported.</span></span>
> <span data-ttu-id="871e5-142">Pour mettre à jour l’interface de ligne de commande, ré-exécutez `sudo apt-get update && sudo apt-get install azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="871e5-142">To update the CLI, run `sudo apt-get update && sudo apt-get install azure-cli` again.</span></span>
> 
> <span data-ttu-id="871e5-143">Pour désinstaller l’interface, exécutez `sudo apt-get remove azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="871e5-143">To uninstall, run `sudo apt-get remove azure-cli`.</span></span>

## <a name="docker"></a><span data-ttu-id="871e5-144">Docker</span><span class="sxs-lookup"><span data-stu-id="871e5-144">Docker</span></span>

<span data-ttu-id="871e5-145">Nous fournissons une image Docker pré-configurée avec l’interface de ligne de commande Azure 2.0.</span><span class="sxs-lookup"><span data-stu-id="871e5-145">We maintain a Docker image preconfigured with the Azure CLI 2.0.</span></span>

<span data-ttu-id="871e5-146">Installez l’interface de ligne de commande à l’aide de `docker run`.</span><span class="sxs-lookup"><span data-stu-id="871e5-146">Install the CLI using `docker run`.</span></span>

```bash
docker run azuresdk/azure-cli-python:<version>
```

<span data-ttu-id="871e5-147">Consultez nos [balises Docker](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/) pour connaître les versions disponibles.</span><span class="sxs-lookup"><span data-stu-id="871e5-147">See our [Docker tags](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/) for available versions.</span></span>

> [!NOTE]
> <span data-ttu-id="871e5-148">Si vous souhaitez sélectionner les clés SSH à partir de votre environnement utilisateur, vous pouvez utiliser `-v ${HOME}:/root` pour monter $HOME en tant que `/root`.</span><span class="sxs-lookup"><span data-stu-id="871e5-148">If you want to pick up the SSH keys from your user environment, you can use `-v ${HOME}:/root` to mount $HOME as `/root`.</span></span>

>> ```bash
> docker run -v ${HOME}:/root azuresdk/azure-cli-python:<version>
> ```

<span data-ttu-id="871e5-149">L’interface de ligne de commande est installé sur l’image en tant que commande `az` dans `/usr/local/bin`.</span><span class="sxs-lookup"><span data-stu-id="871e5-149">The CLI is installed on the image as the `az` command in `/usr/local/bin`.</span></span>

> [!NOTE]
> <span data-ttu-id="871e5-150">L’image Docker ne prend pas en charge la fonctionnalité [`az component`](/cli/azure/component).</span><span class="sxs-lookup"><span data-stu-id="871e5-150">The Docker image does not support the [`az component`](/cli/azure/component) feature.</span></span>
> <span data-ttu-id="871e5-151">Pour mettre à jour l’interface de ligne de commande avec la version Azure CLI 2.0, utilisez `docker run` afin d’installer la dernière image ou l’image qui vous intéresse.</span><span class="sxs-lookup"><span data-stu-id="871e5-151">To update the Azure CLI 2.0, use `docker run` to install the latest image, or the specific image that you want.</span></span>

## <a name="linux"></a><span data-ttu-id="871e5-152">Linux</span><span class="sxs-lookup"><span data-stu-id="871e5-152">Linux</span></span>

1. <span data-ttu-id="871e5-153">Installez [Python](https://www.python.org/downloads) si vous ne l’avez pas encore fait.</span><span class="sxs-lookup"><span data-stu-id="871e5-153">If you don't have it, install [Python](https://www.python.org/downloads).</span></span>

2. <span data-ttu-id="871e5-154">Selon votre distribution Linux, installez les composants requis.</span><span class="sxs-lookup"><span data-stu-id="871e5-154">Depending on your Linux distribution, install the prerequisites.</span></span>

   ```
   Platform              | Prerequisites
   ----------------------|---------------------------------------------
   Ubuntu 15.10 or 16.04 | sudo apt-get update && sudo apt-get install -y libssl-dev libffi-dev python-dev build-essential
   Ubuntu 12.04 or 14.04 | sudo apt-get update && sudo apt-get install -y libssl-dev libffi-dev python-dev
   Debian 8              | sudo apt-get update && sudo apt-get install -y libssl-dev libffi-dev python-dev build-essential
   Debian 7              | sudo apt-get update && sudo apt-get install -y libssl-dev libffi-dev python-dev
   CentOS 7.1 or 7.2     | sudo yum check-update; sudo yum install -y gcc libffi-devel python-devel openssl-devel
   RedHat 7.2            | sudo yum check-update; sudo yum install -y gcc libffi-devel python-devel openssl-devel
   SUSE OpenSUSE 13.2    | sudo zypper refresh && sudo zypper --non-interactive install gcc libffi-devel python-devel openssl-devel
   ```

3. <span data-ttu-id="871e5-155">Installez l’interface CLI à l’aide d’une commande `curl`.</span><span class="sxs-lookup"><span data-stu-id="871e5-155">Install the CLI with one `curl` command.</span></span>

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

4. <span data-ttu-id="871e5-156">Vous devrez peut-être redémarrer votre interface de commande pour que certaines modifications soient prises en compte.</span><span class="sxs-lookup"><span data-stu-id="871e5-156">You may have to restart your command shell for some changes to take effect.</span></span>

   ```bash
   exec -l $SHELL
   ```

5. <span data-ttu-id="871e5-157">Exécutez l’interface de ligne de commande Azure 2.0 à partir de l’invite de commandes avec la commande `az` .</span><span class="sxs-lookup"><span data-stu-id="871e5-157">Run the CLI from the command prompt with the `az` command.</span></span>

> [!Note]
> <span data-ttu-id="871e5-158">Lorsque vous effectuez l’installation avec InstallAzureCli, [`az component update`](/cli/azure/component#update) n’est pas pris en charge.</span><span class="sxs-lookup"><span data-stu-id="871e5-158">When you install with InstallAzureCli, [`az component update`](/cli/azure/component#update) isn't supported.</span></span>
> <span data-ttu-id="871e5-159">Pour mettre à jour l’interface de ligne de commande avec la dernière version, ré-exécutez `curl -L https://aka.ms/InstallAzureCli | bash`.</span><span class="sxs-lookup"><span data-stu-id="871e5-159">To update to the latest CLI, run `curl -L https://aka.ms/InstallAzureCli | bash` again.</span></span>
> 
> <span data-ttu-id="871e5-160">Pour désinstaller l’interface, reportez-vous aux [instructions de désinstallation manuelle](#uninstall).</span><span class="sxs-lookup"><span data-stu-id="871e5-160">To uninstall, see the [manual uninstall instructions](#uninstall).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="871e5-161">Résolution des problèmes</span><span class="sxs-lookup"><span data-stu-id="871e5-161">Troubleshooting</span></span>

### <a name="errors-with-curl-redirection"></a><span data-ttu-id="871e5-162">Erreurs de redirection curl</span><span class="sxs-lookup"><span data-stu-id="871e5-162">Errors with curl redirection</span></span>

<span data-ttu-id="871e5-163">Si la commande `curl` renvoie une erreur concernant le paramètre `-L` ou un message d’erreur « Objet déplacé », essayez d’utiliser l’URL complète plutôt que l’URL aka.ms :</span><span class="sxs-lookup"><span data-stu-id="871e5-163">If you get an error from the `curl` command regarding the `-L` parameter, or an error saying "Object Moved", try using the full url instead of the aka.ms url:</span></span>

```
# If you see this:
curl -L https://aka.ms/InstallAzureCli | bash
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100   175  100   175    0     0    562      0 --:--:-- --:--:-- --:--:--   560
bash: line 1: syntax error near unexpected token `<'
'ash: line 1: `<html><head><title>Object moved</title></head><body>

#### Try this instead:
curl https://azurecliprod.blob.core.windows.net/install | bash
```

## <a name="uninstall"></a><span data-ttu-id="871e5-164">Désinstaller l’interface</span><span class="sxs-lookup"><span data-stu-id="871e5-164">Uninstall</span></span>

<span data-ttu-id="871e5-165">Si vous avez installé l’interface de ligne de commande en utilisant le script accessible à l’adresse https://aka.ms/InstallAzureCli, vous pouvez désinstaller l’interface à l’aide de la procédure suivante.</span><span class="sxs-lookup"><span data-stu-id="871e5-165">If you used the script at https://aka.ms/InstallAzureCli to install the CLI, you can uninstall it with these steps.</span></span>

1. <span data-ttu-id="871e5-166">Supprimez les fichiers installés.</span><span class="sxs-lookup"><span data-stu-id="871e5-166">Remove the installed files.</span></span>

   ```bash
   rm -r <install location>/lib/azure-cli
   rm <install location>/bin/az
   ```

2. <span data-ttu-id="871e5-167">Supprimez la ligne `<install location>/lib/azure-cli/az.completion` de `<install location>/.bash_profile`.</span><span class="sxs-lookup"><span data-stu-id="871e5-167">Delete the line `<install location>/lib/azure-cli/az.completion` from `<install location>/.bash_profile`.</span></span>

> [!Note]
> <span data-ttu-id="871e5-168">L’emplacement d’installation par défaut est `/Users/<username>`.</span><span class="sxs-lookup"><span data-stu-id="871e5-168">The default install location is `/Users/<username>`.</span></span>

<span data-ttu-id="871e5-169">Si vous avez utilisé apt-get, Docker ou le msi pour installer l’interface de ligne de commande, utilisez le même outil pour la désinstaller.</span><span class="sxs-lookup"><span data-stu-id="871e5-169">If you used apt-get, Docker, or the msi to install the CLI, use the same tool to uninstall it.</span></span>

## <a name="reporting-issues-and-feedback"></a><span data-ttu-id="871e5-170">Signalement de problèmes et envoi de commentaires</span><span class="sxs-lookup"><span data-stu-id="871e5-170">Reporting issues and feedback</span></span>

<span data-ttu-id="871e5-171">Si vous rencontrez des bogues en utilisant l’outil, signalez un problème dans la section [Issues](https://github.com/Azure/azure-cli/issues) (Problèmes) de notre référentiel GitHub.</span><span class="sxs-lookup"><span data-stu-id="871e5-171">If you encounter any bugs with the tool, file an issue in the [Issues](https://github.com/Azure/azure-cli/issues) section of our GitHub repo.</span></span>
<span data-ttu-id="871e5-172">Pour fournir des commentaires à partir de la ligne de commande, essayez la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="871e5-172">To provide feedback from the command line, try the `az feedback` command.</span></span>
