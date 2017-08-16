---
title: Installer Azure CLI 2.0
description: "Documents de référence concernant Azure CLI 2.0"
keywords: "Azure CLI 2.0, Référence Azure CLI 2.0, Installer Azure CLI 2.0, interface de ligne de commande Python Azure, Désinstaller Azure CLI 2.0"
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 04/06/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: ea5c0ee1-c530-4a1e-a83f-e1be71f6d416
ms.openlocfilehash: 7065ed5270ef9bfc70beea81d0bc442a7b4df38c
ms.sourcegitcommit: c077bd5cbe07f7225714c41714d3981fa0d9928f
ms.contentlocale: fr-FR
ms.lasthandoff: 05/16/2017
---
# <a name="install-azure-cli-20"></a><span data-ttu-id="bcf31-104">Installer Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="bcf31-104">Install Azure CLI 2.0</span></span>

<span data-ttu-id="bcf31-105">Installez la nouvelle version de l’interface de ligne de commande Azure dès aujourd’hui.</span><span class="sxs-lookup"><span data-stu-id="bcf31-105">Install the new version of the Azure CLI today!</span></span>
<span data-ttu-id="bcf31-106">Nous avons amélioré et mis à jour cette interface afin d’offrir une expérience de ligne de commande native d’exception pour la gestion des ressources Azure.</span><span class="sxs-lookup"><span data-stu-id="bcf31-106">We've improved and updated it to provide a great native command-line experience for managing Azure resources.</span></span>
<span data-ttu-id="bcf31-107">Elle peut être utilisée sur macOS, Linux et Windows.</span><span class="sxs-lookup"><span data-stu-id="bcf31-107">It can be used on macOS, Linux, and Windows.</span></span>
<span data-ttu-id="bcf31-108">Pour plus d’informations sur la version la plus récente, consultez les [notes de publication](release-notes-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="bcf31-108">For information about the latest release, see the [release notes](release-notes-azure-cli.md).</span></span>

> [!NOTE]
> <span data-ttu-id="bcf31-109">Si vous devez utiliser la version précédente d’Azure CLI, voici comment [installer Azure 1.0](/azure/cli-install-nodejs).</span><span class="sxs-lookup"><span data-stu-id="bcf31-109">If you need the previous version of the Azure CLI, here's how to [install Azure 1.0](/azure/cli-install-nodejs).</span></span>

## <a name="macos"></a><span data-ttu-id="bcf31-110">macOS</span><span class="sxs-lookup"><span data-stu-id="bcf31-110">macOS</span></span>

1. <span data-ttu-id="bcf31-111">Installez Azure CLI 2.0 avec une commande `curl`.</span><span class="sxs-lookup"><span data-stu-id="bcf31-111">Install Azure CLI 2.0 with one `curl` command.</span></span>

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

2. <span data-ttu-id="bcf31-112">Vous devrez peut-être redémarrer votre interface de commande pour que certaines modifications soient prises en compte.</span><span class="sxs-lookup"><span data-stu-id="bcf31-112">You may have to restart your command shell for some changes to take effect.</span></span>

   ```bash
   exec -l $SHELL
   ```
   
3. <span data-ttu-id="bcf31-113">Exécutez Azure CLI 2.0 à partir de l’invite de commandes avec la commande `az`.</span><span class="sxs-lookup"><span data-stu-id="bcf31-113">Run Azure CLI 2.0 from the command prompt with the `az` command.</span></span>

> [!Note]
> <span data-ttu-id="bcf31-114">Lorsque vous effectuez l’installation avec InstallAzureCli, `az component update` n’est pas pris en charge.</span><span class="sxs-lookup"><span data-stu-id="bcf31-114">When you install with InstallAzureCli, `az component update` isn't supported.</span></span>
> <span data-ttu-id="bcf31-115">Pour mettre à jour l’interface de ligne de commande avec la dernière version, ré-exécutez `curl -L https://aka.ms/InstallAzureCli | bash`.</span><span class="sxs-lookup"><span data-stu-id="bcf31-115">To update to the latest CLI, run `curl -L https://aka.ms/InstallAzureCli | bash` again.</span></span>
> 
> <span data-ttu-id="bcf31-116">Pour désinstaller l’interface, reportez-vous aux [instructions de désinstallation manuelle](#uninstall).</span><span class="sxs-lookup"><span data-stu-id="bcf31-116">To uninstall, see the [manual uninstall instructions](#uninstall).</span></span>

## <a name="windows"></a><span data-ttu-id="bcf31-117">Windows</span><span class="sxs-lookup"><span data-stu-id="bcf31-117">Windows</span></span>

<span data-ttu-id="bcf31-118">Vous pouvez installer l’interface de ligne de commande avec le MSI et l’utiliser dans la ligne de commande Windows, ou vous pouvez installer l’interface de ligne de commande avec apt-get avec Bash sur Ubuntu sous Windows.</span><span class="sxs-lookup"><span data-stu-id="bcf31-118">You can install the CLI with the MSI and use it in the Windows command-line, or you can install the CLI with apt-get on Bash on Ubuntu on Windows.</span></span>

### <a name="msi-for-the-windows-command-line"></a><span data-ttu-id="bcf31-119">MSI pour la ligne de commande Windows</span><span class="sxs-lookup"><span data-stu-id="bcf31-119">MSI for the Windows command-line</span></span> 

<span data-ttu-id="bcf31-120">Pour installer l’interface de ligne de commande sous Windows et l’utiliser dans la ligne de commande Windows, téléchargez et exécutez le [msi](https://aka.ms/InstallAzureCliWindows).</span><span class="sxs-lookup"><span data-stu-id="bcf31-120">To install the CLI on Windows and use it in the Windows command-line, download and run the [msi](https://aka.ms/InstallAzureCliWindows).</span></span>

> [!NOTE]
> <span data-ttu-id="bcf31-121">Lorsque vous installez le msi, `az component` n’est pas pris en charge.</span><span class="sxs-lookup"><span data-stu-id="bcf31-121">When you install with the msi, `az component` isn't supported.</span></span>
> <span data-ttu-id="bcf31-122">Pour mettre à jour vers l’interface de ligne de commande la plus récente, réexécutez le [msi](https://aka.ms/InstallAzureCliWindows).</span><span class="sxs-lookup"><span data-stu-id="bcf31-122">To update to the latest CLI, run the [msi](https://aka.ms/InstallAzureCliWindows) again.</span></span>
> 
> <span data-ttu-id="bcf31-123">Pour désinstaller l’interface de ligne de commande, réexécutez le [msi](https://aka.ms/InstallAzureCliWindows) et choisissez Désinstaller.</span><span class="sxs-lookup"><span data-stu-id="bcf31-123">To uninstall the CLI, run the [msi](https://aka.ms/InstallAzureCliWindows) again and choose uninstall.</span></span>

### <a name="apt-get-for-bash-on-ubuntu-on-windows"></a><span data-ttu-id="bcf31-124">apt-get pour Bash sur Ubuntu sous Windows</span><span class="sxs-lookup"><span data-stu-id="bcf31-124">apt-get for Bash on Ubuntu on Windows</span></span>

1. <span data-ttu-id="bcf31-125">Si vous ne disposez pas de Bash sur Windows, [installez-le](https://msdn.microsoft.com/commandline/wsl/install_guide).</span><span class="sxs-lookup"><span data-stu-id="bcf31-125">If you don't have Bash on Windows, [install it](https://msdn.microsoft.com/commandline/wsl/install_guide).</span></span>

2. <span data-ttu-id="bcf31-126">Ouvrez l’interpréteur de commandes Bash.</span><span class="sxs-lookup"><span data-stu-id="bcf31-126">Open the Bash shell.</span></span>

3. <span data-ttu-id="bcf31-127">Modifiez votre liste de sources.</span><span class="sxs-lookup"><span data-stu-id="bcf31-127">Modify your sources list.</span></span>

   ```bash
   echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
   ```

4. <span data-ttu-id="bcf31-128">Exécutez les commandes sudo suivantes :</span><span class="sxs-lookup"><span data-stu-id="bcf31-128">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

> [!NOTE]
> <span data-ttu-id="bcf31-129">Lorsque vous effectuez l’installation avec apt-get, `az component` n’est pas pris en charge.</span><span class="sxs-lookup"><span data-stu-id="bcf31-129">When you install with apt-get, `az component` isn't supported.</span></span>
> <span data-ttu-id="bcf31-130">Pour mettre à jour l’interface de ligne de commande, ré-exécutez `sudo apt-get update && sudo apt-get install azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="bcf31-130">To update the CLI, run `sudo apt-get update && sudo apt-get install azure-cli` again.</span></span>
> 
> <span data-ttu-id="bcf31-131">Pour désinstaller l’interface, exécutez `sudo apt-get remove azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="bcf31-131">To uninstall, run `sudo apt-get remove azure-cli`.</span></span>

## <a name="linux"></a><span data-ttu-id="bcf31-132">Linux</span><span class="sxs-lookup"><span data-stu-id="bcf31-132">Linux</span></span>

1. <span data-ttu-id="bcf31-133">Sur Linux, vous pouvez avoir besoin d’installer des [composants requis](#linux-prerequisites) spécifiques.</span><span class="sxs-lookup"><span data-stu-id="bcf31-133">On Linux, you may need to install specific [prerequisites](#linux-prerequisites).</span></span>

2. <span data-ttu-id="bcf31-134">Installez Azure CLI 2.0 avec une commande `curl`.</span><span class="sxs-lookup"><span data-stu-id="bcf31-134">Install Azure CLI 2.0 with one `curl` command.</span></span>

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

3. <span data-ttu-id="bcf31-135">Vous devrez peut-être redémarrer votre interface de commande pour que certaines modifications soient prises en compte.</span><span class="sxs-lookup"><span data-stu-id="bcf31-135">You may have to restart your command shell for some changes to take effect.</span></span>

   ```bash
   exec -l $SHELL
   ```

4. <span data-ttu-id="bcf31-136">Exécutez Azure CLI 2.0 à partir de l’invite de commandes avec la commande `az`.</span><span class="sxs-lookup"><span data-stu-id="bcf31-136">Run Azure CLI 2.0 from the command prompt with the `az` command.</span></span>

> [!Note]
> <span data-ttu-id="bcf31-137">Lorsque vous effectuez l’installation avec InstallAzureCli, `az component update` n’est pas pris en charge.</span><span class="sxs-lookup"><span data-stu-id="bcf31-137">When you install with InstallAzureCli, `az component update` isn't supported.</span></span>
> <span data-ttu-id="bcf31-138">Pour mettre à jour l’interface de ligne de commande avec la dernière version, ré-exécutez `curl -L https://aka.ms/InstallAzureCli | bash`.</span><span class="sxs-lookup"><span data-stu-id="bcf31-138">To update to the latest CLI, run `curl -L https://aka.ms/InstallAzureCli | bash` again.</span></span>
> 
> <span data-ttu-id="bcf31-139">Pour désinstaller l’interface, reportez-vous aux [instructions de désinstallation manuelle](#uninstall).</span><span class="sxs-lookup"><span data-stu-id="bcf31-139">To uninstall, see the [manual uninstall instructions](#uninstall).</span></span>

## <a name="docker"></a><span data-ttu-id="bcf31-140">Docker</span><span class="sxs-lookup"><span data-stu-id="bcf31-140">Docker</span></span>

<span data-ttu-id="bcf31-141">Nous fournissons une image Docker préconfigurée avec l’interface de ligne de commande Azure.</span><span class="sxs-lookup"><span data-stu-id="bcf31-141">We maintain a Docker image preconfigured with the Azure CLI.</span></span>

<span data-ttu-id="bcf31-142">Installez l’interface de ligne de commande Azure à l’aide de la commande `docker run`.</span><span class="sxs-lookup"><span data-stu-id="bcf31-142">Install the Azure CLI using `docker run`.</span></span>

```bash
docker run azuresdk/azure-cli-python:<version>
```

<span data-ttu-id="bcf31-143">Consultez nos [balises Docker](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/) pour connaître les versions disponibles.</span><span class="sxs-lookup"><span data-stu-id="bcf31-143">See our [Docker tags](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/) for available versions.</span></span>

> [!NOTE]
> <span data-ttu-id="bcf31-144">Si vous souhaitez sélectionner les clés SSH à partir de votre environnement utilisateur, vous pouvez utiliser `-v ${HOME}:/root` pour monter $HOME en tant que `/root`.</span><span class="sxs-lookup"><span data-stu-id="bcf31-144">If you want to pick up the SSH keys from your user environment, you can use `-v ${HOME}:/root` to mount $HOME as `/root`.</span></span>
>
> ```bash
> docker run -v ${HOME}:/root azuresdk/azure-cli-python:<version>
> ```

> [!NOTE]
> <span data-ttu-id="bcf31-145">L’image Docker ne prend pas en charge la [fonctionnalité `component`](/cli/azure/component).</span><span class="sxs-lookup"><span data-stu-id="bcf31-145">The Docker image does not support the [`component` feature](/cli/azure/component).</span></span>
> <span data-ttu-id="bcf31-146">Pour mettre à jour l’interface de ligne de commande avec la version Azure CLI 2.0, utilisez `docker run` afin d’installer la dernière image ou l’image qui vous intéresse.</span><span class="sxs-lookup"><span data-stu-id="bcf31-146">To update the Azure CLI 2.0, use `docker run` to install the latest image, or the specific image that you want.</span></span>

## <a name="apt-get"></a><span data-ttu-id="bcf31-147">apt-get</span><span class="sxs-lookup"><span data-stu-id="bcf31-147">apt-get</span></span>

<span data-ttu-id="bcf31-148">Dans le cas des systèmes Debian/Ubuntu, vous pouvez installer Azure CLI 2.0 par le biais de la commande `apt-get`.</span><span class="sxs-lookup"><span data-stu-id="bcf31-148">For Debian/Ubuntu based systems, you can install Azure CLI 2.0 via `apt-get`.</span></span>

1. <span data-ttu-id="bcf31-149">Modifiez votre liste de sources.</span><span class="sxs-lookup"><span data-stu-id="bcf31-149">Modify your sources list.</span></span>

   - <span data-ttu-id="bcf31-150">Système 32 bits</span><span class="sxs-lookup"><span data-stu-id="bcf31-150">32-bit system</span></span>

     ```bash
     echo "deb https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

   - <span data-ttu-id="bcf31-151">Système 64 bits</span><span class="sxs-lookup"><span data-stu-id="bcf31-151">64-bit system</span></span>

     ```bash
     echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

2. <span data-ttu-id="bcf31-152">Exécutez les commandes sudo suivantes :</span><span class="sxs-lookup"><span data-stu-id="bcf31-152">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

> [!NOTE]
> <span data-ttu-id="bcf31-153">Lorsque vous effectuez l’installation avec apt-get, `az component` n’est pas pris en charge.</span><span class="sxs-lookup"><span data-stu-id="bcf31-153">When you install with apt-get, `az component` isn't supported.</span></span>
> <span data-ttu-id="bcf31-154">Pour mettre à jour l’interface de ligne de commande, ré-exécutez `sudo apt-get update && sudo apt-get install azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="bcf31-154">To update the CLI, run `sudo apt-get update && sudo apt-get install azure-cli` again.</span></span>
> 
> <span data-ttu-id="bcf31-155">Pour désinstaller l’interface, exécutez `sudo apt-get remove azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="bcf31-155">To uninstall, run `sudo apt-get remove azure-cli`.</span></span>

## <a name="linux-prerequisites"></a><span data-ttu-id="bcf31-156">Composants requis Linux</span><span class="sxs-lookup"><span data-stu-id="bcf31-156">Linux Prerequisites</span></span>

1. <span data-ttu-id="bcf31-157">Installez [Python](https://www.python.org/downloads) si vous ne l’avez pas encore fait.</span><span class="sxs-lookup"><span data-stu-id="bcf31-157">If you don't have it, install [Python](https://www.python.org/downloads).</span></span>

2. <span data-ttu-id="bcf31-158">Selon votre distribution Linux, installez les composants requis.</span><span class="sxs-lookup"><span data-stu-id="bcf31-158">Depending on your Linux distribution, install the prerequisites.</span></span>

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

## <a name="troubleshooting"></a><span data-ttu-id="bcf31-159">Résolution des problèmes</span><span class="sxs-lookup"><span data-stu-id="bcf31-159">Troubleshooting</span></span>

### <a name="errors-with-curl-redirection"></a><span data-ttu-id="bcf31-160">Erreurs de redirection curl</span><span class="sxs-lookup"><span data-stu-id="bcf31-160">Errors with curl redirection</span></span>

<span data-ttu-id="bcf31-161">Si la commande `curl` renvoie une erreur concernant le paramètre `-L` ou un message d’erreur « Objet déplacé », essayez d’utiliser l’URL complète plutôt que l’URL aka.ms :</span><span class="sxs-lookup"><span data-stu-id="bcf31-161">If you get an error from the `curl` command regarding the `-L` parameter, or an error saying "Object Moved", try using the full url instead of the aka.ms url:</span></span>

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

## <a name="uninstall"></a><span data-ttu-id="bcf31-162">Désinstaller l’interface</span><span class="sxs-lookup"><span data-stu-id="bcf31-162">Uninstall</span></span>

<span data-ttu-id="bcf31-163">Si vous avez installé l’interface de ligne de commande en utilisant le script accessible à l’adresse https://aka.ms/InstallAzureCli, vous pouvez désinstaller l’interface à l’aide de la procédure suivante.</span><span class="sxs-lookup"><span data-stu-id="bcf31-163">If you used the script at https://aka.ms/InstallAzureCli to install the CLI, you can uninstall it with these steps.</span></span>

1. <span data-ttu-id="bcf31-164">Supprimez les fichiers installés.</span><span class="sxs-lookup"><span data-stu-id="bcf31-164">Remove the installed files.</span></span>

   ```bash
   rm -r <install location>/lib/azure-cli
   rm <install location>/bin/az
   ```

2. <span data-ttu-id="bcf31-165">Supprimez la ligne `<install location>/lib/azure-cli/az.completion` de `<install location>/.bash_profile`.</span><span class="sxs-lookup"><span data-stu-id="bcf31-165">Delete the line `<install location>/lib/azure-cli/az.completion` from `<install location>/.bash_profile`.</span></span>

> [!Note]
> <span data-ttu-id="bcf31-166">L’emplacement d’installation par défaut est `/Users/<username>`.</span><span class="sxs-lookup"><span data-stu-id="bcf31-166">The default install location is `/Users/<username>`.</span></span>

<span data-ttu-id="bcf31-167">Si vous avez utilisé apt-get, Docker ou le msi pour installer l’interface de ligne de commande, utilisez le même outil pour la désinstaller.</span><span class="sxs-lookup"><span data-stu-id="bcf31-167">If you used apt-get, Docker, or the msi to install the CLI, use the same tool to uninstall it.</span></span>

## <a name="reporting-issues-and-feedback"></a><span data-ttu-id="bcf31-168">Signalement de problèmes et envoi de commentaires</span><span class="sxs-lookup"><span data-stu-id="bcf31-168">Reporting issues and feedback</span></span>

<span data-ttu-id="bcf31-169">Si vous rencontrez des bogues en utilisant l’outil, signalez un problème dans la section [Issues](https://github.com/Azure/azure-cli/issues) (Problèmes) de notre référentiel GitHub.</span><span class="sxs-lookup"><span data-stu-id="bcf31-169">If you encounter any bugs with the tool, file an issue in the [Issues](https://github.com/Azure/azure-cli/issues) section of our GitHub repo.</span></span>
<span data-ttu-id="bcf31-170">Pour fournir des commentaires à partir de la ligne de commande, essayez la commande `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="bcf31-170">To provide feedback from the command line, try the `az feedback` command.</span></span>
