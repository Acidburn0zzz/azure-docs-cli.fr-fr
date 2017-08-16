---
title: Mode interactif Azure CLI 2.0
description: Utilisez Azure CLI 2.0 en mode interactif.
keywords: Azure CLI 2.0, mode interactif
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 04/06/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: 
ms.openlocfilehash: de6a366b84efa5475fd6146ff29c32e32dfe4672
ms.sourcegitcommit: 1791991b82e6ce8ad4a050cab1695e0c93734e08
ms.contentlocale: fr-FR
ms.lasthandoff: 05/12/2017
---
# <a name="interactive-azure-cli-20"></a><span data-ttu-id="17550-104">Azure CLI 2.0 interactive</span><span class="sxs-lookup"><span data-stu-id="17550-104">Interactive Azure CLI 2.0</span></span>

<span data-ttu-id="17550-105">Vous pouvez utiliser Azure CLI 2.0 en mode interactif en exécutant la commande `az interactive`.</span><span class="sxs-lookup"><span data-stu-id="17550-105">You can use Azure CLI 2.0 in interactive mode by running the `az interactive` command.</span></span>
<span data-ttu-id="17550-106">Cette commande vous place dans un shell interactif où vos commandes sont automatiquement renseignées et vous avez accès à des descriptions des commandes et de leurs paramètres, ainsi qu’à des exemples de commandes.</span><span class="sxs-lookup"><span data-stu-id="17550-106">That places you in an interactive shell where your commands are auto-completed and you have access to descriptions of commands and their parameters and command examples.</span></span>

![mode interactif](./media/interactive-azure-cli/webapp-create.png)

> [!NOTE]
> <span data-ttu-id="17550-108">Ici, nous n’utilisons pas le style par défaut, qui ne lit pas aussi bien sur un arrière-plan noir.</span><span class="sxs-lookup"><span data-stu-id="17550-108">We're not using the default style here, which doesn't read as well on a black background.</span></span>

<span data-ttu-id="17550-109">Si vous n'êtes pas déjà connecté à votre compte, utilisez la commande `login` pour ce faire.</span><span class="sxs-lookup"><span data-stu-id="17550-109">If you're not already logged in to your account, use the `login` command to do that.</span></span>

## <a name="configure"></a><span data-ttu-id="17550-110">Configuration</span><span class="sxs-lookup"><span data-stu-id="17550-110">Configure</span></span>

<span data-ttu-id="17550-111">Le mode interactif affiche, si vous le souhaitez, des descriptions des commandes, des descriptions des paramètres et des exemples de commandes.</span><span class="sxs-lookup"><span data-stu-id="17550-111">Interactive mode optionally displays command descriptions, parameter descriptions, and command examples.</span></span>
<span data-ttu-id="17550-112">Vous pouvez activer ou désactiver les descriptions et les exemples à l’aide de `F1`.</span><span class="sxs-lookup"><span data-stu-id="17550-112">You can turn descriptions and examples on or off using `F1`.</span></span>

![descriptions et exemples](./media/interactive-azure-cli/descriptions-and-examples.png)

<span data-ttu-id="17550-114">Vous pouvez activer ou désactiver l’affichage des valeurs par défaut des paramètres à l’aide de `F2`.</span><span class="sxs-lookup"><span data-stu-id="17550-114">You can turn the display of parameter defaults on or off using `F2`.</span></span>

![valeurs par défaut](./media/interactive-azure-cli/defaults.png)

<span data-ttu-id="17550-116">`F3` active ou désactive l’affichage de certains mouvements clés.</span><span class="sxs-lookup"><span data-stu-id="17550-116">`F3` toggles the display of some key gestures.</span></span>

![mouvements](./media/interactive-azure-cli/gestures.png)

## <a name="scope"></a><span data-ttu-id="17550-118">Scope</span><span class="sxs-lookup"><span data-stu-id="17550-118">Scope</span></span>

<span data-ttu-id="17550-119">Vous pouvez étendre votre mode interactif à un groupe de commandes spécifique comme `vm` ou `vm image`.</span><span class="sxs-lookup"><span data-stu-id="17550-119">You can scope your interactive mode to a specific command group like `vm` or `vm image`.</span></span>
<span data-ttu-id="17550-120">Dans ce cas, toutes les commandes sont interprétées dans le cadre de cette étendue.</span><span class="sxs-lookup"><span data-stu-id="17550-120">When you do, all commands are interpreted in that scope.</span></span>
<span data-ttu-id="17550-121">Il s’agit d’un raccourci pratique si vous effectuez tout votre travail dans ce groupe de commandes.</span><span class="sxs-lookup"><span data-stu-id="17550-121">It's a great shorthand if you're doing all your work in that command group.</span></span>

<span data-ttu-id="17550-122">Au lieu de taper les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="17550-122">Instead of typing these commands:</span></span>

```azurecli
az>> vm create -n myVM -g myRG --image UbuntuLTS
az>> vm list -o table
```

<span data-ttu-id="17550-123">Vous pouvez définir l’étendue au groupe de commandes de la machine virtuelle et taper les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="17550-123">You can scope to the vm command group and type these commands:</span></span>

```azurecli
az>> %%vm
az vm>> create -n myVM -g myRG --image UbuntuLTS
az vm>>list -o table
```

<span data-ttu-id="17550-124">Vous pouvez également définir l’étendue pour des groupes de commandes de niveau inférieur.</span><span class="sxs-lookup"><span data-stu-id="17550-124">You can scope to lower-level command groups as well.</span></span>
<span data-ttu-id="17550-125">Vous pouvez définir l’étendue à `vm image` à l’aide de `%%vm image`.</span><span class="sxs-lookup"><span data-stu-id="17550-125">You could scope to `vm image` using `%%vm image`.</span></span>
<span data-ttu-id="17550-126">Dans ce cas, étant donné que nous avons déjà défini l’étendue à `vm`, nous utilisons `%%image`.</span><span class="sxs-lookup"><span data-stu-id="17550-126">In this case, since we're already scoped to `vm`, we would use `%%image`.</span></span>

```azurecli
az vm>> %%image
az vm image>>
```

<span data-ttu-id="17550-127">À ce stade, nous pouvons redéfinir l’étendue sur `vm` à l’aide de `%%..`, ou nous pouvons étendre à la racine en utilisant simplement `%%`.</span><span class="sxs-lookup"><span data-stu-id="17550-127">At that point, we can pop the scope back up to `vm` using `%%..`, or we can scope to the root with just `%%`.</span></span>

```azurecli
az vm image>> %%
az>>
```

## <a name="query"></a><span data-ttu-id="17550-128">Requête</span><span class="sxs-lookup"><span data-stu-id="17550-128">Query</span></span>

<span data-ttu-id="17550-129">Vous pouvez exécuter une requête JMESPath sur les résultats de la dernière commande exécutée.</span><span class="sxs-lookup"><span data-stu-id="17550-129">You can execute a JMESPath query on the results of the last command that you executed.</span></span>
<span data-ttu-id="17550-130">Par exemple, après avoir créé une machine virtuelle, vous pouvez vous assurer qu’elle est entièrement configurée.</span><span class="sxs-lookup"><span data-stu-id="17550-130">For example, after you create a VM, you can make sure it has fully provisioned.</span></span>

```azurecli
az>> vm create --name myVM --resource-group myRG --image UbuntuLTS --no-wait
az>> ? [*].provisioningState
```

```
[
  "Creating"
]
```

<span data-ttu-id="17550-131">Pour plus d’informations sur l’interrogation des résultats de vos commandes, consultez [Interroger les résultats d’une commande avec Azure 2.0](query-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="17550-131">To learn more about querying the results of your commands, see [Query command results with Azure 2.0](query-azure-cli.md).</span></span>

## <a name="bash-commands"></a><span data-ttu-id="17550-132">Commandes Bash</span><span class="sxs-lookup"><span data-stu-id="17550-132">Bash commands</span></span>

<span data-ttu-id="17550-133">Vous pouvez exécuter des commandes shell sans quitter le mode interactif à l’aide de `#[cmd]`.</span><span class="sxs-lookup"><span data-stu-id="17550-133">You can run shell commands without leaving interactive mode using `#[cmd]`.</span></span>

```azurecli
az>> #dir
```

## <a name="examples"></a><span data-ttu-id="17550-134">Exemples</span><span class="sxs-lookup"><span data-stu-id="17550-134">Examples</span></span>

<span data-ttu-id="17550-135">Certaines commandes comportent un grand nombre d’exemples.</span><span class="sxs-lookup"><span data-stu-id="17550-135">Some commands have lots of examples.</span></span>
<span data-ttu-id="17550-136">Vous pouvez faire défiler vers la page suivante des exemples à l’aide de `CTRL-N` et vers la page précédente à l’aide de `CTRL-Y`.</span><span class="sxs-lookup"><span data-stu-id="17550-136">You can scroll to the next page of examples using `CTRL-N` and the previous page using `CTRL-Y`.</span></span>

![exemples](./media/interactive-azure-cli/examples.png)

<span data-ttu-id="17550-138">Vous pouvez également consulter un exemple spécifique à l’aide de `::#`.</span><span class="sxs-lookup"><span data-stu-id="17550-138">You can also look at a specific example using `::#`.</span></span>

```azurecli
az>> vm create ::8
```
