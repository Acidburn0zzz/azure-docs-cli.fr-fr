---
title: Extension d’alias d’Azure CLI
description: Comment utiliser l’extension d’alias d’Azure CLI
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 09/07/2018
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 4d324235360e017970a215226572e3effeb9b917
ms.sourcegitcommit: 7caa6673f65e61deb8d6def6386e4eb9acdac923
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/28/2020
ms.locfileid: "77780007"
---
# <a name="the-azure-cli-alias-extension"></a><span data-ttu-id="e1003-103">L’extension d’alias d’Azure CLI</span><span class="sxs-lookup"><span data-stu-id="e1003-103">The Azure CLI alias extension</span></span>

<span data-ttu-id="e1003-104">L’extension d’alias permet aux utilisateurs de définir des commandes personnalisées pour l’interface Azure CLI, à l’aide des commandes existantes.</span><span class="sxs-lookup"><span data-stu-id="e1003-104">The alias extension allows users to define custom commands for the Azure CLI by using existing commands.</span></span> <span data-ttu-id="e1003-105">Les alias aident à garantir une simplicité dans votre flux de travail en y autorisant les raccourcis.</span><span class="sxs-lookup"><span data-stu-id="e1003-105">Aliases help keep your workflow simple by allowing shortcuts.</span></span> <span data-ttu-id="e1003-106">Comme les alias sont alimentés par le moteur de modèles Jinja2, ils prennent bien souvent en charge le traitement avancé des arguments.</span><span class="sxs-lookup"><span data-stu-id="e1003-106">Since aliases are powered by the Jinja2 template engine, they even offer advanced argument processing.</span></span>

> [!NOTE]
> <span data-ttu-id="e1003-107">L’extension d’alias est en préversion publique.</span><span class="sxs-lookup"><span data-stu-id="e1003-107">The Alias Extension is in public preview.</span></span> <span data-ttu-id="e1003-108">Les fonctionnalités et le format du fichier de configuration peuvent changer.</span><span class="sxs-lookup"><span data-stu-id="e1003-108">The features and configuration file format may change.</span></span>

## <a name="install-the-alias-extension"></a><span data-ttu-id="e1003-109">Installer l’extension d’alias</span><span class="sxs-lookup"><span data-stu-id="e1003-109">Install the alias extension</span></span>

<span data-ttu-id="e1003-110">La version minimale requise de l’interface Azure CLI pour utiliser l’extension d’alias est **2.0.28**.</span><span class="sxs-lookup"><span data-stu-id="e1003-110">The minimum required Azure CLI version to use the alias extension is **2.0.28**.</span></span> <span data-ttu-id="e1003-111">Pour vérifier votre version de l’interface CLI, exécutez `az --version`.</span><span class="sxs-lookup"><span data-stu-id="e1003-111">To check your CLI version, run `az --version`.</span></span> <span data-ttu-id="e1003-112">Si vous devez mettre à jour votre installation, suivez les instructions de la section [Installer Azure CLI](./install-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="e1003-112">If you need to update your installation,  follow the instructions in [Install the Azure CLI](./install-azure-cli.md).</span></span>

<span data-ttu-id="e1003-113">Installez l’extension avec la commande [az extension add](/cli/azure/extension#az-extension-add).</span><span class="sxs-lookup"><span data-stu-id="e1003-113">Install the extension with the [az extension add](/cli/azure/extension#az-extension-add) command.</span></span>

```azurecli-interactive
az extension add --name alias
```

<span data-ttu-id="e1003-114">Vérifiez l’installation de l’extension avec [az extension list](/cli/azure/extension#az-extension-list).</span><span class="sxs-lookup"><span data-stu-id="e1003-114">Verify the installation of the extension with [az extension list](/cli/azure/extension#az-extension-list).</span></span> <span data-ttu-id="e1003-115">Si l’extension d’alias a été correctement installée, elle est répertoriée dans la sortie de la commande.</span><span class="sxs-lookup"><span data-stu-id="e1003-115">If the alias extension was installed properly, it's listed in the command output.</span></span>

```azurecli-interactive
az extension list --output table --query '[].{Name:name}'
```

```output
Name
------
alias
```

## <a name="keep-the-extension-up-to-date"></a><span data-ttu-id="e1003-116">Maintenez l’extension à jour</span><span class="sxs-lookup"><span data-stu-id="e1003-116">Keep the extension up-to-date</span></span>

<span data-ttu-id="e1003-117">L’extension d’alias est en cours de développement actif ; de nouvelles versions sont régulièrement publiées.</span><span class="sxs-lookup"><span data-stu-id="e1003-117">The alias extension is under active development and new versions are released regularly.</span></span> <span data-ttu-id="e1003-118">Les nouvelles versions ne sont pas installées lorsque vous mettez à jour l’interface CLI.</span><span class="sxs-lookup"><span data-stu-id="e1003-118">New versions aren't installed when you update the CLI.</span></span> <span data-ttu-id="e1003-119">Installez les mises à jour de l’extension avec [az extension update](/cli/azure/extension#az-extension-update).</span><span class="sxs-lookup"><span data-stu-id="e1003-119">Install the updates for the extension with [az extension update](/cli/azure/extension#az-extension-update).</span></span>

```azurecli-interactive
az extension update --name alias
```

## <a name="manage-aliases-for-the-azure-cli"></a><span data-ttu-id="e1003-120">Gestion des alias pour Azure CLI</span><span class="sxs-lookup"><span data-stu-id="e1003-120">Manage aliases for the Azure CLI</span></span>

<span data-ttu-id="e1003-121">L’extension d’alias vous permet de créer et de gérer les alias pour d’autres commandes CLI.</span><span class="sxs-lookup"><span data-stu-id="e1003-121">The alias extension lets you create and manage aliases for other CLI commands.</span></span> <span data-ttu-id="e1003-122">Pour afficher toutes les commandes disponibles et les détails de paramètres, exécutez la commande de l’alias avec `--help`.</span><span class="sxs-lookup"><span data-stu-id="e1003-122">To view all the available commands and parameter details, run the alias command with `--help`.</span></span>

```azurecli-interactive
az alias --help
```

## <a name="create-simple-alias-commands"></a><span data-ttu-id="e1003-123">Créer des commandes alias simples</span><span class="sxs-lookup"><span data-stu-id="e1003-123">Create simple alias commands</span></span>

<span data-ttu-id="e1003-124">Les alias peuvent par exemple servir à raccourcir les noms existants des groupes de commandes ou des commandes.</span><span class="sxs-lookup"><span data-stu-id="e1003-124">One use of aliases is for shortening existing command groups or command names.</span></span> <span data-ttu-id="e1003-125">Par exemple, vous pouvez raccourcir le nom du groupe de commandes `group` en le ramenant à `rg` et le nom de la commande `list` en `ls`.</span><span class="sxs-lookup"><span data-stu-id="e1003-125">For example, you can shorten the `group` command group to `rg` and the `list` command to `ls`.</span></span>

```azurecli-interactive
az alias create --name rg --command group
az alias create --name ls --command list
```

<span data-ttu-id="e1003-126">Ces alias nouvellement définis peuvent désormais être utilisés dans l’ensemble des emplacements pouvant héberger leur définition.</span><span class="sxs-lookup"><span data-stu-id="e1003-126">These newly defined aliases can now be used anywhere that their definition would be.</span></span>

```azurecli-interactive
az rg list
az rg ls
az vm ls
```

<span data-ttu-id="e1003-127">N’incluez pas `az` dans la commande.</span><span class="sxs-lookup"><span data-stu-id="e1003-127">Do not include `az` as part of the command.</span></span>

<span data-ttu-id="e1003-128">Les alias peuvent également être des raccourcis de commandes complètes.</span><span class="sxs-lookup"><span data-stu-id="e1003-128">Aliases can also be shortcuts for complete commands.</span></span> <span data-ttu-id="e1003-129">Le prochain exemple répertorie les groupes de ressources disponibles et leur emplacement dans la sortie de table :</span><span class="sxs-lookup"><span data-stu-id="e1003-129">The next example lists available resource groups and their locations in table output:</span></span>

```azurecli-interactive
az alias create --name ls-groups --command "group list --query '[].{Name:name, Location:location}' --output table"
```

<span data-ttu-id="e1003-130">Désormais, `ls-groups` peut être exécutée comme toute autre commande CLI.</span><span class="sxs-lookup"><span data-stu-id="e1003-130">Now `ls-groups` can be run like any other CLI command.</span></span>

```azurecli-interactive
az ls-groups
```

## <a name="create-an-alias-command-with-arguments"></a><span data-ttu-id="e1003-131">Créer une commande d’alias avec des arguments</span><span class="sxs-lookup"><span data-stu-id="e1003-131">Create an alias command with arguments</span></span>

<span data-ttu-id="e1003-132">Il est également possible d’ajouter des arguments positionnels à une commande d’alias en les incluant en tant que `{{ arg_name }}` dans le nom d’alias.</span><span class="sxs-lookup"><span data-stu-id="e1003-132">You can also add positional arguments to an alias command by including them as `{{ arg_name }}` in the alias name.</span></span> <span data-ttu-id="e1003-133">L’espace à l’intérieur des accolades est requis.</span><span class="sxs-lookup"><span data-stu-id="e1003-133">The whitespace inside the braces is required.</span></span>

```azurecli-interactive
az alias create --name "alias_name {{ arg1 }} {{ arg2 }} ..." --command "invoke_including_args"
```

<span data-ttu-id="e1003-134">Le prochain exemple d’alias indique comment utiliser des arguments positionnels afin de récupérer l’adresse IP publique d’une machine virtuelle.</span><span class="sxs-lookup"><span data-stu-id="e1003-134">The next example alias shows how to use positional arguments to get the public IP address for a VM.</span></span>

```azurecli-interactive
az alias create \
    --name "get-vm-ip {{ resourceGroup }} {{ vmName }}" \
    --command "vm list-ip-addresses --resource-group {{ resourceGroup }} --name {{ vmName }}
        --query [0].virtualMachine.network.publicIpAddresses[0].ipAddress"
```

<span data-ttu-id="e1003-135">Lorsque vous exécutez cette commande, vous octroyez des valeurs aux arguments positionnels.</span><span class="sxs-lookup"><span data-stu-id="e1003-135">When running this command, you give values to the positional arguments.</span></span>

```azurecli-interactive
az get-vm-ip MyResourceGroup MyVM
```

<span data-ttu-id="e1003-136">Vous pouvez également utiliser des variables d’environnement dans les commandes alias, qui sont évaluées au moment de l’exécution.</span><span class="sxs-lookup"><span data-stu-id="e1003-136">You can also use environment variables in aliased commands, which are evaluated at runtime.</span></span> <span data-ttu-id="e1003-137">Le prochain exemple ajoute l’alias `create-rg`, qui crée un groupe de ressources dans `eastus` et ajoute une balise `owner`.</span><span class="sxs-lookup"><span data-stu-id="e1003-137">The next example adds the `create-rg` alias, which creates a resource group in `eastus` and adds an `owner` tag.</span></span> <span data-ttu-id="e1003-138">Cette balise se voit affecter la valeur de la variable d’environnement local `USER`.</span><span class="sxs-lookup"><span data-stu-id="e1003-138">This tag is assigned the value of the local environment variable `USER`.</span></span>

```azurecli-interactive
az alias create \
    --name "create-rg {{ groupName }}" \
    --command "group create --name {{ groupName }} --location eastus --tags owner=\$USER"
```

<span data-ttu-id="e1003-139">Pour enregistrer les variables d’environnement à l’intérieur de la commande de l’alias, le signe dollar `$` doit être placé dans une séquence d’échappement.</span><span class="sxs-lookup"><span data-stu-id="e1003-139">To register the environment variables inside the command of the alias, the dollar sign `$` must be escaped.</span></span>

## <a name="process-arguments-using-jinja2-templates"></a><span data-ttu-id="e1003-140">Traiter les arguments à l’aide des modèles Jinja2</span><span class="sxs-lookup"><span data-stu-id="e1003-140">Process arguments using Jinja2 templates</span></span>

<span data-ttu-id="e1003-141">La substitution d’argument dans l’extension d’alias est effectuée par [Jinja2](http://jinja.pocoo.org/docs/2.10/).</span><span class="sxs-lookup"><span data-stu-id="e1003-141">Argument substitution in the alias extension is performed by [Jinja2](http://jinja.pocoo.org/docs/2.10/).</span></span> <span data-ttu-id="e1003-142">Les modèles Jinja2 permettent de manipuler les arguments.</span><span class="sxs-lookup"><span data-stu-id="e1003-142">Jinja2 templates allow for manipulating the arguments.</span></span>

<span data-ttu-id="e1003-143">Avec les modèles Jinja2, vous pouvez écrire des alias qui acceptent des types d’arguments supplémentaires par rapport à la commande sous-jacente.</span><span class="sxs-lookup"><span data-stu-id="e1003-143">With Jinja2 templates, you can write aliases that take different types of arguments than the underlying command.</span></span> <span data-ttu-id="e1003-144">Par exemple, vous pouvez développer un alias acceptant une URL de stockage.</span><span class="sxs-lookup"><span data-stu-id="e1003-144">For example, you can make an alias that takes a storage URL.</span></span> <span data-ttu-id="e1003-145">Par la suite, cette URL est analysée afin de transmettre les noms de compte et de conteneur à la commande de stockage.</span><span class="sxs-lookup"><span data-stu-id="e1003-145">Then this URL is parsed to pass the account and container names to the storage command.</span></span>

```azurecli-interactive
az alias create \
    --name 'storage-ls {{ url }}' \
    --command "storage blob list
        --account-name {{ url.replace('https://', '').split('.')[0] }}
        --container-name {{ url.replace('https://', '').split('/')[1] }}"
```

<span data-ttu-id="e1003-146">Pour en savoir plus sur le moteur de modèles Jinja2, consultez la [documentation Jinja2](http://jinja.pocoo.org/docs/2.10/templates/).</span><span class="sxs-lookup"><span data-stu-id="e1003-146">To learn about the Jinja2 template engine, see [the Jinja2 documentation](http://jinja.pocoo.org/docs/2.10/templates/).</span></span>

## <a name="alias-configuration-file"></a><span data-ttu-id="e1003-147">Fichier de configuration d’alias</span><span class="sxs-lookup"><span data-stu-id="e1003-147">Alias configuration file</span></span>

<span data-ttu-id="e1003-148">Une autre façon de créer et de modifier des alias est de modifier le fichier de configuration d’alias.</span><span class="sxs-lookup"><span data-stu-id="e1003-148">Another way to create and modify aliases is to alter the alias configuration file.</span></span> <span data-ttu-id="e1003-149">Les définitions des commandes alias sont consignées dans un fichier de configuration, qui se situe sur `$AZURE_USER_CONFIG/alias`.</span><span class="sxs-lookup"><span data-stu-id="e1003-149">Alias command definitions are written into a configuration file, located at `$AZURE_USER_CONFIG/alias`.</span></span> <span data-ttu-id="e1003-150">La valeur par défaut de `AZURE_USER_CONFIG` est `$HOME/.azure` sous macOS et Linux, et `%USERPROFILE%\.azure` sous Windows.</span><span class="sxs-lookup"><span data-stu-id="e1003-150">The default value of `AZURE_USER_CONFIG` is `$HOME/.azure` on macOS and Linux, and `%USERPROFILE%\.azure` on Windows.</span></span> <span data-ttu-id="e1003-151">Le fichier de configuration d’alias est consigné au format du fichier de configuration INI.</span><span class="sxs-lookup"><span data-stu-id="e1003-151">The alias configuration file is written in the INI configuration file format.</span></span> <span data-ttu-id="e1003-152">Le format des commandes alias est le suivant :</span><span class="sxs-lookup"><span data-stu-id="e1003-152">The format for alias commands is:</span></span>

```ini
[alias_name]
command = invoked_commands
```

<span data-ttu-id="e1003-153">Pour les alias qui possèdent des arguments de position, le format des commandes alias est :</span><span class="sxs-lookup"><span data-stu-id="e1003-153">For aliases that have positional arguments, the format for alias commands is:</span></span>

```ini
[alias_name {{ arg1 }} {{ arg2 }} ...]
command = invoked_commands_including_args
```

## <a name="create-an-alias-command-with-arguments-via-the-alias-configuration-file"></a><span data-ttu-id="e1003-154">Créer une commande alias avec des arguments via le fichier de configuration d’alias</span><span class="sxs-lookup"><span data-stu-id="e1003-154">Create an alias command with arguments via the alias configuration file</span></span>

<span data-ttu-id="e1003-155">L’exemple suivant illustre un alias pour une commande avec des arguments.</span><span class="sxs-lookup"><span data-stu-id="e1003-155">The next example shows an alias for a command with arguments.</span></span> <span data-ttu-id="e1003-156">Cette commande obtient l’adresse IP publique pour une machine virtuelle.</span><span class="sxs-lookup"><span data-stu-id="e1003-156">This command gets the public IP address for a VM.</span></span> <span data-ttu-id="e1003-157">Les commandes d’un alias doivent toutes se trouver sur une seule ligne et utiliser tous les arguments dans le nom d’alias.</span><span class="sxs-lookup"><span data-stu-id="e1003-157">Aliased commands must all be on a single line, and use all of the arguments in the alias name.</span></span>

```ini
[get-vm-ip {{ resourceGroup }} {{ vmName }}]
command = vm list-ip-addresses --resource-group {{ resourceGroup }} --name {{ vmName }} --query [0].virtualMachine.network.publicIpAddresses[0].ipAddress
```

## <a name="uninstall-the-alias-extension"></a><span data-ttu-id="e1003-158">Désinstaller l’extension d’alias</span><span class="sxs-lookup"><span data-stu-id="e1003-158">Uninstall the alias extension</span></span>

<span data-ttu-id="e1003-159">Pour désinstaller l’extension, utilisez la commande [az extension remove](/cli/azure/extension#az-extension-remove).</span><span class="sxs-lookup"><span data-stu-id="e1003-159">To uninstall the extension, use the [az extension remove](/cli/azure/extension#az-extension-remove) command.</span></span>

```azurecli-interactive
az extension remove --name alias
```

<span data-ttu-id="e1003-160">Si vous avez procédé à la désinstallation en raison d’un bogue ou d’un problème lié à l’extension, veuillez [signaler un incident GitHub](https://github.com/Azure/azure-cli-extensions/issues) afin que nous puissions réfléchir à la correction.</span><span class="sxs-lookup"><span data-stu-id="e1003-160">If you uninstalled because a bug or other problem with the extension, [file a GitHub issue](https://github.com/Azure/azure-cli-extensions/issues) so that we can provide a fix.</span></span>
