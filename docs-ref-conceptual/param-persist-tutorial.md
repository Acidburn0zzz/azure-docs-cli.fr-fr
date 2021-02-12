---
title: Tutoriel sur l’utilisation de paramètres persistants avec Azure CLI
description: Tutoriel sur l’utilisation de la commande az config param-persist pour stocker les valeurs de paramètres Azure CLI en vue d’une utilisation répétée
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.prod: azure
ms.date: 11/25/2020
ms.topic: conceptual
ms.devlang: azurecli
ms.technology: azure-cli
ms.custom: devex-track-azurecli
ms.openlocfilehash: 75833b18da0aea04dfc2aa33d9d7d18910525e98
ms.sourcegitcommit: 4c41593455b473c796735c73590403d9b6be87a2
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/05/2021
ms.locfileid: "99572780"
---
# <a name="tutorial-use-persisted-parameters-to-simplify-sequential-azure-cli-commands"></a>Tutoriel : Utiliser des paramètres persistants pour simplifier les commandes Azure CLI séquentielles

Azure CLI offre des paramètres persistants qui vous permettent de stocker les valeurs de paramètres en vue d’une utilisation continue.  Dans ce tutoriel, vous allez apprendre à vous servir de valeurs persistantes et à utiliser ces valeurs locales pour exécuter efficacement des commandes séquentielles.

Ce didacticiel vous apprendra à effectuer les opérations suivantes :

> [!div class="checklist"]
> * Utiliser des commandes de référence `az config param-persist`
> * Exécuter des commandes séquentielles à l’aide de paramètres persistants

Ce tutoriel utilise les commandes Azure CLI suivantes :

- [az config param-persist delete](/cli/azure/config/param-persist#az_config_param_persist_delete)
- [az config param-persist off](/cli/azure/config/param-persist#az_config_param_persist_off)
- [az config param-persist on](/cli/azure/config/param-persist#az_config_param_persist_on)
- [az config param-persist show](/cli/azure/config/param-persist#az_config_param_persist_show)
- [az function app create](/cli/azure/functionapp#az_functionapp_create)
- [az group create](/cli/azure/group#az_group_create)
- [az storage account create](/cli/azure/storage/account#az_storage_account_create)


Si vous n’avez pas d’abonnement Azure, créez un [compte gratuit](https://azure.microsoft.com/free/?WT.mc_id=A261C142F) avant de commencer.

## <a name="prerequisites"></a>Prérequis

1. [Installer l’interface de ligne de commande Microsoft Azure](install-azure-cli.md)

   Si vous préférez, vous pouvez également utiliser Azure Cloud Shell pour effectuer les étapes décrites dans ce didacticiel.  Azure Cloud Shell est un environnement d’interpréteur de commandes interactif que vous utilisez dans votre navigateur.  Démarrez Cloud Shell à l’aide de l’une des méthodes suivantes :

   - Ouvrez Cloud Shell en accédant à [https://shell.azure.com](https://shell.azure.com).

   - Sélectionnez le bouton **Cloud Shell** dans la barre de menus en haut à droite du [portail Azure](https://portal.azure.com).

1. Si vous utilisez une installation locale d’Azure CLI, effectuez les étapes suivantes :
   - Connectez-vous à l’aide de la commande [az login](/cli/azure/reference-index#az-login), puis suivez les étapes affichées dans votre terminal pour effectuer le processus d’authentification.

     ```azurecli
     az login
     ```
    - Ce tutoriel nécessite Azure CLI version 2.12.0 ou ultérieure.  Exécutez [az version](/cli/azure/reference-index#az_version) pour rechercher la version et les bibliothèques dépendantes installées. Pour effectuer une mise à niveau vers la dernière version, exécutez [az upgrade](/cli/azure/reference-index#az_upgrade).

## <a name="1-determine-your-local-directory"></a>1. Déterminer votre répertoire local

Les valeurs de paramètres persistants sont stockées dans le répertoire de travail du compte de stockage Azure utilisé par Azure Cloud Shell.  Si vous utilisez une installation locale d’Azure CLI, les valeurs sont stockées dans le répertoire de travail sur votre ordinateur.

Pour rechercher, créer ou changer le répertoire de travail utilisé par Azure CLI, utilisez ces commandes CLI bien connues.

```azurecli
# List directories
dir

# Make directory
mkdir azCLI

# Change directory
cd azCLI
```

## <a name="2-turn-on-persisted-parameters"></a>2. Activer les paramètres persistants

Vous devez activer les [paramètres persistants](/cli/azure/param-persist) pour pouvoir stocker les valeurs de paramètres.  Un avertissement s’affiche tant que `az config param-persist` est en phase expérimentale.  Consultez [Vue d’ensemble : Types et état de référence Azure CLI](/cli/azure/reference-types-and-status) pour en savoir plus sur les types de référence, états et niveaux de prise en charge Azure CLI.

```azurecli
az config param-persist on
```

## <a name="3-create-persisted-parameters"></a>3. Créer des paramètres persistants

Pour stocker les valeurs de paramètres persistants, exécutez une commande Azure CLI de votre choix qui contient les paramètres à stocker.  Par exemple, si vous créez un groupe de ressources, les paramètres `--location` et `--name` sont stockés en vue d’une utilisation ultérieure.

1. Stockez l’emplacement (location) et le nom du groupe de ressources (name).
   ```azurecli
   # With persisted parameters turned on, create a resource group
   az group create --name RG1forTutorial --location eastus2

   # See new persisted parameters
   az config param-persist show
   ```

   ```output
   {
     "all": {
       "location": "eastus2",
       "resource_group_name": "RG1forTutorial"
     }
   }
   ```

1. À l’aide des nouveaux paramètres persistants, créez un compte de stockage.

   ```azurecli
   # Create a storage account
   az storage account create --name sa1fortutorial

   # See that storage_account_name has been added to persisted parameters
   az config param-persist show
   ```

   ```output
   {
     "all": {
       "location": "eastus2",
       "resource_group_name": "RG1forTutorial",
       "storage_account_name": "sa1fortutorial"
     }
   }
   ```

1. Créez un paramètre persistant sans définir de nouvelle ressource.

   Si vous ne souhaitez pas définir une nouvelle ressource Azure, les paramètres `resource_group_name` et `location` peuvent être stockés à l’aide de commandes non-create comme `show` ou `list`.   Pour obtenir la liste complète des paramètres pris en charge et l’action nécessaire pour conserver les valeurs, consultez [Paramètres persistants dans Azure CLI](/cli/azure/param-persist-howto#compare-parameter-persistence-and-global-variables).  Cet exemple supprime également toutes les valeurs des paramètres à l’aide de la commande [az config param-persist delete](/cli/azure/config/param-persist#az-param-persist-delete).

   ```azurecli
   # Clear all persisted parameters for demonstration.
   az config param-persist delete --all

   # List all storage accounts which will create the `resource_group_name` stored parameter value.
   az storage account show --resource-group RG1forTutorial --name sa1fortutorial

   # See the new stored value created for resource group.  The storage account name is only stored with a 'create' command.
   az config param-persist show
   ```

   ```output
   {
     "all": {
       "resource_group_name": "RG1forTutorial"
     }
   }
   ```

## <a name="4-replace-persisted-parameters"></a>4. Remplacer des paramètres persistants

Pour remplacer une valeur de paramètre stockée, il suffit d’exécuter une commande contenant une valeur différente.

1. Définissez de nouveaux paramètres persistants.
   ```azurecli
   # Clear all persisted parameters for demonstration
   az config param-persist delete --all

   # Create a storage account placing "location", "resource_group_name", and "storage_account_name" into persisted parameters
   az storage account create --name sa1fortutorial --resource-group RG1forTutorial --location eastus2

   # See persisted parameters entries
   az config param-persist show
   ```

   ```output
   {
     "all": {
       "location": "eastus2",
       "resource_group_name": "RG1forTutorial",
       "storage_account_name": "sa1fortutorial"
     }
   }
   ```

1. Remplacez les valeurs nouvellement stockées.

   ```azurecli
   # Create a second storage account while changing both the "storage_account_name" and "location" persisted parameters
   az storage account create --name sa2fortutorial --location westeurope

   # See new persisted parameters
   az config param-persist show
   ```

   ```output
   {
     "all": {
       "location": "westeurope",
       "resource_group_name": "RG1forTutorial",
       "storage_account_name": "sa2fortutorial"
     }
   }
   ```

   > [!NOTE]
   >
   > Même si les paramètres persistants sont activés, vous n’êtes pas obligé de les utiliser.  Vous pouvez toujours exécuter des commandes en spécifiant toutes les valeurs des paramètres.  Toutefois, sachez que lorsque les paramètres persistants sont activés, _vous créez des paramètres persistants ou remplacez des paramètres persistants existants_.

## <a name="5-execute-sequential-commands"></a>5. Exécuter des commandes séquentielles

Ces scripts créent une application de fonction Azure à l’aide du plan Consommation.

### <a name="using-persisted-parameters"></a>[Utilisation de paramètres persistants](#tab/azure-cli)

```azurecli
# Reminder: function app and storage account names must be unique.

# Turn persisted parameters on.
az config param-persist on

# Create a resource group.
az group create --name RG2forTutorial --location westeurope

# Create an Azure storage account in the resource group omitting "--location" and "--resource-group" parameters.
az storage account create \
  --name sa3fortutorial \
  --sku Standard_LRS

# Create a serverless function app in the resource group omitting "--storage-account" and "--resource-group" parameters.
az functionapp create \
  --name FAforTutorial \
  --consumption-plan-location westeurope \
  --functions-version 2

# See the stored parameter values.
az config param-persist show
```

### <a name="without-persisted-parameters"></a>[Sans paramètres persistants](#tab/azure-portal)

```azurecli
# Reminder: function app and storage account names must be unique.

# turn persisted parameters off
az config param-persist off

# Create a resource group.
az group create --name RG2forTutorial --location westeurope

# Create an Azure storage account in the resource group.
az storage account create \
  --name sa3fortutorial \
  --location westeurope \
  --resource-group RG2forTutorial \
  --sku Standard_LRS

# Create a serverless function app in the resource group.
az functionapp create \
  --name FAforTutorial \
  --storage-account sa3fortutorial \
  --consumption-plan-location westeurope \
  --resource-group RG2forTutorial \
  --functions-version 2
```

* * *

## <a name="6-delete-persisted-parameters"></a>6. Supprimer des paramètres persistants

Utilisez la commande [az config param-persist delete](/cli/azure/param-persist#az-param-persist-delete) pour supprimer des entrées.

```azurecli
# Remove a single persisted parameters entry by specifying the name, not the value
az config param-persist delete resource_group_name

# Remove all persisted parameters entries and do not prompt for confirmation
az config param-persist delete --all --yes
```

> [!IMPORTANT]
>
> Les paramètres persistants ne sont pas mis à jour quand une ressource Azure est supprimée.
>
> ```azurecli
> # delete a resource group
> az group delete --name RG1forTutorial
>
> # verify that the resource group no longer exists
> az group list --output table
>
> # See that the resource group name remains in persisted parameters
> az config param-persist show
> ```

## <a name="7-turn-persisted-parameters-off"></a>7. Désactiver les paramètres persistants

Vous pouvez désactiver les paramètres persistants à l’aide de la commande [az config param-persist off](/cli/azure/param-persist#az-param-persist-off), mais les données enregistrées des paramètres persistants ne sont pas supprimées.

```azurecli
# Turn persisted parameters off
az config param-persist off

# See that your persisted parameters still exist
az config param-persist show

# Try to create a new resource relying on persisted parameters and receive error "...the following arguments are required:..."
az storage account create --name SA4inAzCLI --sku Standard_LRS
```

## <a name="8-clean-up-resources"></a>8. Nettoyer les ressources

Quand vous n’avez plus besoin du groupe de ressources, utilisez la commande [az group delete](/cli/azure/group) pour supprimer celui-ci ainsi que toutes les ressources associées.

```azurecli
az group delete --name RG1forTutorial
```

## <a name="see-also"></a>Voir aussi

- [Comment utiliser des paramètres persistants Azure CLI](param-persist-howto.md)
- [Configuration d’Azure CLI avec az configure](/cli/azure/azure-cli-configuration)
