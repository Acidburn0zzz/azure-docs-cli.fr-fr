---
title: Extensions Azure CLI 2.0
description: "Utilisation d’extensions avec Azure CLI 2.0"
keywords: Azure CLI, extensions
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 02/13/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 548c06c64cc98598a2bd24bcc5959e59bffb4930
ms.sourcegitcommit: b93a19222e116d5880bbe64c03507c64e190331e
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/15/2018
---
# <a name="using-extensions-with-the-azure-cli-20"></a><span data-ttu-id="3d321-104">Utilisation d’extensions avec Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="3d321-104">Using extensions with the Azure CLI 2.0</span></span>

<span data-ttu-id="3d321-105">Les extensions sont des modules individuels non fournis avec Azure CLI, qui ajoutent des fonctionnalités via de nouvelles commandes.</span><span class="sxs-lookup"><span data-stu-id="3d321-105">Extensions are individual modules not shipped with the Azure CLI itself that add functionality through new commands.</span></span> <span data-ttu-id="3d321-106">Il peut s’agir d’offres expérimentales ou en version préliminaire, d’outils spécialisés de Microsoft, ou de fonctionnalités personnalisées que vous écrivez vous-même.</span><span class="sxs-lookup"><span data-stu-id="3d321-106">These might be experimental or pre-release offerings, specialized tools from Microsoft, or custom features you write yourself.</span></span> <span data-ttu-id="3d321-107">Les extensions vous offrent un certain degré de flexibilité avec la CLI, ce qui vous permet de la modifier en fonction de vos besoins, sans avoir à fournir de nombreux packages supplémentaires n’étant pas considérés comme composants de l’ensemble de fonctionnalités principal.</span><span class="sxs-lookup"><span data-stu-id="3d321-107">Extensions allow for a degree of flexibility with the CLI that let you modify it to your own needs, without having to ship a lot of additional packages that aren't considered part of the core feature set.</span></span>

<span data-ttu-id="3d321-108">Cet article va vous aider à comprendre comment installer, mettre à jour et supprimer des extensions pour l’interface CLI.</span><span class="sxs-lookup"><span data-stu-id="3d321-108">This article helps you understand how to install, update, and remove extensions for the CLI.</span></span> <span data-ttu-id="3d321-109">Il doit également apporter des réponses à des questions courantes sur le comportement des extensions.</span><span class="sxs-lookup"><span data-stu-id="3d321-109">It should also answer common questions about extension behavior.</span></span>

## <a name="finding-extensions"></a><span data-ttu-id="3d321-110">Recherche d’extensions</span><span class="sxs-lookup"><span data-stu-id="3d321-110">Finding extensions</span></span>

<span data-ttu-id="3d321-111">Pour savoir quelles sont les extensions disponibles, vous pouvez utiliser la commande [az extension list-available](/cli/azure/extension?view=azure-cli-latest#az_extension_list_available).</span><span class="sxs-lookup"><span data-stu-id="3d321-111">In order to know what extensions are available, you can use [az extension list-available](/cli/azure/extension?view=azure-cli-latest#az_extension_list_available).</span></span> <span data-ttu-id="3d321-112">Cette commande répertorie les extensions officielles et disponibles qui sont fournies et prises en charge par Microsoft.</span><span class="sxs-lookup"><span data-stu-id="3d321-112">This command lists the available, official extensions which are provided and supported by Microsoft.</span></span>

## <a name="installing-extensions"></a><span data-ttu-id="3d321-113">Installation des extensions</span><span class="sxs-lookup"><span data-stu-id="3d321-113">Installing extensions</span></span>

<span data-ttu-id="3d321-114">Une fois que vous avez trouvé une extension à installer, utilisez la commande [az extension add](https://docs.microsoft.com/en-us/cli/azure/extension?view=azure-cli-latest#az_extension_add) pour l’obtenir.</span><span class="sxs-lookup"><span data-stu-id="3d321-114">Once you have found an extension to install, use [az extension add](https://docs.microsoft.com/en-us/cli/azure/extension?view=azure-cli-latest#az_extension_add) to get it.</span></span> <span data-ttu-id="3d321-115">Si l’extension est répertoriée dans `az extension list-available`, vous pouvez installer l’extension par nom.</span><span class="sxs-lookup"><span data-stu-id="3d321-115">If the extension is listed in `az extension list-available`, you can install the extension by name.</span></span>

```azurecli
az extension add --name <extension-name>
```

<span data-ttu-id="3d321-116">Si l’extension provient d’une ressource externe ou si vous avez un lien direct vers celle-ci, vous pouvez fournir le chemin d’accès local ou l’URL source.</span><span class="sxs-lookup"><span data-stu-id="3d321-116">If the extension is from an external resource or you have a direct link to it, you can provide the source URL or local path.</span></span> <span data-ttu-id="3d321-117">Cela _doit_ être un fichier Wheel Python compilé.</span><span class="sxs-lookup"><span data-stu-id="3d321-117">This _must_ be a compiled Python wheel file.</span></span>

```azurecli
az extension add --source <URL-or-path>
```

<span data-ttu-id="3d321-118">Une fois qu’une extension est installée, elle se trouve sous la valeur de la variable d’interpréteur de commandes `$AZURE_EXTENSION_DIR`.</span><span class="sxs-lookup"><span data-stu-id="3d321-118">Once an extension is installed, it can be found under the value of the `$AZURE_EXTENSION_DIR` shell variable.</span></span> <span data-ttu-id="3d321-119">Si cette variable n’est pas définie, par défaut la valeur est `$HOME/.azure/cliextensions` sur Linux et macOS, et `%USERPROFILE%\.azure\cliextensions` sur Windows.</span><span class="sxs-lookup"><span data-stu-id="3d321-119">If this variable is unset, by default the value is `$HOME/.azure/cliextensions` on Linux and macOS, and `%USERPROFILE%\.azure\cliextensions` on Windows.</span></span>

## <a name="updating-extensions"></a><span data-ttu-id="3d321-120">Mise à jour des extensions</span><span class="sxs-lookup"><span data-stu-id="3d321-120">Updating extensions</span></span>

<span data-ttu-id="3d321-121">Les extensions ne peuvent être mises à jour que par nom, à l’aide de la commande [az extension update](https://docs.microsoft.com/en-us/cli/azure/extension?view=azure-cli-latest#az_extension_update).</span><span class="sxs-lookup"><span data-stu-id="3d321-121">Extensions can only be updated by name, using [az extension update](https://docs.microsoft.com/en-us/cli/azure/extension?view=azure-cli-latest#az_extension_update).</span></span>

```azurecli
az extension update --name <extension-name>
```

<span data-ttu-id="3d321-122">Si le nom d’une extension ne peut pas être résolu par la CLI pour une raison quelconque, réinstallez l’extension pour la mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="3d321-122">If an extension name cannot be resolved by the CLI for whatever reason, reinstall the extension to update it.</span></span> <span data-ttu-id="3d321-123">Il est également possible que l’extension ne soit plus en préversion, mais qu’elle soit devenue une commande intégrée de la CLI.</span><span class="sxs-lookup"><span data-stu-id="3d321-123">There is also the possibility that the extension was moved out of preview and became a built-in command for the CLI.</span></span> <span data-ttu-id="3d321-124">Dans ce cas, mettez la CLI à jour et désinstallez l’extension.</span><span class="sxs-lookup"><span data-stu-id="3d321-124">In that case, update the CLI and uninstall the extension.</span></span>

## <a name="uninstalling-extensions"></a><span data-ttu-id="3d321-125">Désinstallation des extensions</span><span class="sxs-lookup"><span data-stu-id="3d321-125">Uninstalling extensions</span></span>

<span data-ttu-id="3d321-126">Si vous n’avez plus besoin d’une extension, elle peut être supprimée avec la commande [az extension remove](https://docs.microsoft.com/en-us/cli/azure/extension?view=azure-cli-latest#az_extension_remove).</span><span class="sxs-lookup"><span data-stu-id="3d321-126">If you no longer need an extension, it can be removed with [az extension remove](https://docs.microsoft.com/en-us/cli/azure/extension?view=azure-cli-latest#az_extension_remove).</span></span>

```azurecli
az extension remove --name <extension-name>
```

<span data-ttu-id="3d321-127">Vous pouvez également supprimer une extension manuellement en la supprimant de l’emplacement où elle a été installée.</span><span class="sxs-lookup"><span data-stu-id="3d321-127">You can also remove an extension manually by deleting it from the location where it was installed.</span></span> <span data-ttu-id="3d321-128">Il s’agit de la valeur de la variable d’interpréteur de commandes `$AZURE_EXTENSION_DIR`.</span><span class="sxs-lookup"><span data-stu-id="3d321-128">This will be the value of the `$AZURE_EXTENSION_DIR` shell variable.</span></span> <span data-ttu-id="3d321-129">Si cette variable n’est pas définie, par défaut la valeur est `$HOME/.azure/cliextensions` sur Linux et macOS, et `%USERPROFILE%\.azure\cliextensions` sur Windows.</span><span class="sxs-lookup"><span data-stu-id="3d321-129">If this variable is unset, by default the value is `$HOME/.azure/cliextensions` on Linux and macOS, and `%USERPROFILE%\.azure\cliextensions` on Windows.</span></span>

```bash
rm -rf $AZURE_EXTENSION_DIR/<extension-name>
```

<span data-ttu-id="3d321-130">Il est recommandé d’utiliser `az extension remove` pour les désinstallations.</span><span class="sxs-lookup"><span data-stu-id="3d321-130">It is recommended that you uninstall using `az extension remove`.</span></span>

## <a name="faq"></a><span data-ttu-id="3d321-131">Forum Aux Questions</span><span class="sxs-lookup"><span data-stu-id="3d321-131">FAQ</span></span>

<span data-ttu-id="3d321-132">Voici les réponses à d’autres questions courantes sur les extensions de CLI.</span><span class="sxs-lookup"><span data-stu-id="3d321-132">Here are some answers to other common questions about CLI extensions.</span></span>

### <a name="what-file-formats-are-allowed-for-installation"></a><span data-ttu-id="3d321-133">Quels sont les formats de fichiers autorisés pour l’installation ?</span><span class="sxs-lookup"><span data-stu-id="3d321-133">What file formats are allowed for installation?</span></span>

<span data-ttu-id="3d321-134">Actuellement, seuls les fichiers Wheel Python compilés peuvent être installés en tant qu’extensions.</span><span class="sxs-lookup"><span data-stu-id="3d321-134">Currently, only compiled Python wheels can be installed as extensions.</span></span>

### <a name="can-extensions-replace-existing-commands"></a><span data-ttu-id="3d321-135">Les extensions peuvent-elles remplacer des commandes existantes ?</span><span class="sxs-lookup"><span data-stu-id="3d321-135">Can extensions replace existing commands?</span></span>

<span data-ttu-id="3d321-136">Oui.</span><span class="sxs-lookup"><span data-stu-id="3d321-136">Yes.</span></span> <span data-ttu-id="3d321-137">Les extensions peuvent remplacer des commandes existantes, mais avant l’exécution d’une commande qui a été remplacée, la CLI émet un avertissement.</span><span class="sxs-lookup"><span data-stu-id="3d321-137">Extensions may replace existing commands, but before running a command that has been replaced the CLI will issue a warning.</span></span>

### <a name="how-can-i-tell-if-an-extension-is-in-pre-release"></a><span data-ttu-id="3d321-138">Comment puis-je savoir si une extension est en version préliminaire ?</span><span class="sxs-lookup"><span data-stu-id="3d321-138">How can I tell if an extension is in pre-release?</span></span>

<span data-ttu-id="3d321-139">La documentation et le contrôle de version d’une extension doivent indiquer si celle-ci est en version préliminaire.</span><span class="sxs-lookup"><span data-stu-id="3d321-139">An extension should indicate through its own documentation and versioning if it is in pre-release.</span></span> <span data-ttu-id="3d321-140">Il est également commun pour Microsoft de publier des commandes en préversion pour la CLI en tant qu’extensions, avec des plans pour les migrer dans l’interface CLI principale une fois que le produit n’est plus en préversion.</span><span class="sxs-lookup"><span data-stu-id="3d321-140">It is also common for Microsoft to release preview commands for the CLI as extensions, with plans to move them into the main CLI interface once the product is out of preview.</span></span>

### <a name="can-extensions-depend-upon-each-other"></a><span data-ttu-id="3d321-141">Les extensions peuvent-elles dépendre les unes des autres ?</span><span class="sxs-lookup"><span data-stu-id="3d321-141">Can extensions depend upon each other?</span></span>

<span data-ttu-id="3d321-142">Non.</span><span class="sxs-lookup"><span data-stu-id="3d321-142">No.</span></span> <span data-ttu-id="3d321-143">Les extensions doivent être des packages individuels qui ne reposent pas les uns sur les autres.</span><span class="sxs-lookup"><span data-stu-id="3d321-143">Extensions must be individual packages which do not rely on one another.</span></span> <span data-ttu-id="3d321-144">Cela s’explique par le fait que la CLI ne donne aucune garantie quant au moment où les extensions sont chargées, et ainsi le chargement des dépendances ne peut pas être garanti.</span><span class="sxs-lookup"><span data-stu-id="3d321-144">This is because the CLI gives no guarantee about when extensions are loaded, so dependencies could not be guaranteed to be satisfied.</span></span> <span data-ttu-id="3d321-145">En installant une extension, vous n’installez aucun autre élément, et celle-ci doit continuer à fonctionner même si vous supprimez d’autres extensions.</span><span class="sxs-lookup"><span data-stu-id="3d321-145">Installing an extension installs that extension only, and it should continue to work even if you remove other extensions.</span></span>

### <a name="are-extensions-updated-along-with-the-cli"></a><span data-ttu-id="3d321-146">Les extensions sont-elles mises à jour en même temps que la CLI ?</span><span class="sxs-lookup"><span data-stu-id="3d321-146">Are extensions updated along with the CLI?</span></span>

<span data-ttu-id="3d321-147">Non.</span><span class="sxs-lookup"><span data-stu-id="3d321-147">No.</span></span> <span data-ttu-id="3d321-148">Les extensions doivent être mises à jour séparément, comme décrit dans la section [Mise à jour des extensions](#updating-extensions).</span><span class="sxs-lookup"><span data-stu-id="3d321-148">Extensions must be updated separately, as described in the [Updating extensions](#updating-extensions) section.</span></span>
