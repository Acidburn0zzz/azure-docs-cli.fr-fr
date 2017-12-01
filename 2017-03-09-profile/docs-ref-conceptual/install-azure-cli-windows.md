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
ms.openlocfilehash: 96a123575226f281accf125cb5bb29ee7d14ef2a
ms.sourcegitcommit: 905939cc44764b4d1cc79a9b36c0793f7055a686
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/20/2017
---
# <a name="install-azure-cli-20-on-windows"></a><span data-ttu-id="bb1e0-104">Installation d’Azure CLI 2.0 sur Windows</span><span class="sxs-lookup"><span data-stu-id="bb1e0-104">Install Azure CLI 2.0 on Windows</span></span>

<span data-ttu-id="bb1e0-105">Sous Windows, vous pouvez installer un fichier binaire natif à partir d’un fichier MSI, que vous pouvez utiliser à l’invite de commandes Windows ou de PowerShell.</span><span class="sxs-lookup"><span data-stu-id="bb1e0-105">On Windows, you can install a native binary from an MSI, which you can use through the Windows Command Prompt or PowerShell.</span></span> <span data-ttu-id="bb1e0-106">Si vous exécutez le sous-système Windows pour Linux, des packages sont disponibles pour la distribution que vous exécutez.</span><span class="sxs-lookup"><span data-stu-id="bb1e0-106">If you are running Windows Subsystem for Linux (WSL) there are packages available for the distribution you are running.</span></span> <span data-ttu-id="bb1e0-107">Consultez la [page d’installation principale](install-azure-cli.md) pour obtenir la liste des gestionnaires de packages pris en charge ou pour savoir comment installer manuellement avec le sous-système Windows pour Linux.</span><span class="sxs-lookup"><span data-stu-id="bb1e0-107">See the [main install page](install-azure-cli.md) for the list of supported package managers or how to install manually under WSL.</span></span>

## <a name="install-or-update-with-msi"></a><span data-ttu-id="bb1e0-108">Installer ou mettre à jour avec MSI</span><span class="sxs-lookup"><span data-stu-id="bb1e0-108">Install or update with MSI</span></span>

<span data-ttu-id="bb1e0-109">Le fichier MSI distribuable est utilisé pour l’installation, la mise à jour et la désinstallation de la commande `az` sous Windows.</span><span class="sxs-lookup"><span data-stu-id="bb1e0-109">The MSI distributable is used for installing, updating, and uninstalling the `az` command on Windows.</span></span> <span data-ttu-id="bb1e0-110">Vous pouvez [télécharger le programme d’installation MSI](https://aka.ms/InstallAzureCliWindows), exécutez-le ensuite pour installer ou mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="bb1e0-110">You can [download the MSI installer](https://aka.ms/InstallAzureCliWindows) and then run it to install or update.</span></span>

<span data-ttu-id="bb1e0-111">Lorsque le programme d’installation vous demande s’il peut apporter des modifications à votre ordinateur, cliquez sur la case « Oui ».</span><span class="sxs-lookup"><span data-stu-id="bb1e0-111">When the installer asks if it can make changes to your computer, click the "Yes" box.</span></span>

<span data-ttu-id="bb1e0-112">Vous pouvez désormais exécuter l’interface de ligne de commande Azure avec la commande `az` à partir de l’invite de commandes Windows ou PowerShell.</span><span class="sxs-lookup"><span data-stu-id="bb1e0-112">You can now run the Azure CLI with the `az` command from either Windows Command Prompt or PowerShell.</span></span>

## <a name="uninstall-with-msi"></a><span data-ttu-id="bb1e0-113">Désinstaller avec MSI</span><span class="sxs-lookup"><span data-stu-id="bb1e0-113">Uninstall with MSI</span></span>

<span data-ttu-id="bb1e0-114">Si jamais vous décidez de désinstaller l’interface de ligne de commande Azure, nous sommes désolés de vous voir partir.</span><span class="sxs-lookup"><span data-stu-id="bb1e0-114">If you ever decide to uninstall the Azure CLI, we're sorry to see you go.</span></span> <span data-ttu-id="bb1e0-115">Avant de désinstaller, utilisez la commande `az feedback`, afin de nous donner quelques raisons pour lesquelles vous avez choisi de désinstaller et nous aider à améliorer l’expérience CLI.</span><span class="sxs-lookup"><span data-stu-id="bb1e0-115">Before you uninstall, use the `az feedback` command to give us some reasons why you chose to uninstall and how we could improve the CLI experience.</span></span> <span data-ttu-id="bb1e0-116">Nous souhaitons nous assurer que l’interface de ligne de commande Azure est aussi conviviale et exempte de bogues que possible.</span><span class="sxs-lookup"><span data-stu-id="bb1e0-116">We want to make sure that the Azure CLI is as bug-free and user-friendly as we can make it.</span></span> <span data-ttu-id="bb1e0-117">Vous pouvez également [signaler un problème lié à GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="bb1e0-117">You can also [file a github issue](https://github.com/Azure/azure-cli/issues).</span></span>

<span data-ttu-id="bb1e0-118">La désinstallation peut être réalisée en exécutant le fichier MSI à nouveau, en choisissant l’option « Désinstaller ».</span><span class="sxs-lookup"><span data-stu-id="bb1e0-118">Uninstalling can be done by running the MSI again, and choosing the "Uninstall" option.</span></span> <span data-ttu-id="bb1e0-119">Vous pouvez [télécharger le programme d’installation MSI](https://aka.ms/InstallAzureCliWindows) si vous n’y avez plus accès.</span><span class="sxs-lookup"><span data-stu-id="bb1e0-119">You can [download the MSI installer](https://aka.ms/InstallAzureCliWindows) if you no longer have it available.</span></span>
