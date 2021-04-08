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
<span data-ttu-id="0e61b-101">L’interface CLI fournit une commande dans l’outil pour effectuer une mise à jour vers la version la plus récente :</span><span class="sxs-lookup"><span data-stu-id="0e61b-101">The CLI provides an in-tool command to update to the latest version:</span></span>

```azurecli
az upgrade
```

> [!NOTE]
>
> <span data-ttu-id="0e61b-102">La commande `az upgrade` a été ajoutée dans la version 2.11.0 et elle ne fonctionne pas avec les versions antérieures.</span><span class="sxs-lookup"><span data-stu-id="0e61b-102">The `az upgrade` command was added in version 2.11.0 and will not work with versions prior to 2.11.0.</span></span> <span data-ttu-id="0e61b-103">Les anciennes versions peuvent être mises à jour en les réinstallant, comme décrit dans [Installer l’interface Azure CLI](/cli/azure/install-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="0e61b-103">Older versions can be updated by reinstalling as described in [Install the Azure CLI](/cli/azure/install-azure-cli.md).</span></span>
>
> <span data-ttu-id="0e61b-104">Cette commande met également à jour toutes les extensions installées par défaut.</span><span class="sxs-lookup"><span data-stu-id="0e61b-104">This command will also update all installed extensions by default.</span></span> <span data-ttu-id="0e61b-105">Pour plus d’options `az upgrade`, consultez la [page de référence des commandes](/cli/azure/reference-index#az_upgrade).</span><span class="sxs-lookup"><span data-stu-id="0e61b-105">For more `az upgrade` options, please refer to the [command reference page](/cli/azure/reference-index#az_upgrade).</span></span>
