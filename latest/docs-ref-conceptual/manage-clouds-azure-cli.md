---
title: "La gestion de plusieurs clouds avec l’interface de ligne de commande Azure 2.0"
description: "Créer, se connecter et gérer plusieurs clouds avec l’interface de ligne de commande Azure 2.0."
keywords: "Interface de ligne de commande Azure 2.0, Azure, clouds, centres de données, gouvernement, région, Chine, Allemagne"
author: sptramer
manager: douge
ms.author: sttramer
ms.date: 06/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.openlocfilehash: 0222b7339e46346ef6c7e9ad98616d9b71129942
ms.sourcegitcommit: f107cf927ea1ef51de181d87fc4bc078e9288e47
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/04/2017
---
# <a name="managing-multiple-clouds-with-azure-cli-20"></a>La gestion de plusieurs clouds avec l’interface de ligne de commande Azure 2.0

Si vous avez plusieurs abonnements associés à Azure, il se peut que vous ayez plusieurs cloud disponibles. Chaque cloud a ses propres points de terminaison associés et ses propres capacités. Ils sont souvent associés à une région particulière qui a des normes de protection de données ou des configurations différentes.

Pour travailler efficacement avec plusieurs clouds, vous devez être en mesure de basculer entre ceux qui sont actuellement actifs et éventuellement créer de nouveaux clouds.

## <a name="listing-clouds"></a>Énumération des clouds

Vous pouvez énumérer vos clouds disponibles avec la commande [liste des clouds](/cli/azure/cloud#list) . Cela indique le cloud actuellement actif, son profil actuel et vous fournit des informations sur les noms d’hôte et les suffixes régionaux.

Pour obtenir une liste des clouds disponibles et de celui qui est actuellement actif :

```azurecli
az cloud list --output table
```

```output
IsActive    Name               Profile
----------  -----------------  ---------
True        AzureCloud         latest
            AzureChinaCloud    latest
            AzureUSGovernment  latest
            AzureGermanCloud   latest
```

## <a name="switching-the-active-cloud"></a>Changement du cloud actif

Pour basculer le cloud actuellement actif, vous devez exécuter la commande [ensemble de clouds](/cli/azure/cloud#set) . Cette commande accepte un argument obligatoire, qui est le nom du cloud.

```azurecli
az cloud set --name AzureChinaCloud
```

> [!IMPORTANT]
> Si vous n’avez jamais effectué d’authentification pour le cloud actif, vous devez le faire avant d’effectuer d’autres opérations de l’interface de ligne de commande. Pour obtenir des instructions sur l’authentification, consultez [Se connecter avec l’interface de ligne de commande Azure 2.0](/cli/azure/authenticate-azure-cli).

## <a name="register-or-unregister-a-cloud"></a>Inscrire ou désinscrire un cloud

Inscrire un nouveau cloud si vous avez vos propres points de terminaison ou si vous avez besoin d’un profil différent. La création d’un cloud s’effectue avec la commande [cloud register](/cli/azure/cloud#register) . Cette commande nécessite un nom et éventuellement un ensemble de configurations et de désignations de point de terminaison.

Pour créer un cloud avec un point de terminaison spécialisé pour le gestionnaire de ressources, avec un profil spécifique :

```azurecli
az cloud register --name MyCloud --endpoint-resource-manager "https://my.endpoint.manager" --profile 2017-03-09-profile
```

Cela crée le cloud, mais ne le sélectionne _pas_ automatiquement.

Si vous n’avez plus besoin du cloud créé, il peut être annulé avec la commande [cloud unregister](/cli/azure/cloud#unregister) :

```azurecli
az cloud unregister --name MyCloud
```

