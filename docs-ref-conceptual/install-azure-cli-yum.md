---
title: Installer Azure CLI 2.0 avec yum
description: "Installation d’Azure CLI 2.0 avec yum"
keywords: "Azure CLI, installation d’Azure CLI, Azure yum, Azure RHEL, Azure Fedora, Azure CentOS"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 11/01/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ROBOTS: NOINDEX,NOFOLLOW
ms.openlocfilehash: f0d5effcd8315094b30050a35119e41eddf89961
ms.sourcegitcommit: 2e4d0bdd94c626e061434883032367b5619de4fe
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/09/2017
---
# <a name="install-azure-cli-20-with-yum"></a>Installer Azure CLI 2.0 avec yum

Si vous exécutez une distribution qui est fournie avec `yum`, telle que RHEL, Fedora, ou CentOS, vous pouvez installer un package pour l’interface de ligne de commande Azure sur votre système.

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

Si jamais vous décidez de désinstaller l’interface de ligne de commande Azure, nous sommes désolés de vous voir partir. Avant de désinstaller, utilisez la commande `az feedback`, afin de nous donner quelques raisons pour lesquelles vous avez choisi de désinstaller et nous aider à améliorer l’expérience CLI. Nous souhaitons nous assurer que l’interface de ligne de commande Azure est aussi conviviale et exempte de bogues que possible. Vous pouvez également [signaler un problème lié à GitHub](https://github.com/Azure/azure-cli/issues).

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
