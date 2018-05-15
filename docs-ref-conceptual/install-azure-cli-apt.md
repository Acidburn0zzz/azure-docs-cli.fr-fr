---
title: Installation d’Azure CLI 2.0 pour Linux avec apt
description: Installation d’Azure CLI 2.0 avec le gestionnaire de package apt
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 02/06/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 7eb04b408f403264f3951bf663d43686601c4ab8
ms.sourcegitcommit: 1d18f667af28b59f5524a3499a4b7dc12af5163d
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/09/2018
---
# <a name="install-azure-cli-20-with-apt"></a><span data-ttu-id="6dcc8-103">Installer Azure CLI 2.0 avec apt</span><span class="sxs-lookup"><span data-stu-id="6dcc8-103">Install Azure CLI 2.0 with apt</span></span>

<span data-ttu-id="6dcc8-104">Si vous exécutez une distribution qui est fournie avec `apt`, telle que Ubuntu ou Debian, un package 64 bits est disponible pour l’interface de ligne de commande Azure.</span><span class="sxs-lookup"><span data-stu-id="6dcc8-104">If you are running a distribution that comes with `apt`, such as Ubuntu or Debian, there is a 64-bit package available for the Azure CLI.</span></span> <span data-ttu-id="6dcc8-105">Ce package a été testé avec :</span><span class="sxs-lookup"><span data-stu-id="6dcc8-105">This package has been tested with:</span></span>

* <span data-ttu-id="6dcc8-106">Ubuntu trusty, xenial, et artful</span><span class="sxs-lookup"><span data-stu-id="6dcc8-106">Ubuntu trusty, xenial, and artful</span></span>
* <span data-ttu-id="6dcc8-107">Debian wheezy, jessie, et stretch</span><span class="sxs-lookup"><span data-stu-id="6dcc8-107">Debian wheezy, jessie, and stretch</span></span>

## <a name="install"></a><span data-ttu-id="6dcc8-108">Installer</span><span class="sxs-lookup"><span data-stu-id="6dcc8-108">Install</span></span>

1. <span data-ttu-id="6dcc8-109">Modifiez votre liste de sources :</span><span class="sxs-lookup"><span data-stu-id="6dcc8-109">Modify your sources list:</span></span>

     ```bash
     AZ_REPO=$(lsb_release -cs)
     echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

2. <span data-ttu-id="6dcc8-110">Obtenir la clé de signature Microsoft :</span><span class="sxs-lookup"><span data-stu-id="6dcc8-110">Get the Microsoft signing key:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
   ```

  > [!WARNING]
  > <span data-ttu-id="6dcc8-111">Cette clé de signature est déconseillée et sera remplacée fin mai 2018.</span><span class="sxs-lookup"><span data-stu-id="6dcc8-111">This signing key is deprecated, and will be replaced at the end of May 2018.</span></span> <span data-ttu-id="6dcc8-112">Afin de continuer à recevoir les mises à jour avec `apt`, veillez à installer également la nouvelle clé :</span><span class="sxs-lookup"><span data-stu-id="6dcc8-112">In order to keep getting updates with `apt`, make sure that you also install the new key:</span></span>
  > 
  > ```bash
  > curl -L https://packages.microsoft.com/keys/microsoft.asc | sudo apt-key add -
  > ``` 

3. <span data-ttu-id="6dcc8-113">Installer l’interface de ligne de commande :</span><span class="sxs-lookup"><span data-stu-id="6dcc8-113">Install the CLI:</span></span>

   ```bash
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

<span data-ttu-id="6dcc8-114">Vous pouvez ensuite exécuter l’interface de ligne de commande Azure avec la commande `az`.</span><span class="sxs-lookup"><span data-stu-id="6dcc8-114">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="6dcc8-115">Pour vous connecter, exécutez la commande `az login`.</span><span class="sxs-lookup"><span data-stu-id="6dcc8-115">To log in, run the `az login` command.</span></span>

```azurecli
az login
```

<span data-ttu-id="6dcc8-116">Pour en savoir plus sur les différentes méthodes de connexion, consultez [Se connecter avec Azure CLI 2.0](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="6dcc8-116">To learn more about different login methods, see [Log in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="6dcc8-117">Résolution de problèmes</span><span class="sxs-lookup"><span data-stu-id="6dcc8-117">Troubleshooting</span></span>

<span data-ttu-id="6dcc8-118">Voici certains problèmes courants lors de l’installation avec `apt`.</span><span class="sxs-lookup"><span data-stu-id="6dcc8-118">Here are some common problems seen when installing with `apt`.</span></span> <span data-ttu-id="6dcc8-119">Si votre problème ne figure pas ici, veuillez [signaler le problème sur Github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="6dcc8-119">If your issue is not listed here, please [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="lsbrelease-fails-with-command-not-found"></a><span data-ttu-id="6dcc8-120">lsb_release échoue avec « Commande introuvable »</span><span class="sxs-lookup"><span data-stu-id="6dcc8-120">lsb_release fails with "Command not found"</span></span>

<span data-ttu-id="6dcc8-121">Lorsque vous exécutez la commande `lsb_release`, vous pouvez voir une sortie similaire à l’erreur suivante :</span><span class="sxs-lookup"><span data-stu-id="6dcc8-121">When running the `lsb_release` command, you may see output similar to the following error:</span></span>

```output
-bash: lsb_release: command not found
```

<span data-ttu-id="6dcc8-122">L’erreur est due au fait que lsb_release n’est pas installé.</span><span class="sxs-lookup"><span data-stu-id="6dcc8-122">The error is due to lsb_release not being installed.</span></span> <span data-ttu-id="6dcc8-123">Vous pouvez résoudre ce problème en installant le package `lsb-release`.</span><span class="sxs-lookup"><span data-stu-id="6dcc8-123">You can resolve it by installing the `lsb-release` package.</span></span>

```bash
sudo apt-get install lsb-release
```

### <a name="apt-key-fails-with-no-dirmngr"></a><span data-ttu-id="6dcc8-124">Clé apt échoue avec le message « No dirmngr »</span><span class="sxs-lookup"><span data-stu-id="6dcc8-124">apt-key fails with "No dirmngr"</span></span>

<span data-ttu-id="6dcc8-125">Lorsque vous exécutez la commande `apt-key`, vous pouvez voir une sortie similaire à l’erreur suivante :</span><span class="sxs-lookup"><span data-stu-id="6dcc8-125">When running the `apt-key` command, you may see output similar to the following error:</span></span>

```output
gpg: failed to start the dirmngr '/usr/bin/dirmngr': No such file or directory
gpg: connecting dirmngr at '/tmp/apt-key-gpghome.kt5zo27tp1/S.dirmngr' failed: No such file or directory
gpg: keyserver receive failed: No dirmngr
```

<span data-ttu-id="6dcc8-126">Cette erreur est due à un composant manquant requis par `apt-key`.</span><span class="sxs-lookup"><span data-stu-id="6dcc8-126">The error is due to a missing component required by `apt-key`.</span></span> <span data-ttu-id="6dcc8-127">Vous pouvez résoudre ce problème en installant le package `dirmngr`.</span><span class="sxs-lookup"><span data-stu-id="6dcc8-127">You can resolve it by installing the `dirmngr` package.</span></span>

```bash
sudo apt-get install dirmngr
```

### <a name="apt-key-hangs"></a><span data-ttu-id="6dcc8-128">apt-key se bloque</span><span class="sxs-lookup"><span data-stu-id="6dcc8-128">apt-key hangs</span></span>

<span data-ttu-id="6dcc8-129">Lorsqu’un pare-feu bloque les connexions sortantes au port 11371, la commande `apt-key` peut se bloquer indéfiniment.</span><span class="sxs-lookup"><span data-stu-id="6dcc8-129">When behind a firewall blocking outgoing connections to port 11371, the `apt-key` command might hang indefinitely.</span></span> <span data-ttu-id="6dcc8-130">Votre pare-feu peut nécessiter l’utilisation d’un proxy HTTP pour les connexions sortantes :</span><span class="sxs-lookup"><span data-stu-id="6dcc8-130">Your firewall may require the use of an HTTP proxy for outgoing connections:</span></span>

```bash
sudo apt-key adv --keyserver-options http-proxy=http://<USER>:<PASSWORD>@<PROXY-HOST>:<PROXY-PORT>/ --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
```

<span data-ttu-id="6dcc8-131">Si vous ne savez pas si vous disposez d’un proxy, contactez votre administrateur système.</span><span class="sxs-lookup"><span data-stu-id="6dcc8-131">If you do not know if you have a proxy, contact your system administrator.</span></span> <span data-ttu-id="6dcc8-132">Si votre proxy ne nécessite pas de connexion, ignorez l’utilisateur, le mot de passe, et le jeton `@`.</span><span class="sxs-lookup"><span data-stu-id="6dcc8-132">If your proxy does not require a login then leave out the user, password, and `@` token.</span></span>

## <a name="update"></a><span data-ttu-id="6dcc8-133">Mettre à jour</span><span class="sxs-lookup"><span data-stu-id="6dcc8-133">Update</span></span>

<span data-ttu-id="6dcc8-134">Utilisez `apt-get upgrade` pour mettre à jour le package de l’interface de ligne de commande.</span><span class="sxs-lookup"><span data-stu-id="6dcc8-134">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> <span data-ttu-id="6dcc8-135">Cette commande met à niveau tous les packages installés sur votre système n’ayant pas de modification de dépendance.</span><span class="sxs-lookup"><span data-stu-id="6dcc8-135">This command upgrades all of the installed packages on your system that have not had a dependency change.</span></span>
> <span data-ttu-id="6dcc8-136">Pour mettre à niveau uniquement l’interface CLI, utilisez `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="6dcc8-136">To upgrade the CLI only, use `apt-get install`.</span></span>
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

## <a name="uninstall"></a><span data-ttu-id="6dcc8-137">Désinstaller l’interface</span><span class="sxs-lookup"><span data-stu-id="6dcc8-137">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="6dcc8-138">Désinstaller avec `apt-get remove`.</span><span class="sxs-lookup"><span data-stu-id="6dcc8-138">Uninstall with `apt-get remove`.</span></span>

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. <span data-ttu-id="6dcc8-139">Si vous ne souhaitez pas réinstaller l’interface de ligne de commande, supprimez les informations de référentiel Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="6dcc8-139">If you do not plan to reinstall the CLI, remove the Azure CLI repository information.</span></span>

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. <span data-ttu-id="6dcc8-140">Supprimez tous les packages inutiles.</span><span class="sxs-lookup"><span data-stu-id="6dcc8-140">Remove any unneeded packages.</span></span>

   ```bash
   sudo apt autoremove
   ```
