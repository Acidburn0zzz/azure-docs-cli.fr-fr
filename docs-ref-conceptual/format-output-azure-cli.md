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
ms.openlocfilehash: a5d629675b468421e3abee41b9c8bffd7e96e5b0
ms.sourcegitcommit: b93a19222e116d5880bbe64c03507c64e190331e
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/15/2018
---
# <a name="output-formats-for-azure-cli-20-commands"></a><span data-ttu-id="649ed-103">Formats de sortie pour les commandes Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="649ed-103">Output formats for Azure CLI 2.0 commands</span></span>

<span data-ttu-id="649ed-104">Azure CLI 2.0 utilise json comme option de sortie par défaut, mais vous pouvez mettre en forme la sortie des commandes de différentes façons.</span><span class="sxs-lookup"><span data-stu-id="649ed-104">Azure CLI 2.0 uses json as its default output option, but offers various ways for you to format the output of any command.</span></span>  <span data-ttu-id="649ed-105">Utilisez le paramètre `--output` (ou `--out` ou `-o`) pour mettre en forme la sortie de la commande avec l’un des types de sortie indiqués dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="649ed-105">Use the `--output` (or `--out` or `-o`) parameter to format the output of the command into one of the output types noted in the following table.</span></span>

<span data-ttu-id="649ed-106">--output</span><span class="sxs-lookup"><span data-stu-id="649ed-106">--output</span></span> | <span data-ttu-id="649ed-107">DESCRIPTION</span><span class="sxs-lookup"><span data-stu-id="649ed-107">Description</span></span>
---------|-------------------------------
`json`   | <span data-ttu-id="649ed-108">Chaîne JSON.</span><span class="sxs-lookup"><span data-stu-id="649ed-108">json string.</span></span> <span data-ttu-id="649ed-109">`json` est la valeur par défaut.</span><span class="sxs-lookup"><span data-stu-id="649ed-109">`json` is the default.</span></span>
`jsonc`  | <span data-ttu-id="649ed-110">Chaîne json colorée.</span><span class="sxs-lookup"><span data-stu-id="649ed-110">colorized json string.</span></span>
`table`  | <span data-ttu-id="649ed-111">Table avec en-têtes de colonnes.</span><span class="sxs-lookup"><span data-stu-id="649ed-111">table with column headings.</span></span>
`tsv`    | <span data-ttu-id="649ed-112">Valeurs séparées par des tabulations.</span><span class="sxs-lookup"><span data-stu-id="649ed-112">tab-separated values.</span></span>

[!INCLUDE [cloud-shell-try-it.md](includes/cloud-shell-try-it.md)]

## <a name="using-the-json-option"></a><span data-ttu-id="649ed-113">Utilisation de l’option json</span><span class="sxs-lookup"><span data-stu-id="649ed-113">Using the json option</span></span>

<span data-ttu-id="649ed-114">L’exemple suivant affiche la liste des machines virtuelles dans vos abonnements au format json par défaut.</span><span class="sxs-lookup"><span data-stu-id="649ed-114">The following example displays the list of virtual machines in your subscriptions in the default json format.</span></span>

```azurecli-interactive
az vm list --output json
```

<span data-ttu-id="649ed-115">Les résultats sont affichés au format suivant (affiche uniquement des résultats partiels, par souci de clarté).</span><span class="sxs-lookup"><span data-stu-id="649ed-115">The results are in this form (only showing partial output for sake of brevity).</span></span>

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

## <a name="using-the-table-option"></a><span data-ttu-id="649ed-116">Utilisation de l’option table</span><span class="sxs-lookup"><span data-stu-id="649ed-116">Using the table option</span></span>

<span data-ttu-id="649ed-117">L’option table fournit une sortie facile à lire, mais notez que les objets imbriqués ne sont pas inclus dans la sortie avec la commande simple `--output table`, contrairement à l’exemple .json précédent.</span><span class="sxs-lookup"><span data-stu-id="649ed-117">The table option provides an easy to read set of output, but note that nested objects are not included in the output with the simple `--output table`, unlike the preceding .json example.</span></span>  <span data-ttu-id="649ed-118">L’utilisation du même exemple avec le format de sortie « table » fournit une liste organisée des valeurs de propriété les plus courantes.</span><span class="sxs-lookup"><span data-stu-id="649ed-118">Using the same example with 'table' output format provides a curated list of most common property values.</span></span>

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

<span data-ttu-id="649ed-119">Vous pouvez utiliser le paramètre `--query` pour personnaliser les propriétés et les colonnes à afficher dans la liste générée.</span><span class="sxs-lookup"><span data-stu-id="649ed-119">You can use the `--query` parameter to customize the properties and columns you want to show in the list output.</span></span> <span data-ttu-id="649ed-120">L’exemple suivant montre comment sélectionner uniquement le nom de la machine virtuelle et le nom du groupe de ressources dans la commande `list`.</span><span class="sxs-lookup"><span data-stu-id="649ed-120">The following example shows how to select just the VM Name and the Resource Group Name in the `list` command.</span></span>

```azurecli-interactive
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

## <a name="using-the-tsv-option"></a><span data-ttu-id="649ed-121">Utilisation de l’option tsv</span><span class="sxs-lookup"><span data-stu-id="649ed-121">Using the tsv option</span></span>

<span data-ttu-id="649ed-122">Le format de sortie « tsv » retourne une sortie texte simple et séparée par des tabulations, sans en-tête ni tiret.</span><span class="sxs-lookup"><span data-stu-id="649ed-122">'tsv' output format returns a simple text-based and tab-separated output with no headings and dashes.</span></span> <span data-ttu-id="649ed-123">Avec ce format, il est facile de consommer la sortie dans d’autres commandes et outils qui ont besoin de traiter le texte dans une forme donnée.</span><span class="sxs-lookup"><span data-stu-id="649ed-123">This format makes it easy to consume the output into other commands and tools that need to process the text in some form.</span></span> <span data-ttu-id="649ed-124">L’exécution de l’exemple précédent avec l’option `tsv` retourne le résultat séparé par des tabulations.</span><span class="sxs-lookup"><span data-stu-id="649ed-124">Using the preceding example with the `tsv` option outputs the tab-separated result.</span></span>

```azurecli-interactive
az vm list --out tsv
```

```
None    None        /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/DemoVM010    None    None    westus  DemoVM010           None    Succeeded   DEMORG1 None            Microsoft.Compute/virtualMachines   cbd56d9b-9340-44bc-a722-25f15b578444
None    None        /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm212    None    None    westus  demovm212           None    Succeeded   DEMORG1 None            Microsoft.Compute/virtualMachines   4bdac85d-c2f7-410f-9907-ca7921d930b4
None    None        /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm213    None    None    westus  demovm213           None    Succeeded   DEMORG1 None            Microsoft.Compute/virtualMachines   2131c664-221a-4b7f-9653-f6d542fbfa34
None    None        /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo001VM    None    None    westus  KBDemo001VM         None    Succeeded   RGDEMO001   None            Microsoft.Compute/virtualMachines   14e74761-c17e-4530-a7be-9e4ff06ea74b
None    None        /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo02None   None    westus  KBDemo020           None    Succeeded   RGDEMO001   None            Microsoft.Compute/virtualMachinesed36baa9-9b80-48a8-b4a9-854c7a858ece
```

<span data-ttu-id="649ed-125">L’exemple suivant montre comment la sortie `tsv` peut être dirigée vers des commandes telles que `grep` et `cut` pour analyser plus en détail des valeurs spécifiques de la sortie `list`.</span><span class="sxs-lookup"><span data-stu-id="649ed-125">The next example shows how the `tsv` output can be piped to commands like `grep` and `cut` to further parse specific values out of the `list` output.</span></span> <span data-ttu-id="649ed-126">La commande `grep` sélectionne uniquement les éléments contenant le texte « RGD », puis la commande `cut` sélectionne uniquement la valeur du huitième champ (séparé par des tabulations) pour l’afficher dans la sortie.</span><span class="sxs-lookup"><span data-stu-id="649ed-126">The `grep` command selects only items that have text "RGD" in them and then the `cut` command selects only the eighth field (separated by tabs) value to show in the output.</span></span>

```azurecli
az vm list --out tsv | grep RGD | cut -f8
```

```
KBDemo001VM
KBDemo020
```

## <a name="setting-the-default-output-format"></a><span data-ttu-id="649ed-127">Définition du format de sortie par défaut</span><span class="sxs-lookup"><span data-stu-id="649ed-127">Setting the default output format</span></span>

<span data-ttu-id="649ed-128">Vous pouvez utiliser la commande `az configure` pour configurer votre environnement ou établir des préférences telles que les paramètres par défaut pour les formats de sortie.</span><span class="sxs-lookup"><span data-stu-id="649ed-128">You can use the `az configure` command to set up your environment or establish preferences such as default settings for output formats.</span></span> <span data-ttu-id="649ed-129">Pour une utilisation courante, le format de sortie par défaut le plus simple est le format « table » : sélectionnez **3** quand vous êtes invité à choisir le format de sortie.</span><span class="sxs-lookup"><span data-stu-id="649ed-129">For common use, the easiest output format default is the "table" format - select **3** when prompted for output format choices.</span></span>

```
What default output format would you like?
 [1] json - JSON formatted output that most closely matches API responses
 [2] jsonc - Colored JSON formatted output that most closely matches API responses
 [3] table - Human-readable output format
 [4] tsv - Tab and Newline delimited, great for GREP, AWK, etc.
Please enter a choice [3]:
```
