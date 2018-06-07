---
title: Extensions Azure CLI 2.0
description: Utilisation d’extensions avec Azure CLI 2.0
keywords: Azure CLI, extensions
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/16/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 1b983faef4c1678763b3483192e94a6c96e24f32
ms.sourcegitcommit: 80189ff103c91f8c47ab8ebf586df815fff5dd5d
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/07/2018
ms.locfileid: "34479470"
---
# <a name="using-extensions-with-the-azure-cli-20"></a><span data-ttu-id="2ad1f-104">Utilisation d’extensions avec Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="2ad1f-104">Using extensions with the Azure CLI 2.0</span></span>

<span data-ttu-id="2ad1f-105">Les extensions sont des modules individuels non fournis avec Azure CLI, qui ajoutent des fonctionnalités via de nouvelles commandes.</span><span class="sxs-lookup"><span data-stu-id="2ad1f-105">Extensions are individual modules not shipped with the Azure CLI itself that add functionality through new commands.</span></span> <span data-ttu-id="2ad1f-106">Il peut s’agir d’offres expérimentales ou en version préliminaire, d’outils spécialisés de Microsoft, ou de fonctionnalités personnalisées que vous écrivez vous-même.</span><span class="sxs-lookup"><span data-stu-id="2ad1f-106">These might be experimental or pre-release offerings, specialized tools from Microsoft, or custom features you write yourself.</span></span> <span data-ttu-id="2ad1f-107">Les extensions vous offrent un certain degré de flexibilité avec la CLI, ce qui vous permet de la modifier en fonction de vos besoins, sans avoir à fournir de nombreux packages supplémentaires n’étant pas considérés comme composants de l’ensemble de fonctionnalités principal.</span><span class="sxs-lookup"><span data-stu-id="2ad1f-107">Extensions allow for a degree of flexibility with the CLI that let you modify it to your own needs, without having to ship a lot of additional packages that aren't considered part of the core feature set.</span></span>

<span data-ttu-id="2ad1f-108">Cet article va vous aider à comprendre comment installer, mettre à jour et supprimer des extensions pour l’interface CLI.</span><span class="sxs-lookup"><span data-stu-id="2ad1f-108">This article helps you understand how to install, update, and remove extensions for the CLI.</span></span> <span data-ttu-id="2ad1f-109">Il répond également à des questions courantes sur le comportement des extensions.</span><span class="sxs-lookup"><span data-stu-id="2ad1f-109">It also answers common questions about extension behavior.</span></span>

## <a name="find-extensions"></a><span data-ttu-id="2ad1f-110">Rechercher des extensions</span><span class="sxs-lookup"><span data-stu-id="2ad1f-110">Find extensions</span></span>

<span data-ttu-id="2ad1f-111">Pour savoir quelles sont les extensions disponibles, vous pouvez utiliser la commande [az extension list-available](/cli/azure/extension#az-extension-list-available).</span><span class="sxs-lookup"><span data-stu-id="2ad1f-111">In order to know what extensions are available, you can use [az extension list-available](/cli/azure/extension#az-extension-list-available).</span></span> <span data-ttu-id="2ad1f-112">Cette commande répertorie les extensions officielles fournies et gérées par Microsoft.</span><span class="sxs-lookup"><span data-stu-id="2ad1f-112">This command lists the official extensions provided and maintained by Microsoft.</span></span>

```azurecli-interactive
az extension list-available --output table
```

<span data-ttu-id="2ad1f-113">Nous hébergeons également une [liste des extensions Microsoft](azure-cli-extensions-list.md) sur le site de la documentation.</span><span class="sxs-lookup"><span data-stu-id="2ad1f-113">We also host a [list of Microsoft extensions](azure-cli-extensions-list.md) on the documentation site.</span></span>

## <a name="install-extensions"></a><span data-ttu-id="2ad1f-114">Installer les extensions</span><span class="sxs-lookup"><span data-stu-id="2ad1f-114">Install extensions</span></span>

<span data-ttu-id="2ad1f-115">Une fois que vous avez trouvé une extension à installer, utilisez la commande [az extension add](https://docs.microsoft.com/cli/azure/extension#az-extension-add) pour l’obtenir.</span><span class="sxs-lookup"><span data-stu-id="2ad1f-115">Once you have found an extension to install, use [az extension add](https://docs.microsoft.com/cli/azure/extension#az-extension-add) to get it.</span></span> <span data-ttu-id="2ad1f-116">Si l’extension est répertoriée dans `az extension list-available`, vous pouvez installer l’extension par nom.</span><span class="sxs-lookup"><span data-stu-id="2ad1f-116">If the extension is listed in `az extension list-available`, you can install the extension by name.</span></span>

```azurecli-interactive
az extension add --name <extension-name>
```

<span data-ttu-id="2ad1f-117">Si l’extension provient d’une ressource externe ou si vous avez un lien direct vers celle-ci, vous pouvez fournir le chemin d’accès local ou l’URL source.</span><span class="sxs-lookup"><span data-stu-id="2ad1f-117">If the extension is from an external resource or you have a direct link to it, you can provide the source URL or local path.</span></span> <span data-ttu-id="2ad1f-118">Cela _doit_ être un fichier Wheel Python compilé.</span><span class="sxs-lookup"><span data-stu-id="2ad1f-118">This _must_ be a compiled Python wheel file.</span></span>

```azurecli-interactive
az extension add --source <URL-or-path>
```

<span data-ttu-id="2ad1f-119">Une fois qu’une extension est installée, elle se trouve sous la valeur de la variable d’interpréteur de commandes `$AZURE_EXTENSION_DIR`.</span><span class="sxs-lookup"><span data-stu-id="2ad1f-119">Once an extension is installed, it can be found under the value of the `$AZURE_EXTENSION_DIR` shell variable.</span></span> <span data-ttu-id="2ad1f-120">Si cette variable n’est pas définie, par défaut la valeur est `$HOME/.azure/cliextensions` sur Linux et macOS, et `%USERPROFILE%\.azure\cliextensions` sur Windows.</span><span class="sxs-lookup"><span data-stu-id="2ad1f-120">If this variable is unset, by default the value is `$HOME/.azure/cliextensions` on Linux and macOS, and `%USERPROFILE%\.azure\cliextensions` on Windows.</span></span>

## <a name="update-extensions"></a><span data-ttu-id="2ad1f-121">Mettre à jour les extensions</span><span class="sxs-lookup"><span data-stu-id="2ad1f-121">Update extensions</span></span>

<span data-ttu-id="2ad1f-122">Si une extension a été installée par nom, elle peut être mise à jour à l’aide de la commande [az extension update](https://docs.microsoft.com/cli/azure/extension#az-extension-update).</span><span class="sxs-lookup"><span data-stu-id="2ad1f-122">If an extension was installed by name, it can be updated using [az extension update](https://docs.microsoft.com/cli/azure/extension#az-extension-update).</span></span>

```azurecli-interactive
az extension update --name <extension-name>
```

<span data-ttu-id="2ad1f-123">Sinon, il est possible de mettre à jour une extension à partir de la source, en suivant les instructions de la section [Installer les extensions](#install-extensions).</span><span class="sxs-lookup"><span data-stu-id="2ad1f-123">Otherwise, an extension can be updated from source by following the [Install extensions](#install-extensions) instructions.</span></span>

<span data-ttu-id="2ad1f-124">Si un nom d’extension ne peut pas être résolu par l’interface CLI, désinstallez-la et tentez de procéder à une réinstallation.</span><span class="sxs-lookup"><span data-stu-id="2ad1f-124">If an extension name cannot be resolved by the CLI, uninstall it and attempt to reinstall.</span></span> <span data-ttu-id="2ad1f-125">Il est également possible que l’extension ait été déplacée de la version préliminaire pour devenir une commande intégrée pour l’interface CLI.</span><span class="sxs-lookup"><span data-stu-id="2ad1f-125">There's also the possibility that the extension was moved out of preview and became a built-in command for the CLI.</span></span> <span data-ttu-id="2ad1f-126">Tentez de mettre à jour l’interface CLI en suivant les instructions de la section [Installer Azure CLI 2.0](install-azure-cli.md) et observez si les commandes de l’extension ont été ajoutées.</span><span class="sxs-lookup"><span data-stu-id="2ad1f-126">Try updating the CLI as described in [Install the Azure CLI 2.0](install-azure-cli.md) and see if the extension's commands were added.</span></span> 

## <a name="uninstall-extensions"></a><span data-ttu-id="2ad1f-127">Désinstaller les extensions</span><span class="sxs-lookup"><span data-stu-id="2ad1f-127">Uninstall extensions</span></span>

<span data-ttu-id="2ad1f-128">Si vous n’avez plus besoin d’une extension, elle peut être supprimée avec la commande [az extension remove](https://docs.microsoft.com/cli/azure/extension#az-extension-remove).</span><span class="sxs-lookup"><span data-stu-id="2ad1f-128">If you no longer need an extension, it can be removed with [az extension remove](https://docs.microsoft.com/cli/azure/extension#az-extension-remove).</span></span>

```azurecli-interactive
az extension remove --name <extension-name>
```

<span data-ttu-id="2ad1f-129">Vous pouvez également supprimer une extension manuellement en la supprimant de l’emplacement où elle a été installée.</span><span class="sxs-lookup"><span data-stu-id="2ad1f-129">You can also remove an extension manually by deleting it from the location where it was installed.</span></span> <span data-ttu-id="2ad1f-130">Il s’agit de la valeur de la variable d’interpréteur de commandes `$AZURE_EXTENSION_DIR`.</span><span class="sxs-lookup"><span data-stu-id="2ad1f-130">This will be the value of the `$AZURE_EXTENSION_DIR` shell variable.</span></span> <span data-ttu-id="2ad1f-131">Si cette variable n’est pas définie, par défaut la valeur est `$HOME/.azure/cliextensions` sur Linux et macOS, et `%USERPROFILE%\.azure\cliextensions` sur Windows.</span><span class="sxs-lookup"><span data-stu-id="2ad1f-131">If this variable is unset, by default the value is `$HOME/.azure/cliextensions` on Linux and macOS, and `%USERPROFILE%\.azure\cliextensions` on Windows.</span></span>

```bash
rm -rf $AZURE_EXTENSION_DIR/<extension-name>
```

<span data-ttu-id="2ad1f-132">Il est recommandé d’utiliser `az extension remove` pour les désinstallations.</span><span class="sxs-lookup"><span data-stu-id="2ad1f-132">It is recommended that you uninstall using `az extension remove`.</span></span>

## <a name="faq"></a><span data-ttu-id="2ad1f-133">Forum Aux Questions</span><span class="sxs-lookup"><span data-stu-id="2ad1f-133">FAQ</span></span>

<span data-ttu-id="2ad1f-134">Voici les réponses à d’autres questions courantes sur les extensions de CLI.</span><span class="sxs-lookup"><span data-stu-id="2ad1f-134">Here are some answers to other common questions about CLI extensions.</span></span>

### <a name="what-file-formats-are-allowed-for-installation"></a><span data-ttu-id="2ad1f-135">Quels sont les formats de fichiers autorisés pour l’installation ?</span><span class="sxs-lookup"><span data-stu-id="2ad1f-135">What file formats are allowed for installation?</span></span>

<span data-ttu-id="2ad1f-136">Actuellement, seuls les fichiers Wheel Python compilés peuvent être installés en tant qu’extensions.</span><span class="sxs-lookup"><span data-stu-id="2ad1f-136">Currently, only compiled Python wheels can be installed as extensions.</span></span>

### <a name="can-extensions-replace-existing-commands"></a><span data-ttu-id="2ad1f-137">Les extensions peuvent-elles remplacer des commandes existantes ?</span><span class="sxs-lookup"><span data-stu-id="2ad1f-137">Can extensions replace existing commands?</span></span>

<span data-ttu-id="2ad1f-138">Oui.</span><span class="sxs-lookup"><span data-stu-id="2ad1f-138">Yes.</span></span> <span data-ttu-id="2ad1f-139">Les extensions peuvent remplacer des commandes existantes, mais avant l’exécution d’une commande qui a été remplacée, la CLI émet un avertissement.</span><span class="sxs-lookup"><span data-stu-id="2ad1f-139">Extensions may replace existing commands, but before running a command that has been replaced the CLI will issue a warning.</span></span>

### <a name="how-can-i-tell-if-an-extension-is-in-pre-release"></a><span data-ttu-id="2ad1f-140">Comment puis-je savoir si une extension est en version préliminaire ?</span><span class="sxs-lookup"><span data-stu-id="2ad1f-140">How can I tell if an extension is in pre-release?</span></span>

<span data-ttu-id="2ad1f-141">La documentation et le contrôle de version d’une extension doivent indiquer si celle-ci est en version préliminaire.</span><span class="sxs-lookup"><span data-stu-id="2ad1f-141">An extension should indicate through its own documentation and versioning if it is in pre-release.</span></span> <span data-ttu-id="2ad1f-142">Il est également commun pour Microsoft de publier des commandes en préversion pour la CLI en tant qu’extensions, avec des plans pour les migrer dans l’interface CLI principale une fois que le produit n’est plus en préversion.</span><span class="sxs-lookup"><span data-stu-id="2ad1f-142">It is also common for Microsoft to release preview commands for the CLI as extensions, with plans to move them into the main CLI interface once the product is out of preview.</span></span>

### <a name="can-extensions-depend-upon-each-other"></a><span data-ttu-id="2ad1f-143">Les extensions peuvent-elles dépendre les unes des autres ?</span><span class="sxs-lookup"><span data-stu-id="2ad1f-143">Can extensions depend upon each other?</span></span>

<span data-ttu-id="2ad1f-144">Non.</span><span class="sxs-lookup"><span data-stu-id="2ad1f-144">No.</span></span> <span data-ttu-id="2ad1f-145">Les extensions doivent être des packages individuels qui ne reposent pas les uns sur les autres.</span><span class="sxs-lookup"><span data-stu-id="2ad1f-145">Extensions must be individual packages which do not rely on one another.</span></span> <span data-ttu-id="2ad1f-146">Cela s’explique par le fait que la CLI ne donne aucune garantie quant au moment où les extensions sont chargées, et ainsi le chargement des dépendances ne peut pas être garanti.</span><span class="sxs-lookup"><span data-stu-id="2ad1f-146">This is because the CLI gives no guarantee about when extensions are loaded, so dependencies could not be guaranteed to be satisfied.</span></span> <span data-ttu-id="2ad1f-147">En installant une extension, vous n’installez aucun autre élément, et celle-ci doit continuer à fonctionner même si vous supprimez d’autres extensions.</span><span class="sxs-lookup"><span data-stu-id="2ad1f-147">Installing an extension installs that extension only, and it should continue to work even if you remove other extensions.</span></span>

### <a name="are-extensions-updated-along-with-the-cli"></a><span data-ttu-id="2ad1f-148">Les extensions sont-elles mises à jour en même temps que la CLI ?</span><span class="sxs-lookup"><span data-stu-id="2ad1f-148">Are extensions updated along with the CLI?</span></span>

<span data-ttu-id="2ad1f-149">Non.</span><span class="sxs-lookup"><span data-stu-id="2ad1f-149">No.</span></span> <span data-ttu-id="2ad1f-150">Les extensions sont à mettre à jour séparément, comme décrit dans la section [Mettre à jour les extensions](#update-extensions).</span><span class="sxs-lookup"><span data-stu-id="2ad1f-150">Extensions must be updated separately, as described in [Update extensions](#update-extensions).</span></span>
