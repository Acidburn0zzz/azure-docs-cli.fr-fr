---
title: "Exécuter Azure CLI 2.0 dans un conteneur Docker"
description: "Exécution d’un conteneur Docker hébergeant l’interface Azure CLI 2.0"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 01/29/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 3a09eb6d83bb5401628bd952d199a03ecbb8216e
ms.sourcegitcommit: b93a19222e116d5880bbe64c03507c64e190331e
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/15/2018
---
# <a name="run-azure-cli-20-in-a-docker-container"></a><span data-ttu-id="bf4f7-103">Exécuter Azure CLI 2.0 dans un conteneur Docker</span><span class="sxs-lookup"><span data-stu-id="bf4f7-103">Run Azure CLI 2.0 in a Docker container</span></span>

<span data-ttu-id="bf4f7-104">Vous pouvez utiliser Docker pour exécuter un conteneur Linux autonome avec Azure CLI 2.0 préinstallé.</span><span class="sxs-lookup"><span data-stu-id="bf4f7-104">You can use Docker to run a standalone Linux container with the Azure CLI 2.0 pre-installed.</span></span> <span data-ttu-id="bf4f7-105">Docker vous permet de commencer rapidement avec un environnement dans lequel vous pouvez essayer l’interface de ligne de commande pour décider si elle vous convient, ou utiliser notre image comme une base pour votre propre déploiement.</span><span class="sxs-lookup"><span data-stu-id="bf4f7-105">Docker lets you get started quickly with an environment where you can try out the CLI to decide if it's right for you, or use our image as a base for your own deployment.</span></span>

## <a name="run-in-a-docker-container"></a><span data-ttu-id="bf4f7-106">Exécution dans un conteneur Docker</span><span class="sxs-lookup"><span data-stu-id="bf4f7-106">Run in a Docker container</span></span>

<span data-ttu-id="bf4f7-107">Installez l’interface de ligne de commande à l’aide de `docker run`.</span><span class="sxs-lookup"><span data-stu-id="bf4f7-107">Install the CLI using `docker run`.</span></span>

   ```bash
   docker run -it microsoft/azure-cli
   ```

<span data-ttu-id="bf4f7-108">L’interface de ligne de commande est installé sur l’image en tant que commande `az` dans `/usr/local/bin`.</span><span class="sxs-lookup"><span data-stu-id="bf4f7-108">The CLI is installed on the image as the `az` command in `/usr/local/bin`.</span></span>

> [!NOTE]
> <span data-ttu-id="bf4f7-109">Si vous souhaitez sélectionner les clés SSH à partir de votre environnement utilisateur, vous pouvez utiliser `-v ${HOME}:/root` pour monter $HOME en tant que `/root`.</span><span class="sxs-lookup"><span data-stu-id="bf4f7-109">If you want to pick up the SSH keys from your user environment, you can use `-v ${HOME}:/root` to mount $HOME as `/root`.</span></span>

> ```bash
> docker run -it -v ${HOME}:/root microsoft/azure-cli
> ```

## <a name="update-docker-image"></a><span data-ttu-id="bf4f7-110">Mise à jour d’une image Docker</span><span class="sxs-lookup"><span data-stu-id="bf4f7-110">Update Docker image</span></span>

<span data-ttu-id="bf4f7-111">La mise à jour avec Docker nécessite l’extraction de la nouvelle image et la recréation de tous les conteneurs existants.</span><span class="sxs-lookup"><span data-stu-id="bf4f7-111">Updating with Docker requires both pulling the new image and re-creating any existing containers.</span></span> <span data-ttu-id="bf4f7-112">Pour cette raison, évitez d’utiliser un conteneur hébergeant l’interface de ligne de commande comme magasin de données.</span><span class="sxs-lookup"><span data-stu-id="bf4f7-112">For this reason you should try to avoid using a container that hosts the CLI as a data store.</span></span>

<span data-ttu-id="bf4f7-113">Mettre à jour votre image locale avec `docker pull`.</span><span class="sxs-lookup"><span data-stu-id="bf4f7-113">Update your local image with `docker pull`.</span></span>

```bash
docker pull microsoft/azure-cli
```

## <a name="uninstall-docker-image"></a><span data-ttu-id="bf4f7-114">Désinstallation d’une image Docker</span><span class="sxs-lookup"><span data-stu-id="bf4f7-114">Uninstall Docker image</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="bf4f7-115">Après l’arrêt de tous les conteneurs exécutant l’image de l’interface CLI, supprimez-la.</span><span class="sxs-lookup"><span data-stu-id="bf4f7-115">After halting any containers running the CLI image, remove it.</span></span>

```bash
docker rmi microsoft/azure-cli
```
