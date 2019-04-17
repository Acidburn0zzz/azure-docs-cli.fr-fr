---
title: Exécuter Azure CLI dans un conteneur Docker
description: Comment exécuter un conteneur Docker hébergeant Azure CLI
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 01/29/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 346014c1890cd7aa5b4225df15078e55db908a33
ms.sourcegitcommit: 754c550b417f26e27f2e31cd0a04826aa8ff4f64
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/08/2019
ms.locfileid: "59289081"
---
# <a name="run-azure-cli-in-a-docker-container"></a><span data-ttu-id="c58d6-103">Exécuter Azure CLI dans un conteneur Docker</span><span class="sxs-lookup"><span data-stu-id="c58d6-103">Run Azure CLI in a Docker container</span></span>

<span data-ttu-id="c58d6-104">Vous pouvez utiliser Docker pour exécuter un conteneur Linux autonome avec Azure CLI préinstallée.</span><span class="sxs-lookup"><span data-stu-id="c58d6-104">You can use Docker to run a standalone Linux container with the Azure CLI pre-installed.</span></span> <span data-ttu-id="c58d6-105">Docker vous permet de vous familiariser rapidement avec un environnement isolé pour pouvoir y exécuter l’interface CLI.</span><span class="sxs-lookup"><span data-stu-id="c58d6-105">Docker gets you started quickly with an isolated environment to run the CLI in.</span></span> <span data-ttu-id="c58d6-106">L’image peut également être utilisée comme base pour vos propres déploiements.</span><span class="sxs-lookup"><span data-stu-id="c58d6-106">The image can also be used as a base for your own deployments.</span></span>

## <a name="run-in-a-docker-container"></a><span data-ttu-id="c58d6-107">Exécution dans un conteneur Docker</span><span class="sxs-lookup"><span data-stu-id="c58d6-107">Run in a Docker container</span></span>

> [!NOTE]
> <span data-ttu-id="c58d6-108">Azure CLI a été déplacé vers [Microsoft Container Registry](https://azure.microsoft.com/services/container-registry).</span><span class="sxs-lookup"><span data-stu-id="c58d6-108">The Azure CLI has migrated to [Microsoft Container Registry](https://azure.microsoft.com/services/container-registry).</span></span> <span data-ttu-id="c58d6-109">Les balises existantes sur Docker Hub sont toujours prises en charge, mais les nouvelles versions pourront uniquement être utilisées sous la forme mcr.microsoft.com/azure-cli.</span><span class="sxs-lookup"><span data-stu-id="c58d6-109">Existing tags on Docker Hub are still supported, but new releases will only be available as mcr.microsoft.com/azure-cli.</span></span>

<span data-ttu-id="c58d6-110">Installez l’interface de ligne de commande à l’aide de `docker run`.</span><span class="sxs-lookup"><span data-stu-id="c58d6-110">Install the CLI using `docker run`.</span></span>

   ```bash
   docker run -it mcr.microsoft.com/azure-cli
   ```

> [!NOTE]
> <span data-ttu-id="c58d6-111">Si vous souhaitez sélectionner les clés SSH à partir de votre environnement utilisateur, utilisez `-v ${HOME}/.ssh:/root/.ssh` pour monter vos clés SSH dans l’environnement.</span><span class="sxs-lookup"><span data-stu-id="c58d6-111">If you want to pick up the SSH keys from your user environment, use `-v ${HOME}/.ssh:/root/.ssh` to mount your SSH keys in the environment.</span></span>
>
> ```bash
> docker run -it -v ${HOME}/.ssh:/root/.ssh mcr.microsoft.com/azure-cli
> ```

<span data-ttu-id="c58d6-112">L’interface de ligne de commande est installé sur l’image en tant que commande `az` dans `/usr/local/bin`.</span><span class="sxs-lookup"><span data-stu-id="c58d6-112">The CLI is installed on the image as the `az` command in `/usr/local/bin`.</span></span> <span data-ttu-id="c58d6-113">Pour vous connecter, exécutez la commande [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="c58d6-113">To sign in, run the [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="c58d6-114">Pour en savoir plus sur les différentes méthodes d’authentification, consultez [Se connecter avec Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="c58d6-114">To learn more about different authentication methods, see [Sign in with the Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="update-docker-image"></a><span data-ttu-id="c58d6-115">Mise à jour d’une image Docker</span><span class="sxs-lookup"><span data-stu-id="c58d6-115">Update Docker image</span></span>

<span data-ttu-id="c58d6-116">La mise à jour avec Docker nécessite l’extraction de la nouvelle image et la recréation de tous les conteneurs existants.</span><span class="sxs-lookup"><span data-stu-id="c58d6-116">Updating with Docker requires both pulling the new image and re-creating any existing containers.</span></span> <span data-ttu-id="c58d6-117">Pour cette raison, évitez d’utiliser un conteneur hébergeant l’interface CLI comme magasin de données.</span><span class="sxs-lookup"><span data-stu-id="c58d6-117">For this reason, you should try to avoid using a container that hosts the CLI as a data store.</span></span>

<span data-ttu-id="c58d6-118">Mettre à jour votre image locale avec `docker pull`.</span><span class="sxs-lookup"><span data-stu-id="c58d6-118">Update your local image with `docker pull`.</span></span>

```bash
docker pull mcr.microsoft.com/azure-cli
```

## <a name="uninstall-docker-image"></a><span data-ttu-id="c58d6-119">Désinstallation d’une image Docker</span><span class="sxs-lookup"><span data-stu-id="c58d6-119">Uninstall Docker image</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="c58d6-120">Après l’arrêt de tous les conteneurs exécutant l’image de l’interface CLI, supprimez-la.</span><span class="sxs-lookup"><span data-stu-id="c58d6-120">After halting any containers running the CLI image, remove it.</span></span>

```bash
docker rmi mcr.microsoft.com/azure-cli
```

## <a name="next-steps"></a><span data-ttu-id="c58d6-121">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="c58d6-121">Next Steps</span></span>

<span data-ttu-id="c58d6-122">Maintenant que vous êtes prêt à utiliser l’interface CLI, découvrez ses fonctionnalités et ses commandes courantes.</span><span class="sxs-lookup"><span data-stu-id="c58d6-122">Now that you're ready to use the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="c58d6-123">Bien démarrer avec Azure CLI</span><span class="sxs-lookup"><span data-stu-id="c58d6-123">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
