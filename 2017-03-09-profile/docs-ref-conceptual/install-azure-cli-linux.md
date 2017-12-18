---
title: Installer manuellement Azure CLI 2.0 pour Linux
description: "Installation manuelle d’Azure CLI 2.0 pour Linux"
keywords: "Azure CLI, Installation d’Azure CLI, Azure Linux, installation Azure Linux"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 11/01/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ROBOTS: NOINDEX,NOFOLLOW
ms.openlocfilehash: cf1405cae70762146f63bc6629edc0dd1d949fff
ms.sourcegitcommit: 2e4d0bdd94c626e061434883032367b5619de4fe
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/09/2017
---
# <a name="install-azure-cli-20-on-linux-manually"></a>Installer manuellement Azure CLI 2.0 sur Linux

Si vous n’avez pas de package disponible sur votre distribution pour l’interface de ligne de commande Azure, vous pouvez toujours installer l’interface de ligne de commande manuellement en exécutant un script d’installation. Si vous disposez d’un package disponible, il s’agit toujours de la méthode d’installation recommandée.

## <a name="prerequisites"></a>Composants requis

Pour installer l’interface de ligne de commande, vous devrez disposer des logiciels suivants sur votre système :

* [Python 2.7 ou Python 3.x](https://www.python.org/downloads/)
* [libffi](https://sourceware.org/libffi/)
* [OpenSSL 1.0.2](https://www.openssl.org/source/)

## <a name="install-or-update-manually"></a>Installation ou mise à jour manuelle

Que vous installiez ou que vous mettiez à jour l’interface de ligne de commande, vous devrez effectuer une installation complète. Une fois que vous disposez de la configuration requise, vous pouvez installer l’interface de ligne de commande en exécutant `curl`.

```bash
curl -L https://aka.ms/InstallAzureCli | bash
```

Si vous préférez, ou si vous n’avez pas `curl` sur votre système, vous pouvez télécharger le script et l’exécuter localement à la place. Vous devrez peut-être redémarrer votre interpréteur de commandes pour que certaines modifications soient prises en compte. Après l’installation, exécutez l’interface de ligne de commande avec la commande `az`.

## <a name="troubleshooting"></a>Résolution des problèmes

### <a name="curl-object-moved-error"></a>erreur curl « Objet déplacé »

Si la commande `curl` renvoie une erreur concernant le `-L` paramètre ou un message d’erreur indiquant « Objet déplacé », essayez d’utiliser l’URL complète plutôt que la `aka.ms` redirection :

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

### <a name="az-command-not-found"></a>`az` commande introuvable

Après l’installation, si vous ne pouvez pas exécuter la commande, vous devrez peut-être effacer le cache de hachage de commande de l’interpréteur de commandes. Exécuter

```bash
hash -r
```

et vérifier si le problème est résolu.

Cela peut également se produire si vous n’avez pas redémarré votre interpréteur de commandes après l’installation. Assurez-vous que l’emplacement de la commande `az` se trouve dans votre `$PATH`.

Si vous avez exécuté le script d’installation, il s’agira de :

```bash
<install path>/bin
```

## <a name="unstinall-manually"></a>Désinstaller manuellement

Si jamais vous décidez de désinstaller l’interface de ligne de commande Azure, nous sommes désolés de vous voir partir. Avant de désinstaller, utilisez la commande `az feedback`, afin de nous donner quelques raisons pour lesquelles vous avez choisi de désinstaller et nous aider à améliorer l’expérience CLI. Nous souhaitons nous assurer que l’interface de ligne de commande Azure est aussi conviviale et exempte de bogues que possible. Vous pouvez également [signaler un problème lié à GitHub](https://github.com/Azure/azure-cli/issues).

Vous pouvez désinstaller l’interface de ligne de commande en supprimant directement les fichiers de l’emplacement d’installation. Votre emplacement d’installation doit être spécifié au moment de l’installation, si vous avez installé via le script `https://aka.ms/InstallAzureCLI`. L’emplacement d’installation par défaut est `$HOME`.

Tout d’abord, supprimez les fichiers CLI installés :

```bash
rm -r <install location>/lib/azure-cli
rm <install location>/bin/az
```

Modifiez ensuite votre fichier `$HOME/.bash_profile` pour supprimer la ligne :

```
<install location>/lib/azure-cli/az.completion
```

Enfin, rechargez le cache de commande de l’interpréteur de commandes s’il en utilise un. Les utilisateurs `bash`et `zsh` devront effectuer cette étape :

```bash
hash -r
```
