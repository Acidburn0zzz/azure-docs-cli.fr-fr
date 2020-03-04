---
title: Prise en main d’Azure CLI
description: Commencez à utiliser Azure CLI en apprenant les commandes de base.
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 01/30/2020
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: bef8ef96ffefd6214bc924d7378971348d528304
ms.sourcegitcommit: 7caa6673f65e61deb8d6def6386e4eb9acdac923
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/28/2020
ms.locfileid: "77779633"
---
# <a name="get-started-with-azure-cli"></a><span data-ttu-id="34590-103">Prise en main d’Azure CLI</span><span class="sxs-lookup"><span data-stu-id="34590-103">Get started with Azure CLI</span></span>

<span data-ttu-id="34590-104">Bienvenue dans Azure CLI !</span><span class="sxs-lookup"><span data-stu-id="34590-104">Welcome to the Azure CLI!</span></span>  <span data-ttu-id="34590-105">Cet article présente l’interface CLI et fournit des liens qui vont vous aider à commencer.</span><span class="sxs-lookup"><span data-stu-id="34590-105">This article introduces the CLI and provides links to help you get started.</span></span>

> [!NOTE]
>
> <span data-ttu-id="34590-106">Dans les scripts et sur le site de documentation de Microsoft, les exemples Azure CLI sont écrits pour l’interpréteur de commandes `bash`.</span><span class="sxs-lookup"><span data-stu-id="34590-106">In scripts and on the Microsoft documentation site, Azure CLI examples are written for the `bash` shell.</span></span> <span data-ttu-id="34590-107">Les exemples d’une ligne seront exécutés sur n’importe quelle plateforme.</span><span class="sxs-lookup"><span data-stu-id="34590-107">One-line examples will run on any platform.</span></span> <span data-ttu-id="34590-108">Les exemples plus longs qui se répartissent sur plusieurs lignes (`\`) ou incluent l’attribution de variables doivent être modifiés pour fonctionner sur d’autres interpréteurs de commandes, y compris PowerShell.</span><span class="sxs-lookup"><span data-stu-id="34590-108">Longer examples which include line continuations (`\`) or variable assignment need to be modified to work on other shells, including PowerShell.</span></span>

## <a name="install-or-run-in-azure-cloud-shell"></a><span data-ttu-id="34590-109">Installer ou exécuter dans Azure Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="34590-109">Install or run in Azure Cloud Shell</span></span>

<span data-ttu-id="34590-110">Pour commencer avec l’interface CLI, le plus simple est de l’exécuter dans un environnement Azure Cloud Shell via votre navigateur.</span><span class="sxs-lookup"><span data-stu-id="34590-110">The easiest way to get started with the Azure CLI is by running it in an Azure Cloud Shell environment through your browser.</span></span> <span data-ttu-id="34590-111">Pour en savoir plus sur Cloud Shell, consultez [Démarrage rapide de Bash dans Azure Cloud Shell](/azure/cloud-shell/quickstart).</span><span class="sxs-lookup"><span data-stu-id="34590-111">To learn about Cloud Shell, see  [Quickstart for Bash in Azure Cloud Shell](/azure/cloud-shell/quickstart).</span></span>

<span data-ttu-id="34590-112">Lorsque vous êtes prêt à installer l’interface CLI, consultez les [instructions d’installation](install-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="34590-112">When you're ready to install the CLI, see the [installation instructions](install-azure-cli.md).</span></span>

<span data-ttu-id="34590-113">Après avoir installé l’interface CLI pour la première fois, vérifiez qu’elle est bien installée et que vous disposez de la version appropriée en exécutant `az --version`.</span><span class="sxs-lookup"><span data-stu-id="34590-113">After installing the CLI for the first time, check that it's installed and you've got the correct version by running `az --version`.</span></span>

> [!NOTE]
> <span data-ttu-id="34590-114">Si vous utilisez le modèle de déploiement Azure CLI Classic, [installez l’interface de ligne de commande Azure CLI Classic](install-classic-cli.md).</span><span class="sxs-lookup"><span data-stu-id="34590-114">If you're using the Azure classic deployment model, [install the Azure classic CLI](install-classic-cli.md).</span></span>

## <a name="sign-in"></a><span data-ttu-id="34590-115">Se connecter</span><span class="sxs-lookup"><span data-stu-id="34590-115">Sign in</span></span>

<span data-ttu-id="34590-116">Avant d’utiliser les commandes CLI avec une installation locale, vous devez vous connecter avec la commande [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="34590-116">Before using any CLI commands with a local install, you need to sign in with [az login](/cli/azure/reference-index#az-login).</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="34590-117">Après vous être connecté, vous voyez une liste des abonnements associés à votre compte Azure.</span><span class="sxs-lookup"><span data-stu-id="34590-117">After logging in, you see a list of subscriptions associated with your Azure account.</span></span> <span data-ttu-id="34590-118">Les informations d’abonnement avec `isDefault: true` correspond à l’abonnement actuellement activé après vous être connecté.</span><span class="sxs-lookup"><span data-stu-id="34590-118">The subscription information with `isDefault: true` is the currently activated subscription after logging in.</span></span> <span data-ttu-id="34590-119">Pour sélectionner un autre abonnement, utilisez la commande [az account set](/cli/azure/account#az-account-set) avec l’ID d’abonnement auquel vous voulez passer.</span><span class="sxs-lookup"><span data-stu-id="34590-119">To select another subscription, use the [az account set](/cli/azure/account#az-account-set) command with the subscription ID to switch to.</span></span> <span data-ttu-id="34590-120">Pour plus d’informations sur la sélection d’abonnements, consultez [Utiliser plusieurs abonnements Azure](manage-azure-subscriptions-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="34590-120">For more information about subscription selection, see [Use multiple Azure subscriptions](manage-azure-subscriptions-azure-cli.md).</span></span>

<span data-ttu-id="34590-121">Il existe des méthodes pour se connecter de manière non interactive, qui sont dévelopées en détail dans [Se connecter avec Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="34590-121">There are ways to sign in non-interactively, which are covered in detail in [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="common-commands"></a><span data-ttu-id="34590-122">Commandes courantes</span><span class="sxs-lookup"><span data-stu-id="34590-122">Common commands</span></span>

<span data-ttu-id="34590-123">Ce tableau répertorie certaines commandes courantes utilisées dans l’interface CLI ainsi que des liens vers leur documentation de référence.</span><span class="sxs-lookup"><span data-stu-id="34590-123">This table lists some common commands used in the CLI and links to their reference documentation.</span></span>

| <span data-ttu-id="34590-124">Type de ressource</span><span class="sxs-lookup"><span data-stu-id="34590-124">Resource type</span></span> | <span data-ttu-id="34590-125">Groupe de commandes Azure CLI</span><span class="sxs-lookup"><span data-stu-id="34590-125">Azure CLI command group</span></span> |
|---------------|-------------------------|
| [<span data-ttu-id="34590-126">Groupe de ressources</span><span class="sxs-lookup"><span data-stu-id="34590-126">Resource group</span></span>](/azure/azure-resource-manager/resource-group-overview) | [<span data-ttu-id="34590-127">az group</span><span class="sxs-lookup"><span data-stu-id="34590-127">az group</span></span>](/cli/azure/group) |
| [<span data-ttu-id="34590-128">Machines virtuelles</span><span class="sxs-lookup"><span data-stu-id="34590-128">Virtual machines</span></span>](/azure/virtual-machines) | [<span data-ttu-id="34590-129">az vm</span><span class="sxs-lookup"><span data-stu-id="34590-129">az vm</span></span>](/cli/azure/vm) |
| [<span data-ttu-id="34590-130">Comptes de stockage</span><span class="sxs-lookup"><span data-stu-id="34590-130">Storage accounts</span></span>](/azure/storage/common/storage-introduction) | [<span data-ttu-id="34590-131">az storage account</span><span class="sxs-lookup"><span data-stu-id="34590-131">az storage account</span></span>](/cli/azure/storage/account) |
| [<span data-ttu-id="34590-132">Key Vault</span><span class="sxs-lookup"><span data-stu-id="34590-132">Key Vault</span></span>](/azure/key-vault/key-vault-whatis) | [<span data-ttu-id="34590-133">az keyvault</span><span class="sxs-lookup"><span data-stu-id="34590-133">az keyvault</span></span>](/cli/azure/keyvault) |
| [<span data-ttu-id="34590-134">Applications web</span><span class="sxs-lookup"><span data-stu-id="34590-134">Web applications</span></span>](/azure/app-service) | [<span data-ttu-id="34590-135">az webapp</span><span class="sxs-lookup"><span data-stu-id="34590-135">az webapp</span></span>](/cli/azure/webapp) |
| [<span data-ttu-id="34590-136">Bases de données SQL</span><span class="sxs-lookup"><span data-stu-id="34590-136">SQL databases</span></span>](/azure/sql-database) | [<span data-ttu-id="34590-137">az sql server</span><span class="sxs-lookup"><span data-stu-id="34590-137">az sql server</span></span>](/cli/azure/sql/server) |
| [<span data-ttu-id="34590-138">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="34590-138">CosmosDB</span></span>](/azure/cosmos-db) | [<span data-ttu-id="34590-139">az cosmosdb</span><span class="sxs-lookup"><span data-stu-id="34590-139">az cosmosdb</span></span>](/cli/azure/cosmosdb) |

## <a name="finding-commands"></a><span data-ttu-id="34590-140">Recherche de commandes</span><span class="sxs-lookup"><span data-stu-id="34590-140">Finding commands</span></span>

<span data-ttu-id="34590-141">Les commandes dans l’interface CLI sont classées par _commandes_ de _groupes_.</span><span class="sxs-lookup"><span data-stu-id="34590-141">Commands in the CLI are organized as _commands_ of _groups_.</span></span> <span data-ttu-id="34590-142">Chaque groupe représente un service Azure, et les commandes agissent sur ce service.</span><span class="sxs-lookup"><span data-stu-id="34590-142">Each group represents an Azure service, and commands operate on that service.</span></span>

<span data-ttu-id="34590-143">Pour rechercher des commandes, utilisez la commande [az find](/cli/azure/reference-index#az-find).</span><span class="sxs-lookup"><span data-stu-id="34590-143">To search for commands, use [az find](/cli/azure/reference-index#az-find).</span></span> <span data-ttu-id="34590-144">Par exemple, pour rechercher des noms de commandes contenant `secret`, utilisez la commande suivante :</span><span class="sxs-lookup"><span data-stu-id="34590-144">For example, to search for command names containing `secret`, use the following command:</span></span>

```azurecli-interactive
az find secret
```

<span data-ttu-id="34590-145">Utilisez l’argument `--help` pour obtenir une liste complète des commandes et des sous-groupes d’un groupe.</span><span class="sxs-lookup"><span data-stu-id="34590-145">Use the `--help` argument to get a complete list of commands and subgroups of a group.</span></span> <span data-ttu-id="34590-146">Par exemple, pour trouver les commandes CLI pour fonctionner avec des groupes de sécurité réseau (NSG) :</span><span class="sxs-lookup"><span data-stu-id="34590-146">For example, to find the CLI commands for working with Network Security Groups (NSGs):</span></span>

```azurecli-interactive
az network nsg --help
```

<span data-ttu-id="34590-147">L’interface CLI dispose de la saisie semi-automatique via la touche Tab pour les commandes de l’interpréteur de commandes bash.</span><span class="sxs-lookup"><span data-stu-id="34590-147">The CLI has full tab completion for commands under the bash shell.</span></span>

## <a name="globally-available-arguments"></a><span data-ttu-id="34590-148">Arguments globalement disponibles</span><span class="sxs-lookup"><span data-stu-id="34590-148">Globally available arguments</span></span>

<span data-ttu-id="34590-149">Certains arguments sont disponibles pour chaque commande.</span><span class="sxs-lookup"><span data-stu-id="34590-149">There are some arguments that are available for every command.</span></span>

* <span data-ttu-id="34590-150">`--help` imprime les informations de référence CLI sur les commandes et leurs arguments, et répertorie les commandes et sous-groupes disponibles.</span><span class="sxs-lookup"><span data-stu-id="34590-150">`--help` prints CLI reference information about commands and their arguments and lists available subgroups and commands.</span></span>
* <span data-ttu-id="34590-151">`--output` modifie le format de sortie.</span><span class="sxs-lookup"><span data-stu-id="34590-151">`--output` changes the output format.</span></span> <span data-ttu-id="34590-152">Les formats de sortie disponibles sont `json`, `jsonc` (JSON coloré), `tsv` (valeurs séparées par des tabulations), `table` (tables ASCII lisibles) et `yaml`.</span><span class="sxs-lookup"><span data-stu-id="34590-152">The available output formats are `json`, `jsonc` (colorized JSON), `tsv` (Tab-Separated Values), `table` (human-readable ASCII tables), and `yaml`.</span></span> <span data-ttu-id="34590-153">Par défaut, l’interface CLI génère `json`.</span><span class="sxs-lookup"><span data-stu-id="34590-153">By default the CLI outputs `json`.</span></span> <span data-ttu-id="34590-154">Pour en savoir plus sur les formats de sortie disponibles, consultez [Formats de sortie pour Azure CLI](format-output-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="34590-154">To learn more about the available output formats, see [Output formats for Azure CLI](format-output-azure-cli.md).</span></span>
* <span data-ttu-id="34590-155">`--query` utilise le [langage de requête JMESPath](http://jmespath.org/) pour filtrer la sortie retournée à partir des services Azure.</span><span class="sxs-lookup"><span data-stu-id="34590-155">`--query` uses the [JMESPath query language](http://jmespath.org/) to filter the output returned from Azure services.</span></span> <span data-ttu-id="34590-156">Pour en savoir plus sur les requêtes, consultez [Interroger des résultats de commande avec Azure CLI](query-azure-cli.md) et le [tutoriel JMESPath](http://jmespath.org/tutorial.html).</span><span class="sxs-lookup"><span data-stu-id="34590-156">To learn more about queries, see [Query command results with Azure CLI](query-azure-cli.md) and the [JMESPath tutorial](http://jmespath.org/tutorial.html).</span></span>
* <span data-ttu-id="34590-157">`--verbose` imprime les informations sur les ressources créées dans Azure pendant une opération, et d’autres informations utiles.</span><span class="sxs-lookup"><span data-stu-id="34590-157">`--verbose` prints information about resources created in Azure during an operation, and other useful information.</span></span>
* <span data-ttu-id="34590-158">`--debug` imprime davantage d’informations sur les opérations CLI, utilisées pour le débogage.</span><span class="sxs-lookup"><span data-stu-id="34590-158">`--debug` prints even more information about CLI operations, used for debugging purposes.</span></span> <span data-ttu-id="34590-159">Si vous rencontrez un bogue, fournissez la sortie générée avec l’indicateur `--debug` lors de l’envoi d’un rapport de bogue.</span><span class="sxs-lookup"><span data-stu-id="34590-159">If you find a bug, provide output generated with the `--debug` flag on when submitting a bug report.</span></span>

## <a name="interactive-mode"></a><span data-ttu-id="34590-160">Mode interactif</span><span class="sxs-lookup"><span data-stu-id="34590-160">Interactive mode</span></span>

<span data-ttu-id="34590-161">L’interface CLI propose un mode interactif qui affiche automatiquement les informations d’aide et qui facilite la sélection de sous-commandes.</span><span class="sxs-lookup"><span data-stu-id="34590-161">The CLI offers an interactive mode that automatically displays help information and makes it easier to select subcommands.</span></span> <span data-ttu-id="34590-162">Vous pouvez entrer en mode interactif avec la commande [az interactive](/cli/azure/reference-index#az-interactive).</span><span class="sxs-lookup"><span data-stu-id="34590-162">You enter interactive mode with the [az interactive](/cli/azure/reference-index#az-interactive) command.</span></span>

```azurecli-interactive
az interactive
```

<span data-ttu-id="34590-163">Pour plus d’informations sur le mode interactif, consultez [Mode interactif Azure CLI](interactive-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="34590-163">For more information on interactive mode, see [Azure CLI Interactive Mode](interactive-azure-cli.md).</span></span>

<span data-ttu-id="34590-164">Il existe également un [plug-in Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azurecli) qui propose une expérience interactive, comprenant l’autocomplétion et le survol de la documentation.</span><span class="sxs-lookup"><span data-stu-id="34590-164">There's also a [Visual Studio Code plugin](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azurecli) that offers an interactive experience, including autocomplete and mouse-over documentation.</span></span>

## <a name="learn-cli-basics-with-quickstarts-and-tutorials"></a><span data-ttu-id="34590-165">Apprendre les concepts de base CLI à l’aide des démarrages rapides et des didacticiels</span><span class="sxs-lookup"><span data-stu-id="34590-165">Learn CLI basics with quickstarts and tutorials</span></span>

<span data-ttu-id="34590-166">Pour vous aider à prendre en main Azure CLI, lancez-vous dans un didacticiel approfondi de configuration des machines virtuelles, et utilisez la puissance de l’interface de ligne de commande pour interroger des ressources Azure.</span><span class="sxs-lookup"><span data-stu-id="34590-166">To get you started with the Azure CLI, try an in-depth tutorial for setting up virtual machines and using the power of the CLI to query Azure resources.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="34590-167">Créer des machines virtuelles avec le didacticiel Azure CLI</span><span class="sxs-lookup"><span data-stu-id="34590-167">Create virtual machines with the Azure CLI tutorial</span></span>](azure-cli-vm-tutorial.yml)

<span data-ttu-id="34590-168">Il existe également des guides de démarrage rapide pour les autres services populaires.</span><span class="sxs-lookup"><span data-stu-id="34590-168">There are also quickstarts for other popular services.</span></span>

* [<span data-ttu-id="34590-169">Créer un compte de stockage à l’aide d’Azure CLI</span><span class="sxs-lookup"><span data-stu-id="34590-169">Create a storage account using the Azure CLI</span></span>](/azure/storage/common/storage-quickstart-create-storage-account-cli)
* [<span data-ttu-id="34590-170">Transférer des objets vers/à partir du stockage blob Azure à l’aide de l’interface CLI</span><span class="sxs-lookup"><span data-stu-id="34590-170">Transfer objects to/from Azure Blob storage using the CLI</span></span>](/azure/storage/blobs/storage-quickstart-blobs-cli)
* [<span data-ttu-id="34590-171">Créer une base de données Azure SQL unique à l’aide d’Azure CLI</span><span class="sxs-lookup"><span data-stu-id="34590-171">Create a single Azure SQL database using the Azure CLI</span></span>](/azure/sql-database/sql-database-get-started-cli)
* [<span data-ttu-id="34590-172">Créer un serveur de base de données Azure pour MySQL à l’aide d’Azure CLI</span><span class="sxs-lookup"><span data-stu-id="34590-172">Create an Azure Database for MySQL server using the Azure CLI</span></span>](/azure/mysql/quickstart-create-mysql-server-database-using-azure-cli)
* [<span data-ttu-id="34590-173">Création d’une instance d’Azure Database pour PostgreSQL à l’aide de la CLI Azure</span><span class="sxs-lookup"><span data-stu-id="34590-173">Create an Azure Database for PostgreSQL using the Azure CLI</span></span>](/azure/postgresql/quickstart-create-server-database-azure-cli)
* [<span data-ttu-id="34590-174">Créer une application web Python dans Azure</span><span class="sxs-lookup"><span data-stu-id="34590-174">Create a Python web app in Azure</span></span>](/azure/app-service/app-service-web-get-started-python)
* [<span data-ttu-id="34590-175">Exécuter une image Docker Hub personnalisée dans Azure Web App for Containers</span><span class="sxs-lookup"><span data-stu-id="34590-175">Run a custom Docker Hub image in Azure Web Apps for Containers</span></span>](/azure/app-service/containers/quickstart-custom-docker-image)

## <a name="give-feedback"></a><span data-ttu-id="34590-176">Envoyer des commentaires</span><span class="sxs-lookup"><span data-stu-id="34590-176">Give feedback</span></span>

<span data-ttu-id="34590-177">N’hésitez pas à nous faire part de vos commentaires au sujet de l’interface CLI pour nous aider à l’améliorer et à résoudre les bogues.</span><span class="sxs-lookup"><span data-stu-id="34590-177">We welcome your feedback for the CLI to help us make improvements and resolve bugs.</span></span> <span data-ttu-id="34590-178">Vous pouvez [signaler un problème sur GitHub](https://github.com/azure/azure-cli/issues) ou utiliser les fonctionnalités intégrées de l’interface CLI pour laisser des commentaires d’ordre général à l’aide de la commande [az feedback](/cli/azure/reference-index#az-feedback).</span><span class="sxs-lookup"><span data-stu-id="34590-178">You can [file an issue on GitHub](https://github.com/azure/azure-cli/issues) or use the built-in features of the CLI to leave general feedback with the [az feedback](/cli/azure/reference-index#az-feedback) command.</span></span>

```azurecli-interactive
az feedback
```
