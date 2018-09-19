---
title: Installation d’Azure CLI 2.0 pour Linux avec zypper
description: Installation d’Azure CLI 2.0 avec zypper
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: ed92443b6de4e538eaf5da41376e836aa2c771a0
ms.sourcegitcommit: 0e688704889fc88b91588bb6678a933c2d54f020
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/11/2018
ms.locfileid: "44388301"
---
# <a name="install-azure-cli-20-with-zypper"></a><span data-ttu-id="bc4f9-103">Installer Azure CLI 2.0 avec zypper</span><span class="sxs-lookup"><span data-stu-id="bc4f9-103">Install Azure CLI 2.0 with zypper</span></span>

<span data-ttu-id="bc4f9-104">Pour les distributions Linux avec `zypper`, telles que openSUSE ou SLES, un package est disponible pour l’Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="bc4f9-104">For Linux distributions with `zypper`, such as openSUSE or SLES, there's a package available for the Azure CLI.</span></span> <span data-ttu-id="bc4f9-105">Ce package a été testé avec openSUSE 42.2 et SLES 12 SP 2.</span><span class="sxs-lookup"><span data-stu-id="bc4f9-105">This package has been tested with openSUSE 42.2 and SLES 12 SP 2.</span></span>

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a><span data-ttu-id="bc4f9-106">Installer</span><span class="sxs-lookup"><span data-stu-id="bc4f9-106">Install</span></span>

1. <span data-ttu-id="bc4f9-107">Installez `curl` :</span><span class="sxs-lookup"><span data-stu-id="bc4f9-107">Install `curl`:</span></span>

   ```bash
   sudo zypper install -y curl
   ```

2. <span data-ttu-id="bc4f9-108">Importer la clé de référentiel Microsoft :</span><span class="sxs-lookup"><span data-stu-id="bc4f9-108">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

3. <span data-ttu-id="bc4f9-109">Créer des informations de référentiel `azure-cli` locales :</span><span class="sxs-lookup"><span data-stu-id="bc4f9-109">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo zypper addrepo --name 'Azure CLI' --check https://packages.microsoft.com/yumrepos/azure-cli azure-cli
   ```

4. <span data-ttu-id="bc4f9-110">Mettre à jour l’index de package `zypper` et l’installer :</span><span class="sxs-lookup"><span data-stu-id="bc4f9-110">Update the `zypper` package index and install:</span></span>

   ```bash
   sudo zypper install --from azure-cli -y azure-cli
   ```

<span data-ttu-id="bc4f9-111">Vous pouvez ensuite exécuter l’interface de ligne de commande Azure avec la commande `az`.</span><span class="sxs-lookup"><span data-stu-id="bc4f9-111">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="bc4f9-112">Pour vous connecter, utilisez la commande [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="bc4f9-112">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="bc4f9-113">Pour en savoir plus sur les différentes méthodes d’authentification, consultez [Se connecter avec Azure CLI 2.0](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="bc4f9-113">To learn more about different authentication methods, see [Sign in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

## <a name="update"></a><span data-ttu-id="bc4f9-114">Mettre à jour</span><span class="sxs-lookup"><span data-stu-id="bc4f9-114">Update</span></span>

<span data-ttu-id="bc4f9-115">Vous pouvez mettre à jour le package avec la commande `zypper update`.</span><span class="sxs-lookup"><span data-stu-id="bc4f9-115">You can update the package with the `zypper update` command.</span></span>

```bash
sudo zypper refresh
sudo zypper update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="bc4f9-116">Désinstaller l’interface</span><span class="sxs-lookup"><span data-stu-id="bc4f9-116">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="bc4f9-117">Supprimez le package de votre système.</span><span class="sxs-lookup"><span data-stu-id="bc4f9-117">Remove the package from your system.</span></span>

    ```bash
    sudo zypper remove -y azure-cli
    ```

2. <span data-ttu-id="bc4f9-118">Si vous ne prévoyez pas de réinstaller l’interface CLI, supprimez les informations de référentiel.</span><span class="sxs-lookup"><span data-stu-id="bc4f9-118">If you don't plan to reinstall the CLI, remove the repository information.</span></span>

  ```bash
  sudo zypper removerepo azure-cli
  ```

3. <span data-ttu-id="bc4f9-119">Si vous avez supprimé les informations de référentiel, supprimez également la clé de signature Microsoft GPG.</span><span class="sxs-lookup"><span data-stu-id="bc4f9-119">If you removed the repository information, also remove the Microsoft GPG signature key.</span></span>

  ```bash
  MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
  sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
  ```