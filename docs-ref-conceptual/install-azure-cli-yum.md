---
title: Installer Azure CLI 2.0 avec yum
description: "Installation d’Azure CLI 2.0 avec yum"
keywords: "Azure CLI, installation d’Azure CLI, Azure yum, Azure RHEL, Azure Fedora, Azure CentOS"
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
ms.openlocfilehash: f0d5effcd8315094b30050a35119e41eddf89961
ms.sourcegitcommit: 3eef136ae752eb90c67af604d4ddd298d70b1c9d
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/06/2018
---
# <a name="install-azure-cli-20-with-yum"></a><span data-ttu-id="6ae78-104">Installer Azure CLI 2.0 avec yum</span><span class="sxs-lookup"><span data-stu-id="6ae78-104">Install Azure CLI 2.0 with yum</span></span>

<span data-ttu-id="6ae78-105">Si vous exécutez une distribution qui est fournie avec `yum`, telle que RHEL, Fedora, ou CentOS, vous pouvez installer un package pour l’interface de ligne de commande Azure sur votre système.</span><span class="sxs-lookup"><span data-stu-id="6ae78-105">If you are running a distirbution that comes with `yum`, such as RHEL, Fedora, or CentOS, there is an available package for the Azure CLI that you can install on your system.</span></span>

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a><span data-ttu-id="6ae78-106">Installer</span><span class="sxs-lookup"><span data-stu-id="6ae78-106">Install</span></span>

1. <span data-ttu-id="6ae78-107">Importer la clé de référentiel Microsoft :</span><span class="sxs-lookup"><span data-stu-id="6ae78-107">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. <span data-ttu-id="6ae78-108">Créer des informations de référentiel `azure-cli` locales :</span><span class="sxs-lookup"><span data-stu-id="6ae78-108">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/azure-cli.repo'
   ```

3. <span data-ttu-id="6ae78-109">Mettre à jour l’index de package `yum` et l’installer :</span><span class="sxs-lookup"><span data-stu-id="6ae78-109">Update the `yum` package index and install:</span></span>

   ```bash
   yum check-update
   sudo yum install azure-cli
   ```

<span data-ttu-id="6ae78-110">Exécutez Azure CLI avec la commande `az`.</span><span class="sxs-lookup"><span data-stu-id="6ae78-110">Run the Azure CLI with the `az` command.</span></span>

## <a name="update"></a><span data-ttu-id="6ae78-111">Mettre à jour</span><span class="sxs-lookup"><span data-stu-id="6ae78-111">Update</span></span>

<span data-ttu-id="6ae78-112">Mettre à jour Azure CLI avec la commande `yum update`.</span><span class="sxs-lookup"><span data-stu-id="6ae78-112">Update the Azure CLI with the `yum update` command.</span></span>

```bash
yum check-update
sudo yum update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="6ae78-113">Désinstaller l’interface</span><span class="sxs-lookup"><span data-stu-id="6ae78-113">Uninstall</span></span>

<span data-ttu-id="6ae78-114">Si jamais vous décidez de désinstaller l’interface de ligne de commande Azure, nous sommes désolés de vous voir partir.</span><span class="sxs-lookup"><span data-stu-id="6ae78-114">If you ever decide to uninstall the Azure CLI, we're sorry to see you go.</span></span> <span data-ttu-id="6ae78-115">Avant de désinstaller, utilisez la commande `az feedback`, afin de nous donner quelques raisons pour lesquelles vous avez choisi de désinstaller et nous aider à améliorer l’expérience CLI.</span><span class="sxs-lookup"><span data-stu-id="6ae78-115">Before you uninstall, use the `az feedback` command to give us some reasons why you chose to uninstall and how we could improve the CLI experience.</span></span> <span data-ttu-id="6ae78-116">Nous souhaitons nous assurer que l’interface de ligne de commande Azure est aussi conviviale et exempte de bogues que possible.</span><span class="sxs-lookup"><span data-stu-id="6ae78-116">We want to make sure that the Azure CLI is as bug-free and user-friendly as we can make it.</span></span> <span data-ttu-id="6ae78-117">Vous pouvez également [signaler un problème lié à GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="6ae78-117">You can also [file a github issue](https://github.com/Azure/azure-cli/issues).</span></span>

1. <span data-ttu-id="6ae78-118">Supprimez le package de votre système.</span><span class="sxs-lookup"><span data-stu-id="6ae78-118">Remove the package from your system.</span></span>

   ```bash
   sudo yum remove azure-cli
   ```

2. <span data-ttu-id="6ae78-119">Si vous ne souhaitez pas réinstaller l’interface CLI, supprimez les informations de référentiel.</span><span class="sxs-lookup"><span data-stu-id="6ae78-119">If you do not plan to reinstall the CLI, remove the repository information.</span></span>

   ```bash
   sudo rm /etc/yum.repos.d/azure-cli.repo
   ```

3. <span data-ttu-id="6ae78-120">Si vous avez supprimé les informations de référentiel, supprimez également la clé de signature Microsoft GPG.</span><span class="sxs-lookup"><span data-stu-id="6ae78-120">If you removed the repository information, also remove the Microsoft GPG signature key.</span></span>

  ```bash
  MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
  sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
  ```
