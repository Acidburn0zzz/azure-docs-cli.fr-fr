---
title: Prise en main d’Azure CLI
description: Commencez à utiliser Azure CLI en apprenant les commandes de base.
keywords: Azure CLI, aide CLI, aide Azure, requête, automatisation,
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/07/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: b018f41824946dca36d0b806de0dd32a335a15b5
ms.sourcegitcommit: 1987a39809f9865034b27130e56f30b2bd1eb72c
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/19/2019
ms.locfileid: "56422015"
---
# <a name="get-started-with-azure-cli"></a><span data-ttu-id="18906-104">Prise en main d’Azure CLI</span><span class="sxs-lookup"><span data-stu-id="18906-104">Get started with Azure CLI</span></span>

<span data-ttu-id="18906-105">Bienvenue dans Azure CLI !</span><span class="sxs-lookup"><span data-stu-id="18906-105">Welcome to the Azure CLI!</span></span> <span data-ttu-id="18906-106">L’interface CLI est un outil conçu pour vous aider à utiliser rapidement et efficacement les services Azure, en mettant l’accent sur l’automatisation.</span><span class="sxs-lookup"><span data-stu-id="18906-106">The CLI is a tool designed to get you working quickly and efficiently with Azure services, with an emphasis on automation.</span></span> <span data-ttu-id="18906-107">Cet article présente les fonctionnalités de l’interface CLI et des liens vers des ressources qui vous aideront à être productif.</span><span class="sxs-lookup"><span data-stu-id="18906-107">This article introduces features of the CLI and links out to resources that help you be productive.</span></span>

## <a name="install-or-run-in-azure-cloud-shell"></a><span data-ttu-id="18906-108">Installer ou exécuter dans Azure Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="18906-108">Install or run in Azure Cloud Shell</span></span>

<span data-ttu-id="18906-109">Pour commencer avec l’interface CLI, le plus simple est de l’exécuter dans un environnement Azure Cloud Shell via votre navigateur.</span><span class="sxs-lookup"><span data-stu-id="18906-109">The easiest way to get started with the Azure CLI is by running it in an Azure Cloud Shell environment through your browser.</span></span> <span data-ttu-id="18906-110">Pour en savoir plus sur Cloud Shell, consultez [Démarrage rapide de Bash dans Azure Cloud Shell](/azure/cloud-shell/quickstart).</span><span class="sxs-lookup"><span data-stu-id="18906-110">To learn about Cloud Shell, see  [Quickstart for Bash in Azure Cloud Shell](/azure/cloud-shell/quickstart).</span></span>

<span data-ttu-id="18906-111">Lorsque vous êtes prêt à installer l’interface CLI, consultez les [instructions d’installation](install-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="18906-111">When you're ready to install the CLI, see the [installation instructions](install-azure-cli.md).</span></span>

<span data-ttu-id="18906-112">Après avoir installé l’interface CLI pour la première fois, vérifiez qu’elle est bien installée et que vous disposez de la version appropriée en exécutant `az --version`.</span><span class="sxs-lookup"><span data-stu-id="18906-112">After installing the CLI for the first time, check that it's installed and you've got the correct version by running `az --version`.</span></span>

## <a name="sign-in"></a><span data-ttu-id="18906-113">Se connecter</span><span class="sxs-lookup"><span data-stu-id="18906-113">Sign in</span></span>

<span data-ttu-id="18906-114">Avant d’utiliser les commandes CLI avec une installation locale, vous devez vous connecter avec la commande [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="18906-114">Before using any CLI commands with a local install, you need to sign in with [az login](/cli/azure/reference-index#az-login).</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="18906-115">Il existe des méthodes pour se connecter de manière non interactive, qui sont dévelopées en détail dans [Se connecter avec Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="18906-115">There are ways to sign in non-interactively, which are covered in detail in [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="common-commands"></a><span data-ttu-id="18906-116">Commandes courantes</span><span class="sxs-lookup"><span data-stu-id="18906-116">Common commands</span></span>

<span data-ttu-id="18906-117">Ce tableau répertorie certaines commandes courantes utilisées dans l’interface CLI ainsi que des liens vers leur documentation de référence.</span><span class="sxs-lookup"><span data-stu-id="18906-117">This table lists some common commands used in the CLI and links to their reference documentation.</span></span>

| <span data-ttu-id="18906-118">Type de ressource</span><span class="sxs-lookup"><span data-stu-id="18906-118">Resource type</span></span> | <span data-ttu-id="18906-119">Groupe de commandes Azure CLI</span><span class="sxs-lookup"><span data-stu-id="18906-119">Azure CLI command group</span></span> |
|---------------|-------------------------|
| [<span data-ttu-id="18906-120">Groupe de ressources</span><span class="sxs-lookup"><span data-stu-id="18906-120">Resource group</span></span>](/azure/azure-resource-manager/resource-group-overview) | [<span data-ttu-id="18906-121">az group</span><span class="sxs-lookup"><span data-stu-id="18906-121">az group</span></span>](/cli/azure/group) |
| [<span data-ttu-id="18906-122">Machines virtuelles</span><span class="sxs-lookup"><span data-stu-id="18906-122">Virtual machines</span></span>](/azure/virtual-machines) | [<span data-ttu-id="18906-123">az vm</span><span class="sxs-lookup"><span data-stu-id="18906-123">az vm</span></span>](/cli/azure/vm) |
| [<span data-ttu-id="18906-124">Comptes de stockage</span><span class="sxs-lookup"><span data-stu-id="18906-124">Storage accounts</span></span>](/azure/storage/common/storage-introduction) | [<span data-ttu-id="18906-125">az storage account</span><span class="sxs-lookup"><span data-stu-id="18906-125">az storage account</span></span>](/cli/azure/storage/account) |
| [<span data-ttu-id="18906-126">Key Vault</span><span class="sxs-lookup"><span data-stu-id="18906-126">Key Vault</span></span>](/azure/key-vault/key-vault-whatis) | [<span data-ttu-id="18906-127">az keyvault</span><span class="sxs-lookup"><span data-stu-id="18906-127">az keyvault</span></span>](/cli/azure/keyvault) |
| [<span data-ttu-id="18906-128">Applications web</span><span class="sxs-lookup"><span data-stu-id="18906-128">Web applications</span></span>](/azure/app-service) | [<span data-ttu-id="18906-129">az webapp</span><span class="sxs-lookup"><span data-stu-id="18906-129">az webapp</span></span>](/cli/azure/webapp) |
| [<span data-ttu-id="18906-130">Bases de données SQL</span><span class="sxs-lookup"><span data-stu-id="18906-130">SQL databases</span></span>](/azure/sql-database) | [<span data-ttu-id="18906-131">az sql server</span><span class="sxs-lookup"><span data-stu-id="18906-131">az sql server</span></span>](/cli/azure/sql/server) |
| [<span data-ttu-id="18906-132">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="18906-132">CosmosDB</span></span>](/azure/cosmos-db) | [<span data-ttu-id="18906-133">az cosmosdb</span><span class="sxs-lookup"><span data-stu-id="18906-133">az cosmosdb</span></span>](/cli/azure/cosmosdb) |

## <a name="finding-commands"></a><span data-ttu-id="18906-134">Recherche de commandes</span><span class="sxs-lookup"><span data-stu-id="18906-134">Finding commands</span></span>

<span data-ttu-id="18906-135">Les commandes dans l’interface CLI sont classées par _commandes_ de _groupes_.</span><span class="sxs-lookup"><span data-stu-id="18906-135">Commands in the CLI are organized as _commands_ of _groups_.</span></span> <span data-ttu-id="18906-136">Chaque groupe représente un service Azure, et les commandes agissent sur ce service.</span><span class="sxs-lookup"><span data-stu-id="18906-136">Each group represents an Azure service, and commands operate on that service.</span></span>

<span data-ttu-id="18906-137">Pour rechercher des commandes, utilisez la commande [az find](/cli/azure/reference-index#az-find).</span><span class="sxs-lookup"><span data-stu-id="18906-137">To search for commands, use [az find](/cli/azure/reference-index#az-find).</span></span> <span data-ttu-id="18906-138">Par exemple, pour rechercher des noms de commandes contenant `secret`, utilisez la commande suivante :</span><span class="sxs-lookup"><span data-stu-id="18906-138">For example, to search for command names containing `secret`, use the following command:</span></span>

```azurecli-interactive
az find -q secret
```

<span data-ttu-id="18906-139">Utilisez l’argument `--help` pour obtenir une liste complète des commandes et des sous-groupes d’un groupe.</span><span class="sxs-lookup"><span data-stu-id="18906-139">Use the `--help` argument to get a complete list of commands and subgroups of a group.</span></span> <span data-ttu-id="18906-140">Par exemple, pour trouver les commandes CLI pour fonctionner avec des groupes de sécurité réseau (NSG) :</span><span class="sxs-lookup"><span data-stu-id="18906-140">For example, to find the CLI commands for working with Network Security Groups (NSGs):</span></span>

```azurecli-interactive
az network nsg --help
```

<span data-ttu-id="18906-141">L’interface CLI dispose de la saisie semi-automatique via la touche Tab pour les commandes de l’interpréteur de commandes bash.</span><span class="sxs-lookup"><span data-stu-id="18906-141">The CLI has full tab completion for commands under the bash shell.</span></span>

## <a name="globally-available-arguments"></a><span data-ttu-id="18906-142">Arguments globalement disponibles</span><span class="sxs-lookup"><span data-stu-id="18906-142">Globally available arguments</span></span>

<span data-ttu-id="18906-143">Certains arguments sont disponibles pour chaque commande.</span><span class="sxs-lookup"><span data-stu-id="18906-143">There are some arguments that are available for every command.</span></span>

* <span data-ttu-id="18906-144">`--help` imprime les informations de référence CLI sur les commandes et leurs arguments, et répertorie les commandes et sous-groupes disponibles.</span><span class="sxs-lookup"><span data-stu-id="18906-144">`--help` prints CLI reference information about commands and their arguments and lists available subgroups and commands.</span></span>
* <span data-ttu-id="18906-145">`--output` modifie le format de sortie.</span><span class="sxs-lookup"><span data-stu-id="18906-145">`--output` changes the output format.</span></span> <span data-ttu-id="18906-146">Les formats de sortie disponibles sont `json`, `jsonc` (JSON coloré), `tsv` (valeurs séparées par des tabulations), `table` (tables ASCII lisibles) et `yaml`.</span><span class="sxs-lookup"><span data-stu-id="18906-146">The available output formats are `json`, `jsonc` (colorized JSON), `tsv` (Tab-Separated Values), `table` (human-readable ASCII tables), and `yaml`.</span></span> <span data-ttu-id="18906-147">Par défaut, l’interface CLI génère `json`.</span><span class="sxs-lookup"><span data-stu-id="18906-147">By default the CLI outputs `json`.</span></span> <span data-ttu-id="18906-148">Pour en savoir plus sur les formats de sortie disponibles, consultez [Formats de sortie pour Azure CLI](format-output-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="18906-148">To learn more about the available output formats, see [Output formats for Azure CLI](format-output-azure-cli.md).</span></span>
* <span data-ttu-id="18906-149">`--query` utilise le [langage de requête JMESPath](http://jmespath.org/) pour filtrer la sortie retournée à partir des services Azure.</span><span class="sxs-lookup"><span data-stu-id="18906-149">`--query` uses the [JMESPath query language](http://jmespath.org/) to filter the output returned from Azure services.</span></span> <span data-ttu-id="18906-150">Pour en savoir plus sur les requêtes, consultez [Interroger des résultats de commande avec Azure CLI](query-azure-cli.md) et le [tutoriel JMESPath](http://jmespath.org/tutorial.html).</span><span class="sxs-lookup"><span data-stu-id="18906-150">To learn more about queries, see [Query command results with Azure CLI](query-azure-cli.md) and the [JMESPath tutorial](http://jmespath.org/tutorial.html).</span></span>
* <span data-ttu-id="18906-151">`--verbose` imprime les informations sur les ressources créées dans Azure pendant une opération, et d’autres informations utiles.</span><span class="sxs-lookup"><span data-stu-id="18906-151">`--verbose` prints information about resources created in Azure during an operation, and other useful information.</span></span>
* <span data-ttu-id="18906-152">`--debug` imprime davantage d’informations sur les opérations CLI, utilisées pour le débogage.</span><span class="sxs-lookup"><span data-stu-id="18906-152">`--debug` prints even more information about CLI operations, used for debugging purposes.</span></span> <span data-ttu-id="18906-153">Si vous rencontrez un bogue, fournissez la sortie générée avec l’indicateur `--debug` lors de l’envoi d’un rapport de bogue.</span><span class="sxs-lookup"><span data-stu-id="18906-153">If you find a bug, provide output generated with the `--debug` flag on when submitting a bug report.</span></span>

## <a name="interactive-mode"></a><span data-ttu-id="18906-154">Mode interactif</span><span class="sxs-lookup"><span data-stu-id="18906-154">Interactive mode</span></span>

<span data-ttu-id="18906-155">L’interface CLI propose un mode interactif qui affiche automatiquement les informations d’aide et qui facilite la sélection de sous-commandes.</span><span class="sxs-lookup"><span data-stu-id="18906-155">The CLI offers an interactive mode that automatically displays help information and makes it easier to select subcommands.</span></span> <span data-ttu-id="18906-156">Vous pouvez entrer en mode interactif avec la commande [az interactive](/cli/azure/reference-index#az-interactive).</span><span class="sxs-lookup"><span data-stu-id="18906-156">You enter interactive mode with the [az interactive](/cli/azure/reference-index#az-interactive) command.</span></span>

```azurecli-interactive
az interactive
```

<span data-ttu-id="18906-157">Pour plus d’informations sur le mode interactif, consultez [Mode interactif Azure CLI](interactive-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="18906-157">For more information on interactive mode, see [Azure CLI Interactive Mode](interactive-azure-cli.md).</span></span>

<span data-ttu-id="18906-158">Il existe également un [plug-in Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azurecli) qui propose une expérience interactive, comprenant l’autocomplétion et le survol de la documentation.</span><span class="sxs-lookup"><span data-stu-id="18906-158">There's also a [Visual Studio Code plugin](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azurecli) that offers an interactive experience, including autocomplete and mouse-over documentation.</span></span>

## <a name="learn-cli-basics-with-quickstarts-and-tutorials"></a><span data-ttu-id="18906-159">Apprendre les concepts de base CLI à l’aide des démarrages rapides et des didacticiels</span><span class="sxs-lookup"><span data-stu-id="18906-159">Learn CLI basics with quickstarts and tutorials</span></span>

<span data-ttu-id="18906-160">Pour vous aider à prendre en main Azure CLI, lancez-vous dans un didacticiel approfondi de configuration des machines virtuelles, et utilisez la puissance de l’interface de ligne de commande pour interroger des ressources Azure.</span><span class="sxs-lookup"><span data-stu-id="18906-160">To get you started with the Azure CLI, try an in-depth tutorial for setting up virtual machines and using the power of the CLI to query Azure resources.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="18906-161">Créer des machines virtuelles avec le didacticiel Azure CLI</span><span class="sxs-lookup"><span data-stu-id="18906-161">Create virtual machines with the Azure CLI tutorial</span></span>](azure-cli-vm-tutorial.yml)

<span data-ttu-id="18906-162">Il existe également des guides de démarrage rapide pour les autres services populaires.</span><span class="sxs-lookup"><span data-stu-id="18906-162">There are also quickstarts for other popular services.</span></span>

* [<span data-ttu-id="18906-163">Créer un compte de stockage à l’aide d’Azure CLI</span><span class="sxs-lookup"><span data-stu-id="18906-163">Create a storage account using the Azure CLI</span></span>](/azure/storage/common/storage-quickstart-create-storage-account-cli)
* [<span data-ttu-id="18906-164">Transférer des objets vers/à partir du stockage blob Azure à l’aide de l’interface CLI</span><span class="sxs-lookup"><span data-stu-id="18906-164">Transfer objects to/from Azure Blob storage using the CLI</span></span>](/azure/storage/blobs/storage-quickstart-blobs-cli)
* [<span data-ttu-id="18906-165">Créer une base de données SQL Azure unique à l’aide d’Azure CLI</span><span class="sxs-lookup"><span data-stu-id="18906-165">Create a single Azure SQL database using the Azure CLI</span></span>](/azure/sql-database/sql-database-get-started-cli)
* [<span data-ttu-id="18906-166">Créer un serveur de base de données Azure pour MySQL à l’aide d’Azure CLI</span><span class="sxs-lookup"><span data-stu-id="18906-166">Create an Azure Database for MySQL server using the Azure CLI</span></span>](/azure/mysql/quickstart-create-mysql-server-database-using-azure-cli)
* [<span data-ttu-id="18906-167">Création d’une instance d’Azure Database pour PostgreSQL à l’aide de la CLI Azure</span><span class="sxs-lookup"><span data-stu-id="18906-167">Create an Azure Database for PostgreSQL using the Azure CLI</span></span>](/azure/postgresql/quickstart-create-server-database-azure-cli)
* [<span data-ttu-id="18906-168">Créer une application web Python dans Azure</span><span class="sxs-lookup"><span data-stu-id="18906-168">Create a Python web app in Azure</span></span>](/azure/app-service/app-service-web-get-started-python)
* [<span data-ttu-id="18906-169">Exécuter une image Docker Hub personnalisée dans Azure Web App for Containers</span><span class="sxs-lookup"><span data-stu-id="18906-169">Run a custom Docker Hub image in Azure Web Apps for Containers</span></span>](/azure/app-service/containers/quickstart-custom-docker-image)

## <a name="give-feedback"></a><span data-ttu-id="18906-170">Envoyer des commentaires</span><span class="sxs-lookup"><span data-stu-id="18906-170">Give feedback</span></span>

<span data-ttu-id="18906-171">N’hésitez pas à nous faire part de vos commentaires au sujet de l’interface CLI pour nous aider à l’améliorer et à résoudre les bogues.</span><span class="sxs-lookup"><span data-stu-id="18906-171">We welcome your feedback for the CLI to help us make improvements and resolve bugs.</span></span> <span data-ttu-id="18906-172">Vous pouvez [signaler un problème sur GitHub](https://github.com/azure/azure-cli/issues) ou utiliser les fonctionnalités intégrées de l’interface CLI pour laisser des commentaires d’ordre général à l’aide de la commande [az feedback](/cli/azure/reference-index#az-feedback).</span><span class="sxs-lookup"><span data-stu-id="18906-172">You can [file an issue on GitHub](https://github.com/azure/azure-cli/issues) or use the built-in features of the CLI to leave general feedback with the [az feedback](/cli/azure/reference-index#az-feedback) command.</span></span>

```azurecli-interactive
az feedback
```
