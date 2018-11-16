---
title: Installer Azure CLI sur Linux avec apt
description: Comment installer Azure CLI avec le gestionnaire de package apt
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 11/12/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 0d4311e88fec9903c1aab1410cc71328f896dc65
ms.sourcegitcommit: 728a050f13d3682122be4a8993596cc4185a45ce
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/15/2018
ms.locfileid: "51680932"
---
# <a name="install-azure-cli-with-apt"></a><span data-ttu-id="1ca57-103">Installer Azure CLI avec apt</span><span class="sxs-lookup"><span data-stu-id="1ca57-103">Install Azure CLI with apt</span></span>

<span data-ttu-id="1ca57-104">Si vous exécutez une distribution qui est fournie avec `apt`, telle que Ubuntu ou Debian, un package 64 bits est disponible pour Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="1ca57-104">If you are running a distribution that comes with `apt`, such as Ubuntu or Debian, there's a 64-bit package available for the Azure CLI.</span></span> <span data-ttu-id="1ca57-105">Ce package a été testé avec :</span><span class="sxs-lookup"><span data-stu-id="1ca57-105">This package has been tested with:</span></span>

* <span data-ttu-id="1ca57-106">Ubuntu trusty, xenial, artful et bionic</span><span class="sxs-lookup"><span data-stu-id="1ca57-106">Ubuntu trusty, xenial, artful, and bionic</span></span>
* <span data-ttu-id="1ca57-107">Debian wheezy, jessie, et stretch</span><span class="sxs-lookup"><span data-stu-id="1ca57-107">Debian wheezy, jessie, and stretch</span></span>

## <a name="install"></a><span data-ttu-id="1ca57-108">Installer</span><span class="sxs-lookup"><span data-stu-id="1ca57-108">Install</span></span>

1. <div id="install-step-1"/><span data-ttu-id="1ca57-109">Modifiez votre liste de sources :</span><span class="sxs-lookup"><span data-stu-id="1ca57-109">Modify your sources list:</span></span>

    ```bash
    sudo apt-get install apt-transport-https lsb-release software-properties-common -y
    AZ_REPO=$(lsb_release -cs)
    echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
    ```

2. <div id="signingKey"/><span data-ttu-id="1ca57-110">Obtenir la clé de signature Microsoft :</span><span class="sxs-lookup"><span data-stu-id="1ca57-110">Get the Microsoft signing key:</span></span>

   ```bash
   sudo apt-key --keyring /etc/apt/trusted.gpg.d/Microsoft.gpg adv \
        --keyserver packages.microsoft.com \
        --recv-keys BC528686B50D79E339D3721CEB3E94ADBE1229CF
   ```

3. <span data-ttu-id="1ca57-111">Installer l’interface de ligne de commande :</span><span class="sxs-lookup"><span data-stu-id="1ca57-111">Install the CLI:</span></span>

   ```bash
   sudo apt-get update
   sudo apt-get install azure-cli
   ```

   > [!WARNING]
   > <span data-ttu-id="1ca57-112">La clé de signature a été mise à jour en mai 2018 et a été remplacée.</span><span class="sxs-lookup"><span data-stu-id="1ca57-112">The signing key was updated in May 2018, and has been replaced.</span></span> <span data-ttu-id="1ca57-113">Si vous recevez des erreurs de signature, veillez à disposer de la [dernière clé de signature](#signingKey).</span><span class="sxs-lookup"><span data-stu-id="1ca57-113">If you receive signing errors, make sure you have [the latest signing key](#signingKey).</span></span>

<span data-ttu-id="1ca57-114">Vous pouvez ensuite exécuter l’interface de ligne de commande Azure avec la commande `az`.</span><span class="sxs-lookup"><span data-stu-id="1ca57-114">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="1ca57-115">Pour vous connecter, utilisez la commande [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="1ca57-115">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="1ca57-116">Pour en savoir plus sur les différentes méthodes d’authentification, consultez [Se connecter avec Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="1ca57-116">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="1ca57-117">Résolution de problèmes</span><span class="sxs-lookup"><span data-stu-id="1ca57-117">Troubleshooting</span></span>

<span data-ttu-id="1ca57-118">Voici certains problèmes courants lors de l’installation avec `apt`.</span><span class="sxs-lookup"><span data-stu-id="1ca57-118">Here are some common problems seen when installing with `apt`.</span></span> <span data-ttu-id="1ca57-119">Si vous rencontrez un problème n’étant pas évoqué ici, [signalez un problème sur github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="1ca57-119">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="lsbrelease-does-not-return-the-base-distribution-version"></a><span data-ttu-id="1ca57-120">lsb_release ne renvoie pas la version de la distribution de base</span><span class="sxs-lookup"><span data-stu-id="1ca57-120">lsb_release does not return the base distribution version</span></span>

<span data-ttu-id="1ca57-121">Certaines distributions Ubuntu ou Debian dérivées, telles que Linux Mint peuvent ne pas retourner le nom de version correct de `lsb_release`.</span><span class="sxs-lookup"><span data-stu-id="1ca57-121">Some Ubuntu- or Debian-derived distributions such as Linux Mint may not return the correct version name from `lsb_release`.</span></span> <span data-ttu-id="1ca57-122">Cette valeur est utilisée dans le processus d’installation pour déterminer le package à installer.</span><span class="sxs-lookup"><span data-stu-id="1ca57-122">This value is used in the install process to determine the package to install.</span></span> <span data-ttu-id="1ca57-123">Si vous connaissez le nom de la version dont votre distribution est dérivée, vous pouvez définir la valeur `AZ_REPO` manuellement dans [installation de l’étape 1](#install-step-1).</span><span class="sxs-lookup"><span data-stu-id="1ca57-123">If you know the name of the version your distribution is derived from, you can set the `AZ_REPO` value manually in [install step 1](#install-step-1).</span></span> <span data-ttu-id="1ca57-124">Dans le cas contraire, recherchez des informations concernant votre distribution, sur la façon de déterminer le nom de la distribution de base et de définir `AZ_REPO` sur la valeur correcte.</span><span class="sxs-lookup"><span data-stu-id="1ca57-124">Otherwise, look up information for your distribution on how to determine the base distribution name and set `AZ_REPO` to the correct value.</span></span>

### <a name="apt-key-fails-with-no-dirmngr"></a><span data-ttu-id="1ca57-125">Clé apt échoue avec le message « No dirmngr »</span><span class="sxs-lookup"><span data-stu-id="1ca57-125">apt-key fails with "No dirmngr"</span></span>

<span data-ttu-id="1ca57-126">Lorsque vous exécutez la commande `apt-key`, vous pouvez voir une sortie similaire à l’erreur suivante :</span><span class="sxs-lookup"><span data-stu-id="1ca57-126">When running the `apt-key` command, you may see output similar to the following error:</span></span>

```output
gpg: failed to start the dirmngr '/usr/bin/dirmngr': No such file or directory
gpg: connecting dirmngr at '/tmp/apt-key-gpghome.kt5zo27tp1/S.dirmngr' failed: No such file or directory
gpg: keyserver receive failed: No dirmngr
```

<span data-ttu-id="1ca57-127">Cette erreur est due à un composant manquant requis par `apt-key`.</span><span class="sxs-lookup"><span data-stu-id="1ca57-127">The error is due to a missing component required by `apt-key`.</span></span> <span data-ttu-id="1ca57-128">Vous pouvez résoudre ce problème en installant le package `dirmngr`.</span><span class="sxs-lookup"><span data-stu-id="1ca57-128">You can resolve it by installing the `dirmngr` package.</span></span>

```bash
sudo apt-get install dirmngr
```

### <a name="apt-key-hangs"></a><span data-ttu-id="1ca57-129">apt-key se bloque</span><span class="sxs-lookup"><span data-stu-id="1ca57-129">apt-key hangs</span></span>

<span data-ttu-id="1ca57-130">Lorsqu’un pare-feu bloque les connexions sortantes au port 11371, la commande `apt-key` peut se bloquer indéfiniment.</span><span class="sxs-lookup"><span data-stu-id="1ca57-130">When behind a firewall blocking outgoing connections to port 11371, the `apt-key` command might hang indefinitely.</span></span>
<span data-ttu-id="1ca57-131">Votre pare-feu peut nécessiter l’utilisation d’un proxy HTTP pour les connexions sortantes :</span><span class="sxs-lookup"><span data-stu-id="1ca57-131">Your firewall may require an HTTP proxy for outgoing connections:</span></span>

```bash
sudo apt-key --keyring /etc/apt/trusted.gpg.d/Microsoft.gpg adv \
    --keyserver-options http-proxy=http://<USER>:<PASSWORD>@<PROXY-HOST>:<PROXY-PORT>/ \
    --keyserver packages.microsoft.com \
    --recv-keys BC528686B50D79E339D3721CEB3E94ADBE1229CF
```

<span data-ttu-id="1ca57-132">Pour vous assurer que vous disposez d’un proxy, contactez votre administrateur système.</span><span class="sxs-lookup"><span data-stu-id="1ca57-132">To determine if you have a proxy, contact your system administrator.</span></span> <span data-ttu-id="1ca57-133">Si votre proxy ne nécessite pas de connexion, ignorez les informations d’utilisateur et de mot de passe.</span><span class="sxs-lookup"><span data-stu-id="1ca57-133">If your proxy does not require a login, then leave out the user and password information.</span></span>

## <a name="update"></a><span data-ttu-id="1ca57-134">Mettre à jour</span><span class="sxs-lookup"><span data-stu-id="1ca57-134">Update</span></span>

<span data-ttu-id="1ca57-135">Utilisez `apt-get upgrade` pour mettre à jour le package de l’interface de ligne de commande.</span><span class="sxs-lookup"><span data-stu-id="1ca57-135">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!WARNING]
> <span data-ttu-id="1ca57-136">La clé de signature a été mise à jour en mai 2018 et a été remplacée.</span><span class="sxs-lookup"><span data-stu-id="1ca57-136">The signing key was updated in May 2018, and has been replaced.</span></span> <span data-ttu-id="1ca57-137">Si vous recevez des erreurs de signature, veillez à disposer de la [dernière clé de signature](#signingKey).</span><span class="sxs-lookup"><span data-stu-id="1ca57-137">If you receive signing errors, make sure you have [the latest signing key](#signingKey).</span></span>
>
> [!NOTE]
> <span data-ttu-id="1ca57-138">Cette commande met à niveau tous les packages installés sur votre système n’ayant pas de modification de dépendance.</span><span class="sxs-lookup"><span data-stu-id="1ca57-138">This command upgrades all of the installed packages on your system that have not had a dependency change.</span></span>
> <span data-ttu-id="1ca57-139">Pour mettre à niveau uniquement l’interface CLI, utilisez `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="1ca57-139">To upgrade the CLI only, use `apt-get install`.</span></span>
> 
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

## <a name="uninstall"></a><span data-ttu-id="1ca57-140">Désinstaller l’interface</span><span class="sxs-lookup"><span data-stu-id="1ca57-140">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="1ca57-141">Désinstaller avec `apt-get remove` :</span><span class="sxs-lookup"><span data-stu-id="1ca57-141">Uninstall with `apt-get remove`:</span></span>

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. <span data-ttu-id="1ca57-142">Si vous ne prévoyez pas de réinstaller l’interface CLI, supprimez les informations de référentiel Azure CLI :</span><span class="sxs-lookup"><span data-stu-id="1ca57-142">If you don't plan to reinstall the CLI, remove the Azure CLI repository information:</span></span>

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. <span data-ttu-id="1ca57-143">Supprimer la clé de signature :</span><span class="sxs-lookup"><span data-stu-id="1ca57-143">Remove the signing key:</span></span>

    ```bash
    sudo rm /etc/apt/trusted.gpg.d/Microsoft.gpg
    ```

4. <span data-ttu-id="1ca57-144">Supprimer tous les packages inutiles :</span><span class="sxs-lookup"><span data-stu-id="1ca57-144">Remove any unneeded packages:</span></span>

   ```bash
   sudo apt autoremove
   ```

## <a name="next-steps"></a><span data-ttu-id="1ca57-145">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="1ca57-145">Next Steps</span></span>

<span data-ttu-id="1ca57-146">Maintenant que vous avez installé l’interface CLI, découvrez ses fonctionnalités et ses commandes courantes.</span><span class="sxs-lookup"><span data-stu-id="1ca57-146">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="1ca57-147">Prise en main de l’interface Azure CLI</span><span class="sxs-lookup"><span data-stu-id="1ca57-147">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)