---
title: Extensions Azure CLI
description: Utilisation d’extensions avec Azure CLI
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 09/07/2018
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 73488fc464ed052f22f071f6373fb6b8f682b778
ms.sourcegitcommit: 7caa6673f65e61deb8d6def6386e4eb9acdac923
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/28/2020
ms.locfileid: "77779990"
---
# <a name="use-extensions-with-azure-cli"></a><span data-ttu-id="3ac8e-103">Utilisez des extensions avec Azure CLI</span><span class="sxs-lookup"><span data-stu-id="3ac8e-103">Use extensions with Azure CLI</span></span> 

<span data-ttu-id="3ac8e-104">L’interface de ligne de commande Azure offre la possibilité de charger des extensions.</span><span class="sxs-lookup"><span data-stu-id="3ac8e-104">The Azure CLI offers the capability to load extensions.</span></span> <span data-ttu-id="3ac8e-105">Les extensions sont des roues Python qui ne sont pas fournies comme partie de la CLI mais qui sont exécutées en tant que commandes CLI.</span><span class="sxs-lookup"><span data-stu-id="3ac8e-105">Extensions are Python wheels that aren't shipped as part of the CLI but run as CLI commands.</span></span>
<span data-ttu-id="3ac8e-106">Avec les extensions, vous obtenez l’accès aux commandes expérimentales et préliminaires, ainsi que la capacité d’écrire vos propres interfaces CLI.</span><span class="sxs-lookup"><span data-stu-id="3ac8e-106">With extensions, you gain access to experimental and pre-release commands along with the ability to write your own CLI interfaces.</span></span> <span data-ttu-id="3ac8e-107">Cet article explique comment gérer les extensions et répond aux questions courantes concernant leur utilisation.</span><span class="sxs-lookup"><span data-stu-id="3ac8e-107">This article covers how to manage extensions and answers common questions about their use.</span></span>

## <a name="find-extensions"></a><span data-ttu-id="3ac8e-108">Rechercher des extensions</span><span class="sxs-lookup"><span data-stu-id="3ac8e-108">Find extensions</span></span>

<span data-ttu-id="3ac8e-109">Pour voir les extensions fournies et gérées par Microsoft, utiliser la commande [az extension list-available](/cli/azure/extension#az-extension-list-available).</span><span class="sxs-lookup"><span data-stu-id="3ac8e-109">To see the extensions provided and maintained by Microsoft, use the [az extension list-available](/cli/azure/extension#az-extension-list-available) command.</span></span>

```azurecli-interactive
az extension list-available --output table
```

<span data-ttu-id="3ac8e-110">Nous hébergeons également une [liste des extensions](azure-cli-extensions-list.md) sur le site de la documentation.</span><span class="sxs-lookup"><span data-stu-id="3ac8e-110">We also host a [list of extensions](azure-cli-extensions-list.md) on the documentation site.</span></span>

## <a name="install-extensions"></a><span data-ttu-id="3ac8e-111">Installer les extensions</span><span class="sxs-lookup"><span data-stu-id="3ac8e-111">Install extensions</span></span>

<span data-ttu-id="3ac8e-112">Une fois que vous avez trouvé une extension à installer, utilisez la commande [az extension add](https://docs.microsoft.com/cli/azure/extension#az-extension-add) pour l’obtenir.</span><span class="sxs-lookup"><span data-stu-id="3ac8e-112">Once you have found an extension to install, use [az extension add](https://docs.microsoft.com/cli/azure/extension#az-extension-add) to get it.</span></span> <span data-ttu-id="3ac8e-113">Si l’extension est répertoriée dans `az extension list-available`, vous pouvez installer l’extension par nom.</span><span class="sxs-lookup"><span data-stu-id="3ac8e-113">If the extension is listed in `az extension list-available`, you can install the extension by name.</span></span>

```azurecli-interactive
az extension add --name <extension-name>
```

<span data-ttu-id="3ac8e-114">Si l’extension provient d’une ressource externe ou si vous disposez d’un lien direct vers celle-ci, fournissez le chemin d’accès local ou l’URL source.</span><span class="sxs-lookup"><span data-stu-id="3ac8e-114">If the extension is from an external resource or you have a direct link to it, provide the source URL or local path.</span></span> <span data-ttu-id="3ac8e-115">L’extension _doit_ être un fichier de roue Python compilé.</span><span class="sxs-lookup"><span data-stu-id="3ac8e-115">The extension _must_ be a compiled Python wheel file.</span></span>

```azurecli-interactive
az extension add --source <URL-or-path>
```

<span data-ttu-id="3ac8e-116">Une fois qu’une extension est installée, elle se trouve sous la valeur de la variable d’interpréteur de commandes `$AZURE_EXTENSION_DIR`.</span><span class="sxs-lookup"><span data-stu-id="3ac8e-116">Once an extension is installed, it's found under the value of the `$AZURE_EXTENSION_DIR` shell variable.</span></span> <span data-ttu-id="3ac8e-117">Si cette variable n’est pas définie, par défaut la valeur est `$HOME/.azure/cliextensions` sur Linux et macOS, et `%USERPROFILE%\.azure\cliextensions` sur Windows.</span><span class="sxs-lookup"><span data-stu-id="3ac8e-117">If this variable is unset, by default the value is `$HOME/.azure/cliextensions` on Linux and macOS, and `%USERPROFILE%\.azure\cliextensions` on Windows.</span></span>

## <a name="update-extensions"></a><span data-ttu-id="3ac8e-118">Mettre à jour les extensions</span><span class="sxs-lookup"><span data-stu-id="3ac8e-118">Update extensions</span></span>

<span data-ttu-id="3ac8e-119">Si une extension a été installée par nom, mettez-la à jour à l’aide de la commande [az extension update](https://docs.microsoft.com/cli/azure/extension#az-extension-update).</span><span class="sxs-lookup"><span data-stu-id="3ac8e-119">If an extension was installed by name, update it using [az extension update](https://docs.microsoft.com/cli/azure/extension#az-extension-update).</span></span>

```azurecli-interactive
az extension update --name <extension-name>
```

<span data-ttu-id="3ac8e-120">Sinon, il est possible de mettre à jour une extension à partir de la source, en suivant les instructions de la section [Installer les extensions](#install-extensions).</span><span class="sxs-lookup"><span data-stu-id="3ac8e-120">Otherwise, an extension can be updated from source by following the [Install extensions](#install-extensions) instructions.</span></span>

<span data-ttu-id="3ac8e-121">Si un nom d’extension ne peut pas être résolu par l’interface CLI, désinstallez cette extension et tentez de procéder à une réinstallation.</span><span class="sxs-lookup"><span data-stu-id="3ac8e-121">If an extension name can't be resolved by the CLI, uninstall it and attempt to reinstall.</span></span> <span data-ttu-id="3ac8e-122">L’extension aurait également pu faire partie de l’interface CLI de base.</span><span class="sxs-lookup"><span data-stu-id="3ac8e-122">The extension could also have become part of the base CLI.</span></span>
<span data-ttu-id="3ac8e-123">Essayez de mettre à jour l’interface de ligne de commande en suivant les instructions de la section [Installer Azure CLI](install-azure-cli.md) et vérifiez que les commandes de l’extension ont été ajoutées.</span><span class="sxs-lookup"><span data-stu-id="3ac8e-123">Try updating the CLI as described in [Install the Azure CLI](install-azure-cli.md) and see if the extension's commands were added.</span></span>

## <a name="uninstall-extensions"></a><span data-ttu-id="3ac8e-124">Désinstaller les extensions</span><span class="sxs-lookup"><span data-stu-id="3ac8e-124">Uninstall extensions</span></span>

<span data-ttu-id="3ac8e-125">Si vous n’avez plus besoin d’une extension, vous pouvez la supprimer avec la commande [az extension remove](https://docs.microsoft.com/cli/azure/extension#az-extension-remove).</span><span class="sxs-lookup"><span data-stu-id="3ac8e-125">If you no longer need an extension, remove it with [az extension remove](https://docs.microsoft.com/cli/azure/extension#az-extension-remove).</span></span>

```azurecli-interactive
az extension remove --name <extension-name>
```

<span data-ttu-id="3ac8e-126">Vous pouvez également supprimer une extension manuellement en la supprimant de l’emplacement où elle a été installée.</span><span class="sxs-lookup"><span data-stu-id="3ac8e-126">You can also remove an extension manually by deleting it from the location where it was installed.</span></span> <span data-ttu-id="3ac8e-127">La variable d’interpréteur de commandes `$AZURE_EXTENSION_DIR` définit l’emplacement dans lequel sont installés les modules.</span><span class="sxs-lookup"><span data-stu-id="3ac8e-127">The `$AZURE_EXTENSION_DIR` shell variable defines where modules are installed.</span></span>
<span data-ttu-id="3ac8e-128">Si cette variable n’est pas définie, par défaut la valeur est `$HOME/.azure/cliextensions` sur Linux et macOS, et `%USERPROFILE%\.azure\cliextensions` sur Windows.</span><span class="sxs-lookup"><span data-stu-id="3ac8e-128">If this variable is unset, by default the value is `$HOME/.azure/cliextensions` on Linux and macOS, and `%USERPROFILE%\.azure\cliextensions` on Windows.</span></span>

```bash
rm -rf $AZURE_EXTENSION_DIR/<extension-name>
```

## <a name="faq"></a><span data-ttu-id="3ac8e-129">Questions fréquentes (FAQ)</span><span class="sxs-lookup"><span data-stu-id="3ac8e-129">FAQ</span></span>

<span data-ttu-id="3ac8e-130">Voici les réponses à d’autres questions courantes sur les extensions de CLI.</span><span class="sxs-lookup"><span data-stu-id="3ac8e-130">Here are some answers to other common questions about CLI extensions.</span></span>

### <a name="what-file-formats-are-allowed-for-installation"></a><span data-ttu-id="3ac8e-131">Quels sont les formats de fichiers autorisés pour l’installation ?</span><span class="sxs-lookup"><span data-stu-id="3ac8e-131">What file formats are allowed for installation?</span></span>

<span data-ttu-id="3ac8e-132">Actuellement, seuls les fichiers Wheel Python compilés peuvent être installés en tant qu’extensions.</span><span class="sxs-lookup"><span data-stu-id="3ac8e-132">Currently, only compiled Python wheels can be installed as extensions.</span></span>

### <a name="can-extensions-replace-existing-commands"></a><span data-ttu-id="3ac8e-133">Les extensions peuvent-elles remplacer des commandes existantes ?</span><span class="sxs-lookup"><span data-stu-id="3ac8e-133">Can extensions replace existing commands?</span></span>

<span data-ttu-id="3ac8e-134">Oui.</span><span class="sxs-lookup"><span data-stu-id="3ac8e-134">Yes.</span></span> <span data-ttu-id="3ac8e-135">Les extensions peuvent remplacer des commandes existantes, mais avant l’exécution d’une commande qui a été remplacée, la CLI émet un avertissement.</span><span class="sxs-lookup"><span data-stu-id="3ac8e-135">Extensions may replace existing commands, but before running a command that has been replaced the CLI will issue a warning.</span></span>

### <a name="how-can-i-tell-if-an-extension-is-in-pre-release"></a><span data-ttu-id="3ac8e-136">Comment puis-je savoir si une extension est en version préliminaire ?</span><span class="sxs-lookup"><span data-stu-id="3ac8e-136">How can I tell if an extension is in pre-release?</span></span>

<span data-ttu-id="3ac8e-137">Une documentation et un contrôle de version d’une extension s’afficheront si celle-ci est en version préliminaire.</span><span class="sxs-lookup"><span data-stu-id="3ac8e-137">An extension's documentation and versioning will show if it's in pre-release.</span></span> <span data-ttu-id="3ac8e-138">Microsoft publie souvent des préversions de commandes sous forme d’extensions CLI, avec la possibilité de les déplacer ultérieurement dans le produit principal de la CLI.</span><span class="sxs-lookup"><span data-stu-id="3ac8e-138">Microsoft often releases preview commands as CLI extensions, with the option of moving them into the main CLI product later.</span></span> <span data-ttu-id="3ac8e-139">Lorsque les commandes sont déplacées en dehors des extensions, vous devez désinstaller l’ancienne extension.</span><span class="sxs-lookup"><span data-stu-id="3ac8e-139">When commands are moved out of extensions, the old extension should be uninstalled.</span></span> 

### <a name="can-extensions-depend-upon-each-other"></a><span data-ttu-id="3ac8e-140">Les extensions peuvent-elles dépendre les unes des autres ?</span><span class="sxs-lookup"><span data-stu-id="3ac8e-140">Can extensions depend upon each other?</span></span>

<span data-ttu-id="3ac8e-141">Non.</span><span class="sxs-lookup"><span data-stu-id="3ac8e-141">No.</span></span> <span data-ttu-id="3ac8e-142">Étant donné que l’interface CLI ne garantit pas un ordre de chargement, les dépendances peuvent ne pas être satisfaites.</span><span class="sxs-lookup"><span data-stu-id="3ac8e-142">Since the CLI doesn't guarantee a load order, dependencies might not be satisfied.</span></span> <span data-ttu-id="3ac8e-143">La suppression d’une extension n’affecte pas les autres.</span><span class="sxs-lookup"><span data-stu-id="3ac8e-143">Removing an extension won't affect any others.</span></span>

### <a name="are-extensions-updated-along-with-the-cli"></a><span data-ttu-id="3ac8e-144">Les extensions sont-elles mises à jour en même temps que la CLI ?</span><span class="sxs-lookup"><span data-stu-id="3ac8e-144">Are extensions updated along with the CLI?</span></span>

<span data-ttu-id="3ac8e-145">Non.</span><span class="sxs-lookup"><span data-stu-id="3ac8e-145">No.</span></span> <span data-ttu-id="3ac8e-146">Les extensions sont à mettre à jour séparément, comme décrit dans la section [Mettre à jour les extensions](#update-extensions).</span><span class="sxs-lookup"><span data-stu-id="3ac8e-146">Extensions must be updated separately, as described in [Update extensions](#update-extensions).</span></span>

### <a name="how-to-develop-our-own-extension"></a><span data-ttu-id="3ac8e-147">Comment développer votre propre extension ?</span><span class="sxs-lookup"><span data-stu-id="3ac8e-147">How to develop our own extension?</span></span>
<span data-ttu-id="3ac8e-148">Pour obtenir de l’aide, reportez-vous au dépôt officiel.</span><span class="sxs-lookup"><span data-stu-id="3ac8e-148">Please refer to the official repository for more help.</span></span> [<span data-ttu-id="3ac8e-149">Azure/azure-cli-extensions</span><span class="sxs-lookup"><span data-stu-id="3ac8e-149">Azure/azure-cli-extensions</span></span>](https://github.com/Azure/azure-cli/tree/master/doc/extensions)
