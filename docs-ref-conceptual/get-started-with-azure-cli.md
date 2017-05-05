---
title: "Bien démarrer avec Azure CLI 2.0"
description: "Bien démarrer avec Azure CLI 2.0 sur Linux, Mac ou Windows."
keywords: Azure CLI 2.0, Linux, Mac, Windows, OS X, Ubuntu, Debian, CentOS, RHEL, SUSE, CoreOS, Docker, Windows, Python, PIP
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 02/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: 85c418a8-6177-4833-bb8d-ff4ce2233c1a
ms.openlocfilehash: f5a88012b21e814262436a864b13f053d836cf07
ms.sourcegitcommit: bcf93ad8ed8802072249cd8187cd4420da89b4c6
translationtype: HT
---
# <a name="get-started-with-azure-cli-20"></a>Bien démarrer avec Azure CLI 2.0

Azure CLI 2.0 est la nouvelle expérience de ligne de commande Azure pour la gestion des ressources Azure.
Elle peut être utilisée sur macOS, Linux et Windows. 

Azure CLI 2.0 est optimisé pour la gestion et l’administration des ressources Azure à partir de la ligne de commande, et pour la création de scripts d’automatisation qui opèrent sur Azure Resource Manager.
Cet article vous aide à bien démarrer et explique les concepts de base.

Pour plus d’informations sur la version la plus récente, consultez les [Notes de publication](release-notes-azure-cli.md).

## <a name="install-azure-cli"></a>Installation de l’interface de ligne de commande Azure

La première étape consiste à vérifier que la dernière version d’Azure CLI est installé :

1. [Installez Azure CLI 2.0](install-azure-cli.md) sur votre plateforme.

2. Pour vérifier que l’installation a réussi, exécutez `az --version` à partir de la ligne de commande. 

Vous devez voir le numéro de version d’Azure CLI et d’autres bibliothèques dépendantes installées sur votre ordinateur.  
  
Si une erreur s’affiche, un problème d’installation de l’interface de ligne de commande s’est sans doute produit. Consultez la section « Dépannage de l’installation » de l’article sur [l’installation d’Azure CLI 2.0](install-azure-cli.md#troubleshooting) pour obtenir des instructions, ou publiez un commentaire dans la discussion en bas de cette page pour obtenir de l’aide.

## <a name="log-in-to-azure"></a>Se connecter à Azure

Maintenant qu’Azure CLI 2.0 est installé, l’étape suivante consiste à vous connecter de manière sécurisée à votre compte Azure. Pour cela, utilisez la commande `az login`.

1. Exécutez la commande suivante à partir de la ligne de commande.

   ```azurecli
   az login
   ```
   
   Cette commande génère un code à utiliser lors de l’étape suivante. 

2. Ouvrez la page [https://aka.ms/devicelogin](https://aka.ms/devicelogin) dans un navigateur web et entrez le code.
  
3. À l’invite, connectez-vous à l’aide de vos informations d’identification Azure.

Vous pouvez désormais exécuter des commandes à partir d’Azure CLI 2.0 sur les ressources et les services Azure accessibles à votre compte.

## <a name="create-a-resource-group"></a>Créer un groupe de ressources

Maintenant que tout est configuré, nous allons utiliser Azure CLI pour créer des ressources dans Azure.

Créez d’abord un groupe de ressources.  Les groupes de ressources dans Azure permettent de gérer plusieurs ressources que vous souhaitez regrouper logiquement.  Par exemple, vous pouvez créer un groupe de ressources pour une application ou un projet, et y ajouter une machine virtuelle, une base de données et un service CDN.

Nous allons créer un groupe de ressources nommé « MyResourceGroup » dans la région *westus2* d’Azure.  Pour ce faire, tapez la commande suivante :

```azurecli
az group create -n MyResourceGroup -l westus2 
```

Une fois le groupe de ressources créé, la commande `az group create` génère plusieurs propriétés de la ressource nouvellement créée :

```Output
{
  "id": "/subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/MyResourceGroup",
  "location": "westus2",
  "managedBy": null,
  "name": "MyResourceGroup",
  "properties": {
    "provisioningState": "Succeeded"
  },
  "tags": null
}
```

## <a name="create-a-linux-virtual-machine"></a>Créer une machine virtuelle Linux

Maintenant que nous avons notre groupe de ressources, nous allons y créer une machine virtuelle Linux.

Vous pouvez créer une machine virtuelle Linux à l’aide de l’image UbuntuTLS populaire, avec deux disques de stockage de 10 et 20 Go, à l’aide de la commande suivante :

```azurecli
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS --data-disk-sizes-gb 10 20
```

Quand vous exécutez la commande précédente, Azure CLI 2.0 recherche une paire de clés SSH stockée dans votre répertoire ~/.ssh.  Si aucune paire de clés SSH n’est encore stockée à cet emplacement, vous pouvez demander à Azure CLI d’en créer automatiquement une pour vous en passant le paramètre --generate-ssh-keys :

```azurecli
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS --generate-ssh-keys
```

La commande `az vm create` retourne un résultat une fois la machine virtuelle entièrement créée, accessible et utilisable. La sortie contient plusieurs propriétés de la nouvelle machine virtuelle, notamment son adresse IP publique :

```Output
{
  "fqdns": "",
  "id": "/subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/MyResourceGroup/providers/Microsoft.Compute/virtualMachines/MyLinuxVM",
  "location": "westus2",
  "macAddress": "xx-xx-xx-xx-xx-xx",
  "powerState": "VM running",
  "privateIpAddress": "xx.x.x.x",
  "publicIpAddress": "xx.xxx.xxx.xx",
  "resourceGroup": "MyResourceGroup"
}
```

Vous pouvez maintenant vous connecter à votre nouvelle machine virtuelle Linux à l’aide de **SSH** avec l’adresse IP publique de la machine virtuelle que vous avez créée :

```azurecli
ssh xx.xxx.xxx.xxx
```

```Output
Welcome to Ubuntu 14.04.4 LTS (GNU/Linux 3.19.0-65-generic x86_64)

 * Documentation:  https://help.ubuntu.com/

  System information as of Sun Feb 19 00:32:28 UTC 2017

  System load: 0.31              Memory usage: 3%   Processes:       89
  Usage of /:  39.6% of 1.94GB   Swap usage:   0%   Users logged in: 0

  Graph this data and manage this system at:
    https://landscape.canonical.com/

  Get cloud support with Ubuntu Advantage Cloud Guest:
    http://www.ubuntu.com/business/services/cloud

0 packages can be updated.
0 updates are security updates.



The programs included with the Ubuntu system are free software;
the exact distribution terms for each program are described in the
individual files in /usr/share/doc/*/copyright.

Ubuntu comes with ABSOLUTELY NO WARRANTY, to the extent permitted by
applicable law.

my-login@MyLinuxVM:~$
```

## <a name="create-a-windows-server-virtual-machine"></a>Créer une machine virtuelle Windows Server

Nous allons maintenant créer une machine virtuelle Windows Server 2016 Datacenter à l’aide de la commande `az vm create`, puis l’ajouter au groupe de ressources « MyResourceGroup » que nous avons utilisé pour notre machine virtuelle Linux.  Comme pour l’exemple de machine virtuelle Linux, nous allons attacher deux disques de stockage à l’aide du paramètre `--data-disk-sizes-gb`.

Azure vous demande d’éviter d’utiliser des noms d’utilisateur/mots de passe faciles à deviner. Il existe des règles spécifiques sur les caractères pouvant être utilisés et sur la longueur minimale du nom d’utilisateur et du mot de passe.  

> [!NOTE]
> Vous serez invité à entrer votre nom d’utilisateur et votre mot de passe lors de l’exécution de cette commande.

```azurecli
az vm create -n MyWinVM -g MyResourceGroup --image Win2016Datacenter
```

La commande `az vm create` retourne un résultat une fois la machine virtuelle entièrement créée, accessible et utilisable.

```Output
{
  "fqdns": "",
  "id": "/subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/MyResourceGroup/providers/Microsoft.Compute/virtualMachines/MyWinVM",
  "location": "westus2",
  "macAddress": "xx-xx-xx-xx-xx-xx",
  "powerState": "VM running",
  "privateIpAddress": "xx.x.x.x",
  "publicIpAddress": "xx.xxx.xx.xxx",
  "resourceGroup": "MyResourceGroup"
}
```

Connectez-vous maintenant à la machine virtuelle Windows Server que vous venez de créer à l’aide du Bureau à distance et de l’adresse IP publique de la machine virtuelle (qui est retournée dans la sortie de `az vm create`).  
Si vous êtes sur un système Windows, vous pouvez pour cela exécuter la commande `mstsc` à partir de la ligne de commande :

```azurecli
mstsc /v:xx.xxx.xx.xxx
```

Fournissez la même combinaison de nom d’utilisateur/mot de passe que celle que vous avez utilisée lors de la création de la machine virtuelle pour vous connecter.

## <a name="creating-other-resources-in-azure"></a>Création d’autres ressources dans Azure

Nous avons vu comment créer un groupe de ressources, une machine virtuelle Linux et une machine virtuelle Windows Server. Vous pouvez créer de nombreux autres types de ressources Azure.  

Toutes les nouvelles ressources sont créées à l’aide d’un modèle de nommage `az <resource type name> create` cohérent.  Par exemple, pour créer un équilibreur de charge réseau Azure que nous pourrions ensuite associer avec nos nouvelles machines virtuelles, nous pouvons utiliser la commande create suivante :

```azurecli
az network lb create -n MyLoadBalancer -g MyResourceGroup
```

Nous pourrions aussi créer un réseau privé virtuel (communément appelé « VNet » dans Azure) pour notre infrastructure à l’aide de la commande create suivante :

```azurecli
az network vnet create -n MyVirtualNetwork -g MyResourceGroup --address-prefix 10.0.0.0/16
```

Ce qui rend Azure et Azure CLI si puissants, c’est que nous pouvons les utiliser non seulement pour obtenir une infrastructure cloud, mais également pour créer des services de plateforme gérés.  Les services de plateforme gérés peuvent aussi être combinés avec l’infrastructure pour générer des solutions encore plus puissantes.

Par exemple, vous pouvez utiliser Azure CLI pour créer un service Azure App Service.  Azure App Service est un service de plateforme géré qui offre un excellent moyen d’héberger des applications web sans avoir à se soucier de l’infrastructure.  Après avoir créé le service Azure App Service, vous pouvez créer deux nouvelles applications web Azure dans l’App Service à l’aide des commandes create suivantes :

```azurecli
# Create an Azure AppService that we can host any number of web apps within
az appservice plan create -n MyAppServicePlan -g MyResourceGroup

# Create Two Web Apps within the AppService (note: name param must be a unique DNS entry)
az appservice web create -n MyWebApp43432 -g MyResourceGroup --plan MyAppServicePlan 
az appservice web create -n MyWebApp43433 -g MyResourceGroup --plan MyAppServicePlan 
```

Une fois que vous avez compris les principes fondamentaux du modèle `az <resource type name> create`, il devient facile de créer tout ce que vous voulez. Voici quelques types de ressources Azure populaires et les commandes create Azure CLI correspondantes pour les créer :

```
Resource Type               Azure CLI create command
-------------               ------------------------
Resource Group              az group create
Virtual Machine             az vm create
Virtual Network             az network vnet create
Load Balancer               az network lb create
Managed Disk                az disk create
Storage account             az storage account create
Virtual Machine Scale Set   az vmss create
Azure Container Service     az acs create
Web App                     az appservice web create
SQL Database Server         az sql server create
Document DB                 az documentdb create
```

Consultez la [documentation de référence](/azure/doc-ref-autogen) pour en savoir plus sur les paramètres propres aux ressources supplémentaires que vous pouvez passer à chacune des commandes précédentes et sur les types de ressources que vous pouvez créer. 

## <a name="useful-tip-optimizing-create-operations-using---no-wait"></a>Astuce : Optimisation des opérations de création à l’aide de --no-wait

Par défaut, quand vous créez des ressources à l’aide d’Azure CLI 2.0, la commande `az <resource type name> create` attend que la ressource ait été créée et soit prête à l’emploi.  Par exemple, si vous créez une machine virtuelle, la commande `az vm create`, par défaut, ne retourne qu’une fois la machine virtuelle créée et prête à ce que vous y accédiez par SSH ou RDP.

Nous adoptons cette approche car elle facilite l’écriture des scripts d’automatisation qui contiennent plusieurs étapes avec des dépendances (et qui ont besoin qu’une tâche précédente soit terminée avant de continuer).

Si vous n’avez pas besoin d’attendre lors de la création d’une ressource, vous pouvez utiliser l’option `no-wait` pour démarrer une action de création en arrière-plan. Vous pouvez continuer à utiliser l’interface de ligne de commande pour d’autres commandes.

Par exemple, la commande `az vm create` ci-dessous démarre un déploiement de machine virtuelle, puis retourne beaucoup plus rapidement (et avant que la machine virtuelle ait démarré complètement) :

```azurecli
az vm create -n MyLinuxVM2 -g MyResourceGroup --image UbuntuLTS --no-wait
```

`--no-wait` peut vous aider à optimiser sensiblement les performances de vos scripts d’automatisation.

## <a name="listing-resources-and-formatting-output"></a>Liste des ressources et mise en forme de la sortie

Vous pouvez utiliser la commande `list` dans Azure CLI pour rechercher et lister les ressources en cours d’exécution dans Azure. 

Comme avec la commande create, vous pouvez lister les ressources à l’aide d’Azure CLI 2.0 avec un modèle de nommage `az <resource type name> list` commun et cohérent entre tous les types de ressources.  Différents formats de sortie et options de requête sont disponibles pour filtrer et trier la liste des ressources à votre goût.

Par exemple, `az vm list` affiche la liste de toutes vos machines virtuelles.   

```azurecli
az vm list 
```
Les valeurs retournées sont par défaut au format JSON (affichant uniquement une sortie partielle, par souci de clarté).

```json
[
  {
    "availabilitySet": null,
    "diagnosticsProfile": null,
    "hardwareProfile": {
      "vmSize": "Standard_DS1_v2"
    },
    "id": "/subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/DemoVM010",
    "instanceView": null,
    "licenseType": null,
    "location": "westus2",
    "name": "MyLinuxVM",
    "networkProfile": {
      "networkInterfaces": [
        {
          "id": "/subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/demorg1/providers/Microsoft.Network/networkInterfaces/DemoVM010VMNic",
          "primary": null,
          "resourceGroup": "MyResourceGroup"
        }
      ]
    },
          ...
          ...
          ...   
]
```

Vous pouvez modifier le format de sortie à l’aide de l’option `--output`.  Exécutez la commande `az vm list` pour afficher les machines virtuelles Linux et Windows Server créées précédemment, ainsi que les propriétés les plus courantes d’une machine virtuelle, à l’aide de l’option de format *table* facile à lire :

```azurecli
az vm list --output table
```

```Output
Name       ResourceGroup    Location
---------  ---------------  ----------
MyLinuxVM  MyResourceGroup  westus2
MyWinVM    MyResourceGroup  westus2
```

Vous pouvez utiliser l’option de sortie *tsv* pour obtenir un format textuel de valeurs séparées par des tabulations, sans en-tête.  Ce format est utile quand vous souhaitez diriger la sortie vers un autre outil texte comme grep. 

```azurecli
az vm list --output tsv
```

```
None    None            /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/MyResourceGroup/providers/Microsoft.Compute/virtualMachines/MyLinuxVM        None    None    westus2 MyLinuxVM                   None        Succeeded       MyResourceGroup None                    Microsoft.Compute/virtualMachines       XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
None    None            /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/MyResourceGroup/providers/Microsoft.Compute/virtualMachines/MyWinVM  None    None    westus2 MyWinVM                 None    Succeeded       MyResourceGroup None                    Microsoft.Compute/virtualMachines       XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
```
Consultez l’article sur les [formats de sortie](format-output-azure-cli.md) pour en savoir plus sur les autres méthodes permettant de lister les ressources et de mettre en forme la sortie.

## <a name="querying-resources-and-shaping-outputs"></a>Interrogation de ressources et mise en forme des sorties

Souvent, vous souhaitez pouvoir interroger uniquement les ressources qui remplissent une condition spécifique.  

La commande `list` offre une prise en charge intégrée qui simplifie le filtrage des ressources par nom de groupe de ressources.  Par exemple, vous pouvez passer un paramètre `--ResourceGroup` ou `-g` à une commande `list` pour récupérer uniquement les ressources appartenant à un groupe de ressources spécifique :

```azurecli
az vm list -g MyResouceGroup --output table
```

```Output
Name       ResourceGroup    Location
---------  ---------------  ----------
MyLinuxVM  MyResourceGroup  westus2
MyWinVM    MyResourceGroup  westus2
```

Pour des requêtes encore plus poussées, vous pouvez utiliser le paramètre `--query` pour exécuter une requête JMESPath sur les résultats de *n’importe quelle* commande `az`.  Vous pouvez utiliser des requêtes JMESPath pour filtrer et mettre en forme la sortie de n’importe quel résultat retourné.

Par exemple, exécutez la commande suivante pour rechercher les ressources de machine virtuelle dans tous les groupes de ressources qui contiennent les lettres « My » :

```azurecli
az vm list --output table --query "[?contains(resourceGroup,'MY')]" 
```

```Output
ResourceGroup    ProvisioningState    Name       Location    VmId
---------------  -------------------  ---------  ----------  ------------------------------------
MYRESOURCEGROUP  Succeeded            MyLinuxVM  westus2     XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
MYRESOURCEGROUP  Succeeded            MyWinVM    westus2     XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
```

Ensuite, nous pouvons choisir d’affiner davantage la sortie en exploitant la fonctionnalité de mise en forme des requêtes JMESPath pour générer des valeurs différentes.  Par exemple, la commande suivante récupère le type de disque de système d’exploitation utilisé par la machine virtuelle afin de déterminer s’il s’agit d’un système d’exploitation Linux ou Windows :

```azurecli
az vm list --output table --query "[?contains(resourceGroup,'MY')].{ VMName:name,OSType:storageProfile.osDisk.osType }" 
```

```Output
VMName     OSType
---------  --------
MyLinuxVM  Linux
MyWinVM    Windows
```

La prise en charge de JMESPath dans Azure CLI est puissante.  Pour en savoir plus sur son utilisation, consultez notre article sur les [requêtes](query-azure-cli.md).

## <a name="deleting-resources"></a>Suppression de ressources

Vous pouvez utiliser la commande `delete` dans Azure CLI pour supprimer les ressources dont vous n’avez plus besoin. Vous pouvez utiliser la commande `delete` avec n’importe quelle ressource, comme avec la commande `create`.

```azurecli
az vm delete -n MyLinuxVM -g MyResourceGroup
```

Par défaut, l’interface de ligne de commande vous invite à confirmer la suppression.  Vous pouvez supprimer cette invite pour les scripts automatisés.

```Output
Are you sure you want to perform this operation? (y/n): y
EndTime                           Name                                  StartTime                         Status
--------------------------------  ------------------------------------  --------------------------------  ---------
2017-02-19T02:35:56.678905+00:00  5b74ab80-9b29-4329-b483-52b406583e2f  2017-02-19T02:33:35.372769+00:00  Succeeded
```

Vous pouvez aussi utiliser la commande `delete` pour supprimer de nombreuses ressources à la fois. Par exemple, la commande suivante supprime toutes les ressources du groupe de ressources « MyResourceGroup » que nous avons utilisées pour tous les exemples de ce didacticiel.

```azurecli
az group delete -n MyResourceGroup
```

```Output
Are you sure you want to perform this operation? (y/n): y
```

## <a name="get-samples"></a>Obtenir les exemples

Pour plus d’informations sur les différentes façons d’utiliser Azure CLI, découvrez nos scripts les plus courants pour les [machines virtuelles Linux](/azure/virtual-machines/virtual-machines-linux-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json), les [machines virtuelles Windows](/azure/virtual-machines/virtual-machines-windows-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json), les [applications web](/azure/app-service-web/app-service-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json) et les [bases de données SQL](/azure/sql-database/sql-database-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json).

## <a name="read-the-api-reference-docs"></a>Lire la documentation de référence sur les API

[Informations de référence sur les API](/cli/azure)

## <a name="get-help"></a>Obtenir de l'aide

Azure CLI contient une documentation d’aide intégrée, qui correspond à notre documentation web que vous pouvez exécuter à partir de la ligne de commande :

```azurecli
az [command-group [command]] -h
```

Par exemple, pour afficher les sous-groupes et les commandes disponibles pour les machines virtuelles, exécutez :

```azurecli
az vm -h
```

Pour obtenir de l’aide avec la commande de création de machine virtuelle, exécutez :

```azurecli
az vm create -h
```

## <a name="switch-from-azure-cli-10"></a>Transition à partir d’Azure CLI 1.0

Si vous savez déjà comment utiliser Azure CLI 1.0 (azure.js), vous remarquerez certains emplacements où les commandes ne sont pas identiques.
Parfois, les commandes pour effectuer une tâche sont très différentes.
Pour vous aider à passer d’Azure CLI 1.0 à Azure CLI 2.0, nous avons commencé cette [mise en correspondance des commandes](https://github.com/Azure/azure-cli/blob/master/doc/azure2az_commands.rst).

## <a name="send-us-your-feedback"></a>Envoyez-nous vos commentaires

```azurecli
az feedback
```
