---
title: Interroger des résultats de commande avec Azure CLI 2.0
description: Apprenez à exécuter des requêtes JMESPath sur la sortie des commandes Azure CLI 2.0.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 02/22/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: eb9311686bf950a450db4bc450da363bbe409f49
ms.sourcegitcommit: ae72b6c8916aeb372a92188090529037e63930ba
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/28/2018
---
# <a name="use-jmespath-queries-with-azure-cli-20"></a>Utiliser des requêtes JMESPath avec Azure CLI 2.0

Azure CLI 2.0 utilise l’argument `--query` pour exécuter une [requête JMESPath](http://jmespath.org) sur les résultats des commandes. JMESPath est un langage de requête pour JSON, qui vous permet de sélectionner et de présenter des données depuis une sortie CLI. Ces requêtes sont exécutées sur la sortie JSON, avant de réaliser toute mise en forme d’affichage.

L’argument `--query` est pris en charge par toutes les commandes dans Azure CLI. Les exemples de cet article détaillent les cas d’usage courants et montrent comment utiliser les fonctionnalités de JMESPath.

## <a name="work-with-dictionary-output"></a>Utiliser la sortie du dictionnaire

Les commandes qui retournent un dictionnaire JSON ne peuvent être analysées que par leurs noms de clé. Les chemins d’accès de clé utilisent le caractère `.` comme séparateur. L’exemple suivant extrait une liste des clés SSH publiques autorisées à se connecter à une machine virtuelle Linux :

```azurecli
az vm show -g QueryDemo -n TestVM --query osProfile.linuxConfiguration.ssh.publicKeys
```

Vous pouvez également obtenir plusieurs valeurs et les placer dans un tableau ordonné. Le tableau ne dispose d’aucune information de clé, mais l’ordre des éléments qu’il contient correspond à l’ordre des clé demandées. L’exemple suivant montre comment récupérer l’image Azure en donnant le nom et la taille du disque du système d’exploitation :

```azurecli
az vm show -g QueryDemo -n TestVM --query 'storageProfile.[imageReference.offer, osDisk.diskSizeGb]'
```

```json
[
  "UbuntuServer",
  30
]
```

Si vous voulez des clés dans vos sorties, vous pouvez utiliser une syntaxe de dictionnaire alternative. La sélection d’éléments multiples dans un dictionnaire utilise le format `{displayKey:keyPath, ...}` pour filtrer dans l’expression JMESPath `keyPath`. Cela s’affiche dans la sortie en tant que `{displayKey: value}`. L’exemple suivant reprend la requête de l’exemple précédent, et la rend plus claire en assignant des clés à la sortie :

```azurecli
az vm show -g QueryDemo -n TestVM --query 'storageProfile.{image:imageReference.offer, diskSize:osDisk.diskSizeGb}'
```

```json
{
  "diskSize": 30,
  "image": "UbuntuServer"
}
```

Lors de l’affichage des informations dans le format de sortie `table`, l’affichage du dictionnaire est particulièrement utile. Ceci vous permet de définir vos propres en-têtes de colonne, rendant ainsi la sortie encore plus facile à lire. Pour en savoir plus sur les formats de sortie, consultez l’article [Formats de sortie pour les commandes Azure CLI 2.0](/cli/azure/format-output-azure-cli).

> [!NOTE]
> Certaines clés sont filtrées et non pas imprimées dans l’affichage de table. Il s’agit des clés `id`, `type` et `etag`. Si vous avez besoin de voir ces informations, vous pouvez changer le nom de clé et éviter de filtrer.
>
> ```azurecli
> az vm show -g QueryDemo -n TestVM --query "{objectID:id}" -o table
> ```

## <a name="work-with-list-output"></a>Utiliser la sortie de liste

Les commandes CLI qui peuvent retourner plus d’une valeur renvoient toujours un tableau. Il est possible d’accéder aux éléments des tableaux avec l’index, mais le même ordre n’est jamais garanti depuis la CLI. La meilleure façon de demander un tableau de valeurs est de les aplatir avec l’opérateur `[]`. L’opérateur est écrit dans le tableau après la clé, ou comme le premier élément de l’expression. L’aplanissement exécute la requête contre chaque élément individuel du tableau, et place les valeurs résultantes dans un nouveau tableau. L’exemple suivant imprime le nom et le système d’exploitation exécutés sur chaque machine virtuelle d’un groupe de ressources. 

```azurecli
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

Les tableaux qui font partie d’un chemin d’accès de clé peuvent également être aplatis. Cet exemple montre une requête qui obtient les ID d’objet Azure pour les cartes d’interface réseau auxquelles une machine virtuelle est connectée.

```azurecli
az vm show -g QueryDemo -n TestVM --query 'networkProfile.networkInterfaces[].id'
```

## <a name="filter-array-output-with-predicates"></a>Filtrer une sortie de tableau avec prédicats

JMESPath offre [des expressions de filtrage](http://jmespath.org/specification.html#filterexpressions) pour filtrer les données affichées. Ces expressions sont puissantes, surtout lorsqu’elles sont combinées avec des [fonctions intégrées JMESPath](http://jmespath.org/specification.html#built-in-functions) pour réaliser des correspondances partielles ou pour manipuler des données dans un format standard. Le filtrage des expressions n’est possible que pour des données de tableau, et renvoie la valeur `null` lorsqu’il est utilisé dans d’autres situations. Par exemple, vous pouvez choisir la sortie de commandes telle que `vm list` et la filtrer pour chercher des types spécifiques de machines virtuelles. L’exemple suivant développe le précédent en filtrant le type de machine virtuelle pour obtenir uniquement les machines virtuelles Windows et imprimer leur nom.

```azurecli
az vm list --query '[?osProfile.windowsConfiguration!=null].name'
```

```json
[
  "WinServ"
]
```

## <a name="experiment-with-queries-interactively"></a>Essayer des requêtes de façon interactive

Pour essayer des expressions JMESPath, vous devrez travailler de façon à pouvoir modifier rapidement des requêtes et inspecter la sortie. Un environnement interactif est offert par le package Python [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal), qui permet de conduire des données comme entrée avant d’écrire des requêtes dans le programme pour extraire les données.

```bash
pip install jmespath-terminal
az vm list --output json | jpterm
```
