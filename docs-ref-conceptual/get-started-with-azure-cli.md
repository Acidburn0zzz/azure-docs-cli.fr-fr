---
title: Bien démarrer avec Azure CLI 2.0
description: Commencez à utiliser Azure CLI 2.0 en apprenant les commandes de base.
keywords: Azure CLI, aide CLI, aide Azure, requête, automatisation,
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/16/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 0c7746e70125dcc1678ed19f93322efea8a2b01b
ms.sourcegitcommit: 8b4629a42ceecf30c1efbc6fdddf512f4dddfab0
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/18/2018
ms.locfileid: "34306095"
---
# <a name="get-started-with-azure-cli-20"></a><span data-ttu-id="07593-104">Bien démarrer avec Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="07593-104">Get started with Azure CLI 2.0</span></span>

<span data-ttu-id="07593-105">Bienvenue dans Azure CLI 2.0 !</span><span class="sxs-lookup"><span data-stu-id="07593-105">Welcome to the Azure CLI 2.0!</span></span> <span data-ttu-id="07593-106">L’interface CLI est un outil conçu pour vous aider à utiliser rapidement et efficacement les services Azure, en mettant l’accent sur l’automatisation.</span><span class="sxs-lookup"><span data-stu-id="07593-106">The CLI is a tool designed to get you working quickly and efficiently with Azure services, with an emphasis on automation.</span></span> <span data-ttu-id="07593-107">Cet article présente les fonctionnalités de l’interface CLI et des liens vers des ressources qui vous aideront à être productif.</span><span class="sxs-lookup"><span data-stu-id="07593-107">This article introduces features of the CLI and links out to resources that help you be productive.</span></span>

## <a name="install-and-log-in"></a><span data-ttu-id="07593-108">Installer et se connecter</span><span class="sxs-lookup"><span data-stu-id="07593-108">Install and log in</span></span>

<span data-ttu-id="07593-109">Si ce n’est pas déjà fait, [installez l’interface CLI](install-azure-cli.md) ou essayez [Azure Cloud Shell](/azure/cloud-shell/overview).</span><span class="sxs-lookup"><span data-stu-id="07593-109">If you haven't already, [install the CLI](install-azure-cli.md) or try out the [Azure Cloud Shell](/azure/cloud-shell/overview).</span></span>

<span data-ttu-id="07593-110">Avant d’utiliser les commandes CLI avec une installation locale, vous devez vous connecter avec la commande [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="07593-110">Before using any CLI commands with a local install, you need to log in with [az login](/cli/azure/reference-index#az-login).</span></span>

```azurecli
az login
```

<span data-ttu-id="07593-111">Cette commande vous invite à vous connecter avec un code d’authentification via un site Web.</span><span class="sxs-lookup"><span data-stu-id="07593-111">This command prompts you to log in with an authentication code via a website.</span></span> <span data-ttu-id="07593-112">Il existe des méthodes pour se connecter de manière non interactive, qui sont traitées en détail dans [Se connecter avec Azure CLI 2.0](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="07593-112">There are ways to log in non-interactively, which are covered in detail in [Log in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

## <a name="common-commands"></a><span data-ttu-id="07593-113">Commandes courantes</span><span class="sxs-lookup"><span data-stu-id="07593-113">Common commands</span></span>

<span data-ttu-id="07593-114">Ce tableau répertorie quelques commandes courantes utilisées dans les liens CLI vers leurs pages de documentation dans la référence.</span><span class="sxs-lookup"><span data-stu-id="07593-114">This table lists a few of the common commands used in the CLI links out to their documentation pages in the reference.</span></span>
<span data-ttu-id="07593-115">Toutes les sous-commandes de ces groupes et leur documentation peuvent être consultées dans la référence en ligne ou avec l’argument `--help`.</span><span class="sxs-lookup"><span data-stu-id="07593-115">All subcommands of these groups and their documentation can be looked up in online reference or with the `--help` argument.</span></span>

| <span data-ttu-id="07593-116">Type de ressource</span><span class="sxs-lookup"><span data-stu-id="07593-116">Resource type</span></span> | <span data-ttu-id="07593-117">Groupe de commandes Azure CLI</span><span class="sxs-lookup"><span data-stu-id="07593-117">Azure CLI command group</span></span> |
|---------------|-------------------------|
| [<span data-ttu-id="07593-118">Groupe de ressources</span><span class="sxs-lookup"><span data-stu-id="07593-118">Resource group</span></span>](/azure/azure-resource-manager/resource-group-overview) | [<span data-ttu-id="07593-119">az group</span><span class="sxs-lookup"><span data-stu-id="07593-119">az group</span></span>](/cli/azure/group) |
| [<span data-ttu-id="07593-120">Machines virtuelles</span><span class="sxs-lookup"><span data-stu-id="07593-120">Virtual machines</span></span>](/azure/virtual-machines) | [<span data-ttu-id="07593-121">az vm</span><span class="sxs-lookup"><span data-stu-id="07593-121">az vm</span></span>](/cli/azure/vm) |
| [<span data-ttu-id="07593-122">Comptes de stockage</span><span class="sxs-lookup"><span data-stu-id="07593-122">Storage accounts</span></span>](/azure/storage/common/storage-introduction) | [<span data-ttu-id="07593-123">az storage account</span><span class="sxs-lookup"><span data-stu-id="07593-123">az storage account</span></span>](/cli/azure/storage/account) |
| [<span data-ttu-id="07593-124">Key Vault</span><span class="sxs-lookup"><span data-stu-id="07593-124">Key Vault</span></span>](/azure/key-vault/key-vault-whatis) | [<span data-ttu-id="07593-125">az keyvault</span><span class="sxs-lookup"><span data-stu-id="07593-125">az keyvault</span></span>](/cli/azure/keyvault) |
| [<span data-ttu-id="07593-126">Applications web</span><span class="sxs-lookup"><span data-stu-id="07593-126">Web applications</span></span>](/azure/ap-service) | [<span data-ttu-id="07593-127">az webapp</span><span class="sxs-lookup"><span data-stu-id="07593-127">az webapp</span></span>](/cli/azure/webapp) |
| [<span data-ttu-id="07593-128">Bases de données SQL</span><span class="sxs-lookup"><span data-stu-id="07593-128">SQL databases</span></span>](/azure/sql-database) | [<span data-ttu-id="07593-129">az sql server</span><span class="sxs-lookup"><span data-stu-id="07593-129">az sql server</span></span>](/cli/azure/sql/server) |
| [<span data-ttu-id="07593-130">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="07593-130">CosmosDB</span></span>](/azure/cosmos-db) | [<span data-ttu-id="07593-131">az cosmosdb</span><span class="sxs-lookup"><span data-stu-id="07593-131">az cosmosdb</span></span>](/cli/azure/cosmosdb) |

## <a name="finding-commands"></a><span data-ttu-id="07593-132">Recherche de commandes</span><span class="sxs-lookup"><span data-stu-id="07593-132">Finding commands</span></span>

<span data-ttu-id="07593-133">Les commandes de l’interface CLI sont fournies en tant que _sous-commandes_ de _groupes_.</span><span class="sxs-lookup"><span data-stu-id="07593-133">Commands in the CLI are provided as _subcommands_ of _groups_.</span></span>
<span data-ttu-id="07593-134">Chaque groupe représente un service fourni par Azure, et les sous-groupes divisent les commandes pour ces services en regroupements logiques.</span><span class="sxs-lookup"><span data-stu-id="07593-134">Each group represents a service provided by Azure, and the subgroups divide commands for these services into logical groupings.</span></span>

<span data-ttu-id="07593-135">Pour rechercher des commandes, utilisez la commande [az find](/cli/azure/reference-index#az-find).</span><span class="sxs-lookup"><span data-stu-id="07593-135">To search for commands, use [az find](/cli/azure/reference-index#az-find).</span></span> <span data-ttu-id="07593-136">Par exemple, pour rechercher des noms de commandes contenant `secret`, utilisez la commande suivante :</span><span class="sxs-lookup"><span data-stu-id="07593-136">For example, to search for command names containing `secret`, use the following command:</span></span>

```azurecli-interactive
az find -q secret
```

<span data-ttu-id="07593-137">Si vous savez avec quel groupe de commandes vous souhaitez travailler, l’argument `--help` constitue peut-être un meilleur choix.</span><span class="sxs-lookup"><span data-stu-id="07593-137">If you know which group of commands you want to work with, the `--help` argument may be a better choice.</span></span> <span data-ttu-id="07593-138">Il n’affiche pas que des informations détaillées pour une commande, mais lorsqu’il est utilisé avec un groupe de commandes, il affiche toutes les sous-commandes disponibles.</span><span class="sxs-lookup"><span data-stu-id="07593-138">This displays not just detailed information for a command, but when used with a command group, displays all of the available subcommands.</span></span> <span data-ttu-id="07593-139">Par exemple, lorsque vous travaillez avec des groupes de sécurité réseau (NSG), vous pouvez trouver les sous-groupes et commandes NSG disponibles.</span><span class="sxs-lookup"><span data-stu-id="07593-139">For example, when working with Network Security Groups (NSGs) you can find the available NSG subgroups and commands.</span></span>

```azurecli-interactive
az network nsg --help
```

<span data-ttu-id="07593-140">L’interface CLI dispose de la saisie semi-automatique via la touche Tab pour les commandes de l’interpréteur de commandes bash.</span><span class="sxs-lookup"><span data-stu-id="07593-140">The CLI has full tab completion for commands under the bash shell.</span></span>

## <a name="globally-available-arguments"></a><span data-ttu-id="07593-141">Arguments globalement disponibles</span><span class="sxs-lookup"><span data-stu-id="07593-141">Globally available arguments</span></span>

<span data-ttu-id="07593-142">Certains arguments sont disponibles pour chaque commande.</span><span class="sxs-lookup"><span data-stu-id="07593-142">There are some arguments that are available for every command.</span></span>

* <span data-ttu-id="07593-143">`--help` imprime les informations de référence CLI sur les commandes et leurs arguments, et répertorie les commandes et sous-groupes disponibles.</span><span class="sxs-lookup"><span data-stu-id="07593-143">`--help` prints CLI reference information about commands and their arguments and lists available subgroups and commands.</span></span>
* <span data-ttu-id="07593-144">`--output` modifie le format de sortie.</span><span class="sxs-lookup"><span data-stu-id="07593-144">`--output` changes the output format.</span></span> <span data-ttu-id="07593-145">Les formats de sortie disponibles sont `json`, `jsonc` (JSON coloré), `tsv` (valeurs séparées par des tabulations.), et `table` (tables ASCII lisibles).</span><span class="sxs-lookup"><span data-stu-id="07593-145">The available output formats are `json`, `jsonc` (colorized JSON), `tsv` (Tab-Separated Values), and `table` (human-readable ASCII tables).</span></span> <span data-ttu-id="07593-146">Par défaut, l’interface CLI génère `json`.</span><span class="sxs-lookup"><span data-stu-id="07593-146">By default the CLI outputs `json`.</span></span> <span data-ttu-id="07593-147">Pour en savoir plus sur les formats de sortie disponibles, consultez [Formats de sortie pour Azure CLI 2.0](format-output-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="07593-147">To learn more about the available output formats, see [Output formats for Azure CLI 2.0](format-output-azure-cli.md).</span></span>
* <span data-ttu-id="07593-148">`--query` utilise le [langage de requête JMESPath](http://jmespath.org/) pour filtrer la sortie retournée à partir des services Azure.</span><span class="sxs-lookup"><span data-stu-id="07593-148">`--query` uses the [JMESPath query language](http://jmespath.org/) to filter the output returned from Azure services.</span></span> <span data-ttu-id="07593-149">Pour en savoir plus sur les requêtes, consultez [Interroger des résultats de commande avec Azure CLI 2.0](query-azure-cli.md) et le [didacticiel JMESPath](http://jmespath.org/tutorial.html).</span><span class="sxs-lookup"><span data-stu-id="07593-149">To learn To learn more about queries, see [Query command results with Azure CLI 2.0](query-azure-cli.md) and the [JMESPath tutorial](http://jmespath.org/tutorial.html).</span></span>
* <span data-ttu-id="07593-150">`--verbose` imprime les informations sur les ressources créées dans Azure pendant une opération, et d’autres informations utiles.</span><span class="sxs-lookup"><span data-stu-id="07593-150">`--verbose` prints information about resources created in Azure during an operation, and other useful information.</span></span>
* <span data-ttu-id="07593-151">`--debug` imprime davantage d’informations sur les opérations CLI, utilisées pour le débogage.</span><span class="sxs-lookup"><span data-stu-id="07593-151">`--debug` prints even more information about CLI operations, used for debugging purposes.</span></span> <span data-ttu-id="07593-152">Si vous rencontrez un bogue, fournissez la sortie générée avec l’indicateur `--debug` lors de l’envoi d’un rapport de bogue.</span><span class="sxs-lookup"><span data-stu-id="07593-152">If you encounter a bug, provide output generated with the `--debug` flag on when submitting a bug report.</span></span>


## <a name="interactive-mode"></a><span data-ttu-id="07593-153">Mode interactif</span><span class="sxs-lookup"><span data-stu-id="07593-153">Interactive mode</span></span>

<span data-ttu-id="07593-154">L’interface CLI propose un mode interactif qui affiche automatiquement les informations d’aide et qui facilite la sélection de sous-commandes.</span><span class="sxs-lookup"><span data-stu-id="07593-154">The CLI offers an interactive mode that automatically displays help information and makes it easier to select subcommands.</span></span> <span data-ttu-id="07593-155">Vous pouvez entrer en mode interactif avec la commande [az interactive](/cli/azure/reference-index#az-interactive).</span><span class="sxs-lookup"><span data-stu-id="07593-155">You enter interactive mode with the [az interactive](/cli/azure/reference-index#az-interactive) command.</span></span>

```azurecli-interactive
az interactive
```

<span data-ttu-id="07593-156">Pour plus d’informations sur le mode interactif, consultez [Mode interactif Azure CLI 2.0](interactive-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="07593-156">For more information on interactive mode, see [Azure CLI 2.0 Interactive Mode](interactive-azure-cli.md).</span></span>

<span data-ttu-id="07593-157">Il existe également un [plug-in Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azurecli) qui propose une expérience interactive, comprenant la saisie semi-automatique et le survol de la documentation.</span><span class="sxs-lookup"><span data-stu-id="07593-157">There is also a [Visual Studio Code plugin](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azurecli) that offers an interactive experience, including autocomplete and mouse-over documentation.</span></span>

## <a name="learn-cli-basics-with-quickstarts-and-tutorials"></a><span data-ttu-id="07593-158">Apprendre les concepts de base CLI à l’aide des démarrages rapides et des didacticiels</span><span class="sxs-lookup"><span data-stu-id="07593-158">Learn CLI basics with quickstarts and tutorials</span></span>

<span data-ttu-id="07593-159">Pour vous aider à démarrer avec l’interface Azure CLI 2.0, essayez un didacticiel approfondi pour configurer les machines virtuelles et utiliser la puissance de l’interface CLI pour interroger les ressources Azure.</span><span class="sxs-lookup"><span data-stu-id="07593-159">To get you started with the Azure CLI 2.0, try an in-depth tutorial for setting up virtual machines and using the power of the CLI to query Azure resources.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="07593-160">Créer des machines virtuelles avec le didacticiel Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="07593-160">Create virtual machines with the Azure CLI 2.0 tutorial</span></span>](azure-cli-vm-tutorial.yml)

<span data-ttu-id="07593-161">Si vous préférez vous concentrer sur d’autres services, il existe plusieurs Démarrages rapides pour les services Azure qui utilisent l’interface CLI.</span><span class="sxs-lookup"><span data-stu-id="07593-161">If you would rather focus on other services, there are a variety of quickstarts for Azure services that use the CLI.</span></span>

* [<span data-ttu-id="07593-162">Créer un compte de stockage à l’aide d’Azure CLI</span><span class="sxs-lookup"><span data-stu-id="07593-162">Create a storage account using the Azure CLI</span></span>](/azure/storage/common/storage-quickstart-create-storage-account-cli)
* [<span data-ttu-id="07593-163">Transférer des objets vers/à partir du stockage blob Azure à l’aide de l’interface CLI</span><span class="sxs-lookup"><span data-stu-id="07593-163">Transfer objects to/from Azure Blob storage using the CLI</span></span>](/azure/storage/blobs/storage-quickstart-blobs-cli)
* [<span data-ttu-id="07593-164">Créer une base de données SQL Azure unique à l’aide d’Azure CLI</span><span class="sxs-lookup"><span data-stu-id="07593-164">Create a single Azure SQL database using the Azure CLI</span></span>](/azure/sql-database/sql-database-get-started-cli)
* [<span data-ttu-id="07593-165">Créer un serveur de base de données Azure pour MySQL à l’aide d’Azure CLI</span><span class="sxs-lookup"><span data-stu-id="07593-165">Create an Azure Database for MySQL server using the Azure CLI</span></span>](/azure/mysql/quickstart-create-mysql-server-database-using-azure-cli)
* [<span data-ttu-id="07593-166">Création d’une instance d’Azure Database pour PostgreSQL à l’aide de la CLI Azure</span><span class="sxs-lookup"><span data-stu-id="07593-166">Create an Azure Database for PostgreSQL using the Azure CLI</span></span>](/azure/postgresql/quickstart-create-server-database-azure-cli)
* [<span data-ttu-id="07593-167">Créer une application web Python dans Azure</span><span class="sxs-lookup"><span data-stu-id="07593-167">Create a Python web app in Azure</span></span>](/azure/app-service/app-service-web-get-started-python)
* [<span data-ttu-id="07593-168">Exécuter une image Docker Hub personnalisée dans Azure Web App for Containers</span><span class="sxs-lookup"><span data-stu-id="07593-168">Run a custom Docker Hub image in Azure Web Apps for Containers</span></span>](/azure/app-service/containers/quickstart-custom-docker-image)

## <a name="give-feedback"></a><span data-ttu-id="07593-169">Envoyer des commentaires</span><span class="sxs-lookup"><span data-stu-id="07593-169">Give feedback</span></span>

<span data-ttu-id="07593-170">N’hésitez pas à nous faire part de vos commentaires au sujet de l’interface CLI pour nous aider à l’améliorer et à résoudre les bogues.</span><span class="sxs-lookup"><span data-stu-id="07593-170">We welcome your feedback for the CLI to help us make improvements and resolve bugs.</span></span> <span data-ttu-id="07593-171">Vous pouvez [signaler un problème sur Github](https://github.com/azure/azure-cli/issues) ou utiliser les fonctionnalités intégrées de l’interface CLI pour laisser un commentaire général avec la commande [az feedback](/cli/azure/reference-index#az-feedback).</span><span class="sxs-lookup"><span data-stu-id="07593-171">You can [file an issue on Github](https://github.com/azure/azure-cli/issues) or use the built-in features of the CLI to leave general feedback with the [az feedback](/cli/azure/reference-index#az-feedback) command.</span></span>

```azurecli-interactive
az feedback
```
