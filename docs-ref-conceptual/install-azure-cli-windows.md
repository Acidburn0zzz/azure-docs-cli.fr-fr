---
title: Installer l’interface de ligne de commande Azure pour Windows
description: Installation d’Azure CLI 2.0 sur Windows
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 01/29/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: c3ed3585b601ee55b267ea6cfc43ce41c54f084a
ms.sourcegitcommit: 15d6dfaee2075d0abceb2aa2423f0b6ef7b2ac9b
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/07/2018
---
# <a name="install-azure-cli-20-on-windows"></a>Installation d’Azure CLI 2.0 sur Windows

Sur Windows, le fichier binaire Azure CLI est installé via un fichier MSI, qui vous donne accès à l’interface de ligne de commande via l’Invite de commandes Windows (CMD) ou PowerShell.

> [!div class="nextstepaction"]
> [Téléchargez le programme d’installation MSI](https://aka.ms/installazurecliwindows)

Lorsque le programme d’installation vous demande s’il peut apporter des modifications à votre ordinateur, cliquez sur la case « Oui ».

Vous pouvez désormais exécuter l’interface de ligne de commande Azure avec la commande `az` à partir de l’invite de commandes Windows ou PowerShell. PowerShell offre des fonctionnalités de saisie semi-automatique via la touche TAB non disponibles à partir de l’invite de commandes Windows. Pour vous connecter, exécutez la commande `az login`.

```azurecli
az login
```

Pour en savoir plus sur les différentes méthodes de connexion, consultez [Se connecter avec Azure CLI 2.0](authenticate-azure-cli.md).

## <a name="uninstall"></a>Désinstaller l’interface

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

La désinstallation peut être réalisée en exécutant le fichier MSI à nouveau, en choisissant l’option « Désinstaller ».

> [!div class="nextstepaction"]
> [Téléchargez le programme d’installation MSI](https://aka.ms/installazurecliwindows)
