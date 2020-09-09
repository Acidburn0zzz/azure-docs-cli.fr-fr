---
title: Formats de sortie pour Azure CLI
description: Apprenez à mettre la sortie des commandes Azure CLI aux formats de listes, de tableaux ou de json.
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 09/23/2019
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: d4cc869aa7e23f87cf6f13b8aca9f10cbbca82b5
ms.sourcegitcommit: 2da241715d25407ed22c1065c0c793acfd865996
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/09/2020
ms.locfileid: "89563159"
---
# <a name="output-formats-for-azure-cli-commands"></a><span data-ttu-id="bf350-103">Formats de sortie pour les commandes Azure CLI</span><span class="sxs-lookup"><span data-stu-id="bf350-103">Output formats for Azure CLI commands</span></span>

<span data-ttu-id="bf350-104">Azure CLI utilise JSON comme format de sortie par défaut, mais il propose d’autres formats.</span><span class="sxs-lookup"><span data-stu-id="bf350-104">The Azure CLI uses JSON as its default output format, but offers other formats.</span></span>  <span data-ttu-id="bf350-105">Utilisez le paramètre `--output` (`--out` ou `-o`) pour formater la sortie de l’interface CLI.</span><span class="sxs-lookup"><span data-stu-id="bf350-105">Use the `--output` (`--out` or `-o`) parameter to format CLI output.</span></span> <span data-ttu-id="bf350-106">Les valeurs d’argument et les types de sortie sont :</span><span class="sxs-lookup"><span data-stu-id="bf350-106">The argument values and types of output are:</span></span>

<span data-ttu-id="bf350-107">--output</span><span class="sxs-lookup"><span data-stu-id="bf350-107">--output</span></span> | <span data-ttu-id="bf350-108">Description</span><span class="sxs-lookup"><span data-stu-id="bf350-108">Description</span></span>
---------|-------------------------------
`json`   | <span data-ttu-id="bf350-109">Chaîne JSON.</span><span class="sxs-lookup"><span data-stu-id="bf350-109">JSON string.</span></span> <span data-ttu-id="bf350-110">Paramètre par défaut</span><span class="sxs-lookup"><span data-stu-id="bf350-110">This setting is the default</span></span>
`jsonc`  | <span data-ttu-id="bf350-111">JSON coloré</span><span class="sxs-lookup"><span data-stu-id="bf350-111">Colorized JSON</span></span>
`yaml`   | <span data-ttu-id="bf350-112">YAML, alternative à JSON pouvant être lue par la machine</span><span class="sxs-lookup"><span data-stu-id="bf350-112">YAML, a machine-readable alternative to JSON</span></span>
`table`  | <span data-ttu-id="bf350-113">Table ASCII avec des clés en tant qu’en-têtes de colonne</span><span class="sxs-lookup"><span data-stu-id="bf350-113">ASCII table with keys as column headings</span></span>
`tsv`    | <span data-ttu-id="bf350-114">Valeurs séparées par des tabulations, sans clés</span><span class="sxs-lookup"><span data-stu-id="bf350-114">Tab-separated values, with no keys</span></span>
`none`   | <span data-ttu-id="bf350-115">Aucune sortie autre que des erreurs et des avertissements</span><span class="sxs-lookup"><span data-stu-id="bf350-115">No output other than errors and warnings</span></span>

## <a name="json-output-format"></a><span data-ttu-id="bf350-116">Format de sortie JSON</span><span class="sxs-lookup"><span data-stu-id="bf350-116">JSON output format</span></span>

<span data-ttu-id="bf350-117">L’exemple suivant affiche la liste des machines virtuelles de vos abonnements au format JSON par défaut.</span><span class="sxs-lookup"><span data-stu-id="bf350-117">The following example displays the list of virtual machines in your subscriptions in the default JSON format.</span></span>

```azurecli-interactive
az vm list --output json
```

<span data-ttu-id="bf350-118">Certains champs de la sortie suivante ont été omis par souci de concision et des informations d’identification ont été remplacées.</span><span class="sxs-lookup"><span data-stu-id="bf350-118">The following output has some fields omitted for brevity, and identifying information replaced.</span></span>

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

## <a name="yaml-output-format"></a><span data-ttu-id="bf350-119">Format de sortie YAML</span><span class="sxs-lookup"><span data-stu-id="bf350-119">YAML output format</span></span>

<span data-ttu-id="bf350-120">Le format `yaml` affiche la sortie en tant que [YAML](http://yaml.org/), un format de sérialisation de données en texte brut.</span><span class="sxs-lookup"><span data-stu-id="bf350-120">The `yaml` format prints output as [YAML](http://yaml.org/), a plain-text data serialization format.</span></span> <span data-ttu-id="bf350-121">YAML est souvent plus simple à lire que JSON et se mappe facilement vers ce format.</span><span class="sxs-lookup"><span data-stu-id="bf350-121">YAML tends to be easier to read than JSON, and easily maps to that format.</span></span> <span data-ttu-id="bf350-122">Certaines applications et commandes CLI utilisent YAML en tant qu’entrée de configuration, plutôt que JSON.</span><span class="sxs-lookup"><span data-stu-id="bf350-122">Some applications and CLI commands take YAML as configuration input, instead of JSON.</span></span>

```azurecli-interactive
az vm list --out yaml
```

<span data-ttu-id="bf350-123">Certains champs de la sortie suivante ont été omis par souci de concision et des informations d’identification ont été remplacées.</span><span class="sxs-lookup"><span data-stu-id="bf350-123">The following output has some fields omitted for brevity, and identifying information replaced.</span></span>

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

## <a name="table-output-format"></a><span data-ttu-id="bf350-124">Format de sortie de la table</span><span class="sxs-lookup"><span data-stu-id="bf350-124">Table output format</span></span>

<span data-ttu-id="bf350-125">Le format `table` imprime la sortie sous forme de tableau ASCII, ce qui la rend facile à lire et à analyser.</span><span class="sxs-lookup"><span data-stu-id="bf350-125">The `table` format prints output as an ASCII table, making it easy to read and scan.</span></span> <span data-ttu-id="bf350-126">Les objets imbriqués ne sont pas inclus dans le tableau de sortie, mais peuvent toujours être filtrés dans le cadre d’une requête.</span><span class="sxs-lookup"><span data-stu-id="bf350-126">Nested objects aren't included in table output, but can still be filtered as part of a query.</span></span> <span data-ttu-id="bf350-127">Certains champs ne sont pas compris dans le tableau. Ainsi, ce format est le plus approprié si vous souhaitez obtenir un aperçu des données rapide et consultable pour un être humain.</span><span class="sxs-lookup"><span data-stu-id="bf350-127">Some fields aren't included in the table, so this format is best when you want a quick, human-searchable overview of data.</span></span>

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

<span data-ttu-id="bf350-128">Vous pouvez utiliser le paramètre `--query` pour personnaliser les propriétés et les colonnes à afficher dans la liste générée.</span><span class="sxs-lookup"><span data-stu-id="bf350-128">You can use the `--query` parameter to customize the properties and columns you want to show in the list output.</span></span> <span data-ttu-id="bf350-129">L’exemple suivant montre comment sélectionner uniquement le nom de la machine virtuelle et le nom du groupe de ressources dans la commande `list`.</span><span class="sxs-lookup"><span data-stu-id="bf350-129">The following example shows how to select just the VM Name and the Resource Group Name in the `list` command.</span></span>

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
> <span data-ttu-id="bf350-130">Certaines clés ne sont pas imprimées dans l’affichage du tableau par défaut.</span><span class="sxs-lookup"><span data-stu-id="bf350-130">Some keys are not printed in the table view by default.</span></span> <span data-ttu-id="bf350-131">Il s’agit de `id`, `type`, et `etag`.</span><span class="sxs-lookup"><span data-stu-id="bf350-131">These are `id`, `type`, and `etag`.</span></span> <span data-ttu-id="bf350-132">Si vous avez besoin de les voir dans votre sortie, vous pouvez utiliser la fonction JMESPath de régénération des clés pour modifier le nom de clé et éviter le filtrage.</span><span class="sxs-lookup"><span data-stu-id="bf350-132">If you need to see these in your output, you can use the JMESPath re-keying feature to change the key name and avoid filtering.</span></span>
>
> ```azurecli-interactive
> az vm list --query "[].{objectID:id}" -o table
> ```

<span data-ttu-id="bf350-133">Pour plus d’informations concernant l’utilisation des requêtes pour filtrer les données, consultez [Utiliser des requêtes JMESPath avec Azure CLI](/cli/azure/query-azure-cli).</span><span class="sxs-lookup"><span data-stu-id="bf350-133">For more about using queries to filter data, see [Use JMESPath queries with Azure CLI](/cli/azure/query-azure-cli).</span></span>

## <a name="tsv-output-format"></a><span data-ttu-id="bf350-134">Format de sortie TSV</span><span class="sxs-lookup"><span data-stu-id="bf350-134">TSV output format</span></span>

<span data-ttu-id="bf350-135">Le format de sortie `tsv` retourne des valeurs séparées par des tabulations et des sauts de ligne sans mise en forme, clés ou autres symboles supplémentaires.</span><span class="sxs-lookup"><span data-stu-id="bf350-135">The `tsv` output format returns tab- and newline-separated values without additional formatting, keys, or other symbols.</span></span> <span data-ttu-id="bf350-136">Avec ce format, il est facile de consommer la sortie dans d’autres commandes et outils qui ont besoin de traiter le texte dans une forme donnée.</span><span class="sxs-lookup"><span data-stu-id="bf350-136">This format makes it easy to consume the output into other commands and tools that need to process the text in some form.</span></span> <span data-ttu-id="bf350-137">Comme pour le format `table`, le format `tsv` n’imprime pas les objets imbriqués.</span><span class="sxs-lookup"><span data-stu-id="bf350-137">Like the `table` format, `tsv` doesn't print nested objects.</span></span>

<span data-ttu-id="bf350-138">L’exécution de l’exemple précédent avec l’option `tsv` retourne le résultat séparé par des tabulations.</span><span class="sxs-lookup"><span data-stu-id="bf350-138">Using the preceding example with the `tsv` option outputs the tab-separated result.</span></span>

```azurecli-interactive
az vm list --out tsv
```

```output
None    None        /subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/DemoVM010    None    None    westus    DemoVM010            None    Succeeded    DEMORG1    None            Microsoft.Compute/virtualMachines    cbd56d9b-9340-44bc-a722-25f15b578444
None    None        /subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm212    None    None    westus    demovm212            None    Succeeded    DEMORG1    None            Microsoft.Compute/virtualMachines    4bdac85d-c2f7-410f-9907-ca7921d930b4
None    None        /subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm213    None    None    westus    demovm213            None    Succeeded    DEMORG1    None            Microsoft.Compute/virtualMachines    2131c664-221a-4b7f-9653-f6d542fbfa34
None    None        /subscriptions/.../resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo001VM    None    None    westus    KBDemo001VM            None    Succeeded    RGDEMO001    None            Microsoft.Compute/virtualMachines    14e74761-c17e-4530-a7be-9e4ff06ea74b
None    None        /subscriptions/.../resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo020   None    None    westus    KBDemo020            None    Succeeded    RGDEMO001    None            Microsoft.Compute/virtualMachines    36baa9-9b80-48a8-b4a9-854c7a858ece
```

<span data-ttu-id="bf350-139">L’une des restrictions du format de sortie TSV est qu’il n’existe aucune garantie quant à l’ordre de la sortie.</span><span class="sxs-lookup"><span data-stu-id="bf350-139">One restriction of the TSV output format is that there isn't a guarantee on output ordering.</span></span> <span data-ttu-id="bf350-140">L’interface CLI fait de son mieux pour préserver l’ordre en triant les clés dans le code JSON de la réponse par ordre alphabétique, puis en imprimant leurs valeurs dans l’ordre pour la sortie TSV.</span><span class="sxs-lookup"><span data-stu-id="bf350-140">The CLI makes a best effort to preserve ordering by sorting keys in the response JSON alphebetically, and then printing their values in order for TSV output.</span></span> <span data-ttu-id="bf350-141">Il n’est donc pas garanti que l’ordre soit toujours le même puisque le format de la réponse du service Azure peut changer.</span><span class="sxs-lookup"><span data-stu-id="bf350-141">This isn't a guarantee that the order is always identical though, since the Azure service response format may change.</span></span>

<span data-ttu-id="bf350-142">Pour appliquer un ordre cohérent, vous devez utiliser le paramètre `--query` et le format de [liste à sélection multiple](query-azure-cli.md#get-multiple-values).</span><span class="sxs-lookup"><span data-stu-id="bf350-142">In order to enforce consistent ordering, you'll need to use the `--query` parameter and the [multiselect list](query-azure-cli.md#get-multiple-values) format.</span></span> <span data-ttu-id="bf350-143">Quand une commande CLI retourne un dictionnaire JSON unique, utilisez le format général `[key1, key2, ..., keyN]` pour forcer l’ordre des clés.</span><span class="sxs-lookup"><span data-stu-id="bf350-143">When a CLI command returns a single JSON dictionary, use the general format `[key1, key2, ..., keyN]` to force a key order.</span></span>  <span data-ttu-id="bf350-144">Pour les commandes CLI qui retournent un tableau, utilisez le format général `[].[key1, key2, ..., keyN]` pour ordonner les valeurs de colonne.</span><span class="sxs-lookup"><span data-stu-id="bf350-144">For CLI commands which return an array, use the general format `[].[key1, key2, ..., keyN]` to order column values.</span></span>

<span data-ttu-id="bf350-145">Par exemple, pour ordonner les informations affichées ci-dessus par ID, emplacement, groupe de ressources et nom de machine virtuelle :</span><span class="sxs-lookup"><span data-stu-id="bf350-145">For example, to order the information displayed above by ID, location, resource group, and VM name:</span></span>

```azurecli-interactive
az vm list --out tsv --query '[].[id, location, resourceGroup, name]'
```

```output
/subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/DemoVM010    westus    DEMORG1    DemoVM010
/subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm212    westus    DEMORG1    demovm212
/subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm213    westus    DEMORG1    demovm213
/subscriptions/.../resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo001VM     westus  RGDEMO001       KBDemo001VM
/subscriptions/.../resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo020       westus  RGDEMO001       KBDemo020
```

<span data-ttu-id="bf350-146">L’exemple suivant montre comment la sortie `tsv` peut être transmise à d’autres commandes dans Bash.</span><span class="sxs-lookup"><span data-stu-id="bf350-146">The next example shows how `tsv` output can be piped to other commands in bash.</span></span> <span data-ttu-id="bf350-147">La requête permet de filtrer la sortie et de forcer l’ordre, `grep` sélectionne les éléments contenant le texte « RGD », puis la commande `cut` sélectionne le quatrième champ pour afficher le nom de la machine virtuelle dans la sortie.</span><span class="sxs-lookup"><span data-stu-id="bf350-147">The query is used to filter output and force ordering, `grep` selects items that have text "RGD" in them, then the `cut` command selects the fourth field to show the name of the VM in output.</span></span>

```azurecli-interactive
az vm list --out tsv --query '[].[id, location, resourceGroup, name]' | grep RGD | cut -f4
```

```output
KBDemo001VM
KBDemo020
```

## <a name="set-the-default-output-format"></a><span data-ttu-id="bf350-148">Définir le format de sortie par défaut</span><span class="sxs-lookup"><span data-stu-id="bf350-148">Set the default output format</span></span>

<span data-ttu-id="bf350-149">Utilisez la commande interactive `az configure` pour configurer votre environnement et établir des paramètres par défaut pour les formats de sortie.</span><span class="sxs-lookup"><span data-stu-id="bf350-149">Use the interactive `az configure` command to set up your environment and establish default settings for output formats.</span></span> <span data-ttu-id="bf350-150">Le format de sortie par défaut est `json`.</span><span class="sxs-lookup"><span data-stu-id="bf350-150">The default output format is `json`.</span></span>

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

<span data-ttu-id="bf350-151">Pour en savoir plus sur la configuration de votre environnement, consultez [Configuration d’Azure CLI](/cli/azure/azure-cli-configuration).</span><span class="sxs-lookup"><span data-stu-id="bf350-151">To learn more about configuring your environment, see [Azure CLI configuration](/cli/azure/azure-cli-configuration).</span></span>
