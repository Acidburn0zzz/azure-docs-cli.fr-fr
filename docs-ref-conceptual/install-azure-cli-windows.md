---
title: Installer l’interface de ligne de commande Azure pour Windows
description: Comment installer Azure CLI sur Windows
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: ffd9c279302377de6eca1b64c45749196bd99096
ms.sourcegitcommit: 1987a39809f9865034b27130e56f30b2bd1eb72c
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/19/2019
ms.locfileid: "56421871"
---
# <a name="install-azure-cli-on-windows"></a>Installer Azure CLI sur Windows

Sur Windows, Azure CLI est installée via un fichier MSI, ce qui vous donne accès à l’interface CLI via l’Invite de commande Windows (CMD) ou PowerShell.
Lors de son installation sur le sous-système Windows pour Linux (WSL), des packages sont disponibles pour votre distribution Linux. Consultez la [page d’installation principale](install-azure-cli.md) pour obtenir la liste des gestionnaires de packages pris en charge ou pour savoir comment installer manuellement avec le sous-système Windows pour Linux.

[!INCLUDE [current-version](includes/current-version.md)]

## <a name="install-or-update"></a>Installation ou mise à jour

Le fichier MSI distribuable est utilisé pour l’installation, la mise à jour et la désinstallation de la commande `az` sous Windows.

> [!div class="nextstepaction"]
> [Téléchargez le programme d’installation MSI](https://aka.ms/installazurecliwindows)

Lorsque le programme d’installation vous demande s’il peut apporter des modifications à votre ordinateur, cliquez sur la case « Oui ».

Vous pouvez désormais exécuter l’interface de ligne de commande Azure avec la commande `az` à partir de l’invite de commandes Windows ou PowerShell. PowerShell offre des fonctionnalités de saisie semi-automatique via la touche TAB non disponibles à partir de l’invite de commandes Windows. Pour vous connecter, exécutez la commande [az login](/cli/azure/reference-index#az-login).

[!INCLUDE [interactive-login](includes/interactive-login.md)]

Pour en savoir plus sur les différentes méthodes d’authentification, consultez [Se connecter avec Azure CLI](authenticate-azure-cli.md).

## <a name="uninstall"></a>Désinstaller l’interface

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

La désinstallation peut être réalisée en exécutant le fichier MSI à nouveau, en choisissant l’option « Désinstaller ».

> [!div class="nextstepaction"]
> [Téléchargez le programme d’installation MSI](https://aka.ms/installazurecliwindows)

## <a name="next-steps"></a>Étapes suivantes

Maintenant que vous avez installé l’interface CLI, découvrez ses fonctionnalités et ses commandes courantes.

> [!div class="nextstepaction"]
> [Prise en main de l’interface Azure CLI](get-started-with-azure-cli.md)
