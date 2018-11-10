---
title: Interroger des résultats de commande avec Azure CLI
description: Apprenez à exécuter des requêtes JMESPath sur la sortie des commandes Azure CLI.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 1736d1677fb6c7fc83a092493e8706c2d5edfccd
ms.sourcegitcommit: 0d6b08048b5b35bf0bb3d7b91ff567adbaab2a8b
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/07/2018
ms.locfileid: "51222529"
---
# <a name="use-jmespath-queries-with-azure-cli"></a>Utiliser des requêtes JMESPath avec Azure CLI 

Azure CLI utilise l’argument `--query` pour exécuter une [requête JMESPath](http://jmespath.org) sur les résultats des commandes. JMESPath est un langage de requête pour JSON, qui vous permet de sélectionner et de présenter des données depuis une sortie CLI. Ces requêtes sont exécutées sur la sortie JSON, avant toute mise en forme de l’affichage.

L’argument `--query` est pris en charge par toutes les commandes dans Azure CLI. Les exemples de cet article détaillent les cas d’usage courants et montrent comment utiliser les fonctionnalités de JMESPath.

## <a name="work-with-dictionary-output"></a>Utiliser la sortie du dictionnaire

Les commandes qui retournent un dictionnaire JSON ne peuvent être analysées que par leurs noms de clé. Les chemins d’accès de clé utilisent le caractère `.` comme séparateur. L’exemple suivant extrait une liste des clés SSH publiques autorisées à se connecter à une machine virtuelle Linux :

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query osProfile.linuxConfiguration.ssh.publicKeys
```

Plusieurs valeurs peuvent être placées dans un tableau ordonné. L’exemple suivant montre comment récupérer l’image Azure en donnant le nom et la taille du disque du système d’exploitation :

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query 'storageProfile.[imageReference.offer, osDisk.diskSizeGb]'
```

```json
[
  "UbuntuServer",
  30
]
```

Si vous voulez des clés dans vos sorties, vous pouvez utiliser une syntaxe de dictionnaire alternative.  La sélection d’éléments dans un dictionnaire utilise le format `{displayKey:keyPath, ...}` pour filtrer dans l’expression JMESPath `keyPath`. Dans les valeurs de sortie, les paires clé/valeur sont modifiées en `{displayKey: value}`. L’exemple suivant reprend la requête de l’exemple précédent, et la rend plus claire en assignant des clés à la sortie :

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query 'storageProfile.{image:imageReference.offer, diskSize:osDisk.diskSizeGb}'
```

```json
{
  "diskSize": 30,
  "image": "UbuntuServer"
}
```

Lors de l’affichage des informations dans le format de sortie `table`, l’affichage du dictionnaire vous permet de paramétrer vos propres en-têtes de colonnes. Pour en savoir plus sur les formats de sortie, consultez l’article [Formats de sortie pour les commandes Azure CLI](/cli/azure/format-output-azure-cli).

> [!NOTE]
> Certaines clés sont filtrées et non pas imprimées dans l’affichage de table. Il s’agit des clés `id`, `type` et `etag`. Si vous avez besoin de voir ces informations, vous pouvez changer le nom de clé et éviter de filtrer.
>
> ```azurecli-interactive
> az vm show -g QueryDemo -n TestVM --query "{objectID:id}" -o table
> ```

## <a name="work-with-list-output"></a>Utiliser la sortie de liste

Les commandes CLI qui peuvent retourner plus d’une valeur renvoient un tableau. Les éléments de tableau sont accessibles par index et peuvent ne pas être retournés dans le même ordre à chaque fois. Vous pouvez interroger tous les éléments de tableau à la fois en les aplanissant avec l’opérateur `[]`. L’opérateur est placé après le tableau, ou en tant que premier élément dans une expression. La mise à plat d’un tableau exécute la requête après celle-ci pour chaque élément du tableau.

L’exemple suivant imprime le nom et le système d’exploitation exécutés sur chaque machine virtuelle d’un groupe de ressources.

```azurecli-interactive
az vm list -g QueryDemo --query '[].{name:name, image:storageProfile.imageReference.offer}'
```

```json
[
  {
    "image": "CentOS",
    "name": "CentBox"
  },
  {
    "image": "openSUSE-Leap",
    "name": "SUSEBox"
  },
  {
    "image": "UbuntuServer",
    "name": "TestVM"
  },
  {
    "image": "UbuntuServer",
    "name": "Test2"
  },
  {
    "image": "WindowsServer",
    "name": "WinServ"
  }
]
```

Les tableaux qui font partie d’un chemin d’accès de clé peuvent également être aplatis. La requête suivante reçoit les ID d’objet Azure pour les cartes d’interface réseau auxquelles une machine virtuelle est connectée.

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query 'networkProfile.networkInterfaces[].id'
```

## <a name="filter-array-output-with-predicates"></a>Filtrer une sortie de tableau avec prédicats

JMESPath offre [des expressions de filtrage](http://jmespath.org/specification.html#filterexpressions) pour filtrer les données affichées. Ces expressions sont puissantes, surtout lorsqu’elles sont combinées avec des [fonctions intégrées JMESPath](http://jmespath.org/specification.html#built-in-functions) pour effectuer des correspondances partielles ou pour manipuler des données dans un format standard. Le filtrage des expressions n’est possible que pour des données de tableau, et renvoie la valeur `null` lorsqu’il est utilisé dans d’autres situations. Par exemple, vous pouvez choisir la sortie de commandes telle que `vm list` et la filtrer pour chercher des types spécifiques de machines virtuelles. L’exemple suivant développe le précédent en filtrant le type de machine virtuelle pour obtenir uniquement les machines virtuelles Windows et imprimer leur nom.

```azurecli-interactive
az vm list --query '[?osProfile.windowsConfiguration!=null].name'
```

```json
[
  "WinServ"
]
```

## <a name="experiment-with-queries-interactively"></a>Essayer des requêtes de façon interactive

Pour commencer à découvrir JMESPath, le package Python [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal) propose un environnement interactif permettant de faire des essais avec des requêtes. Les données sont transmises en tant qu’entrée, les requêtes dans le programme sont ensuite écrites et modifiées pour extraire les données.

```bash
pip install jmespath-terminal
az vm list --output json | jpterm
```
