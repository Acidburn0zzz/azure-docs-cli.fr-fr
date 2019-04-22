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
ms.openlocfilehash: 003576ba22cdc4fc64977b653d0fb6859cd38446
ms.sourcegitcommit: 334a1da92a73e42e715e33470057f4194f10b2ea
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/17/2019
ms.locfileid: "59429028"
---
# <a name="get-started-with-azure-cli"></a><span data-ttu-id="18d07-104">Prise en main d’Azure CLI</span><span class="sxs-lookup"><span data-stu-id="18d07-104">Get started with Azure CLI</span></span>

<span data-ttu-id="18d07-105">Bienvenue dans Azure CLI !</span><span class="sxs-lookup"><span data-stu-id="18d07-105">Welcome to the Azure CLI!</span></span> <span data-ttu-id="18d07-106">L’interface CLI est un outil conçu pour vous aider à utiliser rapidement et efficacement les services Azure, en mettant l’accent sur l’automatisation.</span><span class="sxs-lookup"><span data-stu-id="18d07-106">The CLI is a tool designed to get you working quickly and efficiently with Azure services, with an emphasis on automation.</span></span> <span data-ttu-id="18d07-107">Cet article présente les fonctionnalités de l’interface CLI et des liens vers des ressources qui vous aideront à être productif.</span><span class="sxs-lookup"><span data-stu-id="18d07-107">This article introduces features of the CLI and links out to resources that help you be productive.</span></span>

## <a name="install-or-run-in-azure-cloud-shell"></a><span data-ttu-id="18d07-108">Installer ou exécuter dans Azure Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="18d07-108">Install or run in Azure Cloud Shell</span></span>

<span data-ttu-id="18d07-109">Pour commencer avec l’interface CLI, le plus simple est de l’exécuter dans un environnement Azure Cloud Shell via votre navigateur.</span><span class="sxs-lookup"><span data-stu-id="18d07-109">The easiest way to get started with the Azure CLI is by running it in an Azure Cloud Shell environment through your browser.</span></span> <span data-ttu-id="18d07-110">Pour en savoir plus sur Cloud Shell, consultez [Démarrage rapide de Bash dans Azure Cloud Shell](/azure/cloud-shell/quickstart).</span><span class="sxs-lookup"><span data-stu-id="18d07-110">To learn about Cloud Shell, see  [Quickstart for Bash in Azure Cloud Shell](/azure/cloud-shell/quickstart).</span></span>

<span data-ttu-id="18d07-111">Lorsque vous êtes prêt à installer l’interface CLI, consultez les [instructions d’installation](install-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="18d07-111">When you're ready to install the CLI, see the [installation instructions](install-azure-cli.md).</span></span>

<span data-ttu-id="18d07-112">Après avoir installé l’interface CLI pour la première fois, vérifiez qu’elle est bien installée et que vous disposez de la version appropriée en exécutant `az --version`.</span><span class="sxs-lookup"><span data-stu-id="18d07-112">After installing the CLI for the first time, check that it's installed and you've got the correct version by running `az --version`.</span></span>

## <a name="sign-in"></a><span data-ttu-id="18d07-113">Se connecter</span><span class="sxs-lookup"><span data-stu-id="18d07-113">Sign in</span></span>

<span data-ttu-id="18d07-114">Avant d’utiliser les commandes CLI avec une installation locale, vous devez vous connecter avec la commande [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="18d07-114">Before using any CLI commands with a local install, you need to sign in with [az login](/cli/azure/reference-index#az-login).</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="18d07-115">Après vous être connecté, vous voyez une liste des abonnements associés à votre compte Azure.</span><span class="sxs-lookup"><span data-stu-id="18d07-115">After logging in, you see a list of subscriptions associated with your Azure account.</span></span> <span data-ttu-id="18d07-116">Les informations d’abonnement avec `isDefault: true` correspond à l’abonnement actuellement activé après vous être connecté.</span><span class="sxs-lookup"><span data-stu-id="18d07-116">The subscription information with `isDefault: true` is the currently activated subscription after logging in.</span></span> <span data-ttu-id="18d07-117">Pour sélectionner un autre abonnement, utilisez la commande [az account set](/cli/azure/account#az-account-set) avec l’ID d’abonnement auquel vous voulez passer.</span><span class="sxs-lookup"><span data-stu-id="18d07-117">To select another subscription, use the [az account set](/cli/azure/account#az-account-set) command with the subscription ID to switch to.</span></span> <span data-ttu-id="18d07-118">Pour plus d’informations sur la sélection d’abonnements, consultez [Utiliser plusieurs abonnements Azure](manage-azure-subscriptions-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="18d07-118">For more information about subscription selection, see [Use multiple Azure subscriptions](manage-azure-subscriptions-azure-cli.md).</span></span>

<span data-ttu-id="18d07-119">Il existe des méthodes pour se connecter de manière non interactive, qui sont dévelopées en détail dans [Se connecter avec Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="18d07-119">There are ways to sign in non-interactively, which are covered in detail in [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="common-commands"></a><span data-ttu-id="18d07-120">Commandes courantes</span><span class="sxs-lookup"><span data-stu-id="18d07-120">Common commands</span></span>

<span data-ttu-id="18d07-121">Ce tableau répertorie certaines commandes courantes utilisées dans l’interface CLI ainsi que des liens vers leur documentation de référence.</span><span class="sxs-lookup"><span data-stu-id="18d07-121">This table lists some common commands used in the CLI and links to their reference documentation.</span></span>

| <span data-ttu-id="18d07-122">Type de ressource</span><span class="sxs-lookup"><span data-stu-id="18d07-122">Resource type</span></span> | <span data-ttu-id="18d07-123">Groupe de commandes Azure CLI</span><span class="sxs-lookup"><span data-stu-id="18d07-123">Azure CLI command group</span></span> |
|---------------|-------------------------|
| [<span data-ttu-id="18d07-124">Groupe de ressources</span><span class="sxs-lookup"><span data-stu-id="18d07-124">Resource group</span></span>](/azure/azure-resource-manager/resource-group-overview) | [<span data-ttu-id="18d07-125">az group</span><span class="sxs-lookup"><span data-stu-id="18d07-125">az group</span></span>](/cli/azure/group) |
| [<span data-ttu-id="18d07-126">Machines virtuelles</span><span class="sxs-lookup"><span data-stu-id="18d07-126">Virtual machines</span></span>](/azure/virtual-machines) | [<span data-ttu-id="18d07-127">az vm</span><span class="sxs-lookup"><span data-stu-id="18d07-127">az vm</span></span>](/cli/azure/vm) |
| [<span data-ttu-id="18d07-128">Comptes de stockage</span><span class="sxs-lookup"><span data-stu-id="18d07-128">Storage accounts</span></span>](/azure/storage/common/storage-introduction) | [<span data-ttu-id="18d07-129">az storage account</span><span class="sxs-lookup"><span data-stu-id="18d07-129">az storage account</span></span>](/cli/azure/storage/account) |
| [<span data-ttu-id="18d07-130">Key Vault</span><span class="sxs-lookup"><span data-stu-id="18d07-130">Key Vault</span></span>](/azure/key-vault/key-vault-whatis) | [<span data-ttu-id="18d07-131">az keyvault</span><span class="sxs-lookup"><span data-stu-id="18d07-131">az keyvault</span></span>](/cli/azure/keyvault) |
| [<span data-ttu-id="18d07-132">Applications web</span><span class="sxs-lookup"><span data-stu-id="18d07-132">Web applications</span></span>](/azure/app-service) | [<span data-ttu-id="18d07-133">az webapp</span><span class="sxs-lookup"><span data-stu-id="18d07-133">az webapp</span></span>](/cli/azure/webapp) |
| [<span data-ttu-id="18d07-134">Bases de données SQL</span><span class="sxs-lookup"><span data-stu-id="18d07-134">SQL databases</span></span>](/azure/sql-database) | [<span data-ttu-id="18d07-135">az sql server</span><span class="sxs-lookup"><span data-stu-id="18d07-135">az sql server</span></span>](/cli/azure/sql/server) |
| [<span data-ttu-id="18d07-136">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="18d07-136">CosmosDB</span></span>](/azure/cosmos-db) | [<span data-ttu-id="18d07-137">az cosmosdb</span><span class="sxs-lookup"><span data-stu-id="18d07-137">az cosmosdb</span></span>](/cli/azure/cosmosdb) |

## <a name="finding-commands"></a><span data-ttu-id="18d07-138">Recherche de commandes</span><span class="sxs-lookup"><span data-stu-id="18d07-138">Finding commands</span></span>

<span data-ttu-id="18d07-139">Les commandes dans l’interface CLI sont classées par _commandes_ de _groupes_.</span><span class="sxs-lookup"><span data-stu-id="18d07-139">Commands in the CLI are organized as _commands_ of _groups_.</span></span> <span data-ttu-id="18d07-140">Chaque groupe représente un service Azure, et les commandes agissent sur ce service.</span><span class="sxs-lookup"><span data-stu-id="18d07-140">Each group represents an Azure service, and commands operate on that service.</span></span>

<span data-ttu-id="18d07-141">Pour rechercher des commandes, utilisez la commande [az find](/cli/azure/reference-index#az-find).</span><span class="sxs-lookup"><span data-stu-id="18d07-141">To search for commands, use [az find](/cli/azure/reference-index#az-find).</span></span> <span data-ttu-id="18d07-142">Par exemple, pour rechercher des noms de commandes contenant `secret`, utilisez la commande suivante :</span><span class="sxs-lookup"><span data-stu-id="18d07-142">For example, to search for command names containing `secret`, use the following command:</span></span>

```azurecli-interactive
az find secret
```

<span data-ttu-id="18d07-143">Utilisez l’argument `--help` pour obtenir une liste complète des commandes et des sous-groupes d’un groupe.</span><span class="sxs-lookup"><span data-stu-id="18d07-143">Use the `--help` argument to get a complete list of commands and subgroups of a group.</span></span> <span data-ttu-id="18d07-144">Par exemple, pour trouver les commandes CLI pour fonctionner avec des groupes de sécurité réseau (NSG) :</span><span class="sxs-lookup"><span data-stu-id="18d07-144">For example, to find the CLI commands for working with Network Security Groups (NSGs):</span></span>

```azurecli-interactive
az network nsg --help
```

<span data-ttu-id="18d07-145">L’interface CLI dispose de la saisie semi-automatique via la touche Tab pour les commandes de l’interpréteur de commandes bash.</span><span class="sxs-lookup"><span data-stu-id="18d07-145">The CLI has full tab completion for commands under the bash shell.</span></span>

## <a name="globally-available-arguments"></a><span data-ttu-id="18d07-146">Arguments globalement disponibles</span><span class="sxs-lookup"><span data-stu-id="18d07-146">Globally available arguments</span></span>

<span data-ttu-id="18d07-147">Certains arguments sont disponibles pour chaque commande.</span><span class="sxs-lookup"><span data-stu-id="18d07-147">There are some arguments that are available for every command.</span></span>

* <span data-ttu-id="18d07-148">`--help` imprime les informations de référence CLI sur les commandes et leurs arguments, et répertorie les commandes et sous-groupes disponibles.</span><span class="sxs-lookup"><span data-stu-id="18d07-148">`--help` prints CLI reference information about commands and their arguments and lists available subgroups and commands.</span></span>
* <span data-ttu-id="18d07-149">`--output` modifie le format de sortie.</span><span class="sxs-lookup"><span data-stu-id="18d07-149">`--output` changes the output format.</span></span> <span data-ttu-id="18d07-150">Les formats de sortie disponibles sont `json`, `jsonc` (JSON coloré), `tsv` (valeurs séparées par des tabulations), `table` (tables ASCII lisibles) et `yaml`.</span><span class="sxs-lookup"><span data-stu-id="18d07-150">The available output formats are `json`, `jsonc` (colorized JSON), `tsv` (Tab-Separated Values), `table` (human-readable ASCII tables), and `yaml`.</span></span> <span data-ttu-id="18d07-151">Par défaut, l’interface CLI génère `json`.</span><span class="sxs-lookup"><span data-stu-id="18d07-151">By default the CLI outputs `json`.</span></span> <span data-ttu-id="18d07-152">Pour en savoir plus sur les formats de sortie disponibles, consultez [Formats de sortie pour Azure CLI](format-output-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="18d07-152">To learn more about the available output formats, see [Output formats for Azure CLI](format-output-azure-cli.md).</span></span>
* <span data-ttu-id="18d07-153">`--query` utilise le [langage de requête JMESPath](http://jmespath.org/) pour filtrer la sortie retournée à partir des services Azure.</span><span class="sxs-lookup"><span data-stu-id="18d07-153">`--query` uses the [JMESPath query language](http://jmespath.org/) to filter the output returned from Azure services.</span></span> <span data-ttu-id="18d07-154">Pour en savoir plus sur les requêtes, consultez [Interroger des résultats de commande avec Azure CLI](query-azure-cli.md) et le [tutoriel JMESPath](http://jmespath.org/tutorial.html).</span><span class="sxs-lookup"><span data-stu-id="18d07-154">To learn more about queries, see [Query command results with Azure CLI](query-azure-cli.md) and the [JMESPath tutorial](http://jmespath.org/tutorial.html).</span></span>
* <span data-ttu-id="18d07-155">`--verbose` imprime les informations sur les ressources créées dans Azure pendant une opération, et d’autres informations utiles.</span><span class="sxs-lookup"><span data-stu-id="18d07-155">`--verbose` prints information about resources created in Azure during an operation, and other useful information.</span></span>
* <span data-ttu-id="18d07-156">`--debug` imprime davantage d’informations sur les opérations CLI, utilisées pour le débogage.</span><span class="sxs-lookup"><span data-stu-id="18d07-156">`--debug` prints even more information about CLI operations, used for debugging purposes.</span></span> <span data-ttu-id="18d07-157">Si vous rencontrez un bogue, fournissez la sortie générée avec l’indicateur `--debug` lors de l’envoi d’un rapport de bogue.</span><span class="sxs-lookup"><span data-stu-id="18d07-157">If you find a bug, provide output generated with the `--debug` flag on when submitting a bug report.</span></span>

## <a name="interactive-mode"></a><span data-ttu-id="18d07-158">Mode interactif</span><span class="sxs-lookup"><span data-stu-id="18d07-158">Interactive mode</span></span>

<span data-ttu-id="18d07-159">L’interface CLI propose un mode interactif qui affiche automatiquement les informations d’aide et qui facilite la sélection de sous-commandes.</span><span class="sxs-lookup"><span data-stu-id="18d07-159">The CLI offers an interactive mode that automatically displays help information and makes it easier to select subcommands.</span></span> <span data-ttu-id="18d07-160">Vous pouvez entrer en mode interactif avec la commande [az interactive](/cli/azure/reference-index#az-interactive).</span><span class="sxs-lookup"><span data-stu-id="18d07-160">You enter interactive mode with the [az interactive](/cli/azure/reference-index#az-interactive) command.</span></span>

```azurecli-interactive
az interactive
```

<span data-ttu-id="18d07-161">Pour plus d’informations sur le mode interactif, consultez [Mode interactif Azure CLI](interactive-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="18d07-161">For more information on interactive mode, see [Azure CLI Interactive Mode](interactive-azure-cli.md).</span></span>

<span data-ttu-id="18d07-162">Il existe également un [plug-in Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azurecli) qui propose une expérience interactive, comprenant l’autocomplétion et le survol de la documentation.</span><span class="sxs-lookup"><span data-stu-id="18d07-162">There's also a [Visual Studio Code plugin](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azurecli) that offers an interactive experience, including autocomplete and mouse-over documentation.</span></span>

## <a name="learn-cli-basics-with-quickstarts-and-tutorials"></a><span data-ttu-id="18d07-163">Apprendre les concepts de base CLI à l’aide des démarrages rapides et des didacticiels</span><span class="sxs-lookup"><span data-stu-id="18d07-163">Learn CLI basics with quickstarts and tutorials</span></span>

<span data-ttu-id="18d07-164">Pour vous aider à prendre en main Azure CLI, lancez-vous dans un didacticiel approfondi de configuration des machines virtuelles, et utilisez la puissance de l’interface de ligne de commande pour interroger des ressources Azure.</span><span class="sxs-lookup"><span data-stu-id="18d07-164">To get you started with the Azure CLI, try an in-depth tutorial for setting up virtual machines and using the power of the CLI to query Azure resources.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="18d07-165">Créer des machines virtuelles avec le didacticiel Azure CLI</span><span class="sxs-lookup"><span data-stu-id="18d07-165">Create virtual machines with the Azure CLI tutorial</span></span>](azure-cli-vm-tutorial.yml)

<span data-ttu-id="18d07-166">Il existe également des guides de démarrage rapide pour les autres services populaires.</span><span class="sxs-lookup"><span data-stu-id="18d07-166">There are also quickstarts for other popular services.</span></span>

* [<span data-ttu-id="18d07-167">Créer un compte de stockage à l’aide d’Azure CLI</span><span class="sxs-lookup"><span data-stu-id="18d07-167">Create a storage account using the Azure CLI</span></span>](/azure/storage/common/storage-quickstart-create-storage-account-cli)
* [<span data-ttu-id="18d07-168">Transférer des objets vers/à partir du stockage blob Azure à l’aide de l’interface CLI</span><span class="sxs-lookup"><span data-stu-id="18d07-168">Transfer objects to/from Azure Blob storage using the CLI</span></span>](/azure/storage/blobs/storage-quickstart-blobs-cli)
* [<span data-ttu-id="18d07-169">Créer une base de données SQL Azure unique à l’aide d’Azure CLI</span><span class="sxs-lookup"><span data-stu-id="18d07-169">Create a single Azure SQL database using the Azure CLI</span></span>](/azure/sql-database/sql-database-get-started-cli)
* [<span data-ttu-id="18d07-170">Créer un serveur de base de données Azure pour MySQL à l’aide d’Azure CLI</span><span class="sxs-lookup"><span data-stu-id="18d07-170">Create an Azure Database for MySQL server using the Azure CLI</span></span>](/azure/mysql/quickstart-create-mysql-server-database-using-azure-cli)
* [<span data-ttu-id="18d07-171">Création d’une instance d’Azure Database pour PostgreSQL à l’aide de la CLI Azure</span><span class="sxs-lookup"><span data-stu-id="18d07-171">Create an Azure Database for PostgreSQL using the Azure CLI</span></span>](/azure/postgresql/quickstart-create-server-database-azure-cli)
* [<span data-ttu-id="18d07-172">Créer une application web Python dans Azure</span><span class="sxs-lookup"><span data-stu-id="18d07-172">Create a Python web app in Azure</span></span>](/azure/app-service/app-service-web-get-started-python)
* [<span data-ttu-id="18d07-173">Exécuter une image Docker Hub personnalisée dans Azure Web App for Containers</span><span class="sxs-lookup"><span data-stu-id="18d07-173">Run a custom Docker Hub image in Azure Web Apps for Containers</span></span>](/azure/app-service/containers/quickstart-custom-docker-image)

## <a name="give-feedback"></a><span data-ttu-id="18d07-174">Envoyer des commentaires</span><span class="sxs-lookup"><span data-stu-id="18d07-174">Give feedback</span></span>

<span data-ttu-id="18d07-175">N’hésitez pas à nous faire part de vos commentaires au sujet de l’interface CLI pour nous aider à l’améliorer et à résoudre les bogues.</span><span class="sxs-lookup"><span data-stu-id="18d07-175">We welcome your feedback for the CLI to help us make improvements and resolve bugs.</span></span> <span data-ttu-id="18d07-176">Vous pouvez [signaler un problème sur GitHub](https://github.com/azure/azure-cli/issues) ou utiliser les fonctionnalités intégrées de l’interface CLI pour laisser des commentaires d’ordre général à l’aide de la commande [az feedback](/cli/azure/reference-index#az-feedback).</span><span class="sxs-lookup"><span data-stu-id="18d07-176">You can [file an issue on GitHub](https://github.com/azure/azure-cli/issues) or use the built-in features of the CLI to leave general feedback with the [az feedback](/cli/azure/reference-index#az-feedback) command.</span></span>

```azurecli-interactive
az feedback
```
