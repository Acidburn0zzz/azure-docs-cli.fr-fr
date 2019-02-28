---
title: Installer l’interface de ligne de commande Azure pour macOS
description: Comment installer Azure CLI sur macOS
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 11/05/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 61be6c31e7251c8b374bf09072a9ecba9b914342
ms.sourcegitcommit: 1987a39809f9865034b27130e56f30b2bd1eb72c
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/19/2019
ms.locfileid: "56422049"
---
# <a name="install-azure-cli-on-macos"></a>Installer Azure CLI sur macOS

Pour la plateforme macOS, vous pouvez installer Azure CLI avec le [Gestionnaire de package Homebrew](https://brew.sh). Homebrew facilite le maintien à jour de votre installation de la mise à jour de l’interface CLI. Le package CLI a été testé sur macOS 10.9 et les versions ultérieures.

[!INCLUDE [current-version](includes/current-version.md)]

## <a name="install"></a>Installer

Homebrew est le moyen le plus simple pour gérer votre installation d’interface de ligne de commande. Il offre des moyens pratiques pour installer, mettre à jour et désinstaller.
Si vous ne disposez pas de Homebrew sur votre système, [installez Homebrew](https://docs.brew.sh/Installation.html) avant de continuer.

Vous pouvez installer l’interface de ligne de commande en mettant à jour vos informations de référentiel Homebrew, puis en exécutant la commande `install` :

```bash
brew update && brew install azure-cli
```

> [!IMPORTANT]
>
> Azure CLI a une dépendance avec le package `python3` dans Homebrew et va l’installer sur votre système, même si Python 2 est disponible. Azure CLI offre la garantie d’être compatible avec la dernière version de `python3` publiée sur Homebrew.

Vous pouvez ensuite exécuter l’interface de ligne de commande Azure avec la commande `az`. Pour vous connecter, utilisez la commande [az login](/cli/azure/reference-index#az-login).

[!INCLUDE [interactive-login](includes/interactive-login.md)]

Pour en savoir plus sur les différentes méthodes d’authentification, consultez [Se connecter avec Azure CLI](authenticate-azure-cli.md).

## <a name="troubleshooting"></a>Résolution de problèmes

Si vous rencontrez un problème lors de l’installation de l’interface de ligne de commande via Homebrew, voici quelques erreurs courantes. Si vous rencontrez un problème n’étant pas évoqué ici, [signalez un problème sur github](https://github.com/Azure/azure-cli/issues).

### <a name="unable-to-find-python-or-installed-packages"></a>Impossible de trouver des packages Python ou des packages installés

Une incompatibilité de version mineure ou un autre problème a pu se produire lors de l’installation de Homebrew. L’interface CLI n’utilise pas d’environnement virtuel Python, ainsi, elle s’appuie sur la recherche de la version de Python installée. Un correctif possible consiste à installer et à relier la dépendance `python3` depuis Homebrew.

```bash
brew update && brew install python3 && brew upgrade python3
brew link --overwrite python3
```

### <a name="cli-version-1x-is-installed"></a>La version 1.x de l’interface de ligne de commande est installée

Si une version obsolète a été installée, cela peut être dû à un cache Homebrew périmé. Suivez les instructions de [mise à jour](#Update).

## <a name="update"></a>Mettre à jour

L’interface de ligne de commande est régulièrement mise à jour avec des correctifs de bogues, des améliorations, de nouvelles fonctions ainsi que des fonctionnalités en préversion. Une nouvelle version est disponible à peu près toutes les deux semaines. Mettez à jour vos informations de référentiel local, puis mettez à niveau le package `azure-cli`.

```bash
brew update && brew upgrade azure-cli
```

## <a name="uninstall"></a>Désinstaller l’interface

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

Utilisez homebrew pour désinstaller le package `azure-cli`.

```bash
brew uninstall azure-cli
```

## <a name="other-installation-methods"></a>Autres méthodes d’installation

Si vous ne pouvez pas utiliser homebrew pour installer Azure CLI dans votre environnement, il est possible d’utiliser les instructions manuelles pour Linux. Notez que ce processus n’est pas officiellement conservé pour être compatible avec macOS. L’utilisation d’un gestionnaire de package tel que Homebrew est toujours recommandée. Utilisez uniquement la méthode d’installation manuelle si vous ne disposez d’aucune autre option disponible.

Pour les instructions d’installation manuelle, consultez [Installer Azure CLI sur Linux manuellement](install-azure-cli-linux.md).

## <a name="next-steps"></a>Étapes suivantes

Maintenant que vous avez installé l’interface CLI, découvrez ses fonctionnalités et ses commandes courantes.

> [!div class="nextstepaction"]
> [Prise en main de l’interface Azure CLI](get-started-with-azure-cli.md)
