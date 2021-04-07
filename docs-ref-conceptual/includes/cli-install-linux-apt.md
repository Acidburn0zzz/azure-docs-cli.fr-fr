---
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 09/29/2020
ms.topic: include
ms.custom: devx-track-azurecli
ms.openlocfilehash: 5f395b922ae4c39932854adf9f10fba14d71e47a
ms.sourcegitcommit: 8bff8b2ce4492ab99ad39390e4c802fb4f4425c8
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/26/2021
ms.locfileid: "105582908"
---
## <a name="overview"></a><span data-ttu-id="2a658-101">Vue d’ensemble</span><span class="sxs-lookup"><span data-stu-id="2a658-101">Overview</span></span>

<span data-ttu-id="2a658-102">Le gestionnaire de package `apt` contient un package x86_64 pour Azure CLI qui a été testé sur les distributions suivantes.</span><span class="sxs-lookup"><span data-stu-id="2a658-102">The `apt` package manager contains an x86_64 package for the Azure CLI that has been tested on the following distributions.</span></span>

| <span data-ttu-id="2a658-103">Distribution</span><span class="sxs-lookup"><span data-stu-id="2a658-103">Distribution</span></span> | <span data-ttu-id="2a658-104">Version</span><span class="sxs-lookup"><span data-stu-id="2a658-104">Version</span></span> |
|:-------------|:--------|
| <span data-ttu-id="2a658-105">Ubuntu</span><span class="sxs-lookup"><span data-stu-id="2a658-105">Ubuntu</span></span>       | <span data-ttu-id="2a658-106">14.04 LTS (Trusty Tahir), 16.04 LTS (Xenial Xerus), 18.04 LTS (Bionic Beaver), 20.04 LTS (Focal Fossa), 20.10 (Groovy Gorilla)</span><span class="sxs-lookup"><span data-stu-id="2a658-106">14.04 LTS (Trusty Tahir), 16.04 LTS (Xenial Xerus), 18.04 LTS (Bionic Beaver), 20.04 LTS (Focal Fossa), 20.10 (Groovy Gorilla)</span></span> |
| <span data-ttu-id="2a658-107">Debian</span><span class="sxs-lookup"><span data-stu-id="2a658-107">Debian</span></span>       | <span data-ttu-id="2a658-108">Debian 8 (Jessie), Debian 9 (Stretch), Debian 10 (Buster)</span><span class="sxs-lookup"><span data-stu-id="2a658-108">Debian 8 (Jessie), Debian 9 (Stretch), Debian 10 (Buster)</span></span> |

> [!WARNING]
> <span data-ttu-id="2a658-109">Ubuntu 20.04 (Focal Fossa) et 20.10 (Groovy Gorilla) incluent un package `azure-cli` avec la version `2.0.81` fourni par le référentiel `universe`.</span><span class="sxs-lookup"><span data-stu-id="2a658-109">Ubuntu 20.04 (Focal Fossa) and 20.10 (Groovy Gorilla) include an `azure-cli` package with version `2.0.81` provided by the `universe` repository.</span></span> <span data-ttu-id="2a658-110">Ce package est obsolète et n’est pas recommandé.</span><span class="sxs-lookup"><span data-stu-id="2a658-110">This package is outdated and not recommended.</span></span> <span data-ttu-id="2a658-111">Si ce package est installé, exécutez la commande `sudo apt remove azure-cli -y && sudo apt autoremove -y` pour le supprimer avant de continuer.</span><span class="sxs-lookup"><span data-stu-id="2a658-111">If this package is installed, remove the package before continuing by running the command `sudo apt remove azure-cli -y && sudo apt autoremove -y`.</span></span>

## <a name="installation-options"></a><span data-ttu-id="2a658-112">Options d'installation</span><span class="sxs-lookup"><span data-stu-id="2a658-112">Installation Options</span></span>

<span data-ttu-id="2a658-113">Pour installer Azure CLI sur votre système, deux options s’offrent à vous.</span><span class="sxs-lookup"><span data-stu-id="2a658-113">There are two options to install the Azure CLI on your system.</span></span>  <span data-ttu-id="2a658-114">Vous pouvez soit exécuter une seule commande qui télécharge un script d’installation et exécute les commandes d’installation pour vous,</span><span class="sxs-lookup"><span data-stu-id="2a658-114">First, you may execute a single command that will download an install script and run the install commands for you.</span></span>  <span data-ttu-id="2a658-115">soit exécuter les commandes d’installation vous-même dans un processus pas à pas.</span><span class="sxs-lookup"><span data-stu-id="2a658-115">Or if you prefer, you can execute the install commands yourself in a step-by-step process.</span></span>  <span data-ttu-id="2a658-116">Les deux méthodes sont présentées ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="2a658-116">Both methods are provided below.</span></span>

## <a name="option-1-install-with-one-command"></a><span data-ttu-id="2a658-117">Option 1 : Installer avec une seule commande</span><span class="sxs-lookup"><span data-stu-id="2a658-117">Option 1: Install with one command</span></span>

<span data-ttu-id="2a658-118">L’équipe d’Azure CLI propose un script qui permet d’exécuter toutes les commandes d’installation en une seule étape.</span><span class="sxs-lookup"><span data-stu-id="2a658-118">The Azure CLI team maintains a script to run all installation commands in one step.</span></span>  <span data-ttu-id="2a658-119">Ce script, à télécharger avec `curl`, est dirigé directement vers `bash` pour installer l’interface CLI.</span><span class="sxs-lookup"><span data-stu-id="2a658-119">This script is downloaded via `curl` and piped directly to `bash` to install the CLI.</span></span>

<span data-ttu-id="2a658-120">Si vous souhaitez inspecter le contenu du script avant de l’exécuter, téléchargez-le avec `curl` et examinez-le dans votre éditeur de texte favori.</span><span class="sxs-lookup"><span data-stu-id="2a658-120">If you wish to inspect the contents of the script yourself before executing, simply download the script first using `curl` and inspect it in your favorite text editor.</span></span>

```bash
curl -sL https://aka.ms/InstallAzureCLIDeb | sudo bash
```

## <a name="option-2-step-by-step-installation-instructions"></a><span data-ttu-id="2a658-121">Option n°2 : Instructions d’installation pas à pas</span><span class="sxs-lookup"><span data-stu-id="2a658-121">Option 2: Step-by-step installation instructions</span></span>

<span data-ttu-id="2a658-122">Si vous préférez suivre un processus d’installation pas à pas, effectuez les étapes suivantes pour installer Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="2a658-122">If you prefer a step-by-step installation process, complete the following steps to install the Azure CLI.</span></span>

1. <span data-ttu-id="2a658-123">Obtenez les packages nécessaires pour le processus d’installation :</span><span class="sxs-lookup"><span data-stu-id="2a658-123">Get packages needed for the install process:</span></span>

    ```bash
    sudo apt-get update
    sudo apt-get install ca-certificates curl apt-transport-https lsb-release gnupg
    ```

2. <span data-ttu-id="2a658-124">Téléchargez et installez la clé de signature Microsoft :</span><span class="sxs-lookup"><span data-stu-id="2a658-124">Download and install the Microsoft signing key:</span></span>

    ```bash
    curl -sL https://packages.microsoft.com/keys/microsoft.asc |
        gpg --dearmor |
        sudo tee /etc/apt/trusted.gpg.d/microsoft.gpg > /dev/null
    ```

3. <div id="set-release"/><span data-ttu-id="2a658-125">Ajoutez le référentiel de logiciels Azure CLI (ignorez cette étape sur les distributions Linux ARM64) :</span><span class="sxs-lookup"><span data-stu-id="2a658-125">Add the Azure CLI software repository (skip this step on ARM64 Linux distributions):</span></span>

    ```bash
    AZ_REPO=$(lsb_release -cs)
    echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" |
        sudo tee /etc/apt/sources.list.d/azure-cli.list
    ```

4. <span data-ttu-id="2a658-126">Mettez à jour les informations concernant le référentiel, puis installez le package `azure-cli` :</span><span class="sxs-lookup"><span data-stu-id="2a658-126">Update repository information and install the `azure-cli` package:</span></span>

    ```bash
    sudo apt-get update
    sudo apt-get install azure-cli
    ```

## <a name="sign-in-to-azure-with-the-azure-cli"></a><span data-ttu-id="2a658-127">Se connecter à Azure avec Azure CLI</span><span class="sxs-lookup"><span data-stu-id="2a658-127">Sign in to Azure with the Azure CLI</span></span>

<span data-ttu-id="2a658-128">Exécutez Azure CLI avec la commande `az`.</span><span class="sxs-lookup"><span data-stu-id="2a658-128">Run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="2a658-129">Pour vous connecter, utilisez la commande [az login](/cli/azure/reference-index#az_login).</span><span class="sxs-lookup"><span data-stu-id="2a658-129">To sign in, use the [az login](/cli/azure/reference-index#az_login) command.</span></span>

[!INCLUDE [interactive-login](interactive-login.md)]

<span data-ttu-id="2a658-130">Pour en savoir plus sur les différentes méthodes d’authentification, consultez [Se connecter avec Azure CLI](../authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="2a658-130">To learn more about different authentication methods, see [Sign in with Azure CLI](../authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="2a658-131">Dépannage</span><span class="sxs-lookup"><span data-stu-id="2a658-131">Troubleshooting</span></span>

<span data-ttu-id="2a658-132">Voici certains problèmes courants lors de l’installation avec `apt`.</span><span class="sxs-lookup"><span data-stu-id="2a658-132">Here are some common problems seen when installing with `apt`.</span></span> <span data-ttu-id="2a658-133">Si vous rencontrez un problème n’étant pas évoqué ici, [signalez un problème sur github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="2a658-133">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="no-module-issue-on-ubuntu-2004-focalwsl"></a><span data-ttu-id="2a658-134">Aucun problème de module sur Ubuntu 20.04 (Focal)/WSL</span><span class="sxs-lookup"><span data-stu-id="2a658-134">No module issue on Ubuntu 20.04 (Focal)/WSL</span></span>

<span data-ttu-id="2a658-135">Si vous avez installé `azure-cli` sur `Focal` sans ajouter le référentiel de logiciels Azure CLI dans l’[étape 3](#set-release) des instructions d’installation manuelle ou si vous utilisez notre [script](#option-1-install-with-one-command), vous pouvez rencontrer des problèmes tels qu’aucun module nommé « decorator » ou « antlr4 », car le package que vous avez installé est le package `azure-cli 2.0.81` obsolète du référentiel `focal/universe`.</span><span class="sxs-lookup"><span data-stu-id="2a658-135">If you installed `azure-cli` on `Focal` without adding the Azure CLI software repository in [step 3](#set-release) of the manual install instructions or using our [script](#option-1-install-with-one-command), you may encounter issues such as no module named 'decorator' or 'antlr4' as the package you installed is the outdated `azure-cli 2.0.81` from the `focal/universe` repository.</span></span> <span data-ttu-id="2a658-136">Commencez par le supprimer en exécutant `sudo apt remove azure-cli -y && sudo apt autoremove -y`, puis suivez les [instructions](#install) ci-dessus pour installer le dernier package `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="2a658-136">Please remove it first by running `sudo apt remove azure-cli -y && sudo apt autoremove -y`, then follow the above [instructions](#install) to install the latest `azure-cli` package.</span></span>

### <a name="lsb_release-does-not-return-the-correct-base-distribution-version"></a><span data-ttu-id="2a658-137">lsb_release ne renvoie pas la bonne version de la distribution de base</span><span class="sxs-lookup"><span data-stu-id="2a658-137">lsb_release does not return the correct base distribution version</span></span>

<span data-ttu-id="2a658-138">Certaines distributions Ubuntu ou Debian dérivées, telles que Linux Mint peuvent ne pas retourner le nom de version correct de `lsb_release`.</span><span class="sxs-lookup"><span data-stu-id="2a658-138">Some Ubuntu- or Debian-derived distributions such as Linux Mint may not return the correct version name from `lsb_release`.</span></span> <span data-ttu-id="2a658-139">Cette valeur est utilisée dans le processus d’installation pour déterminer le package à installer.</span><span class="sxs-lookup"><span data-stu-id="2a658-139">This value is used in the install process to determine the package to install.</span></span> <span data-ttu-id="2a658-140">Si vous connaissez le nom de code de la version Ubuntu ou Debian dont votre distribution est dérivée, vous pouvez définir la valeur `AZ_REPO` manuellement lors de l’[ajout du référentiel](#set-release).</span><span class="sxs-lookup"><span data-stu-id="2a658-140">If you know the code name of the Ubuntu or Debian version your distribution is derived from, you can set the `AZ_REPO` value manually when [adding the repository](#set-release).</span></span> <span data-ttu-id="2a658-141">Dans le cas contraire, recherchez des informations expliquant comment déterminer le nom de code de la distribution de base et définir `AZ_REPO` sur la valeur appropriée.</span><span class="sxs-lookup"><span data-stu-id="2a658-141">Otherwise, look up information for your distribution on how to determine the base distribution code name and set `AZ_REPO` to the correct value.</span></span>

### <a name="no-package-for-your-distribution"></a><span data-ttu-id="2a658-142">Aucun package pour votre distribution</span><span class="sxs-lookup"><span data-stu-id="2a658-142">No package for your distribution</span></span>

<span data-ttu-id="2a658-143">Après la publication d’une distribution, il peut se passer un certain temps avant que le package Azure CLI associé ne soit disponible.</span><span class="sxs-lookup"><span data-stu-id="2a658-143">Sometimes it may be a while after a distribution is released before there's an Azure CLI package available for it.</span></span> <span data-ttu-id="2a658-144">Azure CLI est conçu pour résister à de futures versions de dépendances, et repose sur peu d’entre elles.</span><span class="sxs-lookup"><span data-stu-id="2a658-144">The Azure CLI designed to be resilient with regards to future versions of dependencies and rely on as few of them as possible.</span></span> <span data-ttu-id="2a658-145">Si aucun package n’est disponible pour votre distribution de base, essayez d’utiliser le package d’une distribution antérieure.</span><span class="sxs-lookup"><span data-stu-id="2a658-145">If there's no package available for your base distribution, try a package for an earlier distribution.</span></span>

<span data-ttu-id="2a658-146">Pour cela, définissez la valeur de `AZ_REPO` manuellement lors de l’[ajout du référentiel](#set-release).</span><span class="sxs-lookup"><span data-stu-id="2a658-146">To do this, set the value of `AZ_REPO` manually when [adding the repository](#set-release).</span></span> <span data-ttu-id="2a658-147">Pour les distributions Ubuntu, utilisez le référentiel `bionic`, et `stretch` pour les distributions Debian.</span><span class="sxs-lookup"><span data-stu-id="2a658-147">For Ubuntu distributions use the `bionic` repository, and for Debian distributions use `stretch`.</span></span> <span data-ttu-id="2a658-148">Les distributions publiées avant Ubuntu Trusty et Debian Wheezy ne sont pas prises en charge.</span><span class="sxs-lookup"><span data-stu-id="2a658-148">Distributions released before Ubuntu Trusty and Debian Wheezy are not supported.</span></span>

### <a name="elementary-os-eos-fails-to-install-the-azure-cli"></a><span data-ttu-id="2a658-149">Le système d’exploitation élémentaire (EOS, elementary OS) ne parvient pas à installer Azure CLI</span><span class="sxs-lookup"><span data-stu-id="2a658-149">Elementary OS (EOS) fails to install the Azure CLI</span></span>

<span data-ttu-id="2a658-150">EOS ne parvient pas à installer Azure CLI parce que `lsb_release` retourne `HERA`, qui est le nom de la version EOS.</span><span class="sxs-lookup"><span data-stu-id="2a658-150">EOS fails to install the Azure cli because `lsb_release` returns `HERA`, which is the EOS release name.</span></span>  <span data-ttu-id="2a658-151">La solution consiste à corriger le fichier `/etc/apt/sources.list.d/azure-cli.list` et à remplacer `hera main` par `bionic main`.</span><span class="sxs-lookup"><span data-stu-id="2a658-151">The solution is to fix the file `/etc/apt/sources.list.d/azure-cli.list` and change `hera main` to `bionic main`.</span></span>

<span data-ttu-id="2a658-152">Contenu du fichier d’origine :</span><span class="sxs-lookup"><span data-stu-id="2a658-152">Original file contents:</span></span>

```
deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ hera main
```

<span data-ttu-id="2a658-153">Contenu du fichier modifié</span><span class="sxs-lookup"><span data-stu-id="2a658-153">Modified file contents</span></span>

```
deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ bionic main
```

### <a name="proxy-blocks-connection"></a><span data-ttu-id="2a658-154">Le proxy bloque la connexion</span><span class="sxs-lookup"><span data-stu-id="2a658-154">Proxy blocks connection</span></span>

[!INCLUDE[configure-proxy](configure-proxy.md)]

<span data-ttu-id="2a658-155">Vous pouvez également configurer de manière explicite `apt` pour utiliser ce proxy à tout moment.</span><span class="sxs-lookup"><span data-stu-id="2a658-155">You may also want to explicitly configure `apt` to use this proxy at all times.</span></span> <span data-ttu-id="2a658-156">Vérifiez que les lignes suivantes s’affichent dans un fichier de configuration `apt` dans `/etc/apt/apt.conf.d/`.</span><span class="sxs-lookup"><span data-stu-id="2a658-156">Make sure that the following lines appear in an `apt` configuration file in `/etc/apt/apt.conf.d/`.</span></span> <span data-ttu-id="2a658-157">Nous vous recommandons d’utiliser votre fichier de configuration global existant, un fichier de configuration de proxy existant, `40proxies` ou `99local`. Mais suivez vos besoins d’administration système.</span><span class="sxs-lookup"><span data-stu-id="2a658-157">We recommend using either your existing global configuration file, an existing proxy configuration file, `40proxies`, or `99local`, but follow your system administration requirements.</span></span>

```apt.conf
Acquire {
    http::proxy "http://[username]:[password]@[proxy]:[port]";
    https::proxy "https://[username]:[password]@[proxy]:[port]";
}
```

<span data-ttu-id="2a658-158">Si votre proxy n’utilise pas l’authentification de base, __supprimez__ la partie `[username]:[password]@` de l’URI du proxy.</span><span class="sxs-lookup"><span data-stu-id="2a658-158">If your proxy does not use basic auth, __remove__ the `[username]:[password]@` portion of the proxy URI.</span></span> <span data-ttu-id="2a658-159">Si vous avez besoin de plus d’informations sur la configuration du proxy, consultez la documentation officielle Ubuntu :</span><span class="sxs-lookup"><span data-stu-id="2a658-159">If you require more information for proxy configuration, see the official Ubuntu documentation:</span></span>

* [<span data-ttu-id="2a658-160">apt.conf manpage</span><span class="sxs-lookup"><span data-stu-id="2a658-160">apt.conf manpage</span></span>](http://manpages.ubuntu.com/manpages/bionic/en/man5/apt.conf.5.html)
* [<span data-ttu-id="2a658-161">Ubuntu wiki - apt-get howto</span><span class="sxs-lookup"><span data-stu-id="2a658-161">Ubuntu wiki - apt-get howto</span></span>](https://help.ubuntu.com/community/AptGet/Howto#Setting_up_apt-get_to_use_a_http-proxy)

<span data-ttu-id="2a658-162">Pour obtenir la clé de signature Microsoft et obtenir le package à partir de notre dépôt, votre proxy doit autoriser les connexions HTTPS à l’adresse suivante :</span><span class="sxs-lookup"><span data-stu-id="2a658-162">In order to get the Microsoft signing key and get the package from our repository, your proxy needs to allow HTTPS connections to the following address:</span></span>

* `https://packages.microsoft.com`

[!INCLUDE[troubleshoot-wsl.md](troubleshoot-wsl.md)]

## <a name="update"></a><span data-ttu-id="2a658-163">Update</span><span class="sxs-lookup"><span data-stu-id="2a658-163">Update</span></span>
[!INCLUDE [az-upgrade](az-upgrade.md)]

<span data-ttu-id="2a658-164">Vous pouvez aussi utiliser `apt-get upgrade` pour mettre à jour le package CLI.</span><span class="sxs-lookup"><span data-stu-id="2a658-164">You can also use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> <span data-ttu-id="2a658-165">Cette commande met à niveau tous les packages installés sur votre système n’ayant pas de modification de dépendance.</span><span class="sxs-lookup"><span data-stu-id="2a658-165">This command upgrades all of the installed packages on your system that have not had a dependency change.</span></span>
> <span data-ttu-id="2a658-166">Pour mettre à niveau uniquement l’interface CLI, utilisez `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="2a658-166">To upgrade the CLI only, use `apt-get install`.</span></span>
>
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

## <a name="uninstall"></a><span data-ttu-id="2a658-167">Désinstaller l’interface</span><span class="sxs-lookup"><span data-stu-id="2a658-167">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](uninstall-boilerplate.md)]

1. <span data-ttu-id="2a658-168">Désinstaller avec `apt-get remove` :</span><span class="sxs-lookup"><span data-stu-id="2a658-168">Uninstall with `apt-get remove`:</span></span>

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. <span data-ttu-id="2a658-169">Si vous ne prévoyez pas de réinstaller l’interface CLI, supprimez les informations de référentiel Azure CLI :</span><span class="sxs-lookup"><span data-stu-id="2a658-169">If you don't plan to reinstall the CLI, remove the Azure CLI repository information:</span></span>

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. <span data-ttu-id="2a658-170">Si vous n’utilisez pas d’autres packages de Microsoft, supprimez la clé de signature :</span><span class="sxs-lookup"><span data-stu-id="2a658-170">If you use no other packages from Microsoft, remove the signing key:</span></span>

    ```bash
    sudo rm /etc/apt/trusted.gpg.d/microsoft.gpg
    ```

4. <span data-ttu-id="2a658-171">Supprimer tous les packages inutiles :</span><span class="sxs-lookup"><span data-stu-id="2a658-171">Remove any unneeded packages:</span></span>

   ```bash
   sudo apt autoremove
   ```
