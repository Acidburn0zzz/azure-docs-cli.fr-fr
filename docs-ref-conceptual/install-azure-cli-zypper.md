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
ms.custom: devx-track-azurecli
ms.openlocfilehash: 1fe5b06985bb3aabf7e99f0dcebf481a79ebd6e7
ms.sourcegitcommit: bf84dfb62e910ea246586481863bb43d09d07795
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/04/2020
ms.locfileid: "87551485"
---
# <a name="install-azure-cli-with-zypper"></a>Installez Azure CLI avec zypper

Pour les distributions Linux avec `zypper`, telles que openSUSE ou SLES, un package est disponible pour l’Azure CLI. Ce package a été testé avec openSUSE Leap 15.1 and SLES 15.

[!INCLUDE [current-version](includes/current-version.md)]

[!INCLUDE [rpm-warning](includes/rpm-warning.md)]

## <a name="install"></a>Installer

1. Installez `curl` :

   ```bash
   sudo zypper install -y curl
   ```

2. Importer la clé de référentiel Microsoft :

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

3. Créer des informations de référentiel `azure-cli` locales :

   ```bash
   sudo zypper addrepo --name 'Azure CLI' --check https://packages.microsoft.com/yumrepos/azure-cli azure-cli
   ```

4. Mettre à jour l’index de package `zypper` et l’installer :

   ```bash
   sudo zypper install --from azure-cli azure-cli
   ```
   Entrez 2 pour continuer l’installation en ignorant certaines de ses dépendances.

Vous pouvez ensuite exécuter l’interface de ligne de commande Azure avec la commande `az`. Pour vous connecter, utilisez la commande [az login](/cli/azure/reference-index#az-login).

[!INCLUDE [interactive-login](includes/interactive-login.md)]

Pour en savoir plus sur les différentes méthodes d’authentification, consultez [Se connecter avec Azure CLI](authenticate-azure-cli.md).

## <a name="troubleshooting"></a>Dépannage

Voici certains problèmes courants lors de l’installation avec `zypper`. Si vous rencontrez un problème n’étant pas évoqué ici, [signalez un problème sur github](https://github.com/Azure/azure-cli/issues).

### <a name="install-on-sles-12-or-other-systems-without-python-36"></a>Installer sur SLES 12 ou d’autres systèmes sans Python 3.6

Sur SLES 12, le package python3 par défaut est la version 3.4 et n’est pas pris en charge par Azure CLI. Vous pouvez d’abord générer une version de python3 plus récente à partir de la source. Vous pouvez alors télécharger le package Azure CLI et l’installer sans dépendance.
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

### <a name="proxy-blocks-connection"></a>Le proxy bloque la connexion

[!INCLUDE[configure-proxy](includes/configure-proxy.md)]

Vous pouvez également configurer de manière explicite `zypper` (via `yast2`) pour utiliser ce proxy à tout moment. Pour ce faire, exécutez la commande `yast2 proxy` en tant que superutilisateur et remplissez les informations présentées dans le formulaire. Si vous avez un gestionnaire de fenêtres disponible sur votre système, vous pouvez également utiliser le volet `Network Services > Proxy` dans le `YaST Control Center`.

Pour la configuration avancée ou plus d’informations, consultez la [documentation de configuration de proxy OpenSUSE](https://www.suse.com/documentation/slms1/book_slms/data/sec_wy_config_updates_proxy.html)

Pour obtenir la clé de signature Microsoft et obtenir le package à partir de notre dépôt, votre proxy doit autoriser les connexions HTTPS aux adresses suivantes :

* `https://packages.microsoft.com`
* `https://download.opensuse.org`

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

### <a name="ssl-certificate-problem"></a>Problème de certificat SSL

Lorsqu’un certificat est arrêté ou obsolète sur un ordinateur, vous pouvez recevoir une erreur indiquant que curl n’a pas réussi à vérifier la légitimité du serveur et n’a donc pas pu établir de connexion sécurisée.  Mettez à jour votre certificat pour corriger le problème.  

```bach
sudo zypper update-ca-certificates
```

## <a name="update"></a>Update

Vous pouvez mettre à jour le package avec la commande `zypper update`.

```bash
sudo zypper refresh
sudo zypper update azure-cli
```

## <a name="uninstall"></a>Désinstaller l’interface

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. Supprimez le package de votre système.

    ```bash
    sudo zypper remove -y azure-cli
    ```

2. Si vous ne prévoyez pas de réinstaller l’interface CLI, supprimez les informations de référentiel.

   ```bash
   sudo zypper removerepo azure-cli
   ```

3. Si vous n’utilisez pas d’autres packages Microsoft, supprimez la clé de signature Microsoft.

   ```bash
   MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
   sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
   ```

## <a name="next-steps"></a>Étapes suivantes

Maintenant que vous avez installé l’interface CLI, découvrez ses fonctionnalités et ses commandes courantes.

> [!div class="nextstepaction"]
> [Prise en main de l’interface Azure CLI](get-started-with-azure-cli.md)
