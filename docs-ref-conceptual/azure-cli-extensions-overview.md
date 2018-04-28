---
title: Extensions Azure CLI 2.0
description: Utilisation d’extensions avec Azure CLI 2.0
keywords: Azure CLI, extensions
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 03/15/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 01d7b3d58bf24d5a30386564fb64630d4db055e3
ms.sourcegitcommit: ae72b6c8916aeb372a92188090529037e63930ba
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/28/2018
---
# <a name="using-extensions-with-the-azure-cli-20"></a>Utilisation d’extensions avec Azure CLI 2.0

Les extensions sont des modules individuels non fournis avec Azure CLI, qui ajoutent des fonctionnalités via de nouvelles commandes. Il peut s’agir d’offres expérimentales ou en version préliminaire, d’outils spécialisés de Microsoft, ou de fonctionnalités personnalisées que vous écrivez vous-même. Les extensions vous offrent un certain degré de flexibilité avec la CLI, ce qui vous permet de la modifier en fonction de vos besoins, sans avoir à fournir de nombreux packages supplémentaires n’étant pas considérés comme composants de l’ensemble de fonctionnalités principal.

Cet article va vous aider à comprendre comment installer, mettre à jour et supprimer des extensions pour l’interface CLI. Il répond également à des questions courantes sur le comportement des extensions.

## <a name="find-extensions"></a>Rechercher des extensions

Pour savoir quelles sont les extensions disponibles, vous pouvez utiliser la commande [az extension list-available](/cli/azure/extension#az-extension-list-available). Cette commande répertorie les extensions officielles fournies et gérées par Microsoft.

```azurecli
az extension list-available --output table
```

Nous hébergeons également une [liste des extensions Microsoft](azure-cli-extensions-list.md) sur le site de la documentation.

## <a name="install-extensions"></a>Installer les extensions

Une fois que vous avez trouvé une extension à installer, utilisez la commande [az extension add](https://docs.microsoft.com/en-us/cli/azure/extension#az-extension-add) pour l’obtenir. Si l’extension est répertoriée dans `az extension list-available`, vous pouvez installer l’extension par nom.

```azurecli
az extension add --name <extension-name>
```

Si l’extension provient d’une ressource externe ou si vous avez un lien direct vers celle-ci, vous pouvez fournir le chemin d’accès local ou l’URL source. Cela _doit_ être un fichier Wheel Python compilé.

```azurecli
az extension add --source <URL-or-path>
```

Une fois qu’une extension est installée, elle se trouve sous la valeur de la variable d’interpréteur de commandes `$AZURE_EXTENSION_DIR`. Si cette variable n’est pas définie, par défaut la valeur est `$HOME/.azure/cliextensions` sur Linux et macOS, et `%USERPROFILE%\.azure\cliextensions` sur Windows.

## <a name="update-extensions"></a>Mettre à jour les extensions

Si une extension a été installée par nom, elle peut être mise à jour à l’aide de la commande [az extension update](https://docs.microsoft.com/en-us/cli/azure/extension#az-extension-update).

```azurecli
az extension update --name <extension-name>
```

Sinon, il est possible de mettre à jour une extension à partir de la source, en suivant les instructions de la section [Installer les extensions](#install-extensions).

Si un nom d’extension ne peut pas être résolu par l’interface CLI, désinstallez-la et tentez de procéder à une réinstallation. Il est également possible que l’extension ait été déplacée de la version préliminaire pour devenir une commande intégrée pour l’interface CLI. Tentez de mettre à jour l’interface CLI en suivant les instructions de la section [Installer Azure CLI 2.0](install-azure-cli.md) et observez si les commandes de l’extension ont été ajoutées. 

## <a name="uninstall-extensions"></a>Désinstaller les extensions

Si vous n’avez plus besoin d’une extension, elle peut être supprimée avec la commande [az extension remove](https://docs.microsoft.com/en-us/cli/azure/extension#az-extension-remove).

```azurecli
az extension remove --name <extension-name>
```

Vous pouvez également supprimer une extension manuellement en la supprimant de l’emplacement où elle a été installée. Il s’agit de la valeur de la variable d’interpréteur de commandes `$AZURE_EXTENSION_DIR`. Si cette variable n’est pas définie, par défaut la valeur est `$HOME/.azure/cliextensions` sur Linux et macOS, et `%USERPROFILE%\.azure\cliextensions` sur Windows.

```bash
rm -rf $AZURE_EXTENSION_DIR/<extension-name>
```

Il est recommandé d’utiliser `az extension remove` pour les désinstallations.

## <a name="faq"></a>Forum Aux Questions

Voici les réponses à d’autres questions courantes sur les extensions de CLI.

### <a name="what-file-formats-are-allowed-for-installation"></a>Quels sont les formats de fichiers autorisés pour l’installation ?

Actuellement, seuls les fichiers Wheel Python compilés peuvent être installés en tant qu’extensions.

### <a name="can-extensions-replace-existing-commands"></a>Les extensions peuvent-elles remplacer des commandes existantes ?

Oui. Les extensions peuvent remplacer des commandes existantes, mais avant l’exécution d’une commande qui a été remplacée, la CLI émet un avertissement.

### <a name="how-can-i-tell-if-an-extension-is-in-pre-release"></a>Comment puis-je savoir si une extension est en version préliminaire ?

La documentation et le contrôle de version d’une extension doivent indiquer si celle-ci est en version préliminaire. Il est également commun pour Microsoft de publier des commandes en préversion pour la CLI en tant qu’extensions, avec des plans pour les migrer dans l’interface CLI principale une fois que le produit n’est plus en préversion.

### <a name="can-extensions-depend-upon-each-other"></a>Les extensions peuvent-elles dépendre les unes des autres ?

Non. Les extensions doivent être des packages individuels qui ne reposent pas les uns sur les autres. Cela s’explique par le fait que la CLI ne donne aucune garantie quant au moment où les extensions sont chargées, et ainsi le chargement des dépendances ne peut pas être garanti. En installant une extension, vous n’installez aucun autre élément, et celle-ci doit continuer à fonctionner même si vous supprimez d’autres extensions.

### <a name="are-extensions-updated-along-with-the-cli"></a>Les extensions sont-elles mises à jour en même temps que la CLI ?

Non. Les extensions sont à mettre à jour séparément, comme décrit dans la section [Mettre à jour les extensions](#update-extensions).
