---
title: Installez Azure CLI sur Linux avec zypper
description: Comment installer Azure CLI avec zypper
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: f8a3bec4fffb731c6521fa7b8a2a90798ef191e6
ms.sourcegitcommit: 08043c47d3ccf23522b91e6bba3932e312c04c7f
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/04/2019
ms.locfileid: "66516241"
---
# <a name="install-azure-cli-with-zypper"></a>Installez Azure CLI avec zypper

Pour les distributions Linux avec `zypper`, telles que openSUSE ou SLES, un package est disponible pour l’Azure CLI. Ce package a été testé avec openSUSE 42.2 et ultérieur et SLES 12 SP 2 et ultérieur.

[!INCLUDE [current-version](includes/current-version.md)]

[!INCLUDE [rpm-warning](includes/rpm-warning.md)]

## <a name="install"></a>Installer

1. Installez `curl` :

   ```bash
   sudo zypper install -y curl
   ```

2. Importer la clé de référentiel Microsoft :

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

3. Créer des informations de référentiel `azure-cli` locales :

   ```bash
   sudo zypper addrepo --name 'Azure CLI' --check https://packages.microsoft.com/yumrepos/azure-cli azure-cli
   ```

4. Mettre à jour l’index de package `zypper` et l’installer :

   ```bash
   sudo zypper install --from azure-cli -y azure-cli
   ```

Vous pouvez ensuite exécuter l’interface de ligne de commande Azure avec la commande `az`. Pour vous connecter, utilisez la commande [az login](/cli/azure/reference-index#az-login).

[!INCLUDE [interactive-login](includes/interactive-login.md)]

Pour en savoir plus sur les différentes méthodes d’authentification, consultez [Se connecter avec Azure CLI](authenticate-azure-cli.md).

## <a name="troubleshooting"></a>Résolution de problèmes

Voici certains problèmes courants lors de l’installation avec `zypper`. Si vous rencontrez un problème n’étant pas évoqué ici, [signalez un problème sur github](https://github.com/Azure/azure-cli/issues).

### <a name="proxy-blocks-connection"></a>Le proxy bloque la connexion

[!INCLUDE[configure-proxy](includes/configure-proxy.md)]

Vous pouvez également configurer de manière explicite `zypper` (via `yast2`) pour utiliser ce proxy à tout moment. Pour ce faire, exécutez la commande `yast2 proxy` en tant que superutilisateur et remplissez les informations présentées dans le formulaire. Si vous avez un gestionnaire de fenêtres disponible sur votre système, vous pouvez également utiliser le volet `Network Services > Proxy` dans le `YaST Control Center`.

Pour la configuration avancée ou plus d’informations, consultez la [documentation de configuration de proxy OpenSUSE](https://www.suse.com/documentation/slms1/book_slms/data/sec_wy_config_updates_proxy.html)

Pour obtenir la clé de signature Microsoft et obtenir le package à partir de notre dépôt, votre proxy doit autoriser les connexions HTTPS aux adresses suivantes :

* `https://packages.microsoft.com`
* `https://download.opensuse.org`

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

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

2. Si vous ne prévoyez pas de réinstaller l’interface CLI, supprimez les informations de référentiel.

   ```bash
   sudo zypper removerepo azure-cli
   ```

3. Si vous avez supprimé les informations de référentiel, supprimez également la clé de signature Microsoft GPG.

   ```bash
   MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
   sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
   ```

## <a name="next-steps"></a>Étapes suivantes

Maintenant que vous avez installé l’interface CLI, découvrez ses fonctionnalités et ses commandes courantes.

> [!div class="nextstepaction"]
> [Prise en main de l’interface Azure CLI](get-started-with-azure-cli.md)
