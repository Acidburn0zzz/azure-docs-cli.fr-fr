---
title: Différences entre les produits d’Azure CLI
description: Comprendre comment les produits Azure CLI sont nommés et versionnés, et comment ils sont mis à jour.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 07/12/2018
ms.topic: conceptual
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: a39f6b0fbccf937aec2b227ed4e3f4ff8d92137f
ms.sourcegitcommit: 7f79860c799e78fd8a591d7a5550464080e07aa9
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/12/2019
ms.locfileid: "56158445"
---
# <a name="differences-between-azure-cli-products"></a><span data-ttu-id="91550-103">Différences entre les produits d’Azure CLI</span><span class="sxs-lookup"><span data-stu-id="91550-103">Differences between Azure CLI products</span></span>

<span data-ttu-id="91550-104">Depuis fin juin 2018, les numéros de version explicites ont été supprimés des noms de produits Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="91550-104">As of the end of June 2018, explicit version numbers have been removed from Azure CLI product names.</span></span> <span data-ttu-id="91550-105">Cette modification permet d’éviter toute confusion apparaissant parfois dans la documentation où les utilisateurs devaient utiliser « Azure CLI », mais il était difficile de savoir quelle version du produit était référencée.</span><span class="sxs-lookup"><span data-stu-id="91550-105">This change helps eliminate confusion that sometimes showed up in documentation where users were told to use "the Azure CLI" but it was unclear what version of the product was being referenced.</span></span> <span data-ttu-id="91550-106">Si vous connaissez les anciens noms de produit, voici les modifications qui leur ont été apportées :</span><span class="sxs-lookup"><span data-stu-id="91550-106">If you're familiar with the old product names, here is how they have changed:</span></span>

* <span data-ttu-id="91550-107">Azure CLI 2.0 et ses versions ultérieures sont désormais uniquement appelées « Azure CLI ».</span><span class="sxs-lookup"><span data-stu-id="91550-107">Azure CLI versions 2.0 and later are now referred to only as "Azure CLI."</span></span>
* <span data-ttu-id="91550-108">Les anciennes versions d’Azure CLI (1.x et antérieures) sont désormais appelées « Azure CLI Classic ».</span><span class="sxs-lookup"><span data-stu-id="91550-108">Earlier Azure CLI versions (1.x and lower) are now referred to as "Azure classic CLI."</span></span>

<span data-ttu-id="91550-109">Le changement de nom pour Azure CLI Classic indique plus clairement que cet outil est destiné à être utilisé uniquement avec le modèle de déploiement classique.</span><span class="sxs-lookup"><span data-stu-id="91550-109">The name change to Azure classic CLI makes it clear that this tool is meant to be used only with the classic deployment model.</span></span> <span data-ttu-id="91550-110">L’interface de ligne de commande classique n’est également plus mise à jour ni maintenue.</span><span class="sxs-lookup"><span data-stu-id="91550-110">The classic CLI is also no longer updated or maintained.</span></span> <span data-ttu-id="91550-111">Pour cette raison et pour bien d’autres, il est recommandé de déplacer tous les déploiements classiques afin d’utiliser le modèle Azure Resource Manager et de le migrer vers la dernière version disponible d’Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="91550-111">For this reason, and many more, it's recommended that you move any classic deployments to use the Azure Resource Manager model and migrate to the latest available version of the Azure CLI.</span></span>

<span data-ttu-id="91550-112">Si vous utilisez toujours l’interface CLI classique, vous pouvez en savoir plus sur le processus de migration dans les articles suivants :</span><span class="sxs-lookup"><span data-stu-id="91550-112">If you are still using the classic CLI, you can learn about the process of migrating in the following articles:</span></span>

* [<span data-ttu-id="91550-113">Migrer de Classic vers Azure Resource Manager</span><span class="sxs-lookup"><span data-stu-id="91550-113">Migrate from Classic to Azure Resource Manager</span></span>](/azure/virtual-machines/linux/migration-classic-resource-manager-overview)
* [<span data-ttu-id="91550-114">Installer l’interface de ligne de commande Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="91550-114">Install the Azure CLI</span></span>](install-azure-cli.md)
* [<span data-ttu-id="91550-115">Migration à partir d’Azure CLI classique vers Azure CLI</span><span class="sxs-lookup"><span data-stu-id="91550-115">Migrating from Azure classic CLI to Azure CLI</span></span>](https://github.com/Azure/azure-cli/blob/dev/doc/classic_cli_migration.md)
