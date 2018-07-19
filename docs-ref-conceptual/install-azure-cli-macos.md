---
title: Installer l’interface de ligne de commande Azure pour macOS
description: Installation d’Azure CLI 2.0 sur macOS
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 01/29/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 76b9afec92aa3da916382b85d2261547b6877e03
ms.sourcegitcommit: fb3fed8701aff6c46af856e8fdc3e56ff9a678bc
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/11/2018
ms.locfileid: "38228918"
---
# <a name="install-azure-cli-20-on-macos"></a>Installation d’Azure CLI 2.0 sur macOS

Pour la plateforme macOS, vous pouvez installer Azure CLI avec le [Gestionnaire de package Homebrew](http://brew.sh). Homebrew facilite le maintien à jour de votre installation de la mise à jour de l’interface CLI. Le package CLI a été testé sur macOS 10.9 et les versions ultérieures.

## <a name="install"></a>Installer

Homebrew est le moyen le plus simple pour gérer votre installation d’interface de ligne de commande. Il offre des moyens pratiques pour installer, mettre à jour et désinstaller.
Si vous ne disposez pas de Homebrew sur votre système, [installez Homebrew](https://docs.brew.sh/Installation.html) avant de continuer.

Vous pouvez installer l’interface de ligne de commande en mettant à jour vos informations de référentiel Homebrew, puis en exécutant la commande `install` :

```bash
brew update && brew install azure-cli
```

Vous pouvez ensuite exécuter l’interface de ligne de commande Azure avec la commande `az`. Pour vous connecter, utilisez la commande [az login](/cli/azure/reference-index#az-login).

[!INCLUDE [interactive-login](includes/interactive-login.md)]

Pour en savoir plus sur les différentes méthodes d’authentification, consultez [Se connecter avec Azure CLI 2.0](authenticate-azure-cli.md).

## <a name="troubleshooting"></a>Résolution de problèmes

Si vous rencontrez un problème lors de l’installation de l’interface de ligne de commande via Homebrew, voici quelques erreurs courantes. Si votre problème ne figure pas ici, veuillez [signaler le problème sur Github](https://github.com/Azure/azure-cli/issues).

### <a name="unable-to-find-python-or-installed-packages"></a>Impossible de trouver des packages Python ou des packages installés

Si votre programme d’installation ne trouve pas les packages Python ou les packages installés, il se peut qu’il y ait une incompatibilité de version mineure ou un autre problème qui s’est produit lors de l’installation de Homebrew. Étant donné que l’interface CLI n’utilise pas un environnement virtuel Python, cela dépend de sa capacité à trouver des versions appropriées de Python. Vous pourrez peut-être résoudre ces problèmes en liant à nouveau votre installation de Python.

```bash
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
