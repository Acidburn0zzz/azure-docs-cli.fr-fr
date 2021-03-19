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
# <a name="install-azure-cli-beta-version"></a><span data-ttu-id="faf9a-103">Installer la version bêta d’Azure CLI</span><span class="sxs-lookup"><span data-stu-id="faf9a-103">Install Azure CLI beta version</span></span>

<span data-ttu-id="faf9a-104">La nouvelle version bêta d’Azure CLI qui vient d’être publiée renforce la sécurité du cache des jetons, des jetons d’accès et des certificats SSL.</span><span class="sxs-lookup"><span data-stu-id="faf9a-104">A new beta version of the Azure CLI has been released that offers increased security for token cache, access tokens and SSL certificates.</span></span>  <span data-ttu-id="faf9a-105">Vous pouvez installer cette version bêta dans les environnements Windows, macOS et Linux. Elle reste synchronisée avec la version la plus récente.</span><span class="sxs-lookup"><span data-stu-id="faf9a-105">This beta vesion can be installed in Windows, macOS and Linux environments and will stay in sync with the most recent release.</span></span>

> [!NOTE]
>
>  <span data-ttu-id="faf9a-106">Des CHANGEMENTS CASSANTS sont introduits dans cette version.</span><span class="sxs-lookup"><span data-stu-id="faf9a-106">BREAKING CHANGES are introduced in this release.</span></span>  <span data-ttu-id="faf9a-107">Lisez attentivement toutes les [notes de publication](/cli/azure/release-notes-azure-cli?tabs=azure-cli-beta) avant de procéder à l’installation.</span><span class="sxs-lookup"><span data-stu-id="faf9a-107">Carefully read all [release notes](/cli/azure/release-notes-azure-cli?tabs=azure-cli-beta) prior to installation.</span></span>
>
> <span data-ttu-id="faf9a-108">La version bêta ne garantit pas la qualité du produit. Ne l’utilisez pas dans votre environnement de production.</span><span class="sxs-lookup"><span data-stu-id="faf9a-108">The beta version does not guarantee product level quality so it should not be used in your production environment.</span></span>

## <a name="understand-beta-changes"></a><span data-ttu-id="faf9a-109">Comprendre les changements apportés par la version bêta</span><span class="sxs-lookup"><span data-stu-id="faf9a-109">Understand beta changes</span></span>

### <a name="accesstokensjson-deprecation"></a><span data-ttu-id="faf9a-110">Dépréciation de `accessTokens.json`</span><span class="sxs-lookup"><span data-stu-id="faf9a-110">`accessTokens.json` deprecation</span></span>

<span data-ttu-id="faf9a-111">La version actuelle d’Azure CLI enregistre les jetons d’actualisation ADAL et les jetons d’accès dans `~/.azure/accessToken.json`.</span><span class="sxs-lookup"><span data-stu-id="faf9a-111">The current Azure CLI saves the ADAL refresh tokens and access tokens to `~/.azure/accessToken.json`.</span></span> <span data-ttu-id="faf9a-112">Azure CLI bêta utilise MSAL et ne génère plus `accessTokens.json`.</span><span class="sxs-lookup"><span data-stu-id="faf9a-112">Azure CLI beta uses MSAL and will no longer generate `accessTokens.json`.</span></span>  <span data-ttu-id="faf9a-113">Les jetons sont enregistrés dans le cache de jetons partagé de MSAL, appelé `msal.cache`.</span><span class="sxs-lookup"><span data-stu-id="faf9a-113">Tokens will be saved to MSAL's shared token cache called `msal.cache`.</span></span> 

<span data-ttu-id="faf9a-114">Le cache de jetons MSAL étant chiffré sur Windows, macOS et Linux avec un environnement de bureau, l’accès direct au cache de jetons MSAL est impossible.</span><span class="sxs-lookup"><span data-stu-id="faf9a-114">The MSAL token cache will be encrypted on Windows, macOS and Linux with a desktop environment; therefore, directly accessing the MSAL token cache will not work.</span></span> <span data-ttu-id="faf9a-115">Tout workflow existant qui dépend de `accessTokens.json` cesse donc de fonctionner.</span><span class="sxs-lookup"><span data-stu-id="faf9a-115">Any existing workflow depending on `accessTokens.json` will stop working.</span></span>

<span data-ttu-id="faf9a-116">Voici quelques solutions alternatives que vous pouvez adopter :</span><span class="sxs-lookup"><span data-stu-id="faf9a-116">Below are several alternatives you may consider:</span></span> 

#### <a name="calling-az-account-get-access-token"></a><span data-ttu-id="faf9a-117">Appel de `az account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="faf9a-117">Calling `az account get-access-token`</span></span>

<span data-ttu-id="faf9a-118">Vous pouvez appeler manuellement `az account get-access-token` dans un terminal ou utiliser le sous-processus pour l’appeler à partir d’un autre langage de programmation.</span><span class="sxs-lookup"><span data-stu-id="faf9a-118">You can manually call `az account get-access-token` in a terminal or use subprocess to call it from another programming language.</span></span> <span data-ttu-id="faf9a-119">Par défaut, le jeton retourné correspond à l’abonnement/au locataire par défaut indiqués dans `az account show`.</span><span class="sxs-lookup"><span data-stu-id="faf9a-119">By default, the returned token is for the default subscription/tenant shown in `az account show`.</span></span>

#### <a name="using-azureclicredential"></a><span data-ttu-id="faf9a-120">Utilisation de `AzureCliCredential`</span><span class="sxs-lookup"><span data-stu-id="faf9a-120">Using `AzureCliCredential`</span></span>

<span data-ttu-id="faf9a-121">`AzureCliCredential` est un type d’informations d’identification dans tous les kits SDK de langage existants.</span><span class="sxs-lookup"><span data-stu-id="faf9a-121">`AzureCliCredential` is a credential type in all existing language SDKs.</span></span> <span data-ttu-id="faf9a-122">Il utilise en interne le sous-processus pour appeler `az account get-access-token` afin d’obtenir un jeton d’accès à partir des comptes CLI actuellement connectés.</span><span class="sxs-lookup"><span data-stu-id="faf9a-122">It internally uses subprocess to call `az account get-access-token` to gets an access token from current logged in CLI accounts.</span></span> 

#### <a name="accessing-shared-msal-cache"></a><span data-ttu-id="faf9a-123">Accès au cache MSAL partagé</span><span class="sxs-lookup"><span data-stu-id="faf9a-123">Accessing shared MSAL cache</span></span>

<span data-ttu-id="faf9a-124">Les applications internes peuvent utiliser `SharedTokenCacheCredential` à partir du kit SDK Azure Identity pour accéder directement au cache MSAL partagé.</span><span class="sxs-lookup"><span data-stu-id="faf9a-124">First party apps can use `SharedTokenCacheCredential` from Azure Identity SDK to directly access the shared MSAL cache.</span></span>

## <a name="install-azure-cli-beta"></a><span data-ttu-id="faf9a-125">Installer Azure CLI bêta</span><span class="sxs-lookup"><span data-stu-id="faf9a-125">Install Azure CLI beta</span></span>

<span data-ttu-id="faf9a-126">Azure CLI repose sur [Python](https://www.python.org/).</span><span class="sxs-lookup"><span data-stu-id="faf9a-126">Azure CLI is built on [Python](https://www.python.org/).</span></span> <span data-ttu-id="faf9a-127">Les versions de Python prises en charge sont 3.6, 3.7 et 3.8.</span><span class="sxs-lookup"><span data-stu-id="faf9a-127">The supported Python versions are 3.6, 3.7, 3.8.</span></span> <span data-ttu-id="faf9a-128">Sur Windows, vous devez d’abord [installer Python](https://www.python.org/downloads/windows/).</span><span class="sxs-lookup"><span data-stu-id="faf9a-128">On Windows, you will first need to [install Python](https://www.python.org/downloads/windows/).</span></span>

<span data-ttu-id="faf9a-129">Vous pouvez uniquement installer Azure CLI bêta avec `pip` à partir d’un référentiel Microsoft.</span><span class="sxs-lookup"><span data-stu-id="faf9a-129">Azure CLI beta can only be installed with `pip` from a Microsoft repository.</span></span>  <span data-ttu-id="faf9a-130">Utilisez [Azure Cloud Shell](https://shell.azure.com) pour exécuter les commandes suivantes, ou `python3`, en fonction de la distribution de Linux ou de la version installée de Python.</span><span class="sxs-lookup"><span data-stu-id="faf9a-130">Use [Azure Cloud Shell](https://shell.azure.com) to execute the following commands, or `python3`, depending on the Linux distribution or your installed Python version.</span></span>

<span data-ttu-id="faf9a-131">Pour ne pas remplacer la version d’Azure CLI installée, nous vous recommandons d’installer la version bêta dans un [environnement virtuel](https://docs.python.org/3/tutorial/venv.html).</span><span class="sxs-lookup"><span data-stu-id="faf9a-131">To avoid overwriting your installed Azure CLI, we recommend installing the beta version in a [virtual environment](https://docs.python.org/3/tutorial/venv.html).</span></span>

1. <span data-ttu-id="faf9a-132">Créer un environnement virtuel</span><span class="sxs-lookup"><span data-stu-id="faf9a-132">Create a virtual environment</span></span>

   <span data-ttu-id="faf9a-133">Accédez au dossier dans lequel vous souhaitez créer l’environnement virtuel, puis exécutez :</span><span class="sxs-lookup"><span data-stu-id="faf9a-133">Navigate to the folder where you want to create the virtual environment, then run:</span></span>

   ```bash
   python -m venv <env_name>
   ```

1. <span data-ttu-id="faf9a-134">Activer l’environnement virtuel</span><span class="sxs-lookup"><span data-stu-id="faf9a-134">Activate the virtual environment</span></span>

      ### <a name="windows-powershell"></a>[<span data-ttu-id="faf9a-135">Windows PowerShell</span><span class="sxs-lookup"><span data-stu-id="faf9a-135">Windows PowerShell</span></span>](#tab/powershell)

   ```powershell
   . .\$env\Scripts\Activate.ps1
   ```

   ### <a name="linuxmacos-bash"></a>[<span data-ttu-id="faf9a-136">Linux/macOS Bash</span><span class="sxs-lookup"><span data-stu-id="faf9a-136">Linux/macOS Bash</span></span>](#tab/bash)

   ```bash
   . $env/bin/activate
   ```
   ---
   <span data-ttu-id="faf9a-137">Vous pouvez également utiliser ces commandes pour réactiver votre environnement virtuel.</span><span class="sxs-lookup"><span data-stu-id="faf9a-137">These commands can also be used to reactivate your virtual environment.</span></span>

1. <span data-ttu-id="faf9a-138">Installer Azure CLI bêta</span><span class="sxs-lookup"><span data-stu-id="faf9a-138">Install Azure CLI beta</span></span>

   ```bash
   pip install --pre --extra-index-url https://azcliprod.blob.core.windows.net/beta/simple/ azure-cli
   ```

1. <span data-ttu-id="faf9a-139">Désactiver l’environnement virtuel</span><span class="sxs-lookup"><span data-stu-id="faf9a-139">Deactivate the virtual environment</span></span>

   <span data-ttu-id="faf9a-140">Quand vous avez fini d’utiliser Azure CLI bêta, vous pouvez fermer la fenêtre du terminal ou utiliser la commande `deactivate`.</span><span class="sxs-lookup"><span data-stu-id="faf9a-140">After you finish using Azure CLI beta, you can close the terminal window, or use the `deactivate` command.</span></span>

   ```bash
   deactivate
   ```

## <a name="uninstall-azure-cli-beta"></a><span data-ttu-id="faf9a-141">Désinstaller Azure CLI bêta</span><span class="sxs-lookup"><span data-stu-id="faf9a-141">Uninstall Azure CLI beta</span></span>

<span data-ttu-id="faf9a-142">Pour désinstaller Azure CLI bêta, supprimez le dossier d’environnement virtuel.</span><span class="sxs-lookup"><span data-stu-id="faf9a-142">To uninstall Azure CLI beta, delete the virtual environment folder.</span></span>

### <a name="windows-powershell"></a>[<span data-ttu-id="faf9a-143">Windows PowerShell</span><span class="sxs-lookup"><span data-stu-id="faf9a-143">Windows PowerShell</span></span>](#tab/powershell)

```powershell
Remove-Item -Force -Recurse <env_name>
```

### <a name="linuxmacos-bash"></a>[<span data-ttu-id="faf9a-144">Linux/macOS Bash</span><span class="sxs-lookup"><span data-stu-id="faf9a-144">Linux/macOS Bash</span></span>](#tab/bash)

```bash
rm -rf <env_name>
```

---
