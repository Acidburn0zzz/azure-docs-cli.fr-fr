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
Si vous ne parvenez pas à vous connecter à une ressource externe en raison d’un proxy, vérifiez que vous avez correctement défini les variables `HTTP_PROXY` et `HTTPS_PROXY` dans votre interpréteur de commandes. Vous devez contacter votre administrateur système pour connaître les hôtes et ports à utiliser pour ces proxies.

Ces valeurs sont respectées par de nombreux programmes Linux, notamment ceux qui sont utilisés dans le processus d’installation. Pour obtenir ces valeurs :

```bash
# No auth
export HTTP_PROXY=http://[proxy]:[port]
export HTTPS_PROXY=https://[proxy]:[port]

# Basic auth
export HTTP_PROXY=http://[username]:[password]@[proxy]:[port]
export HTTPS_PROXY=https://[username]:[password]@[proxy]:[port]
```

> [!IMPORTANT]
> Si vous vous trouvez derrière un proxy, ces variables d’interpréteur de commandes doivent être définies pour se connecter aux services Azure avec l’interface CLI.
> Si vous n’utilisez pas l’authentification de base, il est recommandé d’exporter ces variables dans votre fichier `.bashrc`.
> Suivez toujours les stratégies de sécurité de votre entreprise et les exigences de votre administrateur système.
