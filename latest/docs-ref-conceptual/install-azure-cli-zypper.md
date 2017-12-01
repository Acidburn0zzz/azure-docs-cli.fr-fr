---
title: Installer Azure CLI 2.0 avec zypper
description: "Installation d’Azure CLI 2.0 avec zypper"
keywords: "Azure CLI, installation d’Azure CLI, Azure CLI zypper, Azure CLI opensuse, Azure CLI sle"
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
ms.openlocfilehash: c01679ccb77880f1f628f4e48683d8ff030a568b
ms.sourcegitcommit: 905939cc44764b4d1cc79a9b36c0793f7055a686
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/20/2017
---
# <a name="install-azure-cli-20-with-zypper"></a><span data-ttu-id="26afe-104">Installer Azure CLI 2.0 avec zypper</span><span class="sxs-lookup"><span data-stu-id="26afe-104">Install Azure CLI 2.0 with zypper</span></span>

<span data-ttu-id="26afe-105">Si vous exécutez une distribution qui est fournie avec `zypper`, telle que OpenSUSE ou SLE, vous pouvez installer un package pour l’interface de ligne de commande Azure sur votre système.</span><span class="sxs-lookup"><span data-stu-id="26afe-105">If you are running a distirbution that comes with `zypper`, such as OpenSUSE or SLE, there is an available package for the Azure CLI that you can install on your system.</span></span>

> [!NOTE]
> <span data-ttu-id="26afe-106">Vous devez disposer de Python 2.7.x ou Python 3.x pour pouvoir utiliser l’interface CLI.</span><span class="sxs-lookup"><span data-stu-id="26afe-106">You must have Python 2.7.x or Python 3.x in order to use the CLI.</span></span> <span data-ttu-id="26afe-107">Si votre distribution ne dispose pas d’un package pour l’un ou l’autre, [installez Python](https://www.python.org/downloads/).</span><span class="sxs-lookup"><span data-stu-id="26afe-107">If your distribution does not have a package for either, [install Python](https://www.python.org/downloads/).</span></span>

## <a name="install"></a><span data-ttu-id="26afe-108">Installer</span><span class="sxs-lookup"><span data-stu-id="26afe-108">Install</span></span> 

1. <span data-ttu-id="26afe-109">Installez `curl` :</span><span class="sxs-lookup"><span data-stu-id="26afe-109">Install `curl`:</span></span>

   ```bash
   sudo zypper refresh
   sudo zypper install -y curl
   ```

2. <span data-ttu-id="26afe-110">Importer la clé de référentiel Microsoft :</span><span class="sxs-lookup"><span data-stu-id="26afe-110">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

3. <span data-ttu-id="26afe-111">Créer des informations de référentiel `azure-cli` locales :</span><span class="sxs-lookup"><span data-stu-id="26afe-111">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ntype=rpm-md\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/zypp/repos.d/azure-cli.repo'
   ```

4. <span data-ttu-id="26afe-112">Mettre à jour l’index de package `zypper` et l’installer :</span><span class="sxs-lookup"><span data-stu-id="26afe-112">Update the `zypper` package index and install:</span></span>

   ```bash
   sudo zypper refresh
   sudo zypper install -y azure-cli
   ```

<span data-ttu-id="26afe-113">Vous pouvez exécuter l’interface de ligne de commande avec la commande `az`.</span><span class="sxs-lookup"><span data-stu-id="26afe-113">You can run the CLI with the `az` command.</span></span>

## <a name="update"></a><span data-ttu-id="26afe-114">Mettre à jour</span><span class="sxs-lookup"><span data-stu-id="26afe-114">Update</span></span>

<span data-ttu-id="26afe-115">Vous pouvez mettre à jour le package avec la commande `zypper update`.</span><span class="sxs-lookup"><span data-stu-id="26afe-115">You can update the package with the `zypper update` command.</span></span>

```bash
sudo zypper refresh
sudo zypper update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="26afe-116">Désinstaller l’interface</span><span class="sxs-lookup"><span data-stu-id="26afe-116">Uninstall</span></span>

<span data-ttu-id="26afe-117">Si jamais vous décidez de désinstaller l’interface de ligne de commande Azure, nous sommes désolés de vous voir partir.</span><span class="sxs-lookup"><span data-stu-id="26afe-117">If you ever decide to uninstall the Azure CLI, we're sorry to see you go.</span></span> <span data-ttu-id="26afe-118">Avant de désinstaller, utilisez la commande `az feedback`, afin de nous donner quelques raisons pour lesquelles vous avez choisi de désinstaller et nous aider à améliorer l’expérience CLI.</span><span class="sxs-lookup"><span data-stu-id="26afe-118">Before you uninstall, use the `az feedback` command to give us some reasons why you chose to uninstall and how we could improve the CLI experience.</span></span> <span data-ttu-id="26afe-119">Nous souhaitons nous assurer que l’interface de ligne de commande Azure est aussi conviviale et exempte de bogues que possible.</span><span class="sxs-lookup"><span data-stu-id="26afe-119">We want to make sure that the Azure CLI is as bug-free and user-friendly as we can make it.</span></span> <span data-ttu-id="26afe-120">Vous pouvez également [signaler un problème lié à GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="26afe-120">You can also [file a github issue](https://github.com/Azure/azure-cli/issues).</span></span>

1. <span data-ttu-id="26afe-121">Supprimez le package de votre système.</span><span class="sxs-lookup"><span data-stu-id="26afe-121">Remove the package from your system.</span></span>

    ```bash
    sudo zypper remove -y azure-cli
    ```

2. <span data-ttu-id="26afe-122">Si vous ne souhaitez pas réinstaller l’interface CLI, supprimez les informations de référentiel.</span><span class="sxs-lookup"><span data-stu-id="26afe-122">If you do not plan to reinstall the CLI, remove the repository information.</span></span>

  ```bash
  sudo rm /etc/zypp/repos.d/azure-cli.repo
  ```

3. <span data-ttu-id="26afe-123">Si vous avez supprimé les informations de référentiel, supprimez également la clé de signature Microsoft GPG.</span><span class="sxs-lookup"><span data-stu-id="26afe-123">If you removed the repository information, also remove the Microsoft GPG signature key.</span></span>

  ```bash
  MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
  sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
  ```

