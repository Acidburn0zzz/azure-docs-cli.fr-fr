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
# <a name="run-azure-cli-20-in-a-docker-container"></a><span data-ttu-id="55b0e-104">Exécuter Azure CLI 2.0 dans un conteneur Docker</span><span class="sxs-lookup"><span data-stu-id="55b0e-104">Run Azure CLI 2.0 in a Docker container</span></span>

<span data-ttu-id="55b0e-105">Vous pouvez utiliser Docker pour exécuter un conteneur Linux autonome avec Azure CLI 2.0 préinstallé.</span><span class="sxs-lookup"><span data-stu-id="55b0e-105">You can use Docker to run a standalone Linux container with the Azure CLI 2.0 pre-installed.</span></span> <span data-ttu-id="55b0e-106">Docker vous permet de commencer rapidement avec un environnement dans lequel vous pouvez essayer l’interface de ligne de commande pour décider si elle vous convient, ou utiliser notre image comme une base pour votre propre déploiement.</span><span class="sxs-lookup"><span data-stu-id="55b0e-106">Docker lets you get started quickly with an environment where you can try out the CLI to decide if it's right for you, or use our image as a base for your own deployment.</span></span>

## <a name="run-in-a-docker-container"></a><span data-ttu-id="55b0e-107">Exécution dans un conteneur Docker</span><span class="sxs-lookup"><span data-stu-id="55b0e-107">Run in a Docker container</span></span>

<span data-ttu-id="55b0e-108">Installez l’interface de ligne de commande à l’aide de `docker run`.</span><span class="sxs-lookup"><span data-stu-id="55b0e-108">Install the CLI using `docker run`.</span></span>

   ```bash
   docker run -it microsoft/azure-cli
   ```

<span data-ttu-id="55b0e-109">L’interface de ligne de commande est installé sur l’image en tant que commande `az` dans `/usr/local/bin`.</span><span class="sxs-lookup"><span data-stu-id="55b0e-109">The CLI is installed on the image as the `az` command in `/usr/local/bin`.</span></span>

> [!NOTE]
> <span data-ttu-id="55b0e-110">Si vous souhaitez sélectionner les clés SSH à partir de votre environnement utilisateur, vous pouvez utiliser `-v ${HOME}:/root` pour monter $HOME en tant que `/root`.</span><span class="sxs-lookup"><span data-stu-id="55b0e-110">If you want to pick up the SSH keys from your user environment, you can use `-v ${HOME}:/root` to mount $HOME as `/root`.</span></span>

> ```bash
> docker run -it -v ${HOME}:/root microsoft/azure-cli
> ```

## <a name="update-docker-image"></a><span data-ttu-id="55b0e-111">Mise à jour d’une image Docker</span><span class="sxs-lookup"><span data-stu-id="55b0e-111">Update Docker image</span></span>

<span data-ttu-id="55b0e-112">La mise à jour avec Docker nécessite l’extraction de la nouvelle image et la recréation de tous les conteneurs existants.</span><span class="sxs-lookup"><span data-stu-id="55b0e-112">Updating with Docker requires both pulling the new image and re-creating any existing containers.</span></span> <span data-ttu-id="55b0e-113">Pour cette raison, évitez d’utiliser un conteneur hébergeant l’interface de ligne de commande comme magasin de données.</span><span class="sxs-lookup"><span data-stu-id="55b0e-113">For this reason you should try to avoid using a container that hosts the CLI as a data store.</span></span>

<span data-ttu-id="55b0e-114">Mettre à jour votre image locale avec `docker pull`.</span><span class="sxs-lookup"><span data-stu-id="55b0e-114">Update your local image with `docker pull`.</span></span>

```bash
docker pull microsoft/azure-cli
```

## <a name="uninstall-docker-image"></a><span data-ttu-id="55b0e-115">Désinstallation d’une image Docker</span><span class="sxs-lookup"><span data-stu-id="55b0e-115">Uninstall Docker image</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="55b0e-116">Après l’arrêt de tous les conteneurs exécutant l’image de l’interface CLI, supprimez-la.</span><span class="sxs-lookup"><span data-stu-id="55b0e-116">After halting any containers running the CLI image, remove it.</span></span>

```bash
docker rmi microsoft/azure-cli
```
