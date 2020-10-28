---
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 09/25/2020
ms.topic: include
ms.openlocfilehash: b931b465c8d4e7f6a507630a02f9fb7f06579a89
ms.sourcegitcommit: 19c24ebcd1e15ac23ca40ebc28b8c4804bd1327f
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/14/2020
ms.locfileid: "92038522"
---
<span data-ttu-id="396c2-101">L’interface CLI fournit une commande dans l’outil pour effectuer une mise à jour vers la version la plus récente :</span><span class="sxs-lookup"><span data-stu-id="396c2-101">The CLI provides an in-tool command to update to the latest version:</span></span>

```azurecli
az upgrade
```

> [!NOTE]
>
> <span data-ttu-id="396c2-102">La commande `az upgrade` a été ajoutée dans la version 2.11.0 et elle ne fonctionne pas avec les versions antérieures.</span><span class="sxs-lookup"><span data-stu-id="396c2-102">The `az upgrade` command was added in version 2.11.0 and will not work with versions prior to 2.11.0.</span></span>
>
> <span data-ttu-id="396c2-103">Cette commande met également à jour toutes les extensions installées par défaut.</span><span class="sxs-lookup"><span data-stu-id="396c2-103">This command will also update all installed extensions by default.</span></span> <span data-ttu-id="396c2-104">Pour plus d’options `az upgrade`, consultez la [page de référence des commandes](/cli/azure/reference-index#az_upgrade).</span><span class="sxs-lookup"><span data-stu-id="396c2-104">For more `az upgrade` options, please refer to the [command reference page](/cli/azure/reference-index#az_upgrade).</span></span>
