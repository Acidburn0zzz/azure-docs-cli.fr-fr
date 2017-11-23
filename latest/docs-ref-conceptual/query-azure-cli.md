---
title: "Interroger des résultats de commande avec Azure CLI 2.0"
description: "Utilisez --query pour exécuter des requêtes JMESPath sur la sortie des commandes Azure CLI 2.0."
keywords: "Azure CLI 2.0, JMESPath, requête, Linux, Mac, Windows, OS X"
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 02/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: 5979acc5-21a5-41e2-a4b6-3183bfe6aa22
ms.openlocfilehash: 8ab4a5e38f06199c5f044b8526c581828ba61927
ms.sourcegitcommit: 0149f195a0d9f0ea9b7ff5c6e00ad4242223a1a8
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/18/2017
---
# <a name="using-jmespath-queries-with-azure-cli-20"></a>Utilisation de requêtes JMESPath avec Azure CLI 2.0

Azure CLI 2.0 utilise le paramètre `--query` pour exécuter une [requête JMESPath](http://jmespath.org) sur les résultats de votre commande `az`. JMESPath est un langage de requête puissant pour les sorties JSON.  Si vous n’avez pas une bonne connaissance des requêtes JMESPath, vous trouverez un didacticiel à l’adresse [JMESPath.org/tutorial](http://JMESPath.org/tutorial.html).

Le paramètre `Query` est pris en charge par chaque type de ressource (conteneur de services, applications web, machines virtuelles, etc.) dans Azure CLI 2.0, et peut servir à différentes fins.  Nous avons répertorié plusieurs exemples ci-dessous.

## <a name="selecting-simple-properties"></a>Sélection de propriété simple

La commande `list` simple avec le format de sortie `table` retourne un ensemble organisé des propriétés les plus simples pour chaque type de ressource dans un format tabulaire facile à lire.

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

Vous pouvez utiliser le paramètre `--query` pour afficher uniquement le nom du groupe de ressources et le nom de la machine virtuelle pour toutes les machines virtuelles dans votre abonnement.

```azurecli-interactive
az vm list \
  --query [*].[name, resourceGroup] --out table
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

Dans l’exemple précédent, vous remarquerez que les en-têtes de colonnes sont « Column1 » et « Column2 ».  Vous pouvez aussi ajouter des étiquettes ou des noms conviviaux aux propriétés que vous sélectionnez.  Dans l’exemple suivant, nous avons ajouté les étiquettes « VMName » et « RGName » aux propriétés sélectionnées « name » et « resourceGroup ».


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

## <a name="selecting-complex-nested-properties"></a>Sélection de propriétés imbriquées complexes

Si la propriété que vous souhaitez sélectionner est imbriquée en profondeur dans la sortie JSON, vous devez fournir le chemin complet à cette propriété imbriquée. L’exemple suivant montre comment sélectionner le nom de la machine virtuelle et le type de système d’exploitation à partir de la commande vm list.

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

## <a name="filter-with-the-contains-function"></a>Filtrer avec la fonction contains

Vous pouvez utiliser la fonction `contains` de JMESPath pour affiner les résultats retournés par la requête.
Dans l’exemple suivant, la commande sélectionne uniquement les machines virtuelles dont le nom contient le texte « RGD ».  

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

Dans l’exemple suivant, les résultats retournent les machines virtuelles dont la vmSize est « Standard_DS1 ».

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

## <a name="filter-with-grep"></a>Filtrer avec grep

Le format de sortie `tsv` est un texte séparé par des tabulations, sans en-tête. Il peut être dirigé vers des commandes telles que `grep` et `cut` pour analyser plus en détail des valeurs spécifiques de la sortie `list`. Dans l’exemple suivant, la commande `grep` sélectionne uniquement les machines virtuelles dont le nom contient le texte « RGD ».  La commande `cut` sélectionne uniquement la valeur du huitième champ (séparé par des tabulations) à afficher dans la sortie.

```azurecli-interactive
az vm list --out tsv | grep RGD | cut -f8
```

```
KBDemo001VM
KBDemo020
```

## <a name="explore-with-jpterm"></a>Explorer avec jpterm

Vous pouvez également diriger la sortie de la commande vers [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal) et y faire des essais avec votre requête JMESPath.

```bash
pip install jmespath-terminal
az vm list | jpterm
```

