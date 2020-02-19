---
title: Installation d’Azure CLI pour Linux avec yum
description: Comment installer Azure CLI avec yum
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 11/26/2019
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 53d480c24e624d87ff0cc67ac143c2172344edf4
ms.sourcegitcommit: 91c1e5423bd054a948620999b559bc3a9828a688
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/19/2020
ms.locfileid: "77453722"
---
# <a name="install-azure-cli-with-yum"></a><span data-ttu-id="1ef21-103">Installer Azure CLI avec yum</span><span class="sxs-lookup"><span data-stu-id="1ef21-103">Install Azure CLI with yum</span></span>

<span data-ttu-id="1ef21-104">Pour les distributions Linux avec `yum` telles que RHEL, Fedora ou CentOS, il existe un package pour Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="1ef21-104">For Linux distributions with `yum` such as RHEL, Fedora, or CentOS, there's a package for the Azure CLI.</span></span> <span data-ttu-id="1ef21-105">Ce package a été testé avec RHEL 7.7, RHEL 8, Fedora 24 et versions ultérieures, CentOS 7 et CentOS 8.</span><span class="sxs-lookup"><span data-stu-id="1ef21-105">This package has been tested with RHEL 7.7, RHEL 8, Fedora 24 and higher, CentOS 7 and CentOS 8.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

[!INCLUDE [rpm-warning](includes/rpm-warning.md)]

## <a name="install"></a><span data-ttu-id="1ef21-106">Installer</span><span class="sxs-lookup"><span data-stu-id="1ef21-106">Install</span></span>

1. <span data-ttu-id="1ef21-107">Importez la clé de référentiel Microsoft.</span><span class="sxs-lookup"><span data-stu-id="1ef21-107">Import the Microsoft repository key.</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. <span data-ttu-id="1ef21-108">Créez des informations de référentiel `azure-cli` locales.</span><span class="sxs-lookup"><span data-stu-id="1ef21-108">Create local `azure-cli` repository information.</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]
   name=Azure CLI
   baseurl=https://packages.microsoft.com/yumrepos/azure-cli
   enabled=1
   gpgcheck=1
   gpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/azure-cli.repo'
   ```

3. <span data-ttu-id="1ef21-109">Installez avec la commande `yum install`.</span><span class="sxs-lookup"><span data-stu-id="1ef21-109">Install with the `yum install` command.</span></span>

   ```bash
   sudo yum install azure-cli
   ```

<span data-ttu-id="1ef21-110">Exécutez Azure CLI avec la commande `az`.</span><span class="sxs-lookup"><span data-stu-id="1ef21-110">Run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="1ef21-111">Pour vous connecter, utilisez la commande [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="1ef21-111">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="1ef21-112">Pour en savoir plus sur les différentes méthodes d’authentification, consultez [Se connecter avec Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="1ef21-112">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="1ef21-113">Dépannage</span><span class="sxs-lookup"><span data-stu-id="1ef21-113">Troubleshooting</span></span>

<span data-ttu-id="1ef21-114">Voici certains problèmes courants lors de l’installation avec `yum`.</span><span class="sxs-lookup"><span data-stu-id="1ef21-114">Here are some common problems seen when installing with `yum`.</span></span> <span data-ttu-id="1ef21-115">Si vous rencontrez un problème n’étant pas évoqué ici, [signalez un problème sur github](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="1ef21-115">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="install-on-rhel-76-or-other-systems-without-python-3"></a><span data-ttu-id="1ef21-116">Installer sur RHEL 7.6 ou d’autres systèmes sans Python 3</span><span class="sxs-lookup"><span data-stu-id="1ef21-116">Install on RHEL 7.6 or other systems without Python 3</span></span>

<span data-ttu-id="1ef21-117">Si vous le pouvez, mettez à niveau votre système vers une version avec prise en charge officielle du package `python3`.</span><span class="sxs-lookup"><span data-stu-id="1ef21-117">If you can, please upgrade your system to a verison with official support for `python3` package.</span></span> <span data-ttu-id="1ef21-118">Dans le cas contraire, vous devez d’abord installer un package `python3`, par le biais d’une [génération à partir du source](https://github.com/linux-on-ibm-z/docs/wiki/Building-Python-3.6.x) ou d’une installation par le biais d’un [dépôt supplémentaire](https://developers.redhat.com/blog/2018/08/13/install-python3-rhel/).</span><span class="sxs-lookup"><span data-stu-id="1ef21-118">Otherwise, you need to first install a `python3` package, either [build from source](https://github.com/linux-on-ibm-z/docs/wiki/Building-Python-3.6.x) or install through some [additional repo](https://developers.redhat.com/blog/2018/08/13/install-python3-rhel/).</span></span> <span data-ttu-id="1ef21-119">Vous pouvez alors télécharger le package et l’installer sans dépendance.</span><span class="sxs-lookup"><span data-stu-id="1ef21-119">Then you can download the package and install it without dependency.</span></span>
```bash
$ sudo yum install yum-utils
$ sudo yumdownloader azure-cli
$ sudo rpm -ivh --nodeps azure-cli-*.rpm
```

### <a name="proxy-blocks-connection"></a><span data-ttu-id="1ef21-120">Le proxy bloque la connexion</span><span class="sxs-lookup"><span data-stu-id="1ef21-120">Proxy blocks connection</span></span>

[!INCLUDE[configure-proxy](includes/configure-proxy.md)]

<span data-ttu-id="1ef21-121">Vous pouvez également configurer de manière explicite `yum` pour utiliser ce proxy à tout moment.</span><span class="sxs-lookup"><span data-stu-id="1ef21-121">You may also want to explicitly configure `yum` to use this proxy at all times.</span></span> <span data-ttu-id="1ef21-122">Vérifiez que les lignes suivantes s’affichent sous la section `[main]` de `/etc/yum.conf` :</span><span class="sxs-lookup"><span data-stu-id="1ef21-122">Make sure that the following lines appear under the `[main]` section of `/etc/yum.conf`:</span></span>

```yum.conf
[main]
# ...
proxy=http://[proxy]:[port] # If your proxy requires https, change http->https
proxy_username=[username] # Only required for basic auth
proxy_password=[password] # Only required for basic auth
```

<span data-ttu-id="1ef21-123">Pour obtenir la clé de signature Microsoft et obtenir le package à partir de notre dépôt, votre proxy doit autoriser les connexions HTTPS à l’adresse suivante :</span><span class="sxs-lookup"><span data-stu-id="1ef21-123">In order to get the Microsoft signing key and get the package from our repository, your proxy needs to allow HTTPS connections to the following address:</span></span>

* `https://packages.microsoft.com`

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="update"></a><span data-ttu-id="1ef21-124">Update</span><span class="sxs-lookup"><span data-stu-id="1ef21-124">Update</span></span>

<span data-ttu-id="1ef21-125">Mettre à jour Azure CLI avec la commande `yum update`.</span><span class="sxs-lookup"><span data-stu-id="1ef21-125">Update the Azure CLI with the `yum update` command.</span></span>

```bash
sudo yum update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="1ef21-126">Désinstaller l’interface</span><span class="sxs-lookup"><span data-stu-id="1ef21-126">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="1ef21-127">Supprimez le package de votre système.</span><span class="sxs-lookup"><span data-stu-id="1ef21-127">Remove the package from your system.</span></span>

   ```bash
   sudo yum remove azure-cli
   ```

2. <span data-ttu-id="1ef21-128">Si vous ne prévoyez pas de réinstaller l’interface CLI, supprimez les informations de référentiel.</span><span class="sxs-lookup"><span data-stu-id="1ef21-128">If you don't plan to reinstall the CLI, remove the repository information.</span></span>

   ```bash
   sudo rm /etc/yum.repos.d/azure-cli.repo
   ```

3. <span data-ttu-id="1ef21-129">Si vous n’utilisez pas d’autres packages Microsoft, supprimez la clé de signature.</span><span class="sxs-lookup"><span data-stu-id="1ef21-129">If you don't use any other Microsoft packages, remove the signing key.</span></span>

   ```bash
   MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
   sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
   ```

## <a name="next-steps"></a><span data-ttu-id="1ef21-130">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="1ef21-130">Next Steps</span></span>

<span data-ttu-id="1ef21-131">Maintenant que vous avez installé l’interface CLI, découvrez ses fonctionnalités et ses commandes courantes.</span><span class="sxs-lookup"><span data-stu-id="1ef21-131">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="1ef21-132">Prise en main de l’interface Azure CLI</span><span class="sxs-lookup"><span data-stu-id="1ef21-132">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
