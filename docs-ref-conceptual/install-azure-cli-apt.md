---
title: Installer Azure CLI 2.0 avec apt
description: "Installation d’Azure CLI 2.0 avec le gestionnaire de package apt"
keywords: "Azure CLI, installation d’Azure CLI, Azure apt, Azure Debian, Azure Ubuntu"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 11/01/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ROBOTS: NOINDEX,NOFOLLOW
ms.openlocfilehash: 65e8e78275b0f40a2298934fe8bc9368bbf796a7
ms.sourcegitcommit: 59f0b667f2202bae8914e6fc8dc5c9dc79fef91c
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/25/2018
---
# <a name="install-azure-cli-20-with-apt"></a><span data-ttu-id="969fd-104">Installer Azure CLI 2.0 avec apt</span><span class="sxs-lookup"><span data-stu-id="969fd-104">Install Azure CLI 2.0 with apt</span></span>

<span data-ttu-id="969fd-105">Si vous exécutez une distribution qui est fournie avec `apt`, telle que Ubuntu ou Debian, vous pouvez installer un package pour l’interface de ligne de commande Azure sur votre système.</span><span class="sxs-lookup"><span data-stu-id="969fd-105">If you are running a distirbution that comes with `apt`, such as Ubuntu or Debian, there is an available package for the Azure CLI that you can install on your system.</span></span>

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a><span data-ttu-id="969fd-106">Installer</span><span class="sxs-lookup"><span data-stu-id="969fd-106">Install</span></span>

1. <span data-ttu-id="969fd-107">Modifiez votre liste de sources :</span><span class="sxs-lookup"><span data-stu-id="969fd-107">Modify your sources list:</span></span>

   - <span data-ttu-id="969fd-108">Système 32 bits</span><span class="sxs-lookup"><span data-stu-id="969fd-108">32-bit system</span></span>

     ```bash
     echo "deb https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

   - <span data-ttu-id="969fd-109">Système 64 bits</span><span class="sxs-lookup"><span data-stu-id="969fd-109">64-bit system</span></span>

     ```bash
     echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

2. <span data-ttu-id="969fd-110">Exécutez les commandes sudo suivantes :</span><span class="sxs-lookup"><span data-stu-id="969fd-110">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

<span data-ttu-id="969fd-111">Vous pouvez exécuter l’interface de ligne de commande Azure avec la commande `az`.</span><span class="sxs-lookup"><span data-stu-id="969fd-111">You can run the Azure CLI with the `az` command.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="969fd-112">Résolution de problèmes</span><span class="sxs-lookup"><span data-stu-id="969fd-112">Troubleshooting</span></span>

### <a name="apt-key-fails-with-no-dirmngr"></a><span data-ttu-id="969fd-113">Clé apt échoue avec le message « No dirmngr »</span><span class="sxs-lookup"><span data-stu-id="969fd-113">apt-key fails with "No dirmngr"</span></span>

<span data-ttu-id="969fd-114">Lorsque vous exécutez la commande `apt-key`, vous pouvez voir une sortie similaire à l’erreur suivante.</span><span class="sxs-lookup"><span data-stu-id="969fd-114">When running the `apt-key` command, you may see output similar to the following error.</span></span>

```output
gpg: failed to start the dirmngr '/usr/bin/dirmngr': No such file or directory
gpg: connecting dirmngr at '/tmp/apt-key-gpghome.kt5zo27tp1/S.dirmngr' failed: No such file or directory
gpg: keyserver receive failed: No dirmngr
```

<span data-ttu-id="969fd-115">Cela est dû à un composant manquant requis par `apt-key`.</span><span class="sxs-lookup"><span data-stu-id="969fd-115">This is due to a missing component required by `apt-key`.</span></span> <span data-ttu-id="969fd-116">Vous pouvez résoudre ce problème en installant le package `dirmngr`.</span><span class="sxs-lookup"><span data-stu-id="969fd-116">You can resolve this by installing the `dirmngr` package.</span></span>

```bash
sudo apt-get install dirmngr
```

## <a name="update"></a><span data-ttu-id="969fd-117">Mettre à jour</span><span class="sxs-lookup"><span data-stu-id="969fd-117">Update</span></span>

<span data-ttu-id="969fd-118">Utilisez `apt-get upgrade` pour mettre à jour le package de l’interface de ligne de commande.</span><span class="sxs-lookup"><span data-stu-id="969fd-118">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> <span data-ttu-id="969fd-119">Cela met à niveau tous les packages installés sur votre système n’ayant pas de modification de dépendance.</span><span class="sxs-lookup"><span data-stu-id="969fd-119">This will upgrade all of the installed packages on your system which have not had a dependency change.</span></span>
> <span data-ttu-id="969fd-120">Pour ne mettre à niveau que l’interface de ligne de commande, utilisez `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="969fd-120">To upgrade only the CLI, use `apt-get install`.</span></span>
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

### <a name="uninstall"></a><span data-ttu-id="969fd-121">Désinstaller l’interface</span><span class="sxs-lookup"><span data-stu-id="969fd-121">Uninstall</span></span>

<span data-ttu-id="969fd-122">Si jamais vous décidez de désinstaller l’interface de ligne de commande Azure, nous sommes désolés de vous voir partir.</span><span class="sxs-lookup"><span data-stu-id="969fd-122">If you ever decide to uninstall the Azure CLI, we're sorry to see you go.</span></span> <span data-ttu-id="969fd-123">Avant de désinstaller, utilisez la commande `az feedback`, afin de nous donner quelques raisons pour lesquelles vous avez choisi de désinstaller et nous aider à améliorer l’expérience CLI.</span><span class="sxs-lookup"><span data-stu-id="969fd-123">Before you uninstall, use the `az feedback` command to give us some reasons why you chose to uninstall and how we could improve the CLI experience.</span></span> <span data-ttu-id="969fd-124">Nous souhaitons nous assurer que l’interface de ligne de commande Azure est aussi conviviale et exempte de bogues que possible.</span><span class="sxs-lookup"><span data-stu-id="969fd-124">We want to make sure that the Azure CLI is as bug-free and user-friendly as we can make it.</span></span> <span data-ttu-id="969fd-125">Vous pouvez également [signaler un problème lié à GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="969fd-125">You can also [file a github issue](https://github.com/Azure/azure-cli/issues).</span></span>

1. <span data-ttu-id="969fd-126">Désinstaller avec `apt-get remove`.</span><span class="sxs-lookup"><span data-stu-id="969fd-126">Uninstall with `apt-get remove`.</span></span>

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. <span data-ttu-id="969fd-127">Si vous ne souhaitez pas réinstaller l’interface de ligne de commande, supprimez les informations de référentiel Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="969fd-127">If you do not plan to reinstall the CLI, remove the Azure CLI repository information.</span></span>

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. <span data-ttu-id="969fd-128">Supprimez tous les packages inutiles.</span><span class="sxs-lookup"><span data-stu-id="969fd-128">Remove any unneeded packages.</span></span>

   ```bash
   sudo apt autoremove
   ```
