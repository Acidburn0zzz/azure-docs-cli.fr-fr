---
title: Installation d’Azure CLI pour Linux avec yum
description: Comment installer Azure CLI avec yum
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: faa1855efe9651ee104880740338c30e7dd84810
ms.sourcegitcommit: f40bd067ece4e6ec13e259782ed8db3e33b61a75
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/18/2018
ms.locfileid: "53593232"
---
# <a name="install-azure-cli-with-yum"></a><span data-ttu-id="6aa09-103">Installer Azure CLI avec yum</span><span class="sxs-lookup"><span data-stu-id="6aa09-103">Install Azure CLI with yum</span></span>

<span data-ttu-id="6aa09-104">Pour les distributions Linux avec `yum` telles que RHEL, Fedora ou CentOS, il existe un package pour Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="6aa09-104">For Linux distributions with  `yum` such as RHEL, Fedora, or CentOS, there's a package for the Azure CLI.</span></span> <span data-ttu-id="6aa09-105">Ce package a été testé avec RHEL 7, Fedora 19 et versions ultérieures et CentOS 7.</span><span class="sxs-lookup"><span data-stu-id="6aa09-105">This package has been tested with RHEL 7, Fedora 19 and higher, and CentOS 7.</span></span>

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a><span data-ttu-id="6aa09-106">Installer</span><span class="sxs-lookup"><span data-stu-id="6aa09-106">Install</span></span>

1. <span data-ttu-id="6aa09-107">Importez la clé de référentiel Microsoft.</span><span class="sxs-lookup"><span data-stu-id="6aa09-107">Import the Microsoft repository key.</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. <span data-ttu-id="6aa09-108">Créez des informations de référentiel `azure-cli` locales.</span><span class="sxs-lookup"><span data-stu-id="6aa09-108">Create local `azure-cli` repository information.</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/azure-cli.repo'
   ```

3. <span data-ttu-id="6aa09-109">Installez avec la commande `yum install`.</span><span class="sxs-lookup"><span data-stu-id="6aa09-109">Install with the `yum install` command.</span></span>

   ```bash
   sudo yum install azure-cli
   ```

<span data-ttu-id="6aa09-110">Vous pouvez ensuite exécuter l’interface de ligne de commande Azure avec la commande `az`.</span><span class="sxs-lookup"><span data-stu-id="6aa09-110">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="6aa09-111">Pour vous connecter, utilisez la commande [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="6aa09-111">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="6aa09-112">Pour en savoir plus sur les différentes méthodes d’authentification, consultez [Se connecter avec Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="6aa09-112">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="6aa09-113">Résolution de problèmes</span><span class="sxs-lookup"><span data-stu-id="6aa09-113">Troubleshooting</span></span>

<span data-ttu-id="6aa09-114">Voici certains problèmes courants lors de l’installation avec `yum`.</span><span class="sxs-lookup"><span data-stu-id="6aa09-114">Here are some common problems seen when installing with `yum`.</span></span> <span data-ttu-id="6aa09-115">Si vous rencontrez un problème n’étant pas évoqué ici, [signalez un problème sur github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="6aa09-115">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="update"></a><span data-ttu-id="6aa09-116">Mettre à jour</span><span class="sxs-lookup"><span data-stu-id="6aa09-116">Update</span></span>

<span data-ttu-id="6aa09-117">Mettre à jour Azure CLI avec la commande `yum update`.</span><span class="sxs-lookup"><span data-stu-id="6aa09-117">Update the Azure CLI with the `yum update` command.</span></span>

```bash
sudo yum update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="6aa09-118">Désinstaller l’interface</span><span class="sxs-lookup"><span data-stu-id="6aa09-118">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="6aa09-119">Supprimez le package de votre système.</span><span class="sxs-lookup"><span data-stu-id="6aa09-119">Remove the package from your system.</span></span>

   ```bash
   sudo yum remove azure-cli
   ```

2. <span data-ttu-id="6aa09-120">Si vous ne prévoyez pas de réinstaller l’interface CLI, supprimez les informations de référentiel.</span><span class="sxs-lookup"><span data-stu-id="6aa09-120">If you don't plan to reinstall the CLI, remove the repository information.</span></span>

   ```bash
   sudo rm /etc/yum.repos.d/azure-cli.repo
   ```

3. <span data-ttu-id="6aa09-121">Si vous avez supprimé les informations de référentiel, supprimez également la clé de signature Microsoft GPG.</span><span class="sxs-lookup"><span data-stu-id="6aa09-121">If you removed the repository information, also remove the Microsoft GPG signature key.</span></span>

   ```bash
   MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
   sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
   ```

## <a name="next-steps"></a><span data-ttu-id="6aa09-122">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="6aa09-122">Next Steps</span></span>

<span data-ttu-id="6aa09-123">Maintenant que vous avez installé l’interface CLI, découvrez ses fonctionnalités et ses commandes courantes.</span><span class="sxs-lookup"><span data-stu-id="6aa09-123">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="6aa09-124">Prise en main de l’interface Azure CLI</span><span class="sxs-lookup"><span data-stu-id="6aa09-124">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
