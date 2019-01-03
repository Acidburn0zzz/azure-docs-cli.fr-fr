---
title: Extension d’alias d’Azure CLI
description: Comment utiliser l’extension d’alias d’Azure CLI
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/07/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 3cd812a0e0e61d50883ca9efd762d6fc05617b76
ms.sourcegitcommit: f40bd067ece4e6ec13e259782ed8db3e33b61a75
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/18/2018
ms.locfileid: "53593572"
---
# <a name="the-azure-cli-alias-extension"></a>L’extension d’alias d’Azure CLI

L’extension d’alias permet aux utilisateurs de définir des commandes personnalisées pour l’interface Azure CLI, à l’aide des commandes existantes. Les alias aident à garantir une simplicité dans votre flux de travail en y autorisant les raccourcis. Comme les alias sont alimentés par le moteur de modèles Jinja2, ils prennent bien souvent en charge le traitement avancé des arguments.

> [!NOTE]
> L’extension d’alias est en préversion publique. Les fonctionnalités et le format du fichier de configuration peuvent changer.

## <a name="install-the-alias-extension"></a>Installer l’extension d’alias

La version minimale requise de l’interface Azure CLI pour utiliser l’extension d’alias est **2.0.28**. Pour vérifier votre version de l’interface CLI, exécutez `az --version`. Si vous devez mettre à jour votre installation, suivez les instructions de la section [Installer Azure CLI](./install-azure-cli.md).

Installez l’extension avec la commande [az extension add](/cli/azure/extension#az-extension-add).

```azurecli-interactive
az extension add --name alias
```

Vérifiez l’installation de l’extension avec [az extension list](/cli/azure/extension#az-extension-list). Si l’extension d’alias a été correctement installée, elle est répertoriée dans la sortie de la commande.

```azurecli-interactive
az extension list --output table --query '[].{Name:name}'
```

```output
Name
------
alias
```

## <a name="keep-the-extension-up-to-date"></a>Maintenez l’extension à jour

L’extension d’alias est en cours de développement actif ; de nouvelles versions sont régulièrement publiées. Les nouvelles versions ne sont pas installées lorsque vous mettez à jour l’interface CLI. Installez les mises à jour de l’extension avec [az extension update](/cli/azure/extension#az-extension-update).

```azurecli-interactive
az extension update --name alias
```

## <a name="manage-aliases-for-the-azure-cli"></a>Gestion des alias pour Azure CLI

L’extension d’alias vous permet de créer et de gérer les alias pour d’autres commandes CLI. Pour afficher toutes les commandes disponibles et les détails de paramètres, exécutez la commande de l’alias avec `--help`.

```azurecli-interactive
az alias --help
```

## <a name="create-simple-alias-commands"></a>Créer des commandes alias simples

Les alias peuvent par exemple servir à raccourcir les noms existants des groupes de commandes ou des commandes. Par exemple, vous pouvez raccourcir le nom du groupe de commandes `group` en le ramenant à `rg` et le nom de la commande `list` en `ls`.

```azurecli-interactive
az alias create --name rg --command group
az alias create --name ls --command list
```

Ces alias nouvellement définis peuvent désormais être utilisés dans l’ensemble des emplacements pouvant héberger leur définition.

```azurecli-interactive
az rg list
az rg ls
az vm ls
```

N’incluez pas `az` dans la commande.

Les alias peuvent également être des raccourcis de commandes complètes. Le prochain exemple répertorie les groupes de ressources disponibles et leur emplacement dans la sortie de table :

```azurecli-interactive
az alias create --name ls-groups --command "group list --query '[].{Name:name, Location:location}' --output table"
```

Désormais, `ls-groups` peut être exécutée comme toute autre commande CLI.

```azurecli-interactive
az ls-groups
```

## <a name="create-an-alias-command-with-arguments"></a>Créer une commande d’alias avec des arguments

Il est également possible d’ajouter des arguments positionnels à une commande d’alias en les incluant en tant que `{{ arg_name }}` dans le nom d’alias. L’espace à l’intérieur des accolades est requis.

```azurecli-interactive
az alias create --name "alias_name {{ arg1 }} {{ arg2 }} ..." --command "invoke_including_args"
```

Le prochain exemple d’alias indique comment utiliser des arguments positionnels afin de récupérer l’adresse IP publique d’une machine virtuelle.

```azurecli-interactive
az alias create \
    --name "get-vm-ip {{ resourceGroup }} {{ vmName }}" \
    --command "vm list-ip-addresses --resource-group {{ resourceGroup }} --name {{ vmName }}
        --query [0].virtualMachine.network.publicIpAddresses[0].ipAddress"
```

Lorsque vous exécutez cette commande, vous octroyez des valeurs aux arguments positionnels.

```azurecli-interactive
az get-vm-ip MyResourceGroup MyVM
```

Vous pouvez également utiliser des variables d’environnement dans les commandes alias, qui sont évaluées au moment de l’exécution. Le prochain exemple ajoute l’alias `create-rg`, qui crée un groupe de ressources dans `eastus` et ajoute une balise `owner`. Cette balise se voit affecter la valeur de la variable d’environnement local `USER`.

```azurecli-interactive
az alias create \
    --name "create-rg {{ groupName }}" \
    --command "group create --name {{ groupName }} --location eastus --tags owner=\$USER"
```

Pour enregistrer les variables d’environnement à l’intérieur de la commande de l’alias, le signe dollar `$` doit être placé dans une séquence d’échappement.

## <a name="process-arguments-using-jinja2-templates"></a>Traiter les arguments à l’aide des modèles Jinja2

La substitution d’argument dans l’extension d’alias est effectuée par [Jinja2](http://jinja.pocoo.org/docs/2.10/). Les modèles Jinja2 permettent de manipuler les arguments.

Avec les modèles Jinja2, vous pouvez écrire des alias qui acceptent des types d’arguments supplémentaires par rapport à la commande sous-jacente. Par exemple, vous pouvez développer un alias acceptant une URL de stockage. Par la suite, cette URL est analysée afin de transmettre les noms de compte et de conteneur à la commande de stockage.

```azurecli-interactive
az alias create \
    --name 'storage-ls {{ url }}' \
    --command "storage blob list
        --account-name {{ url.replace('https://', '').split('.')[0] }}
        --container-name {{ url.replace('https://', '').split('/')[1] }}"
```

Pour en savoir plus sur le moteur de modèles Jinja2, consultez la [documentation Jinja2](http://jinja.pocoo.org/docs/2.10/templates/).

## <a name="alias-configuration-file"></a>Fichier de configuration d’alias

Une autre façon de créer et de modifier des alias est de modifier le fichier de configuration d’alias. Les définitions des commandes alias sont consignées dans un fichier de configuration, qui se situe sur `$AZURE_USER_CONFIG/alias`. La valeur par défaut de `AZURE_USER_CONFIG` est `$HOME/.azure` sous macOS et Linux, et `%USERPROFILE%\.azure` sous Windows. Le fichier de configuration d’alias est consigné au format du fichier de configuration INI. Le format des commandes alias est le suivant :

```ini
[alias_name]
command = invoked_commands
```

Pour les alias qui possèdent des arguments de position, le format des commandes alias est :

```ini
[alias_name {{ arg1 }} {{ arg2 }} ...]
command = invoked_commands_including_args
```

## <a name="create-an-alias-command-with-arguments-via-the-alias-configuration-file"></a>Créer une commande alias avec des arguments via le fichier de configuration d’alias

L’exemple suivant illustre un alias pour une commande avec des arguments. Cette commande obtient l’adresse IP publique pour une machine virtuelle. Les commandes d’un alias doivent toutes se trouver sur une seule ligne et utiliser tous les arguments dans le nom d’alias.

```ini
[get-vm-ip {{ resourceGroup }} {{ vmName }}]
command = vm list-ip-addresses --resource-group {{ resourceGroup }} --name {{ vmName }} --query [0].virtualMachine.network.publicIpAddresses[0].ipAddress
```

## <a name="uninstall-the-alias-extension"></a>Désinstaller l’extension d’alias

Pour désinstaller l’extension, utilisez la commande [az extension remove](/cli/azure/extension#az-extension-remove).

```azurecli-interactive
az extension remove --name alias
```

Si vous avez procédé à la désinstallation en raison d’un bogue ou d’un problème lié à l’extension, veuillez [signaler un incident GitHub](https://github.com/Azure/azure-cli-extensions/issues) afin que nous puissions réfléchir à la correction.
