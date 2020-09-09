---
title: Références Azure CLI pour Azure Data Share
description: Page de destination des références Azure CLI pour Azure Data Share
services: data-share
author: dbradish-microsoft
manager: barbkess
ms.service: data-share
ms.devlang: azurecli
ms.topic: reference
ms.date: 05/27/2020
ms.author: dbradish
ms.custom: devx-track-azurecli
ms.openlocfilehash: e8d834864b2d967beb18e9cd304b922db859ef09
ms.sourcegitcommit: 2da241715d25407ed22c1065c0c793acfd865996
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/09/2020
ms.locfileid: "89562768"
---
# <a name="azure-cli-for-azure-data-share"></a>Azure CLI pour Azure Data Share

L'interface de ligne de commande Azure ([Azure CLI](/cli/azure/what-is-azure-cli)) est un ensemble de commandes utilisées pour créer et gérer des ressources Azure.  Elle est disponible sur de nombreux services Azure, notamment Azure Data Share.  Plus de 65 commandes différentes sont à votre disposition pour le partage des données.  Ces commandes vous permettent d'utiliser efficacement le service à partir d'une ligne de commande.

## <a name="references-for-data-share"></a>Références pour Data Share

Toutes les commandes Azure CLI pour Azure Data Share sont actuellement des extensions d'Azure CLI.  Une extension vous donne accès à des commandes expérimentales et disponibles en préversion.  Découvrez-en plus sur les références des extensions dans [Utiliser des extensions avec Azure CLI](/cli/azure/azure-cli-extensions-overview).

|Référence Azure CLI |Description
|-|-|-|
| [az datashare](/cli/azure/ext/datashare/datashare) | Toutes les commandes permettant de gérer Azure Data Share.
| [az datashare account](/cli/azure/ext/datashare/datashare/account) | Commandes permettant de gérer les comptes Azure Data Share.
| [az datashare consumer](/cli/azure/ext/datashare/datashare/consumer) | Commandes permettant aux consommateurs de gérer Azure Data Share.
| [az datashare dataset](/cli/azure/ext/datashare/datashare/dataset) | Commandes permettant aux fournisseurs de gérer les jeux de données Azure Data Share.
| [az datashare invitation](/cli/azure/ext/datashare/datashare/invitation) | Commandes permettant aux consommateurs de gérer les invitations Azure Data Share.
| [az datashare provider-share-subscription](/cli/azure/ext/datashare/datashare/provider-share-subscription) | Commandes permettant aux fournisseurs de gérer les abonnements Azure Data Share.
| [az datashare synchronization](/cli/azure/ext/datashare/datashare/synchronization)  | Commandes permettant de gérer la synchronisation d'Azure Data Share.
| [az datashare synchronization-setting](/cli/azure/ext/datashare/datashare/synchronization-setting)  | Commandes permettant aux fournisseurs de gérer les paramètres de synchronisation d'Azure Data Share.

## <a name="reference-examples"></a>Exemples de références

Des exemples sont fournis avec chaque référence Azure CLI. Vous pouvez également effectuer ces tâches via le portail Azure, mais l'utilisation d'Azure CLI ne nécessite qu'une seule ligne de commande.  Les blocs de code suivants vous donneront une idée de la facilité d'utilisation d'Azure CLI.

Pour utiliser Azure Data Share, vous devrez d'abord disposer d'un groupe de ressources.  Les groupes de ressources Azure sont faciles à créer et à gérer avec Azure CLI.  

```azurecli
#create a resource group
az group create -location westus -name MyResourceGroup
```

```azurecli
#get a list of resource groups for a subscription
az group list --subscription MySubscription --output table
```

Et il est tout aussi simple de créer un compte de partage de données.

```azurecli
#create a data share account
az datashare account create --location "West US 2" --tags tag1=Red tag2=White --name MyAccount --resource-group MyResourceGroup
```

## <a name="see-also"></a>Voir aussi

* [Prise en main d'Azure CLI](/cli/azure/get-started-with-azure-cli) pour en savoir plus sur l'installation et la connexion.

* Découvrez des références [principales](/cli/azure/reference-index) et [d'extension](/cli/azure/azure-cli-extensions-list) supplémentaires dans la documentation Azure CLI.
