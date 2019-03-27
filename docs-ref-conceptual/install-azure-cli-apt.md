---
title: Installer Azure CLI sur Linux avec apt
description: Comment installer Azure CLI avec le gestionnaire de package apt
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 03/19/2019
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: fa2e1db439b4836d7506409b3abcce74fb6e6695
ms.sourcegitcommit: 5864f72b9a6fbf82a4d98bf805b3a16a7da18556
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/22/2019
ms.locfileid: "58343143"
---
# <a name="install-azure-cli-with-apt"></a><span data-ttu-id="5416a-103">Installer Azure CLI avec apt</span><span class="sxs-lookup"><span data-stu-id="5416a-103">Install Azure CLI with apt</span></span>

<span data-ttu-id="5416a-104">Si vous exécutez une distribution qui est fournie avec `apt`, telle que Ubuntu ou Debian, un package x86_64 est disponible pour Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="5416a-104">If you are running a distribution that comes with `apt`, such as Ubuntu or Debian, there's an x86_64 package available for the Azure CLI.</span></span> <span data-ttu-id="5416a-105">Ce package a été testé avec :</span><span class="sxs-lookup"><span data-stu-id="5416a-105">This package has been tested with:</span></span>

* <span data-ttu-id="5416a-106">Ubuntu trusty, xenial, artful et bionic</span><span class="sxs-lookup"><span data-stu-id="5416a-106">Ubuntu trusty, xenial, artful, and bionic</span></span>
* <span data-ttu-id="5416a-107">Debian wheezy, jessie, et stretch</span><span class="sxs-lookup"><span data-stu-id="5416a-107">Debian wheezy, jessie, and stretch</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

> [!NOTE]
>
> <span data-ttu-id="5416a-108">Le package Azure CLI installe son propre interpréteur Python et n’utilise pas le système Python.</span><span class="sxs-lookup"><span data-stu-id="5416a-108">The package for Azure CLI installs its own Python interpreter, and does not use the system Python.</span></span>

## <a name="install"></a><span data-ttu-id="5416a-109">Installer</span><span class="sxs-lookup"><span data-stu-id="5416a-109">Install</span></span>

1. <span data-ttu-id="5416a-110">Récupérez les packages nécessaires au processus d’installation :</span><span class="sxs-lookup"><span data-stu-id="5416a-110">Get packages needed for the install process:</span></span>

    ```bash
    sudo apt-get update
    sudo apt-get install curl apt-transport-https lsb-release gpg
    ```

2. <span data-ttu-id="5416a-111">Téléchargez et installez la clé de signature Microsoft :</span><span class="sxs-lookup"><span data-stu-id="5416a-111">Download and install the Microsoft signing key:</span></span>

    ```bash
    curl -sL https://packages.microsoft.com/keys/microsoft.asc | \
        gpg --dearmor | \
        sudo tee /etc/apt/trusted.gpg.d/microsoft.asc.gpg > /dev/null
    ```

3. <div id="set-release"/><span data-ttu-id="5416a-112">Ajoutez le référentiel de logiciels Azure CLI :</span><span class="sxs-lookup"><span data-stu-id="5416a-112">Add the Azure CLI software repository:</span></span>

    ```bash
    AZ_REPO=$(lsb_release -cs)
    echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
    ```

4. <span data-ttu-id="5416a-113">Mettez à jour les informations concernant le référentiel, puis installez le package `azure-cli` :</span><span class="sxs-lookup"><span data-stu-id="5416a-113">Update repository information and install the `azure-cli` package:</span></span>

    ```bash
    sudo apt-get update
    sudo apt-get install azure-cli
    ```

<span data-ttu-id="5416a-114">Exécutez Azure CLI avec la commande `az`.</span><span class="sxs-lookup"><span data-stu-id="5416a-114">Run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="5416a-115">Pour vous connecter, utilisez la commande [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="5416a-115">To sign in, use the [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="5416a-116">Pour en savoir plus sur les différentes méthodes d’authentification, consultez [Se connecter avec Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="5416a-116">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="5416a-117">Résolution de problèmes</span><span class="sxs-lookup"><span data-stu-id="5416a-117">Troubleshooting</span></span>

<span data-ttu-id="5416a-118">Voici certains problèmes courants lors de l’installation avec `apt`.</span><span class="sxs-lookup"><span data-stu-id="5416a-118">Here are some common problems seen when installing with `apt`.</span></span> <span data-ttu-id="5416a-119">Si vous rencontrez un problème n’étant pas évoqué ici, [signalez un problème sur github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="5416a-119">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="lsbrelease-does-not-return-the-correct-base-distribution-version"></a><span data-ttu-id="5416a-120">lsb_release ne renvoie pas la bonne version de la distribution de base</span><span class="sxs-lookup"><span data-stu-id="5416a-120">lsb_release does not return the correct base distribution version</span></span>

<span data-ttu-id="5416a-121">Certaines distributions Ubuntu ou Debian dérivées, telles que Linux Mint peuvent ne pas retourner le nom de version correct de `lsb_release`.</span><span class="sxs-lookup"><span data-stu-id="5416a-121">Some Ubuntu- or Debian-derived distributions such as Linux Mint may not return the correct version name from `lsb_release`.</span></span> <span data-ttu-id="5416a-122">Cette valeur est utilisée dans le processus d’installation pour déterminer le package à installer.</span><span class="sxs-lookup"><span data-stu-id="5416a-122">This value is used in the install process to determine the package to install.</span></span> <span data-ttu-id="5416a-123">Si vous connaissez le nom de code de la version Ubuntu ou Debian dont votre distribution est dérivée, vous pouvez définir la valeur `AZ_REPO` manuellement lors de l’[ajout du référentiel](#set-release).</span><span class="sxs-lookup"><span data-stu-id="5416a-123">If you know the code name of the Ubuntu or Debian version your distribution is derived from, you can set the `AZ_REPO` value manually when [adding the repository](#set-release).</span></span> <span data-ttu-id="5416a-124">Dans le cas contraire, recherchez des informations expliquant comment déterminer le nom de code de la distribution de base et définir `AZ_REPO` sur la valeur appropriée.</span><span class="sxs-lookup"><span data-stu-id="5416a-124">Otherwise, look up information for your distribution on how to determine the base distribution code name and set `AZ_REPO` to the correct value.</span></span>

### <a name="no-package-for-your-distribution"></a><span data-ttu-id="5416a-125">Aucun package pour votre distribution</span><span class="sxs-lookup"><span data-stu-id="5416a-125">No package for your distribution</span></span>

<span data-ttu-id="5416a-126">Après la publication d’une distribution, il peut se passer un certain temps avant que le package Azure CLI associé ne soit disponible.</span><span class="sxs-lookup"><span data-stu-id="5416a-126">Sometimes it may be a while after a distribution is released before there's an Azure CLI package available for it.</span></span> <span data-ttu-id="5416a-127">Azure CLI est conçu pour résister à de futures versions de dépendances, et repose sur peu d’entre elles.</span><span class="sxs-lookup"><span data-stu-id="5416a-127">The Azure CLI designed to be resilient with regards to future versions of dependencies and rely on as few of them as possible.</span></span> <span data-ttu-id="5416a-128">Si aucun package n’est disponible pour votre distribution de base, essayez d’utiliser le package d’une distribution antérieure.</span><span class="sxs-lookup"><span data-stu-id="5416a-128">If there's no package available for your base distribution, try a package for an earlier distribution.</span></span>

<span data-ttu-id="5416a-129">Pour cela, définissez la valeur de `AZ_REPO` manuellement lors de l’[ajout du référentiel](#set-release).</span><span class="sxs-lookup"><span data-stu-id="5416a-129">To do this, set the value of `AZ_REPO` manually when [adding the repository](#set-release).</span></span> <span data-ttu-id="5416a-130">Pour les distributions Ubuntu, utilisez le référentiel `bionic`, et `stretch` pour les distributions Debian.</span><span class="sxs-lookup"><span data-stu-id="5416a-130">For Ubuntu distributions use the `bionic` repository, and for Debian distributions use `stretch`.</span></span> <span data-ttu-id="5416a-131">Les distributions publiées avant Ubuntu Trusty et Debian Wheezy ne sont pas prises en charge.</span><span class="sxs-lookup"><span data-stu-id="5416a-131">Distributions released before Ubuntu Trusty and Debian Wheezy are not supported.</span></span>

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="update"></a><span data-ttu-id="5416a-132">Mettre à jour</span><span class="sxs-lookup"><span data-stu-id="5416a-132">Update</span></span>

<span data-ttu-id="5416a-133">Utilisez `apt-get upgrade` pour mettre à jour le package de l’interface de ligne de commande.</span><span class="sxs-lookup"><span data-stu-id="5416a-133">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> <span data-ttu-id="5416a-134">Cette commande met à niveau tous les packages installés sur votre système n’ayant pas de modification de dépendance.</span><span class="sxs-lookup"><span data-stu-id="5416a-134">This command upgrades all of the installed packages on your system that have not had a dependency change.</span></span>
> <span data-ttu-id="5416a-135">Pour mettre à niveau uniquement l’interface CLI, utilisez `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="5416a-135">To upgrade the CLI only, use `apt-get install`.</span></span>
> 
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

## <a name="uninstall"></a><span data-ttu-id="5416a-136">Désinstaller l’interface</span><span class="sxs-lookup"><span data-stu-id="5416a-136">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="5416a-137">Désinstaller avec `apt-get remove` :</span><span class="sxs-lookup"><span data-stu-id="5416a-137">Uninstall with `apt-get remove`:</span></span>

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. <span data-ttu-id="5416a-138">Si vous ne prévoyez pas de réinstaller l’interface CLI, supprimez les informations de référentiel Azure CLI :</span><span class="sxs-lookup"><span data-stu-id="5416a-138">If you don't plan to reinstall the CLI, remove the Azure CLI repository information:</span></span>

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. <span data-ttu-id="5416a-139">Supprimer la clé de signature :</span><span class="sxs-lookup"><span data-stu-id="5416a-139">Remove the signing key:</span></span>

    ```bash
    sudo rm /etc/apt/trusted.gpg.d/microsoft.asc.gpg
    ```

4. <span data-ttu-id="5416a-140">Supprimer tous les packages inutiles :</span><span class="sxs-lookup"><span data-stu-id="5416a-140">Remove any unneeded packages:</span></span>

   ```bash
   sudo apt autoremove
   ```

## <a name="next-steps"></a><span data-ttu-id="5416a-141">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="5416a-141">Next Steps</span></span>

<span data-ttu-id="5416a-142">Maintenant que vous avez installé l’interface CLI, découvrez ses fonctionnalités et ses commandes courantes.</span><span class="sxs-lookup"><span data-stu-id="5416a-142">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="5416a-143">Prise en main de l’interface Azure CLI</span><span class="sxs-lookup"><span data-stu-id="5416a-143">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
