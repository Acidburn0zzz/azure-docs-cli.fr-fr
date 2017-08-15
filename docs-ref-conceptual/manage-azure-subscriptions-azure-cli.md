---
title: "Gérer les abonnements Azure avec Azure CLI 2.0"
description: "Gérer les abonnements Azure avec Azure CLI 2.0 sur Linux, Mac ou Windows."
keywords: Azure CLI 2.0, Linux, Mac, Windows, OS X, subscription
author: kamaljit
ms.author: routlaw
manager: douge
ms.date: 02/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: 98fb955e-6dbf-47e2-80ac-170d6d95cb70
ms.openlocfilehash: 383fb6ebd90ac79f60869187b402d53d4f1791fd
ms.sourcegitcommit: 4fd631a58cf19c494162510d073fbbbdf0524d16
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/05/2017
---
# <a name="manage-multiple-azure-subscriptions"></a><span data-ttu-id="cb034-104">Gérer plusieurs abonnements Azure</span><span class="sxs-lookup"><span data-stu-id="cb034-104">Manage multiple Azure subscriptions</span></span>

<span data-ttu-id="cb034-105">Si vous débutez avec Azure, vous avez probablement un seul abonnement.</span><span class="sxs-lookup"><span data-stu-id="cb034-105">If you are brand new to Azure, you probably only have a single subscription.</span></span>
<span data-ttu-id="cb034-106">Si vous utilisez Azure depuis un moment déjà, vous avez peut-être créé plusieurs abonnements Azure.</span><span class="sxs-lookup"><span data-stu-id="cb034-106">But if you have been using Azure for a while, you may have created multiple Azure subscriptions.</span></span>
<span data-ttu-id="cb034-107">Dans ce cas, vous pouvez configurer Azure CLI 2.0 pour exécuter les commandes sur un abonnement spécifique.</span><span class="sxs-lookup"><span data-stu-id="cb034-107">If so, you can configure Azure CLI 2.0 to execute commands against a particular subscription.</span></span>

[!INCLUDE [cloud-shell-try-it.md](includes/cloud-shell-try-it.md)]

1. <span data-ttu-id="cb034-108">Obtenez la liste de tous les abonnements créés dans votre compte.</span><span class="sxs-lookup"><span data-stu-id="cb034-108">Get a list of all subscriptions in your account.</span></span>

   ```azurecli-interactive
   az account list --output table
   ```

   ```Output
   Name                                         CloudName    SubscriptionId                        State     IsDefault
   -------------------------------------------  -----------  ------------------------------------  --------  -----------
   My Production Subscription                   AzureCloud   XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX  Enabled
   My DevTest Subscription                      AzureCloud   XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX  Enabled   True
   My Demos                                     AzureCloud   XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX  Enabled
   ```

1. <span data-ttu-id="cb034-109">Définissez l’abonnement par défaut.</span><span class="sxs-lookup"><span data-stu-id="cb034-109">Set the default.</span></span>
 
   ```azurecli-interactive
   az account set --subscription "My Demos"
   ```

   > [!NOTE]
   > <span data-ttu-id="cb034-110">Le paramètre `--subscription` accepte soit le nom d’abonnement, soit l’ID d’abonnement.</span><span class="sxs-lookup"><span data-stu-id="cb034-110">The `--subscription` parameter takes either the subscription name or the subscription ID.</span></span>

<span data-ttu-id="cb034-111">Vous pouvez vérifier que cette modification a été prise en compte en réexécutant la commande `az account list --output table`.</span><span class="sxs-lookup"><span data-stu-id="cb034-111">You can verify the change by running the `az account list --output table` command again.</span></span>

<span data-ttu-id="cb034-112">Une fois que vous avez défini votre abonnement par défaut, toutes les commandes Azure CLI ultérieures s’exécuteront sur cet abonnement.</span><span class="sxs-lookup"><span data-stu-id="cb034-112">Once you set your default subscription, all subsequent Azure CLI commands run against this subscription.</span></span>