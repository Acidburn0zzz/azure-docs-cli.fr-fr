---
title: Installation d’Azure CLI 2.0 pour Linux avec zypper
description: Installation d’Azure CLI 2.0 avec zypper
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 01/29/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 01d293eff229ab8b0eb3a3ff4e23978ea9e00174
ms.sourcegitcommit: 0e9aafa07311526f43661c8bd3a7eba7cbc2caed
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/20/2018
---
# <a name="install-azure-cli-20-with-zypper"></a><span data-ttu-id="f7cad-103">Installer Azure CLI 2.0 avec zypper</span><span class="sxs-lookup"><span data-stu-id="f7cad-103">Install Azure CLI 2.0 with zypper</span></span>

<span data-ttu-id="f7cad-104">Si vous exécutez une distribution qui est fournie avec `zypper`, telle que openSUSE ou SLES, un package est disponible pour l’interface de ligne de commande Azure.</span><span class="sxs-lookup"><span data-stu-id="f7cad-104">If you are running a distribution that comes with `zypper`, such as openSUSE or SLES, there is a package available for the Azure CLI.</span></span> <span data-ttu-id="f7cad-105">Ce package a été testé avec openSUSE 42.2 et SLES 12 SP 2.</span><span class="sxs-lookup"><span data-stu-id="f7cad-105">This package has been tested with openSUSE 42.2 and SLES 12 SP 2.</span></span>

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a><span data-ttu-id="f7cad-106">Installer</span><span class="sxs-lookup"><span data-stu-id="f7cad-106">Install</span></span>

1. <span data-ttu-id="f7cad-107">Installez `curl` :</span><span class="sxs-lookup"><span data-stu-id="f7cad-107">Install `curl`:</span></span>

   ```bash
   sudo zypper refresh
   sudo zypper install -y curl
   ```

2. <span data-ttu-id="f7cad-108">Importer la clé de référentiel Microsoft :</span><span class="sxs-lookup"><span data-stu-id="f7cad-108">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

3. <span data-ttu-id="f7cad-109">Créer des informations de référentiel `azure-cli` locales :</span><span class="sxs-lookup"><span data-stu-id="f7cad-109">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ntype=rpm-md\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/zypp/repos.d/azure-cli.repo'
   ```

4. <span data-ttu-id="f7cad-110">Mettre à jour l’index de package `zypper` et l’installer :</span><span class="sxs-lookup"><span data-stu-id="f7cad-110">Update the `zypper` package index and install:</span></span>

   ```bash
   sudo zypper refresh
   sudo zypper install -y azure-cli
   ```

<span data-ttu-id="f7cad-111">Vous pouvez ensuite exécuter l’interface de ligne de commande Azure avec la commande `az`.</span><span class="sxs-lookup"><span data-stu-id="f7cad-111">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="f7cad-112">Pour vous connecter, exécutez la commande `az login`.</span><span class="sxs-lookup"><span data-stu-id="f7cad-112">To log in, run the `az login` command.</span></span>

```azurecli
az login
```

<span data-ttu-id="f7cad-113">Pour en savoir plus sur les différentes méthodes de connexion, consultez [Se connecter avec Azure CLI 2.0](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="f7cad-113">To learn more about different login methods, see [Log in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

## <a name="update"></a><span data-ttu-id="f7cad-114">Mettre à jour</span><span class="sxs-lookup"><span data-stu-id="f7cad-114">Update</span></span>

<span data-ttu-id="f7cad-115">Vous pouvez mettre à jour le package avec la commande `zypper update`.</span><span class="sxs-lookup"><span data-stu-id="f7cad-115">You can update the package with the `zypper update` command.</span></span>

```bash
sudo zypper refresh
sudo zypper update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="f7cad-116">Désinstaller l’interface</span><span class="sxs-lookup"><span data-stu-id="f7cad-116">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="f7cad-117">Supprimez le package de votre système.</span><span class="sxs-lookup"><span data-stu-id="f7cad-117">Remove the package from your system.</span></span>

    ```bash
    sudo zypper remove -y azure-cli
    ```

2. <span data-ttu-id="f7cad-118">Si vous ne souhaitez pas réinstaller l’interface CLI, supprimez les informations de référentiel.</span><span class="sxs-lookup"><span data-stu-id="f7cad-118">If you do not plan to reinstall the CLI, remove the repository information.</span></span>

  ```bash
  sudo rm /etc/zypp/repos.d/azure-cli.repo
  ```

3. <span data-ttu-id="f7cad-119">Si vous avez supprimé les informations de référentiel, supprimez également la clé de signature Microsoft GPG.</span><span class="sxs-lookup"><span data-stu-id="f7cad-119">If you removed the repository information, also remove the Microsoft GPG signature key.</span></span>

  ```bash
  MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
  sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
  ```

