---
title: "Installer l’interface de ligne de commande Azure pour macOS"
description: "Installation d’Azure CLI 2.0 sur macOS"
keywords: "Azure CLI, Installation d’Azure CLI, Azure macOS, installation Azure macOS"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 10/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ROBOTS: NOINDEX,NOFOLLOW
ms.openlocfilehash: e615d2b3ab3b1307e982cb1d4d456633440afdf6
ms.sourcegitcommit: 905939cc44764b4d1cc79a9b36c0793f7055a686
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/20/2017
---
# <a name="install-azure-cli-20-on-macos"></a>Installation d’Azure CLI 2.0 sur macOS

Pour la plateforme macOS, vous pouvez installer l’interface de ligne de commande Azure via le [Gestionnaire de package Homebrew](http://brew.sh) ou manuellement. La méthode d’installation par défaut est via Homebrew, afin de faciliter l’installation, obtenez les mises à jour et désinstallez si besoin.

## <a name="use-homebrew-to-install"></a>Utilisez Homebrew pour l’installation

Homebrew est le moyen le plus simple pour gérer votre installation d’interface de ligne de commande. Il offre des moyens pratiques pour installer, mettre à jour et désinstaller. Il est semblable à d’autres gestionnaires de package comme `apt` ou `yum`.
Si vous ne disposez pas de Homebrew sur votre système, [installez Homebrew](https://docs.brew.sh/Installation.html) avant de continuer.

### <a name="install-with-homebrew"></a>Installer avec Homebrew

Vous pouvez installer l’interface de ligne de commande en mettant à jour vos informations de référentiel Homebrew, puis en exécutant la commande `install` :

```bash
brew update && brew install azure-cli
```

Vous pouvez ensuite exécuter l’interface de ligne de commande Azure avec la commande `az`.

### <a name="update-with-homebrew"></a>Mettre à jour avec Homebrew

L’interface de ligne de commande est régulièrement mise à jour avec des correctifs de bogues, des améliorations, de nouvelles fonctions ainsi que des fonctionnalités en préversion. Une nouvelle version est disponible à peu près toutes les deux semaines. Vous devez mettre à jour vos informations de référentiel local, puis le package de l’interface de ligne de commande.

```bash
brew update && brew upgrade azure-cli
```

### <a name="troubleshooting"></a>Résolution des problèmes

Avez-vous rencontré un problème lors de l’installation ou la mise à jour de l’interface de ligne de commande avec Homebrew ? Voici certaines erreurs courantes qui peuvent se produire et comment les diagnostiquer et les résoudre.

#### <a name="unable-to-find-python-or-installed-packages"></a>Impossible de trouver des packages Python ou des packages installés

Si votre programme d’installation ne peut pas trouver les packages Python ou les packages installés, il se peut qu’il y ait une incompatibilité de version mineure ou un autre problème qui s’est produit lors de l’installation de Homebrew. Étant donné que l’interface CLI n’utilise pas un virtualenv, cela dépend de sa capacité à trouver des versions appropriées de Python installées par Homebrew. Vous pourrez peut-être résoudre ces problèmes en liant à nouveau votre installation de Python :

```bash
brew link --overwrite python3
```

#### <a name="the-cli-version-is-out-of-date"></a>La version de l’interface de ligne de commande est obsolète

Si vous pensez que votre version de l’interface de ligne de commande peut être obsolète, exécutez une commande `brew update`, suivie par `brew upgrade azure-cli`. Si cela ne met pas à jour l’interface de ligne de commande, n’oubliez pas que les packages de Homebrew peuvent se déployer plus lentement que les versions générales. Si vous avez besoin des installations les plus récentes de l’interface de ligne de commande, vous devriez [installer manuellement](#manage-the-cli-manually).

### <a name="uninstall-with-homebrew"></a>Désinstaller avec Homebrew

Si jamais vous décidez de désinstaller l’interface de ligne de commande Azure, nous sommes désolés de vous voir partir. Avant de désinstaller, utilisez la commande `az feedback`, afin de nous donner quelques raisons pour lesquelles vous avez choisi de désinstaller et nous aider à améliorer l’expérience CLI. Nous souhaitons nous assurer que l’interface de ligne de commande Azure est aussi conviviale et exempte de bogues que possible. Vous pouvez également [signaler un problème lié à GitHub](https://github.com/Azure/azure-cli/issues).

Si vous avez installé avec Homebrew, vous devez également l’utiliser pour désinstaller.

```bash
brew uninstall azure-cli
```

## <a name="install-the-cli-manually"></a>Installation manuelle de l’interface de ligne de commande

Si vous ne pouvez pas ou ne souhaitez pas gérer l’installation de l’interface de ligne de commande avec Homebrew, vous pouvez installer manuellement.

Suivez les [instructions d’installation manuelles de Linux](install-azure-cli-linux.md) pour installer manuellement sur macOS. Les versions macOS 10.9 et versions ultérieures doivent inclure toutes les dépendances requises.
