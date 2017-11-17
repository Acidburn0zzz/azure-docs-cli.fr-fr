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
ms.openlocfilehash: c3538077e05d61f3c40880bb8b804226eb99dc85
ms.sourcegitcommit: bcf93ad8ed8802072249cd8187cd4420da89b4c6
ms.translationtype: HT
ms.contentlocale: fr-FR
---
# <a name="manage-multiple-azure-subscriptions"></a><span data-ttu-id="d42a9-104">Gérer plusieurs abonnements Azure</span><span class="sxs-lookup"><span data-stu-id="d42a9-104">Manage multiple Azure subscriptions</span></span>

<span data-ttu-id="d42a9-105">Si vous débutez avec Azure, vous avez probablement un seul abonnement.</span><span class="sxs-lookup"><span data-stu-id="d42a9-105">If you are brand new to Azure, you probably only have a single subscription.</span></span>
<span data-ttu-id="d42a9-106">Si vous utilisez Azure depuis un moment déjà, vous avez peut-être créé plusieurs abonnements Azure.</span><span class="sxs-lookup"><span data-stu-id="d42a9-106">But if you have been using Azure for a while, you may have created multiple Azure subscriptions.</span></span>
<span data-ttu-id="d42a9-107">Dans ce cas, vous pouvez configurer Azure CLI 2.0 pour exécuter les commandes sur un abonnement spécifique.</span><span class="sxs-lookup"><span data-stu-id="d42a9-107">If so, you can configure Azure CLI 2.0 to execute commands against a particular subscription.</span></span>

1. <span data-ttu-id="d42a9-108">Obtenez la liste de tous les abonnements créés dans votre compte.</span><span class="sxs-lookup"><span data-stu-id="d42a9-108">Get a list of all subscriptions in your account.</span></span>

   ```azurecli
   az account list --output table
   ```

   ```Output
   Name                                         CloudName    SubscriptionId                        State     IsDefault
   -------------------------------------------  -----------  ------------------------------------  --------  -----------
   My Production Subscription                   AzureCloud   XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX  Enabled
   My DevTest Subscription                      AzureCloud   XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX  Enabled   True
   My Demos                                     AzureCloud   XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX  Enabled
   ```

1. <span data-ttu-id="d42a9-109">Définissez l’abonnement par défaut.</span><span class="sxs-lookup"><span data-stu-id="d42a9-109">Set the default.</span></span>
 
   ```azurecli
   az account set --subscription "My Demos"
   ```

<span data-ttu-id="d42a9-110">Vous pouvez vérifier que cette modification a été prise en compte en réexécutant la commande `az account list --output table`.</span><span class="sxs-lookup"><span data-stu-id="d42a9-110">You can verify the change by running the `az account list --output table` command again.</span></span>

<span data-ttu-id="d42a9-111">Une fois que vous avez défini votre abonnement par défaut, toutes les commandes Azure CLI ultérieures s’exécuteront sur cet abonnement.</span><span class="sxs-lookup"><span data-stu-id="d42a9-111">Once you set your default subscription, all subsequent Azure CLI commands run against this subscription.</span></span>