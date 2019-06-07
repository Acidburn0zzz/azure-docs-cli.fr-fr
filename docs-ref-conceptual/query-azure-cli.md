---
title: Interroger des résultats de commande avec Azure CLI
description: Apprenez à exécuter des requêtes JMESPath sur la sortie des commandes Azure CLI.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 11/12/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 5e187025e97b1d882bc575fd51970a8250f6210e
ms.sourcegitcommit: bf69c95abf3ed3d589b202c7ff04d8782e2a81ac
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/21/2019
ms.locfileid: "65993047"
---
# <a name="query-azure-cli-command-output"></a><span data-ttu-id="2d6a2-103">Interroger la sortie de commande Azure CLI</span><span class="sxs-lookup"><span data-stu-id="2d6a2-103">Query Azure CLI command output</span></span>

<span data-ttu-id="2d6a2-104">Azure CLI utilise l’argument `--query` pour exécuter une [requête JMESPath](http://jmespath.org) sur les résultats des commandes.</span><span class="sxs-lookup"><span data-stu-id="2d6a2-104">The Azure CLI uses the `--query` argument to execute a [JMESPath query](http://jmespath.org) on the results of commands.</span></span> <span data-ttu-id="2d6a2-105">JMESPath est un langage de requête pour JSON, qui vous permet de sélectionner et de modifier des données depuis une sortie CLI.</span><span class="sxs-lookup"><span data-stu-id="2d6a2-105">JMESPath is a query language for JSON, giving you the ability to select and modify data from CLI output.</span></span> <span data-ttu-id="2d6a2-106">Les requêtes sont exécutées sur la sortie JSON, avant toute mise en forme de l’affichage.</span><span class="sxs-lookup"><span data-stu-id="2d6a2-106">Queries are executed on the JSON output before any display formatting.</span></span>

<span data-ttu-id="2d6a2-107">L’argument `--query` est pris en charge par toutes les commandes dans Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="2d6a2-107">The `--query` argument is supported by all commands in the Azure CLI.</span></span> <span data-ttu-id="2d6a2-108">Cet article explique comment utiliser les fonctionnalités de JMESPath avec une série d’exemples courts et simples.</span><span class="sxs-lookup"><span data-stu-id="2d6a2-108">This article covers how to use the features of JMESPath with a series of small, simple examples.</span></span>

## <a name="dictionary-and-list-cli-results"></a><span data-ttu-id="2d6a2-109">Résultats CLI de liste et de dictionnaire</span><span class="sxs-lookup"><span data-stu-id="2d6a2-109">Dictionary and list CLI results</span></span>

<span data-ttu-id="2d6a2-110">Même quand vous utilisez un format de sortie autre que JSON, les résultats de la commande CLI sont tout d’abord traités comme du code JSON pour les requêtes.</span><span class="sxs-lookup"><span data-stu-id="2d6a2-110">Even when using an output format other than JSON, CLI command results are first treated as JSON for queries.</span></span> <span data-ttu-id="2d6a2-111">Les résultats CLI se présentent sous la forme d’un dictionnaire ou d’un tableau JSON.</span><span class="sxs-lookup"><span data-stu-id="2d6a2-111">CLI results are either a JSON array or dictionary.</span></span> <span data-ttu-id="2d6a2-112">Les tableaux sont des séquences d’objets qui peuvent être indexés, et les dictionnaires sont des objets non ordonnés accessibles avec des clés.</span><span class="sxs-lookup"><span data-stu-id="2d6a2-112">Arrays are sequences of objects that can be indexed, and dictionaries are unordered objects accessed with keys.</span></span> <span data-ttu-id="2d6a2-113">Les commandes qui _peuvent_ renvoyer plus d’un objet renvoient un tableau, et les commandes qui renvoient _toujours_ et _uniquement_ un seul objet renvoient un dictionnaire.</span><span class="sxs-lookup"><span data-stu-id="2d6a2-113">Commands that _could_ return more than one object return an array, and commands that _always_ return _only_ a single object return a dictionary.</span></span>

## <a name="get-properties-in-a-dictionary"></a><span data-ttu-id="2d6a2-114">Récupérer des propriétés dans un dictionnaire</span><span class="sxs-lookup"><span data-stu-id="2d6a2-114">Get properties in a dictionary</span></span>

<span data-ttu-id="2d6a2-115">En utilisant des résultats de dictionnaire, vous pouvez accéder à des propriétés de niveau supérieur simplement avec la clé.</span><span class="sxs-lookup"><span data-stu-id="2d6a2-115">Working with dictionary results, you can access properties from the top level with just the key.</span></span> <span data-ttu-id="2d6a2-116">Le caractère `.` (__sous-expression__) est utilisé pour accéder aux propriétés des dictionnaires imbriqués.</span><span class="sxs-lookup"><span data-stu-id="2d6a2-116">The `.` (__subexpression__) character is used to access properties of nested dictionaries.</span></span> <span data-ttu-id="2d6a2-117">Avant d’introduire des requêtes, examinez la sortie non modifiée de la commande `az vm show` :</span><span class="sxs-lookup"><span data-stu-id="2d6a2-117">Before introducing queries, take a look at the unmodified output of the `az vm show` command:</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM -o json
```

<span data-ttu-id="2d6a2-118">La commande génère un dictionnaire.</span><span class="sxs-lookup"><span data-stu-id="2d6a2-118">The command will output a dictionary.</span></span> <span data-ttu-id="2d6a2-119">Certains contenus ont été omis.</span><span class="sxs-lookup"><span data-stu-id="2d6a2-119">Some content has been omitted.</span></span>

```json
{
  "additionalCapabilities": null,
  "availabilitySet": null,
  "diagnosticsProfile": {
    "bootDiagnostics": {
      "enabled": true,
      "storageUri": "https://xxxxxx.blob.core.windows.net/"
    }
  },
  ...
  "osProfile": {
    "adminPassword": null,
    "adminUsername": "azureuser",
    "allowExtensionOperations": true,
    "computerName": "TestVM",
    "customData": null,
    "linuxConfiguration": {
      "disablePasswordAuthentication": true,
      "provisionVmAgent": true,
      "ssh": {
        "publicKeys": [
          {
            "keyData": "ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQDMobZNJTqgjWn/IB5xlilvE4Y+BMYpqkDnGRUcA0g9BYPgrGSQquCES37v2e3JmpfDPHFsaR+CPKlVr2GoVJMMHeRcMJhj50ZWq0hAnkJBhlZVWy8S7dwdGAqPyPmWM2iJDCVMVrLITAJCno47O4Ees7RCH6ku7kU86b1NOanvrNwqTHr14wtnLhgZ0gQ5GV1oLWvMEVg1YFMIgPRkTsSQKWCG5lLqQ45aU/4NMJoUxGyJTL9i8YxMavaB1Z2npfTQDQo9+womZ7SXzHaIWC858gWNl9e5UFyHDnTEDc14hKkf1CqnGJVcCJkmSfmrrHk/CkmF0ZT3whTHO1DhJTtV stramer@contoso",
            "path": "/home/azureuser/.ssh/authorized_keys"
          }
        ]
      }
    },
    "secrets": [],
    "windowsConfiguration": null
  },
  ....
}
```

<span data-ttu-id="2d6a2-120">La commande suivante récupère les clés publiques SSH autorisées à se connecter à la machine virtuelle en ajoutant une requête :</span><span class="sxs-lookup"><span data-stu-id="2d6a2-120">The following command gets the SSH public keys authorized to connect to the VM by adding a query:</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query osProfile.linuxConfiguration.ssh.publicKeys -o json
```

```json
[
  {
    "keyData": "ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQDMobZNJTqgjWn/IB5xlilvE4Y+BMYpqkDnGRUcA0g9BYPgrGSQquCES37v2e3JmpfDPHFsaR+CPKlVr2GoVJMMHeRcMJhj50ZWq0hAnkJBhlZVWy8S7dwdGAqPyPmWM2iJDCVMVrLITAJCno47O4Ees7RCH6ku7kU86b1NOanvrNwqTHr14wtnLhgZ0gQ5GV1oLWvMEVg1YFMIgPRkTsSQKWCG5lLqQ45aU/4NMJoUxGyJTL9i8YxMavaB1Z2npfTQDQo9+womZ7SXzHaIWC858gWNl9e5UFyHDnTEDc14hKkf1CqnGJVcCJkmSfmrrHk/CkmF0ZT3whTHO1DhJTtV stramer@contoso",
    "path": "/home/azureuser/.ssh/authorized_keys"
  }
]
```

<span data-ttu-id="2d6a2-121">Pour récupérer plusieurs propriétés, placez des expressions entre crochets `[ ]` (une __liste à sélection multiple__) sous la forme d’une liste séparée par des virgules.</span><span class="sxs-lookup"><span data-stu-id="2d6a2-121">To get more than one property, put expressions in square brackets  `[ ]` (a __multiselect list__) as a comma-separated list.</span></span> <span data-ttu-id="2d6a2-122">Pour récupérer en une seule fois le nom de la machine virtuelle, l’utilisateur administrateur et la clé SSH, utilisez la commande :</span><span class="sxs-lookup"><span data-stu-id="2d6a2-122">To get the VM name, admin user, and SSH key all at once use the command:</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query '[name, osProfile.adminUsername, osProfile.linuxConfiguration.ssh.publicKeys[0].keyData]' -o json
```

```json
[
  "TestVM",
  "azureuser",
  "ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQDMobZNJTqgjWn/IB5xlilvE4Y+BMYpqkDnGRUcA0g9BYPgrGSQquCES37v2e3JmpfDPHFsaR+CPKlVr2GoVJMMHeRcMJhj50ZWq0hAnkJBhlZVWy8S7dwdGAqPyPmWM2iJDCVMVrLITAJCno47O4Ees7RCH6ku7kU86b1NOanvrNwqTHr14wtnLhgZ0gQ5GV1oLWvMEVg1YFMIgPRkTsSQKWCG5lLqQ45aU/4NMJoUxGyJTL9i8YxMavaB1Z2npfTQDQo9+womZ7SXzHaIWC858gWNl9e5UFyHDnTEDc14hKkf1CqnGJVcCJkmSfmrrHk/CkmF0ZT3whTHO1DhJTtV stramer@contoso"
]
```

<span data-ttu-id="2d6a2-123">Ces valeurs sont répertoriées dans le tableau des résultats, dans l’ordre où ils ont été donnés dans la requête.</span><span class="sxs-lookup"><span data-stu-id="2d6a2-123">These values are listed in the result array in the order they were given in the query.</span></span> <span data-ttu-id="2d6a2-124">Étant donné que le résultat est un tableau, aucune clé n’est associée aux résultats.</span><span class="sxs-lookup"><span data-stu-id="2d6a2-124">Since the result is an array, there are no keys associated with the results.</span></span>

## <a name="get-a-single-value"></a><span data-ttu-id="2d6a2-125">Obtenir une seule valeur</span><span class="sxs-lookup"><span data-stu-id="2d6a2-125">Get a single value</span></span>

<span data-ttu-id="2d6a2-126">Voici un cas courant : vous avez besoin obtenir _une seule_ valeur d’une commande CLI, telle qu’un ID de ressource Azure, un nom de ressource, un nom d’utilisateur ou un mot de passe.</span><span class="sxs-lookup"><span data-stu-id="2d6a2-126">A common case is that you need to only get _one_ value out of a CLI command, such as an Azure resource ID, a resource name, a username, or a password.</span></span> <span data-ttu-id="2d6a2-127">Dans ce cas, vous souhaitez également souvent stocker la valeur dans une variable d’environnement locale.</span><span class="sxs-lookup"><span data-stu-id="2d6a2-127">In that case, you also often want to store the value in a local environment variable.</span></span> <span data-ttu-id="2d6a2-128">Pour obtenir une seule propriété, veillez d’abord à obtenir une seule propriété de la requête.</span><span class="sxs-lookup"><span data-stu-id="2d6a2-128">To get a single property, first make sure that you're only getting one property out of the query.</span></span> <span data-ttu-id="2d6a2-129">Modification de l’exemple précédent pour obtenir uniquement le nom d’utilisateur administrateur :</span><span class="sxs-lookup"><span data-stu-id="2d6a2-129">Modifying the last example to get only the admin username:</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query 'osProfile.adminUsername' -o json
```

```JSON
"azureuser"
```

<span data-ttu-id="2d6a2-130">Cela ressemble à une seule valeur valide. Toutefois, notez que les caractères `"` sont retournés dans la sortie.</span><span class="sxs-lookup"><span data-stu-id="2d6a2-130">This looks like a valid single value, but note that the `"` characters are returned as part of the output.</span></span> <span data-ttu-id="2d6a2-131">Cela indique que l’objet est une chaîne JSON.</span><span class="sxs-lookup"><span data-stu-id="2d6a2-131">This indicates that the object is a JSON string.</span></span> <span data-ttu-id="2d6a2-132">Note importante : lorsque vous affectez cette valeur directement en tant que sortie de la commande vers une variable d’environnement, les guillemets ne peuvent __pas__ être interprétées par l’interpréteur de commandes :</span><span class="sxs-lookup"><span data-stu-id="2d6a2-132">It's important to note that when you assign this value directly as output from the command to an environment variable, the quotes may __not__ be interpreted by the shell:</span></span>

```bash
USER=$(az vm show -g QueryDemo -n TestVM --query 'osProfile.adminUsername' -o json)
echo $USER
```

```output
"azureuser"
```

<span data-ttu-id="2d6a2-133">Ce n’est probablement pas ce que vous voulez.</span><span class="sxs-lookup"><span data-stu-id="2d6a2-133">This is almost certainly not what you want.</span></span> <span data-ttu-id="2d6a2-134">Dans ce cas, utilisez un format de sortie qui ne place pas les valeurs retournées entre des informations de type.</span><span class="sxs-lookup"><span data-stu-id="2d6a2-134">In this case, you want to use an output format which doesn't enclose returned values with type information.</span></span> <span data-ttu-id="2d6a2-135">La meilleure option de sortie de l’interface CLI à cette fin est `tsv` (valeurs séparées par une tabulation).</span><span class="sxs-lookup"><span data-stu-id="2d6a2-135">The best output option that the CLI offers for this purpose is `tsv`, tab-separated values.</span></span> <span data-ttu-id="2d6a2-136">En particulier, lorsque vous récupérez une valeur qui n’est qu’une seule valeur (pas un dictionnaire ou une liste), vous avez la garantie que la sortie `tsv` n’est pas entre guillemets.</span><span class="sxs-lookup"><span data-stu-id="2d6a2-136">In particular, when retrieving a value that's only a single value (not a dictionary or list), `tsv` output is guaranteed to be unqoted.</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query 'osProfile.adminUsername' -o tsv
```

```output
azureuser
```

<span data-ttu-id="2d6a2-137">Pour plus d’informations sur le format de sortie `tsv`, consultez [Formats de sortie : format de sortie TSV](format-output-azure-cli.md#tsv-output-format)</span><span class="sxs-lookup"><span data-stu-id="2d6a2-137">For more information about the `tsv` output format, see [Output formats - TSV output format](format-output-azure-cli.md#tsv-output-format)</span></span>

## <a name="rename-properties-in-a-query"></a><span data-ttu-id="2d6a2-138">Renommer des propriétés dans une requête</span><span class="sxs-lookup"><span data-stu-id="2d6a2-138">Rename properties in a query</span></span>

<span data-ttu-id="2d6a2-139">Pour récupérer un dictionnaire à la place d’un tableau lors de l’interrogation de plusieurs valeurs, utilisez l’opérateur `{ }` (__code de hachage à sélection multiple__).</span><span class="sxs-lookup"><span data-stu-id="2d6a2-139">To get a dictionary instead of an array when querying for multiple values, use the `{ }` (__multiselect hash__) operator.</span></span>
<span data-ttu-id="2d6a2-140">Le format d’un hachage à sélection multiple est `{displayName:JMESPathExpression, ...}`.</span><span class="sxs-lookup"><span data-stu-id="2d6a2-140">The format for a multiselect hash is `{displayName:JMESPathExpression, ...}`.</span></span>
<span data-ttu-id="2d6a2-141">`displayName` correspond à la chaîne indiquée dans la sortie, tandis que `JMESPathExpression` correspond à l’expression JMESPath à évaluer.</span><span class="sxs-lookup"><span data-stu-id="2d6a2-141">`displayName` will be the string shown in output, and `JMESPathExpression` is the JMESPath expression to evaluate.</span></span> <span data-ttu-id="2d6a2-142">Modification de l’exemple de la dernière section en remplaçant la liste à sélection multiple par un hachage :</span><span class="sxs-lookup"><span data-stu-id="2d6a2-142">Modifying the example from the last section by changing the multiselect list to a hash:</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query '{VMName:name, admin:osProfile.adminUsername, sshKey:osProfile.linuxConfiguration.ssh.publicKeys[0].keyData }' -o json
```

```json
{
  "VMName": "TestVM",
  "admin": "azureuser",
  "ssh-key": "ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQDMobZNJTqgjWn/IB5xlilvE4Y+BMYpqkDnGRUcA0g9BYPgrGSQquCES37v2e3JmpfDPHFsaR+CPKlVr2GoVJMMHeRcMJhj50ZWq0hAnkJBhlZVWy8S7dwdGAqPyPmWM2iJDCVMVrLITAJCno47O4Ees7RCH6ku7kU86b1NOanvrNwqTHr14wtnLhgZ0gQ5GV1oLWvMEVg1YFMIgPRkTsSQKWCG5lLqQ45aU/4NMJoUxGyJTL9i8YxMavaB1Z2npfTQDQo9+womZ7SXzHaIWC858gWNl9e5UFyHDnTEDc14hKkf1CqnGJVcCJkmSfmrrHk/CkmF0ZT3whTHO1DhJTtV stramer@contoso"
}
```

## <a name="get-properties-in-an-array"></a><span data-ttu-id="2d6a2-143">Récupérer des propriétés dans un tableau</span><span class="sxs-lookup"><span data-stu-id="2d6a2-143">Get properties in an array</span></span>

<span data-ttu-id="2d6a2-144">Un tableau n’a aucune propriété propre, mais il peut être indexé.</span><span class="sxs-lookup"><span data-stu-id="2d6a2-144">An array has no properties of its own, but it can be indexed.</span></span> <span data-ttu-id="2d6a2-145">Cette fonctionnalité est illustrée dans le dernier exemple avec l’expression `publicKeys[0]`, qui obtient le premier élément du tableau `publicKeys`.</span><span class="sxs-lookup"><span data-stu-id="2d6a2-145">This feature is shown in the last example with the expression `publicKeys[0]`, which gets the first element of the `publicKeys` array.</span></span> <span data-ttu-id="2d6a2-146">Le fait que la sortie CLI soit ordonnée n’est pas garanti ; nous vous conseillons donc d’éviter d’utiliser l’indexation, sauf si vous êtes certain de l’ordre ou si le type d’élément que vous récupérerez vous importe peu.</span><span class="sxs-lookup"><span data-stu-id="2d6a2-146">There's no guarantee CLI output is ordered, so avoid using indexing unless you're sure of the order or don't care what element you get.</span></span> <span data-ttu-id="2d6a2-147">Pour accéder aux propriétés des éléments dans un tableau, vous effectuez l’une des deux opérations suivantes : _mise à plat_ et _filtrage_.</span><span class="sxs-lookup"><span data-stu-id="2d6a2-147">To access the properties of elements in an array, you do one of two operations: _flattening_ and _filtering_.</span></span> <span data-ttu-id="2d6a2-148">Cette section explique comment aplatir un tableau.</span><span class="sxs-lookup"><span data-stu-id="2d6a2-148">This section covers how to flatten an array.</span></span>

<span data-ttu-id="2d6a2-149">La mise à plat d’un tableau est effectuée avec l’opérateur JMESPath `[]`.</span><span class="sxs-lookup"><span data-stu-id="2d6a2-149">Flattening an array is done with the `[]` JMESPath operator.</span></span> <span data-ttu-id="2d6a2-150">Toutes les expressions après l’opérateur `[]` sont appliquées à chaque élément du tableau actuel.</span><span class="sxs-lookup"><span data-stu-id="2d6a2-150">All expressions after the `[]` operator are applied to each element in the current array.</span></span>
<span data-ttu-id="2d6a2-151">Si l’opérateur `[]` apparaît au début de la requête, il aplatit le résultat de la commande CLI.</span><span class="sxs-lookup"><span data-stu-id="2d6a2-151">If `[]` appears at the start of the query, it flattens the CLI command result.</span></span> <span data-ttu-id="2d6a2-152">Les résultats de `az vm list` peuvent être examinés avec cette fonctionnalité.</span><span class="sxs-lookup"><span data-stu-id="2d6a2-152">The results of `az vm list` can be inspected with this feature.</span></span>
<span data-ttu-id="2d6a2-153">Pour récupérer le nom, le système d’exploitation et le nom d’administrateur de chacune des machines virtuelles dans un groupe de ressources :</span><span class="sxs-lookup"><span data-stu-id="2d6a2-153">To get the name, OS, and administrator name for each VM in a resource group:</span></span>

```azurecli-interactive
az vm list -g QueryDemo --query '[].{Name:name, OS:storageProfile.osDisk.osType, admin:osProfile.adminUsername}' -o json
```

```json
[
  {
    "Name": "Test-2",
    "OS": "Linux",
    "admin": "sttramer"
  },
  {
    "Name": "TestVM",
    "OS": "Linux",
    "admin": "azureuser"
  },
  {
    "Name": "WinTest",
    "OS": "Windows",
    "admin": "winadmin"
  }
]
```

<span data-ttu-id="2d6a2-154">Combinés avec le format de sortie `--output table`, les noms de colonne correspondent à la valeur `displayKey` du hachage à sélection multiple :</span><span class="sxs-lookup"><span data-stu-id="2d6a2-154">When combined with the `--output table` output format, the column names match up with the `displayKey` value of the multiselect hash:</span></span>

```azurecli-interactive
az vm list -g QueryDemo --query '[].{Name:name, OS:storageProfile.osDisk.osType, Admin:osProfile.adminUsername}' --output table
```

```output
Name     OS       Admin
-------  -------  ---------
Test-2   Linux    sttramer
TestVM   Linux    azureuser
WinTest  Windows  winadmin
```

> [!NOTE]
>
> <span data-ttu-id="2d6a2-155">Certaines clés sont filtrées et non pas imprimées dans l’affichage de table.</span><span class="sxs-lookup"><span data-stu-id="2d6a2-155">Certain keys are filtered out and not printed in the table view.</span></span> <span data-ttu-id="2d6a2-156">Il s’agit des clés `id`, `type` et `etag`.</span><span class="sxs-lookup"><span data-stu-id="2d6a2-156">These keys are `id`, `type`, and `etag`.</span></span> <span data-ttu-id="2d6a2-157">Pour afficher ces valeurs, vous pouvez modifier le nom de clé dans un hachage à sélection multiple.</span><span class="sxs-lookup"><span data-stu-id="2d6a2-157">To see these values, you can change the key name in a multiselect hash.</span></span>
>
> ```azurecli-interactive
> az vm show -g QueryDemo -n TestVM --query "{objectID:id}" -o table
> ```

<span data-ttu-id="2d6a2-158">Tous les tableaux peuvent être aplatis, pas seulement le résultat de niveau supérieur renvoyé par la commande.</span><span class="sxs-lookup"><span data-stu-id="2d6a2-158">Any array can be flattened, not just the top-level result returned by the command.</span></span> <span data-ttu-id="2d6a2-159">Dans la dernière section, l’expression `osProfile.linuxConfiguration.ssh.publicKeys[0].keyData` a été utilisée pour récupérer la clé publique SSH pour la connexion.</span><span class="sxs-lookup"><span data-stu-id="2d6a2-159">In the last section, the expression `osProfile.linuxConfiguration.ssh.publicKeys[0].keyData` was used to get the SSH public key for sign-in.</span></span> <span data-ttu-id="2d6a2-160">Pour récupérer _chaque_ clé publique SSH, l’expression peut plutôt être écrite sous la forme `osProfile.linuxConfiguration.ssh.publicKeys[].keyData`.</span><span class="sxs-lookup"><span data-stu-id="2d6a2-160">To get _every_ SSH public key, the expression could instead be written as `osProfile.linuxConfiguration.ssh.publicKeys[].keyData`.</span></span>
<span data-ttu-id="2d6a2-161">Cette expression de requête aplatit le tableau `osProfile.linuxConfiguration.ssh.publicKeys`, puis exécute l’expression `keyData` sur chaque élément :</span><span class="sxs-lookup"><span data-stu-id="2d6a2-161">This query expression flattens the `osProfile.linuxConfiguration.ssh.publicKeys` array, and then runs the `keyData` expression on each element:</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query '{VMName:name, admin:osProfile.adminUsername, sshKeys:osProfile.linuxConfiguration.ssh.publicKeys[].keyData }' -o json
```

```json
{
  "VMName": "TestVM",
  "admin": "azureuser",
  "sshKeys": [
    "ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQDMobZNJTqgjWn/IB5xlilvE4Y+BMYpqkDnGRUcA0g9BYPgrGSQquCES37v2e3JmpfDPHFsaR+CPKlVr2GoVJMMHeRcMJhj50ZWq0hAnkJBhlZVWy8S7dwdGAqPyPmWM2iJDCVMVrLITAJCno47O4Ees7RCH6ku7kU86b1NOanvrNwqTHr14wtnLhgZ0gQ5GV1oLWvMEVg1YFMIgPRkTsSQKWCG5lLqQ45aU/4NMJoUxGyJTL9i8YxMavaB1Z2npfTQDQo9+womZ7SXzHaIWC858gWNl9e5UFyHDnTEDc14hKkf1CqnGJVcCJkmSfmrrHk/CkmF0ZT3whTHO1DhJTtV stramer@contoso\n"
  ]
}
```

## <a name="filter-arrays"></a><span data-ttu-id="2d6a2-162">Filtrer des tableaux</span><span class="sxs-lookup"><span data-stu-id="2d6a2-162">Filter arrays</span></span>

<span data-ttu-id="2d6a2-163">Le _filtrage_ est l’autre opération utilisée pour récupérer des données à partir d’un tableau.</span><span class="sxs-lookup"><span data-stu-id="2d6a2-163">The other operation used to get data from an array is _filtering_.</span></span> <span data-ttu-id="2d6a2-164">Il est effectué avec l’opérateur JMESPath `[?...]`.</span><span class="sxs-lookup"><span data-stu-id="2d6a2-164">Filtering is done with the `[?...]` JMESPath operator.</span></span>
<span data-ttu-id="2d6a2-165">Cet opérateur utilise un prédicat en tant que contenus.</span><span class="sxs-lookup"><span data-stu-id="2d6a2-165">This operator takes a predicate as its contents.</span></span> <span data-ttu-id="2d6a2-166">Un prédicat est une instruction qui peut être évaluée avec les valeurs `true` ou `false`.</span><span class="sxs-lookup"><span data-stu-id="2d6a2-166">A predicate is any statement that can be evaluated to either `true` or `false`.</span></span> <span data-ttu-id="2d6a2-167">Les expressions dans lesquelles la valeur d’évaluation du prédicat est `true` sont incluses dans la sortie.</span><span class="sxs-lookup"><span data-stu-id="2d6a2-167">Expressions where the predicate evaluates to `true` are included in the output.</span></span>

<span data-ttu-id="2d6a2-168">JMESPath propose la comparaison standard et des opérateurs logiques.</span><span class="sxs-lookup"><span data-stu-id="2d6a2-168">JMESPath offers the standard comparison and logical operators.</span></span> <span data-ttu-id="2d6a2-169">Ces derniers comprennent `<`, `<=`, `>`, `>=`, `==` et `!=`.</span><span class="sxs-lookup"><span data-stu-id="2d6a2-169">These include `<`, `<=`, `>`, `>=`, `==`, and `!=`.</span></span>
<span data-ttu-id="2d6a2-170">JMESPath prend également en charge les opérateurs logiques Et (`&&`), Ou (`||`) et Non (`!`).</span><span class="sxs-lookup"><span data-stu-id="2d6a2-170">JMESPath also supports logical and (`&&`), or (`||`), and not (`!`).</span></span> <span data-ttu-id="2d6a2-171">Les expressions peuvent être regroupées dans des parenthèses, ce qui permet d’obtenir des expressions de prédicat plus complexes.</span><span class="sxs-lookup"><span data-stu-id="2d6a2-171">Expressions can be grouped within parenthesis, allowing for more complex predicate expressions.</span></span> <span data-ttu-id="2d6a2-172">Pour plus d’informations sur les prédicats et les opérations logiques, consultez [JMESPath Specification](http://jmespath.org/specification.html) (Spécification JMESPath).</span><span class="sxs-lookup"><span data-stu-id="2d6a2-172">For the full details on predicates and logical operations, see the [JMESPath specification](http://jmespath.org/specification.html).</span></span>

<span data-ttu-id="2d6a2-173">Dans la dernière section, nous avons aplati un tableau pour récupérer la liste complète des machines virtuelles dans un groupe de ressources.</span><span class="sxs-lookup"><span data-stu-id="2d6a2-173">In the last section, we flattened an array to get the complete list of all VMs in a resource group.</span></span> <span data-ttu-id="2d6a2-174">Grâce à des filtres, nous pouvons réduire cette sortie pour afficher uniquement les machines virtuelles Linux :</span><span class="sxs-lookup"><span data-stu-id="2d6a2-174">Using filters, this output can be restricted to only Linux VMs:</span></span>

```azurecli-interactive
az vm list -g QueryDemo --query "[?storageProfile.osDisk.osType=='Linux'].{Name:name,  admin:osProfile.adminUsername}" --output table
```

```output
Name    Admin
------  ---------
Test-2  sttramer
TestVM  azureuser
```

> [!IMPORTANT]
>
> <span data-ttu-id="2d6a2-175">Dans JMESPath, les chaînes sont toujours placées entre des guillemets simples (`'`).</span><span class="sxs-lookup"><span data-stu-id="2d6a2-175">In JMESPath, strings are always surrounded by single quotes (`'`).</span></span> <span data-ttu-id="2d6a2-176">Si vous utilisez des guillemets doubles comme partie d’une chaîne dans un prédicat de filtre, vous obtiendrez une sortie vide.</span><span class="sxs-lookup"><span data-stu-id="2d6a2-176">If you use double quotes as part of a string in a filter predicate, you'll get empty output.</span></span>

<span data-ttu-id="2d6a2-177">JMESPath dispose également de fonctions intégrées qui peuvent simplifier le filtrage.</span><span class="sxs-lookup"><span data-stu-id="2d6a2-177">JMESPath also has built-in functions that can help with filtering.</span></span> <span data-ttu-id="2d6a2-178">C’est le cas de la fonction `contains(string, substring)`, qui vérifie si une chaîne contient une sous-chaîne.</span><span class="sxs-lookup"><span data-stu-id="2d6a2-178">One such function is `contains(string, substring)`, which checks to see if a string contains a substring.</span></span> <span data-ttu-id="2d6a2-179">Les expressions étant évaluées avant d’appeler la fonction, le premier argument peut être une expression JMESPath complète.</span><span class="sxs-lookup"><span data-stu-id="2d6a2-179">Expressions are evaluated before calling the function, so the first argument can be a full JMESPath expression.</span></span> <span data-ttu-id="2d6a2-180">L’exemple suivant recherche toutes les machines virtuelles utilisant un stockage SSD pour leur disque de système d’exploitation :</span><span class="sxs-lookup"><span data-stu-id="2d6a2-180">The next example finds all VMs using SSD storage for their OS disk:</span></span>

```azurecli-interactive
az vm list -g QueryDemo --query "[?contains(storageProfile.osDisk.managedDisk.storageAccountType,'SSD')].{Name:name, Storage:storageProfile.osDisk.managedDisk.storageAccountType}" -o json
```

```json
[
  {
    "Name": "TestVM",
    "Storage": "StandardSSD_LRS"
  },
  {
    "Name": "WinTest",
    "Storage": "StandardSSD_LRS"
  }
]
```

<span data-ttu-id="2d6a2-181">Cette requête est un peu longue.</span><span class="sxs-lookup"><span data-stu-id="2d6a2-181">This query is a little long.</span></span> <span data-ttu-id="2d6a2-182">La clé `storageProfile.osDisk.managedDisk.storageAccountType` est mentionnée à deux reprises, puis récréée dans la sortie.</span><span class="sxs-lookup"><span data-stu-id="2d6a2-182">The `storageProfile.osDisk.managedDisk.storageAccountType` key is mentioned twice, and rekeyed in the output.</span></span> <span data-ttu-id="2d6a2-183">Pour raccourcir ce processus, vous pouvez appliquer le filtre après la mise à plat et la sélection des données.</span><span class="sxs-lookup"><span data-stu-id="2d6a2-183">One way to shorten it is to apply the filter after flattening and selecting data.</span></span>

```azurecli-interactive
az vm list -g QueryDemo --query "[].{Name:name, Storage:storageProfile.osDisk.managedDisk.storageAccountType}[?contains(Storage,'SSD')]" -o json
```

```json
[
  {
    "Name": "TestVM",
    "Storage": "StandardSSD_LRS"
  },
  {
    "Name": "WinTest",
    "Storage": "StandardSSD_LRS"
  }
]
```

<span data-ttu-id="2d6a2-184">Pour les tableaux volumineux, il peut être plus rapide d’appliquer le filtre avant de sélectionner des données.</span><span class="sxs-lookup"><span data-stu-id="2d6a2-184">For large arrays, it may be faster to apply the filter before selecting data.</span></span>

<span data-ttu-id="2d6a2-185">Consultez [JMESPath specification - Built-in Functions](http://jmespath.org/specification.html#built-in-functions) (Spécification JMESPath - Fonctions intégrées) pour obtenir la liste complète des fonctions.</span><span class="sxs-lookup"><span data-stu-id="2d6a2-185">See the [JMESPath specification - Built-in Functions](http://jmespath.org/specification.html#built-in-functions) for the full list of functions.</span></span>

## <a name="change-output"></a><span data-ttu-id="2d6a2-186">Modifier la sortie</span><span class="sxs-lookup"><span data-stu-id="2d6a2-186">Change output</span></span>

<span data-ttu-id="2d6a2-187">Les fonctions JMESPath jouent également un autre rôle, celui d’agir sur les résultats d’une requête.</span><span class="sxs-lookup"><span data-stu-id="2d6a2-187">JMESPath functions also have another purpose, which is to operate on the results of a query.</span></span> <span data-ttu-id="2d6a2-188">Toutes les fonctions qui renvoient une valeur non booléenne modifient le résultat d’une expression.</span><span class="sxs-lookup"><span data-stu-id="2d6a2-188">Any function that returns a non-boolean value changes the result of an expression.</span></span>
<span data-ttu-id="2d6a2-189">Par exemple, vous pouvez trier des données par valeur de propriété avec `sort_by(array, &sort_expression)`.</span><span class="sxs-lookup"><span data-stu-id="2d6a2-189">For example, you can sort data by a property value with `sort_by(array, &sort_expression)`.</span></span> <span data-ttu-id="2d6a2-190">JMESPath utilise un opérateur spécial, `&`, pour les expressions qui doivent être évaluées ultérieurement dans le cadre d’une fonction.</span><span class="sxs-lookup"><span data-stu-id="2d6a2-190">JMESPath uses a special operator, `&`, for expressions that should be evaluated later as part of a function.</span></span> <span data-ttu-id="2d6a2-191">L’exemple suivant montre comment trier une liste de machines virtuelles par taille de disque de système d’exploitation :</span><span class="sxs-lookup"><span data-stu-id="2d6a2-191">The next example shows how to sort a VM list by OS disk size:</span></span>

```azurecli-interactive
az vm list -g QueryDemo --query "sort_by([].{Name:name, Size:storageProfile.osDisk.diskSizeGb}, &Size)" --output table
```

```output
Name     Size
-------  ------
TestVM   30
Test-2   32
WinTest  127
```

<span data-ttu-id="2d6a2-192">Consultez [JMESPath specification - Built-in Functions](http://jmespath.org/specification.html#built-in-functions) (Spécification JMESPath - Fonctions intégrées) pour obtenir la liste complète des fonctions.</span><span class="sxs-lookup"><span data-stu-id="2d6a2-192">See the [JMESPath specification - Built-in Functions](http://jmespath.org/specification.html#built-in-functions) for the full list of functions.</span></span>

## <a name="experiment-with-queries-interactively"></a><span data-ttu-id="2d6a2-193">Essayer des requêtes de façon interactive</span><span class="sxs-lookup"><span data-stu-id="2d6a2-193">Experiment with queries interactively</span></span>

<span data-ttu-id="2d6a2-194">Pour commencer à expérimenter JMESPath, le package Python [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal) propose un environnement interactif permettant d’utiliser des requêtes.</span><span class="sxs-lookup"><span data-stu-id="2d6a2-194">To start experimenting with JMESPath, the [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal) Python package offers an interactive environment to work with queries.</span></span> <span data-ttu-id="2d6a2-195">Les données sont transmises en tant qu’entrées, puis les requêtes sont écrites et exécutées dans l’éditeur.</span><span class="sxs-lookup"><span data-stu-id="2d6a2-195">Data is piped as input, and then queries are written and run in the editor.</span></span>

```bash
pip install jmespath-terminal
az vm list --output json | jpterm
```
