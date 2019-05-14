---
title: Installer l’interface de ligne de commande Azure pour Windows
description: Comment installer Azure CLI sur Windows
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/01/2019
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: c5c499800e49dcdc536337e7655ec1ee280d48f2
ms.sourcegitcommit: 65bf8561a6e047e4eab52186e066a2e8c21f1d40
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/07/2019
ms.locfileid: "65240541"
---
# <a name="install-azure-cli-on-windows"></a>Installer Azure CLI sur Windows

Sur Windows, Azure CLI est installée via un fichier MSI, ce qui vous donne accès à l’interface CLI via l’Invite de commande Windows (CMD) ou PowerShell.
Lors de son installation sur le sous-système Windows pour Linux (WSL), des packages sont disponibles pour votre distribution Linux. Consultez la [page d’installation principale](install-azure-cli.md) pour obtenir la liste des gestionnaires de packages pris en charge ou pour savoir comment installer manuellement avec le sous-système Windows pour Linux.

[!INCLUDE [current-version](includes/current-version.md)]

## <a name="install-or-update"></a>Installation ou mise à jour

Le fichier MSI distribuable est utilisé pour l’installation ou la mise à jour d’Azure CLI sur Windows. L’utilisation du programme d’installation MSI ne nécessite pas la désinstallation des versions actuelles.

> [!div class="nextstepaction"]
> [Téléchargez le programme d’installation MSI](https://aka.ms/installazurecliwindows)

Lorsque le programme d’installation vous demande s’il peut apporter des modifications à votre ordinateur, cliquez sur la case « Oui ».

Vous pouvez désormais exécuter l’interface de ligne de commande Azure avec la commande `az` à partir de l’invite de commandes Windows ou PowerShell. PowerShell offre des fonctionnalités de saisie semi-automatique via la touche TAB non disponibles à partir de l’invite de commandes Windows. Pour vous connecter, exécutez la commande [az login](/cli/azure/reference-index#az-login).

[!INCLUDE [interactive-login](includes/interactive-login.md)]

Pour en savoir plus sur les différentes méthodes d’authentification, consultez [Se connecter avec Azure CLI](authenticate-azure-cli.md).

## <a name="uninstall"></a>Désinstaller l’interface

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

La désinstallation d’Azure CLI s’effectue à partir de la liste « Applications et fonctionnalités » dans Windows. Pour désinstaller :

| Plateforme | Instructions |
|---|---|
| Windows 10 | Démarrer > Paramètres > Applications |
| Windows 8<br/>Windows 7 | Démarrer > Panneau de configuration > Programmes > Désinstaller un programme |

Une fois sur cet écran, tapez __Azure CLI__ dans la barre de recherche du programme. Le programme à désinstaller est listé sous le nom __Microsoft CLI 2.0 pour Azure__. Sélectionnez cette application, puis cliquez sur le bouton `Uninstall`.

## <a name="next-steps"></a>Étapes suivantes

Maintenant que vous avez installé l’interface CLI, découvrez ses fonctionnalités et ses commandes courantes.

> [!div class="nextstepaction"]
> [Prise en main de l’interface Azure CLI](get-started-with-azure-cli.md)
