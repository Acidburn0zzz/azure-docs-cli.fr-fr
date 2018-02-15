---
title: "Installation d’Azure CLI 2.0 pour Linux avec zypper"
description: "Installation d’Azure CLI 2.0 avec zypper"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 01/29/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 6ee3aff74f43fab0c80c58c7fe57c9fa74a6ef2f
ms.sourcegitcommit: b93a19222e116d5880bbe64c03507c64e190331e
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/15/2018
---
# <a name="install-azure-cli-20-with-zypper"></a><span data-ttu-id="fd39f-103">Installer Azure CLI 2.0 avec zypper</span><span class="sxs-lookup"><span data-stu-id="fd39f-103">Install Azure CLI 2.0 with zypper</span></span>

<span data-ttu-id="fd39f-104">Si vous exécutez une distribution qui est fournie avec `zypper`, telle que openSUSE ou SLES, un package est disponible pour l’interface de ligne de commande Azure.</span><span class="sxs-lookup"><span data-stu-id="fd39f-104">If you are running a distribution that comes with `zypper`, such as openSUSE or SLES, there is a package available for the Azure CLI.</span></span> <span data-ttu-id="fd39f-105">Ce package a été testé avec openSUSE 42.2 et SLES 12 SP 2.</span><span class="sxs-lookup"><span data-stu-id="fd39f-105">This package has been tested with openSUSE 42.2 and SLES 12 SP 2.</span></span>

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a><span data-ttu-id="fd39f-106">Installer</span><span class="sxs-lookup"><span data-stu-id="fd39f-106">Install</span></span>

1. <span data-ttu-id="fd39f-107">Installez `curl` :</span><span class="sxs-lookup"><span data-stu-id="fd39f-107">Install `curl`:</span></span>

   ```bash
   sudo zypper refresh
   sudo zypper install -y curl
   ```

2. <span data-ttu-id="fd39f-108">Importer la clé de référentiel Microsoft :</span><span class="sxs-lookup"><span data-stu-id="fd39f-108">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

3. <span data-ttu-id="fd39f-109">Créer des informations de référentiel `azure-cli` locales :</span><span class="sxs-lookup"><span data-stu-id="fd39f-109">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ntype=rpm-md\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/zypp/repos.d/azure-cli.repo'
   ```

4. <span data-ttu-id="fd39f-110">Mettre à jour l’index de package `zypper` et l’installer :</span><span class="sxs-lookup"><span data-stu-id="fd39f-110">Update the `zypper` package index and install:</span></span>

   ```bash
   sudo zypper refresh
   sudo zypper install -y azure-cli
   ```

<span data-ttu-id="fd39f-111">Vous pouvez exécuter l’interface de ligne de commande avec la commande `az`.</span><span class="sxs-lookup"><span data-stu-id="fd39f-111">You can run the CLI with the `az` command.</span></span>

## <a name="update"></a><span data-ttu-id="fd39f-112">Mettre à jour</span><span class="sxs-lookup"><span data-stu-id="fd39f-112">Update</span></span>

<span data-ttu-id="fd39f-113">Vous pouvez mettre à jour le package avec la commande `zypper update`.</span><span class="sxs-lookup"><span data-stu-id="fd39f-113">You can update the package with the `zypper update` command.</span></span>

```bash
sudo zypper refresh
sudo zypper update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="fd39f-114">Désinstaller l’interface</span><span class="sxs-lookup"><span data-stu-id="fd39f-114">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="fd39f-115">Supprimez le package de votre système.</span><span class="sxs-lookup"><span data-stu-id="fd39f-115">Remove the package from your system.</span></span>

    ```bash
    sudo zypper remove -y azure-cli
    ```

2. <span data-ttu-id="fd39f-116">Si vous ne souhaitez pas réinstaller l’interface CLI, supprimez les informations de référentiel.</span><span class="sxs-lookup"><span data-stu-id="fd39f-116">If you do not plan to reinstall the CLI, remove the repository information.</span></span>

  ```bash
  sudo rm /etc/zypp/repos.d/azure-cli.repo
  ```

3. <span data-ttu-id="fd39f-117">Si vous avez supprimé les informations de référentiel, supprimez également la clé de signature Microsoft GPG.</span><span class="sxs-lookup"><span data-stu-id="fd39f-117">If you removed the repository information, also remove the Microsoft GPG signature key.</span></span>

  ```bash
  MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
  sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
  ```

