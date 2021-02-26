---
title: Installer manuellement Azure CLI pour Linux
description: Comment installer manuellement Azure CLI sur Linux
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 12/15/2020
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
zone_pivot_group_filename: azure/zone-pivot-groups.json
zone_pivot_groups: cli-linux-installation-method
ms.openlocfilehash: 03c7e7e4915f48dce70d2bc2cab16b4688f8b5fd
ms.sourcegitcommit: 594e9c620a6f74f5eaedf91a7f6a791e03a64c74
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/17/2021
ms.locfileid: "100631003"
---
# <a name="install-the-azure-cli-on-linux"></a><span data-ttu-id="f3679-103">Installer Azure CLI sur Linux</span><span class="sxs-lookup"><span data-stu-id="f3679-103">Install the Azure CLI on Linux</span></span>

<span data-ttu-id="f3679-104">Nous vous recommandons d’installer Azure CLI à l’aide du gestionnaire de package de votre distribution Linux.</span><span class="sxs-lookup"><span data-stu-id="f3679-104">It is recommended to install the Azure CLI using your Linux distribution's package manager.</span></span> <span data-ttu-id="f3679-105">Sélectionnez le gestionnaire de package approprié pour votre distribution parmi les options ci-dessus.</span><span class="sxs-lookup"><span data-stu-id="f3679-105">Select the appropriate package manager for your distribution from the options above.</span></span>  <span data-ttu-id="f3679-106">Si vous n’avez aucun des gestionnaires de package listés, sélectionnez l’option *Script d’installation* pour installer manuellement Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="f3679-106">If you do not have one of the listed package managers, you may manually install the Azure CLI by selecting the *Install script* option.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

::: zone pivot="apt"

[!INCLUDE [cli-install-linux-apt](includes/cli-install-linux-apt.md)]

::: zone-end

::: zone pivot="dnf"

[!INCLUDE [cli-install-linux-apt](includes/cli-install-linux-dnf.md)]

::: zone-end

::: zone pivot="zypper"

[!INCLUDE [cli-install-linux-apt](includes/cli-install-linux-zypper.md)]

::: zone-end

::: zone pivot="script"

[!INCLUDE [cli-install-linux-apt](includes/cli-install-linux-script.md)]

::: zone-end

## <a name="next-steps"></a><span data-ttu-id="f3679-107">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="f3679-107">Next Steps</span></span>

<span data-ttu-id="f3679-108">Maintenant que vous avez installé l’interface CLI, découvrez ses fonctionnalités et ses commandes courantes.</span><span class="sxs-lookup"><span data-stu-id="f3679-108">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="f3679-109">Prise en main de l’interface Azure CLI</span><span class="sxs-lookup"><span data-stu-id="f3679-109">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
