---
title: Installer Azure CLI sur Linux avec apt
description: Comment installer Azure CLI avec le gestionnaire de package apt
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 10/14/2019
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 302b98717ee422de9bd60a57b18d900bcf5fcaf9
ms.sourcegitcommit: b5ecfc168489cd0d96462d6decf83e8b26a10194
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/31/2020
ms.locfileid: "80417919"
---
# <a name="install-azure-cli-with-apt"></a>Installer Azure CLI avec apt

Si vous exécutez une distribution qui est fournie avec `apt`, telle que Ubuntu ou Debian, un package x86_64 est disponible pour Azure CLI. Ce package a été testé avec les systèmes pris en charge suivants :

* Ubuntu trusty, xenial, artful, bionic et disco
* Debian wheezy, jessie, stretch et buster

[!INCLUDE [current-version](includes/current-version.md)]

> [!NOTE]
>
> Le package Azure CLI installe son propre interpréteur Python et n’utilise pas le système Python.

## <a name="install"></a>Installer

Pour installer Azure CLI avec les distributions prenant en charge `apt`, vous pouvez soit utiliser un script tout-en-un qui exécute les commandes d’installation pour vous, soit suivre vous-même les instructions d’un processus étape par étape.

### <a name="install-with-one-command"></a>Installer avec une seule commande

Nous vous proposons un script à jour qui exécute toutes les commandes d’installation en une seule étape. Pour l’exécuter, utilisez le pipe pour associer `curl` directement à `bash`, ou téléchargez le script dans un fichier et vérifiez-le avant de l’exécuter.

> [!IMPORTANT]
> Ce script a été uniquement validé sur Ubuntu 16.04 et Debian 8+. Il est possible qu’il ne fonctionne pas sur d’autres distributions.
> Si vous utilisez une distribution dérivée telle que Linux Mint, suivez les instructions d’installation manuelle et effectuez les opérations de dépannage nécessaires.

```bash
curl -sL https://aka.ms/InstallAzureCLIDeb | sudo bash
```

### <a name="manual-install-instructions"></a>Instructions d’installation manuelle

Si vous ne souhaitez pas exécuter un script en tant que superutilisateur ou que le script tout-en-un échoue, suivez ces étapes pour installer Azure CLI.

1. Obtenez les packages nécessaires pour le processus d’installation :

    ```bash
    sudo apt-get update
    sudo apt-get install ca-certificates curl apt-transport-https lsb-release gnupg
    ```

2. Téléchargez et installez la clé de signature Microsoft :

    ```bash
    curl -sL https://packages.microsoft.com/keys/microsoft.asc |
        gpg --dearmor |
        sudo tee /etc/apt/trusted.gpg.d/microsoft.asc.gpg > /dev/null
    ```

3. <div id="set-release"/>Ajoutez le référentiel de logiciels Azure CLI :

    ```bash
    AZ_REPO=$(lsb_release -cs)
    echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" |
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

## <a name="troubleshooting"></a>Dépannage

Voici certains problèmes courants lors de l’installation avec `apt`. Si vous rencontrez un problème n’étant pas évoqué ici, [signalez un problème sur github](https://github.com/Azure/azure-cli/issues).

### <a name="lsb_release-does-not-return-the-correct-base-distribution-version"></a>lsb_release ne renvoie pas la bonne version de la distribution de base

Certaines distributions Ubuntu ou Debian dérivées, telles que Linux Mint peuvent ne pas retourner le nom de version correct de `lsb_release`. Cette valeur est utilisée dans le processus d’installation pour déterminer le package à installer. Si vous connaissez le nom de code de la version Ubuntu ou Debian dont votre distribution est dérivée, vous pouvez définir la valeur `AZ_REPO` manuellement lors de l’[ajout du référentiel](#set-release). Dans le cas contraire, recherchez des informations expliquant comment déterminer le nom de code de la distribution de base et définir `AZ_REPO` sur la valeur appropriée.

### <a name="no-package-for-your-distribution"></a>Aucun package pour votre distribution

Après la publication d’une distribution, il peut se passer un certain temps avant que le package Azure CLI associé ne soit disponible. Azure CLI est conçu pour résister à de futures versions de dépendances, et repose sur peu d’entre elles. Si aucun package n’est disponible pour votre distribution de base, essayez d’utiliser le package d’une distribution antérieure.

Pour cela, définissez la valeur de `AZ_REPO` manuellement lors de l’[ajout du référentiel](#set-release). Pour les distributions Ubuntu, utilisez le référentiel `bionic`, et `stretch` pour les distributions Debian. Les distributions publiées avant Ubuntu Trusty et Debian Wheezy ne sont pas prises en charge.

### <a name="elementary-os-eos-fails-to-install-the-azure-cli"></a>Le système d’exploitation élémentaire (EOS, elementary OS) ne parvient pas à installer Azure CLI

EOS ne parvient pas à installer Azure CLI parce que `lsb_release` retourne `HERA`, qui est le nom de la version EOS.  La solution consiste à corriger le fichier `/etc/apt/sources.list.d/azure-cli.list` et à remplacer `hera main` par `bionic main`.

Contenu du fichier d’origine :

```
deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ hera main
```

Contenu du fichier modifié

```
deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ bionic main
```

### <a name="proxy-blocks-connection"></a>Le proxy bloque la connexion

[!INCLUDE[configure-proxy](includes/configure-proxy.md)]

Vous pouvez également configurer de manière explicite `apt` pour utiliser ce proxy à tout moment. Vérifiez que les lignes suivantes s’affichent dans un fichier de configuration `apt` dans `/etc/apt/apt.conf.d/`. Nous vous recommandons d’utiliser votre fichier de configuration global existant, un fichier de configuration de proxy existant, `40proxies` ou `99local`. Mais suivez vos besoins d’administration système.

```apt.conf
Acquire {
    http::proxy "http://[username]:[password]@[proxy]:[port]";
    https::proxy "https://[username]:[password]@[proxy]:[port]";
}
```

Si votre proxy n’utilise pas l’authentification de base, __supprimez__ la partie `[username]:[password]@` de l’URI du proxy. Si vous avez besoin de plus d’informations sur la configuration du proxy, consultez la documentation officielle Ubuntu :

* [apt.conf manpage](http://manpages.ubuntu.com/manpages/bionic/en/man5/apt.conf.5.html)
* [Ubuntu wiki - apt-get howto](https://help.ubuntu.com/community/AptGet/Howto#Setting_up_apt-get_to_use_a_http-proxy)

Pour obtenir la clé de signature Microsoft et obtenir le package à partir de notre dépôt, votre proxy doit autoriser les connexions HTTPS à l’adresse suivante :

* `https://packages.microsoft.com`

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="update"></a>Update

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

3. Si vous n’utilisez pas d’autres packages de Microsoft, supprimez la clé de signature :

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
