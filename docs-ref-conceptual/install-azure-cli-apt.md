---
title: "Installation d’Azure CLI 2.0 pour Linux avec apt"
description: "Installation d’Azure CLI 2.0 avec le gestionnaire de package apt"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 02/06/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 4076fefb902a324f77f97bc042b9f5ba3e787734
ms.sourcegitcommit: b93a19222e116d5880bbe64c03507c64e190331e
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/15/2018
---
# <a name="install-azure-cli-20-with-apt"></a>Installer Azure CLI 2.0 avec apt

Si vous exécutez une distribution qui est fournie avec `apt`, telle que Ubuntu ou Debian, un package 64 bits est disponible pour l’interface de ligne de commande Azure. Ce package a été testé avec :

* Ubuntu wheezy, xenial, et artful
* Debian wheezy, jessie, et stretch

## <a name="install"></a>Installer

1. Modifiez votre liste de sources :

     ```bash
     AZ_REPO=$(lsb_release -cs)
     echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

2. Exécutez les commandes sudo suivantes :

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

Vous pouvez exécuter l’interface de ligne de commande Azure avec la commande `az`.

## <a name="troubleshooting"></a>Résolution de problèmes

Voici certains problèmes courants lors de l’installation avec `apt`. Si votre problème ne figure pas ici, veuillez [signaler le problème sur Github](https://github.com/Azure/azure-cli/issues).

### <a name="apt-key-fails-with-no-dirmngr"></a>Clé apt échoue avec le message « No dirmngr »

Lorsque vous exécutez la commande `apt-key`, vous pouvez voir une sortie similaire à l’erreur suivante :

```output
gpg: failed to start the dirmngr '/usr/bin/dirmngr': No such file or directory
gpg: connecting dirmngr at '/tmp/apt-key-gpghome.kt5zo27tp1/S.dirmngr' failed: No such file or directory
gpg: keyserver receive failed: No dirmngr
```

Cette erreur est due à un composant manquant requis par `apt-key`. Vous pouvez résoudre ce problème en installant le package `dirmngr`.

```bash
sudo apt-get install dirmngr
```

## <a name="update"></a>Mettre à jour

Utilisez `apt-get upgrade` pour mettre à jour le package de l’interface de ligne de commande.

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> Cette commande met à niveau tous les packages installés sur votre système n’ayant pas de modification de dépendance.
> Pour mettre à niveau uniquement l’interface CLI, utilisez `apt-get install`.
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

## <a name="uninstall"></a>Désinstaller l’interface

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

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
