---
title: Installez l’interface de ligne de commande d’Azure CLI Classic
description: Installez l’interface de ligne de commande Azure CLI Classic pour Mac, Linux et Windows afin de commencer à utiliser les services Azure
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 06/11/2018
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: b53fb38c26ac8ad4dba4a956105b91e789334053
ms.sourcegitcommit: d5f026468ea20bbd7ef35bdbf9852bcb2b812d83
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/23/2020
ms.locfileid: "97744542"
---
# <a name="install-the-azure-classic-cli"></a>Installez l’interface de ligne de commande d’Azure CLI Classic

> [!IMPORTANT]
> Cette rubrique décrit comment installer l’interface de ligne de commande Azure CLI Classic. L’interface de ligne de commande classique est déconseillée et doit uniquement être utilisée avec le modèle de déploiement classique.
> Pour tous les autres déploiements, utilisez [Azure CLI](/cli/azure).

Installez rapidement l’interface de ligne de commande Azure CLI Classic pour bénéficier d’un ensemble d’interpréteurs de commandes open source permettant de créer et de gérer des ressources dans Microsoft Azure. Vous avez plusieurs options pour installer ces outils multiplateformes sur votre ordinateur :

* **Package npm** : exécutez npm (le Gestionnaire de package pour JavaScript) afin d’installer le dernier package de l’interface de ligne de commande Azure CLI Classic sur votre système d’exploitation ou sur votre distribution Linux. Nécessite node.js et npm.
* **Programme d’installation** : téléchargez un programme d’installation pour une installation simple sur macOS ou Windows.
* **Conteneur Docker** : utilisez l’interface de ligne de commande classique dans un conteneur Docker prêt à exécuter. Nécessite un hôte Docker.

Pour obtenir davantage d’options générales et de contexte, consultez le référentiel du projet sur [GitHub](https://github.com/azure/azure-xplat-cli).

Une fois l’interface de ligne de commande Azure CLI Classic installée, connectez-vous à l’aide de `azure login` et exécutez les commandes `azure` depuis votre interface de ligne de commande (Bash, terminal, invite de commandes, etc.) pour travailler avec vos ressources Azure.

## <a name="option-1-install-an-npm-package"></a>Option 1 : Installer un package npm

Pour installer l’interface de ligne de commande classique à partir d’un package npm, vérifiez que vous avez téléchargé et installé les [derniers fichiers Node.js et npm](https://nodejs.org/en/download/package-manager/). Ensuite, exécutez `npm install` pour installer le package azure-cli :

```bash
npm install -g azure-cli
```

Sur les distributions Linux, vous devrez peut-être utiliser `sudo` pour exécuter la commande `npm`, comme suit :

```bash
sudo npm install -g azure-cli
```

> [!NOTE]
> Si vous devez installer ou mettre à jour Node.js et npm sur votre système d’exploitation, nous vous recommandons d’installer la dernière version de Node.js LTS 4.x, ou une version ultérieure. Si vous utilisez une version antérieure, vous pouvez obtenir des erreurs d’installation.

Si vous préférez, vous pouvez également télécharger un fichier tar à partir des [versions GitHub](https://github.com/Azure/azure-xplat-cli/releases). Ensuite, installez le package npm téléchargé comme suit (sur les distributions Linux, vous devrez peut-être utiliser `sudo`) :

```bash
npm install -g <path to downloaded tar file>
```

## <a name="option-2-use-an-installer"></a>Option 2 : Utiliser un programme d’installation

Si vous utilisez un ordinateur Mac ou Windows, les programmes d’installation DMG et MSI sont disponibles depuis les [versions GitHub](https://github.com/Azure/azure-xplat-cli/releases).

> [!TIP]
> Sous Windows, vous pouvez également télécharger [Web Platform Installer](https://go.microsoft.com/?linkid=9828653) pour installer l’interface de ligne de commande classique. Ce programme d’installation vous donne la possibilité d’installer des Kits de développement logiciel (SDK) Azure et des outils de ligne de commande supplémentaires.

## <a name="option-3-use-a-docker-container"></a>Option 3 : Utiliser un conteneur Docker

Si vous avez configuré votre ordinateur comme hôte [Docker](https://docs.docker.com/engine/understanding-docker/), vous pouvez exécuter l’interface de ligne de commande Azure CLI Classic dans un conteneur Docker. Exécutez la commande suivante (sur les distributions Linux, vous devrez peut-être utiliser `sudo`) :

```bash
docker run -it mcr.microsoft.com/azure-cli:0.10.14
```

## <a name="run-azure-classic-cli-commands"></a>Exécutez les commandes Azure CLI Classic

Une fois l’interface de ligne de commande classique installée, exécutez la commande `azure` depuis l’interface utilisateur de ligne de commande (Bash, terminal, invite de commandes, etc.). Par exemple, pour exécuter la commande d’aide, saisissez ce qui suit :

```azurecli-interactive
azure help
```

> [!NOTE]
> Dans certaines distributions Linux, vous pouvez recevoir une erreur similaire à `/usr/bin/env: ‘node’: No such file or directory`. Cette erreur est due à l’installation récente de Node.js sous /usr/bin/nodejs. Pour la corriger, créez un lien symbolique vers /usr/bin/node en exécutant cette commande :

```bash
sudo ln -s /usr/bin/nodejs /usr/bin/node
```

Pour afficher la version de l’interface de ligne de commande Azure CLI Classic que vous avez installée, saisissez la commande suivante :

```azurecli-interactive
azure --version
```

> [!NOTE]
> Lorsque vous utilisez l’interface de ligne de commande Azure CLI Classic pour la première fois, vous voyez un message vous demandant si vous souhaitez autoriser Microsoft à recueillir des informations d’utilisation. La participation se fait sur la base du volontariat. Si vous choisissez de participer, vous pouvez arrêter à tout moment en exécutant `azure telemetry --disable`. Pour activer la participation, exécutez `azure telemetry --enable`.

## <a name="update-the-classic-cli"></a>Mettre à jour l’interface de ligne de commande classique

Microsoft peut publier des versions mises à jour de l’interface de ligne de commande Azure CLI Classic. Réinstallez l’interface de ligne de commande classique à l’aide du programme d’installation pour votre système d’exploitation, ou exécutez le conteneur Docker le plus récent. Cependant, si les dernières versions de Node.js et npm sont installées, procédez à la mise à jour en saisissant ce qui suit (dans les distributions Linux, vous devrez peut-être utiliser `sudo`).

```bash
npm update -g azure-cli
```

## <a name="enable-tab-completion"></a>Activer la saisie semi-automatique via la touche Tab

L’autocomplétion des commandes d’interface de ligne de commande classique est prise en charge pour Mac et Linux.

Pour l’activer dans zsh, exécutez :

```bash
echo '. <(azure --completion)' >> .zshrc
```

Pour l’activer dans bash, exécutez :

```bash
azure --completion >> ~/azure.completion.sh
echo 'source ~/azure.completion.sh' >> ~/.bash_profile
```

## <a name="next-steps"></a>Étapes suivantes

* Pour plus d'informations sur l'interface de ligne de commande Azure CLI Classic, téléchargez le code source, signalez des problèmes ou contribuez au projet, en consultant le [Référentiel GitHub pour l'interface de ligne de commande Azure CLI Classic](https://github.com/azure/azure-xplat-cli).
