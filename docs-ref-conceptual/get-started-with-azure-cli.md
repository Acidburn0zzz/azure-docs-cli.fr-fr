---
title: Bien démarrer avec Azure CLI 2.0
description: Commencez à utiliser Azure CLI 2.0 en apprenant les commandes de base.
keywords: Azure CLI, aide CLI, aide Azure, requête, automatisation,
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/16/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: c973d31312fbe0f9232bf3f0f3ed5f3b70b6559a
ms.sourcegitcommit: 308f9eb433a05b814999ac404f63d181169fffeb
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/03/2018
ms.locfileid: "37439939"
---
# <a name="get-started-with-azure-cli-20"></a>Bien démarrer avec Azure CLI 2.0

Bienvenue dans Azure CLI 2.0 ! L’interface CLI est un outil conçu pour vous aider à utiliser rapidement et efficacement les services Azure, en mettant l’accent sur l’automatisation. Cet article présente les fonctionnalités de l’interface CLI et des liens vers des ressources qui vous aideront à être productif.

## <a name="install-and-sign-in"></a>Installation et connexion

Si ce n’est pas déjà fait, [installez l’interface CLI](install-azure-cli.md) ou essayez [Azure Cloud Shell](/azure/cloud-shell/overview).

Avant d’utiliser les commandes CLI avec une installation locale, vous devez vous connecter avec la commande [az login](/cli/azure/reference-index#az-login).

[!INCLUDE [interactive-login](includes/interactive-login.md)]

Il existe des méthodes pour se connecter de manière non interactive, qui sont traitées en détail dans [Se connecter avec Azure CLI 2.0](authenticate-azure-cli.md).

## <a name="common-commands"></a>Commandes courantes

Ce tableau répertorie quelques commandes courantes utilisées dans les liens CLI vers leurs pages de documentation dans la référence.
Toutes les sous-commandes de ces groupes et leur documentation peuvent être consultées dans la référence en ligne ou avec l’argument `--help`.

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

Les commandes de l’interface CLI sont fournies en tant que _sous-commandes_ de _groupes_.
Chaque groupe représente un service fourni par Azure, et les sous-groupes divisent les commandes pour ces services en regroupements logiques.

Pour rechercher des commandes, utilisez la commande [az find](/cli/azure/reference-index#az-find). Par exemple, pour rechercher des noms de commandes contenant `secret`, utilisez la commande suivante :

```azurecli-interactive
az find -q secret
```

Si vous savez avec quel groupe de commandes vous souhaitez travailler, l’argument `--help` constitue peut-être un meilleur choix. Il n’affiche pas que des informations détaillées pour une commande, mais lorsqu’il est utilisé avec un groupe de commandes, il affiche toutes les sous-commandes disponibles. Par exemple, lorsque vous travaillez avec des groupes de sécurité réseau (NSG), vous pouvez trouver les sous-groupes et commandes NSG disponibles.

```azurecli-interactive
az network nsg --help
```

L’interface CLI dispose de la saisie semi-automatique via la touche Tab pour les commandes de l’interpréteur de commandes bash.

## <a name="globally-available-arguments"></a>Arguments globalement disponibles

Certains arguments sont disponibles pour chaque commande.

* `--help` imprime les informations de référence CLI sur les commandes et leurs arguments, et répertorie les commandes et sous-groupes disponibles.
* `--output` modifie le format de sortie. Les formats de sortie disponibles sont `json`, `jsonc` (JSON coloré), `tsv` (valeurs séparées par des tabulations.), et `table` (tables ASCII lisibles). Par défaut, l’interface CLI génère `json`. Pour en savoir plus sur les formats de sortie disponibles, consultez [Formats de sortie pour Azure CLI 2.0](format-output-azure-cli.md).
* `--query` utilise le [langage de requête JMESPath](http://jmespath.org/) pour filtrer la sortie retournée à partir des services Azure. Pour en savoir plus sur les requêtes, consultez [Interroger des résultats de commande avec Azure CLI 2.0](query-azure-cli.md) et le [didacticiel JMESPath](http://jmespath.org/tutorial.html).
* `--verbose` imprime les informations sur les ressources créées dans Azure pendant une opération, et d’autres informations utiles.
* `--debug` imprime davantage d’informations sur les opérations CLI, utilisées pour le débogage. Si vous rencontrez un bogue, fournissez la sortie générée avec l’indicateur `--debug` lors de l’envoi d’un rapport de bogue.


## <a name="interactive-mode"></a>Mode interactif

L’interface CLI propose un mode interactif qui affiche automatiquement les informations d’aide et qui facilite la sélection de sous-commandes. Vous pouvez entrer en mode interactif avec la commande [az interactive](/cli/azure/reference-index#az-interactive).

```azurecli-interactive
az interactive
```

Pour plus d’informations sur le mode interactif, consultez [Mode interactif Azure CLI 2.0](interactive-azure-cli.md).

Il existe également un [plug-in Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azurecli) qui propose une expérience interactive, comprenant la saisie semi-automatique et le survol de la documentation.

## <a name="learn-cli-basics-with-quickstarts-and-tutorials"></a>Apprendre les concepts de base CLI à l’aide des démarrages rapides et des didacticiels

Pour vous aider à démarrer avec l’interface Azure CLI 2.0, essayez un didacticiel approfondi pour configurer les machines virtuelles et utiliser la puissance de l’interface CLI pour interroger les ressources Azure.

> [!div class="nextstepaction"]
> [Créer des machines virtuelles avec le didacticiel Azure CLI 2.0](azure-cli-vm-tutorial.yml)

Si vous préférez vous concentrer sur d’autres services, il existe plusieurs Démarrages rapides pour les services Azure qui utilisent l’interface CLI.

* [Créer un compte de stockage à l’aide d’Azure CLI](/azure/storage/common/storage-quickstart-create-storage-account-cli)
* [Transférer des objets vers/à partir du stockage blob Azure à l’aide de l’interface CLI](/azure/storage/blobs/storage-quickstart-blobs-cli)
* [Créer une base de données SQL Azure unique à l’aide d’Azure CLI](/azure/sql-database/sql-database-get-started-cli)
* [Créer un serveur de base de données Azure pour MySQL à l’aide d’Azure CLI](/azure/mysql/quickstart-create-mysql-server-database-using-azure-cli)
* [Création d’une instance d’Azure Database pour PostgreSQL à l’aide de la CLI Azure](/azure/postgresql/quickstart-create-server-database-azure-cli)
* [Créer une application web Python dans Azure](/azure/app-service/app-service-web-get-started-python)
* [Exécuter une image Docker Hub personnalisée dans Azure Web App for Containers](/azure/app-service/containers/quickstart-custom-docker-image)

## <a name="give-feedback"></a>Envoyer des commentaires

N’hésitez pas à nous faire part de vos commentaires au sujet de l’interface CLI pour nous aider à l’améliorer et à résoudre les bogues. Vous pouvez [signaler un problème sur Github](https://github.com/azure/azure-cli/issues) ou utiliser les fonctionnalités intégrées de l’interface CLI pour laisser un commentaire général avec la commande [az feedback](/cli/azure/reference-index#az-feedback).

```azurecli-interactive
az feedback
```
