---
title: Installez Azure CLI sur Linux avec zypper
description: Comment installer Azure CLI avec zypper
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 09/09/2018
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: d07fe2e807bd6e1fac6d0e9f883bcc8092be46bb
ms.sourcegitcommit: 21bc2a7125b6c38bf1c4def0a0e66e6673de4805
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/10/2020
ms.locfileid: "79037969"
---
# <a name="install-azure-cli-with-zypper"></a><span data-ttu-id="ab089-103">Installez Azure CLI avec zypper</span><span class="sxs-lookup"><span data-stu-id="ab089-103">Install Azure CLI with zypper</span></span>

<span data-ttu-id="ab089-104">Pour les distributions Linux avec `zypper`, telles que openSUSE ou SLES, un package est disponible pour l’Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="ab089-104">For Linux distributions with `zypper`, such as openSUSE or SLES, there's a package available for the Azure CLI.</span></span> <span data-ttu-id="ab089-105">Ce package a été testé avec openSUSE Leap 15.1 and SLES 15.</span><span class="sxs-lookup"><span data-stu-id="ab089-105">This package has been tested with openSUSE Leap 15.1, and SLES 15.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

[!INCLUDE [rpm-warning](includes/rpm-warning.md)]

## <a name="install"></a><span data-ttu-id="ab089-106">Installer</span><span class="sxs-lookup"><span data-stu-id="ab089-106">Install</span></span>

1. <span data-ttu-id="ab089-107">Installez `curl` :</span><span class="sxs-lookup"><span data-stu-id="ab089-107">Install `curl`:</span></span>

   ```bash
   sudo zypper install -y curl
   ```

2. <span data-ttu-id="ab089-108">Importer la clé de référentiel Microsoft :</span><span class="sxs-lookup"><span data-stu-id="ab089-108">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

3. <span data-ttu-id="ab089-109">Créer des informations de référentiel `azure-cli` locales :</span><span class="sxs-lookup"><span data-stu-id="ab089-109">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo zypper addrepo --name 'Azure CLI' --check https://packages.microsoft.com/yumrepos/azure-cli azure-cli
   ```

4. <span data-ttu-id="ab089-110">Mettre à jour l’index de package `zypper` et l’installer :</span><span class="sxs-lookup"><span data-stu-id="ab089-110">Update the `zypper` package index and install:</span></span>

   ```bash
   sudo zypper install --from azure-cli azure-cli
   ```
   <span data-ttu-id="ab089-111">Entrez 2 pour continuer l’installation en ignorant certaines de ses dépendances.</span><span class="sxs-lookup"><span data-stu-id="ab089-111">Input 2 to continue install by ignoring some of its dependencies.</span></span>

<span data-ttu-id="ab089-112">Vous pouvez ensuite exécuter l’interface de ligne de commande Azure avec la commande `az`.</span><span class="sxs-lookup"><span data-stu-id="ab089-112">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="ab089-113">Pour vous connecter, utilisez la commande [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="ab089-113">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="ab089-114">Pour en savoir plus sur les différentes méthodes d’authentification, consultez [Se connecter avec Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="ab089-114">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="ab089-115">Dépannage</span><span class="sxs-lookup"><span data-stu-id="ab089-115">Troubleshooting</span></span>

<span data-ttu-id="ab089-116">Voici certains problèmes courants lors de l’installation avec `zypper`.</span><span class="sxs-lookup"><span data-stu-id="ab089-116">Here are some common problems seen when installing with `zypper`.</span></span> <span data-ttu-id="ab089-117">Si vous rencontrez un problème n’étant pas évoqué ici, [signalez un problème sur github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="ab089-117">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="install-on-sles-12-or-other-systems-without-python-36"></a><span data-ttu-id="ab089-118">Installer sur SLES 12 ou d’autres systèmes sans Python 3.6</span><span class="sxs-lookup"><span data-stu-id="ab089-118">Install on SLES 12 or other systems without Python 3.6</span></span>

<span data-ttu-id="ab089-119">Sur SLES 12, le package python3 par défaut est la version 3.4 et n’est pas pris en charge par Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="ab089-119">On SLES 12, the defualt python3 package is 3.4 and not supported by Azure CLI.</span></span> <span data-ttu-id="ab089-120">Vous pouvez d’abord générer une version de python3 plus récente à partir de la source.</span><span class="sxs-lookup"><span data-stu-id="ab089-120">You can first build a higher version python3 from source.</span></span> <span data-ttu-id="ab089-121">Vous pouvez alors télécharger le package Azure CLI et l’installer sans dépendance.</span><span class="sxs-lookup"><span data-stu-id="ab089-121">Then you can download the Azure CLI package and install it without dependency.</span></span>
```bash
$ sudo zypper install -y gcc gcc-c++ make ncurses patch wget tar zlib-devel zlib openssl-devel
# Download Python source code
$ PYTHON_VERSION="3.6.9"
$ PYTHON_SRC_DIR=$(mktemp -d)
$ wget -qO- https://www.python.org/ftp/python/$PYTHON_VERSION/Python-$PYTHON_VERSION.tgz | tar -xz -C "$PYTHON_SRC_DIR"
# Build Python
$ $PYTHON_SRC_DIR/*/configure
$ make
$ sudo make install
#Download azure-cli package 
$ AZ_VERSION=$(zypper --no-refresh info azure-cli |grep Version | awk -F': ' '{print $2}' | awk '{$1=$1;print}')
$ wget https://packages.microsoft.com/yumrepos/azure-cli/azure-cli-$AZ_VERSION.x86_64.rpm
#Install without dependency
$ sudo rpm -ivh --nodeps azure-cli-$AZ_VERSION.x86_64.rpm
```

### <a name="proxy-blocks-connection"></a><span data-ttu-id="ab089-122">Le proxy bloque la connexion</span><span class="sxs-lookup"><span data-stu-id="ab089-122">Proxy blocks connection</span></span>

[!INCLUDE[configure-proxy](includes/configure-proxy.md)]

<span data-ttu-id="ab089-123">Vous pouvez également configurer de manière explicite `zypper` (via `yast2`) pour utiliser ce proxy à tout moment.</span><span class="sxs-lookup"><span data-stu-id="ab089-123">You may also want to explicitly configure `zypper` (via `yast2`) to use this proxy at all times.</span></span> <span data-ttu-id="ab089-124">Pour ce faire, exécutez la commande `yast2 proxy` en tant que superutilisateur et remplissez les informations présentées dans le formulaire.</span><span class="sxs-lookup"><span data-stu-id="ab089-124">To do so, run the `yast2 proxy` command as superuser, and fill in the information presented in the form.</span></span> <span data-ttu-id="ab089-125">Si vous avez un gestionnaire de fenêtres disponible sur votre système, vous pouvez également utiliser le volet `Network Services > Proxy` dans le `YaST Control Center`.</span><span class="sxs-lookup"><span data-stu-id="ab089-125">If you have a window manager available on your system, you can also use the `Network Services > Proxy` pane in the `YaST Control Center`.</span></span>

<span data-ttu-id="ab089-126">Pour la configuration avancée ou plus d’informations, consultez la [documentation de configuration de proxy OpenSUSE](https://www.suse.com/documentation/slms1/book_slms/data/sec_wy_config_updates_proxy.html)</span><span class="sxs-lookup"><span data-stu-id="ab089-126">For advanced configuration or more information, see the [OpenSUSE Proxy configuration documentation](https://www.suse.com/documentation/slms1/book_slms/data/sec_wy_config_updates_proxy.html)</span></span>

<span data-ttu-id="ab089-127">Pour obtenir la clé de signature Microsoft et obtenir le package à partir de notre dépôt, votre proxy doit autoriser les connexions HTTPS aux adresses suivantes :</span><span class="sxs-lookup"><span data-stu-id="ab089-127">In order to get the Microsoft signing key and get the package from our repository, your proxy needs to allow HTTPS connections to the following addresses:</span></span>

* `https://packages.microsoft.com`
* `https://download.opensuse.org`

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="update"></a><span data-ttu-id="ab089-128">Update</span><span class="sxs-lookup"><span data-stu-id="ab089-128">Update</span></span>

<span data-ttu-id="ab089-129">Vous pouvez mettre à jour le package avec la commande `zypper update`.</span><span class="sxs-lookup"><span data-stu-id="ab089-129">You can update the package with the `zypper update` command.</span></span>

```bash
sudo zypper refresh
sudo zypper update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="ab089-130">Désinstaller l’interface</span><span class="sxs-lookup"><span data-stu-id="ab089-130">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="ab089-131">Supprimez le package de votre système.</span><span class="sxs-lookup"><span data-stu-id="ab089-131">Remove the package from your system.</span></span>

    ```bash
    sudo zypper remove -y azure-cli
    ```

2. <span data-ttu-id="ab089-132">Si vous ne prévoyez pas de réinstaller l’interface CLI, supprimez les informations de référentiel.</span><span class="sxs-lookup"><span data-stu-id="ab089-132">If you don't plan to reinstall the CLI, remove the repository information.</span></span>

   ```bash
   sudo zypper removerepo azure-cli
   ```

3. <span data-ttu-id="ab089-133">Si vous n’utilisez pas d’autres packages Microsoft, supprimez la clé de signature Microsoft.</span><span class="sxs-lookup"><span data-stu-id="ab089-133">If you don't use other Microsoft packages, remove the Microsoft signing key.</span></span>

   ```bash
   MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
   sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
   ```

## <a name="next-steps"></a><span data-ttu-id="ab089-134">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="ab089-134">Next Steps</span></span>

<span data-ttu-id="ab089-135">Maintenant que vous avez installé l’interface CLI, découvrez ses fonctionnalités et ses commandes courantes.</span><span class="sxs-lookup"><span data-stu-id="ab089-135">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="ab089-136">Prise en main de l’interface Azure CLI</span><span class="sxs-lookup"><span data-stu-id="ab089-136">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
