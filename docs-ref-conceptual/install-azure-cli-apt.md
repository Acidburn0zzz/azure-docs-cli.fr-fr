---
title: Installer Azure CLI sur Linux avec apt
description: Comment installer Azure CLI avec le gestionnaire de package apt
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 11/27/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 45e1e7468e5817d0138c9b87da83c5a5228e4965
ms.sourcegitcommit: 1987a39809f9865034b27130e56f30b2bd1eb72c
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/19/2019
ms.locfileid: "56421930"
---
# <a name="install-azure-cli-with-apt"></a>Installer Azure CLI avec apt

Si vous exécutez une distribution qui est fournie avec `apt`, telle que Ubuntu ou Debian, un package 64 bits est disponible pour Azure CLI. Ce package a été testé avec :

* Ubuntu trusty, xenial, artful et bionic
* Debian wheezy, jessie, et stretch

[!INCLUDE [current-version](includes/current-version.md)]

> [!NOTE]
>
> Dans la mesure où le package `.deb` d’Azure CLI installe son propre interpréteur Python et n’utilise pas le système Python, aucune version explicite n’est nécessaire pour une version Python locale.

## <a name="install"></a>Installer

1. Installez les packages prérequis :

    ```bash
    sudo apt-get install apt-transport-https lsb-release software-properties-common dirmngr -y
    ```

2. <div id="set-release"/>Modifiez votre liste de sources :

    ```bash
    AZ_REPO=$(lsb_release -cs)
    echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
    ```

3. <div id="signingKey"/>Obtenir la clé de signature Microsoft :

   ```bash
   sudo apt-key --keyring /etc/apt/trusted.gpg.d/Microsoft.gpg adv \
        --keyserver packages.microsoft.com \
        --recv-keys BC528686B50D79E339D3721CEB3E94ADBE1229CF
   ```

4. Installer l’interface de ligne de commande :

   ```bash
   sudo apt-get update
   sudo apt-get install azure-cli
   ```

   > [!WARNING]
   > La clé de signature a été mise à jour en mai 2018 et a été remplacée. Si vous recevez des erreurs de signature, veillez à disposer de la [dernière clé de signature](#signingKey).

Vous pouvez ensuite exécuter l’interface de ligne de commande Azure avec la commande `az`. Pour vous connecter, utilisez la commande [az login](/cli/azure/reference-index#az-login).

[!INCLUDE [interactive-login](includes/interactive-login.md)]

Pour en savoir plus sur les différentes méthodes d’authentification, consultez [Se connecter avec Azure CLI](authenticate-azure-cli.md).

## <a name="troubleshooting"></a>Résolution de problèmes

Voici certains problèmes courants lors de l’installation avec `apt`. Si vous rencontrez un problème n’étant pas évoqué ici, [signalez un problème sur github](https://github.com/Azure/azure-cli/issues).

### <a name="lsbrelease-does-not-return-the-correct-base-distribution-version"></a>lsb_release ne renvoie pas la bonne version de la distribution de base

Certaines distributions Ubuntu ou Debian dérivées, telles que Linux Mint peuvent ne pas retourner le nom de version correct de `lsb_release`. Cette valeur est utilisée dans le processus d’installation pour déterminer le package à installer. Si vous connaissez le nom de la version dont votre distribution est dérivée, vous pouvez définir la valeur `AZ_REPO` manuellement à [l’étape 2 de l’installation](#set-release). Dans le cas contraire, recherchez des informations concernant votre distribution, sur la façon de déterminer le nom de la distribution de base et de définir `AZ_REPO` sur la valeur correcte.

### <a name="no-package-for-your-distribution"></a>Aucun package pour votre distribution

La disponibilité d’un package Azure CLI pour une distribution Ubuntu après sa publication peut parfois prendre un certain temps. Azure CLI est conçu pour résister à de futures versions de dépendances, et repose sur peu d’entre elles. Si aucun package n’est disponible pour votre distribution de base, essayez d’utiliser le package d’une distribution antérieure.

Pour ce faire, définissez manuellement la valeur de `AZ_REPO` dans [ étape 1 Installer](#install-step-1). Pour les distributions Ubuntu, utilisez le référentiel `bionic`, et `stretch` pour les distributions Debian. Les distributions publiées avant Ubuntu Trusty et Debian Wheezy ne sont pas prises en charge.

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

Si vous êtes sur le sous-système Windows pour Linux (WSL), cette erreur apparaît également sur les versions de Windows antérieures à Windows 10 1809. Pour résoudre ce problème, mettez à jour votre version de Windows.

### <a name="apt-key-hangs"></a>apt-key se bloque

Lorsqu’un pare-feu bloque les connexions sortantes au port 11371, la commande `apt-key` peut se bloquer indéfiniment.
Votre pare-feu peut nécessiter l’utilisation d’un proxy HTTP pour les connexions sortantes :

```bash
sudo apt-key --keyring /etc/apt/trusted.gpg.d/Microsoft.gpg adv \
    --keyserver-options http-proxy=http://<USER>:<PASSWORD>@<PROXY-HOST>:<PROXY-PORT>/ \
    --keyserver packages.microsoft.com \
    --recv-keys BC528686B50D79E339D3721CEB3E94ADBE1229CF
```

Pour vous assurer que vous disposez d’un proxy, contactez votre administrateur système. Si votre proxy ne nécessite pas de connexion, ignorez les informations d’utilisateur et de mot de passe.

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="update"></a>Mettre à jour

Utilisez `apt-get upgrade` pour mettre à jour le package de l’interface de ligne de commande.

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!WARNING]
> La clé de signature a été mise à jour en mai 2018 et a été remplacée. Si vous recevez des erreurs de signature, veillez à disposer de la [dernière clé de signature](#signingKey).
>
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
    sudo rm /etc/apt/trusted.gpg.d/Microsoft.gpg
    ```

4. Supprimer tous les packages inutiles :

   ```bash
   sudo apt autoremove
   ```

## <a name="next-steps"></a>Étapes suivantes

Maintenant que vous avez installé l’interface CLI, découvrez ses fonctionnalités et ses commandes courantes.

> [!div class="nextstepaction"]
> [Prise en main de l’interface Azure CLI](get-started-with-azure-cli.md)
