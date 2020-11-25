---
title: Interroger des résultats de commande avec Azure CLI
description: Apprenez à exécuter des requêtes JMESPath sur la sortie des commandes Azure CLI.
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 09/23/2019
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: 780fc2dc87f949a1f36228af7a49cd987cb10cf6
ms.sourcegitcommit: 753de7d5c45062d5138be86ced7eacddd5696ca3
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/20/2020
ms.locfileid: "94976830"
---
# <a name="query-azure-cli-command-output"></a>Interroger la sortie de commande Azure CLI

Azure CLI utilise l’argument `--query` pour exécuter une [requête JMESPath](http://jmespath.org) sur les résultats des commandes. JMESPath est un langage de requête pour JSON, qui vous permet de sélectionner et de modifier des données depuis une sortie CLI. Les requêtes sont exécutées sur la sortie JSON, avant toute mise en forme de l’affichage.

L’argument `--query` est pris en charge par toutes les commandes dans Azure CLI. Cet article explique comment utiliser les fonctionnalités de JMESPath avec une série d’exemples courts et simples.

> [!NOTE]
>
> Lors de l’utilisation d’Azure CLI dans PowerShell sur Windows, des séquences d’échappement supplémentaires peuvent être nécessaires pour l’argument query. Pour plus d’informations, consultez [Problèmes liés aux guillemets avec PowerShell](https://github.com/Azure/azure-cli/blob/dev/doc/quoting-issues-with-powershell.md).

## <a name="dictionary-and-list-cli-results"></a>Résultats CLI de liste et de dictionnaire

Même quand vous utilisez un format de sortie autre que JSON, les résultats de la commande CLI sont tout d’abord traités comme du code JSON pour les requêtes. Les résultats CLI se présentent sous la forme d’un dictionnaire ou d’un tableau JSON. Les tableaux sont des séquences d’objets qui peuvent être indexés, et les dictionnaires sont des objets non ordonnés accessibles avec des clés. Les commandes qui _peuvent_ renvoyer plus d’un objet renvoient un tableau, et les commandes qui renvoient _toujours_ et _uniquement_ un seul objet renvoient un dictionnaire.

## <a name="get-properties-in-a-dictionary"></a>Récupérer des propriétés dans un dictionnaire

En utilisant des résultats de dictionnaire, vous pouvez accéder à des propriétés de niveau supérieur simplement avec la clé. Le caractère `.` (__sous-expression__) est utilisé pour accéder aux propriétés des dictionnaires imbriqués. Avant d’introduire des requêtes, examinez la sortie non modifiée de la commande `az vm show` :

```azurecli-interactive
az vm show -g QueryDemo -n TestVM -o json
```

La commande génère un dictionnaire. Certains contenus ont été omis.

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

La commande suivante récupère les clés publiques SSH autorisées à se connecter à la machine virtuelle en ajoutant une requête :

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

## <a name="get-a-single-value"></a>Obtenir une seule valeur

Voici un cas courant : vous avez besoin obtenir _une seule_ valeur d’une commande CLI, telle qu’un ID de ressource Azure, un nom de ressource, un nom d’utilisateur ou un mot de passe. Dans ce cas, vous souhaitez également souvent stocker la valeur dans une variable d’environnement locale. Pour obtenir une seule propriété, veillez d’abord à obtenir une seule propriété de la requête. Modification de l’exemple précédent pour obtenir uniquement le nom d’utilisateur administrateur :

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query 'osProfile.adminUsername' -o json
```

```JSON
"azureuser"
```

Cela ressemble à une seule valeur valide. Toutefois, notez que les caractères `"` sont retournés dans la sortie. Cela indique que l’objet est une chaîne JSON. Note importante : lorsque vous affectez cette valeur directement en tant que sortie de la commande vers une variable d’environnement, les guillemets ne peuvent __pas__ être interprétées par l’interpréteur de commandes :

```bash
USER=$(az vm show -g QueryDemo -n TestVM --query 'osProfile.adminUsername' -o json)
echo $USER
```

```output
"azureuser"
```

Ce n’est probablement pas ce que vous voulez. Dans ce cas, utilisez un format de sortie qui ne place pas les valeurs retournées entre des informations de type. La meilleure option de sortie de l’interface CLI à cette fin est `tsv` (valeurs séparées par une tabulation). En particulier, quand vous récupérez une valeur qui n’est qu’une seule valeur (pas un dictionnaire ou une liste), vous avez la garantie que la sortie `tsv` n’est pas entre guillemets.

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query 'osProfile.adminUsername' -o tsv
```

```output
azureuser
```

Pour plus d’informations sur le format de sortie `tsv`, consultez [Formats de sortie : format de sortie TSV](format-output-azure-cli.md#tsv-output-format)

## <a name="get-multiple-values"></a>Obtenir plusieurs valeurs

Pour récupérer plusieurs propriétés, placez des expressions entre crochets `[ ]` (une __liste à sélection multiple__) sous la forme d’une liste séparée par des virgules. Pour récupérer en une seule fois le nom de la machine virtuelle, l’utilisateur administrateur et la clé SSH, utilisez la commande :

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

Ces valeurs sont répertoriées dans le tableau des résultats, dans l’ordre où ils ont été donnés dans la requête. Étant donné que le résultat est un tableau, aucune clé n’est associée aux résultats.

## <a name="rename-properties-in-a-query"></a>Renommer des propriétés dans une requête

Pour récupérer un dictionnaire à la place d’un tableau lors de l’interrogation de plusieurs valeurs, utilisez l’opérateur `{ }` (__code de hachage à sélection multiple__).
Le format d’un hachage à sélection multiple est `{displayName:JMESPathExpression, ...}`.
`displayName` correspond à la chaîne indiquée dans la sortie, tandis que `JMESPathExpression` correspond à l’expression JMESPath à évaluer. Modification de l’exemple de la dernière section en remplaçant la liste à sélection multiple par un hachage :

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

## <a name="get-properties-in-an-array"></a>Récupérer des propriétés dans un tableau

Un tableau n’a aucune propriété propre, mais il peut être indexé. Cette fonctionnalité est illustrée dans le dernier exemple avec l’expression `publicKeys[0]`, qui obtient le premier élément du tableau `publicKeys`. Le fait que la sortie CLI soit ordonnée n’est pas garanti ; nous vous conseillons donc d’éviter d’utiliser l’indexation, sauf si vous êtes certain de l’ordre ou si le type d’élément que vous récupérerez vous importe peu. Pour accéder aux propriétés des éléments dans un tableau, vous effectuez l’une des deux opérations suivantes : _mise à plat_ et _filtrage_. Cette section explique comment aplatir un tableau.

La mise à plat d’un tableau est effectuée avec l’opérateur JMESPath `[]`. Toutes les expressions après l’opérateur `[]` sont appliquées à chaque élément du tableau actuel.
Si l’opérateur `[]` apparaît au début de la requête, il aplatit le résultat de la commande CLI. Les résultats de `az vm list` peuvent être examinés avec cette fonctionnalité.
Pour récupérer le nom, le système d’exploitation et le nom d’administrateur de chacune des machines virtuelles dans un groupe de ressources :

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

Combinés avec le format de sortie `--output table`, les noms de colonne correspondent à la valeur `displayKey` du hachage à sélection multiple :

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
> Certaines clés sont filtrées et non pas imprimées dans l’affichage de table. Il s’agit des clés `id`, `type` et `etag`. Pour afficher ces valeurs, vous pouvez modifier le nom de clé dans un hachage à sélection multiple.
>
> ```azurecli-interactive
> az vm show -g QueryDemo -n TestVM --query "{objectID:id}" -o table
> ```

Tous les tableaux peuvent être aplatis, pas seulement le résultat de niveau supérieur renvoyé par la commande. Dans la dernière section, l’expression `osProfile.linuxConfiguration.ssh.publicKeys[0].keyData` a été utilisée pour récupérer la clé publique SSH pour la connexion. Pour récupérer _chaque_ clé publique SSH, l’expression peut plutôt être écrite sous la forme `osProfile.linuxConfiguration.ssh.publicKeys[].keyData`.
Cette expression de requête aplatit le tableau `osProfile.linuxConfiguration.ssh.publicKeys`, puis exécute l’expression `keyData` sur chaque élément :

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

## <a name="filter-arrays"></a>Filtrer des tableaux

Le _filtrage_ est l’autre opération utilisée pour récupérer des données à partir d’un tableau. Il est effectué avec l’opérateur JMESPath `[?...]`.
Cet opérateur utilise un prédicat en tant que contenus. Un prédicat est une instruction qui peut être évaluée avec les valeurs `true` ou `false`. Les expressions dans lesquelles la valeur d’évaluation du prédicat est `true` sont incluses dans la sortie.

JMESPath propose la comparaison standard et des opérateurs logiques. Ces derniers comprennent `<`, `<=`, `>`, `>=`, `==` et `!=`.
JMESPath prend également en charge les opérateurs logiques Et (`&&`), Ou (`||`) et Non (`!`). Les expressions peuvent être regroupées dans des parenthèses, ce qui permet d’obtenir des expressions de prédicat plus complexes. Pour plus d’informations sur les prédicats et les opérations logiques, consultez [JMESPath Specification](http://jmespath.org/specification.html) (Spécification JMESPath).

Dans la dernière section, nous avons aplati un tableau pour récupérer la liste complète des machines virtuelles dans un groupe de ressources. Grâce à des filtres, nous pouvons réduire cette sortie pour afficher uniquement les machines virtuelles Linux :

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
> Dans JMESPath, les chaînes sont toujours placées entre des guillemets simples (`'`). Si vous utilisez des guillemets doubles comme partie d’une chaîne dans un prédicat de filtre, vous obtiendrez une sortie vide.

JMESPath dispose également de fonctions intégrées qui peuvent simplifier le filtrage. C’est le cas de la fonction `contains(string, substring)`, qui vérifie si une chaîne contient une sous-chaîne. Les expressions étant évaluées avant d’appeler la fonction, le premier argument peut être une expression JMESPath complète. L’exemple suivant recherche toutes les machines virtuelles utilisant un stockage SSD pour leur disque de système d’exploitation :

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

Cette requête est un peu longue. La clé `storageProfile.osDisk.managedDisk.storageAccountType` est mentionnée à deux reprises, puis récréée dans la sortie. Pour raccourcir ce processus, vous pouvez appliquer le filtre après la mise à plat et la sélection des données.

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

Pour les tableaux volumineux, il peut être plus rapide d’appliquer le filtre avant de sélectionner des données.

Consultez [JMESPath specification - Built-in Functions](http://jmespath.org/specification.html#built-in-functions) (Spécification JMESPath - Fonctions intégrées) pour obtenir la liste complète des fonctions.

## <a name="change-output"></a>Modifier la sortie

Les fonctions JMESPath jouent également un autre rôle, celui d’agir sur les résultats d’une requête. Toutes les fonctions qui renvoient une valeur non booléenne modifient le résultat d’une expression.
Par exemple, vous pouvez trier des données par valeur de propriété avec `sort_by(array, &sort_expression)`. JMESPath utilise un opérateur spécial, `&`, pour les expressions qui doivent être évaluées ultérieurement dans le cadre d’une fonction. L’exemple suivant montre comment trier une liste de machines virtuelles par taille de disque de système d’exploitation :

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

Consultez [JMESPath specification - Built-in Functions](http://jmespath.org/specification.html#built-in-functions) (Spécification JMESPath - Fonctions intégrées) pour obtenir la liste complète des fonctions.

## <a name="experiment-with-queries-interactively"></a>Essayer des requêtes de façon interactive

Pour commencer à expérimenter JMESPath, le package Python [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal) propose un environnement interactif permettant d’utiliser des requêtes. Les données sont transmises en tant qu’entrées, puis les requêtes sont écrites et exécutées dans l’éditeur.

```bash
pip install jmespath-terminal
az vm list --output json | jpterm
```
