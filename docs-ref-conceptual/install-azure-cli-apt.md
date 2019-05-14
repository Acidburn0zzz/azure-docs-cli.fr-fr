---
title: Installer Azure CLI sur Linux avec apt
description: Comment installer Azure CLI avec le gestionnaire de package apt
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/08/2019
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: af82eea3fd549cbca85699a3030a19bc82574b73
ms.sourcegitcommit: c65c69bd08fd6b7632ba60dc7c8e9f2b57a9d0b7
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/09/2019
ms.locfileid: "65476257"
---
# <a name="install-azure-cli-with-apt"></a><span data-ttu-id="05320-103">Installer Azure CLI avec apt</span><span class="sxs-lookup"><span data-stu-id="05320-103">Install Azure CLI with apt</span></span>

<span data-ttu-id="05320-104">Si vous exécutez une distribution qui est fournie avec `apt`, telle que Ubuntu ou Debian, un package x86_64 est disponible pour Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="05320-104">If you are running a distribution that comes with `apt`, such as Ubuntu or Debian, there's an x86_64 package available for the Azure CLI.</span></span> <span data-ttu-id="05320-105">Ce package a été testé avec les systèmes pris en charge suivants :</span><span class="sxs-lookup"><span data-stu-id="05320-105">This package has been tested with and is supported for:</span></span>

* <span data-ttu-id="05320-106">Ubuntu trusty, xenial, artful, bionic et disco</span><span class="sxs-lookup"><span data-stu-id="05320-106">Ubuntu trusty, xenial, artful, bionic, and disco</span></span>
* <span data-ttu-id="05320-107">Debian wheezy, jessie, et stretch</span><span class="sxs-lookup"><span data-stu-id="05320-107">Debian wheezy, jessie, and stretch</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

> [!NOTE]
>
> <span data-ttu-id="05320-108">Le package Azure CLI installe son propre interpréteur Python et n’utilise pas le système Python.</span><span class="sxs-lookup"><span data-stu-id="05320-108">The package for Azure CLI installs its own Python interpreter, and does not use the system Python.</span></span>

## <a name="install"></a><span data-ttu-id="05320-109">Installer</span><span class="sxs-lookup"><span data-stu-id="05320-109">Install</span></span>

<span data-ttu-id="05320-110">Pour installer Azure CLI avec les distributions prenant en charge `apt`, vous pouvez soit utiliser un script tout-en-un qui exécute les commandes d’installation pour vous, soit suivre vous-même les instructions d’un processus étape par étape.</span><span class="sxs-lookup"><span data-stu-id="05320-110">We offer two ways to install the Azure CLI with distributions that support `apt`: As an all-in-one script that runs the install commands for you, and instructions that you can run as a step-by-step process on your own.</span></span>

### <a name="install-with-one-command"></a><span data-ttu-id="05320-111">Installer avec une seule commande</span><span class="sxs-lookup"><span data-stu-id="05320-111">Install with one command</span></span>

<span data-ttu-id="05320-112">Nous vous proposons un script à jour qui exécute toutes les commandes d’installation en une seule étape.</span><span class="sxs-lookup"><span data-stu-id="05320-112">We offer and maintain a script which runs all of the installation commands in one step.</span></span> <span data-ttu-id="05320-113">Pour l’exécuter, utilisez le pipe pour associer `curl` directement à `bash`, ou téléchargez le script dans un fichier et vérifiez-le avant de l’exécuter.</span><span class="sxs-lookup"><span data-stu-id="05320-113">Run it by using `curl` and pipe directly to `bash`, or download the script to a file and inspect it before running.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="05320-114">Ce script a été uniquement validé sur Ubuntu 16.04 et Debian 8+.</span><span class="sxs-lookup"><span data-stu-id="05320-114">This script is only verified for Ubuntu 16.04+ and Debian 8+.</span></span> <span data-ttu-id="05320-115">Il est possible qu’il ne fonctionne pas sur d’autres distributions.</span><span class="sxs-lookup"><span data-stu-id="05320-115">It may not work on other distributions.</span></span>
> <span data-ttu-id="05320-116">Si vous utilisez une distribution dérivée telle que Linux Mint, suivez les instructions d’installation manuelle et effectuez les opérations de dépannage nécessaires.</span><span class="sxs-lookup"><span data-stu-id="05320-116">If you're using a derived distribution such as Linux Mint, follow the manual install instructions and perform any necessary troubleshooting.</span></span>

```bash
curl -sL https://aka.ms/InstallAzureCLIDeb | sudo bash
```

### <a name="manual-install-instructions"></a><span data-ttu-id="05320-117">Instructions d’installation manuelle</span><span class="sxs-lookup"><span data-stu-id="05320-117">Manual install instructions</span></span>

<span data-ttu-id="05320-118">Si vous ne souhaitez pas exécuter un script en tant que superutilisateur, suivez ces étapes manuelles pour installer Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="05320-118">If you don't want to run a script as superuser, follow these manual steps to install the Azure CLI.</span></span>

1. <span data-ttu-id="05320-119">Récupérez les packages nécessaires au processus d’installation :</span><span class="sxs-lookup"><span data-stu-id="05320-119">Get packages needed for the install process:</span></span>

    ```bash
    sudo apt-get update
    sudo apt-get install curl apt-transport-https lsb-release gnupg
    ```

2. <span data-ttu-id="05320-120">Téléchargez et installez la clé de signature Microsoft :</span><span class="sxs-lookup"><span data-stu-id="05320-120">Download and install the Microsoft signing key:</span></span>

    ```bash
    curl -sL https://packages.microsoft.com/keys/microsoft.asc | \
        gpg --dearmor | \
        sudo tee /etc/apt/trusted.gpg.d/microsoft.asc.gpg > /dev/null
    ```

3. <div id="set-release"/><span data-ttu-id="05320-121">Ajoutez le référentiel de logiciels Azure CLI :</span><span class="sxs-lookup"><span data-stu-id="05320-121">Add the Azure CLI software repository:</span></span>

    ```bash
    AZ_REPO=$(lsb_release -cs)
    echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
    ```

4. <span data-ttu-id="05320-122">Mettez à jour les informations concernant le référentiel, puis installez le package `azure-cli` :</span><span class="sxs-lookup"><span data-stu-id="05320-122">Update repository information and install the `azure-cli` package:</span></span>

    ```bash
    sudo apt-get update
    sudo apt-get install azure-cli
    ```

<span data-ttu-id="05320-123">Exécutez Azure CLI avec la commande `az`.</span><span class="sxs-lookup"><span data-stu-id="05320-123">Run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="05320-124">Pour vous connecter, utilisez la commande [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="05320-124">To sign in, use the [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="05320-125">Pour en savoir plus sur les différentes méthodes d’authentification, consultez [Se connecter avec Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="05320-125">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="05320-126">Résolution de problèmes</span><span class="sxs-lookup"><span data-stu-id="05320-126">Troubleshooting</span></span>

<span data-ttu-id="05320-127">Voici certains problèmes courants lors de l’installation avec `apt`.</span><span class="sxs-lookup"><span data-stu-id="05320-127">Here are some common problems seen when installing with `apt`.</span></span> <span data-ttu-id="05320-128">Si vous rencontrez un problème n’étant pas évoqué ici, [signalez un problème sur github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="05320-128">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="lsbrelease-does-not-return-the-correct-base-distribution-version"></a><span data-ttu-id="05320-129">lsb_release ne renvoie pas la bonne version de la distribution de base</span><span class="sxs-lookup"><span data-stu-id="05320-129">lsb_release does not return the correct base distribution version</span></span>

<span data-ttu-id="05320-130">Certaines distributions Ubuntu ou Debian dérivées, telles que Linux Mint peuvent ne pas retourner le nom de version correct de `lsb_release`.</span><span class="sxs-lookup"><span data-stu-id="05320-130">Some Ubuntu- or Debian-derived distributions such as Linux Mint may not return the correct version name from `lsb_release`.</span></span> <span data-ttu-id="05320-131">Cette valeur est utilisée dans le processus d’installation pour déterminer le package à installer.</span><span class="sxs-lookup"><span data-stu-id="05320-131">This value is used in the install process to determine the package to install.</span></span> <span data-ttu-id="05320-132">Si vous connaissez le nom de code de la version Ubuntu ou Debian dont votre distribution est dérivée, vous pouvez définir la valeur `AZ_REPO` manuellement lors de l’[ajout du référentiel](#set-release).</span><span class="sxs-lookup"><span data-stu-id="05320-132">If you know the code name of the Ubuntu or Debian version your distribution is derived from, you can set the `AZ_REPO` value manually when [adding the repository](#set-release).</span></span> <span data-ttu-id="05320-133">Dans le cas contraire, recherchez des informations expliquant comment déterminer le nom de code de la distribution de base et définir `AZ_REPO` sur la valeur appropriée.</span><span class="sxs-lookup"><span data-stu-id="05320-133">Otherwise, look up information for your distribution on how to determine the base distribution code name and set `AZ_REPO` to the correct value.</span></span>

### <a name="no-package-for-your-distribution"></a><span data-ttu-id="05320-134">Aucun package pour votre distribution</span><span class="sxs-lookup"><span data-stu-id="05320-134">No package for your distribution</span></span>

<span data-ttu-id="05320-135">Après la publication d’une distribution, il peut se passer un certain temps avant que le package Azure CLI associé ne soit disponible.</span><span class="sxs-lookup"><span data-stu-id="05320-135">Sometimes it may be a while after a distribution is released before there's an Azure CLI package available for it.</span></span> <span data-ttu-id="05320-136">Azure CLI est conçu pour résister à de futures versions de dépendances, et repose sur peu d’entre elles.</span><span class="sxs-lookup"><span data-stu-id="05320-136">The Azure CLI designed to be resilient with regards to future versions of dependencies and rely on as few of them as possible.</span></span> <span data-ttu-id="05320-137">Si aucun package n’est disponible pour votre distribution de base, essayez d’utiliser le package d’une distribution antérieure.</span><span class="sxs-lookup"><span data-stu-id="05320-137">If there's no package available for your base distribution, try a package for an earlier distribution.</span></span>

<span data-ttu-id="05320-138">Pour cela, définissez la valeur de `AZ_REPO` manuellement lors de l’[ajout du référentiel](#set-release).</span><span class="sxs-lookup"><span data-stu-id="05320-138">To do this, set the value of `AZ_REPO` manually when [adding the repository](#set-release).</span></span> <span data-ttu-id="05320-139">Pour les distributions Ubuntu, utilisez le référentiel `disco`, et `stretch` pour les distributions Debian.</span><span class="sxs-lookup"><span data-stu-id="05320-139">For Ubuntu distributions use the `disco` repository, and for Debian distributions use `stretch`.</span></span> <span data-ttu-id="05320-140">Les distributions publiées avant Ubuntu Trusty et Debian Wheezy ne sont pas prises en charge.</span><span class="sxs-lookup"><span data-stu-id="05320-140">Distributions released before Ubuntu Trusty and Debian Wheezy are not supported.</span></span>

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="update"></a><span data-ttu-id="05320-141">Mettre à jour</span><span class="sxs-lookup"><span data-stu-id="05320-141">Update</span></span>

<span data-ttu-id="05320-142">Utilisez `apt-get upgrade` pour mettre à jour le package de l’interface de ligne de commande.</span><span class="sxs-lookup"><span data-stu-id="05320-142">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> <span data-ttu-id="05320-143">Cette commande met à niveau tous les packages installés sur votre système n’ayant pas de modification de dépendance.</span><span class="sxs-lookup"><span data-stu-id="05320-143">This command upgrades all of the installed packages on your system that have not had a dependency change.</span></span>
> <span data-ttu-id="05320-144">Pour mettre à niveau uniquement l’interface CLI, utilisez `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="05320-144">To upgrade the CLI only, use `apt-get install`.</span></span>
> 
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

## <a name="uninstall"></a><span data-ttu-id="05320-145">Désinstaller l’interface</span><span class="sxs-lookup"><span data-stu-id="05320-145">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="05320-146">Désinstaller avec `apt-get remove` :</span><span class="sxs-lookup"><span data-stu-id="05320-146">Uninstall with `apt-get remove`:</span></span>

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. <span data-ttu-id="05320-147">Si vous ne prévoyez pas de réinstaller l’interface CLI, supprimez les informations de référentiel Azure CLI :</span><span class="sxs-lookup"><span data-stu-id="05320-147">If you don't plan to reinstall the CLI, remove the Azure CLI repository information:</span></span>

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. <span data-ttu-id="05320-148">Supprimer la clé de signature :</span><span class="sxs-lookup"><span data-stu-id="05320-148">Remove the signing key:</span></span>

    ```bash
    sudo rm /etc/apt/trusted.gpg.d/microsoft.asc.gpg
    ```

4. <span data-ttu-id="05320-149">Supprimer tous les packages inutiles :</span><span class="sxs-lookup"><span data-stu-id="05320-149">Remove any unneeded packages:</span></span>

   ```bash
   sudo apt autoremove
   ```

## <a name="next-steps"></a><span data-ttu-id="05320-150">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="05320-150">Next Steps</span></span>

<span data-ttu-id="05320-151">Maintenant que vous avez installé l’interface CLI, découvrez ses fonctionnalités et ses commandes courantes.</span><span class="sxs-lookup"><span data-stu-id="05320-151">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="05320-152">Prise en main de l’interface Azure CLI</span><span class="sxs-lookup"><span data-stu-id="05320-152">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
