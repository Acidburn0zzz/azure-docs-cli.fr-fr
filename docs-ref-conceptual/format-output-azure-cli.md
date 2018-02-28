---
title: Formats de sortie pour Azure CLI 2.0
description: "Apprenez à mettre la sortie des commandes Azure CLI 2.0 au format liste, table ou json."
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 02/15/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: ec96d1cb21b32cd982dbec5e4bf38110f8686c25
ms.sourcegitcommit: f82774a6f92598c41da9956284f563757f402774
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/19/2018
---
# <a name="output-formats-for-azure-cli-20-commands"></a>Formats de sortie pour les commandes Azure CLI 2.0

Azure CLI 2.0 utilise json comme option de sortie par défaut, mais vous pouvez mettre en forme la sortie des commandes de différentes façons.  Utilisez le paramètre `--output` (ou `--out` ou `-o`) pour formater la sortie de la commande avec l’un des types de sortie indiqués dans le tableau suivant :

--output | DESCRIPTION
---------|-------------------------------
`json`   | Chaîne JSON. Il s’agit du paramètre par défaut.
`jsonc`  | JSON coloré.
`table`  | Table ASCII avec des clés en tant qu’en-têtes de colonne.
`tsv`    | Valeurs séparées par des tabulations, sans clés

## <a name="json-output-format"></a>Format de sortie JSON

L’exemple suivant affiche la liste des machines virtuelles dans vos abonnements au format json par défaut.

```azurecli
az vm list --output json
```

Certains champs de la sortie suivante ont été omis par souci de concision et des informations d’identification ont été remplacées.

```json
[
  {
    "availabilitySet": null,
    "diagnosticsProfile": null,
    "hardwareProfile": {
      "vmSize": "Standard_DS1"
    },
    "id": "/subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/DemoVM010",
    "instanceView": null,
    "licenseType": null,
    "location": "westus",
    "name": "DemoVM010",
    "networkProfile": {
      "networkInterfaces": [
        {
          "id": "/subscriptions/.../resourceGroups/demorg1/providers/Microsoft.Network/networkInterfaces/DemoVM010VMNic",
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

## <a name="table-output-format"></a>Format de sortie de la table

Le format de sortie `table` fournit une sortie brute formatée en tant que lignes et colonnes de données assemblées, ce qui facilite la lecture et l’analyse. Les objets imbriqués ne sont pas inclus dans la sortie de la table, mais peuvent toujours être filtrés dans le cadre d’une requête. Certains champs sont également omis des données de table. Ce format est donc conseillé lorsque vous souhaitez un aperçu des données rapide et consultable à l’échelle humaine.

```azurecli
az vm list --out table
```

```output
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
az vm list --query "[].{resource:resourceGroup, name:name}" -o table
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

> [!NOTE]
> Certaines clés sont filtrées et non pas imprimées dans l’affichage de table. Il s’agit de `id`, `type`, et `etag`. Si vous avez besoin de les voir dans votre sortie, vous pouvez utiliser la fonction JMESPath de régénération des clés pour modifier le nom de clé et éviter le filtrage.
>
> ```azurecli
> az vm list --query "[].{objectID:id}" -o table
> ```

Pour plus d’informations sur l’utilisation des requêtes pour filtrer les données, consultez [Utiliser des requêtes JMESPath avec Azure CLI 2.0](/cli/azure/query-azure-cli).

## <a name="tsv-output-format"></a>Format de sortie TSV

Le format de sortie `tsv` retourne des valeurs séparées par des tabulations et des sauts de ligne sans mise en forme, clés ou autres symboles supplémentaires. Avec ce format, il est facile de consommer la sortie dans d’autres commandes et outils qui ont besoin de traiter le texte dans une forme donnée. Comme pour le format `table`, l’option de sortie `tsv` n’imprime pas les objets imbriqués.

L’exécution de l’exemple précédent avec l’option `tsv` retourne le résultat séparé par des tabulations.

```azurecli
az vm list --out tsv
```

```output
None    None        /subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/DemoVM010 None    None    westus  DemoVM010           None    Succeeded   DEMORG1 None            Microsoft.Compute/virtualMachines   cbd56d9b-9340-44bc-a722-25f15b578444
None    None        /subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm212 None    None    westus  demovm212           None    Succeeded   DEMORG1 None            Microsoft.Compute/virtualMachines   4bdac85d-c2f7-410f-9907-ca7921d930b4
None    None        /subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm213 None    None    westus  demovm213           None    Succeeded   DEMORG1 None            Microsoft.Compute/virtualMachines   2131c664-221a-4b7f-9653-f6d542fbfa34
None    None        /subscriptions/.../resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo001VM None    None    westus  KBDemo001VM         None    Succeeded   RGDEMO001   None            Microsoft.Compute/virtualMachines   14e74761-c17e-4530-a7be-9e4ff06ea74b
None    None        /subscriptions/.../resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo02None    None    westus  KBDemo020           None    Succeeded   RGDEMO001   None            Microsoft.Compute/virtualMachines    36baa9-9b80-48a8-b4a9-854c7a858ece
```

L’exemple suivant montre comment la sortie `tsv` peut être redirigée vers d’autres commandes sur les systèmes UNIX pour extraire des données plus spécifiques. La commande `grep` sélectionne les éléments contenant le texte « RGD », puis la commande `cut` sélectionne le huitième champ (séparé par des tabulations) pour afficher le nom de la machine virtuelle dans la sortie.

```bash
az vm list --out tsv | grep RGD | cut -f8
```

```output
KBDemo001VM
KBDemo020
```

Dans le cadre du traitement des champs séparés par des tabulations, les valeurs sont dans le même ordre que dans l’objet JSON imprimé. Cette commande est garantie comme étant cohérente entre les exécutions de la commande.

## <a name="set-the-default-output-format"></a>Définir le format de sortie par défaut

Utilisez la commande interactive `az configure` pour configurer votre environnement et établir des paramètres par défaut pour les formats de sortie. Le format de sortie par défaut est `json`. 

```azurecli
az configure
```

```output
Welcome to the Azure CLI! This command will guide you through logging in and setting some default values.

Your settings can be found at /home/defaultuser/.azure/config
Your current configuration is as follows:

  ...

Do you wish to change your settings? (y/N): y

What default output format would you like?
 [1] json - JSON formatted output that most closely matches API responses
 [2] jsonc - Colored JSON formatted output that most closely matches API responses
 [3] table - Human-readable output format
 [4] tsv - Tab- and Newline-delimited, great for GREP, AWK, etc.
Please enter a choice [1]:
```

Pour en savoir plus sur la configuration de votre environnement, consultez [Configuration Azure CLI 2.0](/cli/azure/azure-cli-configuration).
