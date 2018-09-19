---
title: Bien démarrer avec Azure CLI 2.0
description: Commencez à utiliser Azure CLI 2.0 en apprenant les commandes de base.
keywords: Azure CLI, aide CLI, aide Azure, requête, automatisation,
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/07/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 165da295d187edf7dbc19a332670fd49d8f8bdd5
ms.sourcegitcommit: 0e688704889fc88b91588bb6678a933c2d54f020
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/11/2018
ms.locfileid: "44388556"
---
# <a name="get-started-with-azure-cli-20"></a><span data-ttu-id="f4658-104">Bien démarrer avec Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="f4658-104">Get started with Azure CLI 2.0</span></span>

<span data-ttu-id="f4658-105">Bienvenue dans Azure CLI 2.0 !</span><span class="sxs-lookup"><span data-stu-id="f4658-105">Welcome to the Azure CLI 2.0!</span></span> <span data-ttu-id="f4658-106">L’interface CLI est un outil conçu pour vous aider à utiliser rapidement et efficacement les services Azure, en mettant l’accent sur l’automatisation.</span><span class="sxs-lookup"><span data-stu-id="f4658-106">The CLI is a tool designed to get you working quickly and efficiently with Azure services, with an emphasis on automation.</span></span> <span data-ttu-id="f4658-107">Cet article présente les fonctionnalités de l’interface CLI et des liens vers des ressources qui vous aideront à être productif.</span><span class="sxs-lookup"><span data-stu-id="f4658-107">This article introduces features of the CLI and links out to resources that help you be productive.</span></span>

## <a name="install-and-sign-in"></a><span data-ttu-id="f4658-108">Installation et connexion</span><span class="sxs-lookup"><span data-stu-id="f4658-108">Install and sign in</span></span>

<span data-ttu-id="f4658-109">Si ce n’est pas déjà fait, [installez l’interface CLI](install-azure-cli.md) ou essayez [Azure Cloud Shell](/azure/cloud-shell/overview).</span><span class="sxs-lookup"><span data-stu-id="f4658-109">If you haven't already, [install the CLI](install-azure-cli.md) or try out the [Azure Cloud Shell](/azure/cloud-shell/overview).</span></span>

<span data-ttu-id="f4658-110">Avant d’utiliser les commandes CLI avec une installation locale, vous devez vous connecter avec la commande [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="f4658-110">Before using any CLI commands with a local install, you need to sign in with [az login](/cli/azure/reference-index#az-login).</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="f4658-111">Il existe des méthodes pour se connecter de manière non interactive, qui sont traitées en détail dans [Se connecter avec Azure CLI 2.0](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="f4658-111">There are ways to sign in non-interactively, which are covered in detail in [Sign in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

## <a name="common-commands"></a><span data-ttu-id="f4658-112">Commandes courantes</span><span class="sxs-lookup"><span data-stu-id="f4658-112">Common commands</span></span>

<span data-ttu-id="f4658-113">Ce tableau répertorie certaines commandes courantes utilisées dans l’interface CLI ainsi que des liens vers leur documentation de référence.</span><span class="sxs-lookup"><span data-stu-id="f4658-113">This table lists some common commands used in the CLI and links to their reference documentation.</span></span>

| <span data-ttu-id="f4658-114">Type de ressource</span><span class="sxs-lookup"><span data-stu-id="f4658-114">Resource type</span></span> | <span data-ttu-id="f4658-115">Groupe de commandes Azure CLI</span><span class="sxs-lookup"><span data-stu-id="f4658-115">Azure CLI command group</span></span> |
|---------------|-------------------------|
| [<span data-ttu-id="f4658-116">Groupe de ressources</span><span class="sxs-lookup"><span data-stu-id="f4658-116">Resource group</span></span>](/azure/azure-resource-manager/resource-group-overview) | [<span data-ttu-id="f4658-117">az group</span><span class="sxs-lookup"><span data-stu-id="f4658-117">az group</span></span>](/cli/azure/group) |
| [<span data-ttu-id="f4658-118">Machines virtuelles</span><span class="sxs-lookup"><span data-stu-id="f4658-118">Virtual machines</span></span>](/azure/virtual-machines) | [<span data-ttu-id="f4658-119">az vm</span><span class="sxs-lookup"><span data-stu-id="f4658-119">az vm</span></span>](/cli/azure/vm) |
| [<span data-ttu-id="f4658-120">Comptes de stockage</span><span class="sxs-lookup"><span data-stu-id="f4658-120">Storage accounts</span></span>](/azure/storage/common/storage-introduction) | [<span data-ttu-id="f4658-121">az storage account</span><span class="sxs-lookup"><span data-stu-id="f4658-121">az storage account</span></span>](/cli/azure/storage/account) |
| [<span data-ttu-id="f4658-122">Key Vault</span><span class="sxs-lookup"><span data-stu-id="f4658-122">Key Vault</span></span>](/azure/key-vault/key-vault-whatis) | [<span data-ttu-id="f4658-123">az keyvault</span><span class="sxs-lookup"><span data-stu-id="f4658-123">az keyvault</span></span>](/cli/azure/keyvault) |
| [<span data-ttu-id="f4658-124">Applications web</span><span class="sxs-lookup"><span data-stu-id="f4658-124">Web applications</span></span>](/azure/app-service) | [<span data-ttu-id="f4658-125">az webapp</span><span class="sxs-lookup"><span data-stu-id="f4658-125">az webapp</span></span>](/cli/azure/webapp) |
| [<span data-ttu-id="f4658-126">Bases de données SQL</span><span class="sxs-lookup"><span data-stu-id="f4658-126">SQL databases</span></span>](/azure/sql-database) | [<span data-ttu-id="f4658-127">az sql server</span><span class="sxs-lookup"><span data-stu-id="f4658-127">az sql server</span></span>](/cli/azure/sql/server) |
| [<span data-ttu-id="f4658-128">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="f4658-128">CosmosDB</span></span>](/azure/cosmos-db) | [<span data-ttu-id="f4658-129">az cosmosdb</span><span class="sxs-lookup"><span data-stu-id="f4658-129">az cosmosdb</span></span>](/cli/azure/cosmosdb) |

## <a name="finding-commands"></a><span data-ttu-id="f4658-130">Recherche de commandes</span><span class="sxs-lookup"><span data-stu-id="f4658-130">Finding commands</span></span>

<span data-ttu-id="f4658-131">Les commandes dans l’interface CLI sont classées par _commandes_ de _groupes_.</span><span class="sxs-lookup"><span data-stu-id="f4658-131">Commands in the CLI are organized as _commands_ of _groups_.</span></span> <span data-ttu-id="f4658-132">Chaque groupe représente un service Azure, et les commandes agissent sur ce service.</span><span class="sxs-lookup"><span data-stu-id="f4658-132">Each group represents an Azure service, and commands operate on that service.</span></span>

<span data-ttu-id="f4658-133">Pour rechercher des commandes, utilisez la commande [az find](/cli/azure/reference-index#az-find).</span><span class="sxs-lookup"><span data-stu-id="f4658-133">To search for commands, use [az find](/cli/azure/reference-index#az-find).</span></span> <span data-ttu-id="f4658-134">Par exemple, pour rechercher des noms de commandes contenant `secret`, utilisez la commande suivante :</span><span class="sxs-lookup"><span data-stu-id="f4658-134">For example, to search for command names containing `secret`, use the following command:</span></span>

```azurecli-interactive
az find -q secret
```

<span data-ttu-id="f4658-135">Utilisez l’argument `--help` pour obtenir une liste complète des commandes et des sous-groupes d’un groupe.</span><span class="sxs-lookup"><span data-stu-id="f4658-135">Use the `--help` argument to get a complete list of commands and subgroups of a group.</span></span> <span data-ttu-id="f4658-136">Par exemple, pour trouver les commandes CLI pour fonctionner avec des groupes de sécurité réseau (NSG) :</span><span class="sxs-lookup"><span data-stu-id="f4658-136">For example, to find the CLI commands for working with Network Security Groups (NSGs):</span></span>

```azurecli-interactive
az network nsg --help
```

<span data-ttu-id="f4658-137">L’interface CLI dispose de la saisie semi-automatique via la touche Tab pour les commandes de l’interpréteur de commandes bash.</span><span class="sxs-lookup"><span data-stu-id="f4658-137">The CLI has full tab completion for commands under the bash shell.</span></span>

## <a name="globally-available-arguments"></a><span data-ttu-id="f4658-138">Arguments globalement disponibles</span><span class="sxs-lookup"><span data-stu-id="f4658-138">Globally available arguments</span></span>

<span data-ttu-id="f4658-139">Certains arguments sont disponibles pour chaque commande.</span><span class="sxs-lookup"><span data-stu-id="f4658-139">There are some arguments that are available for every command.</span></span>

* <span data-ttu-id="f4658-140">`--help` imprime les informations de référence CLI sur les commandes et leurs arguments, et répertorie les commandes et sous-groupes disponibles.</span><span class="sxs-lookup"><span data-stu-id="f4658-140">`--help` prints CLI reference information about commands and their arguments and lists available subgroups and commands.</span></span>
* <span data-ttu-id="f4658-141">`--output` modifie le format de sortie.</span><span class="sxs-lookup"><span data-stu-id="f4658-141">`--output` changes the output format.</span></span> <span data-ttu-id="f4658-142">Les formats de sortie disponibles sont `json`, `jsonc` (JSON coloré), `tsv` (valeurs séparées par des tabulations.), et `table` (tables ASCII lisibles).</span><span class="sxs-lookup"><span data-stu-id="f4658-142">The available output formats are `json`, `jsonc` (colorized JSON), `tsv` (Tab-Separated Values), and `table` (human-readable ASCII tables).</span></span> <span data-ttu-id="f4658-143">Par défaut, l’interface CLI génère `json`.</span><span class="sxs-lookup"><span data-stu-id="f4658-143">By default the CLI outputs `json`.</span></span> <span data-ttu-id="f4658-144">Pour en savoir plus sur les formats de sortie disponibles, consultez [Formats de sortie pour Azure CLI 2.0](format-output-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="f4658-144">To learn more about the available output formats, see [Output formats for Azure CLI 2.0](format-output-azure-cli.md).</span></span>
* <span data-ttu-id="f4658-145">`--query` utilise le [langage de requête JMESPath](http://jmespath.org/) pour filtrer la sortie retournée à partir des services Azure.</span><span class="sxs-lookup"><span data-stu-id="f4658-145">`--query` uses the [JMESPath query language](http://jmespath.org/) to filter the output returned from Azure services.</span></span> <span data-ttu-id="f4658-146">Pour en savoir plus sur les requêtes, consultez [Interroger des résultats de commande avec Azure CLI 2.0](query-azure-cli.md) et le [didacticiel JMESPath](http://jmespath.org/tutorial.html).</span><span class="sxs-lookup"><span data-stu-id="f4658-146">To learn To learn more about queries, see [Query command results with Azure CLI 2.0](query-azure-cli.md) and the [JMESPath tutorial](http://jmespath.org/tutorial.html).</span></span>
* <span data-ttu-id="f4658-147">`--verbose` imprime les informations sur les ressources créées dans Azure pendant une opération, et d’autres informations utiles.</span><span class="sxs-lookup"><span data-stu-id="f4658-147">`--verbose` prints information about resources created in Azure during an operation, and other useful information.</span></span>
* <span data-ttu-id="f4658-148">`--debug` imprime davantage d’informations sur les opérations CLI, utilisées pour le débogage.</span><span class="sxs-lookup"><span data-stu-id="f4658-148">`--debug` prints even more information about CLI operations, used for debugging purposes.</span></span> <span data-ttu-id="f4658-149">Si vous rencontrez un bogue, fournissez la sortie générée avec l’indicateur `--debug` lors de l’envoi d’un rapport de bogue.</span><span class="sxs-lookup"><span data-stu-id="f4658-149">If you find a bug, provide output generated with the `--debug` flag on when submitting a bug report.</span></span>

## <a name="interactive-mode"></a><span data-ttu-id="f4658-150">Mode interactif</span><span class="sxs-lookup"><span data-stu-id="f4658-150">Interactive mode</span></span>

<span data-ttu-id="f4658-151">L’interface CLI propose un mode interactif qui affiche automatiquement les informations d’aide et qui facilite la sélection de sous-commandes.</span><span class="sxs-lookup"><span data-stu-id="f4658-151">The CLI offers an interactive mode that automatically displays help information and makes it easier to select subcommands.</span></span> <span data-ttu-id="f4658-152">Vous pouvez entrer en mode interactif avec la commande [az interactive](/cli/azure/reference-index#az-interactive).</span><span class="sxs-lookup"><span data-stu-id="f4658-152">You enter interactive mode with the [az interactive](/cli/azure/reference-index#az-interactive) command.</span></span>

```azurecli-interactive
az interactive
```

<span data-ttu-id="f4658-153">Pour plus d’informations sur le mode interactif, consultez [Mode interactif Azure CLI 2.0](interactive-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="f4658-153">For more information on interactive mode, see [Azure CLI 2.0 Interactive Mode](interactive-azure-cli.md).</span></span>

<span data-ttu-id="f4658-154">Il existe également un [plug-in Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azurecli) qui propose une expérience interactive, comprenant l’autocomplétion et le survol de la documentation.</span><span class="sxs-lookup"><span data-stu-id="f4658-154">There's also a [Visual Studio Code plugin](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azurecli) that offers an interactive experience, including autocomplete and mouse-over documentation.</span></span>

## <a name="learn-cli-basics-with-quickstarts-and-tutorials"></a><span data-ttu-id="f4658-155">Apprendre les concepts de base CLI à l’aide des démarrages rapides et des didacticiels</span><span class="sxs-lookup"><span data-stu-id="f4658-155">Learn CLI basics with quickstarts and tutorials</span></span>

<span data-ttu-id="f4658-156">Pour vous aider à démarrer avec l’interface Azure CLI 2.0, essayez un didacticiel approfondi pour configurer les machines virtuelles et utiliser la puissance de l’interface CLI pour interroger les ressources Azure.</span><span class="sxs-lookup"><span data-stu-id="f4658-156">To get you started with the Azure CLI 2.0, try an in-depth tutorial for setting up virtual machines and using the power of the CLI to query Azure resources.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="f4658-157">Créer des machines virtuelles avec le didacticiel Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="f4658-157">Create virtual machines with the Azure CLI 2.0 tutorial</span></span>](azure-cli-vm-tutorial.yml)

<span data-ttu-id="f4658-158">Il existe également des guides de démarrage rapide pour les autres services populaires.</span><span class="sxs-lookup"><span data-stu-id="f4658-158">There are also quickstarts for other popular services.</span></span>

* [<span data-ttu-id="f4658-159">Créer un compte de stockage à l’aide d’Azure CLI</span><span class="sxs-lookup"><span data-stu-id="f4658-159">Create a storage account using the Azure CLI</span></span>](/azure/storage/common/storage-quickstart-create-storage-account-cli)
* [<span data-ttu-id="f4658-160">Transférer des objets vers/à partir du stockage blob Azure à l’aide de l’interface CLI</span><span class="sxs-lookup"><span data-stu-id="f4658-160">Transfer objects to/from Azure Blob storage using the CLI</span></span>](/azure/storage/blobs/storage-quickstart-blobs-cli)
* [<span data-ttu-id="f4658-161">Créer une base de données SQL Azure unique à l’aide d’Azure CLI</span><span class="sxs-lookup"><span data-stu-id="f4658-161">Create a single Azure SQL database using the Azure CLI</span></span>](/azure/sql-database/sql-database-get-started-cli)
* [<span data-ttu-id="f4658-162">Créer un serveur de base de données Azure pour MySQL à l’aide d’Azure CLI</span><span class="sxs-lookup"><span data-stu-id="f4658-162">Create an Azure Database for MySQL server using the Azure CLI</span></span>](/azure/mysql/quickstart-create-mysql-server-database-using-azure-cli)
* [<span data-ttu-id="f4658-163">Création d’une instance d’Azure Database pour PostgreSQL à l’aide de la CLI Azure</span><span class="sxs-lookup"><span data-stu-id="f4658-163">Create an Azure Database for PostgreSQL using the Azure CLI</span></span>](/azure/postgresql/quickstart-create-server-database-azure-cli)
* [<span data-ttu-id="f4658-164">Créer une application web Python dans Azure</span><span class="sxs-lookup"><span data-stu-id="f4658-164">Create a Python web app in Azure</span></span>](/azure/app-service/app-service-web-get-started-python)
* [<span data-ttu-id="f4658-165">Exécuter une image Docker Hub personnalisée dans Azure Web App for Containers</span><span class="sxs-lookup"><span data-stu-id="f4658-165">Run a custom Docker Hub image in Azure Web Apps for Containers</span></span>](/azure/app-service/containers/quickstart-custom-docker-image)

## <a name="give-feedback"></a><span data-ttu-id="f4658-166">Envoyer des commentaires</span><span class="sxs-lookup"><span data-stu-id="f4658-166">Give feedback</span></span>

<span data-ttu-id="f4658-167">N’hésitez pas à nous faire part de vos commentaires au sujet de l’interface CLI pour nous aider à l’améliorer et à résoudre les bogues.</span><span class="sxs-lookup"><span data-stu-id="f4658-167">We welcome your feedback for the CLI to help us make improvements and resolve bugs.</span></span> <span data-ttu-id="f4658-168">Vous pouvez [signaler un problème sur Github](https://github.com/azure/azure-cli/issues) ou utiliser les fonctionnalités intégrées de l’interface CLI pour laisser un commentaire général avec la commande [az feedback](/cli/azure/reference-index#az-feedback).</span><span class="sxs-lookup"><span data-stu-id="f4658-168">You can [file an issue on Github](https://github.com/azure/azure-cli/issues) or use the built-in features of the CLI to leave general feedback with the [az feedback](/cli/azure/reference-index#az-feedback) command.</span></span>

```azurecli-interactive
az feedback
```
