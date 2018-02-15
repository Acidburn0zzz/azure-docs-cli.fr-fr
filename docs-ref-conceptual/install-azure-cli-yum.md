---
title: "Installation d’Azure CLI 2.0 pour Linux avec yum"
description: "Installation d’Azure CLI 2.0 avec yum"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 01/29/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 4b92499d2cb81f64bfbb13215428365711b07874
ms.sourcegitcommit: b93a19222e116d5880bbe64c03507c64e190331e
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/15/2018
---
# <a name="install-azure-cli-20-with-yum"></a>Installer Azure CLI 2.0 avec yum

Si vous exécutez une distribution qui est fournie avec `yum`, telle que RHEL, Fedora, ou CentOS, un package est disponible pour l’interface de ligne de commande Azure. Ce package a été testé avec RHEL 7, Fedora 19 et versions ultérieures et CentOS 7.

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a>Installer

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

Exécutez Azure CLI avec la commande `az`.

## <a name="update"></a>Mettre à jour

Mettre à jour Azure CLI avec la commande `yum update`.

```bash
yum check-update
sudo yum update azure-cli
```

## <a name="uninstall"></a>Désinstaller l’interface

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. Supprimez le package de votre système.

   ```bash
   sudo yum remove azure-cli
   ```

2. Si vous ne souhaitez pas réinstaller l’interface CLI, supprimez les informations de référentiel.

   ```bash
   sudo rm /etc/yum.repos.d/azure-cli.repo
   ```

3. Si vous avez supprimé les informations de référentiel, supprimez également la clé de signature Microsoft GPG.

  ```bash
  MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
  sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
  ```
