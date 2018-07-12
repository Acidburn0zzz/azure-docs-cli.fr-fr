---
title: Formats de sortie pour Azure CLI 2.0
description: Apprenez à mettre la sortie des commandes Azure CLI 2.0 au format liste, table ou json.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/16/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: b402ce89cbf51adb3d521a604e992dd1fb5a42fa
ms.sourcegitcommit: 64f2c628e83d687d0e172c01f13d71c8c39a8040
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/11/2018
ms.locfileid: "38967603"
---
# <a name="output-formats-for-azure-cli-20-commands"></a><span data-ttu-id="03318-103">Formats de sortie pour les commandes Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="03318-103">Output formats for Azure CLI 2.0 commands</span></span>

<span data-ttu-id="03318-104">Azure CLI 2.0 utilise json comme option de sortie par défaut, mais vous pouvez mettre en forme la sortie des commandes de différentes façons.</span><span class="sxs-lookup"><span data-stu-id="03318-104">Azure CLI 2.0 uses json as its default output option, but offers various ways for you to format the output of any command.</span></span>  <span data-ttu-id="03318-105">Utilisez le paramètre `--output` (ou `--out` ou `-o`) pour formater la sortie de la commande avec l’un des types de sortie indiqués dans le tableau suivant :</span><span class="sxs-lookup"><span data-stu-id="03318-105">Use the `--output` (or `--out` or `-o`) parameter to format the output of the command into one of the output types noted in the following table:</span></span>

<span data-ttu-id="03318-106">--output</span><span class="sxs-lookup"><span data-stu-id="03318-106">--output</span></span> | <span data-ttu-id="03318-107">Description</span><span class="sxs-lookup"><span data-stu-id="03318-107">Description</span></span>
---------|-------------------------------
`json`   | <span data-ttu-id="03318-108">Chaîne JSON.</span><span class="sxs-lookup"><span data-stu-id="03318-108">JSON string.</span></span> <span data-ttu-id="03318-109">Il s’agit du paramètre par défaut.</span><span class="sxs-lookup"><span data-stu-id="03318-109">This setting is the default.</span></span>
`jsonc`  | <span data-ttu-id="03318-110">JSON coloré.</span><span class="sxs-lookup"><span data-stu-id="03318-110">Colorized JSON.</span></span>
`table`  | <span data-ttu-id="03318-111">Table ASCII avec des clés en tant qu’en-têtes de colonne.</span><span class="sxs-lookup"><span data-stu-id="03318-111">ASCII table with keys as column headings.</span></span>
`tsv`    | <span data-ttu-id="03318-112">Valeurs séparées par des tabulations, sans clés</span><span class="sxs-lookup"><span data-stu-id="03318-112">Tab-separated values, with no keys</span></span>

## <a name="json-output-format"></a><span data-ttu-id="03318-113">Format de sortie JSON</span><span class="sxs-lookup"><span data-stu-id="03318-113">JSON output format</span></span>

<span data-ttu-id="03318-114">L’exemple suivant affiche la liste des machines virtuelles dans vos abonnements au format json par défaut.</span><span class="sxs-lookup"><span data-stu-id="03318-114">The following example displays the list of virtual machines in your subscriptions in the default json format.</span></span>

```azurecli-interactive
az vm list --output json
```

<span data-ttu-id="03318-115">Certains champs de la sortie suivante ont été omis par souci de concision et des informations d’identification ont été remplacées.</span><span class="sxs-lookup"><span data-stu-id="03318-115">The following output has some fields omitted for brevity, and identifying information replaced.</span></span>

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

## <a name="table-output-format"></a><span data-ttu-id="03318-116">Format de sortie de la table</span><span class="sxs-lookup"><span data-stu-id="03318-116">Table output format</span></span>

<span data-ttu-id="03318-117">Le format de sortie `table` fournit une sortie brute formatée en tant que lignes et colonnes de données assemblées, ce qui facilite la lecture et l’analyse.</span><span class="sxs-lookup"><span data-stu-id="03318-117">The `table` output format provides plain output formatted as rows and columns of collated data, making it easy to read and scan.</span></span> <span data-ttu-id="03318-118">Les objets imbriqués ne sont pas inclus dans la sortie de la table, mais peuvent toujours être filtrés dans le cadre d’une requête.</span><span class="sxs-lookup"><span data-stu-id="03318-118">Nested objects are not included in table output, but can still be filtered as part of a query.</span></span> <span data-ttu-id="03318-119">Certains champs sont également omis des données de table. Ce format est donc conseillé lorsque vous souhaitez un aperçu des données rapide et consultable à l’échelle humaine.</span><span class="sxs-lookup"><span data-stu-id="03318-119">Some fields are also omitted from the table data, so this format is best when you want a quick, human-searchable overview of data.</span></span>

```azurecli-interactive
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

<span data-ttu-id="03318-120">Vous pouvez utiliser le paramètre `--query` pour personnaliser les propriétés et les colonnes à afficher dans la liste générée.</span><span class="sxs-lookup"><span data-stu-id="03318-120">You can use the `--query` parameter to customize the properties and columns you want to show in the list output.</span></span> <span data-ttu-id="03318-121">L’exemple suivant montre comment sélectionner uniquement le nom de la machine virtuelle et le nom du groupe de ressources dans la commande `list`.</span><span class="sxs-lookup"><span data-stu-id="03318-121">The following example shows how to select just the VM Name and the Resource Group Name in the `list` command.</span></span>

```azurecli
az vm list --query "[].{resource:resourceGroup, name:name}" -o table
```

```output
Resource    Name
----------  -----------
DEMORG1     DemoVM010
DEMORG1     demovm212
DEMORG1     demovm213
RGDEMO001   KBDemo001VM
RGDEMO001   KBDemo020
```

> [!NOTE]
> <span data-ttu-id="03318-122">Certaines clés sont filtrées et non pas imprimées dans l’affichage de table.</span><span class="sxs-lookup"><span data-stu-id="03318-122">Certain keys are filtered out and not printed in the table view.</span></span> <span data-ttu-id="03318-123">Il s’agit de `id`, `type`, et `etag`.</span><span class="sxs-lookup"><span data-stu-id="03318-123">These are `id`, `type`, and `etag`.</span></span> <span data-ttu-id="03318-124">Si vous avez besoin de les voir dans votre sortie, vous pouvez utiliser la fonction JMESPath de régénération des clés pour modifier le nom de clé et éviter le filtrage.</span><span class="sxs-lookup"><span data-stu-id="03318-124">If you need to see these in your output, you can use the JMESPath re-keying feature to change the key name and avoid filtering.</span></span>
>
> ```azurecli
> az vm list --query "[].{objectID:id}" -o table
> ```

<span data-ttu-id="03318-125">Pour plus d’informations sur l’utilisation des requêtes pour filtrer les données, consultez [Utiliser des requêtes JMESPath avec Azure CLI 2.0](/cli/azure/query-azure-cli).</span><span class="sxs-lookup"><span data-stu-id="03318-125">For more about using queries to filter data, see [Use JMESPath queries with Azure CLI 2.0](/cli/azure/query-azure-cli).</span></span>

## <a name="tsv-output-format"></a><span data-ttu-id="03318-126">Format de sortie TSV</span><span class="sxs-lookup"><span data-stu-id="03318-126">TSV output format</span></span>

<span data-ttu-id="03318-127">Le format de sortie `tsv` retourne des valeurs séparées par des tabulations et des sauts de ligne sans mise en forme, clés ou autres symboles supplémentaires.</span><span class="sxs-lookup"><span data-stu-id="03318-127">The `tsv` output format returns tab- and newline-separated values without additional formatting, keys, or other symbols.</span></span> <span data-ttu-id="03318-128">Avec ce format, il est facile de consommer la sortie dans d’autres commandes et outils qui ont besoin de traiter le texte dans une forme donnée.</span><span class="sxs-lookup"><span data-stu-id="03318-128">This format makes it easy to consume the output into other commands and tools that need to process the text in some form.</span></span> <span data-ttu-id="03318-129">Comme pour le format `table`, l’option de sortie `tsv` n’imprime pas les objets imbriqués.</span><span class="sxs-lookup"><span data-stu-id="03318-129">Like the `table` format, the `tsv` output option does not print nested objects.</span></span>

<span data-ttu-id="03318-130">L’exécution de l’exemple précédent avec l’option `tsv` retourne le résultat séparé par des tabulations.</span><span class="sxs-lookup"><span data-stu-id="03318-130">Using the preceding example with the `tsv` option outputs the tab-separated result.</span></span>

```azurecli-interactive
az vm list --out tsv
```

```output
None    None        /subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/DemoVM010    None    None    westus    DemoVM010            None    Succeeded    DEMORG1    None            Microsoft.Compute/virtualMachines    cbd56d9b-9340-44bc-a722-25f15b578444
None    None        /subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm212    None    None    westus    demovm212            None    Succeeded    DEMORG1    None            Microsoft.Compute/virtualMachines    4bdac85d-c2f7-410f-9907-ca7921d930b4
None    None        /subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm213    None    None    westus    demovm213            None    Succeeded    DEMORG1    None            Microsoft.Compute/virtualMachines    2131c664-221a-4b7f-9653-f6d542fbfa34
None    None        /subscriptions/.../resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo001VM    None    None    westus    KBDemo001VM            None    Succeeded    RGDEMO001    None            Microsoft.Compute/virtualMachines    14e74761-c17e-4530-a7be-9e4ff06ea74b
None    None        /subscriptions/.../resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo02None    None    westus    KBDemo020            None    Succeeded    RGDEMO001    None            Microsoft.Compute/virtualMachines    36baa9-9b80-48a8-b4a9-854c7a858ece
```

<span data-ttu-id="03318-131">L’exemple suivant montre comment la sortie `tsv` peut être redirigée vers d’autres commandes sur les systèmes UNIX pour extraire des données plus spécifiques.</span><span class="sxs-lookup"><span data-stu-id="03318-131">The next example shows how the `tsv` output can be piped to other commands on UNIX systems to extract more specific data.</span></span> <span data-ttu-id="03318-132">La commande `grep` sélectionne les éléments contenant le texte « RGD », puis la commande `cut` sélectionne le huitième champ (séparé par des tabulations) pour afficher le nom de la machine virtuelle dans la sortie.</span><span class="sxs-lookup"><span data-stu-id="03318-132">The `grep` command selects items that have text "RGD" in them, and then the `cut` command selects the eighth field (separated by tabs) to show the name of the VM in output.</span></span>

```bash
az vm list --out tsv | grep RGD | cut -f8
```

```output
KBDemo001VM
KBDemo020
```

<span data-ttu-id="03318-133">Dans le cadre du traitement des champs séparés par des tabulations, les valeurs sont dans le même ordre que dans l’objet JSON imprimé.</span><span class="sxs-lookup"><span data-stu-id="03318-133">For the purposes of processing tab-separated fields, the values are in the same order that they appear in the printed JSON object.</span></span> <span data-ttu-id="03318-134">Cette commande est garantie comme étant cohérente entre les exécutions de la commande.</span><span class="sxs-lookup"><span data-stu-id="03318-134">This order is guaranteed to be consistent between runs of the command.</span></span>

## <a name="set-the-default-output-format"></a><span data-ttu-id="03318-135">Définir le format de sortie par défaut</span><span class="sxs-lookup"><span data-stu-id="03318-135">Set the default output format</span></span>

<span data-ttu-id="03318-136">Utilisez la commande interactive `az configure` pour configurer votre environnement et établir des paramètres par défaut pour les formats de sortie.</span><span class="sxs-lookup"><span data-stu-id="03318-136">Use the interactive `az configure` command to set up your environment and establish default settings for output formats.</span></span> <span data-ttu-id="03318-137">Le format de sortie par défaut est `json`.</span><span class="sxs-lookup"><span data-stu-id="03318-137">The default output format is `json`.</span></span>

```azurecli-interactive
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

<span data-ttu-id="03318-138">Pour en savoir plus sur la configuration de votre environnement, consultez [Configuration Azure CLI 2.0](/cli/azure/azure-cli-configuration).</span><span class="sxs-lookup"><span data-stu-id="03318-138">To learn more about configuring your environment, see [Azure CLI 2.0 configuration](/cli/azure/azure-cli-configuration).</span></span>