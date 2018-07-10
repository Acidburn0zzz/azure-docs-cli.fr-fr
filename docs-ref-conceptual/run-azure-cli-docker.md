---
title: Exécuter Azure CLI 2.0 dans un conteneur Docker
description: Exécution d’un conteneur Docker hébergeant l’interface Azure CLI 2.0
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 01/29/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 0eb3694c8dcb085e1aeb8cde54a21ac16157b26b
ms.sourcegitcommit: 308f9eb433a05b814999ac404f63d181169fffeb
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/03/2018
ms.locfileid: "37439824"
---
# <a name="run-azure-cli-20-in-a-docker-container"></a>Exécuter Azure CLI 2.0 dans un conteneur Docker

Vous pouvez utiliser Docker pour exécuter un conteneur Linux autonome avec Azure CLI 2.0 préinstallé. Docker vous permet de commencer rapidement avec un environnement dans lequel vous pouvez essayer l’interface de ligne de commande pour décider si elle vous convient, ou utiliser notre image comme une base pour votre propre déploiement.

## <a name="run-in-a-docker-container"></a>Exécution dans un conteneur Docker

Installez l’interface de ligne de commande à l’aide de `docker run`.

   ```bash
   docker run -it microsoft/azure-cli
   ```

> [!NOTE]
> Si vous souhaitez sélectionner les clés SSH à partir de votre environnement utilisateur, vous pouvez utiliser `-v ${HOME}:/root` pour monter $HOME en tant que `/root`.

> ```bash
> docker run -it -v ${HOME}:/root microsoft/azure-cli
> ```

L’interface de ligne de commande est installé sur l’image en tant que commande `az` dans `/usr/local/bin`. Pour vous connecter, exécutez la commande [az login](/cli/azure/reference-index#az-login).

[!INCLUDE [interactive-login](includes/interactive-login.md)]

Pour en savoir plus sur les différentes méthodes de connexion, consultez [Se connecter avec Azure CLI 2.0](authenticate-azure-cli.md).


## <a name="update-docker-image"></a>Mise à jour d’une image Docker

La mise à jour avec Docker nécessite l’extraction de la nouvelle image et la recréation de tous les conteneurs existants. Pour cette raison, évitez d’utiliser un conteneur hébergeant l’interface de ligne de commande comme magasin de données.

Mettre à jour votre image locale avec `docker pull`.

```bash
docker pull microsoft/azure-cli
```

## <a name="uninstall-docker-image"></a>Désinstallation d’une image Docker

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

Après l’arrêt de tous les conteneurs exécutant l’image de l’interface CLI, supprimez-la.

```bash
docker rmi microsoft/azure-cli
```
