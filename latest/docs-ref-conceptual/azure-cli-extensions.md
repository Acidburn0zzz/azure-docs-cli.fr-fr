---
title: Extensions Azure CLI 2.0
description: "Utilisation d’extensions avec Azure CLI 2.0"
keywords: Azure CLI, extensions
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 10/30/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 930073324d68f9719ce5035388120e7b6ac41a98
ms.sourcegitcommit: 93f6bd2c199774fcb3b43c6b14d714196873ed04
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/07/2017
---
# <a name="using-extensions-with-the-azure-cli-20"></a>Utilisation d’extensions avec Azure CLI 2.0

Les extensions sont des modules individuels non fournis avec Azure CLI, qui vous permettent d’ajouter des fonctionnalités via de nouvelles commandes. Il peut s’agir d’offres expérimentales ou en version préliminaire, d’outils spécialisés de Microsoft correspondant à vos besoins ou encore d’extensions que vous avez vous-même écrites. Les extensions vous offrent un certain degré de flexibilité avec la CLI, ce qui vous permet de la modifier en fonction de vos besoins, sans avoir à fournir de nombreux packages supplémentaires n’étant pas considérés comme composants de l’ensemble de fonctionnalités principal.

Cet article va vous aider à comprendre comment installer, mettre à jour et supprimer des extensions pour la CLI. Il doit également apporter des réponses à des questions courantes sur le comportement des extensions.

## <a name="finding-extensions"></a>Recherche d’extensions

Pour savoir quelles sont les extensions disponibles, vous pouvez utiliser `az extension list-available`. Cette commande répertorie les extensions officielles et disponibles qui sont fournies et prises en charge par Microsoft.

## <a name="installing-extensions"></a>Installation des extensions

Une fois que vous avez trouvé une extension à installer, utilisez `az extension add` pour l’obtenir. Si l’extension est une extension Microsoft officielle répertoriée dans `az extension list-available`, vous pouvez installer l’extension par nom.

```azurecli
az extension add --name <extension-name>
```

Si l’extension provient d’une ressource externe ou si vous avez un lien direct vers celle-ci, vous pouvez fournir le chemin d’accès local ou l’URL source. Cela _doit_ être un fichier Wheel Python compilé.

```azurecli
az extension add --source <URL-or-path>
```

Une fois qu’une extension est installée, elle se trouve sous la valeur de la variable d’interpréteur de commandes `$AZURE_EXTENSION_DIR`. Si cette variable n’est pas définie, par défaut la valeur est `$HOME/.azure/cliextensions` sur Linux et macOS, et `%USERPROFILE%\.azure\cliextensions` sur Windows.

## <a name="updating-extensions"></a>Mise à jour des extensions

Les extensions peuvent uniquement être mises à jour par nom :

```azurecli
az extension update --name <extension-name>
```

Si le nom d’une extension ne peut pas être résolu par la CLI pour une raison quelconque, réinstallez l’extension pour la mettre à jour. Il est également possible que l’extension ne soit plus en préversion, mais qu’elle soit devenue une commande intégrée de la CLI. Dans ce cas, mettez la CLI à jour et désinstallez l’extension.

## <a name="uninstalling-extensions"></a>Désinstallation des extensions

Si vous n’avez plus besoin d’une extension, elle peut être supprimée avec `az extension remove`.

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

Non. Les extensions doivent être mises à jour séparément, comme décrit dans la section [Mise à jour des extensions](#updating-extensions).
