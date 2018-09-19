---
title: Interroger des résultats de commande avec Azure CLI 2.0
description: Apprenez à exécuter des requêtes JMESPath sur la sortie des commandes Azure CLI 2.0.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 55880b87e1bffc37bbdeaeb84206deb5b9b7b227
ms.sourcegitcommit: 0e688704889fc88b91588bb6678a933c2d54f020
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/11/2018
ms.locfileid: "44388369"
---
# <a name="use-jmespath-queries-with-azure-cli-20"></a><span data-ttu-id="2dc31-103">Utiliser des requêtes JMESPath avec Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="2dc31-103">Use JMESPath queries with Azure CLI 2.0</span></span>

<span data-ttu-id="2dc31-104">Azure CLI 2.0 utilise l’argument `--query` pour exécuter une [requête JMESPath](http://jmespath.org) sur les résultats des commandes.</span><span class="sxs-lookup"><span data-stu-id="2dc31-104">The Azure CLI 2.0 uses the `--query` argument to execute a [JMESPath query](http://jmespath.org) on the results of commands.</span></span> <span data-ttu-id="2dc31-105">JMESPath est un langage de requête pour JSON, qui vous permet de sélectionner et de présenter des données depuis une sortie CLI.</span><span class="sxs-lookup"><span data-stu-id="2dc31-105">JMESPath is a query language for JSON, giving you the ability to select and present data from CLI output.</span></span> <span data-ttu-id="2dc31-106">Ces requêtes sont exécutées sur la sortie JSON, avant toute mise en forme de l’affichage.</span><span class="sxs-lookup"><span data-stu-id="2dc31-106">These queries are executed on the JSON output before any display formatting.</span></span>

<span data-ttu-id="2dc31-107">L’argument `--query` est pris en charge par toutes les commandes dans Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="2dc31-107">The `--query` argument is supported by all commands in the Azure CLI.</span></span> <span data-ttu-id="2dc31-108">Les exemples de cet article détaillent les cas d’usage courants et montrent comment utiliser les fonctionnalités de JMESPath.</span><span class="sxs-lookup"><span data-stu-id="2dc31-108">This article's examples cover common use cases and demonstrate how to use the features of JMESPath.</span></span>

## <a name="work-with-dictionary-output"></a><span data-ttu-id="2dc31-109">Utiliser la sortie du dictionnaire</span><span class="sxs-lookup"><span data-stu-id="2dc31-109">Work with dictionary output</span></span>

<span data-ttu-id="2dc31-110">Les commandes qui retournent un dictionnaire JSON ne peuvent être analysées que par leurs noms de clé.</span><span class="sxs-lookup"><span data-stu-id="2dc31-110">Commands that return a JSON dictionary can be explored by their key names alone.</span></span> <span data-ttu-id="2dc31-111">Les chemins d’accès de clé utilisent le caractère `.` comme séparateur.</span><span class="sxs-lookup"><span data-stu-id="2dc31-111">Key paths use the `.` character as a separator.</span></span> <span data-ttu-id="2dc31-112">L’exemple suivant extrait une liste des clés SSH publiques autorisées à se connecter à une machine virtuelle Linux :</span><span class="sxs-lookup"><span data-stu-id="2dc31-112">The following example pulls a list of the public SSH keys allowed to connect to a Linux VM:</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query osProfile.linuxConfiguration.ssh.publicKeys
```

<span data-ttu-id="2dc31-113">Plusieurs valeurs peuvent être placées dans un tableau ordonné.</span><span class="sxs-lookup"><span data-stu-id="2dc31-113">Multiple values can be put into an ordered array.</span></span> <span data-ttu-id="2dc31-114">L’exemple suivant montre comment récupérer l’image Azure en donnant le nom et la taille du disque du système d’exploitation :</span><span class="sxs-lookup"><span data-stu-id="2dc31-114">The following example shows how to retrieve the Azure image offering name and the size of the OS disk:</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query 'storageProfile.[imageReference.offer, osDisk.diskSizeGb]'
```

```json
[
  "UbuntuServer",
  30
]
```

<span data-ttu-id="2dc31-115">Si vous voulez des clés dans vos sorties, vous pouvez utiliser une syntaxe de dictionnaire alternative.</span><span class="sxs-lookup"><span data-stu-id="2dc31-115">If you want keys in your output, you can use an alternate dictionary syntax.</span></span>  <span data-ttu-id="2dc31-116">La sélection d’éléments dans un dictionnaire utilise le format `{displayKey:keyPath, ...}` pour filtrer dans l’expression JMESPath `keyPath`.</span><span class="sxs-lookup"><span data-stu-id="2dc31-116">Element selection into a dictionary uses the format `{displayKey:keyPath, ...}` to filter on the `keyPath` JMESPath expression.</span></span> <span data-ttu-id="2dc31-117">Dans les valeurs de sortie, les paires clé/valeur sont modifiées en `{displayKey: value}`.</span><span class="sxs-lookup"><span data-stu-id="2dc31-117">In the output values, the key/value pairs are changed to `{displayKey: value}`.</span></span> <span data-ttu-id="2dc31-118">L’exemple suivant reprend la requête de l’exemple précédent, et la rend plus claire en assignant des clés à la sortie :</span><span class="sxs-lookup"><span data-stu-id="2dc31-118">The next example takes the last example's query, and makes it clearer by assigning keys to the output:</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query 'storageProfile.{image:imageReference.offer, diskSize:osDisk.diskSizeGb}'
```

```json
{
  "diskSize": 30,
  "image": "UbuntuServer"
}
```

<span data-ttu-id="2dc31-119">Lors de l’affichage des informations dans le format de sortie `table`, l’affichage du dictionnaire vous permet de paramétrer vos propres en-têtes de colonnes.</span><span class="sxs-lookup"><span data-stu-id="2dc31-119">When displaying information in the `table` output format, dictionary display allows setting your own column headers.</span></span> <span data-ttu-id="2dc31-120">Pour en savoir plus sur les formats de sortie, consultez l’article [Formats de sortie pour les commandes Azure CLI 2.0](/cli/azure/format-output-azure-cli).</span><span class="sxs-lookup"><span data-stu-id="2dc31-120">For more information on output formats, see [Output formats for Azure CLI 2.0 commands](/cli/azure/format-output-azure-cli).</span></span>

> [!NOTE]
> <span data-ttu-id="2dc31-121">Certaines clés sont filtrées et non pas imprimées dans l’affichage de table.</span><span class="sxs-lookup"><span data-stu-id="2dc31-121">Certain keys are filtered out and not printed in the table view.</span></span> <span data-ttu-id="2dc31-122">Il s’agit des clés `id`, `type` et `etag`.</span><span class="sxs-lookup"><span data-stu-id="2dc31-122">These keys are `id`, `type`, and `etag`.</span></span> <span data-ttu-id="2dc31-123">Si vous avez besoin de voir ces informations, vous pouvez changer le nom de clé et éviter de filtrer.</span><span class="sxs-lookup"><span data-stu-id="2dc31-123">If you need to see this information, you can change the key name and avoid filtering.</span></span>
>
> ```azurecli
> az vm show -g QueryDemo -n TestVM --query "{objectID:id}" -o table
> ```

## <a name="work-with-list-output"></a><span data-ttu-id="2dc31-124">Utiliser la sortie de liste</span><span class="sxs-lookup"><span data-stu-id="2dc31-124">Work with list output</span></span>

<span data-ttu-id="2dc31-125">Les commandes CLI qui peuvent retourner plus d’une valeur renvoient un tableau.</span><span class="sxs-lookup"><span data-stu-id="2dc31-125">CLI commands that may return  more than one value return an array.</span></span> <span data-ttu-id="2dc31-126">Les éléments de tableau sont accessibles par index et peuvent ne pas être retournés dans le même ordre à chaque fois.</span><span class="sxs-lookup"><span data-stu-id="2dc31-126">Array elements are accessed by index and may not be returned in the same order every time.</span></span> <span data-ttu-id="2dc31-127">Vous pouvez interroger tous les éléments de tableau à la fois en les aplanissant avec l’opérateur `[]`.</span><span class="sxs-lookup"><span data-stu-id="2dc31-127">You can query all array elements at once by flattening them with the `[]` operator.</span></span> <span data-ttu-id="2dc31-128">L’opérateur est placé après le tableau, ou en tant que premier élément dans une expression.</span><span class="sxs-lookup"><span data-stu-id="2dc31-128">The operator is put after the array or as the first element in an expression.</span></span> <span data-ttu-id="2dc31-129">La mise à plat d’un tableau exécute la requête après celle-ci pour chaque élément du tableau.</span><span class="sxs-lookup"><span data-stu-id="2dc31-129">Flattening an array runs the query after it against each element of the array.</span></span>

<span data-ttu-id="2dc31-130">L’exemple suivant imprime le nom et le système d’exploitation exécutés sur chaque machine virtuelle d’un groupe de ressources.</span><span class="sxs-lookup"><span data-stu-id="2dc31-130">The following example prints out the name and OS running on each VM in a resource group.</span></span>

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

<span data-ttu-id="2dc31-131">Les tableaux qui font partie d’un chemin d’accès de clé peuvent également être aplatis.</span><span class="sxs-lookup"><span data-stu-id="2dc31-131">Arrays that are part of a key path can be flattened as well.</span></span> <span data-ttu-id="2dc31-132">La requête suivante reçoit les ID d’objet Azure pour les cartes d’interface réseau auxquelles une machine virtuelle est connectée.</span><span class="sxs-lookup"><span data-stu-id="2dc31-132">The following query gets the Azure object IDs for the NICs a VM is connected to.</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query 'networkProfile.networkInterfaces[].id'
```

## <a name="filter-array-output-with-predicates"></a><span data-ttu-id="2dc31-133">Filtrer une sortie de tableau avec prédicats</span><span class="sxs-lookup"><span data-stu-id="2dc31-133">Filter array output with predicates</span></span>

<span data-ttu-id="2dc31-134">JMESPath offre [des expressions de filtrage](http://jmespath.org/specification.html#filterexpressions) pour filtrer les données affichées.</span><span class="sxs-lookup"><span data-stu-id="2dc31-134">JMESPath offers [filtering expressions](http://jmespath.org/specification.html#filterexpressions) to filter out the data displayed.</span></span> <span data-ttu-id="2dc31-135">Ces expressions sont puissantes, surtout lorsqu’elles sont combinées avec des [fonctions intégrées JMESPath](http://jmespath.org/specification.html#built-in-functions) pour effectuer des correspondances partielles ou pour manipuler des données dans un format standard.</span><span class="sxs-lookup"><span data-stu-id="2dc31-135">These expressions are powerful, especially when combined with [JMESPath built-in functions](http://jmespath.org/specification.html#built-in-functions) to do partial matches or manipulate data into a standard format.</span></span> <span data-ttu-id="2dc31-136">Le filtrage des expressions n’est possible que pour des données de tableau, et renvoie la valeur `null` lorsqu’il est utilisé dans d’autres situations.</span><span class="sxs-lookup"><span data-stu-id="2dc31-136">Filtering expressions only work on array data, and when used in any other situation, return the `null` value.</span></span> <span data-ttu-id="2dc31-137">Par exemple, vous pouvez choisir la sortie de commandes telle que `vm list` et la filtrer pour chercher des types spécifiques de machines virtuelles.</span><span class="sxs-lookup"><span data-stu-id="2dc31-137">For example, you can take the output of commands like `vm list` and filter on it to look for specific types of VMs.</span></span> <span data-ttu-id="2dc31-138">L’exemple suivant développe le précédent en filtrant le type de machine virtuelle pour obtenir uniquement les machines virtuelles Windows et imprimer leur nom.</span><span class="sxs-lookup"><span data-stu-id="2dc31-138">The following example expands on the previous by filtering out the VM type to capture only Windows VMs and print their name.</span></span>

```azurecli-interactive
az vm list --query '[?osProfile.windowsConfiguration!=null].name'
```

```json
[
  "WinServ"
]
```

## <a name="experiment-with-queries-interactively"></a><span data-ttu-id="2dc31-139">Essayer des requêtes de façon interactive</span><span class="sxs-lookup"><span data-stu-id="2dc31-139">Experiment with queries interactively</span></span>

<span data-ttu-id="2dc31-140">Pour commencer à découvrir JMESPath, le package Python [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal) propose un environnement interactif permettant de faire des essais avec des requêtes.</span><span class="sxs-lookup"><span data-stu-id="2dc31-140">To start learning JMESPath, the [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal) Python package offers an interactive environment to experiment with queries.</span></span> <span data-ttu-id="2dc31-141">Les données sont transmises en tant qu’entrée, les requêtes dans le programme sont ensuite écrites et modifiées pour extraire les données.</span><span class="sxs-lookup"><span data-stu-id="2dc31-141">Data is piped as input, and then in-program queries are written and edited to extract the data.</span></span>

```bash
pip install jmespath-terminal
az vm list --output json | jpterm
```
