---
title: "Installation d’Azure CLI 2.0 pour Linux avec zypper"
description: "Installation d’Azure CLI 2.0 avec zypper"
keywords: "Azure CLI, installation d’Azure CLI, Azure CLI zypper, Azure CLI opensuse, Azure CLI sle"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 01/29/18
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: c0b566f96e47d34d20f7bf85db0fae32913ed596
ms.sourcegitcommit: 8606f36963e8daa6448d637393d1e4ef2c9859a0
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/01/2018
---
# <a name="install-azure-cli-20-with-zypper"></a>Installer Azure CLI 2.0 avec zypper

Si vous exécutez une distribution qui est fournie avec `zypper`, telle que openSUSE ou SLES, un package est disponible pour l’interface de ligne de commande Azure. Ce package a été testé avec openSUSE 42.2 et SLES 12 SP 2.

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a>Installer

1. Installez `curl` :

   ```bash
   sudo zypper refresh
   sudo zypper install -y curl
   ```

2. Importer la clé de référentiel Microsoft :

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

3. Créer des informations de référentiel `azure-cli` locales :

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ntype=rpm-md\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/zypp/repos.d/azure-cli.repo'
   ```

4. Mettre à jour l’index de package `zypper` et l’installer :

   ```bash
   sudo zypper refresh
   sudo zypper install -y azure-cli
   ```

Vous pouvez exécuter l’interface de ligne de commande avec la commande `az`.

## <a name="update"></a>Mettre à jour

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

2. Si vous ne souhaitez pas réinstaller l’interface CLI, supprimez les informations de référentiel.

  ```bash
  sudo rm /etc/zypp/repos.d/azure-cli.repo
  ```

3. Si vous avez supprimé les informations de référentiel, supprimez également la clé de signature Microsoft GPG.

  ```bash
  MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
  sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
  ```

