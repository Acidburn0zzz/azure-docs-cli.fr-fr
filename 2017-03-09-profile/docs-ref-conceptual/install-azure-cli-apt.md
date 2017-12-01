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
ms.openlocfilehash: 93d947d91973def1c05e2f5b2e7511bc1c5704a2
ms.sourcegitcommit: 905939cc44764b4d1cc79a9b36c0793f7055a686
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/20/2017
---
# <a name="install-azure-cli-20-with-apt"></a><span data-ttu-id="c6c77-104">Installer Azure CLI 2.0 avec apt</span><span class="sxs-lookup"><span data-stu-id="c6c77-104">Install Azure CLI 2.0 with apt</span></span>

<span data-ttu-id="c6c77-105">Si vous exécutez une distribution qui est fournie avec `apt`, telle que Ubuntu ou Debian, vous pouvez installer un package pour l’interface de ligne de commande Azure sur votre système.</span><span class="sxs-lookup"><span data-stu-id="c6c77-105">If you are running a distirbution that comes with `apt`, such as Ubuntu or Debian, there is an available package for the Azure CLI that you can install on your system.</span></span>

> [!NOTE]
> <span data-ttu-id="c6c77-106">Vous devez disposer de Python 2.7.x ou Python 3.x pour pouvoir utiliser l’interface CLI.</span><span class="sxs-lookup"><span data-stu-id="c6c77-106">You must have Python 2.7.x or Python 3.x in order to use the CLI.</span></span> <span data-ttu-id="c6c77-107">Si votre distribution ne dispose pas d’un package pour l’un ou l’autre, [installez Python](https://www.python.org/downloads/).</span><span class="sxs-lookup"><span data-stu-id="c6c77-107">If your distribution does not have a package for either, [install Python](https://www.python.org/downloads/).</span></span>

## <a name="install"></a><span data-ttu-id="c6c77-108">Installer</span><span class="sxs-lookup"><span data-stu-id="c6c77-108">Install</span></span>

1. <span data-ttu-id="c6c77-109">Modifiez votre liste de sources :</span><span class="sxs-lookup"><span data-stu-id="c6c77-109">Modify your sources list:</span></span>
 
   - <span data-ttu-id="c6c77-110">Système 32 bits</span><span class="sxs-lookup"><span data-stu-id="c6c77-110">32-bit system</span></span>

     ```bash
     echo "deb https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

   - <span data-ttu-id="c6c77-111">Système 64 bits</span><span class="sxs-lookup"><span data-stu-id="c6c77-111">64-bit system</span></span>

     ```bash
     echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

2. <span data-ttu-id="c6c77-112">Exécutez les commandes sudo suivantes :</span><span class="sxs-lookup"><span data-stu-id="c6c77-112">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

<span data-ttu-id="c6c77-113">Vous pouvez exécuter l’interface de ligne de commande Azure avec la commande `az`.</span><span class="sxs-lookup"><span data-stu-id="c6c77-113">You can run the Azure CLI with the `az` command.</span></span>

## <a name="update"></a><span data-ttu-id="c6c77-114">Mettre à jour</span><span class="sxs-lookup"><span data-stu-id="c6c77-114">Update</span></span>

<span data-ttu-id="c6c77-115">Utilisez `apt-get upgrade` pour mettre à jour le package de l’interface de ligne de commande.</span><span class="sxs-lookup"><span data-stu-id="c6c77-115">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> <span data-ttu-id="c6c77-116">Cela met à niveau tous les packages installés sur votre système n’ayant pas de modification de dépendance.</span><span class="sxs-lookup"><span data-stu-id="c6c77-116">This will upgrade all of the installed packages on your system which have not had a dependency change.</span></span>
> <span data-ttu-id="c6c77-117">Pour ne mettre à niveau que l’interface de ligne de commande, utilisez `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="c6c77-117">To upgrade only the CLI, use `apt-get install`.</span></span>
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

### <a name="uninstall"></a><span data-ttu-id="c6c77-118">Désinstaller l’interface</span><span class="sxs-lookup"><span data-stu-id="c6c77-118">Uninstall</span></span>

<span data-ttu-id="c6c77-119">Si jamais vous décidez de désinstaller l’interface de ligne de commande Azure, nous sommes désolés de vous voir partir.</span><span class="sxs-lookup"><span data-stu-id="c6c77-119">If you ever decide to uninstall the Azure CLI, we're sorry to see you go.</span></span> <span data-ttu-id="c6c77-120">Avant de désinstaller, utilisez la commande `az feedback`, afin de nous donner quelques raisons pour lesquelles vous avez choisi de désinstaller et nous aider à améliorer l’expérience CLI.</span><span class="sxs-lookup"><span data-stu-id="c6c77-120">Before you uninstall, use the `az feedback` command to give us some reasons why you chose to uninstall and how we could improve the CLI experience.</span></span> <span data-ttu-id="c6c77-121">Nous souhaitons nous assurer que l’interface de ligne de commande Azure est aussi conviviale et exempte de bogues que possible.</span><span class="sxs-lookup"><span data-stu-id="c6c77-121">We want to make sure that the Azure CLI is as bug-free and user-friendly as we can make it.</span></span> <span data-ttu-id="c6c77-122">Vous pouvez également [signaler un problème lié à GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="c6c77-122">You can also [file a github issue](https://github.com/Azure/azure-cli/issues).</span></span>

1. <span data-ttu-id="c6c77-123">Désinstaller avec `apt-get remove`.</span><span class="sxs-lookup"><span data-stu-id="c6c77-123">Uninstall with `apt-get remove`.</span></span>

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. <span data-ttu-id="c6c77-124">Si vous ne souhaitez pas réinstaller l’interface de ligne de commande, supprimez les informations de référentiel Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="c6c77-124">If you do not plan to reinstall the CLI, remove the Azure CLI repository information.</span></span>

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. <span data-ttu-id="c6c77-125">Supprimez tous les packages inutiles.</span><span class="sxs-lookup"><span data-stu-id="c6c77-125">Remove any unneeded packages.</span></span>

   ```bash
   sudo apt autoremove
   ```
