---
title: "Installation d’Azure CLI 2.0 pour Linux avec apt"
description: "Installation d’Azure CLI 2.0 avec le gestionnaire de package apt"
keywords: "Azure CLI, installation d’Azure CLI, Azure apt, Azure Debian, Azure Ubuntu"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 01/29/18
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: fdd9f0061d5d38ed5a349b11eb0f5f27786bc1ab
ms.sourcegitcommit: 8606f36963e8daa6448d637393d1e4ef2c9859a0
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/01/2018
---
# <a name="install-azure-cli-20-with-apt"></a><span data-ttu-id="14830-104">Installer Azure CLI 2.0 avec apt</span><span class="sxs-lookup"><span data-stu-id="14830-104">Install Azure CLI 2.0 with apt</span></span>

<span data-ttu-id="14830-105">Si vous exécutez une distribution qui est fournie avec `apt`, telle que Ubuntu ou Debian, un package est disponible pour l’interface de ligne de commande Azure.</span><span class="sxs-lookup"><span data-stu-id="14830-105">If you are running a distribution that comes with `apt`, such as Ubuntu or Debian, there is a package available for the Azure CLI.</span></span> <span data-ttu-id="14830-106">Ce package a été testé avec Ubuntu Wheezy et Ubuntu Xenial.</span><span class="sxs-lookup"><span data-stu-id="14830-106">This package has been tested with Ubuntu Wheezy and Ubuntu Xenial.</span></span>

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a><span data-ttu-id="14830-107">Installer</span><span class="sxs-lookup"><span data-stu-id="14830-107">Install</span></span>

1. <span data-ttu-id="14830-108">Modifiez votre liste de sources :</span><span class="sxs-lookup"><span data-stu-id="14830-108">Modify your sources list:</span></span>

   - <span data-ttu-id="14830-109">Système 32 bits</span><span class="sxs-lookup"><span data-stu-id="14830-109">32-bit system</span></span>

     ```bash
     echo "deb https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

   - <span data-ttu-id="14830-110">Système 64 bits</span><span class="sxs-lookup"><span data-stu-id="14830-110">64-bit system</span></span>

     ```bash
     echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

2. <span data-ttu-id="14830-111">Exécutez les commandes sudo suivantes :</span><span class="sxs-lookup"><span data-stu-id="14830-111">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

<span data-ttu-id="14830-112">Vous pouvez exécuter l’interface de ligne de commande Azure avec la commande `az`.</span><span class="sxs-lookup"><span data-stu-id="14830-112">You can run the Azure CLI with the `az` command.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="14830-113">Résolution de problèmes</span><span class="sxs-lookup"><span data-stu-id="14830-113">Troubleshooting</span></span>

<span data-ttu-id="14830-114">Voici certains problèmes courants lors de l’installation avec `apt`.</span><span class="sxs-lookup"><span data-stu-id="14830-114">Here are some common problems seen when installing with `apt`.</span></span> <span data-ttu-id="14830-115">Si votre problème ne figure pas ici, veuillez [signaler le problème sur Github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="14830-115">If your issue is not listed here, please [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="apt-key-fails-with-no-dirmngr"></a><span data-ttu-id="14830-116">Clé apt échoue avec le message « No dirmngr »</span><span class="sxs-lookup"><span data-stu-id="14830-116">apt-key fails with "No dirmngr"</span></span>

<span data-ttu-id="14830-117">Lorsque vous exécutez la commande `apt-key`, vous pouvez voir une sortie similaire à l’erreur suivante :</span><span class="sxs-lookup"><span data-stu-id="14830-117">When running the `apt-key` command, you may see output similar to the following error:</span></span>

```output
gpg: failed to start the dirmngr '/usr/bin/dirmngr': No such file or directory
gpg: connecting dirmngr at '/tmp/apt-key-gpghome.kt5zo27tp1/S.dirmngr' failed: No such file or directory
gpg: keyserver receive failed: No dirmngr
```

<span data-ttu-id="14830-118">Cette erreur est due à un composant manquant requis par `apt-key`.</span><span class="sxs-lookup"><span data-stu-id="14830-118">The error is due to a missing component required by `apt-key`.</span></span> <span data-ttu-id="14830-119">Vous pouvez résoudre ce problème en installant le package `dirmngr`.</span><span class="sxs-lookup"><span data-stu-id="14830-119">You can resolve it by installing the `dirmngr` package.</span></span>

```bash
sudo apt-get install dirmngr
```

## <a name="update"></a><span data-ttu-id="14830-120">Mettre à jour</span><span class="sxs-lookup"><span data-stu-id="14830-120">Update</span></span>

<span data-ttu-id="14830-121">Utilisez `apt-get upgrade` pour mettre à jour le package de l’interface de ligne de commande.</span><span class="sxs-lookup"><span data-stu-id="14830-121">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> <span data-ttu-id="14830-122">Cette commande met à niveau tous les packages installés sur votre système n’ayant pas de modification de dépendance.</span><span class="sxs-lookup"><span data-stu-id="14830-122">This command upgrades all of the installed packages on your system that have not had a dependency change.</span></span>
> <span data-ttu-id="14830-123">Pour mettre à niveau uniquement l’interface CLI, utilisez `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="14830-123">To upgrade the CLI only, use `apt-get install`.</span></span>
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

## <a name="uninstall"></a><span data-ttu-id="14830-124">Désinstaller l’interface</span><span class="sxs-lookup"><span data-stu-id="14830-124">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="14830-125">Désinstaller avec `apt-get remove`.</span><span class="sxs-lookup"><span data-stu-id="14830-125">Uninstall with `apt-get remove`.</span></span>

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. <span data-ttu-id="14830-126">Si vous ne souhaitez pas réinstaller l’interface de ligne de commande, supprimez les informations de référentiel Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="14830-126">If you do not plan to reinstall the CLI, remove the Azure CLI repository information.</span></span>

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. <span data-ttu-id="14830-127">Supprimez tous les packages inutiles.</span><span class="sxs-lookup"><span data-stu-id="14830-127">Remove any unneeded packages.</span></span>

   ```bash
   sudo apt autoremove
   ```
