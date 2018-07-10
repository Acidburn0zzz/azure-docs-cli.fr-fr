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
# <a name="run-azure-cli-20-in-a-docker-container"></a><span data-ttu-id="ac1ee-103">Exécuter Azure CLI 2.0 dans un conteneur Docker</span><span class="sxs-lookup"><span data-stu-id="ac1ee-103">Run Azure CLI 2.0 in a Docker container</span></span>

<span data-ttu-id="ac1ee-104">Vous pouvez utiliser Docker pour exécuter un conteneur Linux autonome avec Azure CLI 2.0 préinstallé.</span><span class="sxs-lookup"><span data-stu-id="ac1ee-104">You can use Docker to run a standalone Linux container with the Azure CLI 2.0 pre-installed.</span></span> <span data-ttu-id="ac1ee-105">Docker vous permet de commencer rapidement avec un environnement dans lequel vous pouvez essayer l’interface de ligne de commande pour décider si elle vous convient, ou utiliser notre image comme une base pour votre propre déploiement.</span><span class="sxs-lookup"><span data-stu-id="ac1ee-105">Docker lets you get started quickly with an environment where you can try out the CLI to decide if it's right for you, or use our image as a base for your own deployment.</span></span>

## <a name="run-in-a-docker-container"></a><span data-ttu-id="ac1ee-106">Exécution dans un conteneur Docker</span><span class="sxs-lookup"><span data-stu-id="ac1ee-106">Run in a Docker container</span></span>

<span data-ttu-id="ac1ee-107">Installez l’interface de ligne de commande à l’aide de `docker run`.</span><span class="sxs-lookup"><span data-stu-id="ac1ee-107">Install the CLI using `docker run`.</span></span>

   ```bash
   docker run -it microsoft/azure-cli
   ```

> [!NOTE]
> <span data-ttu-id="ac1ee-108">Si vous souhaitez sélectionner les clés SSH à partir de votre environnement utilisateur, vous pouvez utiliser `-v ${HOME}:/root` pour monter $HOME en tant que `/root`.</span><span class="sxs-lookup"><span data-stu-id="ac1ee-108">If you want to pick up the SSH keys from your user environment, you can use `-v ${HOME}:/root` to mount $HOME as `/root`.</span></span>

> ```bash
> docker run -it -v ${HOME}:/root microsoft/azure-cli
> ```

<span data-ttu-id="ac1ee-109">L’interface de ligne de commande est installé sur l’image en tant que commande `az` dans `/usr/local/bin`.</span><span class="sxs-lookup"><span data-stu-id="ac1ee-109">The CLI is installed on the image as the `az` command in `/usr/local/bin`.</span></span> <span data-ttu-id="ac1ee-110">Pour vous connecter, exécutez la commande [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="ac1ee-110">To log in, run the [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="ac1ee-111">Pour en savoir plus sur les différentes méthodes de connexion, consultez [Se connecter avec Azure CLI 2.0](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="ac1ee-111">To learn more about different login methods, see [Log in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>


## <a name="update-docker-image"></a><span data-ttu-id="ac1ee-112">Mise à jour d’une image Docker</span><span class="sxs-lookup"><span data-stu-id="ac1ee-112">Update Docker image</span></span>

<span data-ttu-id="ac1ee-113">La mise à jour avec Docker nécessite l’extraction de la nouvelle image et la recréation de tous les conteneurs existants.</span><span class="sxs-lookup"><span data-stu-id="ac1ee-113">Updating with Docker requires both pulling the new image and re-creating any existing containers.</span></span> <span data-ttu-id="ac1ee-114">Pour cette raison, évitez d’utiliser un conteneur hébergeant l’interface de ligne de commande comme magasin de données.</span><span class="sxs-lookup"><span data-stu-id="ac1ee-114">For this reason you should try to avoid using a container that hosts the CLI as a data store.</span></span>

<span data-ttu-id="ac1ee-115">Mettre à jour votre image locale avec `docker pull`.</span><span class="sxs-lookup"><span data-stu-id="ac1ee-115">Update your local image with `docker pull`.</span></span>

```bash
docker pull microsoft/azure-cli
```

## <a name="uninstall-docker-image"></a><span data-ttu-id="ac1ee-116">Désinstallation d’une image Docker</span><span class="sxs-lookup"><span data-stu-id="ac1ee-116">Uninstall Docker image</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="ac1ee-117">Après l’arrêt de tous les conteneurs exécutant l’image de l’interface CLI, supprimez-la.</span><span class="sxs-lookup"><span data-stu-id="ac1ee-117">After halting any containers running the CLI image, remove it.</span></span>

```bash
docker rmi microsoft/azure-cli
```
