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
ms.openlocfilehash: 7065ed5270ef9bfc70beea81d0bc442a7b4df38c
ms.sourcegitcommit: c077bd5cbe07f7225714c41714d3981fa0d9928f
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/16/2017
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

Vous pouvez installer l’interface de ligne de commande avec le MSI et l’utiliser dans la ligne de commande Windows, ou vous pouvez installer l’interface de ligne de commande avec apt-get avec Bash sur Ubuntu sous Windows.

### <a name="msi-for-the-windows-command-line"></a>MSI pour la ligne de commande Windows 

Pour installer l’interface de ligne de commande sous Windows et l’utiliser dans la ligne de commande Windows, téléchargez et exécutez le [msi](https://aka.ms/InstallAzureCliWindows).

> [!NOTE]
> Lorsque vous installez le msi, `az component` n’est pas pris en charge.
> Pour mettre à jour vers l’interface de ligne de commande la plus récente, réexécutez le [msi](https://aka.ms/InstallAzureCliWindows).
> 
> Pour désinstaller l’interface de ligne de commande, réexécutez le [msi](https://aka.ms/InstallAzureCliWindows) et choisissez Désinstaller.

### <a name="apt-get-for-bash-on-ubuntu-on-windows"></a>apt-get pour Bash sur Ubuntu sous Windows

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

> [!NOTE]
> Lorsque vous effectuez l’installation avec apt-get, `az component` n’est pas pris en charge.
> Pour mettre à jour l’interface de ligne de commande, ré-exécutez `sudo apt-get update && sudo apt-get install azure-cli`.
> 
> Pour désinstaller l’interface, exécutez `sudo apt-get remove azure-cli`.

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

Si vous avez utilisé apt-get, Docker ou le msi pour installer l’interface de ligne de commande, utilisez le même outil pour la désinstaller.

## <a name="reporting-issues-and-feedback"></a>Signalement de problèmes et envoi de commentaires

Si vous rencontrez des bogues en utilisant l’outil, signalez un problème dans la section [Issues](https://github.com/Azure/azure-cli/issues) (Problèmes) de notre référentiel GitHub.
Pour fournir des commentaires à partir de la ligne de commande, essayez la commande `az feedback`.
