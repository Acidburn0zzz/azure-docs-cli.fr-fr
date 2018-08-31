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
ms.openlocfilehash: 7a50682d549f6383e68128f2c2aef02dc2877a8e
ms.sourcegitcommit: 83826ca154c9f32c6091c63ce4b3e480694ba8d1
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/09/2018
ms.locfileid: "43144892"
---
# <a name="run-azure-cli-20-in-a-docker-container"></a>Exécuter Azure CLI 2.0 dans un conteneur Docker

Vous pouvez utiliser Docker pour exécuter un conteneur Linux autonome avec Azure CLI 2.0 préinstallé. Docker vous permet de commencer rapidement avec un environnement dans lequel vous pouvez essayer l’interface de ligne de commande pour décider si elle vous convient, ou utiliser notre image comme une base pour votre propre déploiement.

## <a name="run-in-a-docker-container"></a>Exécution dans un conteneur Docker

Installez l’interface de ligne de commande à l’aide de `docker run`.

   ```bash
   docker run -it microsoft/azure-cli
   ```

> [!NOTE]
> Si vous souhaitez sélectionner les clés SSH à partir de votre environnement utilisateur, vous pouvez utiliser `-v ${HOME}/.ssh:/root/.ssh` pour monter vos clés SSH dans l’environnement.
>
> ```bash
> docker run -it -v ${HOME}/.ssh:/root/.ssh microsoft/azure-cli
> ```

L’interface de ligne de commande est installé sur l’image en tant que commande `az` dans `/usr/local/bin`. Pour vous connecter, exécutez la commande [az login](/cli/azure/reference-index#az-login).

[!INCLUDE [interactive-login](includes/interactive-login.md)]

Pour en savoir plus sur les différentes méthodes d’authentification, consultez [Se connecter avec Azure CLI 2.0](authenticate-azure-cli.md).

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
