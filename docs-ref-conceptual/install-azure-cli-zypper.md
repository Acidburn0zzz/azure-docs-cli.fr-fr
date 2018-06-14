---
title: Installation d’Azure CLI 2.0 pour Linux avec zypper
description: Installation d’Azure CLI 2.0 avec zypper
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 01/29/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: a862cca17adb1bfa0201af250819158081c29813
ms.sourcegitcommit: 5c80e96e96f9608c92a94fa4a9c4afb25099f3fc
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/13/2018
ms.locfileid: "35512969"
---
# <a name="install-azure-cli-20-with-zypper"></a><span data-ttu-id="0618d-103">Installer Azure CLI 2.0 avec zypper</span><span class="sxs-lookup"><span data-stu-id="0618d-103">Install Azure CLI 2.0 with zypper</span></span>

<span data-ttu-id="0618d-104">Si vous exécutez une distribution qui est fournie avec `zypper`, telle que openSUSE ou SLES, un package est disponible pour l’interface de ligne de commande Azure.</span><span class="sxs-lookup"><span data-stu-id="0618d-104">If you are running a distribution that comes with `zypper`, such as openSUSE or SLES, there is a package available for the Azure CLI.</span></span> <span data-ttu-id="0618d-105">Ce package a été testé avec openSUSE 42.2 et SLES 12 SP 2.</span><span class="sxs-lookup"><span data-stu-id="0618d-105">This package has been tested with openSUSE 42.2 and SLES 12 SP 2.</span></span>

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a><span data-ttu-id="0618d-106">Installer</span><span class="sxs-lookup"><span data-stu-id="0618d-106">Install</span></span>

1. <span data-ttu-id="0618d-107">Installez `curl` :</span><span class="sxs-lookup"><span data-stu-id="0618d-107">Install `curl`:</span></span>

   ```bash
   sudo zypper install -y curl
   ```

2. <span data-ttu-id="0618d-108">Importer la clé de référentiel Microsoft :</span><span class="sxs-lookup"><span data-stu-id="0618d-108">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

3. <span data-ttu-id="0618d-109">Créer des informations de référentiel `azure-cli` locales :</span><span class="sxs-lookup"><span data-stu-id="0618d-109">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo zypper addrepo --name 'Azure CLI' --check https://packages.microsoft.com/yumrepos/azure-cli azure-cli
   ```

4. <span data-ttu-id="0618d-110">Mettre à jour l’index de package `zypper` et l’installer :</span><span class="sxs-lookup"><span data-stu-id="0618d-110">Update the `zypper` package index and install:</span></span>

   ```bash
   sudo zypper install --from azure-cli -y azure-cli
   ```

<span data-ttu-id="0618d-111">Vous pouvez ensuite exécuter l’interface de ligne de commande Azure avec la commande `az`.</span><span class="sxs-lookup"><span data-stu-id="0618d-111">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="0618d-112">Pour vous connecter, exécutez la commande `az login`.</span><span class="sxs-lookup"><span data-stu-id="0618d-112">To log in, run the `az login` command.</span></span>

```azurecli
az login
```

<span data-ttu-id="0618d-113">Pour en savoir plus sur les différentes méthodes de connexion, consultez [Se connecter avec Azure CLI 2.0](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="0618d-113">To learn more about different login methods, see [Log in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

## <a name="update"></a><span data-ttu-id="0618d-114">Mettre à jour</span><span class="sxs-lookup"><span data-stu-id="0618d-114">Update</span></span>

<span data-ttu-id="0618d-115">Vous pouvez mettre à jour le package avec la commande `zypper update`.</span><span class="sxs-lookup"><span data-stu-id="0618d-115">You can update the package with the `zypper update` command.</span></span>

```bash
sudo zypper refresh
sudo zypper update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="0618d-116">Désinstaller l’interface</span><span class="sxs-lookup"><span data-stu-id="0618d-116">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="0618d-117">Supprimez le package de votre système.</span><span class="sxs-lookup"><span data-stu-id="0618d-117">Remove the package from your system.</span></span>

    ```bash
    sudo zypper remove -y azure-cli
    ```

2. <span data-ttu-id="0618d-118">Si vous ne souhaitez pas réinstaller l’interface CLI, supprimez les informations de référentiel.</span><span class="sxs-lookup"><span data-stu-id="0618d-118">If you do not plan to reinstall the CLI, remove the repository information.</span></span>

  ```bash
  sudo zypper removerepo azure-cli
  ```

3. <span data-ttu-id="0618d-119">Si vous avez supprimé les informations de référentiel, supprimez également la clé de signature Microsoft GPG.</span><span class="sxs-lookup"><span data-stu-id="0618d-119">If you removed the repository information, also remove the Microsoft GPG signature key.</span></span>

  ```bash
  MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
  sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
  ```

