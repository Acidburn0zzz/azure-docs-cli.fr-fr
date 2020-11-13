---
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/07/2018
ms.topic: include
ms.openlocfilehash: 7aae9e9050306ee834858e528504ae87ff605fa0
ms.sourcegitcommit: 488d53525f1c647ea853d9227d95fdce35b9fb85
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/04/2020
ms.locfileid: "93331064"
---
1. Exécutez la commande `login`.

    ```azurecli-interactive
    az login
    ```

    Si l’interface CLI peut ouvrir votre navigateur par défaut, elle le fait et charge une page de connexion Azure par la même occasion.

    Sinon, ouvrez une page de navigateur à l’adresse [https://aka.ms/devicelogin](https://aka.ms/devicelogin) et entrez le code d’autorisation affiché dans votre terminal.

    Si aucun navigateur web n’est disponible ou si l’ouverture du navigateur web échoue, utilisez le flux de code de l’appareil avec **az login --use-device-code**.

2. Dans le navigateur, connectez-vous avec les informations d’identification de votre compte.
