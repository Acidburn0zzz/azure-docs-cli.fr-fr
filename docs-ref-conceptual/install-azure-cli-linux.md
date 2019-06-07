---
title: Installer manuellement Azure CLI pour Linux
description: Comment installer manuellement Azure CLI sur Linux
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 13edb9954678aca627529714aeee02062c720219
ms.sourcegitcommit: 08043c47d3ccf23522b91e6bba3932e312c04c7f
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/04/2019
ms.locfileid: "66516300"
---
# <a name="install-azure-cli-on-linux-manually"></a>Installer manuellement Azure CLI sur Linux

S’il n’existe aucun package pour l’interface Azure CLI pour vous et votre distribution, installez l’interface CLI manuellement en exécutant un script.

[!INCLUDE [current-version](includes/current-version.md)]

> [!NOTE]
> Il est fortement recommandé d’installer l’interface CLI avec un gestionnaire de package. Un gestionnaire de package permet de s’assurer que vous obtenez toujours les dernières mises à jour et garantit la stabilité des composants de l’interface CLI. Vérifiez s’il existe un package pour votre distribution avant d’installer manuellement.

## <a name="prerequisites"></a>Prérequis

L’interface CLI requiert les logiciels suivants :

* [Python 3.6.x ou 3.7.x](https://www.python.org/downloads/). 
* [libffi](https://sourceware.org/libffi/)
* [OpenSSL 1.0.2](https://www.openssl.org/source/)

> [!IMPORTANT]
>
> L’interface CLI est également compatible avec Python 2.7.x, dont la fin de vie est prévue pour le 1er janvier 2020. C’est la raison pour laquelle nous vous recommandons d’installer Python 3 afin d’exécuter l’interface CLI.

## <a name="install-or-update"></a>Installation ou mise à jour

L’installation et la mise à jour de l’interface CLI nécessitent toutes de réexécuter le script d’installation. Installez l’interface CLI en exécutant `curl`.

```bash
curl -L https://aka.ms/InstallAzureCli | bash
```

Le script peut également être téléchargé et exécuté localement. Vous devrez peut-être redémarrer votre interpréteur de commandes pour que certaines modifications soient prises en compte.

Vous pouvez ensuite exécuter l’interface de ligne de commande Azure avec la commande `az`. Pour vous connecter, utilisez la commande [az login](/cli/azure/reference-index#az-login).

[!INCLUDE [interactive-login](includes/interactive-login.md)]

Pour en savoir plus sur les différentes méthodes d’authentification, consultez [Se connecter avec Azure CLI](authenticate-azure-cli.md).

## <a name="troubleshooting"></a>Résolution de problèmes

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

[!INCLUDE[configure-proxy](includes/configure-proxy.md)]

Pour obtenir les scripts d’installation, votre proxy doit autoriser les connexions HTTPS aux adresses suivantes :

* `https://aka.ms/`
* `https://azurecliprod.blob.core.windows.net/`
* `https://pypi.python.org`
* Points de terminaison utilisés par le gestionnaire de package de votre distribution (le cas échéant) pour les packages de base

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="uninstall"></a>Désinstaller l’interface

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

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

## <a name="next-steps"></a>Étapes suivantes

Maintenant que vous avez installé l’interface CLI, découvrez ses fonctionnalités et ses commandes courantes.

> [!div class="nextstepaction"]
> [Prise en main de l’interface Azure CLI](get-started-with-azure-cli.md)
