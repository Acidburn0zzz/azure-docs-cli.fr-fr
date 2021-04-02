---
title: Extensions Azure CLI
description: Utilisation d’extensions avec Azure CLI
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 08/06/2020
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: 4569f66f58c18257c461e553d2d6ce0979fa0295
ms.sourcegitcommit: 8bff8b2ce4492ab99ad39390e4c802fb4f4425c8
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/26/2021
ms.locfileid: "105581323"
---
# <a name="use-extensions-with-azure-cli"></a>Utilisez des extensions avec Azure CLI 

L’interface de ligne de commande Azure offre la possibilité de charger des extensions. Les extensions sont des roues Python qui ne sont pas fournies comme partie de la CLI mais qui sont exécutées en tant que commandes CLI.
Avec les extensions, vous obtenez l’accès aux commandes expérimentales et préliminaires, ainsi que la capacité d’écrire vos propres interfaces CLI. Cet article explique comment gérer les extensions et répond aux questions courantes concernant leur utilisation.

## <a name="find-extensions"></a>Rechercher des extensions

Pour voir les extensions fournies et gérées par Microsoft, utiliser la commande [az extension list-available](/cli/azure/extension#az_extension_list_available).

```azurecli-interactive
az extension list-available --output table
```

Nous hébergeons également une [liste des extensions](azure-cli-extensions-list.md) sur le site de la documentation.

## <a name="install-extensions"></a>Installer les extensions

### <a name="install-extensions-manually"></a>Installer les extensions manuellement

Une fois que vous avez trouvé une extension à installer, utilisez la commande [az extension add](/cli/azure/extension#az_extension_add) pour l’obtenir. Si l’extension est répertoriée dans `az extension list-available`, vous pouvez installer l’extension par nom.

```azurecli-interactive
az extension add --name <extension-name>
```

Si l’extension provient d’une ressource externe ou si vous disposez d’un lien direct vers celle-ci, fournissez le chemin d’accès local ou l’URL source. L’extension _doit_ être un fichier de roue Python compilé.

```azurecli-interactive
az extension add --source <URL-or-path>
```

Une fois qu’une extension est installée, elle se trouve sous la valeur de la variable d’interpréteur de commandes `$AZURE_EXTENSION_DIR`. Si cette variable n’est pas définie, par défaut la valeur est `$HOME/.azure/cliextensions` sur Linux et macOS, et `%USERPROFILE%\.azure\cliextensions` sur Windows.

### <a name="install-extensions-automatically"></a>Installer les extensions automatiquement

À compter de la version `2.10.0`, quand vous exécutez une commande d’extension qui n’est pas installée, l’interface Azure CLI peut reconnaître la commande que vous exécutez et installer automatiquement l’extension. Cette fonctionnalité, appelée **installation dynamique**, est activée par configuration.
```azurecli-interactive
az config set extension.use_dynamic_install=yes_prompt
```

Utilisez la commande de configuration suivante pour activer l’installation dynamique sans invite.
```azurecli-interactive
az config set extension.use_dynamic_install=yes_without_prompt
```

Utilisez la commande de configuration suivante pour désactiver la fonctionnalité d’installation dynamique afin de rétablir le comportement par défaut. La commande d’extension retourne une erreur de commande introuvable si l’extension n’est pas installée.
```azurecli-interactive
az config set extension.use_dynamic_install=no
```

Par défaut, l’exécution d’une commande d’extension qui demande l’installation dynamique s’interrompt. Vous pouvez changer le comportement par défaut et faire en sorte que la commande se poursuive en affectant à la propriété `run_after_dynamic_install` la valeur `yes`.
```azurecli-interactive
az config set extension.run_after_dynamic_install=yes
```

## <a name="update-extensions"></a>Mettre à jour les extensions

Si une extension a été installée par nom, mettez-la à jour à l’aide de la commande [az extension update](/cli/azure/extension#az_extension_update).

```azurecli-interactive
az extension update --name <extension-name>
```

Sinon, il est possible de mettre à jour une extension à partir de la source, en suivant les instructions de la section [Installer les extensions](#install-extensions).

Si un nom d’extension ne peut pas être résolu par l’interface CLI, désinstallez cette extension et tentez de procéder à une réinstallation. L’extension aurait également pu faire partie de l’interface CLI de base.
Essayez de mettre à jour l’interface de ligne de commande en suivant les instructions de la section [Installer Azure CLI](install-azure-cli.md) et vérifiez que les commandes de l’extension ont été ajoutées.

## <a name="uninstall-extensions"></a>Désinstaller les extensions

Si vous n’avez plus besoin d’une extension, vous pouvez la supprimer avec la commande [az extension remove](/cli/azure/extension#az_extension_remove).

```azurecli-interactive
az extension remove --name <extension-name>
```

Vous pouvez également supprimer une extension manuellement en la supprimant de l’emplacement où elle a été installée. La variable d’interpréteur de commandes `$AZURE_EXTENSION_DIR` définit l’emplacement dans lequel sont installés les modules.
Si cette variable n’est pas définie, par défaut la valeur est `$HOME/.azure/cliextensions` sur Linux et macOS, et `%USERPROFILE%\.azure\cliextensions` sur Windows.

```bash
rm -rf $AZURE_EXTENSION_DIR/<extension-name>
```

## <a name="faq"></a>Questions fréquentes (FAQ)

Voici les réponses à d’autres questions courantes sur les extensions de CLI.

### <a name="what-file-formats-are-allowed-for-installation"></a>Quels sont les formats de fichiers autorisés pour l’installation ?

Actuellement, seuls les fichiers Wheel Python compilés peuvent être installés en tant qu’extensions.

### <a name="can-extensions-replace-existing-commands"></a>Les extensions peuvent-elles remplacer des commandes existantes ?

Oui. Les extensions peuvent remplacer des commandes existantes, mais avant l’exécution d’une commande qui a été remplacée, la CLI émet un avertissement.

### <a name="how-can-i-tell-if-an-extension-is-in-pre-release"></a>Comment puis-je savoir si une extension est en version préliminaire ?

Une documentation et un contrôle de version d’une extension s’afficheront si celle-ci est en version préliminaire. Microsoft publie souvent des préversions de commandes sous forme d’extensions CLI, avec la possibilité de les déplacer ultérieurement dans le produit principal de la CLI. Lorsque les commandes sont déplacées en dehors des extensions, vous devez désinstaller l’ancienne extension. 

### <a name="can-extensions-depend-upon-each-other"></a>Les extensions peuvent-elles dépendre les unes des autres ?

Non. Étant donné que l’interface CLI ne garantit pas un ordre de chargement, les dépendances peuvent ne pas être satisfaites. La suppression d’une extension n’affecte pas les autres.

### <a name="are-extensions-updated-along-with-the-cli"></a>Les extensions sont-elles mises à jour en même temps que la CLI ?

Non. Les extensions sont à mettre à jour séparément, comme décrit dans la section [Mettre à jour les extensions](#update-extensions).

### <a name="how-to-develop-our-own-extension"></a>Comment développer votre propre extension ?
Pour obtenir de l’aide, reportez-vous au dépôt officiel. [Azure/azure-cli-extensions](https://github.com/Azure/azure-cli/tree/master/doc/extensions)