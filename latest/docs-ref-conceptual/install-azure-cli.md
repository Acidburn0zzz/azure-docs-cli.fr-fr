---
title: Installer Azure CLI 2.0
description: "Documents de référence pour l’installation de l’interface de ligne de commande Azure 2.0"
keywords: "Azure CLI, Installer Azure CLI, Azure Python CLI, Référence sur Azure CLI"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 08/17/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: ea5c0ee1-c530-4a1e-a83f-e1be71f6d416
ms.openlocfilehash: 580438bfc66f3ed0b4dad504258eab453b1b9183
ms.sourcegitcommit: c1df7794ad42adb8640b51b630e4275f4a791ac2
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/19/2017
---
# <a name="install-azure-cli-20"></a>Installer Azure CLI 2.0

Installez la nouvelle version de l’interface de ligne de commande Azure dès aujourd’hui.
Nous avons amélioré et mis à jour cette interface afin d’offrir une expérience de ligne de commande native d’exception pour la gestion des ressources Azure.
Elle peut être utilisée sur macOS, Linux et Windows.
Pour plus d’informations sur la version la plus récente, consultez les [Notes de publication](release-notes-azure-cli.md).

> [!NOTE]
> Si vous devez utiliser la version précédente d’Azure CLI, voici comment [installer Azure 1.0](/azure/cli-install-nodejs).

## <a name="a-namemacosinstall-on-macos"></a><a name="macOS"/>Installer sur macOS

Sur macOS, vous avez le choix de procéder à l’installation avec [Homebrew](https://brew.sh/) ou manuellement.

### <a name="install-with-homebrew"></a>Désinstaller avec Homebrew

1. Si vous ne l’avez pas encore, installez Homebrew en suivant les [instructions d’installation pour Homebrew](https://docs.brew.sh/Installation.html).

2. Mettez à jour vos référentiels Homebrew locaux.

   ```bash
   brew update
   ```

3. Installez le package `azure-cli`.

  ```bash
  brew install azure-cli
  ```

> [!NOTE]
> Si vous avez installé Azure CLI 1.0 avec Homebrew au préalable, au lieu d’installer le package, vous pouvez obtenir CLI 2.0 grâce au processus normal de mise à niveau Homebrew.
>
> ```bash
> brew upgrade
> ```

### <a name="install-manually"></a>Installer manuellement

1. Installer l’interface de ligne de commande Azure 2.0 avec `curl`.

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

2. Vous devrez peut-être redémarrer votre interpréteur de commandes pour que certaines modifications soient prises en compte.

   ```bash
   exec -l $SHELL
   ```
   
3. Exécutez l’interface de ligne de commande Azure 2.0 à partir de l’invite de commandes avec la commande `az` .

## <a name="install-on-windows"></a>Installer sur Windows

Vous pouvez installer l’interface de ligne de commande Azure 2.0 avec le MSI et l’utiliser dans la ligne de commande Windows, ou vous pouvez installer la CLI avec `apt-get` sur Bash sous Ubuntu ou Windows.

### <a name="install-with-msi-for-the-windows-command-line"></a>Installer avec MSI pour la ligne de commande Windows 

Pour installer l’interface de ligne de commande sous Windows et l’utiliser dans la ligne de commande Windows, téléchargez et exécutez le [MSI](https://aka.ms/InstallAzureCliWindows).

### <a name="install-with-apt-get-for-bash-on-ubuntu-on-windows"></a>Installer avec apt-get pour Bash sous Ubuntu ou Windows

1. Si vous ne disposez pas de Bash sur Windows, [installez-le](https://msdn.microsoft.com/commandline/wsl/install_guide).

2. Ouvrez l’interpréteur de commandes Bash.

3. Modifiez votre liste de sources.

   ```bash
   echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
   ```

4. Exécutez les commandes sudo suivantes :

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

5.  Exécutez l’interface de ligne de commande Azure 2.0 à partir de l’invite de commandes avec la commande `az` .

## <a name="install-on-debianubuntu-with-apt-get"></a>Installer sous Debian/Ubuntu avec apt-get

Dans le cas des systèmes Debian/Ubuntu, vous pouvez installer Azure CLI 2.0 par le biais de la commande `apt-get`.

1. Modifiez votre liste de sources :
 
   - Système 32 bits

     ```bash
     echo "deb https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

   - Système 64 bits

     ```bash
     echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

2. Exécutez les commandes sudo suivantes :

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

3.  Exécutez l’interface de ligne de commande Azure 2.0 à partir de l’invite de commandes avec la commande `az` .

## <a name="install-on-rhel-fedora-and-centos-with-yum"></a>Installer sur RHEL, Fedora et CentOS avec yum

Pour une distribution basée sur RedHat et qui contient le gestionnaire de package `yum`, vous pouvez installer Azure CLI 2.0 via `yum`.

1. Importer la clé de référentiel Microsoft :

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. Créer des informations de référentiel `azure-cli` locales :

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/azure-cli.repo'
   ```

3. Mettre à jour l’index de package `yum` et l’installer :

   ```bash
   yum check-update
   sudo yum install azure-cli
   ```

4. Exécutez l’interface de ligne de commande Azure 2.0 à partir de l’invite de commandes avec la commande `az` .

## <a name="install-on-opensuse-and-sle-with-zypper"></a>Installer sur openSUSE et SLE avec zypper

1. Importer la clé de référentiel Microsoft :

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. Créer des informations de référentiel `azure-cli` locales :

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ntype=rpm-md\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/zypp/repos.d/azure-cli.repo'
   ```

3. Mettre à jour l’index de package `zypper` et l’installer :

   ```bash
   sudo zypper refresh
   sudo zypper install azure-cli
   ```

4. Exécutez l’interface de ligne de commande Azure 2.0 à partir de l’invite de commandes avec la commande `az` .

## <a name="install-with-docker"></a>Installer avec Docker

Nous fournissons une image Docker pré-configurée avec l’interface de ligne de commande Azure 2.0.

Installez l’interface de ligne de commande à l’aide de `docker run`.

   ```bash
   docker run azuresdk/azure-cli-python:<version>
   ```

Consultez nos [balises Docker](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/) pour connaître les versions disponibles.

L’interface de ligne de commande est installé sur l’image en tant que commande `az` dans `/usr/local/bin`.

> [!NOTE]
> Si vous souhaitez sélectionner les clés SSH à partir de votre environnement utilisateur, vous pouvez utiliser `-v ${HOME}:/root` pour monter $HOME en tant que `/root`.

> ```bash
> docker run -v ${HOME}:/root azuresdk/azure-cli-python:<version>
> ```

## <a name="a-namelinuxinstall-on-linux-without-apt-get"></a><a name="Linux"/>Installer sous Linux sans apt-get

Il est recommandé d’installer l’interface de ligne de commande avec un gestionnaire de package si possible. Pour les distributions ne disposant pas de gestionnaire de package, vous pouvez procéder à une installation manuelle.

1. Installez les composants requis en fonction de votre distribution Linux.

   ```
   Platform              | Prerequisites
   ----------------------|---------------------------------------------
   Ubuntu 15.10 or 16.04 | sudo apt-get update && sudo apt-get install -y python libssl-dev libffi-dev python-dev build-essential
   Ubuntu 12.04 or 14.04 | sudo apt-get update && sudo apt-get install -y python libssl-dev libffi-dev python-dev
   Debian 8              | sudo apt-get update && sudo apt-get install -y python libssl-dev libffi-dev python-dev build-essential
   Debian 7              | sudo apt-get update && sudo apt-get install -y python libssl-dev libffi-dev python-dev
   CentOS 7.1 or 7.2     | sudo yum check-update; sudo yum install -y gcc python libffi-devel python-devel openssl-devel
   RedHat 7.2            | sudo yum check-update; sudo yum install -y gcc python libffi-devel python-devel openssl-devel
   SUSE OpenSUSE 13.2    | sudo zypper refresh && sudo zypper --non-interactive install curl gcc python python-xml libffi-devel python-devel openssl-devel
   ```

Si votre distribution ne figure pas ci-dessus, vous devez installer [Python](https://www.python.org/downloads/), [libffi](https://sourceware.org/libffi/), et [OpenSSL](https://www.openssl.org/source/).

2. Installez l’interface de ligne de commande à l’aide de `curl`.

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

3. Vous devrez peut-être redémarrer votre interpréteur de commandes pour que certaines modifications soient prises en compte.

   ```bash
   exec -l $SHELL
   ```

4. Exécutez l’interface de ligne de commande Azure 2.0 à partir de l’invite de commandes avec la commande `az` .

## <a name="troubleshooting"></a>Résolution des problèmes

Si vous rencontrez un problème lors de l’installation de l’interface de ligne de commande, consultez cette section pour savoir si votre cas particulier est couvert. Si votre problème n’est pas ici, veuillez [signaler le problème lié à Github](https://github.com/Azure/azure-cli/issues).

### <a name="curl-object-moved-error"></a>erreur curl « Objet déplacé »

Si la commande `curl` renvoie une erreur concernant le `-L` paramètre ou un message d’erreur indiquant « Objet déplacé », essayez d’utiliser l’URL complète plutôt que la `aka.ms` redirection :

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

## <a name="uninstall-cli-1x-versions"></a>Désinstaller les versions 1.x de l’interface de ligne de commande

Si vous votre système dispose d’une version 1.x antérieure de l’interface de ligne de commande, vous pouvez la désinstaller en fonction du type d’installation utilisé.

### <a name="uninstall-with-npm"></a>Désinstaller avec npm

Supprimez l’ancienne interface de ligne de commande avec `npm uninstall`.

  ```bash
  npm uninstall -g azure-cli
  ```

### <a name="uninstall-with-distributable"></a>Désinstaller avec distribuable

Si vous avez installé [MSI](http://aka.ms/webpi-azure-cli) ou un [package macOS](http://aka.ms/mac-azure-cli), utilisez le même outil pour supprimer votre installation.

### <a name="uninstall-with-docker"></a>Désinstaller avec Docker

Si vous avez installé une image Docker pour utiliser la version antérieure de l’interface de ligne de commande, supprimez cette image et tous les conteneurs associés. Vous pouvez ensuite recréer les conteneurs après l’installation de la nouvelle image Docker comme décrit dans les instructions d’installation.

  ```bash
  docker rmi -f microsoft/azure-cli
  ```

## <a name="update-the-cli"></a>Mise à jour de l’interface CLI

Pour mettre à jour l’interface de ligne de commande Azure, utilisez la même méthode que vous avez utilisée pour l’installer.

### <a name="update-with-homebrew"></a>Mettre à jour avec Homebrew

1. Mettez à jour vos informations de référentiel Homebrew locales.

   ```bash
   brew update
   ```

2. Mettez à niveau les packages installés.

   ```bash
   brew upgrade
   ```

### <a name="update-with-msi"></a>Mettre à jour avec MSI

Exécutez de nouveau le [MSI](https://aka.ms/InstallAzureCliWindows) .

### <a name="update-with-apt-get"></a>Mettre à jour avec apt-get

Utilisez `apt-get upgrade` pour mettre à jour le package de l’interface de ligne de commande.

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> Cela met à niveau tous les packages installés sur votre système n’ayant pas de modification de dépendance.
> Pour ne mettre à niveau que l’interface de ligne de commande, utilisez `apt-get install`.
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

### <a name="update-with-docker"></a>Mettre à jour avec Docker

1. Mettre à jour votre image locale avec `docker pull`.

   ```bash
   docker pull azuresdk/azure-cli-python
   ```

2. Obtenir les conteneurs qui utilisent actuellement l’image de l’interface de ligne de commande.

   ```bash
   docker container ls -a --filter 'ancestor=azuresdk/azure-cli-python'
   ```

   ```output
   CONTAINER ID        IMAGE                              COMMAND             CREATED             STATUS                        PORTS               NAMES
   34a868beb2ab        azuresdk/azure-cli-python:latest      "/bin/sh -c bash"   8 minutes ago       Exited (0) 8 minutes ago                       inspiring_benz
   ```

> [!NOTE]
> Si vous avez installé une version spécifique de l’image, vous devez ajouter `:<version>` à la fin du nom de l’image.

3. Interrompre et recréer les conteneurs.

   ```bash
   docker stop inspiring_benz
   docker rm inspiring_benz
   docker run azuresdk/azure-cli-python
   ```

### <a name="update-manually"></a>Mettre à jour manuellement

Suivez les instructions d’installation manuelle de [macOS](#macOS) ou [Linux](#Linux) pour effectuer la mise à jour.

## <a name="uninstall"></a>Désinstaller l’interface

Si vous décidez de désinstaller l’interface de ligne de commande, nous sommes désolés de vous voir partir. Vous devez effectuer la désinstallation à l’aide de la même méthode que vous avez utilisée pour installer l’interface de ligne de commande.

### <a name="uninstall-with-homebrew"></a>Désinstaller avec Homebrew

Désinstallez le package `azure-cli`.

   ```bash
   brew uninstall azure-cli
   ```

### <a name="uninstall-with-msi"></a>Désinstaller avec MSI

Exécutez le [MSI](https://aka.ms/InstallAzureCliWindows) de nouveau et choisissez Désinstaller.

### <a name="uninstall-with-apt-get"></a>Désinstaller avec apt-get

Désinstallation via `apt-get remove`:

  ```bash
  sudo apt-get remove -y azure-cli
  ```

### <a name="uninstall-with-docker"></a>Désinstaller avec Docker

Si vous avez installé une image docker, vous devez supprimer tous les conteneurs qui l’exécutent avant de supprimer l’image locale.

1. Obtenez les conteneurs qui exécutent l’image de l’interface de ligne de commande Azure.

   ```bash
   docker container ls -a --filter 'ancestor=azuresdk/azure-cli-python'
   ```

   ```output
   CONTAINER ID        IMAGE                              COMMAND             CREATED             STATUS                        PORTS               NAMES
   34a868beb2ab        azuresdk/azure-cli-python:latest      "/bin/sh -c bash"   8 minutes ago       Exited (0) 8 minutes ago                       inspiring_benz
   ```

2. Supprimez tous les conteneurs avec l’image de l’interface de ligne de commande.

   ```bash
   docker rm 34a868beb2ab
   ```

3. Supprimez l’image de l’interface de ligne de commande installée localement.

   ```bash
   docker rmi azuresdk/azure-cli-python
   ```

> [!NOTE]
> Si vous avez installé une version spécifique de l’image, vous devez ajouter `:<version>` à la fin du nom de l’image.

### <a name="uninstall-manually"></a>Désinstaller manuellement

Si vous avez installé l’interface de ligne de commande en utilisant le script accessible à l’adresse https://aka.ms/InstallAzureCli, vous pouvez désinstaller l’interface à l’aide de la procédure suivante.

1. Supprimez les fichiers installés.

   ```bash
   rm -r <install location>/lib/azure-cli
   rm <install location>/bin/az
   ```

2. Supprimez la ligne `<install location>/lib/azure-cli/az.completion` de `<install location>/.bash_profile`.

> [!Note]
> L’emplacement d’installation par défaut est `/Users/<username>`.

## <a name="report-cli-issues-and-feedback"></a>Signaler des problèmes avec CLI et commentaires

Si vous rencontrez des bogues en utilisant l’outil, signalez un problème dans la section [Problèmes](https://github.com/Azure/azure-cli/issues) de notre référentiel GitHub.
Pour fournir des commentaires à partir de la ligne de commande, utilisez la commande `az feedback`.
