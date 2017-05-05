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
translationtype: HT
---
# <a name="manage-multiple-azure-subscriptions"></a>Gérer plusieurs abonnements Azure

Si vous débutez avec Azure, vous avez probablement un seul abonnement.
Si vous utilisez Azure depuis un moment déjà, vous avez peut-être créé plusieurs abonnements Azure.
Dans ce cas, vous pouvez configurer Azure CLI 2.0 pour exécuter les commandes sur un abonnement spécifique.

1. Obtenez la liste de tous les abonnements créés dans votre compte.

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

1. Définissez l’abonnement par défaut.
 
   ```azurecli
   az account set --subscription "My Demos"
   ```

Vous pouvez vérifier que cette modification a été prise en compte en réexécutant la commande `az account list --output table`.

Une fois que vous avez défini votre abonnement par défaut, toutes les commandes Azure CLI ultérieures s’exécuteront sur cet abonnement.