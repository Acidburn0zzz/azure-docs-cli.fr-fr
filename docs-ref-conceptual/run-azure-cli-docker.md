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
ms.openlocfilehash: 2a4515f5301daca68f6e1a161fb2327f6caa0cf5
ms.sourcegitcommit: 7f79860c799e78fd8a591d7a5550464080e07aa9
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/12/2019
ms.locfileid: "56158253"
---
# <a name="run-azure-cli-in-a-docker-container"></a><span data-ttu-id="9da56-103">Exécuter Azure CLI dans un conteneur Docker</span><span class="sxs-lookup"><span data-stu-id="9da56-103">Run Azure CLI in a Docker container</span></span>

<span data-ttu-id="9da56-104">Vous pouvez utiliser Docker pour exécuter un conteneur Linux autonome avec Azure CLI préinstallée.</span><span class="sxs-lookup"><span data-stu-id="9da56-104">You can use Docker to run a standalone Linux container with the Azure CLI pre-installed.</span></span> <span data-ttu-id="9da56-105">Docker vous permet de vous familiariser rapidement avec un environnement isolé pour pouvoir y exécuter l’interface CLI.</span><span class="sxs-lookup"><span data-stu-id="9da56-105">Docker gets you started quickly with an isolated environment to run the CLI in.</span></span> <span data-ttu-id="9da56-106">L’image peut également être utilisée comme base pour vos propres déploiements.</span><span class="sxs-lookup"><span data-stu-id="9da56-106">The image can also be used as a base for your own deployments.</span></span>

## <a name="run-in-a-docker-container"></a><span data-ttu-id="9da56-107">Exécution dans un conteneur Docker</span><span class="sxs-lookup"><span data-stu-id="9da56-107">Run in a Docker container</span></span>

<span data-ttu-id="9da56-108">Installez l’interface de ligne de commande à l’aide de `docker run`.</span><span class="sxs-lookup"><span data-stu-id="9da56-108">Install the CLI using `docker run`.</span></span>

   ```bash
   docker run -it microsoft/azure-cli
   ```

> [!NOTE]
> <span data-ttu-id="9da56-109">Si vous souhaitez sélectionner les clés SSH à partir de votre environnement utilisateur, utilisez `-v ${HOME}/.ssh:/root/.ssh` pour monter vos clés SSH dans l’environnement.</span><span class="sxs-lookup"><span data-stu-id="9da56-109">If you want to pick up the SSH keys from your user environment, use `-v ${HOME}/.ssh:/root/.ssh` to mount your SSH keys in the environment.</span></span>
>
> ```bash
> docker run -it -v ${HOME}/.ssh:/root/.ssh microsoft/azure-cli
> ```

<span data-ttu-id="9da56-110">L’interface de ligne de commande est installé sur l’image en tant que commande `az` dans `/usr/local/bin`.</span><span class="sxs-lookup"><span data-stu-id="9da56-110">The CLI is installed on the image as the `az` command in `/usr/local/bin`.</span></span> <span data-ttu-id="9da56-111">Pour vous connecter, exécutez la commande [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="9da56-111">To sign in, run the [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="9da56-112">Pour en savoir plus sur les différentes méthodes d’authentification, consultez [Se connecter avec Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="9da56-112">To learn more about different authentication methods, see [Sign in with the Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="update-docker-image"></a><span data-ttu-id="9da56-113">Mise à jour d’une image Docker</span><span class="sxs-lookup"><span data-stu-id="9da56-113">Update Docker image</span></span>

<span data-ttu-id="9da56-114">La mise à jour avec Docker nécessite l’extraction de la nouvelle image et la recréation de tous les conteneurs existants.</span><span class="sxs-lookup"><span data-stu-id="9da56-114">Updating with Docker requires both pulling the new image and re-creating any existing containers.</span></span> <span data-ttu-id="9da56-115">Pour cette raison, évitez d’utiliser un conteneur hébergeant l’interface CLI comme magasin de données.</span><span class="sxs-lookup"><span data-stu-id="9da56-115">For this reason, you should try to avoid using a container that hosts the CLI as a data store.</span></span>

<span data-ttu-id="9da56-116">Mettre à jour votre image locale avec `docker pull`.</span><span class="sxs-lookup"><span data-stu-id="9da56-116">Update your local image with `docker pull`.</span></span>

```bash
docker pull microsoft/azure-cli
```

## <a name="uninstall-docker-image"></a><span data-ttu-id="9da56-117">Désinstallation d’une image Docker</span><span class="sxs-lookup"><span data-stu-id="9da56-117">Uninstall Docker image</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="9da56-118">Après l’arrêt de tous les conteneurs exécutant l’image de l’interface CLI, supprimez-la.</span><span class="sxs-lookup"><span data-stu-id="9da56-118">After halting any containers running the CLI image, remove it.</span></span>

```bash
docker rmi microsoft/azure-cli
```

## <a name="next-steps"></a><span data-ttu-id="9da56-119">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="9da56-119">Next Steps</span></span>

<span data-ttu-id="9da56-120">Maintenant que vous êtes prêt à utiliser l’interface CLI, découvrez ses fonctionnalités et ses commandes courantes.</span><span class="sxs-lookup"><span data-stu-id="9da56-120">Now that you're ready to use the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="9da56-121">Prise en main de l’interface Azure CLI</span><span class="sxs-lookup"><span data-stu-id="9da56-121">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
