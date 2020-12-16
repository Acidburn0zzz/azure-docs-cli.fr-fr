---
title: Mettre à jour Azure CLI
description: Informations de référence pour la mise à jour d’Azure CLI
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 10/19/2020
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: 475b58bca5ec9dca52a70416cb89860dcbd39278
ms.sourcegitcommit: e1faf297ba2cdf2ba7e821fbeedff9c9a724c975
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/16/2020
ms.locfileid: "97576783"
---
# <a name="update-the-azure-cli"></a>Mettre à jour Azure CLI

Vous pouvez vous servir de gestionnaires de packages pour mettre à jour une installation locale de l’interface de ligne de commande Azure CLI dans les environnements Windows, macOS et Linux (consultez la section `Update` dans les instructions d’installation propres à chaque plateforme). L’interface CLI propose également des commandes dans l’outil pour effectuer une mise à niveau manuelle ou automatique.

## <a name="manual-update"></a>Mise à niveau manuelle
[!INCLUDE [az-upgrade](includes/az-upgrade.md)]

La commande `az upgrade` est prise en charge sur Windows, macOS et certaines distributions Linux pourvu que l’installation soit prise en charge. Elle prend uniquement en charge la mise à niveau vers la dernière version. Si vous exécutez Azure CLI via Azure Cloud Shell, il est très probable que vous utilisez déjà l’installation la plus récente d’Azure CLI. Si ce n’est pour une raison déterminée telle que la publication ad-hoc d’une version de correctif de bogue mineur, vous devez attendre la prochaine build d’Azure Cloud Shell, car la commande `az upgrade` n’est pas prise en charge dans Azure Cloud Shell.

Quand `azure-cli` est déjà la version la plus récente, l’exécution de `az upgrade` entraîne la vérification et la mise à jour de toutes les [extensions](azure-cli-extensions-overview.md) installées.

## <a name="automatic-update"></a>Mise à jour automatique

Par défaut, la mise à niveau automatique est désactivée pour Azure CLI. Si vous voulez être certain d’avoir toujours la dernière version, vous pouvez activer la mise à niveau automatique via la [configuration](/cli/azure/config).

```azurecli
az config set auto-upgrade.enable=yes
```

Azure CLI vérifie alors régulièrement s’il existe une nouvelle version. Si c’est le cas, vous êtes invité à procéder à la mise à niveau après l’exécution d’une commande, le cas échéant.

Il se peut que le message d’invite et les messages de sortie qui s’affichent pendant la mise à niveau interrompent le résultat de votre commande si elle est assignée à une variable ou si elle fait partie d’un flux automatisé. Pour éviter toute interruption, vous pouvez utiliser la configuration suivante pour permettre à la mise à jour de se dérouler automatiquement sans confirmation et pour faire en sorte que seuls les avertissements et les erreurs s’affichent pendant la mise à niveau.

```azurecli
az config set auto-upgrade.prompt=no
```

Par défaut, toutes les extensions installées sont aussi mises à jour. Vous pouvez désactiver la mise à jour des extensions via la configuration.

```azurecli
az config set auto-upgrade.all=no
```

> [!NOTE]
> Attendez que la commande `az upgrade` prenne fin avant de passer au jeu de commandes suivant, car les nouvelles versions de l’interface CLI (et des extensions) risquent de présenter des changements cassants.

Si vous préférez ne plus utiliser la fonctionnalité de mise à jour automatique par exemple pour assurer l’exécution stable des scripts de commandes, vous pouvez la désactiver via la configuration.
```azurecli
az config set auto-upgrade.enable=no
```
