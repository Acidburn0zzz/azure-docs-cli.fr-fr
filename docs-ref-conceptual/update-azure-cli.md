---
title: Mettre à jour Azure CLI
description: Informations de référence pour la mise à jour d’Azure CLI
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 10/19/2020
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: 91ed79b9f59af4ad070983eb7d0744bc85d09216
ms.sourcegitcommit: 9beaf9abb794f1006a56acee4e1cfb8ea7fe2405
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/08/2020
ms.locfileid: "96850873"
---
# <a name="update-the-azure-cli"></a><span data-ttu-id="9a9ff-103">Mettre à jour Azure CLI</span><span class="sxs-lookup"><span data-stu-id="9a9ff-103">Update the Azure CLI</span></span>

<span data-ttu-id="9a9ff-104">Vous pouvez vous servir de gestionnaires de packages pour mettre à jour une installation locale de l’interface de ligne de commande Azure CLI dans les environnements Windows, macOS et Linux (consultez la section `Update` dans les instructions d’installation propres à chaque plateforme).</span><span class="sxs-lookup"><span data-stu-id="9a9ff-104">You can rely on package managers to update a local install of the Azure CLI on Windows, macOS and Linux environments (see the `Update` section in each platform-specific install instruction).</span></span> <span data-ttu-id="9a9ff-105">L’interface CLI propose également des commandes dans l’outil pour effectuer une mise à niveau manuelle ou automatique.</span><span class="sxs-lookup"><span data-stu-id="9a9ff-105">The CLI also provides in-tool commands to upgrade manually or automatically.</span></span>

## <a name="manual-update"></a><span data-ttu-id="9a9ff-106">Mise à niveau manuelle</span><span class="sxs-lookup"><span data-stu-id="9a9ff-106">Manual Update</span></span>
[!INCLUDE [az-upgrade](includes/az-upgrade.md)]

<span data-ttu-id="9a9ff-107">La commande `az upgrade` est prise en charge sur Windows, macOS et certaines distributions Linux pourvu que l’installation soit prise en charge.</span><span class="sxs-lookup"><span data-stu-id="9a9ff-107">`az upgrade` is supported on Windows, macOS and some Linux distros as long as installation is supported.</span></span> <span data-ttu-id="9a9ff-108">Elle prend uniquement en charge la mise à niveau vers la dernière version.</span><span class="sxs-lookup"><span data-stu-id="9a9ff-108">It only supports upgrading to the latest version.</span></span> <span data-ttu-id="9a9ff-109">Si vous exécutez Azure CLI via Azure Cloud Shell, il est très probable que vous utilisez déjà l’installation la plus récente d’Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="9a9ff-109">If you are running the Azure CLI through Azure Cloud Shell, you are most likely already using the most recent Azure CLI install.</span></span> <span data-ttu-id="9a9ff-110">Si ce n’est pour une raison déterminée telle que la publication ad-hoc d’une version de correctif de bogue mineur, vous devez attendre la prochaine build d’Azure Cloud Shell, car la commande `az upgrade` n’est pas prise en charge dans Azure Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="9a9ff-110">If not due to cases like ad-hoc release of a minor bug fix version, you need to wait for the next build of Azure Cloud Shell as `az upgrade` is not supported in Azure Cloud Shell.</span></span>

<span data-ttu-id="9a9ff-111">Quand `azure-cli` est déjà la version la plus récente, l’exécution de `az upgrade` entraîne la vérification et la mise à jour de toutes les [extensions](azure-cli-extensions-overview.md) installées.</span><span class="sxs-lookup"><span data-stu-id="9a9ff-111">When `azure-cli` is already the latest version, running `az upgrade` will check and update all installed [extensions](azure-cli-extensions-overview.md).</span></span>

## <a name="automatic-update"></a><span data-ttu-id="9a9ff-112">Mise à jour automatique</span><span class="sxs-lookup"><span data-stu-id="9a9ff-112">Automatic Update</span></span>

<span data-ttu-id="9a9ff-113">Par défaut, la mise à niveau automatique est désactivée pour Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="9a9ff-113">By default, auto-upgrade for Azure CLI is disabled.</span></span> <span data-ttu-id="9a9ff-114">Si vous voulez être certain d’avoir toujours la dernière version, vous pouvez activer la mise à niveau automatique via la [configuration](/cli/azure/config).</span><span class="sxs-lookup"><span data-stu-id="9a9ff-114">If you would like to keep up with the latest version, you can enable auto-upgrade through [configuration](/cli/azure/config).</span></span>

```azurecli
az config set auto-upgrade.enable=yes
```

<span data-ttu-id="9a9ff-115">Azure CLI vérifie alors régulièrement s’il existe une nouvelle version. Si c’est le cas, vous êtes invité à procéder à la mise à niveau après l’exécution d’une commande, le cas échéant.</span><span class="sxs-lookup"><span data-stu-id="9a9ff-115">The Azure CLI will check new versions regularly and prompt you to upgrade after any command finishes running once the update is available.</span></span>

<span data-ttu-id="9a9ff-116">Il se peut que le message d’invite et les messages de sortie qui s’affichent pendant la mise à niveau interrompent le résultat de votre commande si elle est assignée à une variable ou si elle fait partie d’un flux automatisé.</span><span class="sxs-lookup"><span data-stu-id="9a9ff-116">The prompt message and output messages during upgrade may interrupt your command result if it is assigned to some variable or in an automated flow.</span></span> <span data-ttu-id="9a9ff-117">Pour éviter toute interruption, vous pouvez utiliser la configuration suivante pour permettre à la mise à jour de se dérouler automatiquement sans confirmation et pour faire en sorte que seuls les avertissements et les erreurs s’affichent pendant la mise à niveau.</span><span class="sxs-lookup"><span data-stu-id="9a9ff-117">To avoid interruption, you can use the following configuration to allow the update to happen automatically without confirmation and only show warnings and errors during the upgrade.</span></span>

```azurecli
az config auto-upgrade.prompt=no
```

<span data-ttu-id="9a9ff-118">Par défaut, toutes les extensions installées sont aussi mises à jour.</span><span class="sxs-lookup"><span data-stu-id="9a9ff-118">By default, all installed extensions will also be updated.</span></span> <span data-ttu-id="9a9ff-119">Vous pouvez désactiver la mise à jour des extensions via la configuration.</span><span class="sxs-lookup"><span data-stu-id="9a9ff-119">You can disable extension update through configuration.</span></span>

```azurecli
az config auto-upgrade.all=no
```

> [!NOTE]
> <span data-ttu-id="9a9ff-120">Attendez que la commande `az upgrade` prenne fin avant de passer au jeu de commandes suivant, car les nouvelles versions de l’interface CLI (et des extensions) risquent de présenter des changements cassants.</span><span class="sxs-lookup"><span data-stu-id="9a9ff-120">Please wait for `az upgrade` to complete before proceeding to the next set of commands, else the new versions of the CLI (+extensions) may have breaking changes.</span></span>

<span data-ttu-id="9a9ff-121">Si vous préférez ne plus utiliser la fonctionnalité de mise à jour automatique par exemple pour assurer l’exécution stable des scripts de commandes, vous pouvez la désactiver via la configuration.</span><span class="sxs-lookup"><span data-stu-id="9a9ff-121">If you decide not to use the automatic update feature any more for cases like keeping command scripts running stably, you can turn it off through configuration.</span></span>
```azurecli
az config set auto-upgrade.enable=no
```
