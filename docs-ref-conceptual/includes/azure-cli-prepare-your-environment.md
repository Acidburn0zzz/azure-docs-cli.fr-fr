---
ms.topic: include
ms.date: 09/10/2020
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.custom: devx-track-azurecli
ms.openlocfilehash: 4835cc399942fba3cbf7408b1309480cd2bcc152
ms.sourcegitcommit: bd2dbc80328936dadd211764d25c32a14fc58083
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/04/2021
ms.locfileid: "100631161"
---
## <a name="prerequisites"></a><span data-ttu-id="b28cb-101">Prérequis</span><span class="sxs-lookup"><span data-stu-id="b28cb-101">Prerequisites</span></span>

- <span data-ttu-id="b28cb-102">Utilisez [Azure Cloud Shell](/azure/cloud-shell/quickstart) à l’aide de l’environnement Bash.</span><span class="sxs-lookup"><span data-stu-id="b28cb-102">Use [Azure Cloud Shell](/azure/cloud-shell/quickstart) using the bash environment.</span></span>

   <span data-ttu-id="b28cb-103">[![Lancement de l’incorporation](https://shell.azure.com/images/launchcloudshell.png "Lancement d’Azure Cloud Shell")](https://shell.azure.com)</span><span class="sxs-lookup"><span data-stu-id="b28cb-103">[![Embed launch](https://shell.azure.com/images/launchcloudshell.png "Launch Azure Cloud Shell")](https://shell.azure.com)</span></span>   
- <span data-ttu-id="b28cb-104">Si vous préférez, [installez](../install-azure-cli.md) l’interface Azure CLI pour exécuter les commandes de référence de l’interface de ligne de commande.</span><span class="sxs-lookup"><span data-stu-id="b28cb-104">If you prefer, [install](../install-azure-cli.md) the Azure CLI to run CLI reference commands.</span></span>
   - <span data-ttu-id="b28cb-105">Si vous utilisez une installation locale, connectez-vous à Azure CLI à l’aide de la commande [az login](/cli/azure/reference-index#az_login).</span><span class="sxs-lookup"><span data-stu-id="b28cb-105">If you're using a local install, sign in with Azure CLI by using the [az login](/cli/azure/reference-index#az_login) command.</span></span>  <span data-ttu-id="b28cb-106">Pour finir le processus d’authentification, suivez les étapes affichées dans votre terminal.</span><span class="sxs-lookup"><span data-stu-id="b28cb-106">To finish the authentication process, follow the steps displayed in your terminal.</span></span>  <span data-ttu-id="b28cb-107">Consultez [Se connecter avec Azure CLI](../authenticate-azure-cli.md) pour connaître les autres options de connexion.</span><span class="sxs-lookup"><span data-stu-id="b28cb-107">See [Sign in with Azure CLI](../authenticate-azure-cli.md) for additional sign-in options.</span></span>
  - <span data-ttu-id="b28cb-108">Lorsque vous y êtes invité, installez les extensions Azure CLI lors de la première utilisation.</span><span class="sxs-lookup"><span data-stu-id="b28cb-108">When you're prompted, install Azure CLI extensions on first use.</span></span>  <span data-ttu-id="b28cb-109">Pour plus d’informations sur les extensions, consultez [Utiliser des extensions avec Azure CLI](../azure-cli-extensions-overview.md).</span><span class="sxs-lookup"><span data-stu-id="b28cb-109">For more information about extensions, see [Use extensions with Azure CLI](../azure-cli-extensions-overview.md).</span></span>
  - <span data-ttu-id="b28cb-110">Exécutez [az version](/cli/azure/reference-index#az_version) pour rechercher la version et les bibliothèques dépendantes installées.</span><span class="sxs-lookup"><span data-stu-id="b28cb-110">Run [az version](/cli/azure/reference-index#az_version) to find the version and dependent libraries that are installed.</span></span> <span data-ttu-id="b28cb-111">Pour effectuer une mise à niveau vers la dernière version, exécutez [az upgrade](/cli/azure/reference-index#az_upgrade).</span><span class="sxs-lookup"><span data-stu-id="b28cb-111">To upgrade to the latest version, run [az upgrade](/cli/azure/reference-index#az_upgrade).</span></span>
