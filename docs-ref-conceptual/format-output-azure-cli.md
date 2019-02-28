---
title: Formats de sortie pour Azure CLI
description: Apprenez à mettre la sortie des commandes Azure CLI aux formats de listes, de tableaux ou de json.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/07/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 0b90e6375beccafee88b2a1d1b7896275dc14407
ms.sourcegitcommit: 1987a39809f9865034b27130e56f30b2bd1eb72c
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/19/2019
ms.locfileid: "56421947"
---
# <a name="output-formats-for-azure-cli-commands"></a><span data-ttu-id="e60af-103">Formats de sortie pour les commandes Azure CLI</span><span class="sxs-lookup"><span data-stu-id="e60af-103">Output formats for Azure CLI commands</span></span>

<span data-ttu-id="e60af-104">Azure CLI utilise JSON comme format de sortie par défaut, mais il propose d’autres formats.</span><span class="sxs-lookup"><span data-stu-id="e60af-104">The Azure CLI uses JSON as its default output format, but offers other formats.</span></span>  <span data-ttu-id="e60af-105">Utilisez le paramètre `--output` (`--out` ou `-o`) pour formater la sortie de l’interface CLI.</span><span class="sxs-lookup"><span data-stu-id="e60af-105">Use the `--output` (`--out` or `-o`) parameter to format CLI output.</span></span> <span data-ttu-id="e60af-106">Les valeurs d’argument et les types de sortie sont :</span><span class="sxs-lookup"><span data-stu-id="e60af-106">The argument values and types of output are:</span></span>

<span data-ttu-id="e60af-107">--output</span><span class="sxs-lookup"><span data-stu-id="e60af-107">--output</span></span> | <span data-ttu-id="e60af-108">Description</span><span class="sxs-lookup"><span data-stu-id="e60af-108">Description</span></span>
---------|-------------------------------
`json`   | <span data-ttu-id="e60af-109">Chaîne JSON.</span><span class="sxs-lookup"><span data-stu-id="e60af-109">JSON string.</span></span> <span data-ttu-id="e60af-110">Il s’agit du paramètre par défaut.</span><span class="sxs-lookup"><span data-stu-id="e60af-110">This setting is the default.</span></span>
`jsonc`  | <span data-ttu-id="e60af-111">JSON coloré.</span><span class="sxs-lookup"><span data-stu-id="e60af-111">Colorized JSON.</span></span>
`yaml`   | <span data-ttu-id="e60af-112">YAML, une alternative à JSON pouvant être lue par la machine.</span><span class="sxs-lookup"><span data-stu-id="e60af-112">YAML, a machine-readable alternative to JSON.</span></span>
`table`  | <span data-ttu-id="e60af-113">Table ASCII avec des clés en tant qu’en-têtes de colonne.</span><span class="sxs-lookup"><span data-stu-id="e60af-113">ASCII table with keys as column headings.</span></span>
`tsv`    | <span data-ttu-id="e60af-114">Valeurs séparées par des tabulations, sans clés</span><span class="sxs-lookup"><span data-stu-id="e60af-114">Tab-separated values, with no keys</span></span>

## <a name="json-output-format"></a><span data-ttu-id="e60af-115">Format de sortie JSON</span><span class="sxs-lookup"><span data-stu-id="e60af-115">JSON output format</span></span>

<span data-ttu-id="e60af-116">L’exemple suivant affiche la liste des machines virtuelles de vos abonnements au format JSON par défaut.</span><span class="sxs-lookup"><span data-stu-id="e60af-116">The following example displays the list of virtual machines in your subscriptions in the default JSON format.</span></span>

```azurecli-interactive
az vm list --output json
```

<span data-ttu-id="e60af-117">Certains champs de la sortie suivante ont été omis par souci de concision et des informations d’identification ont été remplacées.</span><span class="sxs-lookup"><span data-stu-id="e60af-117">The following output has some fields omitted for brevity, and identifying information replaced.</span></span>

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

## <a name="yaml-output-format"></a><span data-ttu-id="e60af-118">Format de sortie YAML</span><span class="sxs-lookup"><span data-stu-id="e60af-118">YAML output format</span></span>

<span data-ttu-id="e60af-119">Le format `yaml` affiche la sortie en tant que [YAML](http://yaml.org/), un format de sérialisation de données en texte brut.</span><span class="sxs-lookup"><span data-stu-id="e60af-119">The `yaml` format prints output as [YAML](http://yaml.org/), a plain-text data serialization format.</span></span> <span data-ttu-id="e60af-120">YAML est souvent plus simple à lire que JSON et se mappe facilement vers ce format.</span><span class="sxs-lookup"><span data-stu-id="e60af-120">YAML tends to be easier to read than JSON, and easily maps to that format.</span></span> <span data-ttu-id="e60af-121">Certaines applications et commandes CLI utilisent YAML en tant qu’entrée de configuration, plutôt que JSON.</span><span class="sxs-lookup"><span data-stu-id="e60af-121">Some applications and CLI commands take YAML as configuration input, instead of JSON.</span></span>

```azurecli-interactive
az vm list --out yaml
```

<span data-ttu-id="e60af-122">Certains champs de la sortie suivante ont été omis par souci de concision et des informations d’identification ont été remplacées.</span><span class="sxs-lookup"><span data-stu-id="e60af-122">The following output has some fields omitted for brevity, and identifying information replaced.</span></span>

```yaml
- availabilitySet: null
  diagnosticsProfile: null
  hardwareProfile:
    vmSize: Standard_DS1_v2
  id: /subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/DemoVM010
  identity: null
  instanceView: null
  licenseType: null
  location: westus
  name: ExampleVM1
  networkProfile:
    networkInterfaces:
    - id: /subscriptions/.../resourceGroups/DemoRG1/providers/Microsoft.Network/networkInterfaces/DemoVM010Nic
      primary: null
      resourceGroup: DemoRG1
  ...
...
```

## <a name="table-output-format"></a><span data-ttu-id="e60af-123">Format de sortie de la table</span><span class="sxs-lookup"><span data-stu-id="e60af-123">Table output format</span></span>

<span data-ttu-id="e60af-124">Le format `table` imprime la sortie sous forme de tableau ASCII, ce qui la rend facile à lire et à analyser.</span><span class="sxs-lookup"><span data-stu-id="e60af-124">The `table` format prints output as an ASCII table, making it easy to read and scan.</span></span> <span data-ttu-id="e60af-125">Les objets imbriqués ne sont pas inclus dans le tableau de sortie, mais peuvent toujours être filtrés dans le cadre d’une requête.</span><span class="sxs-lookup"><span data-stu-id="e60af-125">Nested objects aren't included in table output, but can still be filtered as part of a query.</span></span> <span data-ttu-id="e60af-126">Certains champs ne sont pas compris dans le tableau. Ainsi, ce format est le plus approprié si vous souhaitez obtenir un aperçu des données rapide et consultable pour un être humain.</span><span class="sxs-lookup"><span data-stu-id="e60af-126">Some fields aren't included in the table, so this format is best when you want a quick, human-searchable overview of data.</span></span>

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

<span data-ttu-id="e60af-127">Vous pouvez utiliser le paramètre `--query` pour personnaliser les propriétés et les colonnes à afficher dans la liste générée.</span><span class="sxs-lookup"><span data-stu-id="e60af-127">You can use the `--query` parameter to customize the properties and columns you want to show in the list output.</span></span> <span data-ttu-id="e60af-128">L’exemple suivant montre comment sélectionner uniquement le nom de la machine virtuelle et le nom du groupe de ressources dans la commande `list`.</span><span class="sxs-lookup"><span data-stu-id="e60af-128">The following example shows how to select just the VM Name and the Resource Group Name in the `list` command.</span></span>

```azurecli-interactive
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
> <span data-ttu-id="e60af-129">Certaines clés ne sont pas imprimées dans l’affichage du tableau par défaut.</span><span class="sxs-lookup"><span data-stu-id="e60af-129">Some keys are not printed in the table view by default.</span></span> <span data-ttu-id="e60af-130">Il s’agit de `id`, `type`, et `etag`.</span><span class="sxs-lookup"><span data-stu-id="e60af-130">These are `id`, `type`, and `etag`.</span></span> <span data-ttu-id="e60af-131">Si vous avez besoin de les voir dans votre sortie, vous pouvez utiliser la fonction JMESPath de régénération des clés pour modifier le nom de clé et éviter le filtrage.</span><span class="sxs-lookup"><span data-stu-id="e60af-131">If you need to see these in your output, you can use the JMESPath re-keying feature to change the key name and avoid filtering.</span></span>
>
> ```azurecli-interactive
> az vm list --query "[].{objectID:id}" -o table
> ```

<span data-ttu-id="e60af-132">Pour plus d’informations concernant l’utilisation des requêtes pour filtrer les données, consultez [Utiliser des requêtes JMESPath avec Azure CLI](/cli/azure/query-azure-cli).</span><span class="sxs-lookup"><span data-stu-id="e60af-132">For more about using queries to filter data, see [Use JMESPath queries with Azure CLI](/cli/azure/query-azure-cli).</span></span>

## <a name="tsv-output-format"></a><span data-ttu-id="e60af-133">Format de sortie TSV</span><span class="sxs-lookup"><span data-stu-id="e60af-133">TSV output format</span></span>

<span data-ttu-id="e60af-134">Le format de sortie `tsv` retourne des valeurs séparées par des tabulations et des sauts de ligne sans mise en forme, clés ou autres symboles supplémentaires.</span><span class="sxs-lookup"><span data-stu-id="e60af-134">The `tsv` output format returns tab- and newline-separated values without additional formatting, keys, or other symbols.</span></span> <span data-ttu-id="e60af-135">Avec ce format, il est facile de consommer la sortie dans d’autres commandes et outils qui ont besoin de traiter le texte dans une forme donnée.</span><span class="sxs-lookup"><span data-stu-id="e60af-135">This format makes it easy to consume the output into other commands and tools that need to process the text in some form.</span></span> <span data-ttu-id="e60af-136">Comme pour le format `table`, le format `tsv` n’imprime pas les objets imbriqués.</span><span class="sxs-lookup"><span data-stu-id="e60af-136">Like the `table` format, `tsv` doesn't print nested objects.</span></span>

<span data-ttu-id="e60af-137">L’exécution de l’exemple précédent avec l’option `tsv` retourne le résultat séparé par des tabulations.</span><span class="sxs-lookup"><span data-stu-id="e60af-137">Using the preceding example with the `tsv` option outputs the tab-separated result.</span></span>

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

<span data-ttu-id="e60af-138">L’exemple suivant montre comment la sortie `tsv` peut être transmise à d’autres commandes dans Bash.</span><span class="sxs-lookup"><span data-stu-id="e60af-138">The next example shows how `tsv` output can be piped to other commands in bash.</span></span> <span data-ttu-id="e60af-139">La commande `grep` sélectionne les éléments contenant le texte « RGD », puis la commande `cut` sélectionne le huitième champ pour afficher le nom de la machine virtuelle dans la sortie.</span><span class="sxs-lookup"><span data-stu-id="e60af-139">`grep` selects items that have text "RGD" in them, then the `cut` command selects the eighth field to show the name of the VM in output.</span></span>

```bash
az vm list --out tsv | grep RGD | cut -f8
```

```output
KBDemo001VM
KBDemo020
```

<span data-ttu-id="e60af-140">Dans le cadre du traitement des champs séparés par des tabulations, les valeurs sont dans le même ordre que dans l’objet JSON imprimé.</span><span class="sxs-lookup"><span data-stu-id="e60af-140">For the purposes of processing tab-separated fields, the values are in the same order that they appear in the printed JSON object.</span></span> <span data-ttu-id="e60af-141">Cette commande est garantie comme étant cohérente entre les exécutions de la commande.</span><span class="sxs-lookup"><span data-stu-id="e60af-141">This order is guaranteed to be consistent between runs of the command.</span></span>

## <a name="set-the-default-output-format"></a><span data-ttu-id="e60af-142">Définir le format de sortie par défaut</span><span class="sxs-lookup"><span data-stu-id="e60af-142">Set the default output format</span></span>

<span data-ttu-id="e60af-143">Utilisez la commande interactive `az configure` pour configurer votre environnement et établir des paramètres par défaut pour les formats de sortie.</span><span class="sxs-lookup"><span data-stu-id="e60af-143">Use the interactive `az configure` command to set up your environment and establish default settings for output formats.</span></span> <span data-ttu-id="e60af-144">Le format de sortie par défaut est `json`.</span><span class="sxs-lookup"><span data-stu-id="e60af-144">The default output format is `json`.</span></span>

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
 [1] json - JSON formatted output that most closely matches API responses.
 [2] jsonc - Colored JSON formatted output that most closely matches API responses.
 [3] table - Human-readable output format.
 [4] tsv - Tab- and Newline-delimited. Great for GREP, AWK, etc.
 [5] yaml - YAML formatted output. An alternative to JSON. Great for configuration files.
 [6] none - No output, except for errors and warnings.
Please enter a choice [1]:
```

<span data-ttu-id="e60af-145">Pour en savoir plus sur la configuration de votre environnement, consultez [Configuration d’Azure CLI](/cli/azure/azure-cli-configuration).</span><span class="sxs-lookup"><span data-stu-id="e60af-145">To learn more about configuring your environment, see [Azure CLI configuration](/cli/azure/azure-cli-configuration).</span></span>
