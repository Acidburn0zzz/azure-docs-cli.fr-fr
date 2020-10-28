---
title: Installez Azure CLI sur Linux avec zypper
description: Comment installer Azure CLI avec zypper
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 09/25/2020
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: e501d05985b0483442ab11f78343d773fd7e55bf
ms.sourcegitcommit: 1187fb75b68426c46e84b3f294c509ee7b7da9be
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/27/2020
ms.locfileid: "92687083"
---
# <a name="install-azure-cli-with-zypper"></a><span data-ttu-id="8c0a1-103">Installez Azure CLI avec zypper</span><span class="sxs-lookup"><span data-stu-id="8c0a1-103">Install Azure CLI with zypper</span></span>

<span data-ttu-id="8c0a1-104">Pour les distributions Linux avec `zypper`, telles que openSUSE ou SLES, un package est disponible pour l’Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="8c0a1-104">For Linux distributions with `zypper`, such as openSUSE or SLES, there's a package available for the Azure CLI.</span></span> <span data-ttu-id="8c0a1-105">Ce package a été testé avec openSUSE Leap 15.1 and SLES 15.</span><span class="sxs-lookup"><span data-stu-id="8c0a1-105">This package has been tested with openSUSE Leap 15.1, and SLES 15.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

[!INCLUDE [rpm-warning](includes/rpm-warning.md)]

## <a name="install"></a><span data-ttu-id="8c0a1-106">Installer</span><span class="sxs-lookup"><span data-stu-id="8c0a1-106">Install</span></span>

1. <span data-ttu-id="8c0a1-107">Installez `curl` :</span><span class="sxs-lookup"><span data-stu-id="8c0a1-107">Install `curl`:</span></span>

   ```bash
   sudo zypper install -y curl
   ```

2. <span data-ttu-id="8c0a1-108">Importer la clé de référentiel Microsoft :</span><span class="sxs-lookup"><span data-stu-id="8c0a1-108">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

3. <span data-ttu-id="8c0a1-109">Créer des informations de référentiel `azure-cli` locales :</span><span class="sxs-lookup"><span data-stu-id="8c0a1-109">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo zypper addrepo --name 'Azure CLI' --check https://packages.microsoft.com/yumrepos/azure-cli azure-cli
   ```

4. <span data-ttu-id="8c0a1-110">Mettre à jour l’index de package `zypper` et l’installer :</span><span class="sxs-lookup"><span data-stu-id="8c0a1-110">Update the `zypper` package index and install:</span></span>

   ```bash
   sudo zypper install --from azure-cli azure-cli
   ```
   <span data-ttu-id="8c0a1-111">Entrez 2 pour continuer l’installation en ignorant certaines de ses dépendances.</span><span class="sxs-lookup"><span data-stu-id="8c0a1-111">Input 2 to continue install by ignoring some of its dependencies.</span></span>

<span data-ttu-id="8c0a1-112">Vous pouvez ensuite exécuter l’interface de ligne de commande Azure avec la commande `az`.</span><span class="sxs-lookup"><span data-stu-id="8c0a1-112">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="8c0a1-113">Pour vous connecter, utilisez la commande [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="8c0a1-113">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="8c0a1-114">Pour en savoir plus sur les différentes méthodes d’authentification, consultez [Se connecter avec Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="8c0a1-114">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="8c0a1-115">Dépannage</span><span class="sxs-lookup"><span data-stu-id="8c0a1-115">Troubleshooting</span></span>

<span data-ttu-id="8c0a1-116">Voici certains problèmes courants lors de l’installation avec `zypper`.</span><span class="sxs-lookup"><span data-stu-id="8c0a1-116">Here are some common problems seen when installing with `zypper`.</span></span> <span data-ttu-id="8c0a1-117">Si vous rencontrez un problème n’étant pas évoqué ici, [signalez un problème sur github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="8c0a1-117">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="notimplementederror-on-opensuse-15-vm"></a><span data-ttu-id="8c0a1-118">NotImplementedError sur une machine virtuelle OpenSUSE 15</span><span class="sxs-lookup"><span data-stu-id="8c0a1-118">NotImplementedError on OpenSUSE 15 VM</span></span>
<span data-ttu-id="8c0a1-119">La version `2.0.45` d’Azure CLI est préinstallée sur la machine virtuelle OpenSUSE 15. Cette version est obsolète et présente des problèmes avec `az login`.</span><span class="sxs-lookup"><span data-stu-id="8c0a1-119">The OpenSUSE 15 VM has a pre-installed Azure CLI with version `2.0.45`, it's outdated and has issues with `az login`.</span></span> <span data-ttu-id="8c0a1-120">Supprimez-la ainsi que ses dépendances avant de suivre les [instructions d’installation](#install) pour ajouter la dernière version d’Azure CLI :</span><span class="sxs-lookup"><span data-stu-id="8c0a1-120">Please remove it along with its dependencies before following the [Install](#install) instruction to add the latest Azure CLI:</span></span>
```bash
sudo zypper rm -y --clean-deps azure-cli
```

<span data-ttu-id="8c0a1-121">Si vous avez mis à jour Azure CLI sans supprimer les dépendances de la version `2.0.45`, ses anciennes dépendances peuvent affecter la version la plus récente d’Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="8c0a1-121">If you updated Azure CLI without removing the dependencies of version `2.0.45`, its old dependencies may affect the latest version of Azure CLI.</span></span> <span data-ttu-id="8c0a1-122">Vous devez rajouter l’ancienne version pour établir un lien avec ses dépendances, puis supprimer `azure-cli` ainsi que ses dépendances :</span><span class="sxs-lookup"><span data-stu-id="8c0a1-122">You need to add back the old version to link to its dependencies and then remove `azure-cli` along with its dependencies:</span></span>
```bash
# The package name may vary on different system version, run 'zypper --no-refresh info azure-cli' to check the source package format
sudo zypper install --oldpackage azure-cli-2.0.45-4.22.noarch

sudo zypper rm -y --clean-deps azure-cli
```


### <a name="install-on-sles-12-or-other-systems-without-python-36"></a><span data-ttu-id="8c0a1-123">Installer sur SLES 12 ou d’autres systèmes sans Python 3.6</span><span class="sxs-lookup"><span data-stu-id="8c0a1-123">Install on SLES 12 or other systems without Python 3.6</span></span>

<span data-ttu-id="8c0a1-124">Sur SLES 12, le package `python3` par défaut est `3.4`, qui n’est pas pris en charge par Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="8c0a1-124">On SLES 12, the default `python3` package is `3.4` and not supported by Azure CLI.</span></span> <span data-ttu-id="8c0a1-125">Vous pouvez d’abord suivre les étapes 1 à 3 des [instructions d’installation](#install) pour ajouter le dépôt `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="8c0a1-125">You can first follow step 1-3 of the [install instruction](#install) to add the `azure-cli` repository.</span></span> <span data-ttu-id="8c0a1-126">Ensuite, générez une version plus récente de `python3` à partir de la source.</span><span class="sxs-lookup"><span data-stu-id="8c0a1-126">Then build a higher version `python3` from source.</span></span> <span data-ttu-id="8c0a1-127">Enfin, vous pouvez télécharger le package Azure CLI et l’installer sans dépendance.</span><span class="sxs-lookup"><span data-stu-id="8c0a1-127">Finally, you can download the Azure CLI package and install it without dependency.</span></span>

<span data-ttu-id="8c0a1-128">Vous pouvez utiliser la commande suivante pour installer Azure CLI (notez que votre version de Python 3 sera remplacée par Python 3.6) :</span><span class="sxs-lookup"><span data-stu-id="8c0a1-128">You can use the following one command to install Azure CLI (be aware that your existing Python 3 version will be overridden by Python 3.6):</span></span>
```bash
curl -sL https://azurecliprod.blob.core.windows.net/sles12_install.sh | sudo bash
```

<span data-ttu-id="8c0a1-129">Vous pouvez également le faire étape par étape :</span><span class="sxs-lookup"><span data-stu-id="8c0a1-129">Or you can do it step by step:</span></span>

```bash
# !Please add azure-cli repository first following step 1-3 of the install instruction before running below commands
$ sudo zypper refresh
$ sudo zypper install -y gcc gcc-c++ make ncurses patch wget tar zlib-devel zlib openssl-devel
# Download Python source code
$ PYTHON_VERSION="3.6.9"
$ PYTHON_SRC_DIR=$(mktemp -d)
$ wget -qO- https://www.python.org/ftp/python/$PYTHON_VERSION/Python-$PYTHON_VERSION.tgz | tar -xz -C "$PYTHON_SRC_DIR"
# Build Python
# Please be aware that with --prefix=/usr, the command will override the existing Python 3 version
$ $PYTHON_SRC_DIR/*/configure --prefix=/usr
$ make
$ sudo make install
# Download azure-cli package 
$ AZ_VERSION=$(zypper --no-refresh info azure-cli |grep Version | awk -F': ' '{print $2}' | awk '{$1=$1;print}')
$ wget https://packages.microsoft.com/yumrepos/azure-cli/azure-cli-$AZ_VERSION.x86_64.rpm
# Install without dependency
$ sudo rpm -ivh --nodeps azure-cli-$AZ_VERSION.x86_64.rpm
```

### <a name="proxy-blocks-connection"></a><span data-ttu-id="8c0a1-130">Le proxy bloque la connexion</span><span class="sxs-lookup"><span data-stu-id="8c0a1-130">Proxy blocks connection</span></span>

[!INCLUDE[configure-proxy](includes/configure-proxy.md)]

<span data-ttu-id="8c0a1-131">Vous pouvez également configurer de manière explicite `zypper` (via `yast2`) pour utiliser ce proxy à tout moment.</span><span class="sxs-lookup"><span data-stu-id="8c0a1-131">You may also want to explicitly configure `zypper` (via `yast2`) to use this proxy at all times.</span></span> <span data-ttu-id="8c0a1-132">Pour ce faire, exécutez la commande `yast2 proxy` en tant que superutilisateur et remplissez les informations présentées dans le formulaire.</span><span class="sxs-lookup"><span data-stu-id="8c0a1-132">To do so, run the `yast2 proxy` command as superuser, and fill in the information presented in the form.</span></span> <span data-ttu-id="8c0a1-133">Si vous avez un gestionnaire de fenêtres disponible sur votre système, vous pouvez également utiliser le volet `Network Services > Proxy` dans le `YaST Control Center`.</span><span class="sxs-lookup"><span data-stu-id="8c0a1-133">If you have a window manager available on your system, you can also use the `Network Services > Proxy` pane in the `YaST Control Center`.</span></span>

<span data-ttu-id="8c0a1-134">Pour la configuration avancée ou plus d’informations, consultez la [documentation de configuration de proxy OpenSUSE](https://www.suse.com/documentation/slms1/book_slms/data/sec_wy_config_updates_proxy.html)</span><span class="sxs-lookup"><span data-stu-id="8c0a1-134">For advanced configuration or more information, see the [OpenSUSE Proxy configuration documentation](https://www.suse.com/documentation/slms1/book_slms/data/sec_wy_config_updates_proxy.html)</span></span>

<span data-ttu-id="8c0a1-135">Pour obtenir la clé de signature Microsoft et obtenir le package à partir de notre dépôt, votre proxy doit autoriser les connexions HTTPS aux adresses suivantes :</span><span class="sxs-lookup"><span data-stu-id="8c0a1-135">In order to get the Microsoft signing key and get the package from our repository, your proxy needs to allow HTTPS connections to the following addresses:</span></span>

* `https://packages.microsoft.com`
* `https://download.opensuse.org`

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

### <a name="ssl-certificate-problem"></a><span data-ttu-id="8c0a1-136">Problème de certificat SSL</span><span class="sxs-lookup"><span data-stu-id="8c0a1-136">SSL certificate problem</span></span>

<span data-ttu-id="8c0a1-137">Lorsqu’un certificat est arrêté ou obsolète sur un ordinateur, vous pouvez recevoir une erreur indiquant que curl n’a pas réussi à vérifier la légitimité du serveur et n’a donc pas pu établir de connexion sécurisée.</span><span class="sxs-lookup"><span data-stu-id="8c0a1-137">When a certificate is broken or outdated on a machine, you may receive an error indicating that curl failed to verify the legitimacy of the server and therefore could not establish a secure connection.</span></span>  <span data-ttu-id="8c0a1-138">Mettez à jour votre certificat pour corriger le problème.</span><span class="sxs-lookup"><span data-stu-id="8c0a1-138">Update your certificate to correct the problem.</span></span>  

```bach
sudo zypper update-ca-certificates
```

## <a name="update"></a><span data-ttu-id="8c0a1-139">Update</span><span class="sxs-lookup"><span data-stu-id="8c0a1-139">Update</span></span>

[!INCLUDE [az-upgrade](includes/az-upgrade.md)]

<span data-ttu-id="8c0a1-140">Vous pouvez aussi mettre à jour le package avec la commande `zypper update`.</span><span class="sxs-lookup"><span data-stu-id="8c0a1-140">You can also update the package with the `zypper update` command.</span></span>

```bash
sudo zypper refresh
sudo zypper update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="8c0a1-141">Désinstaller l’interface</span><span class="sxs-lookup"><span data-stu-id="8c0a1-141">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="8c0a1-142">Supprimez le package de votre système.</span><span class="sxs-lookup"><span data-stu-id="8c0a1-142">Remove the package from your system.</span></span>

    ```bash
    sudo zypper remove -y azure-cli
    ```

2. <span data-ttu-id="8c0a1-143">Si vous ne prévoyez pas de réinstaller l’interface CLI, supprimez les informations de référentiel.</span><span class="sxs-lookup"><span data-stu-id="8c0a1-143">If you don't plan to reinstall the CLI, remove the repository information.</span></span>

   ```bash
   sudo zypper removerepo azure-cli
   ```

3. <span data-ttu-id="8c0a1-144">Si vous n’utilisez pas d’autres packages Microsoft, supprimez la clé de signature Microsoft.</span><span class="sxs-lookup"><span data-stu-id="8c0a1-144">If you don't use other Microsoft packages, remove the Microsoft signing key.</span></span>

   ```bash
   MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
   sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
   ```

## <a name="next-steps"></a><span data-ttu-id="8c0a1-145">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="8c0a1-145">Next Steps</span></span>

<span data-ttu-id="8c0a1-146">Maintenant que vous avez installé l’interface CLI, découvrez ses fonctionnalités et ses commandes courantes.</span><span class="sxs-lookup"><span data-stu-id="8c0a1-146">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="8c0a1-147">Prise en main de l’interface Azure CLI</span><span class="sxs-lookup"><span data-stu-id="8c0a1-147">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)