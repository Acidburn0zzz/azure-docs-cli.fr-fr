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
1. <span data-ttu-id="b52ee-101">Exécutez la commande `login`.</span><span class="sxs-lookup"><span data-stu-id="b52ee-101">Run the `login` command.</span></span>

    ```azurecli-interactive
    az login
    ```

    <span data-ttu-id="b52ee-102">Si l’interface CLI peut ouvrir votre navigateur par défaut, elle le fait et charge une page de connexion Azure par la même occasion.</span><span class="sxs-lookup"><span data-stu-id="b52ee-102">If the CLI can open your default browser, it will do so and load an Azure sign-in page.</span></span>

    <span data-ttu-id="b52ee-103">Sinon, ouvrez une page de navigateur à l’adresse [https://aka.ms/devicelogin](https://aka.ms/devicelogin) et entrez le code d’autorisation affiché dans votre terminal.</span><span class="sxs-lookup"><span data-stu-id="b52ee-103">Otherwise, open a browser page at [https://aka.ms/devicelogin](https://aka.ms/devicelogin) and enter the  authorization code displayed in your terminal.</span></span>

    <span data-ttu-id="b52ee-104">Si aucun navigateur web n’est disponible ou si l’ouverture du navigateur web échoue, utilisez le flux de code de l’appareil avec **az login --use-device-code**.</span><span class="sxs-lookup"><span data-stu-id="b52ee-104">If no web browser is available or the web browser fails to open, use device code flow with **az login --use-device-code**.</span></span>

2. <span data-ttu-id="b52ee-105">Dans le navigateur, connectez-vous avec les informations d’identification de votre compte.</span><span class="sxs-lookup"><span data-stu-id="b52ee-105">Sign in with your account credentials in the browser.</span></span>
