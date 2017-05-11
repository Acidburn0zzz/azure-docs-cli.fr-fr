---
title: Installer Azure CLI 2.0
description: "Documents de référence concernant Azure CLI 2.0"
keywords: "Azure CLI 2.0, Référence Azure CLI 2.0, Installer Azure CLI 2.0, interface de ligne de commande Python Azure, Désinstaller Azure CLI 2.0"
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 04/06/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: ea5c0ee1-c530-4a1e-a83f-e1be71f6d416
ms.openlocfilehash: b7c0b7c50794333b28c034de9b41f1e506053e25
ms.sourcegitcommit: 663d4188ccc4be425d3d551fe32613fafd05a764
ms.translationtype: HT
ms.contentlocale: fr-FR
---
# <a name="install-azure-cli-20"></a>Installer Azure CLI 2.0

Installez la nouvelle version de l’interface de ligne de commande Azure dès aujourd’hui.
Nous avons amélioré et mis à jour cette interface afin d’offrir une expérience de ligne de commande native d’exception pour la gestion des ressources Azure.
Elle peut être utilisée sur macOS, Linux et Windows.
Pour plus d’informations sur la version la plus récente, consultez les [notes de publication](release-notes-azure-cli.md).

> [!NOTE]
> Si vous devez utiliser la version précédente d’Azure CLI, voici comment [installer Azure 1.0](/azure/cli-install-nodejs).

## <a name="macos"></a>macOS

1. Installez Azure CLI 2.0 avec une commande `curl`.

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

2. Vous devrez peut-être redémarrer votre interface de commande pour que certaines modifications soient prises en compte.

   ```bash
   exec -l $SHELL
   ```
   
3. Exécutez Azure CLI 2.0 à partir de l’invite de commandes avec la commande `az`.

> [!Note]
> Lorsque vous effectuez l’installation avec InstallAzureCli, `az component update` n’est pas pris en charge.
> Pour mettre à jour l’interface de ligne de commande avec la dernière version, ré-exécutez `curl -L https://aka.ms/InstallAzureCli | bash`.
> 
> Pour désinstaller l’interface, reportez-vous aux [instructions de désinstallation manuelle](#uninstall).

## <a name="windows"></a>Windows

Étant donné qu’Azure CLI 2.0 prend en charge la syntaxe de commande Bash, Bash sur Ubuntu sur Windows constitue une excellente façon d’utiliser l’interface de ligne de commande.
Si vous n’utilisez pas Bash, vous pouvez installer et utiliser l’interface de ligne de commande dans la ligne de commande Windows.

### <a name="bash-on-ubuntu-on-windows"></a>Bash sur Ubuntu sur Windows

1. Si vous ne disposez pas de Bash sur Windows, [installez-le](https://msdn.microsoft.com/commandline/wsl/install_guide).

2. Ouvrez l’interpréteur de commandes Bash.

3. Si vous ne disposez pas de Python, installez-le.

   ```bash
   sudo apt-get install python3
   ```

   > [!NOTE]
   > Pour savoir si Python est installé, exécutez `python --version`.

4. Modifiez votre liste de sources.

   ```bash
   echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
   ```

5. Exécutez les commandes sudo suivantes :

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

> [!NOTE]
> Lorsque vous effectuez l’installation avec apt-get, `az component` n’est pas pris en charge.
> Pour mettre à jour l’interface de ligne de commande, ré-exécutez `sudo apt-get update && sudo apt-get install azure-cli`.
> 
> Pour désinstaller l’interface, exécutez `sudo apt-get remove azure-cli`.

### <a name="windows-command-line"></a>Ligne de commande Windows 

1. Accédez au site Python et [téléchargez Python](https://www.python.org/downloads/) pour Windows.
   Lorsque vous installez Python, prenez soin d’installer le composant Pip.
   Une fois l’installation effectuée, ajoutez Python à votre variable d’environnement PATH (lorsque le programme d’installation vous y invite).

2. Vérifiez votre installation de Python à partir d’une invite de commandes.

   ```bash
   python --version
   ```

3. Installez Azure CLI 2.0 en utilisant `pip`.

   ```bash
   pip install --user azure-cli
   ```

4. Ajoutez le dossier contenant le fichier az.bat à votre chemin d’accès.
   Le fichier `az.bat` de l’interface de ligne de commande peut être installé dans `%USERPROFILE%\AppData\Roaming\Python\Scripts` ou dans `%USERPROFILE%\AppData\Roaming\Python\PythonXY\Scripts`, où `XY` correspond à votre version Python (par exemple, `%USERPROFILE%\AppData\Roaming\Python\Python27\Scripts`).
   Ajoutez le dossier contenant le fichier `az.bat` à votre chemin d’accès.
   
4. Exécutez Azure CLI 2.0 à partir de l’invite de commandes avec la commande `az`.

> [!NOTE]
> Si vous avez déjà installé Azure CLI 2.0 et que vous voulez savoir si vous disposez de la dernière version, exécutez la commande `az --version` pour connaître la version que vous utilisez.
> Comparez cette version avec la dernière version disponible sur le site [https://pypi.python.org/pypi/azure-cli](https://pypi.python.org/pypi/azure-cli).
> 
> Pour mettre à jour l’interface de ligne de commande avec la dernière version, exécutez `az component update`.
> 
> Pour désinstaller l’interface, exécutez `pip uninstall azure-cli`.

## <a name="linux"></a>Linux

1. Sur Linux, vous pouvez avoir besoin d’installer des [composants requis](#linux-prerequisites) spécifiques.

2. Installez Azure CLI 2.0 avec une commande `curl`.

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

3. Vous devrez peut-être redémarrer votre interface de commande pour que certaines modifications soient prises en compte.

   ```bash
   exec -l $SHELL
   ```

4. Exécutez Azure CLI 2.0 à partir de l’invite de commandes avec la commande `az`.

> [!Note]
> Lorsque vous effectuez l’installation avec InstallAzureCli, `az component update` n’est pas pris en charge.
> Pour mettre à jour l’interface de ligne de commande avec la dernière version, ré-exécutez `curl -L https://aka.ms/InstallAzureCli | bash`.
> 
> Pour désinstaller l’interface, reportez-vous aux [instructions de désinstallation manuelle](#uninstall).

## <a name="docker"></a>Docker

Nous fournissons une image Docker préconfigurée avec l’interface de ligne de commande Azure.

Installez l’interface de ligne de commande Azure à l’aide de la commande `docker run`.

```bash
docker run azuresdk/azure-cli-python:<version>
```

Consultez nos [balises Docker](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/) pour connaître les versions disponibles.

> [!NOTE]
> Si vous souhaitez sélectionner les clés SSH à partir de votre environnement utilisateur, vous pouvez utiliser `-v ${HOME}:/root` pour monter $HOME en tant que `/root`.
>
> ```bash
> docker run -v ${HOME}:/root azuresdk/azure-cli-python:<version>
> ```

> [!NOTE]
> L’image Docker ne prend pas en charge la [fonctionnalité `component`](/cli/azure/component).
> Pour mettre à jour l’interface de ligne de commande avec la version Azure CLI 2.0, utilisez `docker run` afin d’installer la dernière image ou l’image qui vous intéresse.

## <a name="apt-get"></a>apt-get

Dans le cas des systèmes Debian/Ubuntu, vous pouvez installer Azure CLI 2.0 par le biais de la commande `apt-get`.

1. Modifiez votre liste de sources.

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

> [!NOTE]
> Lorsque vous effectuez l’installation avec apt-get, `az component` n’est pas pris en charge.
> Pour mettre à jour l’interface de ligne de commande, ré-exécutez `sudo apt-get update && sudo apt-get install azure-cli`.
> 
> Pour désinstaller l’interface, exécutez `sudo apt-get remove azure-cli`.

## <a name="linux-prerequisites"></a>Composants requis Linux

1. Installez [Python](https://www.python.org/downloads) si vous ne l’avez pas encore fait.

2. Selon votre distribution Linux, installez les composants requis.

   ```
   Platform              | Prerequisites
   ----------------------|---------------------------------------------
   Ubuntu 15.10 or 16.04 | sudo apt-get update && sudo apt-get install -y libssl-dev libffi-dev python-dev build-essential
   Ubuntu 12.04 or 14.04 | sudo apt-get update && sudo apt-get install -y libssl-dev libffi-dev python-dev
   Debian 8              | sudo apt-get update && sudo apt-get install -y libssl-dev libffi-dev python-dev build-essential
   Debian 7              | sudo apt-get update && sudo apt-get install -y libssl-dev libffi-dev python-dev
   CentOS 7.1 or 7.2     | sudo yum check-update; sudo yum install -y gcc libffi-devel python-devel openssl-devel
   RedHat 7.2            | sudo yum check-update; sudo yum install -y gcc libffi-devel python-devel openssl-devel
   SUSE OpenSUSE 13.2    | sudo zypper refresh && sudo zypper --non-interactive install gcc libffi-devel python-devel openssl-devel
   ```

## <a name="troubleshooting"></a>Résolution des problèmes
-------------------------------

### <a name="errors-with-curl-redirection"></a>Erreurs de redirection curl

Si la commande `curl` renvoie une erreur concernant le paramètre `-L` ou un message d’erreur « Objet déplacé », essayez d’utiliser l’URL complète plutôt que l’URL aka.ms :

```
# If you see this:
curl -L https://aka.ms/InstallAzureCli | bash
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100   175  100   175    0     0    562      0 --:--:-- --:--:-- --:--:--   560
bash: line 1: syntax error near unexpected token `<'
'ash: line 1: `<html><head><title>Object moved</title></head><body>

#### Try this instead:
curl https://azurecliprod.blob.core.windows.net/install | bash
```


### <a name="errors-on-install-with-cffi-or-cryptography"></a>Erreurs d’installation avec `cffi` ou de chiffrement

Si vous obtenez des erreurs lors de l’installation sur OS X, mettez à niveau `pip`.

```bash
pip install --upgrade --force-reinstall pip
```

Si vous obtenez des erreurs dans le cadre de l’installation sur **Debian** ou **Ubuntu**, comme dans les exemples ci-après, installez `libssl-dev` et `libffi-dev`.

```bash
sudo apt-get update
sudo apt-get install -y libssl-dev libffi-dev
```

Installez également Python Dev pour votre version de Python.

Python 2 :

```bash
sudo apt-get install -y python-dev
```

Python 3 :

```bash
sudo apt-get install -y python3-dev
```

Ubuntu 15 peut également nécessiter `build-essential` :

```bash
sudo apt-get install -y build-essential
```

### <a name="example-errors"></a>Exemples d’erreurs

```
Downloading cffi-1.5.2.tar.gz (388kB)
    100% |################################| 389kB 3.9MB/s
    Complete output from command python setup.py egg_info:

        No working compiler found, or bogus compiler options
        passed to the compiler from Python's distutils module.
        See the error messages above.
        (If they are about -mno-fused-madd and you are on OS/X 10.8,
        see http://stackoverflow.com/questions/22313407/ .)

    ----------------------------------------
Command "python setup.py egg_info" failed with error code 1 in /tmp/pip-build-77i2fido/cffi/
```

```
#include <openssl/e_os2.h>
                            ^
compilation terminated.
error: command 'x86_64-linux-gnu-gcc' failed with exit status 1

Failed building wheel for cryptography
```

Reportez-vous à la question du site Stack Overflow : [Failed to install Python Cryptography package with PIP and setup.py](http://stackoverflow.com/questions/22073516/failed-to-install-python-cryptography-package-with-pip-and-setup-py) (Échec de l’installation du package de chiffrement de Python avec PIP et setup.py).

## <a name="uninstall"></a>Désinstaller l’interface

Si vous avez installé l’interface de ligne de commande en utilisant le script accessible à l’adresse https://aka.ms/InstallAzureCli, vous pouvez désinstaller l’interface à l’aide de la procédure suivante.

1. Supprimez les fichiers installés.

   ```bash
   rm -r <install location>/lib/azure-cli
   rm <install location>/bin/az
   ```

2. Supprimez la ligne `<install location>/lib/azure-cli/az.completion` de `<install location>/.bash_profile`.

> [!Note]
> L’emplacement d’installation par défaut est `/Users/<username>`.

Si vous avez utilisé pip, apt-get ou Docker pour installer l’interface de ligne de commande, utilisez le même outil pour désinstaller l’interface.

## <a name="reporting-issues-and-feedback"></a>Signalement de problèmes et envoi de commentaires

Si vous rencontrez des bogues en utilisant l’outil, signalez un problème dans la section [Issues](https://github.com/Azure/azure-cli/issues) (Problèmes) de notre référentiel GitHub.
Pour fournir des commentaires à partir de la ligne de commande, essayez la commande `az feedback`.
