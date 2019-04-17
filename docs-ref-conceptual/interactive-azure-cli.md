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
ms.openlocfilehash: a325b799c7384037ae336093aa5274c7cbf53cbc
ms.sourcegitcommit: cf47338210116437d7dc0f6037d2dabd5c5e6a4b
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/09/2019
ms.locfileid: "59429011"
---
# <a name="azure-cli-interactive-mode"></a><span data-ttu-id="c0753-103">Mode interactif d’Azure CLI</span><span class="sxs-lookup"><span data-stu-id="c0753-103">Azure CLI interactive mode</span></span>

<span data-ttu-id="c0753-104">Vous pouvez utiliser Azure CLI en mode interactif en exécutant la commande `az interactive`.</span><span class="sxs-lookup"><span data-stu-id="c0753-104">You can use Azure CLI in interactive mode by running the `az interactive` command.</span></span>
<span data-ttu-id="c0753-105">Ce mode vous place dans un interpréteur de commandes interactif avec une saisie semi-automatique, des descriptions des commandes ainsi que des exemples.</span><span class="sxs-lookup"><span data-stu-id="c0753-105">This mode places you in an interactive shell with auto-completion, command descriptions, and examples.</span></span>

![mode interactif](./media/interactive-azure-cli/webapp-create.png)

> [!NOTE]
> <span data-ttu-id="c0753-107">Ici, nous n’utilisons pas le style par défaut, qui ne se lit pas aussi bien sur un arrière-plan noir.</span><span class="sxs-lookup"><span data-stu-id="c0753-107">We're not using the default style here, which doesn't read as well on a black background.</span></span>

<span data-ttu-id="c0753-108">Si vous n’êtes pas déjà connecté à votre compte, utilisez la commande `login`.</span><span class="sxs-lookup"><span data-stu-id="c0753-108">If you're not already signed in to your account, use the `login` command.</span></span>

## <a name="configure"></a><span data-ttu-id="c0753-109">Configuration</span><span class="sxs-lookup"><span data-stu-id="c0753-109">Configure</span></span>

<span data-ttu-id="c0753-110">Le mode interactif affiche, si vous le souhaitez, des descriptions des commandes, des descriptions des paramètres et des exemples de commandes.</span><span class="sxs-lookup"><span data-stu-id="c0753-110">Interactive mode optionally displays command descriptions, parameter descriptions, and command examples.</span></span>
<span data-ttu-id="c0753-111">Activez ou désactivez les descriptions et les exemples à l’aide de `F1`.</span><span class="sxs-lookup"><span data-stu-id="c0753-111">Turn descriptions and examples on or off using `F1`.</span></span>

![descriptions et exemples](./media/interactive-azure-cli/descriptions-and-examples.png)

<span data-ttu-id="c0753-113">Vous pouvez activer ou désactiver l’affichage des valeurs par défaut des paramètres à l’aide de `F2`.</span><span class="sxs-lookup"><span data-stu-id="c0753-113">You can turn the display of parameter defaults on or off using `F2`.</span></span>

![valeurs par défaut](./media/interactive-azure-cli/defaults.png)

`F3` <span data-ttu-id="c0753-115">active ou désactive l’affichage de certains mouvements clés.</span><span class="sxs-lookup"><span data-stu-id="c0753-115">toggles the display of some key gestures.</span></span>

![mouvements](./media/interactive-azure-cli/gestures.png)

## <a name="scope"></a><span data-ttu-id="c0753-117">Étendue</span><span class="sxs-lookup"><span data-stu-id="c0753-117">Scope</span></span>

<span data-ttu-id="c0753-118">Vous pouvez étendre votre mode interactif à un groupe de commandes spécifique comme `vm` ou `vm image`.</span><span class="sxs-lookup"><span data-stu-id="c0753-118">You can scope your interactive mode to a specific command group like `vm` or `vm image`.</span></span>
<span data-ttu-id="c0753-119">Dans ce cas, toutes les commandes sont interprétées dans le cadre de cette étendue.</span><span class="sxs-lookup"><span data-stu-id="c0753-119">When you do, all commands are interpreted in that scope.</span></span>
<span data-ttu-id="c0753-120">Il s’agit d’un raccourci pratique si vous effectuez tout votre travail dans ce groupe de commandes.</span><span class="sxs-lookup"><span data-stu-id="c0753-120">It's a great shorthand if you're doing all your work in that command group.</span></span>

<span data-ttu-id="c0753-121">Au lieu de taper les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="c0753-121">Instead of typing these commands:</span></span>

```azurecli
az>> vm create -n myVM -g myRG --image UbuntuLTS
az>> vm list -o table
```

<span data-ttu-id="c0753-122">Vous pouvez définir l’étendue au groupe de commandes de la machine virtuelle et taper les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="c0753-122">You can scope to the vm command group and type these commands:</span></span>

```azurecli
az>> %%vm
az vm>> create -n myVM -g myRG --image UbuntuLTS
az vm>>list -o table
```

<span data-ttu-id="c0753-123">Vous pouvez également définir l’étendue pour des groupes de commandes de niveau inférieur.</span><span class="sxs-lookup"><span data-stu-id="c0753-123">You can scope to lower-level command groups as well.</span></span>
<span data-ttu-id="c0753-124">Vous pouvez définir l’étendue à `vm image` à l’aide de `%%vm image`.</span><span class="sxs-lookup"><span data-stu-id="c0753-124">You could scope to `vm image` using `%%vm image`.</span></span>
<span data-ttu-id="c0753-125">Dans ce cas, étant donné que nous avons déjà défini l’étendue à `vm`, nous utilisons `%%image`.</span><span class="sxs-lookup"><span data-stu-id="c0753-125">In this case, since we're already scoped to `vm`, we would use `%%image`.</span></span>

```azurecli
az vm>> %%image
az vm image>>
```

<span data-ttu-id="c0753-126">À ce stade, nous pouvons redéfinir l’étendue sur `vm` à l’aide de `%%..`, ou nous pouvons étendre à la racine en utilisant simplement `%%`.</span><span class="sxs-lookup"><span data-stu-id="c0753-126">At that point, we can pop the scope back up to `vm` using `%%..`, or we can scope to the root with just `%%`.</span></span>

```azurecli
az vm image>> %%
az>>
```

## <a name="query"></a><span data-ttu-id="c0753-127">Requête</span><span class="sxs-lookup"><span data-stu-id="c0753-127">Query</span></span>

<span data-ttu-id="c0753-128">Vous pouvez exécuter une requête JMESPath sur les résultats de la dernière commande exécutée en utilisant `??` suivi d’une requête JMESPath.</span><span class="sxs-lookup"><span data-stu-id="c0753-128">You can execute a JMESPath query on the results of the last command that you executed by using `??`followed by a JMESPath query.</span></span>
<span data-ttu-id="c0753-129">Par exemple, après avoir créé un groupe, vous pouvez récupérer l’ID du nouveau groupe.</span><span class="sxs-lookup"><span data-stu-id="c0753-129">For example, after you created a group, you can retrieve the id of the new group.</span></span>

```azurecli
az>> group create -n myRG -l westEurope
az>> "?? id"
```

<span data-ttu-id="c0753-130">Cette syntaxe vous permet également d’utiliser le résultat de la commande précédente comme argument dans la commande suivante.\* Par exemple, après avoir listé tous les groupes, vous pouvez lister toutes les ressources de type `virtualMachine` dans le premier groupe dont l’emplacement est westeurope.</span><span class="sxs-lookup"><span data-stu-id="c0753-130">You can also use this syntax to use the result of the previous command as an argument for your next command.\* For instance after having listed all groups, list all the resources of type `virtualMachine`on the first group whose location is westeurope.</span></span> 

```azurecli
az>> vm create --name myVM --resource-group myRG --image UbuntuLTS --no-wait -o json
az>> group list -o json
az>> resource list -g "?? [?location=='westeurope'].name | [0]" --query "[?type=='Microsoft.Compute/virtualMachines'].name
```

<span data-ttu-id="c0753-131">Pour plus d’informations concernant l’interrogation des résultats de vos commandes, consultez [Interroger les résultats d’une commande avec Azure CLI](query-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="c0753-131">To learn more about querying the results of your commands, see [Query command results with the Azure CLI](query-azure-cli.md).</span></span>

## <a name="bash-commands"></a><span data-ttu-id="c0753-132">Commandes Bash</span><span class="sxs-lookup"><span data-stu-id="c0753-132">Bash commands</span></span>

<span data-ttu-id="c0753-133">Vous pouvez exécuter des commandes shell sans quitter le mode interactif à l’aide de `#[cmd]`.</span><span class="sxs-lookup"><span data-stu-id="c0753-133">You can run shell commands without leaving interactive mode using `#[cmd]`.</span></span>

```azurecli
az>> #dir
```

## <a name="examples"></a><span data-ttu-id="c0753-134">Exemples</span><span class="sxs-lookup"><span data-stu-id="c0753-134">Examples</span></span>

<span data-ttu-id="c0753-135">Certaines commandes comportent un grand nombre d’exemples.</span><span class="sxs-lookup"><span data-stu-id="c0753-135">Some commands have lots of examples.</span></span>
<span data-ttu-id="c0753-136">Vous pouvez faire défiler vers la page suivante des exemples à l’aide de `CTRL-N` et vers la page précédente à l’aide de `CTRL-Y`.</span><span class="sxs-lookup"><span data-stu-id="c0753-136">You can scroll to the next page of examples using `CTRL-N` and the previous page using `CTRL-Y`.</span></span>

![exemples](./media/interactive-azure-cli/examples.png)

<span data-ttu-id="c0753-138">Vous pouvez également consulter un exemple spécifique à l’aide de `::#`.</span><span class="sxs-lookup"><span data-stu-id="c0753-138">You can also look at a specific example using `::#`.</span></span>

```azurecli
az>> vm create ::8
```
