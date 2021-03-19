---
title: Installer la version bêta d’Azure CLI
description: Informations de référence sur l’installation de la version bêta d’Azure CLI
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 02/09/2021
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: ccee5c30d625522525065f5cbd57637427d49b86
ms.sourcegitcommit: f9e23f29c59c6957d3df4d5ca2f4425093e6fd80
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/16/2021
ms.locfileid: "103554916"
---
# <a name="install-azure-cli-beta-version"></a>Installer la version bêta d’Azure CLI

La nouvelle version bêta d’Azure CLI qui vient d’être publiée renforce la sécurité du cache des jetons, des jetons d’accès et des certificats SSL.  Vous pouvez installer cette version bêta dans les environnements Windows, macOS et Linux. Elle reste synchronisée avec la version la plus récente.

> [!NOTE]
>
>  Des CHANGEMENTS CASSANTS sont introduits dans cette version.  Lisez attentivement toutes les [notes de publication](/cli/azure/release-notes-azure-cli?tabs=azure-cli-beta) avant de procéder à l’installation.
>
> La version bêta ne garantit pas la qualité du produit. Ne l’utilisez pas dans votre environnement de production.

## <a name="understand-beta-changes"></a>Comprendre les changements apportés par la version bêta

### <a name="accesstokensjson-deprecation"></a>Dépréciation de `accessTokens.json`

La version actuelle d’Azure CLI enregistre les jetons d’actualisation ADAL et les jetons d’accès dans `~/.azure/accessToken.json`. Azure CLI bêta utilise MSAL et ne génère plus `accessTokens.json`.  Les jetons sont enregistrés dans le cache de jetons partagé de MSAL, appelé `msal.cache`. 

Le cache de jetons MSAL étant chiffré sur Windows, macOS et Linux avec un environnement de bureau, l’accès direct au cache de jetons MSAL est impossible. Tout workflow existant qui dépend de `accessTokens.json` cesse donc de fonctionner.

Voici quelques solutions alternatives que vous pouvez adopter : 

#### <a name="calling-az-account-get-access-token"></a>Appel de `az account get-access-token`

Vous pouvez appeler manuellement `az account get-access-token` dans un terminal ou utiliser le sous-processus pour l’appeler à partir d’un autre langage de programmation. Par défaut, le jeton retourné correspond à l’abonnement/au locataire par défaut indiqués dans `az account show`.

#### <a name="using-azureclicredential"></a>Utilisation de `AzureCliCredential`

`AzureCliCredential` est un type d’informations d’identification dans tous les kits SDK de langage existants. Il utilise en interne le sous-processus pour appeler `az account get-access-token` afin d’obtenir un jeton d’accès à partir des comptes CLI actuellement connectés. 

#### <a name="accessing-shared-msal-cache"></a>Accès au cache MSAL partagé

Les applications internes peuvent utiliser `SharedTokenCacheCredential` à partir du kit SDK Azure Identity pour accéder directement au cache MSAL partagé.

## <a name="install-azure-cli-beta"></a>Installer Azure CLI bêta

Azure CLI repose sur [Python](https://www.python.org/). Les versions de Python prises en charge sont 3.6, 3.7 et 3.8. Sur Windows, vous devez d’abord [installer Python](https://www.python.org/downloads/windows/).

Vous pouvez uniquement installer Azure CLI bêta avec `pip` à partir d’un référentiel Microsoft.  Utilisez [Azure Cloud Shell](https://shell.azure.com) pour exécuter les commandes suivantes, ou `python3`, en fonction de la distribution de Linux ou de la version installée de Python.

Pour ne pas remplacer la version d’Azure CLI installée, nous vous recommandons d’installer la version bêta dans un [environnement virtuel](https://docs.python.org/3/tutorial/venv.html).

1. Créer un environnement virtuel

   Accédez au dossier dans lequel vous souhaitez créer l’environnement virtuel, puis exécutez :

   ```bash
   python -m venv <env_name>
   ```

1. Activer l’environnement virtuel

      ### <a name="windows-powershell"></a>[Windows PowerShell](#tab/powershell)

   ```powershell
   . .\$env\Scripts\Activate.ps1
   ```

   ### <a name="linuxmacos-bash"></a>[Linux/macOS Bash](#tab/bash)

   ```bash
   . $env/bin/activate
   ```
   ---
   Vous pouvez également utiliser ces commandes pour réactiver votre environnement virtuel.

1. Installer Azure CLI bêta

   ```bash
   pip install --pre --extra-index-url https://azcliprod.blob.core.windows.net/beta/simple/ azure-cli
   ```

1. Désactiver l’environnement virtuel

   Quand vous avez fini d’utiliser Azure CLI bêta, vous pouvez fermer la fenêtre du terminal ou utiliser la commande `deactivate`.

   ```bash
   deactivate
   ```

## <a name="uninstall-azure-cli-beta"></a>Désinstaller Azure CLI bêta

Pour désinstaller Azure CLI bêta, supprimez le dossier d’environnement virtuel.

### <a name="windows-powershell"></a>[Windows PowerShell](#tab/powershell)

```powershell
Remove-Item -Force -Recurse <env_name>
```

### <a name="linuxmacos-bash"></a>[Linux/macOS Bash](#tab/bash)

```bash
rm -rf <env_name>
```

---
