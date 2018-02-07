---
title: Installer manuellement Azure CLI 2.0 pour Linux
description: "Installation manuelle d’Azure CLI 2.0 pour Linux"
keywords: "Azure CLI, Installation d’Azure CLI, Azure Linux, installation Azure Linux"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 01/29/18
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: d8c88d111c50a3cbb6b643a14dcd2a9773699657
ms.sourcegitcommit: 8606f36963e8daa6448d637393d1e4ef2c9859a0
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/01/2018
---
# <a name="install-azure-cli-20-on-linux-manually"></a>Installer manuellement Azure CLI 2.0 sur Linux

Si vous n’avez pas de package disponible sur votre distribution pour l’interface de ligne de commande Azure, vous pouvez toujours installer l’interface de ligne de commande manuellement en exécutant un script d’installation.

> [!NOTE]
> Il est fortement recommandé d’utiliser un gestionnaire de package pour l’interface CLI. Un gestionnaire de package permet de s’assurer que vous obtenez toujours les dernières mises à jour et garantit la stabilité des composants de l’interface CLI. Vérifiez s’il existe un package pour votre distribution avant d’installer manuellement.

## <a name="prerequisites"></a>configuration requise

Pour installer l’interface de ligne de commande, vous avez besoin des logiciels suivants sur votre système :

* [Python 2.7 ou Python 3.x](https://www.python.org/downloads/)
* [libffi](https://sourceware.org/libffi/)
* [OpenSSL 1.0.2](https://www.openssl.org/source/)

## <a name="install-or-update"></a>Installation ou mise à jour 

Que vous installiez ou que vous mettiez à jour l’interface de ligne de commande, vous devez effectuer une installation complète. Une fois que vous disposez de la configuration requise, vous pouvez installer l’interface de ligne de commande en exécutant `curl`.

```bash
curl -L https://aka.ms/InstallAzureCli | bash
```

Au lieu de cela, vous pouvez également télécharger le script et l’exécuter localement. Vous devrez peut-être redémarrer votre interpréteur de commandes pour que certaines modifications soient prises en compte. Après l’installation, exécutez l’interface de ligne de commande avec la commande `az`.

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
  
  ```
  <install location>/lib/azure-cli/az.completion
  ```

3. Si vous utilisez `bash` ou `zsh`, rechargez le cache de commande de l’interpréteur de commandes.
  
  ```bash
  hash -r
  ```
