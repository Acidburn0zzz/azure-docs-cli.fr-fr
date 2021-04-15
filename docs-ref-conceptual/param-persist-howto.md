---
title: Options des paramètres persistants Azure CLI
description: Comment utiliser des paramètres persistants Azure CLI pour stocker des valeurs de paramètre réutilisables
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.prod: azure
ms.date: 10/30/2020
ms.topic: conceptual
ms.devlang: azurecli
ms.technology: azure-cli
ms.custom: devx-track-azurecli
ms.openlocfilehash: 32d9435447c4cdcd5a0c7148b8ed02729cbe9088
ms.sourcegitcommit: bff138c7d3cd3ce8c90c5809b0e812be71959504
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/14/2021
ms.locfileid: "107385771"
---
# <a name="azure-cli-persisted-parameter"></a>Paramètre persistant Azure CLI

La référence Azure CLI [az config param-persist](/cli/azure/config/param-persist) permet de conserver les valeurs de paramètres persistants en local pour des commandes Azure CLI.  Cela évite de devoir retaper continuellement des paramètres couramment utilisés. Par exemple, les paramètres location et resource-group sont obligatoires dans de nombreuses commandes CLI, mais ils ne contribuent pas à l’_intention_ de la commande.  Quand vous stockez les valeurs de paramètres persistants, vous réduisez la redondance et pouvez écourter considérablement la syntaxe des commandes CLI.

Les valeurs de configuration utilisées par l’interface CLI sont évaluées dans l’ordre suivant. Les éléments situés en haut de la liste sont prioritaires.

1. Paramètres de ligne de commande
1. Valeurs dans le répertoire de travail local définies par `az config param-persist`
1. Variables d'environnement
1. Valeurs du fichier de configuration ou définies avec `az config`

[Installez Azure CLI](install-azure-cli.md) ou ouvrez [Azure Cloud Shell](https://shell.azure.com) pour exécuter les scripts de cet article.  Si vous utilisez une installation locale d’Azure CLI, la version 2.12.0 ou ultérieure est nécessaire pour exécuter les commandes `az config param-persist`.  Exécutez [az version](/cli/azure/reference-index#az_version) pour rechercher la version et les bibliothèques dépendantes installées. Pour effectuer une mise à niveau vers la dernière version, exécutez [az upgrade](/cli/azure/reference-index#az_upgrade).  Azure Cloud Shell dispose toujours de la dernière version d’Azure CLI.

## <a name="persisted-parameter-data-file"></a>Fichier de données des paramètres persistants

Les valeurs des paramètres persistants sont conservées dans un fichier nommé `.param_persist` qui est stocké dans votre répertoire de travail.  Si vous utilisez [Azure Cloud Shell](https://shell.azure.com) pour exécuter des commandes Azure CLI, votre répertoire de travail se trouve dans le compte de stockage utilisé par Azure CLI.  Si vous utilisez une [installation locale](install-azure-cli.md) d’Azure CLI, votre répertoire de travail se trouve sur votre ordinateur local.  Dans les deux cas, le fichier `.param_persist` est masqué et ne doit pas être mis à jour manuellement.

## <a name="persisted-parameter-storage-and-support"></a>Stockage et prise en charge des paramètres persistants

Les paramètres Azure CLI suivants sont pris en charge par le paramètre persistant.  Les paramètres `resource_group_name` et `location` sont stockés différemment, ce qui vous permet de les ajouter au paramètre persistant _sans_ exécuter de commande create.

| Paramètre persistant | Action de stockage | Pris en charge par
|-|-|-|
| location | Exécuter n’importe quelle commande | Toutes les références Azure CLI
| resource_group_name | Exécuter n’importe quelle commande | Toutes les références Azure CLI
| vnet_name | Exécuter une commande create | Azure Web Apps uniquement
| storage_account_name | Exécuter une commande create |  Azure Web Apps uniquement
| webapp_name | Exécuter une commande create | Azure Web Apps uniquement
| function_app_name | Exécuter une commande create | Azure Functions uniquement

## <a name="sample-script-using-persisted-parameters"></a>Exemple de script utilisant des paramètres persistants

Sans paramètres persistants, les commandes CLI séquentielles doivent répéter les mêmes valeurs de paramètres.  Quand les paramètres persistants sont activés, les valeurs stockées de vos paramètres peuvent être omises des commandes séquentielles.  Dans cet exemple, l’`location`, le `resource group name` et le `storage account name` sont répétés dans les commandes suivantes.

```azurecli
# Reminder: function app and storage account names must be unique.

# turn persisted parameters on
az config param-persist on

# Create a resource group which will store "resource group" and "location" in persisted parameter.
az group create --name RGlocalContext --location westeurope

# Create an Azure storage account omitting location and resource group.
az storage account create \
  --name sa1localcontext \
  --sku Standard_LRS

# Create a serverless function app in the resource group omitting storage account and resource group.
az functionapp create \
  --name FAlocalContext \
  --consumption-plan-location westeurope \
  --functions-version 2

# See the stored parameter values
az config param-persist show
```

## <a name="persisted-parameter-and-global-variable-comparison"></a>Comparaison des paramètres persistants et des variables globales

Deux commandes Azure CLI peuvent être utilisées pour définir les valeurs par défaut de paramètres : `az configure` et `az config param-persist`.  Utilisez la commande `az configure` pour spécifier des _variables globales_ telles que le groupe, l’emplacement ou le web.  Utilisez `az param-persist` pour spécifier des _valeurs locales par défaut_ propres à votre charge de travail.  Les valeurs stockées sont utilisées par CLI à la place des arguments obligatoires.

> [!Important]
> Les paramètres persistants remplacent les valeurs de contexte globales.
>

| Informations de référence | Étendue | Définissez | Utilisation
|-|-|-|-|
[az configure](/cli/azure/reference-index#az_configure) | Étendue globale à l’échelle de CLI | Définition explicite avec `az configure --defaults` | Utilisation avec des paramètres liés à la journalisation, la collecte de données et les valeurs d’argument par défaut.
[az config param-persist](/cli/azure/config/param-persist) | Étendue locale à l’échelle d’un répertoire de travail spécifique | Définition automatique une fois les paramètres persistants activés | Utilisation pour des commandes séquentielles de charges de travail individuelles.

### <a name="command-examples"></a>Exemples de commandes

Utilisez `az config param-persist` pour définir une variable globale utilisée dans le cadre de la création d’un compte de stockage Azure.

```azurecli
# set the global variable for resource group
az configure --defaults group=myGlobalVariableRG

# Create an Azure storage account omitting the resource group relying on the global variable value
# Substitute the storage account name parameter with a unique value
az storage account create \
  --name mystorageaccount1 \
  --location westeurope \
  --sku Standard_LRS
```

La sortie de la commande CLI montre qu’un compte de stockage a été créé dans le groupe de ressources trouvé dans la variable globale « myGlobalVariableRG ».

```output
...
},
  "primaryLocation": "westeurope",
  "privateEndpointConnections": [],
  "provisioningState": "Succeeded",
  "resourceGroup": "myGlobalVariableRG",
  "routingPreference": null,
  "secondaryEndpoints": null,
  "secondaryLocation": null,
  "sku": {
    "name": "Standard_LRS",
    "tier": "Standard"
},
...
```

Utilisez `az config param-persist` pour définir les paramètres persistants utilisés dans le cadre de la création d’un compte de stockage Azure.  Si une variable globale est définie pour le même objet, le paramètre persistant remplace la variable globale.

```azurecli
# turn persisted parameter on
az config param-persist on

# Create a resource group in order to write to persisted parameter
az group create --name myParamPersistRG --location westeurope

# Create an Azure storage account omitting the resource group relying on the persisted parameter value
# Substitute the storage account name parameter with a unique value
az storage account create \
  --name mystorageaccount2 \
  --location westeurope \
  --sku Standard_LRS
```

Même avec une variable globale définie pour un groupe de ressources avec la valeur `myGlobalVariableRG`, le compte de stockage est créé avec `myParamPersistRG` si les paramètres persistants sont activés.

```output
...
},
  "primaryLocation": "westeurope",
  "privateEndpointConnections": [],
  "provisioningState": "Succeeded",
  "resourceGroup": "myParamPersistRG",
  "routingPreference": null,
  "secondaryEndpoints": null,
  "secondaryLocation": null,
  "sku": {
    "name": "Standard_LRS",
    "tier": "Standard"
},
...
```

## <a name="see-also"></a>Voir aussi

* [Tutoriel : Utiliser des paramètres persistants avec des commandes Azure CLI séquentielles](param-persist-tutorial.md)
* [Configuration d’Azure CLI avec az configure](azure-cli-configuration.md)
