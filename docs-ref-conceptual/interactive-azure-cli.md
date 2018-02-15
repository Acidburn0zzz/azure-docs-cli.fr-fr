---
title: Mode interactif Azure CLI 2.0
description: Utilisez Azure CLI 2.0 en mode interactif.
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 04/06/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 0d32b7a1e754ba28ec1722fe4bf80e5f36b031e2
ms.sourcegitcommit: b93a19222e116d5880bbe64c03507c64e190331e
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/15/2018
---
# <a name="interactive-azure-cli-20"></a>Azure CLI 2.0 interactive

Vous pouvez utiliser Azure CLI 2.0 en mode interactif en exécutant la commande `az interactive`.
Cette commande vous place dans un shell interactif où vos commandes sont automatiquement renseignées et vous avez accès à des descriptions des commandes et de leurs paramètres, ainsi qu’à des exemples de commandes.

![mode interactif](./media/interactive-azure-cli/webapp-create.png)

> [!NOTE]
> Ici, nous n’utilisons pas le style par défaut, qui ne se lit pas aussi bien sur un arrière-plan noir.

Si vous n'êtes pas déjà connecté à votre compte, utilisez la commande `login` pour ce faire.

## <a name="configure"></a>Configuration

Le mode interactif affiche, si vous le souhaitez, des descriptions des commandes, des descriptions des paramètres et des exemples de commandes.
Vous pouvez activer ou désactiver les descriptions et les exemples à l’aide de `F1`.

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
az>> vm create --name myVM --resource-group myRG --image UbuntuLTS --no-wait
az>> ? [*].provisioningState
```

```
[
  "Creating"
]
```

Pour plus d’informations sur l’interrogation des résultats de vos commandes, consultez [Interroger les résultats d’une commande avec Azure 2.0](query-azure-cli.md).

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
