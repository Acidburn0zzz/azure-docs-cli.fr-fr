---
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 09/29/2020
ms.topic: include
ms.custom: devx-track-azurecli
ms.openlocfilehash: caf16d07ba6bbf6010a3e8e01ef6b49108853566
ms.sourcegitcommit: bd2dbc80328936dadd211764d25c32a14fc58083
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/04/2021
ms.locfileid: "97858027"
---
## <a name="overview"></a>Vue d’ensemble

Le gestionnaire de package `apt` contient un package x86_64 pour Azure CLI qui a été testé sur les distributions suivantes.

| Distribution | Version |
|:-------------|:--------|
| Ubuntu       | 14.04 LTS (Trusty Tahir), 16.04 LTS (Xenial Xerus), 18.04 LTS (Bionic Beaver), 19.10 (Eoan Ermine), 20.04 LTS (Focal Fossa) |
| Debian       | Debian 8 (Jessie), Debian 9 (Stretch), Debian 10 (Buster) |

> [!WARNING]
> Ubuntu 20.04 (Focal Fossa) inclut un package `azure-cli` avec la version `2.0.81` fourni par le référentiel `focal/universe`. Ce package est obsolète et n’est pas recommandé. Si ce package est installé, exécutez la commande `sudo apt remove azure-cli -y && sudo apt autoremove -y` pour le supprimer avant de continuer.

## <a name="installation-options"></a>Options d'installation

Pour installer Azure CLI sur votre système, deux options s’offrent à vous.  Vous pouvez soit exécuter une seule commande qui télécharge un script d’installation et exécute les commandes d’installation pour vous,  soit exécuter les commandes d’installation vous-même dans un processus pas à pas.  Les deux méthodes sont présentées ci-dessous.

## <a name="option-1-install-with-one-command"></a>Option 1 : Installer avec une seule commande

L’équipe d’Azure CLI propose un script qui permet d’exécuter toutes les commandes d’installation en une seule étape.  Ce script, à télécharger avec `curl`, est dirigé directement vers `bash` pour installer l’interface CLI.

Si vous souhaitez inspecter le contenu du script avant de l’exécuter, téléchargez-le avec `curl` et examinez-le dans votre éditeur de texte favori.

```bash
curl -sL https://aka.ms/InstallAzureCLIDeb | sudo bash
```

## <a name="option-2-step-by-step-installation-instructions"></a>Option n°2 : Instructions d’installation pas à pas

Si vous préférez suivre un processus d’installation pas à pas, effectuez les étapes suivantes pour installer Azure CLI.

1. Obtenez les packages nécessaires pour le processus d’installation :

    ```bash
    sudo apt-get update
    sudo apt-get install ca-certificates curl apt-transport-https lsb-release gnupg
    ```

2. Téléchargez et installez la clé de signature Microsoft :

    ```bash
    curl -sL https://packages.microsoft.com/keys/microsoft.asc |
        gpg --dearmor |
        sudo tee /etc/apt/trusted.gpg.d/microsoft.gpg > /dev/null
    ```

3. <div id="set-release"/>Ajoutez le référentiel de logiciels Azure CLI (ignorez cette étape sur les distributions Linux ARM64) :

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

## <a name="sign-in-to-azure-with-the-azure-cli"></a>Se connecter à Azure avec Azure CLI

Exécutez Azure CLI avec la commande `az`. Pour vous connecter, utilisez la commande [az login](/cli/azure/reference-index#az-login).

[!INCLUDE [interactive-login](interactive-login.md)]

Pour en savoir plus sur les différentes méthodes d’authentification, consultez [Se connecter avec Azure CLI](../authenticate-azure-cli.md).

## <a name="troubleshooting"></a>Dépannage

Voici certains problèmes courants lors de l’installation avec `apt`. Si vous rencontrez un problème n’étant pas évoqué ici, [signalez un problème sur github](https://github.com/Azure/azure-cli/issues).

### <a name="no-module-issue-on-ubuntu-2004-focalwsl"></a>Aucun problème de module sur Ubuntu 20.04 (Focal)/WSL

Si vous avez installé `azure-cli` sur `Focal` sans ajouter le référentiel de logiciels Azure CLI dans l’[étape 3](#set-release) des instructions d’installation manuelle ou si vous utilisez notre [script](#option-1-install-with-one-command), vous pouvez rencontrer des problèmes tels qu’aucun module nommé « decorator » ou « antlr4 », car le package que vous avez installé est le package `azure-cli 2.0.81` obsolète du référentiel `focal/universe`. Commencez par le supprimer en exécutant `sudo apt remove azure-cli -y && sudo apt autoremove -y`, puis suivez les [instructions](#install) ci-dessus pour installer le dernier package `azure-cli`.

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

[!INCLUDE[configure-proxy](configure-proxy.md)]

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

[!INCLUDE[troubleshoot-wsl.md](troubleshoot-wsl.md)]

## <a name="update"></a>Update
[!INCLUDE [az-upgrade](az-upgrade.md)]

Vous pouvez aussi utiliser `apt-get upgrade` pour mettre à jour le package CLI.

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

[!INCLUDE [uninstall-boilerplate.md](uninstall-boilerplate.md)]

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
    sudo rm /etc/apt/trusted.gpg.d/microsoft.gpg
    ```

4. Supprimer tous les packages inutiles :

   ```bash
   sudo apt autoremove
   ```
