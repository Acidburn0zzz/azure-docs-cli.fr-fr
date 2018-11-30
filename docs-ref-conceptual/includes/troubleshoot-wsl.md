---
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 11/26/2018
ms.topic: include
ms.openlocfilehash: ee0b2b0c8c557aa54255f28429bb3a174c0e21a9
ms.sourcegitcommit: a8aac038e6ede0b1b352ca6163a04b61ff4eed5b
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/28/2018
ms.locfileid: "52450341"
---
### <a name="cli-fails-to-install-or-run-on-windows-subsystem-for-linux"></a>Échec de l’installation ou de l’exécution de l’interface de ligne de commande sur le sous-système Windows pour Linux

Dans la mesure où le [sous-système Windows pour Linux (WSL)](/windows/wsl/about) est une couche de traduction d’appel système, sur la plateforme Windows, il se peut que vous rencontriez une erreur lors de l’installation ou de l’exécution d’Azure CLI. L’interface CLI repose sur certaines fonctionnalités qui peuvent avoir un bogue dans WSL. Si vous rencontrez une erreur, quelle que soit votre méthode d’installation de l’interface CLI, il y a des chances que l’erreur vienne de WSL et non de la méthode d’installation de l’interface CLI.

Pour réussir l’installation de WSL, et potentiellement les problèmes liés :

* Si possible, employez une méthode d’installation identique sur un appareil ou une machine virtuelle Linux pour voir si cela fonctionne. Le cas échéant, votre problème est probablement lié à WSL. Pour démarrer une machine virtuelle Linux dans Azure, consultez la documentation [Créer une machine virtuelle Linux dans le portail Azure](/azure/virtual-machines/linux/quick-create-portal).
* Assurez-vous que vous exécutez la version la plus récente de WSL. Pour obtenir la version la plus récente, [mettez à jour votre installation Windows 10](https://support.microsoft.com/help/4027667/windows-10-update).
* Vérifiez s’il n’y pas déjà des [problèmes ouverts](https://github.com/Microsoft/WSL/issues) pour WSL qui pourraient régler votre problème.
  Vous trouverez le plus souvent des conseils pour contourner le problème, ou des informations relatives à une future version qui règlera le problème.
* S’il n’y a rien au sujet de votre problème, [renseignez un nouveau problème avec WSL](https://github.com/Microsoft/WSL/issues/new) et veillez à inclure le plus d’informations possible.

Si vous rencontrez de nouveau des problèmes d’installation ou d’exécution sur WSL, vous devrez peut-être [installer l’interface CLI pour Windows](../install-azure-cli-windows.md).
