---
title: Installation d’Azure CLI 2.0 pour Linux avec apt
description: Installation d’Azure CLI 2.0 avec le gestionnaire de package apt
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/07/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 13cc995e099cee47534a46097b2e1afd8e96e8b4
ms.sourcegitcommit: d93b0a2bcfb0d164ef90d6d4618f0552609a8ea6
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/20/2018
ms.locfileid: "46469978"
---
# <a name="install-azure-cli-20-with-apt"></a><span data-ttu-id="4b220-103">Installer Azure CLI 2.0 avec apt</span><span class="sxs-lookup"><span data-stu-id="4b220-103">Install Azure CLI 2.0 with apt</span></span>

<span data-ttu-id="4b220-104">Si vous exécutez une distribution qui est fournie avec `apt`, telle que Ubuntu ou Debian, un package 64 bits est disponible pour Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="4b220-104">If you are running a distribution that comes with `apt`, such as Ubuntu or Debian, there's a 64-bit package available for the Azure CLI.</span></span> <span data-ttu-id="4b220-105">Ce package a été testé avec :</span><span class="sxs-lookup"><span data-stu-id="4b220-105">This package has been tested with:</span></span>

* <span data-ttu-id="4b220-106">Ubuntu trusty, xenial, artful et bionic</span><span class="sxs-lookup"><span data-stu-id="4b220-106">Ubuntu trusty, xenial, artful, and bionic</span></span>
* <span data-ttu-id="4b220-107">Debian wheezy, jessie, et stretch</span><span class="sxs-lookup"><span data-stu-id="4b220-107">Debian wheezy, jessie, and stretch</span></span>

## <a name="install"></a><span data-ttu-id="4b220-108">Installer</span><span class="sxs-lookup"><span data-stu-id="4b220-108">Install</span></span>

1. <div id="install-step-1"/><span data-ttu-id="4b220-109">Modifiez votre liste de sources :</span><span class="sxs-lookup"><span data-stu-id="4b220-109">Modify your sources list:</span></span>

    ```bash
    AZ_REPO=$(lsb_release -cs)
    echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
    ```

2. <div id="signingKey"/><span data-ttu-id="4b220-110">Obtenir la clé de signature Microsoft :</span><span class="sxs-lookup"><span data-stu-id="4b220-110">Get the Microsoft signing key:</span></span>

   ```bash
   curl -L https://packages.microsoft.com/keys/microsoft.asc | sudo apt-key add -
   ```

3. <span data-ttu-id="4b220-111">Installer l’interface de ligne de commande :</span><span class="sxs-lookup"><span data-stu-id="4b220-111">Install the CLI:</span></span>

   ```bash
   sudo apt-get update
   sudo apt-get install apt-transport-https azure-cli
   ```

   > [!WARNING]
   > <span data-ttu-id="4b220-112">La clé de signature a été mise à jour en mai 2018 et a été remplacée.</span><span class="sxs-lookup"><span data-stu-id="4b220-112">The signing key was updated in May 2018, and has been replaced.</span></span> <span data-ttu-id="4b220-113">Si vous recevez des erreurs de clé de signature, assurez-vous d’avoir [acquis la clé de signature la plus récente](#signingKey).</span><span class="sxs-lookup"><span data-stu-id="4b220-113">If you receive signing key errors, please ensure that you have [acquired the latest signing key](#signingKey).</span></span>

<span data-ttu-id="4b220-114">Vous pouvez ensuite exécuter l’interface de ligne de commande Azure avec la commande `az`.</span><span class="sxs-lookup"><span data-stu-id="4b220-114">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="4b220-115">Pour vous connecter, utilisez la commande [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="4b220-115">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="4b220-116">Pour en savoir plus sur les différentes méthodes d’authentification, consultez [Se connecter avec Azure CLI 2.0](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="4b220-116">To learn more about different authentication methods, see [Sign in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="4b220-117">Résolution de problèmes</span><span class="sxs-lookup"><span data-stu-id="4b220-117">Troubleshooting</span></span>

<span data-ttu-id="4b220-118">Voici certains problèmes courants lors de l’installation avec `apt`.</span><span class="sxs-lookup"><span data-stu-id="4b220-118">Here are some common problems seen when installing with `apt`.</span></span> <span data-ttu-id="4b220-119">Si vous rencontrez un problème n’étant pas évoqué ici, [signalez un problème sur github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="4b220-119">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="lsbrelease-fails-with-command-not-found"></a><span data-ttu-id="4b220-120">lsb_release échoue avec « Commande introuvable »</span><span class="sxs-lookup"><span data-stu-id="4b220-120">lsb_release fails with "Command not found"</span></span>

<span data-ttu-id="4b220-121">Lorsque vous exécutez la commande `lsb_release`, vous pouvez voir une sortie similaire à l’erreur suivante :</span><span class="sxs-lookup"><span data-stu-id="4b220-121">When running the `lsb_release` command, you may see output similar to the following error:</span></span>

```output
-bash: lsb_release: command not found
```

<span data-ttu-id="4b220-122">L’erreur est due au fait que la commande `lsb_release` n’est pas installée.</span><span class="sxs-lookup"><span data-stu-id="4b220-122">The error is due to the `lsb_release` command not being installed.</span></span> <span data-ttu-id="4b220-123">Vous pouvez résoudre ce problème en installant le package `lsb-release`.</span><span class="sxs-lookup"><span data-stu-id="4b220-123">You can resolve it by installing the `lsb-release` package.</span></span>

```bash
sudo apt-get install lsb-release
```

### <a name="lsbrelease-does-not-return-the-base-distribution-version"></a><span data-ttu-id="4b220-124">lsb_release ne renvoie pas la version de la distribution de base</span><span class="sxs-lookup"><span data-stu-id="4b220-124">lsb_release does not return the base distribution version</span></span>

<span data-ttu-id="4b220-125">Certaines distributions Ubuntu ou Debian dérivées, telles que Linux Mint peuvent ne pas retourner le nom de version correct de `lsb_release`.</span><span class="sxs-lookup"><span data-stu-id="4b220-125">Some Ubuntu- or Debian-derived distributions such as Linux Mint may not return the correct version name from `lsb_release`.</span></span> <span data-ttu-id="4b220-126">Cette valeur est utilisée dans le processus d’installation pour déterminer le package à installer.</span><span class="sxs-lookup"><span data-stu-id="4b220-126">This value is used in the install process to determine the package to install.</span></span> <span data-ttu-id="4b220-127">Si vous connaissez le nom de la version dont votre distribution est dérivée, vous pouvez définir la valeur `AZ_REPO` manuellement dans [installation de l’étape 1](#install-step-1).</span><span class="sxs-lookup"><span data-stu-id="4b220-127">If you know the name of the version your distribution is derived from, you can set the `AZ_REPO` value manually in [install step 1](#install-step-1).</span></span> <span data-ttu-id="4b220-128">Dans le cas contraire, recherchez des informations concernant votre distribution, sur la façon de déterminer le nom de la distribution de base et de définir `AZ_REPO` sur la valeur correcte.</span><span class="sxs-lookup"><span data-stu-id="4b220-128">Otherwise, look up information for your distribution on how to determine the base distribution name and set `AZ_REPO` to the correct value.</span></span>

### <a name="apt-key-fails-with-no-dirmngr"></a><span data-ttu-id="4b220-129">Clé apt échoue avec le message « No dirmngr »</span><span class="sxs-lookup"><span data-stu-id="4b220-129">apt-key fails with "No dirmngr"</span></span>

<span data-ttu-id="4b220-130">Lorsque vous exécutez la commande `apt-key`, vous pouvez voir une sortie similaire à l’erreur suivante :</span><span class="sxs-lookup"><span data-stu-id="4b220-130">When running the `apt-key` command, you may see output similar to the following error:</span></span>

```output
gpg: failed to start the dirmngr '/usr/bin/dirmngr': No such file or directory
gpg: connecting dirmngr at '/tmp/apt-key-gpghome.kt5zo27tp1/S.dirmngr' failed: No such file or directory
gpg: keyserver receive failed: No dirmngr
```

<span data-ttu-id="4b220-131">Cette erreur est due à un composant manquant requis par `apt-key`.</span><span class="sxs-lookup"><span data-stu-id="4b220-131">The error is due to a missing component required by `apt-key`.</span></span> <span data-ttu-id="4b220-132">Vous pouvez résoudre ce problème en installant le package `dirmngr`.</span><span class="sxs-lookup"><span data-stu-id="4b220-132">You can resolve it by installing the `dirmngr` package.</span></span>

```bash
sudo apt-get install dirmngr
```

### <a name="apt-key-hangs"></a><span data-ttu-id="4b220-133">apt-key se bloque</span><span class="sxs-lookup"><span data-stu-id="4b220-133">apt-key hangs</span></span>

<span data-ttu-id="4b220-134">Lorsqu’un pare-feu bloque les connexions sortantes au port 11371, la commande `apt-key` peut se bloquer indéfiniment.</span><span class="sxs-lookup"><span data-stu-id="4b220-134">When behind a firewall blocking outgoing connections to port 11371, the `apt-key` command might hang indefinitely.</span></span> <span data-ttu-id="4b220-135">Votre pare-feu peut nécessiter l’utilisation d’un proxy HTTP pour les connexions sortantes :</span><span class="sxs-lookup"><span data-stu-id="4b220-135">Your firewall may require the use of an HTTP proxy for outgoing connections:</span></span>

```bash
sudo apt-key adv --keyserver-options http-proxy=http://<USER>:<PASSWORD>@<PROXY-HOST>:<PROXY-PORT>/ --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
```

<span data-ttu-id="4b220-136">Pour vous assurer que vous disposez d’un proxy, contactez votre administrateur système.</span><span class="sxs-lookup"><span data-stu-id="4b220-136">To determine if you have a proxy, contact your system administrator.</span></span> <span data-ttu-id="4b220-137">Si votre proxy ne nécessite pas de connexion, ignorez l’utilisateur, le mot de passe, et le jeton `@`.</span><span class="sxs-lookup"><span data-stu-id="4b220-137">If your proxy does not require a login, then leave out the user, password, and `@` token.</span></span>

## <a name="update"></a><span data-ttu-id="4b220-138">Mettre à jour</span><span class="sxs-lookup"><span data-stu-id="4b220-138">Update</span></span>

<span data-ttu-id="4b220-139">Utilisez `apt-get upgrade` pour mettre à jour le package de l’interface de ligne de commande.</span><span class="sxs-lookup"><span data-stu-id="4b220-139">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!WARNING]
> <span data-ttu-id="4b220-140">La clé de signature a été mise à jour en mai 2018 et a été remplacée.</span><span class="sxs-lookup"><span data-stu-id="4b220-140">The signing key was updated in May 2018, and has been replaced.</span></span> <span data-ttu-id="4b220-141">Si vous recevez des erreurs de clé de signature, assurez-vous d’avoir [acquis la clé de signature la plus récente](#signingKey).</span><span class="sxs-lookup"><span data-stu-id="4b220-141">If you receive signing key errors, please ensure that you have [acquired the latest signing key](#signingKey).</span></span>
>
> [!NOTE]
> <span data-ttu-id="4b220-142">Cette commande met à niveau tous les packages installés sur votre système n’ayant pas de modification de dépendance.</span><span class="sxs-lookup"><span data-stu-id="4b220-142">This command upgrades all of the installed packages on your system that have not had a dependency change.</span></span>
> <span data-ttu-id="4b220-143">Pour mettre à niveau uniquement l’interface CLI, utilisez `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="4b220-143">To upgrade the CLI only, use `apt-get install`.</span></span>
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

## <a name="uninstall"></a><span data-ttu-id="4b220-144">Désinstaller l’interface</span><span class="sxs-lookup"><span data-stu-id="4b220-144">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="4b220-145">Désinstaller avec `apt-get remove`.</span><span class="sxs-lookup"><span data-stu-id="4b220-145">Uninstall with `apt-get remove`.</span></span>

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. <span data-ttu-id="4b220-146">Si vous ne prévoyez pas de réinstaller l’interface CLI, supprimez les informations de référentiel Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="4b220-146">If you don't plan to reinstall the CLI, remove the Azure CLI repository information.</span></span>

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. <span data-ttu-id="4b220-147">Supprimez tous les packages inutiles.</span><span class="sxs-lookup"><span data-stu-id="4b220-147">Remove any unneeded packages.</span></span>

   ```bash
   sudo apt autoremove
   ```

## <a name="next-steps"></a><span data-ttu-id="4b220-148">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="4b220-148">Next Steps</span></span>

<span data-ttu-id="4b220-149">Maintenant que vous avez installé l’interface CLI, découvrez ses fonctionnalités et ses commandes courantes.</span><span class="sxs-lookup"><span data-stu-id="4b220-149">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="4b220-150">Prise en main de l’interface Azure CLI</span><span class="sxs-lookup"><span data-stu-id="4b220-150">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)