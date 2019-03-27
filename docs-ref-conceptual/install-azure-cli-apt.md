---
title: Installer Azure CLI sur Linux avec apt
description: Comment installer Azure CLI avec le gestionnaire de package apt
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 03/19/2019
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: fa2e1db439b4836d7506409b3abcce74fb6e6695
ms.sourcegitcommit: 5864f72b9a6fbf82a4d98bf805b3a16a7da18556
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/22/2019
ms.locfileid: "58343143"
---
# <a name="install-azure-cli-with-apt"></a>Installer Azure CLI avec apt

Si vous exécutez une distribution qui est fournie avec `apt`, telle que Ubuntu ou Debian, un package x86_64 est disponible pour Azure CLI. Ce package a été testé avec :

* Ubuntu trusty, xenial, artful et bionic
* Debian wheezy, jessie, et stretch

[!INCLUDE [current-version](includes/current-version.md)]

> [!NOTE]
>
> Le package Azure CLI installe son propre interpréteur Python et n’utilise pas le système Python.

## <a name="install"></a>Installer

1. Récupérez les packages nécessaires au processus d’installation :

    ```bash
    sudo apt-get update
    sudo apt-get install curl apt-transport-https lsb-release gpg
    ```

2. Téléchargez et installez la clé de signature Microsoft :

    ```bash
    curl -sL https://packages.microsoft.com/keys/microsoft.asc | \
        gpg --dearmor | \
        sudo tee /etc/apt/trusted.gpg.d/microsoft.asc.gpg > /dev/null
    ```

3. <div id="set-release"/>Ajoutez le référentiel de logiciels Azure CLI :

    ```bash
    AZ_REPO=$(lsb_release -cs)
    echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
    ```

4. Mettez à jour les informations concernant le référentiel, puis installez le package `azure-cli` :

    ```bash
    sudo apt-get update
    sudo apt-get install azure-cli
    ```

Exécutez Azure CLI avec la commande `az`. Pour vous connecter, utilisez la commande [az login](/cli/azure/reference-index#az-login).

[!INCLUDE [interactive-login](includes/interactive-login.md)]

Pour en savoir plus sur les différentes méthodes d’authentification, consultez [Se connecter avec Azure CLI](authenticate-azure-cli.md).

## <a name="troubleshooting"></a>Résolution de problèmes

Voici certains problèmes courants lors de l’installation avec `apt`. Si vous rencontrez un problème n’étant pas évoqué ici, [signalez un problème sur github](https://github.com/Azure/azure-cli/issues).

### <a name="lsbrelease-does-not-return-the-correct-base-distribution-version"></a>lsb_release ne renvoie pas la bonne version de la distribution de base

Certaines distributions Ubuntu ou Debian dérivées, telles que Linux Mint peuvent ne pas retourner le nom de version correct de `lsb_release`. Cette valeur est utilisée dans le processus d’installation pour déterminer le package à installer. Si vous connaissez le nom de code de la version Ubuntu ou Debian dont votre distribution est dérivée, vous pouvez définir la valeur `AZ_REPO` manuellement lors de l’[ajout du référentiel](#set-release). Dans le cas contraire, recherchez des informations expliquant comment déterminer le nom de code de la distribution de base et définir `AZ_REPO` sur la valeur appropriée.

### <a name="no-package-for-your-distribution"></a>Aucun package pour votre distribution

Après la publication d’une distribution, il peut se passer un certain temps avant que le package Azure CLI associé ne soit disponible. Azure CLI est conçu pour résister à de futures versions de dépendances, et repose sur peu d’entre elles. Si aucun package n’est disponible pour votre distribution de base, essayez d’utiliser le package d’une distribution antérieure.

Pour cela, définissez la valeur de `AZ_REPO` manuellement lors de l’[ajout du référentiel](#set-release). Pour les distributions Ubuntu, utilisez le référentiel `bionic`, et `stretch` pour les distributions Debian. Les distributions publiées avant Ubuntu Trusty et Debian Wheezy ne sont pas prises en charge.

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="update"></a>Mettre à jour

Utilisez `apt-get upgrade` pour mettre à jour le package de l’interface de ligne de commande.

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> Cette commande met à niveau tous les packages installés sur votre système n’ayant pas de modification de dépendance.
> Pour mettre à niveau uniquement l’interface CLI, utilisez `apt-get install`.
> 
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

## <a name="uninstall"></a>Désinstaller l’interface

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. Désinstaller avec `apt-get remove` :

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. Si vous ne prévoyez pas de réinstaller l’interface CLI, supprimez les informations de référentiel Azure CLI :

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. Supprimer la clé de signature :

    ```bash
    sudo rm /etc/apt/trusted.gpg.d/microsoft.asc.gpg
    ```

4. Supprimer tous les packages inutiles :

   ```bash
   sudo apt autoremove
   ```

## <a name="next-steps"></a>Étapes suivantes

Maintenant que vous avez installé l’interface CLI, découvrez ses fonctionnalités et ses commandes courantes.

> [!div class="nextstepaction"]
> [Prise en main de l’interface Azure CLI](get-started-with-azure-cli.md)
