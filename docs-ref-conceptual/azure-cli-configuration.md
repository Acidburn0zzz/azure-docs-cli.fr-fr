---
title: Options de configuration d’Azure CLI
description: Comment configurer Azure CLI
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 06/11/2018
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 09300c2b0da50e326fc3a7651741b71708c89ec8
ms.sourcegitcommit: bf84dfb62e910ea246586481863bb43d09d07795
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/04/2020
ms.locfileid: "87551181"
---
# <a name="azure-cli-configuration"></a>Configuration d’Azure CLI

Azure CLI autorise une configuration utilisateur pour des paramètres tels que la journalisation, la collecte de données et les valeurs d’argument par défaut.
L’interface CLI propose une commande satisfaisante pour la gestion de certains paramètres par défaut, `az configure`. D’autres valeurs peuvent être définies dans un fichier de configuration ou avec des variables d’environnement.

Les valeurs de configuration utilisées par l’interface CLI sont évaluées dans l’ordre suivant. Les éléments situés en haut de la liste sont prioritaires.

1. Paramètres de ligne de commande
2. Variables d'environnement
3. Valeurs du fichier de configuration ou définies avec `az configure`

## <a name="cli-configuration-with-az-configure"></a>Configuration de l’interface CLI avec az configure

La commande [az configure](/cli/azure/reference-index#az-configure) permet de définir les valeurs par défaut de l’interface CLI.
Cette commande accepte un seul argument, `--defaults`, qui est une liste séparée par des espaces de paires `key=value`. Les valeurs fournies sont utilisées par l’interface CLI à la place des arguments requis.

Le tableau suivant contient une liste des clés de configuration disponibles.

| Nom | Description |
|------|-------------|
| group | Groupe de ressources par défaut à utiliser pour toutes les commandes. |
| location | Emplacement par défaut à utiliser pour toutes les commandes. |
| web | Application par défaut à utiliser pour toutes les commandes `az webapp`. |
| vm | Nom de la machine virtuelle par défaut à utiliser pour les commandes `az vm`. |
| vmss | Nom du groupe de machines virtuelles identiques (VMSS) par défaut à utiliser pour les commandes `az vmss`. |
| acr | Nom du Registre du conteneur par défaut à utiliser pour les commandes `az acr`. |

Par exemple, voici comment vous devez définir le groupe de ressources et l’emplacement par défaut pour toutes les commandes.

```azurecli-interactive
az configure --defaults location=westus2 group=MyResourceGroup
```

## <a name="cli-configuration-file"></a>Fichier de configuration de l’interface CLI

Le fichier de configuration de l’interface CLI contient d’autres paramètres utilisés pour gérer le comportement de l’interface CLI. Le fichier de configuration se trouve sous `$AZURE_CONFIG_DIR/config`. La valeur par défaut `AZURE_CONFIG_DIR` est `$HOME/.azure` sur Linux et macOS, et `%USERPROFILE%\.azure` sous Windows.

Les fichiers de configuration sont écrits sous le format de fichier INI. Ce format de fichier est défini par des en-têtes de section, suivis d’une liste d’entrées de clé-valeur.

* Les en-têtes de section sont écrits en tant que `[section-name]`. Les noms de section sont sensibles à la casse.
* Les entrées sont écrites en tant que `key=value`. Les noms de clés ne sont pas sensibles à la casse.
* Les commentaires sont n’importe quelle ligne commençant par un `#` ou `;`. Les commentaires inclus ne sont pas autorisés.

Les valeurs booléennes ne respectent pas la casse et sont représentées par les valeurs suivantes.

* __True__ : 1, yes, true, on
* __False__ : 0, no, false, off

Voici un exemple de fichier de configuration d’interface CLI qui désactive toutes les invites de confirmation et qui configure la journalisation vers le répertoire `/var/log/azure`.

```ini
[core]
disable_confirm_prompt=Yes

[logging]
enable_log_file=yes
log_dir=/var/log/azure
```

Consultez la section suivante pour en savoir plus sur toutes les valeurs de configuration disponibles et leur signification. Pour obtenir des informations détaillées sur le format de fichier INI, consultez la [documentation Python sur INI](https://docs.python.org/3/library/configparser.html#supported-ini-file-structure).

## <a name="cli-configuration-values-and-environment-variables"></a>Valeurs de configuration de l’interface CLI et variables d’environnement

Le tableau suivant contient l’ensemble des noms d’options et de sections pouvant être placés dans un fichier de configuration. Leurs variables d’environnement correspondantes sont configurées en tant que `AZURE_{section}_{name}` dans toutes les extrémités de fin. Par exemple, la valeur par défaut `output` pour `core` est définie dans la variable `AZURE_CORE_OUTPUT`, tandis que la valeur par défaut `storage_account` pour `batchai` est définie dans la variable `AZURE_BATCHAI_STORAGE_ACCOUNT`.

Lorsque vous fournissez une valeur par défaut, cet argument n’est plus nécessaire à aucune commande. C’est la valeur par défaut qui est alors utilisée.

| Section | Nom      | Type | Description|
|---------|-----------|------|------------|
| __core__ | sortie | string | Format de sortie par défaut. Peut être `json`, `jsonc`, `tsv` ou `table`. |
| | disable\_confirm\_prompt | boolean | Active/Désactive les invites de confirmation. |
| | collect\_telemetry | boolean | Autorise Microsoft à recueillir des données anonymes sur l’utilisation de l’interface CLI. Pour obtenir des informations sur la confidentialité, consultez la [licence MIT Azure CLI](https://github.com/Azure/azure-cli/blob/dev/LICENSE). |
| | only\_show\_errors | boolean | Montre uniquement les erreurs pendant l’appel de commande. En d’autres termes, seules les erreurs sont écrites dans `stderr`. Il supprime les avertissements des commandes en préversion, dépréciées et expérimentales. Il est également disponible pour les commandes individuelles avec le paramètre `--only-show-errors`. |
| | no\_color | boolean | Désactive la couleur. Les messages de couleur d’origine ont le préfixe `DEBUG`, `INFO`, `WARNING` et `ERROR`. Cela contourne le problème d’une bibliothèque tierce où la couleur du terminal ne peut pas être restaurée après une redirection de `stdout`. |
| __logging__ | enable\_log\_file | boolean | Active/Désactive la journalisation. |
| | log\_dir | string | Répertoire dans lequel écrire les journaux d’activité. Par défaut, cette valeur est `${AZURE_CONFIG_DIR}/logs`. |
| __storage__ | connection\_string | string | Chaîne de connexion par défaut à utiliser pour les commandes `az storage`. |
| | account | string | Nom de compte par défaut à utiliser pour les commandes `az storage`. |
| | key | string | Clé de compte par défaut à utiliser pour les commandes `az storage`. |
| | sas\_token | string | Jeton SAS par défaut à utiliser pour les commandes `az storage`. |
| __batchai__ | storage\_account | string | Compte de stockage par défaut à utiliser pour les commandes `az batchai`. |
| | storage\_key | string | Clé de stockage par défaut à utiliser pour les commandes `az batchai`. |
| __batch__ | account | string | Nom de compte Azure Batch par défaut à utiliser pour les commandes `az batch`. |
| | access\_key | string | Clé d’accès par défaut à utiliser pour les commandes `az batch`. Uniquement utilisée avec l’autorisation `aad`. |
| | endpoint | string | Point de terminaison par défaut auquel se connecter pour les commandes `az batch`. |
| | auth\_mode | string | Mode d’autorisation à utiliser pour les commandes `az batch`. Peut être `shared_key` ou `aad`. |
| __cloud__ | name | string | Cloud par défaut pour toutes les commandes `az`.  Les valeurs possibles sont `AzureCloud` (valeur par défaut), `AzureChinaCloud`, `AzureUSGovernment`, `AzureGermanCloud`. Pour changer des clouds, vous pouvez utiliser la commande `az cloud set –name`.  Pour obtenir un exemple, consultez [Gérer des clouds avec l’interface Azure CLI](manage-clouds-azure-cli.md). |
| __extension__ | use_dynamic_install | string | Installez une extension si elle n’est pas encore ajoutée lors de l’exécution d’une commande à partir de celle-ci. Les valeurs possibles sont `no` (valeur par défaut), `yes_prompt`, `yes_without_prompt`. |
| | run_after_dynamic_install | boolean | Poursuivez l’exécution de la commande lorsqu’une extension est installée dynamiquement pour celle-ci. La valeur par défaut est `False`. |

> [!NOTE]
> Votre fichier de configuration peut contenir d’autres valeurs. Toutefois, celles-ci sont gérées directement par le biais de commandes de l’interface CLI, notamment `az configure`. Les valeurs répertoriées dans le tableau ci-dessus sont les seules valeurs que vous devez modifier vous-même.
