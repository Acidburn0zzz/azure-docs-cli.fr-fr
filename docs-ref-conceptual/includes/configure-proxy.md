---
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/28/2019
ms.topic: include
ms.prod: azure
ms.technology: azure-cli
ms.openlocfilehash: 676f33377a4e7122941bc789c51465b7f34aa1d3
ms.sourcegitcommit: 08043c47d3ccf23522b91e6bba3932e312c04c7f
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/04/2019
ms.locfileid: "66516260"
---
<span data-ttu-id="64eb7-101">Si vous ne parvenez pas à vous connecter à une ressource externe en raison d’un proxy, vérifiez que vous avez correctement défini les variables `HTTP_PROXY` et `HTTPS_PROXY` dans votre interpréteur de commandes.</span><span class="sxs-lookup"><span data-stu-id="64eb7-101">If you're unable to connect to an external resource due to a proxy, make sure that you've correctly set the `HTTP_PROXY` and `HTTPS_PROXY` variables in your shell.</span></span> <span data-ttu-id="64eb7-102">Vous devez contacter votre administrateur système pour connaître les hôtes et ports à utiliser pour ces proxies.</span><span class="sxs-lookup"><span data-stu-id="64eb7-102">You will need to contact your system administrator to know what host(s) and port(s) to use for these proxies.</span></span>

<span data-ttu-id="64eb7-103">Ces valeurs sont respectées par de nombreux programmes Linux, notamment ceux qui sont utilisés dans le processus d’installation.</span><span class="sxs-lookup"><span data-stu-id="64eb7-103">These values are respected by many Linux programs, including those which are used in the install process.</span></span> <span data-ttu-id="64eb7-104">Pour obtenir ces valeurs :</span><span class="sxs-lookup"><span data-stu-id="64eb7-104">To set these values:</span></span>

```bash
# No auth
export HTTP_PROXY=http://[proxy]:[port]
export HTTPS_PROXY=https://[proxy]:[port]

# Basic auth
export HTTP_PROXY=http://[username]:[password]@[proxy]:[port]
export HTTPS_PROXY=https://[username]:[password]@[proxy]:[port]
```

> [!IMPORTANT]
> <span data-ttu-id="64eb7-105">Si vous vous trouvez derrière un proxy, ces variables d’interpréteur de commandes doivent être définies pour se connecter aux services Azure avec l’interface CLI.</span><span class="sxs-lookup"><span data-stu-id="64eb7-105">If you are behind a proxy, these shell variables must be set to connect to Azure services with the CLI.</span></span>
> <span data-ttu-id="64eb7-106">Si vous n’utilisez pas l’authentification de base, il est recommandé d’exporter ces variables dans votre fichier `.bashrc`.</span><span class="sxs-lookup"><span data-stu-id="64eb7-106">If you are not using basic auth, it's recommended to export these variables in your `.bashrc` file.</span></span>
> <span data-ttu-id="64eb7-107">Suivez toujours les stratégies de sécurité de votre entreprise et les exigences de votre administrateur système.</span><span class="sxs-lookup"><span data-stu-id="64eb7-107">Always follow your business' security policies and the requirements of your system administrator.</span></span>
