---
title: "Installation d’Azure CLI 2.0 pour Linux avec yum"
description: "Installation d’Azure CLI 2.0 avec yum"
keywords: "Azure CLI, installation d’Azure CLI, Azure yum, Azure RHEL, Azure Fedora, Azure CentOS"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 01/29/18
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 9d11c3cf5d9e7ba58c3e2edd830e0d12669f5b91
ms.sourcegitcommit: 8606f36963e8daa6448d637393d1e4ef2c9859a0
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/01/2018
---
# <a name="install-azure-cli-20-with-yum"></a><span data-ttu-id="e25af-104">Installer Azure CLI 2.0 avec yum</span><span class="sxs-lookup"><span data-stu-id="e25af-104">Install Azure CLI 2.0 with yum</span></span>

<span data-ttu-id="e25af-105">Si vous exécutez une distribution qui est fournie avec `yum`, telle que RHEL, Fedora, ou CentOS, un package est disponible pour l’interface de ligne de commande Azure.</span><span class="sxs-lookup"><span data-stu-id="e25af-105">If you are running a distribution that comes with `yum`, such as RHEL, Fedora, or CentOS, there is a package available for the Azure CLI.</span></span> <span data-ttu-id="e25af-106">Ce package a été testé avec RHEL 7, Fedora 19 et versions ultérieures et CentOS 7.</span><span class="sxs-lookup"><span data-stu-id="e25af-106">This package has been tested with RHEL 7, Fedora 19 and higher, and CentOS 7.</span></span>

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a><span data-ttu-id="e25af-107">Installer</span><span class="sxs-lookup"><span data-stu-id="e25af-107">Install</span></span>

1. <span data-ttu-id="e25af-108">Importer la clé de référentiel Microsoft :</span><span class="sxs-lookup"><span data-stu-id="e25af-108">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. <span data-ttu-id="e25af-109">Créer des informations de référentiel `azure-cli` locales :</span><span class="sxs-lookup"><span data-stu-id="e25af-109">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/azure-cli.repo'
   ```

3. <span data-ttu-id="e25af-110">Mettre à jour l’index de package `yum` et l’installer :</span><span class="sxs-lookup"><span data-stu-id="e25af-110">Update the `yum` package index and install:</span></span>

   ```bash
   yum check-update
   sudo yum install azure-cli
   ```

<span data-ttu-id="e25af-111">Exécutez Azure CLI avec la commande `az`.</span><span class="sxs-lookup"><span data-stu-id="e25af-111">Run the Azure CLI with the `az` command.</span></span>

## <a name="update"></a><span data-ttu-id="e25af-112">Mettre à jour</span><span class="sxs-lookup"><span data-stu-id="e25af-112">Update</span></span>

<span data-ttu-id="e25af-113">Mettre à jour Azure CLI avec la commande `yum update`.</span><span class="sxs-lookup"><span data-stu-id="e25af-113">Update the Azure CLI with the `yum update` command.</span></span>

```bash
yum check-update
sudo yum update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="e25af-114">Désinstaller l’interface</span><span class="sxs-lookup"><span data-stu-id="e25af-114">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="e25af-115">Supprimez le package de votre système.</span><span class="sxs-lookup"><span data-stu-id="e25af-115">Remove the package from your system.</span></span>

   ```bash
   sudo yum remove azure-cli
   ```

2. <span data-ttu-id="e25af-116">Si vous ne souhaitez pas réinstaller l’interface CLI, supprimez les informations de référentiel.</span><span class="sxs-lookup"><span data-stu-id="e25af-116">If you do not plan to reinstall the CLI, remove the repository information.</span></span>

   ```bash
   sudo rm /etc/yum.repos.d/azure-cli.repo
   ```

3. <span data-ttu-id="e25af-117">Si vous avez supprimé les informations de référentiel, supprimez également la clé de signature Microsoft GPG.</span><span class="sxs-lookup"><span data-stu-id="e25af-117">If you removed the repository information, also remove the Microsoft GPG signature key.</span></span>

  ```bash
  MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
  sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
  ```
