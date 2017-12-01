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
# <a name="install-azure-cli-20-with-docker"></a><span data-ttu-id="ded41-104">Installer Azure CLI 2.0 avec Docker</span><span class="sxs-lookup"><span data-stu-id="ded41-104">Install Azure CLI 2.0 with Docker</span></span>

<span data-ttu-id="ded41-105">Vous pouvez utiliser Docker pour installer un conteneur Linux autonome avec Azure CLI 2.0 préinstallé.</span><span class="sxs-lookup"><span data-stu-id="ded41-105">You can use Docker to install a standalone Linux container with the Azure CLI 2.0 pre-installed.</span></span> <span data-ttu-id="ded41-106">Cela vous permet de commencer rapidement avec un environnement dans lequel vous pouvez essayer l’interface de ligne de commande pour décider si elle vous convient, ou vous permet d’utiliser cela comme une image de base.</span><span class="sxs-lookup"><span data-stu-id="ded41-106">This lets you get started quickly with an environment where you can try out the CLI to decide if it's right for you, or allows you to use this as a base image.</span></span>

## <a name="install-with-docker"></a><span data-ttu-id="ded41-107">Installer avec Docker</span><span class="sxs-lookup"><span data-stu-id="ded41-107">Install with Docker</span></span>

<span data-ttu-id="ded41-108">Installez l’interface de ligne de commande à l’aide de `docker run`.</span><span class="sxs-lookup"><span data-stu-id="ded41-108">Install the CLI using `docker run`.</span></span>

   ```bash
   docker run -it azuresdk/azure-cli-python:<version>
   ```

<span data-ttu-id="ded41-109">Consultez nos [balises Docker](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/) pour connaître les versions disponibles.</span><span class="sxs-lookup"><span data-stu-id="ded41-109">See our [Docker tags](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/) for available versions.</span></span>

<span data-ttu-id="ded41-110">L’interface de ligne de commande est installé sur l’image en tant que commande `az` dans `/usr/local/bin`.</span><span class="sxs-lookup"><span data-stu-id="ded41-110">The CLI is installed on the image as the `az` command in `/usr/local/bin`.</span></span>

> [!NOTE]
> <span data-ttu-id="ded41-111">Si vous souhaitez sélectionner les clés SSH à partir de votre environnement utilisateur, vous pouvez utiliser `-v ${HOME}:/root` pour monter $HOME en tant que `/root`.</span><span class="sxs-lookup"><span data-stu-id="ded41-111">If you want to pick up the SSH keys from your user environment, you can use `-v ${HOME}:/root` to mount $HOME as `/root`.</span></span>

> ```bash
> docker run -it -v ${HOME}:/root azuresdk/azure-cli-python:<version>
> ```

### <a name="update-with-docker"></a><span data-ttu-id="ded41-112">Mettre à jour avec Docker</span><span class="sxs-lookup"><span data-stu-id="ded41-112">Update with Docker</span></span>

<span data-ttu-id="ded41-113">La mise à jour avec Docker nécessite l’extraction de la nouvelle image et la recréation de tous les conteneurs existants.</span><span class="sxs-lookup"><span data-stu-id="ded41-113">Updating with Docker requires both pulling the new image and re-creating any existing containers.</span></span> <span data-ttu-id="ded41-114">Pour cette raison, évitez d’utiliser un conteneur hébergeant l’interface de ligne de commande comme magasin de données.</span><span class="sxs-lookup"><span data-stu-id="ded41-114">For this reason you should try and avoid using a container which hosts the CLI as a data store.</span></span>

1. <span data-ttu-id="ded41-115">Mettre à jour votre image locale avec `docker pull`.</span><span class="sxs-lookup"><span data-stu-id="ded41-115">Update your local image with `docker pull`.</span></span>

   ```bash
   docker pull azuresdk/azure-cli-python
   ```

2. <span data-ttu-id="ded41-116">Obtenir les conteneurs qui utilisent actuellement l’image de l’interface de ligne de commande.</span><span class="sxs-lookup"><span data-stu-id="ded41-116">Get the containers currently using the CLI image.</span></span>

   ```bash
   docker container ls -a --filter 'ancestor=azuresdk/azure-cli-python'
   ```

   ```output
   CONTAINER ID        IMAGE                              COMMAND             CREATED             STATUS                        PORTS               NAMES
   34a868beb2ab        azuresdk/azure-cli-python:latest      "/bin/sh -c bash"   8 minutes ago       Exited (0) 8 minutes ago                       inspiring_benz
   ```

  > [!NOTE]
  > <span data-ttu-id="ded41-117">Si vous avez installé une version spécifique de l’image, vous devez ajouter `:<version>` à la fin du nom de l’image.</span><span class="sxs-lookup"><span data-stu-id="ded41-117">If you installed a specific version of the image, you will need to add `:<version>` to the end of the image name.</span></span>

3. <span data-ttu-id="ded41-118">Interrompre et recréer les conteneurs.</span><span class="sxs-lookup"><span data-stu-id="ded41-118">Halt and recreate the containers.</span></span>

   ```bash
   docker stop inspiring_benz
   docker rm inspiring_benz
   docker run azuresdk/azure-cli-python
   ```

### <a name="uninstall-with-docker"></a><span data-ttu-id="ded41-119">Désinstaller avec Docker</span><span class="sxs-lookup"><span data-stu-id="ded41-119">Uninstall with Docker</span></span>

<span data-ttu-id="ded41-120">Si jamais vous décidez de désinstaller l’interface de ligne de commande Azure, nous sommes désolés de vous voir partir.</span><span class="sxs-lookup"><span data-stu-id="ded41-120">If you ever decide to uninstall the Azure CLI, we're sorry to see you go.</span></span> <span data-ttu-id="ded41-121">Avant de désinstaller, utilisez la commande `az feedback`, afin de nous donner quelques raisons pour lesquelles vous avez choisi de désinstaller et nous aider à améliorer l’expérience CLI.</span><span class="sxs-lookup"><span data-stu-id="ded41-121">Before you uninstall, use the `az feedback` command to give us some reasons why you chose to uninstall and how we could improve the CLI experience.</span></span> <span data-ttu-id="ded41-122">Nous souhaitons nous assurer que l’interface de ligne de commande Azure est aussi conviviale et exempte de bogues que possible.</span><span class="sxs-lookup"><span data-stu-id="ded41-122">We want to make sure that the Azure CLI is as bug-free and user-friendly as we can make it.</span></span> <span data-ttu-id="ded41-123">Vous pouvez également [signaler un problème lié à GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="ded41-123">You can also [file a github issue](https://github.com/Azure/azure-cli/issues).</span></span>

<span data-ttu-id="ded41-124">Pour désinstaller correctement l’image Docker de l’interface de ligne de commande, vous devez supprimer tous les conteneurs qui l’exécutent avant de supprimer l’image locale.</span><span class="sxs-lookup"><span data-stu-id="ded41-124">To properly uninstall the CLI Docker image you need to remove any containers running it, and then delete the local image.</span></span>

1. <span data-ttu-id="ded41-125">Obtenez les conteneurs exécutant l’image de l’interface de ligne de commande Azure.</span><span class="sxs-lookup"><span data-stu-id="ded41-125">Get the containers running the azure-cli image.</span></span>

   ```bash
   docker container ls -a --filter 'ancestor=azuresdk/azure-cli-python'
   ```

   ```output
   CONTAINER ID        IMAGE                              COMMAND             CREATED             STATUS                        PORTS               NAMES
   34a868beb2ab        azuresdk/azure-cli-python:latest      "/bin/sh -c bash"   8 minutes ago       Exited (0) 8 minutes ago                       inspiring_benz
   ```
  > [!NOTE]
  > <span data-ttu-id="ded41-126">Si vous avez installé une version spécifique de l’image, vous devez ajouter `:<version>` à la fin du nom de l’image.</span><span class="sxs-lookup"><span data-stu-id="ded41-126">If you installed a specific version of the image, you will need to add `:<version>` to the end of the image name.</span></span>

2. <span data-ttu-id="ded41-127">Supprimez tous les conteneurs avec l’image de l’interface de ligne de commande.</span><span class="sxs-lookup"><span data-stu-id="ded41-127">Delete any containers with the CLI image.</span></span>

   ```bash
   docker rm 34a868beb2ab
   ```

3. <span data-ttu-id="ded41-128">Supprimez l’image de l’interface de ligne de commande installée localement.</span><span class="sxs-lookup"><span data-stu-id="ded41-128">Remove the locally installed CLI image.</span></span>

   ```bash
   docker rmi azuresdk/azure-cli-python
   ```

