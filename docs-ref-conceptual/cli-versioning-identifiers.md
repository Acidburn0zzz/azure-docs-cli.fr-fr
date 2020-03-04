---
title: Différences entre les produits d’Azure CLI
description: Comprendre comment les produits Azure CLI sont nommés et versionnés, et comment ils sont mis à jour.
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 07/12/2018
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 3cd61d2166d03f7b9d58db1ee1cee77d17b5b336
ms.sourcegitcommit: 7caa6673f65e61deb8d6def6386e4eb9acdac923
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/28/2020
ms.locfileid: "77779973"
---
# <a name="differences-between-azure-cli-products"></a>Différences entre les produits d’Azure CLI

Depuis fin juin 2018, les numéros de version explicites ont été supprimés des noms de produits Azure CLI. Cette modification permet d’éviter toute confusion apparaissant parfois dans la documentation où les utilisateurs devaient utiliser « Azure CLI », mais il était difficile de savoir quelle version du produit était référencée. Si vous connaissez les anciens noms de produit, voici les modifications qui leur ont été apportées :

* Azure CLI 2.0 et ses versions ultérieures sont désormais uniquement appelées « Azure CLI ».
* Les anciennes versions d’Azure CLI (1.x et antérieures) sont désormais appelées « Azure CLI Classic ».

Le changement de nom pour Azure CLI Classic indique plus clairement que cet outil est destiné à être utilisé uniquement avec le modèle de déploiement classique. L’interface de ligne de commande classique n’est également plus mise à jour ni maintenue. Pour cette raison et pour bien d’autres, il est recommandé de déplacer tous les déploiements classiques afin d’utiliser le modèle Azure Resource Manager et de le migrer vers la dernière version disponible d’Azure CLI.

Si vous utilisez toujours l’interface CLI classique, vous pouvez en savoir plus sur le processus de migration dans les articles suivants :

* [Migrer de Classic vers Azure Resource Manager](/azure/virtual-machines/linux/migration-classic-resource-manager-overview)
* [Installer l’interface de ligne de commande Microsoft Azure](install-azure-cli.md)
* [Migration à partir d’Azure CLI classique vers Azure CLI](https://github.com/Azure/azure-cli/blob/dev/doc/classic_cli_migration.md)
