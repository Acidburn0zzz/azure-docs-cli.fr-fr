---
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 11/24/2020
ms.topic: include
ms.custom: devx-track-azurecli
ms.openlocfilehash: 6044626c584eba4fd4ec55e11314cb89e20b3417
ms.sourcegitcommit: 8bff8b2ce4492ab99ad39390e4c802fb4f4425c8
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/26/2021
ms.locfileid: "105582269"
---
## <a name="overview"></a><span data-ttu-id="e75bc-101">Vue d’ensemble</span><span class="sxs-lookup"><span data-stu-id="e75bc-101">Overview</span></span>

<span data-ttu-id="e75bc-102">Pour les distributions Linux avec `dnf` telles que RHEL, Fedora ou CentOS, il existe un package pour Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="e75bc-102">For Linux distributions with `dnf` such as RHEL, Fedora, or CentOS, there's a package for the Azure CLI.</span></span> <span data-ttu-id="e75bc-103">Ce package a été testé avec RHEL 7.7, RHEL 8, Fedora 24 et versions ultérieures, CentOS 7 et CentOS 8.</span><span class="sxs-lookup"><span data-stu-id="e75bc-103">This package has been tested with RHEL 7.7, RHEL 8, Fedora 24 and higher, CentOS 7 and CentOS 8.</span></span>

[!INCLUDE [current-version](current-version.md)]

[!INCLUDE [rpm-warning](rpm-warning.md)]

> [!NOTE]
>
> <span data-ttu-id="e75bc-104">Utilisez le Gestionnaire de package `yum` si vous utilisez des systèmes Linux qui ne prennent pas en charge le Gestionnaire de package `dnf`.</span><span class="sxs-lookup"><span data-stu-id="e75bc-104">Use `yum` package manager if you are using Linux systems that don't support `dnf` package manager.</span></span>

## <a name="install"></a><span data-ttu-id="e75bc-105">Installer</span><span class="sxs-lookup"><span data-stu-id="e75bc-105">Install</span></span>

1. <span data-ttu-id="e75bc-106">Importez la clé de référentiel Microsoft.</span><span class="sxs-lookup"><span data-stu-id="e75bc-106">Import the Microsoft repository key.</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. <span data-ttu-id="e75bc-107">Créez des informations de référentiel `azure-cli` locales.</span><span class="sxs-lookup"><span data-stu-id="e75bc-107">Create local `azure-cli` repository information.</span></span>

   ```bash
   echo -e "[azure-cli]
   name=Azure CLI
   baseurl=https://packages.microsoft.com/yumrepos/azure-cli
   enabled=1
   gpgcheck=1
   gpgkey=https://packages.microsoft.com/keys/microsoft.asc" | sudo tee /etc/yum.repos.d/azure-cli.repo
   ```

3. <span data-ttu-id="e75bc-108">Installez avec la commande `dnf install`.</span><span class="sxs-lookup"><span data-stu-id="e75bc-108">Install with the `dnf install` command.</span></span>

   ```bash
   sudo dnf install azure-cli
   ```
 
<span data-ttu-id="e75bc-109">Exécutez Azure CLI avec la commande `az`.</span><span class="sxs-lookup"><span data-stu-id="e75bc-109">Run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="e75bc-110">Pour vous connecter, utilisez la commande [az login](/cli/azure/reference-index#az_login).</span><span class="sxs-lookup"><span data-stu-id="e75bc-110">To sign in, use [az login](/cli/azure/reference-index#az_login) command.</span></span>


[!INCLUDE [interactive-login](interactive-login.md)]

<span data-ttu-id="e75bc-111">Pour en savoir plus sur les différentes méthodes d’authentification, consultez [Se connecter avec Azure CLI](../authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="e75bc-111">To learn more about different authentication methods, see [Sign in with Azure CLI](../authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="e75bc-112">Dépannage</span><span class="sxs-lookup"><span data-stu-id="e75bc-112">Troubleshooting</span></span>

<span data-ttu-id="e75bc-113">Voici certains problèmes courants lors de l’installation avec `dnf`.</span><span class="sxs-lookup"><span data-stu-id="e75bc-113">Here are some common problems seen when installing with `dnf`.</span></span> <span data-ttu-id="e75bc-114">Si vous rencontrez un problème qui n’est pas traité ici, [signalez ce problème sur GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="e75bc-114">If you experience a problem not covered here, [file an issue on GitHub](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="install-on-rhel-76-or-other-systems-without-python-3"></a><span data-ttu-id="e75bc-115">Installer sur RHEL 7.6 ou d’autres systèmes sans Python 3</span><span class="sxs-lookup"><span data-stu-id="e75bc-115">Install on RHEL 7.6 or other systems without Python 3</span></span>

<span data-ttu-id="e75bc-116">Si vous le pouvez, mettez à niveau votre système vers une version avec prise en charge officielle du package `python 3.6+`.</span><span class="sxs-lookup"><span data-stu-id="e75bc-116">If you can, please upgrade your system to a version with official support for `python 3.6+` package.</span></span> <span data-ttu-id="e75bc-117">Si ce n’est pas possible, vous devrez d’abord installer un package `python3`, puis installer Azure CLI sans dépendance.</span><span class="sxs-lookup"><span data-stu-id="e75bc-117">Otherwise, you need to first install a `python3` package then install Azure CLI without dependency.</span></span>

<span data-ttu-id="e75bc-118">Vous pouvez utiliser la commande suivante pour installer Azure CLI avec `python 3.6` généré à partir de la source :</span><span class="sxs-lookup"><span data-stu-id="e75bc-118">You can use the following one command to install Azure CLI with `python 3.6` built from source:</span></span>

```bash
curl -sL https://azurecliprod.blob.core.windows.net/rhel7_6_install.sh | sudo bash
```

<span data-ttu-id="e75bc-119">Vous pouvez également le faire étape par étape :</span><span class="sxs-lookup"><span data-stu-id="e75bc-119">You can also do it step by step:</span></span>

<span data-ttu-id="e75bc-120">Tout d’abord, Azure CLI nécessite `SSL 1.1+`. En outre, vous devez générer `openssl 1.1` à partir de la source avant de générer `python3` :</span><span class="sxs-lookup"><span data-stu-id="e75bc-120">First, Azure CLI requires `SSL 1.1+` and you need to build `openssl 1.1` from source before building `python3`:</span></span>

```bash
$ sudo dnf install gcc gcc-c++ make ncurses patch wget tar zlib zlib-devel -y
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

<span data-ttu-id="e75bc-121">Ensuite, générez Python 3 à partir de la source :</span><span class="sxs-lookup"><span data-stu-id="e75bc-121">Then build Python 3 from source:</span></span>

```bash
$ PYTHON_VERSION="3.6.9"
$ PYTHON_SRC_DIR=$(mktemp -d)
$ wget -qO- https://www.python.org/ftp/python/$PYTHON_VERSION/Python-$PYTHON_VERSION.tgz | tar -xz -C "$PYTHON_SRC_DIR"
$ cd $PYTHON_SRC_DIR/Python-$PYTHON_VERSION
$ ./configure --prefix=/usr --with-openssl=/usr/local/ssl
$ make
$ sudo make install
```

<span data-ttu-id="e75bc-122">Enfin, suivez les étapes 1 et 2 des [instructions d’installation](#install) pour ajouter le dépôt Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="e75bc-122">Finally, follow step 1 and 2 of the [install instruction](#install) to add Azure CLI repository.</span></span> <span data-ttu-id="e75bc-123">Vous pouvez désormais télécharger le package et l’installer sans dépendance.</span><span class="sxs-lookup"><span data-stu-id="e75bc-123">You can now download the package and install it without dependency.</span></span>

> [!NOTE]
>
> <span data-ttu-id="e75bc-124">Si vous n’avez pas installé le plug-in dnf download, vous rencontrerez une erreur de commande introuvable lors de l’exécution du code ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="e75bc-124">In case you don't have the dnf download plugin installed, you will encounter command not found error on executing the below code.</span></span> <span data-ttu-id="e75bc-125">Utilisez `dnf install 'dnf-command(download)'` pour installer le plug-in dnf download.</span><span class="sxs-lookup"><span data-stu-id="e75bc-125">Use `dnf install 'dnf-command(download)'` to   install the dnf download plugin.</span></span>

```bash
$ sudo dnf download azure-cli
$ sudo rpm -ivh --nodeps azure-cli-*.rpm
```

<span data-ttu-id="e75bc-126">En guise d’alternative, vous pouvez également installer Python 3 à l’aide d’un [dépôt supplémentaire](https://developers.redhat.com/blog/2018/08/13/install-python3-rhel/).</span><span class="sxs-lookup"><span data-stu-id="e75bc-126">As an alternative, you can also install Python 3 through some [additional repo](https://developers.redhat.com/blog/2018/08/13/install-python3-rhel/).</span></span> <span data-ttu-id="e75bc-127">Si vous avez configuré `python3`, mais que vous obtenez toujours une erreur `python3: command not found` lorsque vous essayez d’exécuter l’interface CLI, vous devez l’ajouter dans votre chemin.</span><span class="sxs-lookup"><span data-stu-id="e75bc-127">Following this way, if you have set up `python3` but are still getting an error `python3: command not found` when trying to run the cli, you need to add it to your path.</span></span>

```bash
$ scl enable rh-python36 bash
```

### <a name="proxy-blocks-connection"></a><span data-ttu-id="e75bc-128">Le proxy bloque la connexion</span><span class="sxs-lookup"><span data-stu-id="e75bc-128">Proxy blocks connection</span></span>

[!INCLUDE[configure-proxy](configure-proxy.md)]

<span data-ttu-id="e75bc-129">Vous pouvez également configurer de manière explicite `dnf` pour utiliser ce proxy à tout moment.</span><span class="sxs-lookup"><span data-stu-id="e75bc-129">You may also want to explicitly configure `dnf` to use this proxy at all times.</span></span> <span data-ttu-id="e75bc-130">Vérifiez que les lignes suivantes s’affichent sous la section `[main]` de `/etc/dnf/dnf.conf` :</span><span class="sxs-lookup"><span data-stu-id="e75bc-130">Make sure that the following lines appear under the `[main]` section of `/etc/dnf/dnf.conf`:</span></span>

```dnf.conf
[main]
# ...
proxy=http://[proxy]:[port] # If your proxy requires https, change http->https
proxy_username=[username] # Only required for basic auth
proxy_password=[password] # Only required for basic auth
```

<span data-ttu-id="e75bc-131">Pour obtenir la clé de signature Microsoft et obtenir le package à partir de notre dépôt, votre proxy doit autoriser les connexions HTTPS à l’adresse suivante :</span><span class="sxs-lookup"><span data-stu-id="e75bc-131">In order to get the Microsoft signing key and get the package from our repository, your proxy needs to allow HTTPS connections to the following address:</span></span>

* `https://packages.microsoft.com`

[!INCLUDE[troubleshoot-wsl.md](troubleshoot-wsl.md)]

## <a name="update"></a><span data-ttu-id="e75bc-132">Update</span><span class="sxs-lookup"><span data-stu-id="e75bc-132">Update</span></span>

[!INCLUDE [az-upgrade](az-upgrade.md)]

<span data-ttu-id="e75bc-133">Vous pouvez aussi mettre à jour Azure CLI avec la commande `dnf update`.</span><span class="sxs-lookup"><span data-stu-id="e75bc-133">You can also update the Azure CLI with the `dnf update` command.</span></span>

```bash
sudo dnf update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="e75bc-134">Désinstaller l’interface</span><span class="sxs-lookup"><span data-stu-id="e75bc-134">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](uninstall-boilerplate.md)]

1. <span data-ttu-id="e75bc-135">Supprimez le package de votre système.</span><span class="sxs-lookup"><span data-stu-id="e75bc-135">Remove the package from your system.</span></span>

   ```bash
   sudo dnf remove azure-cli
   ```

2. <span data-ttu-id="e75bc-136">Si vous ne prévoyez pas de réinstaller l’interface CLI, supprimez les informations de référentiel.</span><span class="sxs-lookup"><span data-stu-id="e75bc-136">If you don't plan to reinstall the CLI, remove the repository information.</span></span>

   ```bash
   sudo rm /etc/yum.repos.d/azure-cli.repo
   ```

3. <span data-ttu-id="e75bc-137">Si vous n’utilisez pas d’autres packages Microsoft, supprimez la clé de signature.</span><span class="sxs-lookup"><span data-stu-id="e75bc-137">If you don't use any other Microsoft packages, remove the signing key.</span></span>

   ```bash
   MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
   sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
   ```
