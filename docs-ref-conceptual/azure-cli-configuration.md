---
title: Options de configuration d’Azure CLI
description: Comment configurer Azure CLI 2.0
keywords: Azure CLI, configuration, paramètres, Azure
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/16/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: b0d26beac83a7ce3bba44d5e64d129a211c82836
ms.sourcegitcommit: 8b4629a42ceecf30c1efbc6fdddf512f4dddfab0
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/18/2018
ms.locfileid: "34305874"
---
# <a name="azure-cli-20-configuration"></a>Configuration d’Azure CLI 2.0

Azure CLI 2.0 permet à la configuration utilisateur de remplacer les paramètres internes, comme la journalisation et la collecte de données et de fournir des options par défaut pour certains paramètres requis. L’interface CLI permet de gérer facilement certaines de ces valeurs grâce à la commande `az configure`, et d’autres valeurs peuvent être définies dans un fichier de configuration ou avec des variables d’environnement.

Les valeurs de configuration utilisées par l’interface CLI sont évaluées dans l’ordre suivant. Les éléments situés en haut de la liste sont prioritaires.

1. Paramètres de ligne de commande
2. Variables d’environnement
3. Valeurs du fichier de configuration ou définies avec `az configure`

## <a name="cli-configuration-with-az-configure"></a>Configuration de l’interface CLI avec az configure

La commande [az configure](/cli/azure/reference-index#az-configure) permet de définir les valeurs par défaut de l’interface CLI.
Cette commande accepte un seul argument, `--defaults`, qui est une liste séparée par des espaces de paires `key=value`. Les valeurs fournies sont utilisées par l’interface CLI à la place des arguments requis.

Voici une liste des touches disponibles que vous pouvez utiliser.

| NOM | Description |
|------|-------------|
| group | Groupe de ressources par défaut à utiliser pour toutes les commandes. |
| location | Emplacement par défaut à utiliser pour toutes les commandes. |
| web | Application par défaut à utiliser pour toutes les commandes `az webapp`. |
| vm | Nom de la machine virtuelle par défaut à utiliser pour les commandes `az vm`. |
| vmss | Nom VMSS par défaut à utiliser pour les commandes `az vmss`. |
| acr | Nom du Registre du conteneur par défaut à utiliser pour les commandes `az acr`. |
| acs | Nom du service du conteneur par défaut à utiliser pour les commandes `az acs`. |

Par exemple, voici comment vous devez définir le groupe de ressources et l’emplacement par défaut pour toutes les commandes.

```azurecli-interactive
az configure --defaults location=westus2 group=MyResourceGroup
```

## <a name="cli-configuration-file"></a>Fichier de configuration de l’interface CLI

Le fichier de configuration de l’interface CLI contient d’autres paramètres utilisés pour gérer le comportement de l’interface CLI. Le fichier de configuration se trouve sous `$AZURE_CONFIG_DIR/config`. La valeur par défaut `AZURE_CONFIG_DIR` est `$HOME/.azure` sur Linux et macOS, et `%USERPROFILE%\.azure` sous Windows.

Les fichiers de configuration sont écrits sous le format de fichier INI. Ces fichiers sont composés de sections qui commencent par un en-tête `[section-name]`, suivi d’une liste d’entrées `key=value`. Les noms de section respectent la casse, mais pas les noms de clés.
Les commentaires sont n’importe quelle ligne commençant par un `#` ou `;`. Les commentaires inclus ne sont pas autorisés. Les valeurs booléennes ne respectent pas la casse et sont représentées par les valeurs suivantes.

* __True__ : 1, yes, true, on
* __False__ : 0, no, false, off

Voici un exemple de fichier de configuration d’interface CLI qui désactive les invites de confirmation et définit la journalisation sur le répertoire `/var/log/azure` actif.

```ini
[core]
disable_confirm_prompt=Yes

[logging]
enable_log_file=yes
log_dir=/var/log/azure
```

Consultez la section suivante pour en savoir plus sur toutes les valeurs de configuration disponibles et leur signification. Pour obtenir des informations détaillées sur le format de fichier INI, consultez la [documentation Python sur INI](https://docs.python.org/3/library/configparser.html#supported-ini-file-structure).

## <a name="cli-configuration-values-and-environment-variables"></a>Valeurs de configuration de l’interface CLI et variables d’environnement

Le tableau suivant contient l’ensemble des noms d’options et de sections pouvant être placés dans un fichier de configuration. Les variables d’environnement correspondantes peuvent être définies en tant que `AZURE_{section}_{name}`, tout en majuscules. Par exemple, vous pouvez définir la valeur par défaut `storage_account` de la section `batchai` par défaut dans la variable `AZURE_BATCHAI_STORAGE_ACCOUNT`.

La présence de toute valeur disposant d’une valeur par défaut n’est pas nécessaire dans les arguments de ligne de commande, même si elle est requise.

| Section | NOM      | type | Description|
|---------|-----------|------|------------|
| __core__ | sortie | chaîne | Format de sortie par défaut. Peut être `json`, `jsonc`, `tsv` ou `table`. |
| | disable\_confirm\_prompt | booléenne | Active/Désactive les invites de confirmation. |
| | collect\_telemetry | booléenne | Autorise Microsoft à recueillir des données anonymes sur l’utilisation de l’interface CLI. Pour plus d’informations sur la confidentialité, consultez les [conditions d’utilisation d’Azure CLI 2.0](http://aka.ms/AzureCliLegal). |
| __logging__ | enable\_log\_file | booléenne | Active/Désactive la journalisation. |
| | log\_dir | chaîne | Répertoire dans lequel écrire les journaux. (`${AZURE_CONFIG_DIR}/logs` par défaut). |
| __storage__ | connection\_string | chaîne | Chaîne de connexion par défaut à utiliser pour les commandes `az storage`. |
| | compte | chaîne | Nom de compte par défaut à utiliser pour les commandes `az storage`. |
| | key | chaîne | Clé de compte par défaut à utiliser pour les commandes `az storage`. |
| | sas\_token | chaîne | Jeton SAS par défaut à utiliser pour les commandes `az storage`. |
| __batchai__ | storage\_account | chaîne | Compte de stockage par défaut à utiliser pour les commandes `az batchai`. |
| | storage\_key | chaîne | Clé de stockage par défaut à utiliser pour les commandes `az batchai`. |
| __batch__ | compte | chaîne | Nom de compte Azure Batch par défaut à utiliser pour les commandes `az batch`. |
| | access\_key | chaîne | Clé d’accès par défaut à utiliser pour les commandes `az batch`. Uniquement utilisée avec l’autorisation `aad`. |
| | endpoint | chaîne | Point de terminaison par défaut auquel se connecter pour les commandes `az batch`. |
| | auth\_mode | chaîne | Mode d’autorisation à utiliser pour les commandes `az batch`. Peut être `shared_key` ou `aad`. |

> [!NOTE]
> Votre fichier de configuration peut contenir d’autres valeurs. Toutefois, celles-ci sont gérées directement par le biais de commandes de l’interface CLI, notamment `az configure`. Les valeurs répertoriées dans le tableau ci-dessus sont les seules valeurs que vous devez modifier vous-même.