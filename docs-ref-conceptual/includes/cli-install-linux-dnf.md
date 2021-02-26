---
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 11/24/2020
ms.topic: include
ms.custom: devx-track-azurecli
ms.openlocfilehash: c0de92ff9aed581d192d72ca920fafea8bbd192b
ms.sourcegitcommit: 594e9c620a6f74f5eaedf91a7f6a791e03a64c74
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/17/2021
ms.locfileid: "100631002"
---
## <a name="overview"></a>Vue d’ensemble

Pour les distributions Linux avec `dnf` telles que RHEL, Fedora ou CentOS, il existe un package pour Azure CLI. Ce package a été testé avec RHEL 7.7, RHEL 8, Fedora 24 et versions ultérieures, CentOS 7 et CentOS 8.

[!INCLUDE [current-version](current-version.md)]

[!INCLUDE [rpm-warning](rpm-warning.md)]

> [!NOTE]
>
> Utilisez le Gestionnaire de package `yum` si vous utilisez des systèmes Linux qui ne prennent pas en charge le Gestionnaire de package `dnf`.

## <a name="install"></a>Installer

1. Importez la clé de référentiel Microsoft.

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. Créez des informations de référentiel `azure-cli` locales.

   ```bash
   echo -e "[azure-cli]
   name=Azure CLI
   baseurl=https://packages.microsoft.com/yumrepos/azure-cli
   enabled=1
   gpgcheck=1
   gpgkey=https://packages.microsoft.com/keys/microsoft.asc" | sudo tee /etc/yum.repos.d/azure-cli.repo
   ```

3. Installez avec la commande `dnf install`.

   ```bash
   sudo dnf install azure-cli
   ```
 
Exécutez Azure CLI avec la commande `az`. Pour vous connecter, utilisez la commande [az login](/cli/azure/reference-index#az-login).


[!INCLUDE [interactive-login](interactive-login.md)]

Pour en savoir plus sur les différentes méthodes d’authentification, consultez [Se connecter avec Azure CLI](../authenticate-azure-cli.md).

## <a name="troubleshooting"></a>Dépannage

Voici certains problèmes courants lors de l’installation avec `dnf`. Si vous rencontrez un problème qui n’est pas traité ici, [signalez ce problème sur GitHub](https://github.com/Azure/azure-cli/issues).

### <a name="install-on-rhel-76-or-other-systems-without-python-3"></a>Installer sur RHEL 7.6 ou d’autres systèmes sans Python 3

Si vous le pouvez, mettez à niveau votre système vers une version avec prise en charge officielle du package `python 3.6+`. Si ce n’est pas possible, vous devrez d’abord installer un package `python3`, puis installer Azure CLI sans dépendance.

Vous pouvez utiliser la commande suivante pour installer Azure CLI avec `python 3.6` généré à partir de la source :

```bash
curl -sL https://azurecliprod.blob.core.windows.net/rhel7_6_install.sh | sudo bash
```

Vous pouvez également le faire étape par étape :

Tout d’abord, Azure CLI nécessite `SSL 1.1+`. En outre, vous devez générer `openssl 1.1` à partir de la source avant de générer `python3` :

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

Ensuite, générez Python 3 à partir de la source :

```bash
$ PYTHON_VERSION="3.6.9"
$ PYTHON_SRC_DIR=$(mktemp -d)
$ wget -qO- https://www.python.org/ftp/python/$PYTHON_VERSION/Python-$PYTHON_VERSION.tgz | tar -xz -C "$PYTHON_SRC_DIR"
$ cd $PYTHON_SRC_DIR/Python-$PYTHON_VERSION
$ ./configure --prefix=/usr --with-openssl=/usr/local/ssl
$ make
$ sudo make install
```

Enfin, suivez les étapes 1 et 2 des [instructions d’installation](#install) pour ajouter le dépôt Azure CLI. Vous pouvez désormais télécharger le package et l’installer sans dépendance.

> [!NOTE]
>
> Si vous n’avez pas installé le plug-in dnf download, vous rencontrerez une erreur de commande introuvable lors de l’exécution du code ci-dessous. Utilisez `dnf install 'dnf-command(download)'` pour installer le plug-in dnf download.

```bash
$ sudo dnf download azure-cli
$ sudo rpm -ivh --nodeps azure-cli-*.rpm
```

En guise d’alternative, vous pouvez également installer Python 3 à l’aide d’un [dépôt supplémentaire](https://developers.redhat.com/blog/2018/08/13/install-python3-rhel/). Si vous avez configuré `python3`, mais que vous obtenez toujours une erreur `python3: command not found` lorsque vous essayez d’exécuter l’interface CLI, vous devez l’ajouter dans votre chemin.

```bash
$ scl enable rh-python36 bash
```

### <a name="proxy-blocks-connection"></a>Le proxy bloque la connexion

[!INCLUDE[configure-proxy](configure-proxy.md)]

Vous pouvez également configurer de manière explicite `dnf` pour utiliser ce proxy à tout moment. Vérifiez que les lignes suivantes s’affichent sous la section `[main]` de `/etc/dnf/dnf.conf` :

```dnf.conf
[main]
# ...
proxy=http://[proxy]:[port] # If your proxy requires https, change http->https
proxy_username=[username] # Only required for basic auth
proxy_password=[password] # Only required for basic auth
```

Pour obtenir la clé de signature Microsoft et obtenir le package à partir de notre dépôt, votre proxy doit autoriser les connexions HTTPS à l’adresse suivante :

* `https://packages.microsoft.com`

[!INCLUDE[troubleshoot-wsl.md](troubleshoot-wsl.md)]

## <a name="update"></a>Update

[!INCLUDE [az-upgrade](az-upgrade.md)]

Vous pouvez aussi mettre à jour Azure CLI avec la commande `dnf update`.

```bash
sudo dnf update azure-cli
```

## <a name="uninstall"></a>Désinstaller l’interface

[!INCLUDE [uninstall-boilerplate.md](uninstall-boilerplate.md)]

1. Supprimez le package de votre système.

   ```bash
   sudo dnf remove azure-cli
   ```

2. Si vous ne prévoyez pas de réinstaller l’interface CLI, supprimez les informations de référentiel.

   ```bash
   sudo rm /etc/yum.repos.d/azure-cli.repo
   ```

3. Si vous n’utilisez pas d’autres packages Microsoft, supprimez la clé de signature.

   ```bash
   MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
   sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
   ```
