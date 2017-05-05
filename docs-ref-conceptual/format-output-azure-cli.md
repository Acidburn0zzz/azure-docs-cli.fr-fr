---
title: Formats de sortie pour Azure CLI 2.0
description: Utilisez --output pour mettre la sortie des commandes Azure CLI 2.0 au format liste, table ou json.
keywords: Azure CLI 2.0, sortie, format, table, liste, json, Linux, Mac, Windows, OS X
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 02/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: 74bdb727-481d-45f7-a44e-15d18dc55483
ms.openlocfilehash: de37b1ad6aa55c9ac73b5b6b89d9507c86cc1245
ms.sourcegitcommit: bcf93ad8ed8802072249cd8187cd4420da89b4c6
translationtype: HT
---
# <a name="output-formats-for-azure-cli-20-commands"></a>Formats de sortie pour les commandes Azure CLI 2.0

Azure CLI 2.0 utilise json comme option de sortie par défaut, mais vous pouvez mettre en forme la sortie des commandes de différentes façons.  Utilisez le paramètre `--output` (ou `--out` ou `-o`) pour mettre en forme la sortie de la commande avec l’un des types de sortie indiqués dans le tableau suivant. 

--output | Description
---------|-------------------------------
`json`   | Chaîne JSON. `json` est la valeur par défaut.
`jsonc`  | Chaîne json colorée.
`table`  | Table avec en-têtes de colonnes.
`tsv`    | Valeurs séparées par des tabulations.

## <a name="using-the-json-option"></a>Utilisation de l’option json

L’exemple suivant affiche la liste des machines virtuelles dans vos abonnements au format json par défaut.

```azurecli
az vm list --output json
```

Les résultats sont affichés au format suivant (affiche uniquement des résultats partiels, par souci de clarté).

```json
[
  {
    "availabilitySet": null,
    "diagnosticsProfile": null,
    "hardwareProfile": {
      "vmSize": "Standard_DS1"
    },
    "id": "/subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/DemoVM010",
    "instanceView": null,
    "licenseType": null,
    "location": "westus",
    "name": "DemoVM010",
    "networkProfile": {
      "networkInterfaces": [
        {
          "id": "/subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/demorg1/providers/Microsoft.Network/networkInterfaces/DemoVM010VMNic",
          "primary": null,
          "resourceGroup": "demorg1"
        }
      ]
    },
          ...
          ...
          ...   
]
```
 
## <a name="using-the-table-option"></a>Utilisation de l’option table

L’option table fournit une sortie facile à lire, mais notez que les objets imbriqués ne sont pas inclus dans la sortie avec la commande simple `--output table`, contrairement à l’exemple .json précédent.  L’utilisation du même exemple avec le format de sortie « table » fournit une liste organisée des valeurs de propriété les plus courantes.

```azurecli
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

Vous pouvez utiliser le paramètre `--query` pour personnaliser les propriétés et les colonnes à afficher dans la liste générée. L’exemple suivant montre comment sélectionner uniquement le nom de la machine virtuelle et le nom du groupe de ressources dans la commande `list`.

```azurecli
az vm list --query "[].{ resource: resourceGroup, name: name }" -o table
```

```
Resource    Name
----------  -----------
DEMORG1     DemoVM010
DEMORG1     demovm212
DEMORG1     demovm213
RGDEMO001   KBDemo001VM
RGDEMO001   KBDemo020
```

## <a name="using-the-tsv-option"></a>Utilisation de l’option tsv

Le format de sortie « tsv » retourne une sortie texte simple et séparée par des tabulations, sans en-tête ni tiret. Avec ce format, il est facile de consommer la sortie dans d’autres commandes et outils qui ont besoin de traiter le texte dans une forme donnée. L’exécution de l’exemple précédent avec l’option `tsv` retourne le résultat séparé par des tabulations.

```azurecli
az vm list --out tsv
```

```
None    None        /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/DemoVM010    None    None    westus    DemoVM010            None    Succeeded    DEMORG1    None            Microsoft.Compute/virtualMachines    cbd56d9b-9340-44bc-a722-25f15b578444
None    None        /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm212    None    None    westus    demovm212            None    Succeeded    DEMORG1    None            Microsoft.Compute/virtualMachines    4bdac85d-c2f7-410f-9907-ca7921d930b4
None    None        /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm213    None    None    westus    demovm213            None    Succeeded    DEMORG1    None            Microsoft.Compute/virtualMachines    2131c664-221a-4b7f-9653-f6d542fbfa34
None    None        /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo001VM    None    None    westus    KBDemo001VM            None    Succeeded    RGDEMO001    None            Microsoft.Compute/virtualMachines    14e74761-c17e-4530-a7be-9e4ff06ea74b
None    None        /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo02None    None    westus    KBDemo020            None    Succeeded    RGDEMO001    None            Microsoft.Compute/virtualMachinesed36baa9-9b80-48a8-b4a9-854c7a858ece
```

L’exemple suivant montre comment la sortie `tsv` peut être dirigée vers des commandes telles que `grep` et `cut` pour analyser plus en détail des valeurs spécifiques de la sortie `list`. La commande `grep` sélectionne uniquement les éléments contenant le texte « RGD », puis la commande `cut` sélectionne uniquement la valeur du huitième champ (séparé par des tabulations) pour l’afficher dans la sortie.

```azurecli
az vm list --out tsv | grep RGD | cut -f8
```

```
KBDemo001VM
KBDemo020
```

## <a name="setting-the-default-output-format"></a>Définition du format de sortie par défaut

Vous pouvez utiliser la commande `az configure` pour configurer votre environnement ou établir des préférences telles que les paramètres par défaut pour les formats de sortie. Pour une utilisation courante, le format de sortie par défaut le plus simple est le format « table » : sélectionnez **3** quand vous êtes invité à choisir le format de sortie. 

```
What default output format would you like?
 [1] json - JSON formatted output that most closely matches API responses
 [2] jsonc - Colored JSON formatted output that most closely matches API responses
 [3] table - Human-readable output format
 [4] tsv - Tab and Newline delimited, great for GREP, AWK, etc.
Please enter a choice [3]: 
```