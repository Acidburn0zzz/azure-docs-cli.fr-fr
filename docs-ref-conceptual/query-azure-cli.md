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
# <a name="use-jmespath-queries-with-azure-cli-20"></a><span data-ttu-id="625b0-103">Utiliser des requêtes JMESPath avec Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="625b0-103">Use JMESPath queries with Azure CLI 2.0</span></span>

<span data-ttu-id="625b0-104">Azure CLI 2.0 utilise l’argument `--query` pour exécuter une [requête JMESPath](http://jmespath.org) sur les résultats des commandes.</span><span class="sxs-lookup"><span data-stu-id="625b0-104">The Azure CLI 2.0 uses the `--query` argument to execute a [JMESPath query](http://jmespath.org) on the results of commands.</span></span> <span data-ttu-id="625b0-105">JMESPath est un langage de requête pour JSON, qui vous permet de sélectionner et de présenter des données depuis une sortie CLI.</span><span class="sxs-lookup"><span data-stu-id="625b0-105">JMESPath is a query language for JSON, giving you the ability to select and present data from CLI output.</span></span> <span data-ttu-id="625b0-106">Ces requêtes sont exécutées sur la sortie JSON, avant de réaliser toute mise en forme d’affichage.</span><span class="sxs-lookup"><span data-stu-id="625b0-106">These queries are executed on the JSON output, before performing any other display formatting.</span></span>

<span data-ttu-id="625b0-107">L’argument `--query` est pris en charge par toutes les commandes dans Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="625b0-107">The `--query` argument is supported by all commands in the Azure CLI.</span></span> <span data-ttu-id="625b0-108">Les exemples de cet article détaillent les cas d’usage courants et montrent comment utiliser les fonctionnalités de JMESPath.</span><span class="sxs-lookup"><span data-stu-id="625b0-108">This article's examples cover common use cases and demonstrate how to use the features of JMESPath.</span></span>

## <a name="work-with-dictionary-output"></a><span data-ttu-id="625b0-109">Utiliser la sortie du dictionnaire</span><span class="sxs-lookup"><span data-stu-id="625b0-109">Work with dictionary output</span></span>

<span data-ttu-id="625b0-110">Les commandes qui retournent un dictionnaire JSON ne peuvent être analysées que par leurs noms de clé.</span><span class="sxs-lookup"><span data-stu-id="625b0-110">Commands that return a JSON dictionary can be explored by their key names alone.</span></span> <span data-ttu-id="625b0-111">Les chemins d’accès de clé utilisent le caractère `.` comme séparateur.</span><span class="sxs-lookup"><span data-stu-id="625b0-111">Key paths use the `.` character as a separator.</span></span> <span data-ttu-id="625b0-112">L’exemple suivant extrait une liste des clés SSH publiques autorisées à se connecter à une machine virtuelle Linux :</span><span class="sxs-lookup"><span data-stu-id="625b0-112">The following example pulls a list of the public SSH keys allowed to connect to a Linux VM:</span></span>

```azurecli
az vm show -g QueryDemo -n TestVM --query osProfile.linuxConfiguration.ssh.publicKeys
```

<span data-ttu-id="625b0-113">Vous pouvez également obtenir plusieurs valeurs et les placer dans un tableau ordonné.</span><span class="sxs-lookup"><span data-stu-id="625b0-113">You can also get multiple values, putting them in an ordered array.</span></span> <span data-ttu-id="625b0-114">Le tableau ne dispose d’aucune information de clé, mais l’ordre des éléments qu’il contient correspond à l’ordre des clé demandées.</span><span class="sxs-lookup"><span data-stu-id="625b0-114">The array doesn't have any key information, but the order of the array's elements matches the order of the queried keys.</span></span> <span data-ttu-id="625b0-115">L’exemple suivant montre comment récupérer l’image Azure en donnant le nom et la taille du disque du système d’exploitation :</span><span class="sxs-lookup"><span data-stu-id="625b0-115">The following example shows how to retrieve the Azure image offering name and the size of the OS disk:</span></span>

```azurecli
az vm show -g QueryDemo -n TestVM --query 'storageProfile.[imageReference.offer, osDisk.diskSizeGb]'
```

```json
[
  "UbuntuServer",
  30
]
```

<span data-ttu-id="625b0-116">Si vous voulez des clés dans vos sorties, vous pouvez utiliser une syntaxe de dictionnaire alternative.</span><span class="sxs-lookup"><span data-stu-id="625b0-116">If you want keys in your output, you can use an alternate dictionary syntax.</span></span> <span data-ttu-id="625b0-117">La sélection d’éléments multiples dans un dictionnaire utilise le format `{displayKey:keyPath, ...}` pour filtrer dans l’expression JMESPath `keyPath`.</span><span class="sxs-lookup"><span data-stu-id="625b0-117">Multiple element selection into a dictionary uses the format `{displayKey:keyPath, ...}` to filter on the `keyPath` JMESPath expression.</span></span> <span data-ttu-id="625b0-118">Cela s’affiche dans la sortie en tant que `{displayKey: value}`.</span><span class="sxs-lookup"><span data-stu-id="625b0-118">This displays in the output as `{displayKey: value}`.</span></span> <span data-ttu-id="625b0-119">L’exemple suivant reprend la requête de l’exemple précédent, et la rend plus claire en assignant des clés à la sortie :</span><span class="sxs-lookup"><span data-stu-id="625b0-119">The next example takes the last example's query, and makes it clearer by assigning keys to the output:</span></span>

```azurecli
az vm show -g QueryDemo -n TestVM --query 'storageProfile.{image:imageReference.offer, diskSize:osDisk.diskSizeGb}'
```

```json
{
  "diskSize": 30,
  "image": "UbuntuServer"
}
```

<span data-ttu-id="625b0-120">Lors de l’affichage des informations dans le format de sortie `table`, l’affichage du dictionnaire est particulièrement utile.</span><span class="sxs-lookup"><span data-stu-id="625b0-120">When displaying information in the `table` output format, dictionary display is especially useful.</span></span> <span data-ttu-id="625b0-121">Ceci vous permet de définir vos propres en-têtes de colonne, rendant ainsi la sortie encore plus facile à lire.</span><span class="sxs-lookup"><span data-stu-id="625b0-121">This allows for setting your own column headers, making output even easier to read.</span></span> <span data-ttu-id="625b0-122">Pour en savoir plus sur les formats de sortie, consultez l’article [Formats de sortie pour les commandes Azure CLI 2.0](/cli/azure/format-output-azure-cli).</span><span class="sxs-lookup"><span data-stu-id="625b0-122">For more information on output formats, see [Output formats for Azure CLI 2.0 commands](/cli/azure/format-output-azure-cli).</span></span>

> [!NOTE]
> <span data-ttu-id="625b0-123">Certaines clés sont filtrées et non pas imprimées dans l’affichage de table.</span><span class="sxs-lookup"><span data-stu-id="625b0-123">Certain keys are filtered out and not printed in the table view.</span></span> <span data-ttu-id="625b0-124">Il s’agit des clés `id`, `type` et `etag`.</span><span class="sxs-lookup"><span data-stu-id="625b0-124">These keys are `id`, `type`, and `etag`.</span></span> <span data-ttu-id="625b0-125">Si vous avez besoin de voir ces informations, vous pouvez changer le nom de clé et éviter de filtrer.</span><span class="sxs-lookup"><span data-stu-id="625b0-125">If you need to see this information, you can change the key name and avoid filtering.</span></span>
>
> ```azurecli
> az vm show -g QueryDemo -n TestVM --query "{objectID:id}" -o table
> ```

## <a name="work-with-list-output"></a><span data-ttu-id="625b0-126">Utiliser la sortie de liste</span><span class="sxs-lookup"><span data-stu-id="625b0-126">Work with list output</span></span>

<span data-ttu-id="625b0-127">Les commandes CLI qui peuvent retourner plus d’une valeur renvoient toujours un tableau.</span><span class="sxs-lookup"><span data-stu-id="625b0-127">CLI commands that may return more than one value always return an array.</span></span> <span data-ttu-id="625b0-128">Il est possible d’accéder aux éléments des tableaux avec l’index, mais le même ordre n’est jamais garanti depuis la CLI.</span><span class="sxs-lookup"><span data-stu-id="625b0-128">Arrays can have their elements accessed by index, but there's never an order guarantee from the CLI.</span></span> <span data-ttu-id="625b0-129">La meilleure façon de demander un tableau de valeurs est de les aplatir avec l’opérateur `[]`.</span><span class="sxs-lookup"><span data-stu-id="625b0-129">The best way to query an array of values is to flatten them with the `[]` operator.</span></span> <span data-ttu-id="625b0-130">L’opérateur est écrit dans le tableau après la clé, ou comme le premier élément de l’expression.</span><span class="sxs-lookup"><span data-stu-id="625b0-130">The operator is written after the key for the array, or as the first element in the expression.</span></span> <span data-ttu-id="625b0-131">L’aplanissement exécute la requête contre chaque élément individuel du tableau, et place les valeurs résultantes dans un nouveau tableau.</span><span class="sxs-lookup"><span data-stu-id="625b0-131">Flattening runs the query following it against each individual element in the array, and places the resulting values into a new array.</span></span> <span data-ttu-id="625b0-132">L’exemple suivant imprime le nom et le système d’exploitation exécutés sur chaque machine virtuelle d’un groupe de ressources.</span><span class="sxs-lookup"><span data-stu-id="625b0-132">The following example prints out the name and OS running on each VM in a resource group.</span></span> 

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

<span data-ttu-id="625b0-133">Les tableaux qui font partie d’un chemin d’accès de clé peuvent également être aplatis.</span><span class="sxs-lookup"><span data-stu-id="625b0-133">Arrays that are part of a key path can be flattened as well.</span></span> <span data-ttu-id="625b0-134">Cet exemple montre une requête qui obtient les ID d’objet Azure pour les cartes d’interface réseau auxquelles une machine virtuelle est connectée.</span><span class="sxs-lookup"><span data-stu-id="625b0-134">This example demonstrates a query that gets the Azure object IDs for the NICs a VM is connected to.</span></span>

```azurecli
az vm show -g QueryDemo -n TestVM --query 'networkProfile.networkInterfaces[].id'
```

## <a name="filter-array-output-with-predicates"></a><span data-ttu-id="625b0-135">Filtrer une sortie de tableau avec prédicats</span><span class="sxs-lookup"><span data-stu-id="625b0-135">Filter array output with predicates</span></span>

<span data-ttu-id="625b0-136">JMESPath offre [des expressions de filtrage](http://jmespath.org/specification.html#filterexpressions) pour filtrer les données affichées.</span><span class="sxs-lookup"><span data-stu-id="625b0-136">JMESPath offers [filtering expressions](http://jmespath.org/specification.html#filterexpressions) to filter out the data displayed.</span></span> <span data-ttu-id="625b0-137">Ces expressions sont puissantes, surtout lorsqu’elles sont combinées avec des [fonctions intégrées JMESPath](http://jmespath.org/specification.html#built-in-functions) pour réaliser des correspondances partielles ou pour manipuler des données dans un format standard.</span><span class="sxs-lookup"><span data-stu-id="625b0-137">These expressions are powerful, especially when combined with [JMESPath built-in functions](http://jmespath.org/specification.html#built-in-functions) to perform partial matches or manipulate data into a standard format.</span></span> <span data-ttu-id="625b0-138">Le filtrage des expressions n’est possible que pour des données de tableau, et renvoie la valeur `null` lorsqu’il est utilisé dans d’autres situations.</span><span class="sxs-lookup"><span data-stu-id="625b0-138">Filtering expressions only work on array data, and when used in any other situation, return the `null` value.</span></span> <span data-ttu-id="625b0-139">Par exemple, vous pouvez choisir la sortie de commandes telle que `vm list` et la filtrer pour chercher des types spécifiques de machines virtuelles.</span><span class="sxs-lookup"><span data-stu-id="625b0-139">For example, you can take the output of commands like `vm list` and filter on it to look for specific types of VMs.</span></span> <span data-ttu-id="625b0-140">L’exemple suivant développe le précédent en filtrant le type de machine virtuelle pour obtenir uniquement les machines virtuelles Windows et imprimer leur nom.</span><span class="sxs-lookup"><span data-stu-id="625b0-140">The following example expands on the previous by filtering out the VM type to capture only Windows VMs and print their name.</span></span>

```azurecli
az vm list --query '[?osProfile.windowsConfiguration!=null].name'
```

```json
[
  "WinServ"
]
```

## <a name="experiment-with-queries-interactively"></a><span data-ttu-id="625b0-141">Essayer des requêtes de façon interactive</span><span class="sxs-lookup"><span data-stu-id="625b0-141">Experiment with queries interactively</span></span>

<span data-ttu-id="625b0-142">Pour essayer des expressions JMESPath, vous devrez travailler de façon à pouvoir modifier rapidement des requêtes et inspecter la sortie.</span><span class="sxs-lookup"><span data-stu-id="625b0-142">To experiment with JMESPath expressions, you might want to work in a way where you can quickly edit queries and inspect the output.</span></span> <span data-ttu-id="625b0-143">Un environnement interactif est offert par le package Python [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal), qui permet de conduire des données comme entrée avant d’écrire des requêtes dans le programme pour extraire les données.</span><span class="sxs-lookup"><span data-stu-id="625b0-143">An interactive environment is offered by the [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal) Python package, which allows for piping data as input and then writing in-program queries to extract the data.</span></span>

```bash
pip install jmespath-terminal
az vm list --output json | jpterm
```
