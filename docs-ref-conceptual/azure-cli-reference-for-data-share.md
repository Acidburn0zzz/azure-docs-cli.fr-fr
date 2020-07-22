---
title: Références Azure CLI pour Azure Data Share
description: Page de destination des références Azure CLI pour Azure Data Share
services: data-share
author: dbradish-microsoft
manager: barbkess
ms.service: data-share
ms.devlang: azurecli
ms.topic: reference
ms.date: 05/27/2020
ms.author: dbradish
ms.openlocfilehash: 404022b13f44174e4b647f0430a58fac5eeb81df
ms.sourcegitcommit: c473377d1c08ac4efd2480bf852c30dbf1044a57
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/16/2020
ms.locfileid: "86415555"
---
# <a name="azure-cli-for-azure-data-share"></a><span data-ttu-id="00074-103">Azure CLI pour Azure Data Share</span><span class="sxs-lookup"><span data-stu-id="00074-103">Azure CLI for Azure Data Share</span></span>

<span data-ttu-id="00074-104">L'interface de ligne de commande Azure ([Azure CLI](/cli/azure/what-is-azure-cli)) est un ensemble de commandes utilisées pour créer et gérer des ressources Azure.</span><span class="sxs-lookup"><span data-stu-id="00074-104">The Azure Command Line Interface ([Azure CLI](/cli/azure/what-is-azure-cli)) is a set of commands used to create and manage Azure resources.</span></span>  <span data-ttu-id="00074-105">Elle est disponible sur de nombreux services Azure, notamment Azure Data Share.</span><span class="sxs-lookup"><span data-stu-id="00074-105">It is available across many Azure services including Azure Data Share.</span></span>  <span data-ttu-id="00074-106">Plus de 65 commandes différentes sont à votre disposition pour le partage des données.</span><span class="sxs-lookup"><span data-stu-id="00074-106">There are over 65 different commands for data share!</span></span>  <span data-ttu-id="00074-107">Ces commandes vous permettent d'utiliser efficacement le service à partir d'une ligne de commande.</span><span class="sxs-lookup"><span data-stu-id="00074-107">These commands give you the ability to work effectively with the service from a command line.</span></span>

## <a name="references-for-data-share"></a><span data-ttu-id="00074-108">Références pour Data Share</span><span class="sxs-lookup"><span data-stu-id="00074-108">References for Data Share</span></span>

<span data-ttu-id="00074-109">Toutes les commandes Azure CLI pour Azure Data Share sont actuellement des extensions d'Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="00074-109">All Azure CLI commands for Azure Data Share are currently extensions to the Azure CLI.</span></span>  <span data-ttu-id="00074-110">Une extension vous donne accès à des commandes expérimentales et disponibles en préversion.</span><span class="sxs-lookup"><span data-stu-id="00074-110">An extension gives you access to experimental and pre-release commands.</span></span>  <span data-ttu-id="00074-111">Découvrez-en plus sur les références des extensions dans [Utiliser des extensions avec Azure CLI](/cli/azure/azure-cli-extensions-overview).</span><span class="sxs-lookup"><span data-stu-id="00074-111">Find out more about extension references in [Use extensions with Azure CLI](/cli/azure/azure-cli-extensions-overview).</span></span>

|<span data-ttu-id="00074-112">Référence Azure CLI</span><span class="sxs-lookup"><span data-stu-id="00074-112">Azure CLI Reference</span></span> |<span data-ttu-id="00074-113">Description</span><span class="sxs-lookup"><span data-stu-id="00074-113">Description</span></span>
|-|-|-|
| [<span data-ttu-id="00074-114">az datashare</span><span class="sxs-lookup"><span data-stu-id="00074-114">az datashare</span></span>](/cli/azure/ext/datashare/datashare) | <span data-ttu-id="00074-115">Toutes les commandes permettant de gérer Azure Data Share.</span><span class="sxs-lookup"><span data-stu-id="00074-115">All commands to manage Azure Data Share.</span></span>
| [<span data-ttu-id="00074-116">az datashare account</span><span class="sxs-lookup"><span data-stu-id="00074-116">az datashare account</span></span>](/cli/azure/ext/datashare/datashare/account) | <span data-ttu-id="00074-117">Commandes permettant de gérer les comptes Azure Data Share.</span><span class="sxs-lookup"><span data-stu-id="00074-117">Commands to manage Azure Data Share accounts.</span></span>
| [<span data-ttu-id="00074-118">az datashare consumer</span><span class="sxs-lookup"><span data-stu-id="00074-118">az datashare consumer</span></span>](/cli/azure/ext/datashare/datashare/consumer) | <span data-ttu-id="00074-119">Commandes permettant aux consommateurs de gérer Azure Data Share.</span><span class="sxs-lookup"><span data-stu-id="00074-119">Commands for consumers to manage Azure Data Share.</span></span>
| [<span data-ttu-id="00074-120">az datashare dataset</span><span class="sxs-lookup"><span data-stu-id="00074-120">az datashare dataset</span></span>](/cli/azure/ext/datashare/datashare/dataset) | <span data-ttu-id="00074-121">Commandes permettant aux fournisseurs de gérer les jeux de données Azure Data Share.</span><span class="sxs-lookup"><span data-stu-id="00074-121">Commands for providers to manage Azure Data Share datasets.</span></span>
| [<span data-ttu-id="00074-122">az datashare invitation</span><span class="sxs-lookup"><span data-stu-id="00074-122">az datashare invitation</span></span>](/cli/azure/ext/datashare/datashare/invitation) | <span data-ttu-id="00074-123">Commandes permettant aux consommateurs de gérer les invitations Azure Data Share.</span><span class="sxs-lookup"><span data-stu-id="00074-123">Commands for consumers to manage Azure Data Share invitations.</span></span>
| [<span data-ttu-id="00074-124">az datashare provider-share-subscription</span><span class="sxs-lookup"><span data-stu-id="00074-124">az datashare provider-share-subscription</span></span>](/cli/azure/ext/datashare/datashare/provider-share-subscription) | <span data-ttu-id="00074-125">Commandes permettant aux fournisseurs de gérer les abonnements Azure Data Share.</span><span class="sxs-lookup"><span data-stu-id="00074-125">Commands for providers to manage Azure Data Share subscriptions.</span></span>
| [<span data-ttu-id="00074-126">az datashare synchronization</span><span class="sxs-lookup"><span data-stu-id="00074-126">az datashare synchronization</span></span>](/cli/azure/ext/datashare/datashare/synchronization)  | <span data-ttu-id="00074-127">Commandes permettant de gérer la synchronisation d'Azure Data Share.</span><span class="sxs-lookup"><span data-stu-id="00074-127">Commands to manage Azure Data Share synchronization.</span></span>
| [<span data-ttu-id="00074-128">az datashare synchronization-setting</span><span class="sxs-lookup"><span data-stu-id="00074-128">az datashare synchronization-setting</span></span>](/cli/azure/ext/datashare/datashare/synchronization-setting)  | <span data-ttu-id="00074-129">Commandes permettant aux fournisseurs de gérer les paramètres de synchronisation d'Azure Data Share.</span><span class="sxs-lookup"><span data-stu-id="00074-129">Commands for providers to manage Azure Data Share synchronization settings.</span></span>

## <a name="reference-examples"></a><span data-ttu-id="00074-130">Exemples de références</span><span class="sxs-lookup"><span data-stu-id="00074-130">Reference examples</span></span>

<span data-ttu-id="00074-131">Des exemples sont fournis avec chaque référence Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="00074-131">Examples are provided with every Azure CLI reference.</span></span> <span data-ttu-id="00074-132">Vous pouvez également effectuer ces tâches via le portail Azure, mais l'utilisation d'Azure CLI ne nécessite qu'une seule ligne de commande.</span><span class="sxs-lookup"><span data-stu-id="00074-132">Although you can also complete these tasks through the Azure portal, using the Azure CLI requires a single command line.</span></span>  <span data-ttu-id="00074-133">Les blocs de code suivants vous donneront une idée de la facilité d'utilisation d'Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="00074-133">Here are a few code blocks to give you an idea of how easy it is to use the Azure CLI.</span></span>

<span data-ttu-id="00074-134">Pour utiliser Azure Data Share, vous devrez d'abord disposer d'un groupe de ressources.</span><span class="sxs-lookup"><span data-stu-id="00074-134">To work with Azure Data Share, you'll first need a resource group.</span></span>  <span data-ttu-id="00074-135">Les groupes de ressources Azure sont faciles à créer et à gérer avec Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="00074-135">Azure resource groups are simple to create and manage with the Azure CLI.</span></span>  

```azurecli
#create a resource group
az group create -location westus -name MyResourceGroup
```

```azurecli
#get a list of resource groups for a subscription
az group list --subscription MySubscription --output table
```

<span data-ttu-id="00074-136">Et il est tout aussi simple de créer un compte de partage de données.</span><span class="sxs-lookup"><span data-stu-id="00074-136">It is as straightforward to create a data share account.</span></span>

```azurecli
#create a data share account
az datashare account create --location "West US 2" --tags tag1=Red tag2=White --name MyAccount --resource-group MyResourceGroup
```

## <a name="see-also"></a><span data-ttu-id="00074-137">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="00074-137">See also</span></span>

* <span data-ttu-id="00074-138">[Prise en main d'Azure CLI](/cli/azure/get-started-with-azure-cli) pour en savoir plus sur l'installation et la connexion.</span><span class="sxs-lookup"><span data-stu-id="00074-138">[Get started with Azure CLI](/cli/azure/get-started-with-azure-cli) to learn about installation and sign in.</span></span>

* <span data-ttu-id="00074-139">Découvrez des références [principales](/cli/azure/reference-index) et [d'extension](/cli/azure/azure-cli-extensions-list) supplémentaires dans la documentation Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="00074-139">Discover additional [core](/cli/azure/reference-index) and [extension](/cli/azure/azure-cli-extensions-list) references in the Azure CLI documentation.</span></span>
