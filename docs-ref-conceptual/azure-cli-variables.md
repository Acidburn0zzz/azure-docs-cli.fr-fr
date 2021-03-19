---
title: Spécification de valeurs dans les commandes Azure CLI
description: Découvrez comment passer des valeurs aux commandes Azure CLI, notamment des variables, et comment réutiliser des valeurs courantes.
author: dbradish-microsoft
ms.author: dbradish
ms.service: azure-cli
ms.topic: how-to
ms.date: 03/01/2021
ms.custom: template-how-to
ms.openlocfilehash: 18bd938403d18a14278a7b8a97ca93bc0e0d0f1c
ms.sourcegitcommit: f9e23f29c59c6957d3df4d5ca2f4425093e6fd80
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/16/2021
ms.locfileid: "103554912"
---
# <a name="specifying-values-in-azure-cli-commands"></a>Spécification de valeurs dans les commandes Azure CLI

En plus de spécifier des valeurs directement dans une commande, vous pouvez recourir à diverses méthodes pour fournir des valeurs :

* Utiliser des variables shell
* Définir un abonnement à utiliser dans plusieurs commandes
* Créer des valeurs par défaut pour certains paramètres
* Utiliser des valeurs persistantes pour certains paramètres

Cet article décrit différentes façons de spécifier des valeurs dans les commandes Azure CLI.

[!INCLUDE [azure-cli-prepare-your-environment.md](includes/azure-cli-prepare-your-environment.md)]

## <a name="use-shell-variables"></a>Utiliser des variables shell

Azure CLI s’exécute dans un interpréteur de commandes (shell). Cet article utilise Bash. Pour plus d’informations sur les autres shells, consultez [Utiliser Azure CLI efficacement](/cli/azure/use-cli-effectively). Vous pouvez utiliser des variables dans Bash pour passer des valeurs de paramètres à des commandes. Les variables permettent également de réutiliser des commandes (fragmentaires ou dans des scripts).

Cet exemple crée un disque de stockage du même type que celui d’une machine virtuelle existante.

```azurecli
# Assign values to variables
MyResourceGroup=ContosoRGforVM
MySubscription="Contoso subscription"
vmName=VM01

# Get a value for a variable based on an existing virtual machine
osType=$(az vm get-instance-view --resource-group $MyResourceGroup \
   --name $vmName --subscription "$MySubscription" \
   --query 'storageProfile.osDisk.osType' --output tsv)

# Create a disk of the same type by using the variable value
az disk create --resource-group $MyResourceGroup --name DestinationDisk --size-gb 20 --os-type $osType
```

Cet exemple affecte des valeurs à des variables qui sont réutilisées, comme **MyResourceGroup**. Une commande obtient une valeur à affecter à **osType**.

Quand vous affectez une valeur à une variable à partir d’une autre commande, vérifiez que la commande utilise un format de sortie compatible. La commande [az vm get-instance-view](/cli/azure/vm#az_vm_get_instance_view) utilise le format de sortie `tsv`. Cette option retourne des valeurs sans mise en forme, clé ou autre symbole supplémentaire. Certains formats de sortie incluent des structures ou des caractères comme des guillemets. Pour plus d’informations, consultez [Formats de sortie pour les commandes Azure CLI](/cli/azure/format-output-azure-cli).

Dans cet exemple, la variable **MySubscription** doit être entre guillemets. Sa valeur contient des espaces que la commande ne peut pas analyser. Si vous travaillez uniquement avec des ID d’abonnement, vous n’avez pas besoin d’utiliser des guillemets.

## <a name="set-a-subscription"></a>Définir un abonnement

De nombreuses commandes nécessitent un abonnement spécifique. Les ressources Azure existent dans des groupes de ressources, lesquels existent dans des abonnements. Azure CLI utilise un abonnement par défaut quand vous êtes dans une session. Pour voir la valeur de votre abonnement actif, exécutez la commande [az account show](/cli/azure/account#az_account_show) :

```azurecli
az account show --output table
```

Il est possible que vous n’ayez accès qu’à un seul abonnement. Pour plus d’informations, consultez [Utiliser des abonnements Azure avec Azure CLI](/cli/azure/manage-azure-subscriptions-azure-cli). Vous pouvez utiliser la commande [az account set](/cli/azure/account#az-account-set) pour définir votre abonnement actif :

```azurecli
az account set --subscription "My Demos"
```

Après avoir défini votre abonnement, vous pouvez omettre le paramètre `--Subscription`. Pour plus d’informations, consultez [Utiliser des abonnements Azure avec Azure CLI](manage-azure-subscriptions-azure-cli.md).

## <a name="create-default-values"></a>Créer des valeurs par défaut

Vous pouvez définir des valeurs pour certains paramètres en utilisant la commande [az config set](/cli/azure/config#az_config_set). Cet exemple définit un groupe de ressources par défaut :

```azurecli
az config set defaults.group=ContosoRGforVM
```

Après avoir exécuté cette commande, exécutez celle-ci pour créer un compte de stockage dans le groupe de ressources ContosoRGforVM :

```azurecli
az storage account create --name storage135 --location eastus --sku Standard_LRS
```

Notez qu’aucun groupe de ressources n’est spécifié dans la commande. Pour plus d’informations, consultez [Définir un groupe de ressources par défaut](manage-azure-groups-azure-cli.md#set-a-default-resource-group).

> [!TIP]
> Les commandes qui obtiennent les valeurs de paramètres de différentes manières peuvent prêter à confusion. Si une commande donne un résultat inattendu, comme l’impossibilité de trouver un groupe de ressources, il peut y avoir une valeur par défaut.
>
> Si vous rencontrez une erreur, réexécutez la commande avec le paramètre et la valeur spécifiés. Une valeur explicite pour un paramètre est toujours prioritaire sur les autres options.

Vous pouvez spécifier des valeurs pour plusieurs paramètres de cette façon. Pour plus d’informations, consultez [Configuration d’Azure CLI](azure-cli-configuration.md).

## <a name="use-persistent-values"></a>Utiliser des valeurs persistantes

Les valeurs persistantes vous permettent de spécifier une valeur de paramètre une seule fois. Si vous effectuez plusieurs actions associées dans un groupe de ressources, vous n’êtes pas obligé de spécifier ce groupe à plusieurs reprises.

Exécutez cette commande pour rendre une valeur de paramètre persistante :

```azurecli
az config param-persist on
```

Une fois la persistance activée, créez un groupe de ressources :

 ```azurecli
az group create --name ContosoStorageRG --location eastus
```

Tant que la persistance est activée, vous pouvez laisser le paramètre `--resource-group` hors des commandes ultérieures. La commande suivante crée un compte de stockage dans le groupe de ressources ContosoStorageRG :

```azurecli
az storage account create --name storage135 --location eastus --sku Standard_LRS
```

Pour plus d’informations, consultez [Paramètre persistant Azure CLI](/cli/azure/param-persist-howto).

## <a name="clean-up-resources"></a>Nettoyer les ressources

Si vous avez créé des ressources pour essayer l’une des commandes de cet article, vous pouvez les supprimer en utilisant la commande [az group delete](/cli/azure/group#az_group_delete) :

```azurecli
az group delete --name ContosoRGforVM
az group delete --name ContosoStorageRG
```

Cette commande supprime le groupe et toutes les ressources qu’il contient en une seule opération.

Vous pouvez supprimer les paramètres persistants en exécutant la commande [az config param-persist delete](/cli/azure/config/param-persist#az_config_param_persist_delete) :

```azurecli
az config param-persist delete --all
```

## <a name="next-steps"></a>Étapes suivantes

* [Paramètre persistant Azure CLI](param-persist-howto.md)
* [Utilisation de groupes de ressources dans Azure CLI](manage-azure-groups-azure-cli.md)
* [Créer une demande de support Azure dans Azure CLI](azure-cli-support-request.md)
