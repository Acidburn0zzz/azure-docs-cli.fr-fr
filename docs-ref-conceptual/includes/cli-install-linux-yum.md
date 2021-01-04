---
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 11/24/2020
ms.topic: include
ms.custom: devx-track-azurecli
ms.openlocfilehash: 6f121eff4f024da81dbf107fba5f5bd9d3b8aa0b
ms.sourcegitcommit: d5f026468ea20bbd7ef35bdbf9852bcb2b812d83
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/23/2020
ms.locfileid: "97744614"
---
## <a name="overview"></a><span data-ttu-id="c8a83-101">Vue d’ensemble</span><span class="sxs-lookup"><span data-stu-id="c8a83-101">Overview</span></span>

<span data-ttu-id="c8a83-102">Pour les distributions Linux avec `yum` telles que RHEL, Fedora ou CentOS, il existe un package pour Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="c8a83-102">For Linux distributions with `yum` such as RHEL, Fedora, or CentOS, there's a package for the Azure CLI.</span></span> <span data-ttu-id="c8a83-103">Ce package a été testé avec RHEL 7.7, RHEL 8, Fedora 24 et versions ultérieures, CentOS 7 et CentOS 8.</span><span class="sxs-lookup"><span data-stu-id="c8a83-103">This package has been tested with RHEL 7.7, RHEL 8, Fedora 24 and higher, CentOS 7 and CentOS 8.</span></span>

[!INCLUDE [current-version](current-version.md)]

[!INCLUDE [rpm-warning](rpm-warning.md)]

## <a name="install"></a><span data-ttu-id="c8a83-104">Installer</span><span class="sxs-lookup"><span data-stu-id="c8a83-104">Install</span></span>

1. <span data-ttu-id="c8a83-105">Importez la clé de référentiel Microsoft.</span><span class="sxs-lookup"><span data-stu-id="c8a83-105">Import the Microsoft repository key.</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. <span data-ttu-id="c8a83-106">Créez des informations de référentiel `azure-cli` locales.</span><span class="sxs-lookup"><span data-stu-id="c8a83-106">Create local `azure-cli` repository information.</span></span>

   ```bash
   echo -e "[azure-cli]
   name=Azure CLI
   baseurl=https://packages.microsoft.com/yumrepos/azure-cli
   enabled=1
   gpgcheck=1
   gpgkey=https://packages.microsoft.com/keys/microsoft.asc" | sudo tee /etc/yum.repos.d/azure-cli.repo
   ```

3. <span data-ttu-id="c8a83-107">Installez avec la commande `yum install`.</span><span class="sxs-lookup"><span data-stu-id="c8a83-107">Install with the `yum install` command.</span></span>

   ```bash
   sudo yum install azure-cli
   ```

<span data-ttu-id="c8a83-108">Exécutez Azure CLI avec la commande `az`.</span><span class="sxs-lookup"><span data-stu-id="c8a83-108">Run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="c8a83-109">Pour vous connecter, utilisez la commande [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="c8a83-109">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](interactive-login.md)]

<span data-ttu-id="c8a83-110">Pour en savoir plus sur les différentes méthodes d’authentification, consultez [Se connecter avec Azure CLI](../authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="c8a83-110">To learn more about different authentication methods, see [Sign in with Azure CLI](../authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="c8a83-111">Dépannage</span><span class="sxs-lookup"><span data-stu-id="c8a83-111">Troubleshooting</span></span>

<span data-ttu-id="c8a83-112">Voici certains problèmes courants lors de l’installation avec `yum`.</span><span class="sxs-lookup"><span data-stu-id="c8a83-112">Here are some common problems seen when installing with `yum`.</span></span> <span data-ttu-id="c8a83-113">Si vous rencontrez un problème qui n’est pas traité ici, [signalez ce problème sur GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="c8a83-113">If you experience a problem not covered here, [file an issue on GitHub](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="install-on-rhel-76-or-other-systems-without-python-3"></a><span data-ttu-id="c8a83-114">Installer sur RHEL 7.6 ou d’autres systèmes sans Python 3</span><span class="sxs-lookup"><span data-stu-id="c8a83-114">Install on RHEL 7.6 or other systems without Python 3</span></span>

<span data-ttu-id="c8a83-115">Si vous le pouvez, mettez à niveau votre système vers une version avec prise en charge officielle du package `python 3.6+`.</span><span class="sxs-lookup"><span data-stu-id="c8a83-115">If you can, please upgrade your system to a version with official support for `python 3.6+` package.</span></span> <span data-ttu-id="c8a83-116">Si ce n’est pas possible, vous devrez d’abord installer un package `python3`, puis installer Azure CLI sans dépendance.</span><span class="sxs-lookup"><span data-stu-id="c8a83-116">Otherwise, you need to first install a `python3` package then install Azure CLI without dependency.</span></span>

<span data-ttu-id="c8a83-117">Vous pouvez utiliser la commande suivante pour installer Azure CLI avec `python 3.6` généré à partir de la source :</span><span class="sxs-lookup"><span data-stu-id="c8a83-117">You can use the following one command to install Azure CLI with `python 3.6` built from source:</span></span>

```bash
curl -sL https://azurecliprod.blob.core.windows.net/rhel7_6_install.sh | sudo bash
```

<span data-ttu-id="c8a83-118">Vous pouvez également le faire étape par étape :</span><span class="sxs-lookup"><span data-stu-id="c8a83-118">You can also do it step by step:</span></span>

<span data-ttu-id="c8a83-119">Tout d’abord, Azure CLI nécessite `SSL 1.1+`. En outre, vous devez générer `openssl 1.1` à partir de la source avant de générer `python3` :</span><span class="sxs-lookup"><span data-stu-id="c8a83-119">First, Azure CLI requires `SSL 1.1+` and you need to build `openssl 1.1` from source before building `python3`:</span></span>

```bash
$ sudo yum install gcc gcc-c++ make ncurses patch wget tar zlib zlib-devel -y
# build openssl from source
$ cd ~
$ wget https://www.openssl.org/source/openssl-1.1.1d.tar.gz
$ tar -xzf openssl-1.1.1d.tar.gz
$ cd openssl-1.1.1d
$ ./config --prefix=/usr/local/ssl --openssldir=/usr/local/ssl
$ make
$ sudo make install
# configure shared object lookup directory so that libssl.so.1.1 can be found
$ echo "/usr/local/ssl/lib" | sudo tee /etc/ld.so.conf.d/openssl-1.1.1d.conf
# reload config
$ sudo ldconfig -v
```

<span data-ttu-id="c8a83-120">Ensuite, générez Python 3 à partir de la source :</span><span class="sxs-lookup"><span data-stu-id="c8a83-120">Then build Python 3 from source:</span></span>

```bash
$ PYTHON_VERSION="3.6.9"
$ PYTHON_SRC_DIR=$(mktemp -d)
$ wget -qO- https://www.python.org/ftp/python/$PYTHON_VERSION/Python-$PYTHON_VERSION.tgz | tar -xz -C "$PYTHON_SRC_DIR"
$ cd $PYTHON_SRC_DIR/Python-$PYTHON_VERSION
$ ./configure --prefix=/usr --with-openssl=/usr/local/ssl
$ make
$ sudo make install
```

<span data-ttu-id="c8a83-121">Enfin, suivez les étapes 1 et 2 des [instructions d’installation](#install) pour ajouter le dépôt Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="c8a83-121">Finally, follow step 1 and 2 of the [install instruction](#install) to add Azure CLI repository.</span></span> <span data-ttu-id="c8a83-122">Vous pouvez désormais télécharger le package et l’installer sans dépendance.</span><span class="sxs-lookup"><span data-stu-id="c8a83-122">You can now download the package and install it without dependency.</span></span>

```bash
$ sudo yum install yum-utils -y
$ sudo yumdownloader azure-cli
$ sudo rpm -ivh --nodeps azure-cli-*.rpm
```

<span data-ttu-id="c8a83-123">En guise d’alternative, vous pouvez également installer Python 3 à l’aide d’un [dépôt supplémentaire](https://developers.redhat.com/blog/2018/08/13/install-python3-rhel/).</span><span class="sxs-lookup"><span data-stu-id="c8a83-123">As an alternative, you can also install Python 3 through some [additional repo](https://developers.redhat.com/blog/2018/08/13/install-python3-rhel/).</span></span> <span data-ttu-id="c8a83-124">Si vous avez configuré `python3`, mais que vous obtenez toujours une erreur `python3: command not found` lorsque vous essayez d’exécuter l’interface CLI, vous devez l’ajouter dans votre chemin.</span><span class="sxs-lookup"><span data-stu-id="c8a83-124">Following this way, if you have set up `python3` but are still getting an error `python3: command not found` when trying to run the cli, you need to add it to your path.</span></span>

```bash
$ scl enable rh-python36 bash
```

### <a name="proxy-blocks-connection"></a><span data-ttu-id="c8a83-125">Le proxy bloque la connexion</span><span class="sxs-lookup"><span data-stu-id="c8a83-125">Proxy blocks connection</span></span>

[!INCLUDE[configure-proxy](configure-proxy.md)]

<span data-ttu-id="c8a83-126">Vous pouvez également configurer de manière explicite `yum` pour utiliser ce proxy à tout moment.</span><span class="sxs-lookup"><span data-stu-id="c8a83-126">You may also want to explicitly configure `yum` to use this proxy at all times.</span></span> <span data-ttu-id="c8a83-127">Vérifiez que les lignes suivantes s’affichent sous la section `[main]` de `/etc/yum.conf` :</span><span class="sxs-lookup"><span data-stu-id="c8a83-127">Make sure that the following lines appear under the `[main]` section of `/etc/yum.conf`:</span></span>

```yum.conf
[main]
# ...
proxy=http://[proxy]:[port] # If your proxy requires https, change http->https
proxy_username=[username] # Only required for basic auth
proxy_password=[password] # Only required for basic auth
```

<span data-ttu-id="c8a83-128">Pour obtenir la clé de signature Microsoft et obtenir le package à partir de notre dépôt, votre proxy doit autoriser les connexions HTTPS à l’adresse suivante :</span><span class="sxs-lookup"><span data-stu-id="c8a83-128">In order to get the Microsoft signing key and get the package from our repository, your proxy needs to allow HTTPS connections to the following address:</span></span>

* `https://packages.microsoft.com`

[!INCLUDE[troubleshoot-wsl.md](troubleshoot-wsl.md)]

## <a name="update"></a><span data-ttu-id="c8a83-129">Update</span><span class="sxs-lookup"><span data-stu-id="c8a83-129">Update</span></span>

[!INCLUDE [az-upgrade](az-upgrade.md)]

<span data-ttu-id="c8a83-130">Vous pouvez aussi mettre à jour Azure CLI avec la commande `yum update`.</span><span class="sxs-lookup"><span data-stu-id="c8a83-130">You can also update the Azure CLI with the `yum update` command.</span></span>

```bash
sudo yum update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="c8a83-131">Désinstaller l’interface</span><span class="sxs-lookup"><span data-stu-id="c8a83-131">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](uninstall-boilerplate.md)]

1. <span data-ttu-id="c8a83-132">Supprimez le package de votre système.</span><span class="sxs-lookup"><span data-stu-id="c8a83-132">Remove the package from your system.</span></span>

   ```bash
   sudo yum remove azure-cli
   ```

2. <span data-ttu-id="c8a83-133">Si vous ne prévoyez pas de réinstaller l’interface CLI, supprimez les informations de référentiel.</span><span class="sxs-lookup"><span data-stu-id="c8a83-133">If you don't plan to reinstall the CLI, remove the repository information.</span></span>

   ```bash
   sudo rm /etc/yum.repos.d/azure-cli.repo
   ```

3. <span data-ttu-id="c8a83-134">Si vous n’utilisez pas d’autres packages Microsoft, supprimez la clé de signature.</span><span class="sxs-lookup"><span data-stu-id="c8a83-134">If you don't use any other Microsoft packages, remove the signing key.</span></span>

   ```bash
   MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
   sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
   ```
