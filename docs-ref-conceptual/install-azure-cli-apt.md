---
title: "Installation d’Azure CLI 2.0 pour Linux avec apt"
description: "Installation d’Azure CLI 2.0 avec le gestionnaire de package apt"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 02/06/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 188e7dfded21bb5c7036b3a950b3e4cb10bc1d33
ms.sourcegitcommit: 5c004b455eff196d853bfbe12901c6114a1652d7
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/15/2018
---
# <a name="install-azure-cli-20-with-apt"></a><span data-ttu-id="db212-103">Installer Azure CLI 2.0 avec apt</span><span class="sxs-lookup"><span data-stu-id="db212-103">Install Azure CLI 2.0 with apt</span></span>

<span data-ttu-id="db212-104">Si vous exécutez une distribution qui est fournie avec `apt`, telle que Ubuntu ou Debian, un package 64 bits est disponible pour l’interface de ligne de commande Azure.</span><span class="sxs-lookup"><span data-stu-id="db212-104">If you are running a distribution that comes with `apt`, such as Ubuntu or Debian, there is a 64-bit package available for the Azure CLI.</span></span> <span data-ttu-id="db212-105">Ce package a été testé avec :</span><span class="sxs-lookup"><span data-stu-id="db212-105">This package has been tested with:</span></span>

* <span data-ttu-id="db212-106">Ubuntu trusty, xenial, et artful</span><span class="sxs-lookup"><span data-stu-id="db212-106">Ubuntu trusty, xenial, and artful</span></span>
* <span data-ttu-id="db212-107">Debian wheezy, jessie, et stretch</span><span class="sxs-lookup"><span data-stu-id="db212-107">Debian wheezy, jessie, and stretch</span></span>

## <a name="install"></a><span data-ttu-id="db212-108">Installer</span><span class="sxs-lookup"><span data-stu-id="db212-108">Install</span></span>

1. <span data-ttu-id="db212-109">Modifiez votre liste de sources :</span><span class="sxs-lookup"><span data-stu-id="db212-109">Modify your sources list:</span></span>

     ```bash
     AZ_REPO=$(lsb_release -cs)
     echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

2. <span data-ttu-id="db212-110">Exécutez les commandes sudo suivantes :</span><span class="sxs-lookup"><span data-stu-id="db212-110">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

<span data-ttu-id="db212-111">Vous pouvez exécuter l’interface de ligne de commande Azure avec la commande `az`.</span><span class="sxs-lookup"><span data-stu-id="db212-111">You can run the Azure CLI with the `az` command.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="db212-112">Résolution de problèmes</span><span class="sxs-lookup"><span data-stu-id="db212-112">Troubleshooting</span></span>

<span data-ttu-id="db212-113">Voici certains problèmes courants lors de l’installation avec `apt`.</span><span class="sxs-lookup"><span data-stu-id="db212-113">Here are some common problems seen when installing with `apt`.</span></span> <span data-ttu-id="db212-114">Si votre problème ne figure pas ici, veuillez [signaler le problème sur Github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="db212-114">If your issue is not listed here, please [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="apt-key-fails-with-no-dirmngr"></a><span data-ttu-id="db212-115">Clé apt échoue avec le message « No dirmngr »</span><span class="sxs-lookup"><span data-stu-id="db212-115">apt-key fails with "No dirmngr"</span></span>

<span data-ttu-id="db212-116">Lorsque vous exécutez la commande `apt-key`, vous pouvez voir une sortie similaire à l’erreur suivante :</span><span class="sxs-lookup"><span data-stu-id="db212-116">When running the `apt-key` command, you may see output similar to the following error:</span></span>

```output
gpg: failed to start the dirmngr '/usr/bin/dirmngr': No such file or directory
gpg: connecting dirmngr at '/tmp/apt-key-gpghome.kt5zo27tp1/S.dirmngr' failed: No such file or directory
gpg: keyserver receive failed: No dirmngr
```

<span data-ttu-id="db212-117">Cette erreur est due à un composant manquant requis par `apt-key`.</span><span class="sxs-lookup"><span data-stu-id="db212-117">The error is due to a missing component required by `apt-key`.</span></span> <span data-ttu-id="db212-118">Vous pouvez résoudre ce problème en installant le package `dirmngr`.</span><span class="sxs-lookup"><span data-stu-id="db212-118">You can resolve it by installing the `dirmngr` package.</span></span>

```bash
sudo apt-get install dirmngr
```

### <a name="apt-key-hangs"></a><span data-ttu-id="db212-119">apt-key se bloque</span><span class="sxs-lookup"><span data-stu-id="db212-119">apt-key hangs</span></span>

<span data-ttu-id="db212-120">Lorsqu’un pare-feu bloque les connexions sortantes au port 11371, la commande `apt-key` peut se bloquer indéfiniment.</span><span class="sxs-lookup"><span data-stu-id="db212-120">When behind a firewall blocking outgoing connections to port 11371, the `apt-key` command might hang indefinitely.</span></span> <span data-ttu-id="db212-121">Votre pare-feu peut nécessiter l’utilisation d’un proxy HTTP pour les connexions sortantes :</span><span class="sxs-lookup"><span data-stu-id="db212-121">Your firewall may require the use of an HTTP proxy for outgoing connections:</span></span>

```bash
sudo apt-key adv --keyserver-options http-proxy=http://<USER>:<PASSWORD>@<PROXY-HOST>:<PROXY-PORT>/ --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
```

<span data-ttu-id="db212-122">Si vous ne savez pas si vous disposez d’un proxy, contactez votre administrateur système.</span><span class="sxs-lookup"><span data-stu-id="db212-122">If you do not know if you have a proxy, contact your system administrator.</span></span> <span data-ttu-id="db212-123">Si votre proxy ne nécessite pas de connexion, ignorez l’utilisateur, le mot de passe, et le jeton `@`.</span><span class="sxs-lookup"><span data-stu-id="db212-123">If your proxy does not require a login then leave out the user, password, and `@` token.</span></span>

## <a name="update"></a><span data-ttu-id="db212-124">Mettre à jour</span><span class="sxs-lookup"><span data-stu-id="db212-124">Update</span></span>

<span data-ttu-id="db212-125">Utilisez `apt-get upgrade` pour mettre à jour le package de l’interface de ligne de commande.</span><span class="sxs-lookup"><span data-stu-id="db212-125">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> <span data-ttu-id="db212-126">Cette commande met à niveau tous les packages installés sur votre système n’ayant pas de modification de dépendance.</span><span class="sxs-lookup"><span data-stu-id="db212-126">This command upgrades all of the installed packages on your system that have not had a dependency change.</span></span>
> <span data-ttu-id="db212-127">Pour mettre à niveau uniquement l’interface CLI, utilisez `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="db212-127">To upgrade the CLI only, use `apt-get install`.</span></span>
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

## <a name="uninstall"></a><span data-ttu-id="db212-128">Désinstaller l’interface</span><span class="sxs-lookup"><span data-stu-id="db212-128">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="db212-129">Désinstaller avec `apt-get remove`.</span><span class="sxs-lookup"><span data-stu-id="db212-129">Uninstall with `apt-get remove`.</span></span>

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. <span data-ttu-id="db212-130">Si vous ne souhaitez pas réinstaller l’interface de ligne de commande, supprimez les informations de référentiel Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="db212-130">If you do not plan to reinstall the CLI, remove the Azure CLI repository information.</span></span>

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. <span data-ttu-id="db212-131">Supprimez tous les packages inutiles.</span><span class="sxs-lookup"><span data-stu-id="db212-131">Remove any unneeded packages.</span></span>

   ```bash
   sudo apt autoremove
   ```
