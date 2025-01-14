---
title: Installer l’interface de ligne de commande Azure pour Windows
description: Comment installer Azure CLI sur Windows
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.prod: azure
ms.date: 09/25/2020
ms.topic: conceptual
ms.devlang: azurecli
ms.technology: azure-cli
ms.custom: devx-track-azurecli
ms.openlocfilehash: e592f4e0787a8e4391e47dc45d1841ff415f24bb
ms.sourcegitcommit: 8bff8b2ce4492ab99ad39390e4c802fb4f4425c8
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/26/2021
ms.locfileid: "105581850"
---
# <a name="install-azure-cli-on-windows"></a>Installer Azure CLI sur Windows

Pour Windows, Azure CLI est installée à l’aide d’un fichier MSI, ce qui vous donne accès à l’interface CLI via l’Invite de commande Windows (CMD) ou PowerShell.
Lors de son installation sur le sous-système Windows pour Linux (WSL), des packages sont disponibles pour votre distribution Linux. Consultez la [page d’installation principale](install-azure-cli.md) pour obtenir la liste des gestionnaires de packages pris en charge ou pour savoir comment installer manuellement avec le sous-système Windows pour Linux.

[!INCLUDE [current-version](includes/current-version.md)]

## <a name="install-or-update"></a>Installation ou mise à jour

Le fichier MSI distribuable est utilisé pour l’installation ou la mise à jour d’Azure CLI sur Windows. Vous n’avez pas besoin de désinstaller les versions actuelles avant d’utiliser le programme d’installation MSI, car celui-ci met à jour toute version existante.

# <a name="microsoft-installer-msi"></a>[Microsoft Installer (MSI)](#tab/azure-cli)

Lorsque le programme d’installation vous demande s’il peut apporter des modifications à votre ordinateur, cliquez sur la case « Oui ».

### <a name="azure-cli-current-version"></a>Version actuelle d’Azure CLI

Téléchargez et installez la version actuelle d’Azure CLI.  Une fois l’installation terminée, vous devez fermer et rouvrir toutes les invites de commandes Windows ou fenêtres PowerShell actives pour pouvoir utiliser Azure CLI.

> [!div class="nextstepaction"]
> [Version actuelle d’Azure CLI](https://aka.ms/installazurecliwindows)

### <a name="azure-cli-beta-version"></a>Version bêta d’Azure CLI

La version bêta d’Azure CLI prend en charge toutes les commandes et reste synchronisée avec la version publiée actuelle.  Pour obtenir des instructions d’installation, consultez [Installer la version bêta d’Azure CLI](install-azure-cli-beta.md). 

# <a name="microsoft-installer-msi-with-command"></a>[Microsoft Installer (MSI) avec commande](#tab/azure-powershell)

### <a name="powershell-command"></a>Commande PowerShell

Vous pouvez également installer Azure CLI en utilisant PowerShell. Démarrez PowerShell en tant qu’administrateur et exécutez la commande suivante :

   ```PowerShell
   Invoke-WebRequest -Uri https://aka.ms/installazurecliwindows -OutFile .\AzureCLI.msi; Start-Process msiexec.exe -Wait -ArgumentList '/I AzureCLI.msi /quiet'; rm .\AzureCLI.msi
   ```

Cette opération télécharge et installe la dernière version d’Azure CLI pour Windows. Si une version est déjà installée, le programme d’installation met à jour la version existante. Une fois l’installation terminée, vous devez rouvrir PowerShell pour utiliser Azure CLI.

### <a name="azure-cli-command-for-update-only"></a>Commande Azure CLI (pour mise à jour uniquement)
[!INCLUDE [az upgrade](includes/az-upgrade.md)]

---

## <a name="run-the-azure-cli"></a>Exécuter Azure CLI

Vous pouvez désormais exécuter l’interface de ligne de commande Azure avec la commande `az` à partir de l’invite de commandes Windows ou PowerShell. PowerShell offre des fonctionnalités de saisie semi-automatique via la touche TAB non disponibles à partir de l’invite de commandes Windows. Pour vous connecter, exécutez la commande [az login](/cli/azure/reference-index#az_login).

[!INCLUDE [interactive-login](includes/interactive-login.md)]

Pour en savoir plus sur les différentes méthodes d’authentification, consultez [Se connecter avec Azure CLI](authenticate-azure-cli.md).

## <a name="troubleshooting"></a>Dépannage

Voici certains problèmes courants lors de l’installation sur Windows. Si vous rencontrez un problème qui n’est pas traité ici, [signalez ce problème sur GitHub](https://github.com/Azure/azure-cli/issues).

### <a name="proxy-blocks-connection"></a>Le proxy bloque la connexion

Si vous ne pouvez pas télécharger le programme d’installation MSI car votre serveur proxy bloque la connexion, vérifiez que votre proxy est configuré correctement. Pour Windows 10, ces paramètres sont gérés dans le volet `Settings > Network & Internet > Proxy`. Contactez votre administrateur système pour connaître les paramètres requis, ou les situations où votre ordinateur peut être géré par configuration ou nécessiter une configuration avancée.

> [!IMPORTANT]
> Ces paramètres sont également requis pour l’accès aux services Azure avec l’interface CLI, PowerShell ou l’invite de commandes. Dans PowerShell, pour ce faire, utilisez la commande suivante :
>
> ```powershell
> (New-Object System.Net.WebClient).Proxy.Credentials = `
>   [System.Net.CredentialCache]::DefaultNetworkCredentials
> ```

Pour obtenir le fichier MSI, votre proxy doit autoriser les connexions HTTPS aux adresses suivantes :

* `https://aka.ms/`
* `https://azcliprod.blob.core.windows.net/`

## <a name="uninstall"></a>Désinstaller l’interface

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

La désinstallation d’Azure CLI s’effectue à partir de la liste « Applications et fonctionnalités » dans Windows. Pour désinstaller :

| Plateforme | Instructions |
|---|---|
| Windows 10 | Démarrer > Paramètres > Applications |
| Windows 8 et Windows 7 | Démarrer > Panneau de configuration > Programmes > Désinstaller un programme |

Une fois sur cet écran, tapez __Azure CLI__ dans la barre de recherche du programme. Le programme à désinstaller est listé sous le nom __Microsoft CLI 2.0 pour Azure__. Sélectionnez cette application, puis cliquez sur le bouton `Uninstall`.

## <a name="next-steps"></a>Étapes suivantes

Maintenant que vous avez installé l’interface CLI, découvrez ses fonctionnalités et ses commandes courantes.

> [!div class="nextstepaction"]
> [Prise en main de l’interface Azure CLI](get-started-with-azure-cli.md)
