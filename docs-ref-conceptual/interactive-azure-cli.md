---
title: Mode interactif d’Azure CLI
description: Utilisez Azure CLI en mode interactif.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 7a6b89953d60fe98910f8141a606ac1fcba318ae
ms.sourcegitcommit: 7f79860c799e78fd8a591d7a5550464080e07aa9
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/12/2019
ms.locfileid: "56158205"
---
# <a name="azure-cli-interactive-mode"></a>Mode interactif d’Azure CLI

Vous pouvez utiliser Azure CLI en mode interactif en exécutant la commande `az interactive`.
Ce mode vous place dans un interpréteur de commandes interactif avec une saisie semi-automatique, des descriptions des commandes ainsi que des exemples.

![mode interactif](./media/interactive-azure-cli/webapp-create.png)

> [!NOTE]
> Ici, nous n’utilisons pas le style par défaut, qui ne se lit pas aussi bien sur un arrière-plan noir.

Si vous n’êtes pas déjà connecté à votre compte, utilisez la commande `login`.

## <a name="configure"></a>Configuration

Le mode interactif affiche, si vous le souhaitez, des descriptions des commandes, des descriptions des paramètres et des exemples de commandes.
Activez ou désactivez les descriptions et les exemples à l’aide de `F1`.

![descriptions et exemples](./media/interactive-azure-cli/descriptions-and-examples.png)

Vous pouvez activer ou désactiver l’affichage des valeurs par défaut des paramètres à l’aide de `F2`.

![valeurs par défaut](./media/interactive-azure-cli/defaults.png)

`F3` active ou désactive l’affichage de certains mouvements clés.

![mouvements](./media/interactive-azure-cli/gestures.png)

## <a name="scope"></a>Étendue

Vous pouvez étendre votre mode interactif à un groupe de commandes spécifique comme `vm` ou `vm image`.
Dans ce cas, toutes les commandes sont interprétées dans le cadre de cette étendue.
Il s’agit d’un raccourci pratique si vous effectuez tout votre travail dans ce groupe de commandes.

Au lieu de taper les commandes suivantes :

```azurecli
az>> vm create -n myVM -g myRG --image UbuntuLTS
az>> vm list -o table
```

Vous pouvez définir l’étendue au groupe de commandes de la machine virtuelle et taper les commandes suivantes :

```azurecli
az>> %%vm
az vm>> create -n myVM -g myRG --image UbuntuLTS
az vm>>list -o table
```

Vous pouvez également définir l’étendue pour des groupes de commandes de niveau inférieur.
Vous pouvez définir l’étendue à `vm image` à l’aide de `%%vm image`.
Dans ce cas, étant donné que nous avons déjà défini l’étendue à `vm`, nous utilisons `%%image`.

```azurecli
az vm>> %%image
az vm image>>
```

À ce stade, nous pouvons redéfinir l’étendue sur `vm` à l’aide de `%%..`, ou nous pouvons étendre à la racine en utilisant simplement `%%`.

```azurecli
az vm image>> %%
az>>
```

## <a name="query"></a>Requête

Vous pouvez exécuter une requête JMESPath sur les résultats de la dernière commande exécutée.
Par exemple, après avoir créé une machine virtuelle, vous pouvez vous assurer qu’elle est entièrement configurée.

```azurecli
az>> vm create --name myVM --resource-group myRG --image UbuntuLTS --no-wait -o json
az>> ? [*].provisioningState
```

```json
[
  "Creating"
]
```

Pour plus d’informations concernant l’interrogation des résultats de vos commandes, consultez [Interroger les résultats d’une commande avec Azure CLI](query-azure-cli.md).

## <a name="bash-commands"></a>Commandes Bash

Vous pouvez exécuter des commandes shell sans quitter le mode interactif à l’aide de `#[cmd]`.

```azurecli
az>> #dir
```

## <a name="examples"></a>Exemples

Certaines commandes comportent un grand nombre d’exemples.
Vous pouvez faire défiler vers la page suivante des exemples à l’aide de `CTRL-N` et vers la page précédente à l’aide de `CTRL-Y`.

![exemples](./media/interactive-azure-cli/examples.png)

Vous pouvez également consulter un exemple spécifique à l’aide de `::#`.

```azurecli
az>> vm create ::8
```
