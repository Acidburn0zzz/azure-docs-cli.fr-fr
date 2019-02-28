---
title: Installer Azure CLI sur Linux avec apt
description: Comment installer Azure CLI avec le gestionnaire de package apt
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 11/27/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 45e1e7468e5817d0138c9b87da83c5a5228e4965
ms.sourcegitcommit: 1987a39809f9865034b27130e56f30b2bd1eb72c
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/19/2019
ms.locfileid: "56421930"
---
# <a name="install-azure-cli-with-apt"></a><span data-ttu-id="e0103-103">Installer Azure CLI avec apt</span><span class="sxs-lookup"><span data-stu-id="e0103-103">Install Azure CLI with apt</span></span>

<span data-ttu-id="e0103-104">Si vous exécutez une distribution qui est fournie avec `apt`, telle que Ubuntu ou Debian, un package 64 bits est disponible pour Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="e0103-104">If you are running a distribution that comes with `apt`, such as Ubuntu or Debian, there's a 64-bit package available for the Azure CLI.</span></span> <span data-ttu-id="e0103-105">Ce package a été testé avec :</span><span class="sxs-lookup"><span data-stu-id="e0103-105">This package has been tested with:</span></span>

* <span data-ttu-id="e0103-106">Ubuntu trusty, xenial, artful et bionic</span><span class="sxs-lookup"><span data-stu-id="e0103-106">Ubuntu trusty, xenial, artful, and bionic</span></span>
* <span data-ttu-id="e0103-107">Debian wheezy, jessie, et stretch</span><span class="sxs-lookup"><span data-stu-id="e0103-107">Debian wheezy, jessie, and stretch</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

> [!NOTE]
>
> <span data-ttu-id="e0103-108">Dans la mesure où le package `.deb` d’Azure CLI installe son propre interpréteur Python et n’utilise pas le système Python, aucune version explicite n’est nécessaire pour une version Python locale.</span><span class="sxs-lookup"><span data-stu-id="e0103-108">The `.deb` package for Azure CLI installs its own Python interpreter, and does not use the system Python, so there is no explicit requirement for a local Python version.</span></span>

## <a name="install"></a><span data-ttu-id="e0103-109">Installer</span><span class="sxs-lookup"><span data-stu-id="e0103-109">Install</span></span>

1. <span data-ttu-id="e0103-110">Installez les packages prérequis :</span><span class="sxs-lookup"><span data-stu-id="e0103-110">Install prerequisite packages:</span></span>

    ```bash
    sudo apt-get install apt-transport-https lsb-release software-properties-common dirmngr -y
    ```

2. <div id="set-release"/><span data-ttu-id="e0103-111">Modifiez votre liste de sources :</span><span class="sxs-lookup"><span data-stu-id="e0103-111">Modify your sources list:</span></span>

    ```bash
    AZ_REPO=$(lsb_release -cs)
    echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
    ```

3. <div id="signingKey"/><span data-ttu-id="e0103-112">Obtenir la clé de signature Microsoft :</span><span class="sxs-lookup"><span data-stu-id="e0103-112">Get the Microsoft signing key:</span></span>

   ```bash
   sudo apt-key --keyring /etc/apt/trusted.gpg.d/Microsoft.gpg adv \
        --keyserver packages.microsoft.com \
        --recv-keys BC528686B50D79E339D3721CEB3E94ADBE1229CF
   ```

4. <span data-ttu-id="e0103-113">Installer l’interface de ligne de commande :</span><span class="sxs-lookup"><span data-stu-id="e0103-113">Install the CLI:</span></span>

   ```bash
   sudo apt-get update
   sudo apt-get install azure-cli
   ```

   > [!WARNING]
   > <span data-ttu-id="e0103-114">La clé de signature a été mise à jour en mai 2018 et a été remplacée.</span><span class="sxs-lookup"><span data-stu-id="e0103-114">The signing key was updated in May 2018, and has been replaced.</span></span> <span data-ttu-id="e0103-115">Si vous recevez des erreurs de signature, veillez à disposer de la [dernière clé de signature](#signingKey).</span><span class="sxs-lookup"><span data-stu-id="e0103-115">If you receive signing errors, make sure you have [the latest signing key](#signingKey).</span></span>

<span data-ttu-id="e0103-116">Vous pouvez ensuite exécuter l’interface de ligne de commande Azure avec la commande `az`.</span><span class="sxs-lookup"><span data-stu-id="e0103-116">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="e0103-117">Pour vous connecter, utilisez la commande [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="e0103-117">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="e0103-118">Pour en savoir plus sur les différentes méthodes d’authentification, consultez [Se connecter avec Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="e0103-118">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="e0103-119">Résolution de problèmes</span><span class="sxs-lookup"><span data-stu-id="e0103-119">Troubleshooting</span></span>

<span data-ttu-id="e0103-120">Voici certains problèmes courants lors de l’installation avec `apt`.</span><span class="sxs-lookup"><span data-stu-id="e0103-120">Here are some common problems seen when installing with `apt`.</span></span> <span data-ttu-id="e0103-121">Si vous rencontrez un problème n’étant pas évoqué ici, [signalez un problème sur github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="e0103-121">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="lsbrelease-does-not-return-the-correct-base-distribution-version"></a><span data-ttu-id="e0103-122">lsb_release ne renvoie pas la bonne version de la distribution de base</span><span class="sxs-lookup"><span data-stu-id="e0103-122">lsb_release does not return the correct base distribution version</span></span>

<span data-ttu-id="e0103-123">Certaines distributions Ubuntu ou Debian dérivées, telles que Linux Mint peuvent ne pas retourner le nom de version correct de `lsb_release`.</span><span class="sxs-lookup"><span data-stu-id="e0103-123">Some Ubuntu- or Debian-derived distributions such as Linux Mint may not return the correct version name from `lsb_release`.</span></span> <span data-ttu-id="e0103-124">Cette valeur est utilisée dans le processus d’installation pour déterminer le package à installer.</span><span class="sxs-lookup"><span data-stu-id="e0103-124">This value is used in the install process to determine the package to install.</span></span> <span data-ttu-id="e0103-125">Si vous connaissez le nom de la version dont votre distribution est dérivée, vous pouvez définir la valeur `AZ_REPO` manuellement à [l’étape 2 de l’installation](#set-release).</span><span class="sxs-lookup"><span data-stu-id="e0103-125">If you know the name of the version your distribution is derived from, you can set the `AZ_REPO` value manually in [install step 2](#set-release).</span></span> <span data-ttu-id="e0103-126">Dans le cas contraire, recherchez des informations concernant votre distribution, sur la façon de déterminer le nom de la distribution de base et de définir `AZ_REPO` sur la valeur correcte.</span><span class="sxs-lookup"><span data-stu-id="e0103-126">Otherwise, look up information for your distribution on how to determine the base distribution name and set `AZ_REPO` to the correct value.</span></span>

### <a name="no-package-for-your-distribution"></a><span data-ttu-id="e0103-127">Aucun package pour votre distribution</span><span class="sxs-lookup"><span data-stu-id="e0103-127">No package for your distribution</span></span>

<span data-ttu-id="e0103-128">La disponibilité d’un package Azure CLI pour une distribution Ubuntu après sa publication peut parfois prendre un certain temps.</span><span class="sxs-lookup"><span data-stu-id="e0103-128">Sometimes it may be a while after an Ubuntu distribution is released before there's an Azure CLI package made available for it.</span></span> <span data-ttu-id="e0103-129">Azure CLI est conçu pour résister à de futures versions de dépendances, et repose sur peu d’entre elles.</span><span class="sxs-lookup"><span data-stu-id="e0103-129">The Azure CLI designed to be resilient with regards to future versions of dependencies and rely on as few of them as possible.</span></span> <span data-ttu-id="e0103-130">Si aucun package n’est disponible pour votre distribution de base, essayez d’utiliser le package d’une distribution antérieure.</span><span class="sxs-lookup"><span data-stu-id="e0103-130">If there's no package available for your base distribution, try a package for an earlier distribution.</span></span>

<span data-ttu-id="e0103-131">Pour ce faire, définissez manuellement la valeur de `AZ_REPO` dans [ étape 1 Installer](#install-step-1).</span><span class="sxs-lookup"><span data-stu-id="e0103-131">To do this, set the value of `AZ_REPO` manually in [install step 1](#install-step-1).</span></span> <span data-ttu-id="e0103-132">Pour les distributions Ubuntu, utilisez le référentiel `bionic`, et `stretch` pour les distributions Debian.</span><span class="sxs-lookup"><span data-stu-id="e0103-132">For Ubuntu distributions use the `bionic` repository, and for Debian distributions use `stretch`.</span></span> <span data-ttu-id="e0103-133">Les distributions publiées avant Ubuntu Trusty et Debian Wheezy ne sont pas prises en charge.</span><span class="sxs-lookup"><span data-stu-id="e0103-133">Distributions released before Ubuntu Trusty and Debian Wheezy are not supported.</span></span>

### <a name="apt-key-fails-with-no-dirmngr"></a><span data-ttu-id="e0103-134">Clé apt échoue avec le message « No dirmngr »</span><span class="sxs-lookup"><span data-stu-id="e0103-134">apt-key fails with "No dirmngr"</span></span>

<span data-ttu-id="e0103-135">Lorsque vous exécutez la commande `apt-key`, vous pouvez voir une sortie similaire à l’erreur suivante :</span><span class="sxs-lookup"><span data-stu-id="e0103-135">When running the `apt-key` command, you may see output similar to the following error:</span></span>

```output
gpg: failed to start the dirmngr '/usr/bin/dirmngr': No such file or directory
gpg: connecting dirmngr at '/tmp/apt-key-gpghome.kt5zo27tp1/S.dirmngr' failed: No such file or directory
gpg: keyserver receive failed: No dirmngr
```

<span data-ttu-id="e0103-136">Cette erreur est due à un composant manquant requis par `apt-key`.</span><span class="sxs-lookup"><span data-stu-id="e0103-136">The error is due to a missing component required by `apt-key`.</span></span> <span data-ttu-id="e0103-137">Vous pouvez résoudre ce problème en installant le package `dirmngr`.</span><span class="sxs-lookup"><span data-stu-id="e0103-137">You can resolve it by installing the `dirmngr` package.</span></span>

```bash
sudo apt-get install dirmngr
```

<span data-ttu-id="e0103-138">Si vous êtes sur le sous-système Windows pour Linux (WSL), cette erreur apparaît également sur les versions de Windows antérieures à Windows 10 1809.</span><span class="sxs-lookup"><span data-stu-id="e0103-138">If you are on Windows Subsystem for Linux (WSL), this error also appears on versions of Windows prior to Windows 10 1809.</span></span> <span data-ttu-id="e0103-139">Pour résoudre ce problème, mettez à jour votre version de Windows.</span><span class="sxs-lookup"><span data-stu-id="e0103-139">To resolve the issue, update your version of Windows.</span></span>

### <a name="apt-key-hangs"></a><span data-ttu-id="e0103-140">apt-key se bloque</span><span class="sxs-lookup"><span data-stu-id="e0103-140">apt-key hangs</span></span>

<span data-ttu-id="e0103-141">Lorsqu’un pare-feu bloque les connexions sortantes au port 11371, la commande `apt-key` peut se bloquer indéfiniment.</span><span class="sxs-lookup"><span data-stu-id="e0103-141">When behind a firewall blocking outgoing connections to port 11371, the `apt-key` command might hang indefinitely.</span></span>
<span data-ttu-id="e0103-142">Votre pare-feu peut nécessiter l’utilisation d’un proxy HTTP pour les connexions sortantes :</span><span class="sxs-lookup"><span data-stu-id="e0103-142">Your firewall may require an HTTP proxy for outgoing connections:</span></span>

```bash
sudo apt-key --keyring /etc/apt/trusted.gpg.d/Microsoft.gpg adv \
    --keyserver-options http-proxy=http://<USER>:<PASSWORD>@<PROXY-HOST>:<PROXY-PORT>/ \
    --keyserver packages.microsoft.com \
    --recv-keys BC528686B50D79E339D3721CEB3E94ADBE1229CF
```

<span data-ttu-id="e0103-143">Pour vous assurer que vous disposez d’un proxy, contactez votre administrateur système.</span><span class="sxs-lookup"><span data-stu-id="e0103-143">To determine if you have a proxy, contact your system administrator.</span></span> <span data-ttu-id="e0103-144">Si votre proxy ne nécessite pas de connexion, ignorez les informations d’utilisateur et de mot de passe.</span><span class="sxs-lookup"><span data-stu-id="e0103-144">If your proxy does not require a login, then leave out the user and password information.</span></span>

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="update"></a><span data-ttu-id="e0103-145">Mettre à jour</span><span class="sxs-lookup"><span data-stu-id="e0103-145">Update</span></span>

<span data-ttu-id="e0103-146">Utilisez `apt-get upgrade` pour mettre à jour le package de l’interface de ligne de commande.</span><span class="sxs-lookup"><span data-stu-id="e0103-146">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!WARNING]
> <span data-ttu-id="e0103-147">La clé de signature a été mise à jour en mai 2018 et a été remplacée.</span><span class="sxs-lookup"><span data-stu-id="e0103-147">The signing key was updated in May 2018, and has been replaced.</span></span> <span data-ttu-id="e0103-148">Si vous recevez des erreurs de signature, veillez à disposer de la [dernière clé de signature](#signingKey).</span><span class="sxs-lookup"><span data-stu-id="e0103-148">If you receive signing errors, make sure you have [the latest signing key](#signingKey).</span></span>
>
> [!NOTE]
> <span data-ttu-id="e0103-149">Cette commande met à niveau tous les packages installés sur votre système n’ayant pas de modification de dépendance.</span><span class="sxs-lookup"><span data-stu-id="e0103-149">This command upgrades all of the installed packages on your system that have not had a dependency change.</span></span>
> <span data-ttu-id="e0103-150">Pour mettre à niveau uniquement l’interface CLI, utilisez `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="e0103-150">To upgrade the CLI only, use `apt-get install`.</span></span>
> 
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

## <a name="uninstall"></a><span data-ttu-id="e0103-151">Désinstaller l’interface</span><span class="sxs-lookup"><span data-stu-id="e0103-151">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="e0103-152">Désinstaller avec `apt-get remove` :</span><span class="sxs-lookup"><span data-stu-id="e0103-152">Uninstall with `apt-get remove`:</span></span>

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. <span data-ttu-id="e0103-153">Si vous ne prévoyez pas de réinstaller l’interface CLI, supprimez les informations de référentiel Azure CLI :</span><span class="sxs-lookup"><span data-stu-id="e0103-153">If you don't plan to reinstall the CLI, remove the Azure CLI repository information:</span></span>

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. <span data-ttu-id="e0103-154">Supprimer la clé de signature :</span><span class="sxs-lookup"><span data-stu-id="e0103-154">Remove the signing key:</span></span>

    ```bash
    sudo rm /etc/apt/trusted.gpg.d/Microsoft.gpg
    ```

4. <span data-ttu-id="e0103-155">Supprimer tous les packages inutiles :</span><span class="sxs-lookup"><span data-stu-id="e0103-155">Remove any unneeded packages:</span></span>

   ```bash
   sudo apt autoremove
   ```

## <a name="next-steps"></a><span data-ttu-id="e0103-156">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="e0103-156">Next Steps</span></span>

<span data-ttu-id="e0103-157">Maintenant que vous avez installé l’interface CLI, découvrez ses fonctionnalités et ses commandes courantes.</span><span class="sxs-lookup"><span data-stu-id="e0103-157">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="e0103-158">Prise en main de l’interface Azure CLI</span><span class="sxs-lookup"><span data-stu-id="e0103-158">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
