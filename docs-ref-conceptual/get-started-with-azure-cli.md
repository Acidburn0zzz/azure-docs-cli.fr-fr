---
title: Prise en main d’Azure CLI
description: Commencez à utiliser Azure CLI en apprenant les commandes de base.
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 01/30/2020
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: bc9b86db6fb9c5b3731550df9dda96debcbfba9f
ms.sourcegitcommit: ee64dc738cfe689a2a479e32a87bf420f96c31c8
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/06/2020
ms.locfileid: "79990113"
---
# <a name="get-started-with-azure-cli"></a>Prise en main d’Azure CLI

Bienvenue dans Azure CLI !  Cet article présente l’interface CLI et vous permet d’effectuer des tâches courantes.

> [!NOTE]
>
> Dans les scripts et sur le site de documentation de Microsoft, les exemples Azure CLI sont écrits pour l’interpréteur de commandes `bash`. Les exemples d’une ligne seront exécutés sur n’importe quelle plateforme. Les exemples plus longs qui se répartissent sur plusieurs lignes (`\`) ou incluent l’attribution de variables doivent être modifiés pour fonctionner sur d’autres interpréteurs de commandes, y compris PowerShell.

## <a name="install-or-run-in-azure-cloud-shell"></a>Installer ou exécuter dans Azure Cloud Shell

Pour commencer avec l’interface CLI, le plus simple est de l’exécuter dans un environnement Azure Cloud Shell via votre navigateur. Pour en savoir plus sur Cloud Shell, consultez [Démarrage rapide de Bash dans Azure Cloud Shell](/azure/cloud-shell/quickstart).

Lorsque vous êtes prêt à installer l’interface CLI, consultez les [instructions d’installation](install-azure-cli.md).

Après avoir installé l’interface CLI pour la première fois, vérifiez qu’elle est bien installée et que vous disposez de la version appropriée en exécutant `az --version`.

> [!NOTE]
> Si vous utilisez le modèle de déploiement Azure CLI Classic, [installez l’interface de ligne de commande Azure CLI Classic](install-classic-cli.md).

## <a name="sign-in"></a>Se connecter

Avant d’utiliser les commandes CLI avec une installation locale, vous devez vous connecter avec la commande [az login](/cli/azure/reference-index#az-login).

[!INCLUDE [interactive-login](includes/interactive-login.md)]

Après vous être connecté, vous voyez une liste des abonnements associés à votre compte Azure. Les informations d’abonnement avec `isDefault: true` correspond à l’abonnement actuellement activé après vous être connecté. Pour sélectionner un autre abonnement, utilisez la commande [az account set](/cli/azure/account#az-account-set) avec l’ID d’abonnement auquel vous voulez passer. Pour plus d’informations sur la sélection d’abonnements, consultez [Utiliser plusieurs abonnements Azure](manage-azure-subscriptions-azure-cli.md).

Il existe des méthodes pour se connecter de manière non interactive, qui sont dévelopées en détail dans [Se connecter avec Azure CLI](authenticate-azure-cli.md).

## <a name="common-commands"></a>Commandes courantes

Ce tableau répertorie certaines commandes courantes utilisées dans l’interface CLI ainsi que des liens vers leur documentation de référence.

| Type de ressource | Groupe de commandes Azure CLI |
|---------------|-------------------------|
| [Groupe de ressources](/azure/azure-resource-manager/resource-group-overview) | [az group](/cli/azure/group) |
| [Machines virtuelles](/azure/virtual-machines) | [az vm](/cli/azure/vm) |
| [Comptes de stockage](/azure/storage/common/storage-introduction) | [az storage account](/cli/azure/storage/account) |
| [Key Vault](/azure/key-vault/key-vault-whatis) | [az keyvault](/cli/azure/keyvault) |
| [Applications web](/azure/app-service) | [az webapp](/cli/azure/webapp) |
| [Bases de données SQL](/azure/sql-database) | [az sql server](/cli/azure/sql/server) |
| [CosmosDB](/azure/cosmos-db) | [az cosmosdb](/cli/azure/cosmosdb) |

## <a name="finding-commands"></a>Recherche de commandes

Les commandes dans l’interface CLI sont classées par _commandes_ de _groupes_. Chaque groupe représente un service Azure, et les commandes agissent sur ce service.

Pour rechercher des commandes, utilisez la commande [az find](/cli/azure/reference-index#az-find). Par exemple, pour rechercher des noms de commandes contenant `secret`, utilisez la commande suivante :

```azurecli-interactive
az find secret
```

Utilisez l’argument `--help` pour obtenir une liste complète des commandes et des sous-groupes d’un groupe. Par exemple, pour trouver les commandes CLI pour fonctionner avec des groupes de sécurité réseau (NSG) :

```azurecli-interactive
az network nsg --help
```

L’interface CLI dispose de la saisie semi-automatique via la touche Tab pour les commandes de l’interpréteur de commandes bash.

## <a name="globally-available-arguments"></a>Arguments globalement disponibles

Certains arguments sont disponibles pour chaque commande.

* `--help` imprime les informations de référence CLI sur les commandes et leurs arguments, et répertorie les commandes et sous-groupes disponibles.
* `--output` modifie le format de sortie. Les formats de sortie disponibles sont `json`, `jsonc` (JSON coloré), `tsv` (valeurs séparées par des tabulations), `table` (tables ASCII lisibles) et `yaml`. Par défaut, l’interface CLI génère `json`. Pour en savoir plus sur les formats de sortie disponibles, consultez [Formats de sortie pour Azure CLI](format-output-azure-cli.md).
* `--query` utilise le [langage de requête JMESPath](http://jmespath.org/) pour filtrer la sortie retournée à partir des services Azure. Pour en savoir plus sur les requêtes, consultez [Interroger des résultats de commande avec Azure CLI](query-azure-cli.md) et le [tutoriel JMESPath](http://jmespath.org/tutorial.html).
* `--verbose` imprime les informations sur les ressources créées dans Azure pendant une opération, et d’autres informations utiles.
* `--debug` imprime davantage d’informations sur les opérations CLI, utilisées pour le débogage. Si vous rencontrez un bogue, fournissez la sortie générée avec l’indicateur `--debug` lors de l’envoi d’un rapport de bogue.

## <a name="interactive-mode"></a>Mode interactif

L’interface CLI propose un mode interactif qui affiche automatiquement les informations d’aide et qui facilite la sélection de sous-commandes. Vous pouvez entrer en mode interactif avec la commande [az interactive](/cli/azure/reference-index#az-interactive).

```azurecli-interactive
az interactive
```

Pour plus d’informations sur le mode interactif, consultez [Mode interactif Azure CLI](interactive-azure-cli.md).

Il existe également un [plug-in Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azurecli) qui propose une expérience interactive, comprenant l’autocomplétion et le survol de la documentation.

## <a name="learn-cli-basics-with-quickstarts-and-tutorials"></a>Apprendre les concepts de base CLI à l’aide des démarrages rapides et des didacticiels

Pour vous aider à prendre en main Azure CLI, lancez-vous dans un didacticiel approfondi de configuration des machines virtuelles, et utilisez la puissance de l’interface de ligne de commande pour interroger des ressources Azure.

> [!div class="nextstepaction"]
> [Créer des machines virtuelles avec le didacticiel Azure CLI](azure-cli-vm-tutorial.yml)

Il existe également des guides de démarrage rapide pour les autres services populaires.

* [Créer un compte de stockage à l’aide d’Azure CLI](/azure/storage/common/storage-quickstart-create-storage-account-cli)
* [Transférer des objets vers/à partir du stockage blob Azure à l’aide de l’interface CLI](/azure/storage/blobs/storage-quickstart-blobs-cli)
* [Créer une base de données Azure SQL unique à l’aide d’Azure CLI](/azure/sql-database/sql-database-get-started-cli)
* [Créer un serveur de base de données Azure pour MySQL à l’aide d’Azure CLI](/azure/mysql/quickstart-create-mysql-server-database-using-azure-cli)
* [Création d’une instance d’Azure Database pour PostgreSQL à l’aide de la CLI Azure](/azure/postgresql/quickstart-create-server-database-azure-cli)
* [Créer une application web Python dans Azure](/azure/app-service/app-service-web-get-started-python)
* [Exécuter une image Docker Hub personnalisée dans Azure Web App for Containers](/azure/app-service/containers/quickstart-custom-docker-image)

## <a name="give-feedback"></a>Envoyer des commentaires

N’hésitez pas à nous faire part de vos commentaires au sujet de l’interface CLI pour nous aider à l’améliorer et à résoudre les bogues. Vous pouvez [signaler un problème sur GitHub](https://github.com/azure/azure-cli/issues) ou utiliser les fonctionnalités intégrées de l’interface CLI pour laisser des commentaires d’ordre général à l’aide de la commande [az feedback](/cli/azure/reference-index#az-feedback).

```azurecli-interactive
az feedback
```

## <a name="see-also"></a>Voir aussi

* [Services pouvant être gérés par l’interface Azure CLI](azure-services-the-azure-cli-can-manage.md)
* [Liste de référence complète des commandes pour Azure CLI](/cli/azure/reference-index)
* [Articles populaires sur l’utilisation de l’interface Azure CLI](popular-articles-using-the-azure-cli.md)
