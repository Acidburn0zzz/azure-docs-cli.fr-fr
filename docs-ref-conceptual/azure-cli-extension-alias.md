---
title: Extension d’alias Azure CLI 2.0
description: Comment utiliser l’extension d’alias Azure CLI 2.0
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 03/14/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: e8419394bb221d2614e15171bd19dd76fd9cd773
ms.sourcegitcommit: b5a6296c006e3a44f66892729e47d7a967267d3e
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/28/2018
---
# <a name="the-azure-cli-20-alias-extension"></a><span data-ttu-id="4a33f-103">L’extension d’alias Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="4a33f-103">The Azure CLI 2.0 alias extension</span></span>

<span data-ttu-id="4a33f-104">L’extension d’alias permet aux utilisateurs de définir des commandes personnalisées pour l’interface Azure CLI, à l’aide des commandes existantes.</span><span class="sxs-lookup"><span data-stu-id="4a33f-104">The alias extension allows users to define custom commands for the Azure CLI by using existing commands.</span></span> <span data-ttu-id="4a33f-105">Avec les alias, votre workflow demeure concis et simple grâce aux raccourcis. De plus, vous être en mesure de recourir à des arguments positionnels.</span><span class="sxs-lookup"><span data-stu-id="4a33f-105">Aliases help keep your workflow concise and simple by allowing shortcuts and giving you the ability to use positional arguments.</span></span> <span data-ttu-id="4a33f-106">Comme les alias sont alimentés par le moteur de modèles Jinja2, ils prennent bien souvent en charge le traitement avancé des arguments.</span><span class="sxs-lookup"><span data-stu-id="4a33f-106">Since aliases are powered by the Jinja2 template engine, they even offer advanced argument processing.</span></span>

> [!NOTE]
> <span data-ttu-id="4a33f-107">L’extension d’alias est en préversion publique.</span><span class="sxs-lookup"><span data-stu-id="4a33f-107">The Alias Extension is in public preview.</span></span> <span data-ttu-id="4a33f-108">Les fonctionnalités et le format du fichier de configuration peuvent changer.</span><span class="sxs-lookup"><span data-stu-id="4a33f-108">The features and configuration file format may change.</span></span>

## <a name="install-the-alias-extension"></a><span data-ttu-id="4a33f-109">Installer l’extension d’alias</span><span class="sxs-lookup"><span data-stu-id="4a33f-109">Install the alias extension</span></span>

<span data-ttu-id="4a33f-110">La version minimale requise de l’interface Azure CLI pour utiliser l’extension d’alias est **2.0.28**.</span><span class="sxs-lookup"><span data-stu-id="4a33f-110">The minimum required Azure CLI version to use the alias extension is **2.0.28**.</span></span> <span data-ttu-id="4a33f-111">Pour vérifier votre version de l’interface CLI, exécutez `az --version`.</span><span class="sxs-lookup"><span data-stu-id="4a33f-111">To check your CLI version, run `az --version`.</span></span> <span data-ttu-id="4a33f-112">Si vous devez mettre à jour votre installation, suivez les instructions de la section [Installer Azure CLI 2.0](./install-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="4a33f-112">If you need to update your installation,  follow the instructions in [Install the Azure CLI 2.0](./install-azure-cli.md).</span></span>

<span data-ttu-id="4a33f-113">Installez l’extension avec la commande [az extension add](/cli/azure/extension#az-extension-add).</span><span class="sxs-lookup"><span data-stu-id="4a33f-113">Install the extension with the [az extension add](/cli/azure/extension#az-extension-add) command.</span></span>

```azurecli
az extension add --name alias
```

<span data-ttu-id="4a33f-114">Vérifiez l’installation de l’extension avec [az extension list](/cli/azure/extension#az-extension-list).</span><span class="sxs-lookup"><span data-stu-id="4a33f-114">Verify the installation of the extension with [az extension list](/cli/azure/extension#az-extension-list).</span></span> <span data-ttu-id="4a33f-115">Si l’extension d’alias a été correctement installée, elle est répertoriée dans la sortie de la commande.</span><span class="sxs-lookup"><span data-stu-id="4a33f-115">If the alias extension was installed properly, it's listed in the command output.</span></span>

```azurecli
az extension list --output table
```

```output
ExtensionType    Name                       Version
---------------  -------------------------  ---------
whl              alias                      0.2.0
```

## <a name="keep-the-extension-up-to-date"></a><span data-ttu-id="4a33f-116">Maintenir l’extension à jour</span><span class="sxs-lookup"><span data-stu-id="4a33f-116">Keep the extension up to date</span></span>

<span data-ttu-id="4a33f-117">L’extension d’alias est en cours de développement actif ; de nouvelles versions sont régulièrement publiées.</span><span class="sxs-lookup"><span data-stu-id="4a33f-117">The alias extension is under active development and new versions are released regularly.</span></span> <span data-ttu-id="4a33f-118">Ces nouvelles versions ne sont pas automatiquement installées lors des mises à jour de l’interface CLI.</span><span class="sxs-lookup"><span data-stu-id="4a33f-118">New versions are not automatically installed whenever you update the CLI.</span></span> <span data-ttu-id="4a33f-119">Installez les mises à jour de l’extension avec [az extension update](/cli/azure/extension#az-extension-update).</span><span class="sxs-lookup"><span data-stu-id="4a33f-119">Install the updates for the extension with [az extension update](/cli/azure/extension#az-extension-update).</span></span>

```azurecli
az extension update --name alias
```

## <a name="alias-commands-file-format"></a><span data-ttu-id="4a33f-120">Format de fichier des commandes alias</span><span class="sxs-lookup"><span data-stu-id="4a33f-120">Alias commands file format</span></span>

<span data-ttu-id="4a33f-121">Les définitions des commandes alias sont consignées dans un fichier de configuration, qui se situe sur `$AZURE_USER_CONFIG/alias`.</span><span class="sxs-lookup"><span data-stu-id="4a33f-121">Alias command definitions are written into a configuration file, located at `$AZURE_USER_CONFIG/alias`.</span></span> <span data-ttu-id="4a33f-122">La valeur par défaut de `AZURE_USER_CONFIG` est `$HOME/.azure` sous macOS et Linux, et `%USERPROFILE%\.azure` sous Windows.</span><span class="sxs-lookup"><span data-stu-id="4a33f-122">The default value of `AZURE_USER_CONFIG` is `$HOME/.azure` on macOS and Linux, and `%USERPROFILE%\.azure` on Windows.</span></span> <span data-ttu-id="4a33f-123">Le fichier de configuration d’alias est consigné au format du fichier de configuration INI.</span><span class="sxs-lookup"><span data-stu-id="4a33f-123">The alias configuration file is written in the INI configuration file format.</span></span> <span data-ttu-id="4a33f-124">Le format général des commandes alias est le suivant :</span><span class="sxs-lookup"><span data-stu-id="4a33f-124">The general format for alias commands is:</span></span>

```
[command_name]
command = invoked_commands
```

<span data-ttu-id="4a33f-125">N’incluez pas `az` dans la commande.</span><span class="sxs-lookup"><span data-stu-id="4a33f-125">Don't include `az` as part of the command.</span></span>

## <a name="create-simple-alias-commands"></a><span data-ttu-id="4a33f-126">Créer des commandes alias simples</span><span class="sxs-lookup"><span data-stu-id="4a33f-126">Create simple alias commands</span></span>

<span data-ttu-id="4a33f-127">Les alias peuvent par exemple servir à raccourcir les noms existants des groupes de commandes ou des commandes.</span><span class="sxs-lookup"><span data-stu-id="4a33f-127">One use of aliases is for shortening existing command groups or command names.</span></span> <span data-ttu-id="4a33f-128">Par exemple, vous pouvez raccourcir le nom du groupe de commandes `group` en le ramenant à `rg` et le nom de la commande `list` en `ls`.</span><span class="sxs-lookup"><span data-stu-id="4a33f-128">For example, you can shorten the `group` command group to `rg` and the `list` command to `ls`.</span></span>

```
[rg]
command = group

[ls]
command = list
```

<span data-ttu-id="4a33f-129">Ces alias nouvellement définis peuvent désormais être utilisés dans l’ensemble des emplacements pouvant héberger leur définition.</span><span class="sxs-lookup"><span data-stu-id="4a33f-129">These newly defined aliases can now be used anywhere that their definition would be.</span></span>

```azurecli
az rg list
az rg ls
az vm ls
```

<span data-ttu-id="4a33f-130">Les alias peuvent également être des raccourcis de commandes complètes.</span><span class="sxs-lookup"><span data-stu-id="4a33f-130">Aliases can also be shortcuts for complete commands.</span></span> <span data-ttu-id="4a33f-131">Le prochain exemple répertorie les groupes de ressources disponibles et leur emplacement dans la sortie de table :</span><span class="sxs-lookup"><span data-stu-id="4a33f-131">The next example lists available resource groups and their locations in table output:</span></span>

```
[ls-groups]
command = group list --query '[].{Name:name, Location:location}' --output table
```

<span data-ttu-id="4a33f-132">Désormais, `ls-groups` peut être exécutée comme toute autre commande CLI.</span><span class="sxs-lookup"><span data-stu-id="4a33f-132">Now `ls-groups` can be run like any other CLI command.</span></span>

```azurecli
az ls-groups
```

## <a name="create-an-alias-command-with-arguments"></a><span data-ttu-id="4a33f-133">Créer une commande d’alias avec des arguments</span><span class="sxs-lookup"><span data-stu-id="4a33f-133">Create an alias command with arguments</span></span>

<span data-ttu-id="4a33f-134">Il est également possible d’ajouter des arguments positionnels à une commande d’alias en les incluant en tant que `{{ arg_name }}` dans le nom d’alias.</span><span class="sxs-lookup"><span data-stu-id="4a33f-134">You can also add positional arguments to an alias command by including them as `{{ arg_name }}` in the alias name.</span></span> <span data-ttu-id="4a33f-135">L’espace à l’intérieur des accolades est requis.</span><span class="sxs-lookup"><span data-stu-id="4a33f-135">The whitespace inside the curly braces is required.</span></span>

```
[alias_name {{ arg1 }} {{ arg2 }} ...]
command = invoke_including_args
```

<span data-ttu-id="4a33f-136">Le prochain exemple d’alias indique comment utiliser des arguments positionnels afin de récupérer l’adresse IP publique d’une machine virtuelle.</span><span class="sxs-lookup"><span data-stu-id="4a33f-136">The next example alias shows how to use positional arguments to get the public IP address for a VM.</span></span>

```
[get-vm-ip {{ resourceGroup }} {{ vmName }}]
command = vm list-ip-addresses --resource-group {{ resourceGroup }} --name {{ vmName }} --query [0].virtualMachine.network.publicIpAddresses[0].ipAddress
```

<span data-ttu-id="4a33f-137">Lorsque vous exécutez cette commande, vous octroyez des valeurs aux arguments positionnels.</span><span class="sxs-lookup"><span data-stu-id="4a33f-137">When running this command, you give values to the positional arguments.</span></span>

```azruecli
az get-vm-ip MyResourceGroup MyVM
```

<span data-ttu-id="4a33f-138">Vous pouvez également utiliser des variables d’environnement dans les commandes appelées par alias, qui sont évaluées au moment de l’exécution.</span><span class="sxs-lookup"><span data-stu-id="4a33f-138">You can also use environment variables in commands invoked by aliases, which are evaluated at runtime.</span></span> <span data-ttu-id="4a33f-139">Le prochain exemple ajoute l’alias `create-rg`, qui crée un groupe de ressources dans `eastus` et ajoute une balise `owner`.</span><span class="sxs-lookup"><span data-stu-id="4a33f-139">The next example adds the `create-rg` alias, which creates a resource group in `eastus` and adds an `owner` tag.</span></span> <span data-ttu-id="4a33f-140">Cette balise se voit affecter la valeur de la variable d’environnement local `USER`.</span><span class="sxs-lookup"><span data-stu-id="4a33f-140">This tag is assigned the value of the local environment variable `USER`.</span></span>

```
[create-rg {{ groupName }}]
command = group create --name {{ groupName }} --location eastus --tags owner=$USER
```

## <a name="process-arguments-using-jinja2-templates"></a><span data-ttu-id="4a33f-141">Traiter les arguments à l’aide des modèles Jinja2</span><span class="sxs-lookup"><span data-stu-id="4a33f-141">Process arguments using Jinja2 templates</span></span>

<span data-ttu-id="4a33f-142">La substitution d’argument dans l’extension d’alias est effectuée par [Jinja2](http://jinja.pocoo.org/docs/2.10/), ce qui vous donne un accès illimité aux fonctionnalités du moteur de modèles Jinja2.</span><span class="sxs-lookup"><span data-stu-id="4a33f-142">Argument substitution in the alias extension is performed by [Jinja2](http://jinja.pocoo.org/docs/2.10/), giving you full access to the capabilities of the Jinja2 template engine.</span></span> <span data-ttu-id="4a33f-143">Les modèles prennent en charge différentes actions, comme l’extraction et la substitution des données sur les chaînes.</span><span class="sxs-lookup"><span data-stu-id="4a33f-143">Templates allow you to perform actions like data extraction and substitution on strings.</span></span>

<span data-ttu-id="4a33f-144">Avec les modèles Jinja2, vous pouvez écrire des alias qui acceptent des types d’arguments supplémentaires par rapport à la commande sous-jacente.</span><span class="sxs-lookup"><span data-stu-id="4a33f-144">With Jinja2 templates, you can write aliases which take different types of arguments than the underlying command.</span></span> <span data-ttu-id="4a33f-145">Par exemple, vous pouvez développer un alias acceptant une URL de stockage.</span><span class="sxs-lookup"><span data-stu-id="4a33f-145">For example, you can make an alias which takes a storage URL.</span></span> <span data-ttu-id="4a33f-146">Par la suite, cette URL est analysée afin de transmettre les noms de compte et de conteneur à la commande de stockage.</span><span class="sxs-lookup"><span data-stu-id="4a33f-146">Then this URL is parsed to pass the account and container names to the storage command.</span></span>

```
[storage-ls {{ url }}]
command = storage blob list --account-name {{ url.replace('https://', '').split('.')[0] }} --container-name {{ url.replace('https://', '').split('/')[1] }}
```

<span data-ttu-id="4a33f-147">Pour en savoir plus sur le moteur de modèles Jinja2, consultez la [documentation Jinja2](http://jinja.pocoo.org/docs/2.10/templates/).</span><span class="sxs-lookup"><span data-stu-id="4a33f-147">To learn about the Jinja2 template engine, see [the Jinja2 documentation](http://jinja.pocoo.org/docs/2.10/templates/).</span></span>

## <a name="uninstall-the-alias-extension"></a><span data-ttu-id="4a33f-148">Désinstaller l’extension d’alias</span><span class="sxs-lookup"><span data-stu-id="4a33f-148">Uninstall the alias extension</span></span>

<span data-ttu-id="4a33f-149">Pour désinstaller l’extension, utilisez la commande [az extension remove](/cli/azure/extension#az-extension-remove).</span><span class="sxs-lookup"><span data-stu-id="4a33f-149">To uninstall the extension, use the [az extension remove](/cli/azure/extension#az-extension-remove) command.</span></span>

```bash
az extension remove --name alias
```

<span data-ttu-id="4a33f-150">Si vous procédez à la désinstallation en raison d’un bogue ou d’un problème lié à l’extension, veuillez [signaler un incident GitHub](https://github.com/Azure/azure-cli-extensions/issues) afin que nous puissions réfléchir à la correction.</span><span class="sxs-lookup"><span data-stu-id="4a33f-150">If you uninstalled due to a bug or other problem with the extension, please [file a GitHub issue](https://github.com/Azure/azure-cli-extensions/issues) so that we can provide a fix.</span></span>
