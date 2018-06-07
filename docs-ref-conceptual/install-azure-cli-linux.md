---
title: Installer manuellement Azure CLI 2.0 pour Linux
description: Installation manuelle d’Azure CLI 2.0 pour Linux
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 01/29/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: b11ab99626227cb53a604d429fa32c560e4255d9
ms.sourcegitcommit: 38549f60d76d4b6b65d180367e83749769fe6e43
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/04/2018
ms.locfileid: "34703126"
---
# <a name="install-azure-cli-20-on-linux-manually"></a>Installer manuellement Azure CLI 2.0 sur Linux

Si vous n’avez pas de package disponible sur votre distribution pour l’interface de ligne de commande Azure, vous pouvez toujours installer l’interface de ligne de commande manuellement en exécutant un script d’installation.

> [!NOTE]
> Il est fortement recommandé d’utiliser un gestionnaire de package pour l’interface CLI. Un gestionnaire de package permet de s’assurer que vous obtenez toujours les dernières mises à jour et garantit la stabilité des composants de l’interface CLI. Vérifiez s’il existe un package pour votre distribution avant d’installer manuellement.

## <a name="prerequisites"></a>Prérequis


Pour installer l’interface de ligne de commande, vous avez besoin des logiciels suivants sur votre système :

* [Python 2.7 ou Python 3.x](https://www.python.org/downloads/)
* [libffi](https://sourceware.org/libffi/)
* [OpenSSL 1.0.2](https://www.openssl.org/source/)

## <a name="install-or-update"></a>Installation ou mise à jour

Que vous installiez ou que vous mettiez à jour l’interface de ligne de commande, vous devez effectuer une installation complète. Une fois que vous disposez de la configuration requise, vous pouvez installer l’interface de ligne de commande en exécutant `curl`.

```bash
curl -L https://aka.ms/InstallAzureCli | bash
```

Au lieu de cela, vous pouvez également télécharger le script et l’exécuter localement. Vous devrez peut-être redémarrer votre interpréteur de commandes pour que certaines modifications soient prises en compte. 

Vous pouvez ensuite exécuter l’interface de ligne de commande Azure avec la commande `az`. Pour vous connecter, exécutez la commande `az login`.

```azurecli
az login
```

Pour en savoir plus sur les différentes méthodes de connexion, consultez [Se connecter avec Azure CLI 2.0](authenticate-azure-cli.md).

## <a name="troubleshooting"></a>Résolution de problèmes

Voici certains problèmes courants rencontrés pendant une installation manuelle. Si votre problème ne figure pas ici, veuillez [signaler le problème sur Github](https://github.com/Azure/azure-cli/issues).
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

Le problème peut également se produire si vous n’avez pas redémarré votre interpréteur de commandes après l’installation. Assurez-vous que l’emplacement de la commande `az` se trouve dans votre `$PATH`. L’emplacement de la commande `az` est

```bash
<install path>/bin
```

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
