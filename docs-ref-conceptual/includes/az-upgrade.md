---
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 09/25/2020
ms.topic: include
ms.openlocfilehash: 4d8baf2e2a2f3b3018569801f5c6e5bde30f05af
ms.sourcegitcommit: 9c232f011357b56f5ae35ffedfa3a3e7e27774ad
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/31/2021
ms.locfileid: "106073549"
---
L’interface CLI fournit une commande dans l’outil pour effectuer une mise à jour vers la version la plus récente :

```azurecli
az upgrade
```

> [!NOTE]
>
> La commande `az upgrade` a été ajoutée dans la version 2.11.0 et elle ne fonctionne pas avec les versions antérieures. Les anciennes versions peuvent être mises à jour en les réinstallant, comme décrit dans [Installer l’interface Azure CLI](/cli/azure/install-azure-cli.md).
>
> Cette commande met également à jour toutes les extensions installées par défaut. Pour plus d’options `az upgrade`, consultez la [page de référence des commandes](/cli/azure/reference-index#az_upgrade).
