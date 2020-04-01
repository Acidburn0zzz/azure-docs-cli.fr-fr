---
title: Installer l’interface de ligne de commande Azure pour Windows
description: Comment installer Azure CLI sur Windows
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 05/01/2019
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: c5e9118a04b0dc608309093866307fdc7083f591
ms.sourcegitcommit: b5ecfc168489cd0d96462d6decf83e8b26a10194
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/31/2020
ms.locfileid: "80417845"
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

Vous pouvez également installer Azure CLI en utilisant PowerShell. Démarrez PowerShell en tant qu’administrateur et exécutez la commande suivante :

   ```PowerShell
   Invoke-WebRequest -Uri https://aka.ms/installazurecliwindows -OutFile .\AzureCLI.msi; Start-Process msiexec.exe -Wait -ArgumentList '/I AzureCLI.msi /quiet'; rm .\AzureCLI.msi
   ```
Cette opération télécharge et installe la dernière version d’Azure CLI pour Windows. Si vous aviez déjà installé une version, celle-ci est mise à jour. Une fois l’installation terminée, vous devez rouvrir PowerShell pour utiliser Azure CLI.

Vous pouvez désormais exécuter l’interface de ligne de commande Azure avec la commande `az` à partir de l’invite de commandes Windows ou PowerShell. PowerShell offre des fonctionnalités de saisie semi-automatique via la touche TAB non disponibles à partir de l’invite de commandes Windows. Pour vous connecter, exécutez la commande [az login](/cli/azure/reference-index#az-login).

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
* `https://azurecliprod.blob.core.windows.net/`

## <a name="uninstall"></a>Désinstaller l’interface

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

La désinstallation d’Azure CLI s’effectue à partir de la liste « Applications et fonctionnalités » dans Windows. Pour désinstaller :

| Plateforme | Instructions |
|---|---|
| Windows 10 | Démarrer > Paramètres > Applications |
| Windows 8<br/>Windows 7 | Démarrer > Panneau de configuration > Programmes > Désinstaller un programme |

Une fois sur cet écran, tapez __Azure CLI__ dans la barre de recherche du programme. Le programme à désinstaller est listé sous le nom __Microsoft CLI 2.0 pour Azure__. Sélectionnez cette application, puis cliquez sur le bouton `Uninstall`.

## <a name="next-steps"></a>Étapes suivantes

Maintenant que vous avez installé l’interface CLI, découvrez ses fonctionnalités et ses commandes courantes.

> [!div class="nextstepaction"]
> [Prise en main de l’interface Azure CLI](get-started-with-azure-cli.md)
