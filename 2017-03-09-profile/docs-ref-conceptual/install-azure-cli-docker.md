---
title: "Installer l’interface de ligne de commande Azure avec Docker"
description: Comment installer un conteneur Docker avec Azure CLI 2.0
keywords: "Azure CLI, installation d’Azure CLI, Azure Docker, image Azure Docker,"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 10/30/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ROBOTS: NOINDEX,NOFOLLOW
ms.openlocfilehash: 76ecf2c9cd0e6e694a31ac160112d1348863f118
ms.sourcegitcommit: 905939cc44764b4d1cc79a9b36c0793f7055a686
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/20/2017
---
# <a name="install-azure-cli-20-with-docker"></a>Installer Azure CLI 2.0 avec Docker

Vous pouvez utiliser Docker pour installer un conteneur Linux autonome avec Azure CLI 2.0 préinstallé. Cela vous permet de commencer rapidement avec un environnement dans lequel vous pouvez essayer l’interface de ligne de commande pour décider si elle vous convient, ou vous permet d’utiliser cela comme une image de base.

## <a name="install-with-docker"></a>Installer avec Docker

Installez l’interface de ligne de commande à l’aide de `docker run`.

   ```bash
   docker run -it azuresdk/azure-cli-python:<version>
   ```

Consultez nos [balises Docker](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/) pour connaître les versions disponibles.

L’interface de ligne de commande est installé sur l’image en tant que commande `az` dans `/usr/local/bin`.

> [!NOTE]
> Si vous souhaitez sélectionner les clés SSH à partir de votre environnement utilisateur, vous pouvez utiliser `-v ${HOME}:/root` pour monter $HOME en tant que `/root`.

> ```bash
> docker run -it -v ${HOME}:/root azuresdk/azure-cli-python:<version>
> ```

### <a name="update-with-docker"></a>Mettre à jour avec Docker

La mise à jour avec Docker nécessite l’extraction de la nouvelle image et la recréation de tous les conteneurs existants. Pour cette raison, évitez d’utiliser un conteneur hébergeant l’interface de ligne de commande comme magasin de données.

1. Mettre à jour votre image locale avec `docker pull`.

   ```bash
   docker pull azuresdk/azure-cli-python
   ```

2. Obtenir les conteneurs qui utilisent actuellement l’image de l’interface de ligne de commande.

   ```bash
   docker container ls -a --filter 'ancestor=azuresdk/azure-cli-python'
   ```

   ```output
   CONTAINER ID        IMAGE                              COMMAND             CREATED             STATUS                        PORTS               NAMES
   34a868beb2ab        azuresdk/azure-cli-python:latest      "/bin/sh -c bash"   8 minutes ago       Exited (0) 8 minutes ago                       inspiring_benz
   ```

  > [!NOTE]
  > Si vous avez installé une version spécifique de l’image, vous devez ajouter `:<version>` à la fin du nom de l’image.

3. Interrompre et recréer les conteneurs.

   ```bash
   docker stop inspiring_benz
   docker rm inspiring_benz
   docker run azuresdk/azure-cli-python
   ```

### <a name="uninstall-with-docker"></a>Désinstaller avec Docker

Si jamais vous décidez de désinstaller l’interface de ligne de commande Azure, nous sommes désolés de vous voir partir. Avant de désinstaller, utilisez la commande `az feedback`, afin de nous donner quelques raisons pour lesquelles vous avez choisi de désinstaller et nous aider à améliorer l’expérience CLI. Nous souhaitons nous assurer que l’interface de ligne de commande Azure est aussi conviviale et exempte de bogues que possible. Vous pouvez également [signaler un problème lié à GitHub](https://github.com/Azure/azure-cli/issues).

Pour désinstaller correctement l’image Docker de l’interface de ligne de commande, vous devez supprimer tous les conteneurs qui l’exécutent avant de supprimer l’image locale.

1. Obtenez les conteneurs exécutant l’image de l’interface de ligne de commande Azure.

   ```bash
   docker container ls -a --filter 'ancestor=azuresdk/azure-cli-python'
   ```

   ```output
   CONTAINER ID        IMAGE                              COMMAND             CREATED             STATUS                        PORTS               NAMES
   34a868beb2ab        azuresdk/azure-cli-python:latest      "/bin/sh -c bash"   8 minutes ago       Exited (0) 8 minutes ago                       inspiring_benz
   ```
  > [!NOTE]
  > Si vous avez installé une version spécifique de l’image, vous devez ajouter `:<version>` à la fin du nom de l’image.

2. Supprimez tous les conteneurs avec l’image de l’interface de ligne de commande.

   ```bash
   docker rm 34a868beb2ab
   ```

3. Supprimez l’image de l’interface de ligne de commande installée localement.

   ```bash
   docker rmi azuresdk/azure-cli-python
   ```

