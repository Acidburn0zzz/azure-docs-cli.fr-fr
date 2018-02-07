---
title: "Exécuter Azure CLI 2.0 dans un conteneur Docker"
description: "Exécution d’un conteneur Docker hébergeant l’interface Azure CLI 2.0"
keywords: "Azure CLI, installation d’Azure CLI, Azure Docker, image Azure Docker,"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 01/29/18
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 819ff0cdb0df6057a5dff8f8ab015796f06c6a9b
ms.sourcegitcommit: 8606f36963e8daa6448d637393d1e4ef2c9859a0
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/01/2018
---
# <a name="run-azure-cli-20-in-a-docker-container"></a>Exécuter Azure CLI 2.0 dans un conteneur Docker

Vous pouvez utiliser Docker pour exécuter un conteneur Linux autonome avec Azure CLI 2.0 préinstallé. Docker vous permet de commencer rapidement avec un environnement dans lequel vous pouvez essayer l’interface de ligne de commande pour décider si elle vous convient, ou utiliser notre image comme une base pour votre propre déploiement.

## <a name="run-in-a-docker-container"></a>Exécution dans un conteneur Docker

Installez l’interface de ligne de commande à l’aide de `docker run`.

   ```bash
   docker run -it microsoft/azure-cli
   ```

L’interface de ligne de commande est installé sur l’image en tant que commande `az` dans `/usr/local/bin`.

> [!NOTE]
> Si vous souhaitez sélectionner les clés SSH à partir de votre environnement utilisateur, vous pouvez utiliser `-v ${HOME}:/root` pour monter $HOME en tant que `/root`.

> ```bash
> docker run -it -v ${HOME}:/root microsoft/azure-cli
> ```

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
