---
title: "Installer l’interface de ligne de commande Azure pour Windows"
description: "Installation d’Azure CLI 2.0 sur Windows"
keywords: "Azure CLI, installation d’Azure CLI, installation Azure Windows, Azure CLI Windows, Azure Windows"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 11/01/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ROBOTS: NOINDEX,NOFOLLOW
ms.openlocfilehash: 247ae43813ca9ca7b7b98ebd8e933e02989c6649
ms.sourcegitcommit: 2e4d0bdd94c626e061434883032367b5619de4fe
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/09/2017
---
# <a name="install-azure-cli-20-on-windows"></a>Installation d’Azure CLI 2.0 sur Windows

Sous Windows, vous pouvez installer un fichier binaire natif à partir d’un fichier MSI, que vous pouvez utiliser à l’invite de commandes Windows ou de PowerShell. Si vous exécutez le sous-système Windows pour Linux, des packages sont disponibles pour la distribution que vous exécutez. Consultez la [page d’installation principale](install-azure-cli.md) pour obtenir la liste des gestionnaires de packages pris en charge ou pour savoir comment installer manuellement avec le sous-système Windows pour Linux.

## <a name="install-or-update-with-msi"></a>Installer ou mettre à jour avec MSI

Le fichier MSI distribuable est utilisé pour l’installation, la mise à jour et la désinstallation de la commande `az` sous Windows. Vous pouvez [télécharger le programme d’installation MSI](https://aka.ms/InstallAzureCliWindows), exécutez-le ensuite pour installer ou mettre à jour.

Lorsque le programme d’installation vous demande s’il peut apporter des modifications à votre ordinateur, cliquez sur la case « Oui ».

Vous pouvez désormais exécuter l’interface de ligne de commande Azure avec la commande `az` à partir de l’invite de commandes Windows ou PowerShell.

## <a name="uninstall-with-msi"></a>Désinstaller avec MSI

Si jamais vous décidez de désinstaller l’interface de ligne de commande Azure, nous sommes désolés de vous voir partir. Avant de désinstaller, utilisez la commande `az feedback`, afin de nous donner quelques raisons pour lesquelles vous avez choisi de désinstaller et nous aider à améliorer l’expérience CLI. Nous souhaitons nous assurer que l’interface de ligne de commande Azure est aussi conviviale et exempte de bogues que possible. Vous pouvez également [signaler un problème lié à GitHub](https://github.com/Azure/azure-cli/issues).

La désinstallation peut être réalisée en exécutant le fichier MSI à nouveau, en choisissant l’option « Désinstaller ». Vous pouvez [télécharger le programme d’installation MSI](https://aka.ms/InstallAzureCliWindows) si vous n’y avez plus accès.
