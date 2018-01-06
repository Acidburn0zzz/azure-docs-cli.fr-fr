---
title: Installer Azure CLI 2.0 avec apt
description: "Installation d’Azure CLI 2.0 avec le gestionnaire de package apt"
keywords: "Azure CLI, installation d’Azure CLI, Azure apt, Azure Debian, Azure Ubuntu"
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
ms.openlocfilehash: 75c531a13a4b730158cd2e874cb6c5d581a27598
ms.sourcegitcommit: 2e4d0bdd94c626e061434883032367b5619de4fe
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/09/2017
---
# <a name="install-azure-cli-20-with-apt"></a>Installer Azure CLI 2.0 avec apt

Si vous exécutez une distribution qui est fournie avec `apt`, telle que Ubuntu ou Debian, vous pouvez installer un package pour l’interface de ligne de commande Azure sur votre système.

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a>Installer

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
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

Vous pouvez exécuter l’interface de ligne de commande Azure avec la commande `az`.

## <a name="update"></a>Mettre à jour

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

### <a name="uninstall"></a>Désinstaller l’interface

Si jamais vous décidez de désinstaller l’interface de ligne de commande Azure, nous sommes désolés de vous voir partir. Avant de désinstaller, utilisez la commande `az feedback`, afin de nous donner quelques raisons pour lesquelles vous avez choisi de désinstaller et nous aider à améliorer l’expérience CLI. Nous souhaitons nous assurer que l’interface de ligne de commande Azure est aussi conviviale et exempte de bogues que possible. Vous pouvez également [signaler un problème lié à GitHub](https://github.com/Azure/azure-cli/issues).

1. Désinstaller avec `apt-get remove`.

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. Si vous ne souhaitez pas réinstaller l’interface de ligne de commande, supprimez les informations de référentiel Azure CLI.

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. Supprimez tous les packages inutiles.

   ```bash
   sudo apt autoremove
   ```
