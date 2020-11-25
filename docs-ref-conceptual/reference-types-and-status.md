---
title: Types de références Azure CLI
description: Explication des types et états de références
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 11/19/2020
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: ff77011db5a64e7c541dc67f2b2564301bfeebfb
ms.sourcegitcommit: 6996f3d05d73f528a95b61fdce1422eee3c7a580
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/25/2020
ms.locfileid: "95870149"
---
# <a name="overview-azure-cli-reference-types-and-status"></a>Présentation : Types et état de référence Azure CLI

L’interface Azure CLI comprend différents types de références qui sont parfois décrits de façon interchangeable avec les états de référence.  Cet article explique la différence entre un type et un état Azure CLI, et fournit des informations sur l’utilisation de chacun d’eux.

## <a name="azure-cli-syntax-components"></a>Composants de la syntaxe d’Azure CLI

La syntaxe d’Azure CLI est une combinaison de références, de commandes et de paramètres.  La **commande de référence complète** est souvent juste appelée **commande**.

| Service Azure | Informations de référence | Sous-service de référence | Commande | Commande de référence complète | Exemples de paramètres
|-|-|-|-|-|-|
| Azure CLI | [az configure](/cli/azure/reference-index#az-configure) | | | az configure | --defaults, --list-default, --scope
| Réseau Azure | [az network](/cli/azure/network) | application-gateway | create | [az network application-gateway create](/cli/azure/network/application-gateway#az-network-application-gateway-create) | --name, --resource-group, --capacity
| Azure DevOps Server | [az pipelines](/cli/azure/pipelines) | agent | list | [az pipelines agent list](/cli/azure/pipelines/agent) | --pool-id, --agent-name, --demands

## <a name="reference-types"></a>Types référence

Un type de référence vous indique si la commande de référence fait partie du service Azure CLI principal ou s’il s’agit d’un complément additionnel.  Il existe deux types de commandes de références Azure CLI : les commandes **principales** et les commandes d’**extension**.

|         | Core  | Extension
|-|-|-|
| **Informations de référence** | Font partie du service Azure CLI principal | Sont des commandes de références facultatives qui doivent être installées
| **Installer** | Conjointement avec le [programme d’installation MSI]() | Individuellement avec [az extension add]()|
| **Publication** | Selon une planification | À mesure que de nouvelles fonctionnalités ou mises à jour sont disponibles
| **État** | Peut être GA (Generally Available), préversion ou expérimental | Peut également être en disponibilité générale, en préversion ou expérimentale

Toutes les références Azure CLI peuvent être exécutées sur Windows, macOS, Linux, Docker et Azure Cloud Shell.

### <a name="core"></a>Core

Les références Azure CLI qui ont été publiées en tant que partie permanente de l’interface CLI sont appelées **références principales**.  Toutes les références principales sont installées avec l’interface Azure CLI et vous ne pouvez pas choisir un sous-ensemble de références.  Si vous exécutez l’interface CLI par le biais d’Azure Cloud Shell, les références principales sont toujours à jour.  Pour obtenir la liste complète des commandes de références principales, consultez la [liste des références principales pour l’interface Azure CLI](/cli/azure/reference-index).

### <a name="extension"></a>Extension

Les extensions ne sont pas fournies dans le cadre de l’interface CLI mais elles sont exécutées en tant que commandes CLI.  Certaines extensions font partie intégrante de l’interface Azure CLI, mais souvent, une extension vous permet d’accéder à la une préversion privée et aux commandes expérimentales.  Une même référence, comme **az iot hub**, peut avoir à la fois des commandes principales et des commandes d’extension.  Voici quatre exemples :

| Commande de référence complète | Est une commande principale | Est une commande d’extension
|-|-|-|
| az iot hub list | Oui |
| az iot hub query | | Oui
| az iot hub certificate create | Oui |
| az iot hub device identify create | | Oui

> [!IMPORTANT]
> Vous devez installer une extension avant de l’utiliser en exécutant la commande [az extension add](/cli/azure/extension#az-extension-add).

Vous pouvez en savoir plus sur les références d’extension, notamment l’installation et la mise à jour dans [Utiliser des extensions avec l’interface Azure CLI](azure-cli-extensions-overview.md).  Passez en revue les [conseils wiki](https://github.com/Azure/azure-network-cli-extension/wiki/Tips) relatifs aux extensions pour optimiser leur utilisation.  Pour obtenir la liste complète des commandes de références d’extension, consultez [Extensions disponibles pour Azure CLI](azure-cli-extensions-list.md).

## <a name="reference-status"></a>États de référence

Quel que soit le type, les références Azure CLI se répartissent en trois catégories d’états : **disponibilité générale** (GA), **préversion publique** ou **expérimental**.  Il s’agit de l’état, et non du type, des commandes de références qui détermine la stabilité et le niveau de support.

| | GA  | Préversion publique | Expérimental
|-|-|-|-|
| **Stabilité** | Permanent | Peut changer en réponse aux commentaires des clients.  Est soumis aux conditions d’utilisation des [préversions de Microsoft Azure](https://azure.microsoft.com/support/legal/preview-supplemental-terms/). | Peut changer en réponse aux commentaires des clients.  Migre souvent vers la préversion publique.  Peut être supprimé.
| **Niveau de support** | Complète | Partial | None

Bien que la plupart des commandes et des paramètres d’une référence unique aient un seul état, cela n’est pas toujours le cas.  Une référence GA qui est conçue pour offrir plus de commandes peut avoir des commandes de références en GA, en préversion et expérimentales. À mesure que de nouveaux paramètres sont ajoutés pour améliorer les fonctionnalités, une même commande peut également avoir des paramètres qui appartiennent à différentes catégories d’état.  Voici des exemples de références qui ont différents états :

| Commande de référence complète | Paramètres | Type | GA | Préversion publique | Expérimental
|-|-|-|-|-|-|
| az network dns zone list | Tous | Core | Oui |
| az network dns zone create | --name, --resource-group, --if-none-match, --parent-name | Core | Oui |
|  | --newFutureParameter1 | Core | | Oui
|  | --newFutureParameter2 | Core | | | Oui
| az network vhub list | Tous |Extension | Oui
| az network vhub create | --address-prefix, --name, --resource-group, -vwan, --location, --sku |Extension | Oui
|  | --newFutureParameter1 |Extension | | Oui
|  | --newFutureParameter2|Extension | | | Oui
| az network firewall create | Tous | Extension | | | Oui

> [!NOTE]
> Les avertissements signalant **préversion publique** ou **expérimental** font partie de la sortie de la commande Azure CLI et il faut s’attendre à les voir.

## <a name="see-also"></a>Voir aussi

- [Liste des références principales pour l’interface Azure CLI](/cli/azure/reference-index)
- [Extensions disponibles pour Azure CLI](azure-cli-extensions-list.md)
