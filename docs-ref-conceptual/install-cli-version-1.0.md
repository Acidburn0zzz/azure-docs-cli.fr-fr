---
title: Installer l’interface de ligne de commande Azure CLI 1.0
description: Installation de l’interface de ligne de commande Azure CLI 1.0 pour Mac, Linux et Windows afin d’utiliser les services Azure
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 03/20/2017
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 92714f32736e0a1a0ea7c8dd4a615b158c955931
ms.sourcegitcommit: ae72b6c8916aeb372a92188090529037e63930ba
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/28/2018
---
# <a name="install-the-azure-cli-10"></a>Installer l’interface de ligne de commande Azure CLI 1.0

> [!IMPORTANT]
> Cette rubrique décrit comment installer Azure CLI 1.0. Cette interface est dépréciée et doit être utilisée uniquement pour la prise en charge avec le modèle Azure Service Management (ASM) avec des ressources « classiques ».
> Pour les déploiements Azure Resource Manager, utilisez [Azure CLI 2.0](/cli/azure).

Installez rapidement l’interface de ligne de commande Azure (Azure CLI 1.0) pour bénéficier d’un ensemble de commandes shell open source permettant de créer et de gérer les ressources dans Microsoft Azure. Vous avez plusieurs options pour installer ces outils multiplateformes sur votre ordinateur :

* **Package npm** : exécutez npm (le Gestionnaire de package de JavaScript) pour installer le dernier package de l’interface Azure CLI 1.0 sur votre système d’exploitation ou distribution Linux. Requiert l’installation de node.js et npm sur votre ordinateur.
* **Programme d’installation** : téléchargez un programme d’installation pour une installation rapide sur Mac ou Windows.
* **Conteneur Docker** : utilisez la dernière interface CLI dans un conteneur Docker prêt à s’exécuter. Nécessite la présence d’un hôte Docker sur votre ordinateur.

Pour obtenir davantage d’options générales et de contexte, consultez le référentiel du projet sur [GitHub](https://github.com/azure/azure-xplat-cli).

Une fois l’interface de ligne de commande Azure CLI 1.0 installée, [connectez-vous à l’aide de votre abonnement Azure](/cli/azure/authenticate-azure-cli) et exécutez les commandes **azure** depuis votre interface de ligne de commande (Bash, Terminal, invite de ligne de commande, etc.) pour travailler avec vos ressources Azure.

## <a name="option-1-install-an-npm-package"></a>Option 1 : Installer un package npm
Pour installer l’interface CLI à partir d’un package npm, vérifiez que vous avez téléchargé et installé les [derniers fichiers Node.js et npm](https://nodejs.org/en/download/package-manager/). Ensuite, exécutez **npm install** pour installer le package azure-cli :

```bash
npm install -g azure-cli
```

Sur les distributions Linux, vous devrez peut-être utiliser **sudo** pour exécuter la commande **npm**, comme suit :

```bash
sudo npm install -g azure-cli
```

> [!NOTE]
> Si vous devez installer ou mettre à jour Node.js et npm sur votre distribution Linux ou votre système d’exploitation, nous vous recommandons d’installer la dernière version de Node.js LTS (4.x). Si vous utilisez une version antérieure, vous pouvez obtenir des erreurs d’installation.

Si vous préférez, téléchargez le dernier [fichier tar][linux-installer] Linux pour le package npm en local. Ensuite, installez le package npm téléchargé comme suit (sur les distributions Linux vous devrez peut-être utiliser **sudo**) :

```bash
npm install -g <path to downloaded tar file>
```

## <a name="option-2-use-an-installer"></a>Option 2 : Utiliser un programme d’installation
Si vous utilisez un ordinateur Mac ou Windows, les programmes d’installation de l’interface CLI suivants sont disponibles au téléchargement :

* [Programme d’installation Mac OS X][mac-installer]
* [MSI Windows][windows-installer]

> [!TIP]
> Sous Windows, vous pouvez également télécharger [Web Platform Installer](https://go.microsoft.com/?linkid=9828653) pour installer l’interface CLI. Ce programme d’installation vous donne la possibilité d’installer des Kits de développement logiciel (SDK) Azure et des outils de ligne de commande supplémentaires après l’installation de l’interface CLI.

## <a name="option-3-use-a-docker-container"></a>Option 3 : Utiliser un conteneur Docker
Si vous avez configuré votre ordinateur comme hôte [Docker](https://docs.docker.com/engine/understanding-docker/) , vous pouvez exécuter la dernière interface de ligne de commande Azure CLI 1.0 dans un conteneur Docker. Exécutez la commande suivante (sur les distributions Linux, vous devrez peut-être utiliser **sudo**.) :

```bash
docker run -it microsoft/azure-cli:0.10.17
```

## <a name="run-azure-cli-10-commands"></a>Exécution des commandes Azure CLI 1.0
Une fois l’interface de ligne de commande Azure CLI 1.0 installée, exécutez la commande **azure** depuis l’interface de ligne de commande utilisateur (Bash, Terminal, invite de ligne de commande, etc.). Par exemple, pour exécuter la commande d’aide, saisissez ce qui suit :

```azurecli
azure help
```

> [!NOTE]
> Dans certaines distributions Linux, vous pouvez recevoir une erreur similaire à `/usr/bin/env: ‘node’: No such file or directory`. Cette erreur est due à l’installation récente de Node.js sous /usr/bin/nodejs. Pour la corriger, créez un lien symbolique vers /usr/bin/node en exécutant cette commande :

```bash
sudo ln -s /usr/bin/nodejs /usr/bin/node
```

Pour afficher la version de l’interface Azure CLI 1.0 que vous avez installée, saisissez la commande suivante :

```azurecli
azure --version
```

Vous avez terminé l’installation. Pour accéder à toutes les commandes de l’interface de ligne de commande et travailler avec vos propres ressources, [connectez-vous à votre abonnement Azure à partir de l’interface de ligne de commande Azure](/cli/azure/authenticate-azure-cli).

> [!NOTE]
> Lorsque vous utilisez l’interface de ligne de commande Azure pour la première fois, vous voyez un message vous demandant si vous souhaitez autoriser Microsoft à recueillir des informations d’utilisation. La participation se fait sur la base du volontariat. Si vous choisissez de participer, vous pouvez arrêter à tout moment en exécutant `azure telemetry --disable`. Pour activer la participation, exécutez `azure telemetry --enable`.

## <a name="update-the-cli"></a>Mise à jour de l’interface CLI
Microsoft publie fréquemment des versions mises à jour de l’interface CLI Azure. Réinstallez l’interface CLI à l’aide du programme d’installation pour votre système d’exploitation, ou exécutez le dernier conteneur Docker. Alternativement, si les dernières versions de Node.js et npm sont installées, procédez à la mise à jour en saisissant ce qui suit (dans les distributions Linux, vous devrez peut-être utiliser **sudo**).

```bash
npm update -g azure-cli
```

## <a name="enable-tab-completion"></a>Activer la saisie semi-automatique via la touche Tab
La saisie semi-automatique via la touche Tab des commandes CLI est prise en charge pour Mac et Linux.

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
* [Se connecter à partir de l’interface de ligne de commande à votre abonnement Azure](/cli/azure/authenticate-azure-cli) pour créer et gérer des ressources Azure.
* Pour plus d'informations sur l'interface de ligne de commande Azure, télécharger un code source, signaler des problèmes ou contribuer au projet, voir [Référentiel GitHub pour l'interface de ligne de commande Azure](https://github.com/azure/azure-xplat-cli)(en anglais).
* Si vous avez des questions sur l’utilisation de l’interface de ligne de commande Azure ou sur l’utilisation d’Azure, consultez les [forums Azure](https://social.msdn.microsoft.com/Forums/en-US/home?forum=azurescripting).


[mac-installer]: http://aka.ms/mac-azure-cli
[windows-installer]: http://aka.ms/webpi-azure-cli
[linux-installer]: http://aka.ms/linux-azure-cli
[cliasm]: /cli/azure/get-started-with-az-cli2
[cliarm]: ./virtual-machines/azure-cli-arm-commands.md
