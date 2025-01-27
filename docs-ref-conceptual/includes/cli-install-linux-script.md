---
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 12/15/2020
ms.topic: include
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: d02856e18fcbf395bb6f304b3dea9a17a6dc0a2c
ms.sourcegitcommit: 8bff8b2ce4492ab99ad39390e4c802fb4f4425c8
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/26/2021
ms.locfileid: "105582348"
---
## <a name="overview"></a>Vue d’ensemble

> [!NOTE]
> Il est fortement recommandé d’installer l’interface CLI avec un gestionnaire de package. Un gestionnaire de package permet de s’assurer que vous obtenez toujours les dernières mises à jour et garantit la stabilité des composants de l’interface CLI. Vérifiez s’il existe un package pour votre distribution avant d’installer manuellement.

L’interface CLI requiert les logiciels suivants :

* [Python 3.6.x, 3.7.x ou 3.8.x](https://www.python.org/downloads/).
* [libffi](https://sourceware.org/libffi/)
* [OpenSSL 1.0.2](https://www.openssl.org/source/)

> [!IMPORTANT]
>
> L’interface CLI a retiré la prise en charge de Python 2.7 depuis la version `2.1.0`. Les nouvelles versions ne garantissent plus une exécution correcte de Python 2.7.

## <a name="install-or-update"></a>Installation ou mise à jour

L’installation et la mise à jour de l’interface CLI nécessitent toutes de réexécuter le script d’installation. Installez l’interface CLI en exécutant `curl`.

```bash
curl -L https://aka.ms/InstallAzureCli | bash
```

Le script peut également être téléchargé et exécuté localement. Vous devrez peut-être redémarrer votre interpréteur de commandes pour que certaines modifications soient prises en compte.

Vous pouvez ensuite exécuter l’interface de ligne de commande Azure avec la commande `az`. Pour vous connecter, utilisez la commande [az login](/cli/azure/reference-index#az_login).

[!INCLUDE [interactive-login](interactive-login.md)]

Pour en savoir plus sur les différentes méthodes d’authentification, consultez [Se connecter avec Azure CLI](../authenticate-azure-cli.md).

## <a name="troubleshooting"></a>Dépannage

Voici certains problèmes courants rencontrés pendant une installation manuelle. Si vous rencontrez un problème qui n’est pas traité ici, [signalez ce problème sur GitHub](https://github.com/Azure/azure-cli/issues).

### <a name="curl-object-moved-error"></a>erreur curl « Objet déplacé »

Si la commande `curl` renvoie une erreur concernant le `-L` paramètre ou un message d’erreur indiquant « Objet déplacé », essayez d’utiliser l’URL complète plutôt que la `aka.ms` redirection :

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

### <a name="az-command-not-found"></a>`az` commande introuvable

Si vous ne pouvez pas exécuter la commande après l’installation et après avoir utilisé `bash` et `zsh`, effacez le cache de hachage de commande de votre interpréteur de commandes. Exécuter

```bash
hash -r
```

et vérifiez si le problème est résolu.

Le problème peut également survenir si vous n’avez pas redémarré votre interpréteur de commandes après l’installation. Assurez-vous que l’emplacement de la commande `az` se trouve dans votre `$PATH`. L’emplacement de la commande `az` est

```bash
<install path>/bin
```

### <a name="proxy-blocks-connection"></a>Le proxy bloque la connexion

[!INCLUDE[configure-proxy](configure-proxy.md)]

Pour obtenir les scripts d’installation, votre proxy doit autoriser les connexions HTTPS aux adresses suivantes :

* `https://aka.ms/`
* `https://azurecliprod.blob.core.windows.net/`
* `https://pypi.python.org`
* Points de terminaison utilisés par le gestionnaire de package de votre distribution (le cas échéant) pour les packages de base

[!INCLUDE[troubleshoot-wsl.md](troubleshoot-wsl.md)]

## <a name="uninstall"></a>Désinstaller l’interface

[!INCLUDE [uninstall-boilerplate.md](uninstall-boilerplate.md)]

Désinstallez l’interface de ligne de commande en supprimant directement les fichiers de l’emplacement spécifié lors de l’installation. L’emplacement d’installation par défaut est `$HOME`.

1. Supprimez les fichiers CLI installés.

   ```bash
   rm -r <install location>/lib/azure-cli
   rm <install location>/bin/az
   ```

2. Modifiez votre fichier `$HOME/.bash_profile` pour supprimer la ligne suivante :

   ```text
   <install location>/lib/azure-cli/az.completion
   ```

3. Si vous utilisez `bash` ou `zsh`, rechargez le cache de commande de l’interpréteur de commandes.

   ```bash
   hash -r
   ```