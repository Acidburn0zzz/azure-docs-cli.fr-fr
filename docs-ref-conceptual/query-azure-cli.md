---
title: "Interroger des résultats de commande avec Azure CLI 2.0"
description: "Apprenez à exécuter des requêtes JMESPath sur la sortie des commandes Azure CLI 2.0."
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 02/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 98bc35c1e8136231011a2303901f42c68c9a7758
ms.sourcegitcommit: b93a19222e116d5880bbe64c03507c64e190331e
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/15/2018
---
# <a name="use-jmespath-queries-with-azure-cli-20"></a><span data-ttu-id="d658a-103">Utiliser des requêtes JMESPath avec Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="d658a-103">Use JMESPath queries with Azure CLI 2.0</span></span>

<span data-ttu-id="d658a-104">Azure CLI 2.0 utilise le paramètre `--query` pour exécuter une [requête JMESPath](http://jmespath.org) sur les résultats de votre commande `az`.</span><span class="sxs-lookup"><span data-stu-id="d658a-104">The Azure CLI 2.0 uses the `--query` parameter to execute a [JMESPath query](http://jmespath.org) on the results of your `az` command.</span></span> <span data-ttu-id="d658a-105">JMESPath est un langage de requête puissant pour les sorties JSON.</span><span class="sxs-lookup"><span data-stu-id="d658a-105">JMESPath is a powerful query language for JSON outputs.</span></span>  <span data-ttu-id="d658a-106">Si vous n’avez pas une bonne connaissance des requêtes JMESPath, vous trouverez un didacticiel à l’adresse [JMESPath.org/tutorial](http://JMESPath.org/tutorial.html).</span><span class="sxs-lookup"><span data-stu-id="d658a-106">If you are unfamiliar with JMESPath queries you can find a tutorial at [JMESPath.org/tutorial](http://JMESPath.org/tutorial.html).</span></span>

<span data-ttu-id="d658a-107">Le paramètre `Query` est pris en charge par chaque type de ressource (conteneur de services, applications web, machines virtuelles, etc.) dans Azure CLI 2.0, et peut servir à différentes fins.</span><span class="sxs-lookup"><span data-stu-id="d658a-107">`Query` parameter is supported by every resource type (Container Services, Web Apps, VM, etc.) within Azure CLI 2.0 and can be used for various different purposes.</span></span>  <span data-ttu-id="d658a-108">Nous avons répertorié plusieurs exemples ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="d658a-108">We have listed several examples below.</span></span>

## <a name="select-simple-properties"></a><span data-ttu-id="d658a-109">Sélectionner des propriétés simples</span><span class="sxs-lookup"><span data-stu-id="d658a-109">Select simple properties</span></span>

<span data-ttu-id="d658a-110">La commande `list` simple avec le format de sortie `table` retourne un ensemble organisé des propriétés les plus simples pour chaque type de ressource dans un format tabulaire facile à lire.</span><span class="sxs-lookup"><span data-stu-id="d658a-110">The simple `list` command with `table` output format returns a curated set of most common, simple properties for each resource type in an easy-to-read tabular format.</span></span>

```azurecli-interactive
az vm list --out table
```

```
Name         ResourceGroup    Location
-----------  ---------------  ----------
DemoVM010    DEMORG1          westus
demovm212    DEMORG1          westus
demovm213    DEMORG1          westus
KBDemo001VM  RGDEMO001        westus
KBDemo020    RGDEMO001        westus
```

<span data-ttu-id="d658a-111">Vous pouvez utiliser le paramètre `--query` pour afficher uniquement le nom du groupe de ressources et le nom de la machine virtuelle pour toutes les machines virtuelles dans votre abonnement.</span><span class="sxs-lookup"><span data-stu-id="d658a-111">You can use the `--query` parameter to show just the Resource Group name and VM name for all virtual machines in your subscription.</span></span>

```azurecli-interactive
az vm list \
  --query "[].[name, resourceGroup]" --out table
```

```
Column1     Column2
---------   -----------
DemoVM010   DEMORG1
demovm111   DEMORG1
demovm211   DEMORG1
demovm212   DEMORG1
demovm213   DEMORG1
demovm214   DEMORG1
demovm222   DEMORG1
KBDemo001VM RGDEMO001
KBDemo020   RGDEMO001
```

<span data-ttu-id="d658a-112">Dans l’exemple précédent, vous remarquerez que les en-têtes de colonnes sont « Column1 » et « Column2 ».</span><span class="sxs-lookup"><span data-stu-id="d658a-112">In the previous example, you notice that the column headings are "Column1" and "Column2".</span></span>  <span data-ttu-id="d658a-113">Vous pouvez aussi ajouter des étiquettes ou des noms conviviaux aux propriétés que vous sélectionnez.</span><span class="sxs-lookup"><span data-stu-id="d658a-113">You can add friendly labels or names to the properties you select, as well.</span></span>  <span data-ttu-id="d658a-114">Dans l’exemple suivant, nous avons ajouté les étiquettes « VMName » et « RGName » aux propriétés sélectionnées « name » et « resourceGroup ».</span><span class="sxs-lookup"><span data-stu-id="d658a-114">In the following example, we added the labels "VMName" and "RGName" to the selected properties "name" and "resourceGroup".</span></span>


```azurecli-interactive
az vm list \
  --query "[].{RGName:resourceGroup, VMName:name}" --out table
```

```
RGName     VMName
---------  -----------
DEMORG1    DemoVM010
DEMORG1    demovm111
DEMORG1    demovm211
DEMORG1    demovm212
DEMORG1    demovm213
DEMORG1    demovm214
DEMORG1    demovm222
RGDEMO001  KBDemo001VM
RGDEMO001  KBDemo020
```

## <a name="select-complex-nested-properties"></a><span data-ttu-id="d658a-115">Sélectionner des propriétés imbriquées complexes</span><span class="sxs-lookup"><span data-stu-id="d658a-115">Select complex nested properties</span></span>

<span data-ttu-id="d658a-116">Si la propriété que vous souhaitez sélectionner est imbriquée en profondeur dans la sortie JSON, vous devez fournir le chemin complet à cette propriété imbriquée.</span><span class="sxs-lookup"><span data-stu-id="d658a-116">If the property you want to select is nested deep in the JSON output you need to supply the full path to that nested property.</span></span> <span data-ttu-id="d658a-117">L’exemple suivant montre comment sélectionner le nom de la machine virtuelle et le type de système d’exploitation à partir de la commande vm list.</span><span class="sxs-lookup"><span data-stu-id="d658a-117">The following example shows how to select the VMName and the OS type from the vm list command.</span></span>

```azurecli-interactive
az vm list \
  --query "[].{VMName:name, OSType:storageProfile.osDisk.osType}" --out table
```

```
VMName       OSType
-----------  --------
DemoVM010    Linux
demovm111    Linux
demovm211    Linux
demovm212    Linux
demovm213    Linux
demovm214    Linux
demovm222    Linux
KBDemo001VM  Linux
KBDemo020    Linux
```

## <a name="filter-with-the-contains-function"></a><span data-ttu-id="d658a-118">Filtrer avec la fonction contains</span><span class="sxs-lookup"><span data-stu-id="d658a-118">Filter with the contains function</span></span>

<span data-ttu-id="d658a-119">Vous pouvez utiliser la fonction `contains` de JMESPath pour affiner les résultats retournés par la requête.</span><span class="sxs-lookup"><span data-stu-id="d658a-119">You can use the JMESPath `contains` function to refine your results returned in the query.</span></span>
<span data-ttu-id="d658a-120">Dans l’exemple suivant, la commande sélectionne uniquement les machines virtuelles dont le nom contient le texte « RGD ».</span><span class="sxs-lookup"><span data-stu-id="d658a-120">In the following example, the command selects only VMs that have the text "RGD" in their name.</span></span>

```azurecli-interactive
az vm list \
  --query "[?contains(resourceGroup, 'RGD')].{ resource: resourceGroup, name: name }" --out table
```

```
Resource    VMName
----------  -----------
RGDEMO001   KBDemo001VM
RGDEMO001   KBDemo020
```

<span data-ttu-id="d658a-121">Dans l’exemple suivant, les résultats retournent les machines virtuelles dont la vmSize est « Standard_DS1 ».</span><span class="sxs-lookup"><span data-stu-id="d658a-121">With the next example, the results will return the VMs that have the vmSize 'Standard_DS1'.</span></span>

```azurecli-interactive
az vm list \
  --query "[?contains(hardwareProfile.vmSize, 'Standard_DS1')]" --out table
```

```
ResourceGroup    VMName     VmId                                  Location    ProvisioningState
---------------  ---------  ------------------------------------  ----------  -------------------
DEMORG1          DemoVM010  cbd56d9b-9340-44bc-a722-25f15b578444  westus      Succeeded
DEMORG1          demovm111  c1c024eb-3837-4075-9117-bfbc212fa7da  westus      Succeeded
DEMORG1          demovm211  95eda642-417f-4036-9475-67246ac0f0d0  westus      Succeeded
DEMORG1          demovm212  4bdac85d-c2f7-410f-9907-ca7921d930b4  westus      Succeeded
DEMORG1          demovm213  2131c664-221a-4b7f-9653-f6d542fbfa34  westus      Succeeded
DEMORG1          demovm214  48f419af-d27a-4df0-87f3-9481007c2e5a  westus      Succeeded
DEMORG1          demovm222  e0f59516-1d69-4d54-b8a2-f6c4a5d031de  westus      Succeeded
```

## <a name="filter-with-grep"></a><span data-ttu-id="d658a-122">Filtrer avec grep</span><span class="sxs-lookup"><span data-stu-id="d658a-122">Filter with grep</span></span>

<span data-ttu-id="d658a-123">Le format de sortie `tsv` est un texte séparé par des tabulations, sans en-tête.</span><span class="sxs-lookup"><span data-stu-id="d658a-123">The `tsv` output format is a tab-separated text with no headers.</span></span> <span data-ttu-id="d658a-124">Il peut être dirigé vers des commandes telles que `grep` et `cut` pour analyser plus en détail des valeurs spécifiques de la sortie `list`.</span><span class="sxs-lookup"><span data-stu-id="d658a-124">It can be piped to commands like `grep` and `cut` to further parse specific values out of the `list` output.</span></span> <span data-ttu-id="d658a-125">Dans l’exemple suivant, la commande `grep` sélectionne uniquement les machines virtuelles dont le nom contient le texte « RGD ».</span><span class="sxs-lookup"><span data-stu-id="d658a-125">In the following example, the `grep` command selects only VMs that have text "RGD" in their name.</span></span>  <span data-ttu-id="d658a-126">La commande `cut` sélectionne uniquement la valeur du huitième champ (séparé par des tabulations) à afficher dans la sortie.</span><span class="sxs-lookup"><span data-stu-id="d658a-126">The `cut` command selects only the 8th field (separated by tabs) value to show in the output.</span></span>

```azurecli-interactive
az vm list --out tsv | grep RGD | cut -f8
```

```
KBDemo001VM
KBDemo020
```

## <a name="explore-with-jpterm"></a><span data-ttu-id="d658a-127">Explorer avec jpterm</span><span class="sxs-lookup"><span data-stu-id="d658a-127">Explore with jpterm</span></span>

<span data-ttu-id="d658a-128">Vous pouvez également diriger la sortie de la commande vers [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal) et y faire des essais avec votre requête JMESPath.</span><span class="sxs-lookup"><span data-stu-id="d658a-128">You can also pipe the command output to [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal) and experiment with your JMESPath query there.</span></span>

```bash
pip install jmespath-terminal
az vm list | jpterm
```

