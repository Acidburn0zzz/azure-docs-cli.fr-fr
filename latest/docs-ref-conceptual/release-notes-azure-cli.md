---
title: "Notes de publication d’Azure CLI 2.0"
description: "En savoir plus sur les dernières mises à jour d’Azure CLI 2.0"
keywords: Azure CLI 2.0, notes de publication
author: sptramer
ms.author: sttramer
manager: douge
ms.date: 04/03/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: ce0428f7-0a59-4e72-9237-d907b171af51
ms.openlocfilehash: e893b99349bbf2a5eec8af254158eb07001f1da7
ms.sourcegitcommit: f107cf927ea1ef51de181d87fc4bc078e9288e47
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/04/2017
---
# <a name="azure-cli-20-release-notes"></a>Notes de publication d’Azure CLI 2.0

## <a name="august-28-2017"></a>28 août 2017

Version 2.0.15

### <a name="cli"></a>Interface de ligne de commande

* Ajout d’une remarque juridique pour `--version`.

### <a name="acs"></a>ACS

* Correction des régions d’aperçu.
* Mise en forme par défaut `dns_name_prefix` correctement.
* Sortie de commande des services ACS optimisée.

### <a name="appservice"></a>AppService

* [MODIFICATION CRITIQUE] Fixation des incohérences dans la sortie de `az webapp config appsettings [delete|set]`
* Ajout d’un nouvel alias de `-i` pour `az webapp config container set --docker-custom-image-name`
* Exposé `az webapp log show`
* Exposition de nouveaux arguments à partir de `az webapp delete` pour conserver le plan de service d'application, les métriques ou l’inscription DNS
* Problème résolu : Détecter les paramètres d’emplacement correctement

### <a name="iot"></a>IoT

* Résolu #3934 : La création de la stratégie n’efface plus les stratégies existantes

### <a name="network"></a>Réseau

* [MODIFICATION CRITIQUE] Renommage `vnet list-private-access-services` à `vnet list-endpoint-services`
* [MODIFICATION CRITIQUE] Renommage de l’option `--private-access-services` en `--service-endpoints` pour `vnet subnet [create|update]`
* Ajout de la prise en charge de plusieurs IP et de plusieurs pages de port pour `nsg rule [create|update]`
* Ajout de la prise en charge de la référence (SKU) pour `lb create`
* Ajout de la prise en charge de la référence (SKU) pour `public-ip create`

### <a name="profile"></a>Profil

* exposés `--msi` et `--msi-port` pour vous connecter à l’aide d’une identité de machine virtuelle

### <a name="service-fabric"></a>Service Fabric

* Version préliminaire
* Règles d’utilisateur du Registre/de mot de passe simplifiées pour la commande
* Invite de mot de passe fixe pour l’utilisateur, même après le passage de paramètre
* Ajout de la prise en charge de vide `registry_cred`

### <a name="storage"></a>Storage

* Paramétrage du niveau blob activé
* Ajout des arguments `--bypass` et `--default-action` à `storage account [create|update]` pour la prise en charge du tunneling de service
* Ajout de commandes permettant d’ajouter des règles de réseau virtuel et des règles basées sur IP à `storage account network-rule`  
* Activation du chiffrement du service par la clé gérée du client
* [MODIFICATION CRITIQUE] Renommage de l’option `--encryption` en `--encryption-services` pour `az storage account create and az storage account update` la commande
* Problème résolu #4220 : `az storage account update encryption` - incompatibilité de syntaxe

### <a name="vm"></a>Machine virtuelle

* Correction d’un problème qui entraînait l’affichage d’informations supplémentaires erronées pour `vmss get-instance-view` lors de l’utilisation `--instance-id *`
* Ajout de la prise en charge de `--lb-sku` pour `vmss create`: 
* Suppression des noms humains de la liste rouge du nom de l’administrateur pour `[vm|vmss] create` 
* Correction d’un problème qui entraînait `[vm|vmss] create` la levée d’une erreur si la commande ne parvenait pas à extraire des informations de plan à partir d’une image
* Correction d’un incident qui se produisait lors de la création d’un groupe identique VMMD avec un équilibrage de charge (LB) interne
* Correction d’un problème qui empêchait `--no-wait` le fonctionnement d’un argument avec `vm availability-set create`


## <a name="august-15-2017"></a>15 août 2017

Version 2.0.14

### <a name="acs"></a>ACS

* Correction du numéro de port sshMaster0 pour kubernetes

### <a name="appservice"></a>AppService

* Correction d’une exception qui se produisait lors de la création d’une nouvelle application web Linux basée sur git

### <a name="event-grid"></a>Event Grid

* Ajout de dépendances du kit de développement logiciel (SDK)

## <a name="august-11-2017"></a>11 août 2017

Version 2.0.13

### <a name="acs"></a>ACS

* Ajout de nouvelles régions d’aperçu

### <a name="batch"></a>Batch

* Mise à jour vers Kit de développement logiciel (DSK) de lot 3.1.0 et Kit de développement logiciel (SDK) de gestion de lot 4.1.0
* Ajout d'une nouvelle commande affichant le nombre de tâches d’un travail
* Correction du bogue dans le traitement de l’URL de la signature d'accès partagé du fichier de ressources
* Point de terminaison de compte Batch prend désormais en charge le préfixe « https:// » facultatif
* Prise en charge de l’ajout des listes de plus de 100 tâches à un travail
* Ajout de l’enregistrement de débogage pour le chargement du module de commande Extensions

### <a name="component"></a>Composant

* Ajout d’un avertissement de désapprobation aux commandes « az component »

### <a name="container"></a>Conteneur

* `create` : correction d’un problème qui empêchait l’autorisation de signe égal à l’intérieur d’une variable d’environnement


### <a name="data-lake-store"></a>Data Lake Store

* Contrôle de progression activé

### <a name="event-grid"></a>Event Grid

* Version initiale

### <a name="network"></a>Réseau

* `lb` : correction d’un problème qui empêchait certains noms de ressources enfant d’être résolus correctement lorsqu’ils étaient omis
* `application-gateway {subresource} delete` : correction d’un problème en raison duquel `--no-wait` n’était pas honorée
* `application-gateway http-settings update` : correction d’un problème `--connection-draining-timeout` qui empêchait la désactivation de
* Correction de erreur argument du mot-clé inattendu `sa_data_size_kilobyes` avec`az network vpn-connection ipsec-policy add`

### <a name="profile"></a>Profil

* `account list` : ajout de `--refresh` pour synchroniser les derniers abonnements à partir du serveur

### <a name="storage"></a>Storage

* Activer le compte de stockage de mise à jour avec l’identité attribuée par le système

### <a name="vm"></a>Machine virtuelle

* `availability-set` : nombre de domaines d’erreur exposé sur convert
* Commande `list-skus` exposée
* Prise en charge pour affecter l’identité avec ou sans création d’attributions de rôle
* Appliquer la référence (SKU) de stockage lors de l’attachement de disques de données
* Suppression du nom du disque du système d’exploitation par défaut et de la référence (SKU) de stockage lors de l’utilisation des disques gérés


## <a name="july-28-2017"></a>28 juillet 2017

Version 2.0.12

* Ajout de commandes de conteneur
* Ajout de modules de facturation et de consommation

```
azure-cli (2.0.12)  

acr (2.0.9)  
acs (2.0.11)  
appservice (0.1.11)  
batch (3.0.3)  
billing (0.1.3)  
cdn (0.0.6)  
cloud (2.0.7)  
cognitiveservices (0.1.6)  
command-modules-nspkg (2.0.1)  
component (2.0.6)  
configure (2.0.10)  
consumption (0.1.3)  
container (0.1.7)  
core (2.0.12)  
cosmosdb (0.1.11)  
dla (0.0.10)  
dls (0.0.11)  
feedback (2.0.6)  
find (0.2.6)  
interactive (0.3.7)  
iot (0.1.10)  
keyvault (2.0.8)  
lab (0.0.9)  
monitor (0.0.8)  
network (2.0.11)  
nspkg (3.0.1)  
profile (2.0.9)  
rdbms (0.0.5)  
redis (0.2.7)  
resource (2.0.11)  
role (2.0.9)  
sf (1.0.5)  
sql (2.0.8)  
storage (2.0.11)  
vm (2.0.11) 
```

### <a name="core"></a>Principal

* Informations d’authentification du Kit de développement logiciel (SDK) de sortie pour les principaux de service avec des certificats
* Correction des exceptions de progression de déploiement
* Utiliser le point de terminaison ARM à partir du cloud actuel pour créer le client de l’abonnement
* Amélioration de la gestion simultanée de fichiers clouds.config (#3636)
* Actualiser l’ID de la demande client pour chaque exécution de la commande
* Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel ( SDK) (#3635)
* Rapports de progression pour les déploiements de modèle (#3510)
* Ajout de la prise en charge des champs de sortie de la table de prélèvement via la requête jmespath (#3581)
* Amélioration de la désactivation des arguments d’analyse et de l’historique Ajout avec des mouvements (#3434)
* Créer des clients de l’abonnement avec le bon profil de Kit de développement logiciel (SDK)
* Déplacer tous les fichiers d’enregistrement existant vers le dernier dossier
* Correction de l’idempotence pour VM/VMSS create (#3586)
* Les chemins d’accès de la commande ne sont plus sensibles à la casse
* Certains paramètres de type booléen ne sont plus sensibles à la casse
* Prise en charge de la connexion à ADFS sur le serveur local de manière identique à Azure Stack
* Correction des écritures simultanées dans clouds.config (#3255)

### <a name="acr"></a>ACR

* Ajout de la commande `show-usage` pour les registres gérés
* Prise en charge de la mise à jour de la référence (SKU) pour les registres gérés
* Ajout de registres gérés avec la référence (SKU) gérée
* Ajout de webhooks pour les registres gérés avec le module de commande acr webhook
* Ajout de l’authentification AAD avec la commande de connexion acr
* Ajout de la commande de suppression pour les référentiels docker, les manifestes et les balises

### <a name="acs"></a>ACS

* Prise en charge des API version 2017-07-01

### <a name="appservice"></a>AppService

* Correction d’un bogue à cause duquel l’énumération d’une application Linux ne retournait absolument rien
* Prise en charge de la récupération de références depuis ACR
* Supprimer toutes les commandes sous `appservice web`
* Masquer les mots de passe du registre docker de la commande de sortie (#3656)
* Vérifier que le navigateur par défaut est utilisé sur macOs sans erreurs (#3623)
* Améliorer l’aide de `webapp log tail` et `webapp log download` (#3624)
* Commandes `traffic-routing` exposées pour configurer le routage statique (#3566)
* Ajout de correctifs de fiabilité pour la configuration du contrôle de code source (#3245)
* Suppression d’un argument non pris en charge `--node-version` de `webapp config update` pour les applications Web de Windows. Utilisez à la place `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`

### <a name="batch"></a>Batch

* Mise à jour vers kit de développement logiciel (SDK) de lot 3.0.0 avec prise en charge pour les machines virtuelles de faible priorité dans des pools
* Renommage `pool create` option `--target-dedicated` en `--target-dedicated-nodes`
* Ajout des options `pool create`, `--target-low-priority-nodes` et `--application-licenses`

### <a name="cdn"></a>CDN

* Fourni un meilleur message d’erreur pour `cdn endpoint list` quand le profil spécifié par `--profile-name` n’existe pas.

### <a name="cloud"></a>Cloud

* Modification de la version de l’API du point de terminaison de métadonnées du cloud au format AAAA-MM-JJ
* Le point de terminaison de la galerie n’est pas nécessaire
* Prise en charge de l’inscription du cloud, avec le point de terminaison ARM resource manager
* Ajout d’une option pour `cloud set` permettant de choisir le profil lors de la sélection du cloud actuel
* Exposé `endpoint_vm_image_alias_doc`

### <a name="cosmosdb"></a>CosmosDB

* Correction relative à la permission de la création de collection avec une clé de partition personnalisée
* Ajout de la prise en charge de la durée de vie par défaut de la collection.

### <a name="data-lake-analytics"></a>Data Lake Analytics

* Ajout de commandes pour la gestion de la stratégie de calcul sous le titre `dla account compute-policy`
* Ajout de `dla job pipeline show`
* Ajotu de `dla job recurrence list`

### <a name="data-lake-store"></a>Data Lake Store

* Ajout de la prise en charge pour la rotation de coffre de clés gérés par l’utilisateur dans `dls account update`
* Mise à jour de la version du kit de développement logiciel (SDK) du système de fichiers Data Lake Store sous-jacente, réglant un problème de performance
* Ajout de la commande `dls enable-key-vault`. Cette commande tente d’activer un utilisateur de coffre de clés fourni par l’utilisateur pour utiliser le chiffrement des données dans un compte Data Lake Store

### <a name="interactive"></a>Interactive

* Amélioration du temps de démarrage à l’aide des commandes en cache
* Couverture de test accrue
* Amélioration du mouvement « ? » pour injecter également dans la commande suivante
* Correction d’erreurs interactives avec le profil 2017-03-09-profil-preview (#3587)
* Autorisé `--version` en tant que paramètre pour le mode interactif (#3645)
* Empêche le mode interactif de lever des erreurs à partir des listes de saisie semi-automatique de validation (#3570)
* Rapports de progression pour les déploiements de modèles (#3510)
* Ajout de l’indicateur `--progress`
* Suppression `--debug` et `--verbose` des listes de saisie semi-automatique
* Suppression `interactive` des listes de saisie semi-automatique (#3324)

### <a name="iot"></a>IoT

* La création de la stratégie n’efface plus les stratégies existantes. (#3934)

### <a name="key-vault"></a>Coffre de clés

* Ajout de commandes pour les fonctionnalités de récupération de coffre de clés :
  * `keyvault`sous-commandes `purge`, `recover`,`keyvault list-deleted`
  * `keyvault secret`sous-commandes `backup`, `restore`, `purge`, `recover`,`list-deleted`
  * `keyvault certificate`sous-commandes `purge`, `recover`,`list-deleted`
  * `keyvault key`sous-commandes `purge`, `recover`,`list-deleted`
* Ajout de l’intégration du coffre de clés du principal du service (#3133)
* Mise à jour du plan de données du coffre de clés vers 0.3.2. (#3307)

### <a name="lab"></a>Laboratoire

* Ajout de la prise en charge de la revendication de toutes les machines virtuelles dans le laboratoire via `az lab vm claim`
* Ajout du formateur de sortie de tableau pour `az lab vm list` et `az lab vm show`

### <a name="monitor"></a>Surveiller

* Correctif pour le fichier de modèle avec `monitor autoscale-settings get-parameters-template` commande (#3349)
* Renommage de `monitor alert-rule-incidents list` en `monitor alert list-incidents`
* Renommage de `monitor alert-rule-incidents show` en `monitor alert show-incident`
* Renommage de `monitor metric-defintions list` en `monitor metrics list-definitions`
* Renommage de `monitor alert-rules` en `monitor alert`
* Modifié `monitor alert create`:
  * sous-commandes`condition` et `action` n’acceptent plus JSON
  * Ajout de nombreux paramètres simplifiant le processus de création de règle
  * `location` n’est plus nécessaire
  * Ajout d’un nom et de la prise en charge de l’ID de la cible
  * Suppression de `--alert-rule-resource-name`
  * Le renommage de `is-enabled` en `enabled`n’est plus nécessaire
  * `description` par défaut sont désormais basées sur la condition fournie
  *  Ajout d’exemples aidant à clarifier le nouveau format
* Prise en charge des noms ou des ID pour les commandes `monitor metric`
* Ajout d’arguments d’usage et d’exemples pour `monitor alert rule update`

### <a name="network"></a>Réseau

* Ajout de la commande `list-private-access-services`
* Ajout de l’argument `--private-access-services` à `vnet subnet create` et `vnet subnet update`
* Correction d’un problème `application-gateway redirect-config create` qui causait l’échec de
* Correction d’un problème `application-gateway redirect-config update` qui `--no-wait` empêchait le fonctionnement de
* Correction d’un bogue lié à l’utilisation d’un `--servers` argument avec `application-gateway address-pool create` et `application-gateway address-pool update`
* Ajout des commandes `application-gateway redirect-config`
* Ajout de commandes à `application-gateway ssl-policy` : `list-options`, `predefined list`, `predefined show`
* Ajout d’arguments à `application-gateway ssl-policy set` : `--name`, `--cipher-suites`, `--min-protocol-version`
* Ajout d’arguments à `application-gateway http-settings create` et `application-gateway http-settings update` : `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`
* Ajout d’arguments à `application-gateway url-path-map create` et `application-gateway url-path-map update`, `--default-redirect-config`, `--redirect-config`
* Ajout d’un argument `--redirect-config` à `application-gateway url-path-map rule create`
* Ajout de la prise en charge de `--no-wait` pour `application-gateway url-path-map rule delete`
* Ajout d’arguments à `application-gateway probe create` et `application-gateway probe update` : `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`
* Ajout d’un argument `--redirect-config` à `application-gateway rule create` et `application-gateway rule update`
* Ajout de la prise en charge de `--accelerated-networking` pour `nic create` et `nic update`
* Suppression de l’ `--internal-dns-name-suffix` argument à partir de `nic create`
* Ajout de la prise en charge de `--dns-servers` pour `nic update` et `nic create` : ajout de la prise en charge pour les serveurs DNS :
* Correction d’un bogue qui faisait `local-gateway create` ignorer `--local-address-prefixes`
* Ajout de la prise en charge de `--dns-servers` pour `vnet update`
* Correction d’un bogue lors de la création d’une homologation sans filtrage de l’itinéraire avec `express-route peering create`
* Correction d’un bogue qui empêchait le fonctionnement des arguments `--provider` et `--bandwidth` avec `express-route update`
* Correction d’un bogue avec `network watcher show-topology` une logique de valeurs par défaut
* Amélioration de la mise en forme de sortie pour `network list-usages`
* Utilisation de l’IP frontale par défaut pour `application-gateway http-listener create` s’il n’en existe qu’une seule
* Utilisation d’un pool d’adresses par défaut, des paramètres HTTP et de l’écouteur HTTP pour `application-gateway rule create` s’il n’en existe qu’une seule
* Utilisation de l’IP frontale par défaut et du pool principal `lb rule create` s’il n’en existe qu’une seule
* Utilisation de l’IP frontale par défaut pour `lb inbound-nat-rule create` s’il n’en existe qu’une seule

### <a name="profile"></a>Profil

* Prise en charge de la connexion à l’intérieur d’une machine virtuelle avec une identité gérée
* Prise en charge de la sortie pour `account show` au format de fichier d’authentification du Kit de développement logiciel (SDK)
* Affichage des avertissements de désapprobation lors de l’utilisation de '--expanded-view'
* Ajout de la commande `get-access-token` permettant de fournir un jeton AAD brut
* Prise en charge de la connexion avec un compte d’utilisateur sans abonnements associés

### <a name="rdbms"></a>SGBDR

* Prise en charge de l’énumération de serveurs à travers un abonnement (#3417)
* Correction de `%s` non traité car il manque `% server_type` (#3393)
* Correction du mappage de la source du document et ajout de la tâche CI permettant la vérification de (#3361)
* Correction concernant l’aide relative à MySQL et PostgreSQL (#3369)

### <a name="resource"></a>Ressource

* Amélioration des invites pour les paramètres manquants de `group deployment create`
* Amélioration de l’analyse de `--parameters KEY=VALUE` syntaxe
* Correction des problèmes à cause desquels `group deployment create` les fichiers de paramètres n’étaient plus reconnus à l’aide de la `@<file>` syntaxe
* Prise en charge de l’ `--ids` argument pour `resource` et `managedapp` les commandes
* Correction de certains messages d’analyse et d’erreur (#3584)
* Correction de l’analyse `--resource-type` permettant à la `lock` commande d’accepter `<resource-namespace>` et `<resource-type>`
* Ajout de la vérification de paramètre des modèles de liaison de modèle (#3629)
* Ajout de la prise en charge de la spécification des paramètres de déploiement à l’aide de la `KEY=VALUE` syntaxe

### <a name="role"></a>Rôle

* Prise en charge de la sortie au format de fichier d’authentification du Kit de développement logiciel (SDK) pour `create-for-rbac`
* Nettoyage des attributions de rôles et de l’application AAD liée lors de la suppression d’un principal de service (#3610)
* Inclusion du format d’heure dans `app create` args `--start-date` et `--end-date` descriptions
* Affichage des avertissements de désapprobation lors de l’utilisation de `--expanded-view`
* Ajout de l’intégration du coffre de clés pour les commandes `create-for-rbac` et `reset-credentials`

### <a name="service-fabric"></a>Service Fabric
* Correction d’un problème avec les fichiers volumineux dans les applications tronquées sur le chargement (#3666)
* Ajout de tests pour les commandes Service Fabric (#3424)
* Correction de nombreuses commandes Service Fabric (#3234)

### <a name="sql"></a>SQL

* Suppression du paramètre rompu `sql server create` `--identity`
* Suppression des valeurs de mot de passe à partir de la sortie de commande `sql server create` et `sql server update`
* Ajout des commandes `sql db list-editions` et `sql elastic-pool list-editions`

### <a name="storage"></a>Storage

* Suppression d’une `--marker` option à partir des commandes `storage blob list`, `storage container list`et `storage share list` (#3745)
* Activation de la création d’un compte de stockage https-only
* Mise à jour des métriques de stockage, de la journalisation et des commandes cors (#3495)
* Reformulation d’un message d’exception de l’ajout CORS (#3638) (#3362)  
* Conversion du générateur à une liste en mode exécution d’essai de la commande de téléchargement de lot (#3592) 
* Correction du problème d’essai associé au lot de téléchargement du blob (#3640) (#3592)

### <a name="vm"></a>Machine virtuelle

* Prise en charge de la configuration du groupe de sécurité réseau
* Correction d’un bogue qui entraînait une configuration incorrecte du serveur DNS
* Prise en charge des identités de service géré
* Correction d’un problème à cause duquel `cmss create` avec un équilibreur de charge existant exigeait `--backend-pool-name`.
* Les disques de données créés avec le numéro d’unité logique `vm image create` commencent à 0


## <a name="may-10-2017"></a>10 mai 2017

Version 2.0.6

* documentdb renommé en cosmosdb
* Ajouter rdbms (mysql, postgres)
* Inclure les modules Data Lake Analytics et Data Lake Store.
* Inclure le module Cognitive Services.
* Inclure le module Service Fabric.
* Inclure le module Interactive (az-shell renommé).
* Ajouter la prise en charge des commandes CDN.
* Supprimer le module Container.
* Ajouter « az -v » comme raccourci pour « az --version » ([#2926](https://github.com/Azure/azure-cli/issues/2926))
* Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))

```
azure-cli (2.0.6)

acr (2.0.4)
acs (2.0.6)
appservice (0.1.6)
batch (2.0.4)
cdn (0.0.2)
cloud (2.0.2)
cognitiveservices (0.1.2)
command-modules-nspkg (2.0.0)
component (2.0.4)
configure (2.0.6)
core (2.0.6)
cosmosdb (0.1.6)
dla (0.0.6)
dls (0.0.6)
feedback (2.0.2)
find (0.2.2)
interactive (0.3.1)
iot (0.1.5)
keyvault (2.0.4)
lab (0.0.4)
monitor (0.0.4)
network (2.0.6)
nspkg (3.0.0)
profile (2.0.4)
rdbms (0.0.1)
redis (0.2.3)
resource (2.0.6)
role (2.0.4)
sf (1.0.1)
sql (2.0.3)
storage (2.0.6)
vm (2.0.6)
```

### <a name="core"></a>Principal

* principal : capturer les exceptions provoquées par un fournisseur non enregistré et l’enregistrer automatiquement   
* performance : conserver le cache de jeton adal en mémoire jusqu’à la fin du processus ([#2603](https://github.com/Azure/azure-cli/issues/2603))
* Corriger les octets retournés par l’empreinte digitale hex -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))
* Téléchargement du certificat Key Vault et intégration AAD SP améliorés ([#3003](https://github.com/Azure/azure-cli/issues/3003))
* Ajouter l’emplacement de Python à « az —version » ([#2986](https://github.com/Azure/azure-cli/issues/2986))
* connexion : prise en charge de la connexion lorsqu’il n’y a aucun abonnement ([#2929](https://github.com/Azure/azure-cli/issues/2929))
* principal : corriger une erreur lors de la connexion à l’aide d’un principal de service deux fois ([#2800](https://github.com/Azure/azure-cli/issues/2800))
* principal : autoriser la configuration du chemin d’accès de accessTokens.json via une variable d’environnement ([#2605](https://github.com/Azure/azure-cli/issues/2605))
* principal : autoriser l’application des valeurs par défaut configurées sur les arguments facultatifs ([#2703](https://github.com/Azure/azure-cli/issues/2703))
* principal : performances améliorées
* principal : certificats d’autorité de certification personnalisés - prise en charge de la définition de la variable d’environnement REQUESTS_CA_BUNDLE
* principal : configuration du cloud - utiliser le point de terminaison « resource manager » si le point de terminaison « management » n’est pas défini

### <a name="acs"></a>ACS

* corriger le nombre de maîtres et d’agents sur un nombre entier au lieu d’une chaîne
* exposer « az acs create --no-wait » et « az acs wait » pour la création asynchrone
* exposer « az acs create --validate » pour les validations de test
* supprimer le profil Windows avant l’appel PUT pour la commande de mise à l’échelle ([#2755](https://github.com/Azure/azure-cli/issues/2755))

### <a name="appservice"></a>AppService

* functionapp : ajouter la prise en charge complète de functionapp, notamment créer, afficher, liste, supprimer, nom d’hôte, ssl, etc.
* Ajout de Team Services (vsts) comme option de livraison continue à « config contrôle source web appservice »
* Créer « az webapp » pour remplacer « az appservice web » (pour la rétrocompatibilité, « az appservice web » sera conservé dans les 2 prochaines versions)
* Exposer des arguments pour configurer le déploiement et des « piles d’exécution » sur webapp create
* Exposer « webapp list-runtimes »
* prendre en charge la configuration des chaînes de connexion ([#2647](https://github.com/Azure/azure-cli/issues/2647))
* prendre en charge le basculement d’emplacement avec aperçu
* Supprimer les erreurs des commandes appservice ([#2948](https://github.com/Azure/azure-cli/issues/2948))
* Utiliser le groupe de ressources du plan app service pour les opérations de certificat ([#2750](https://github.com/Azure/azure-cli/issues/2750))

### <a name="cosmosdb"></a>CosmosDB

* Renommer le module documentdb en cosmosdb.
* Prise en charge ajoutée pour les API de plan de données documentdb : gestion de base de données et de collecte
* Prise en charge ajoutée pour activer le basculement automatique sur les comptes de base de données
* Prise en charge ajoutée pour la nouvelle stratégie de cohérence ConsistentPrefix

### <a name="data-lake-analytics"></a>Data Lake Analytics

* Corriger un bogue dans lequel le filtrage sur le résultat et l’état des listes de travaux lève une erreur.
* Ajouter la prise en charge d’un nouveau type d’élément de catalogue : paquet. accessible via : `az dla catalog package`
* A rendu possible le fait de répertorier les éléments de catalogue suivants à partir d’une base de données (aucune spécification de schéma requise) :

  * Table
  * Fonction table
  * Affichage
  * Statistiques de table. Cela peut également être répertorié avec un schéma, mais sans spécifier un nom de table.

### <a name="data-lake-store"></a>Data Lake Store

* Mettre à jour la version du Kit de développement logiciel (SDK) du système de fichiers sous-jacent, qui offre une meilleure prise en charge pour gérer les scénarios de limitation côté serveur.
* Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))
* aide manquante pour afficher l’accès. ajout en cours. ([#2743](https://github.com/Azure/azure-cli/issues/2743))

### <a name="find"></a>Rechercher

* résultats de la recherche améliorés et autorisation du contrôle de version de l’index de recherche

### <a name="keyvault"></a>KeyVault

* BC : `az keyvault certificate download` remplacer -e dans chaîne ou élément binaire par PEM ou DER afin de mieux représenter les options
* BC : Supprimer --expires et --not-before dans `keyvault certificate create` car ces paramètres ne sont pas pris en charge par le service.
* Ajoute le paramètre --validity à `keyvault certificate create` pour substituer de manière sélective la valeur dans --policy
* Résout le problème dans `keyvault certificate get-default-policy` où « expires » et « not_before » étaient exposés mais « validity_in_months » ne l’était pas.
* correction de keyvault pour l’importation de pem et pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))

### <a name="lab"></a>Laboratoire

* Ajout des commandes créer, afficher, supprimer et liste pour l’environnement dans le laboratoire.
* Ajout des commandes afficher et liste pour afficher les modèles ARM dans le laboratoire.
* Ajout de l’indicateur --environment dans `az lab vm list` pour filtrer les machines virtuelles selon l’environnement du laboratoire.
* Ajout de la commande pratique `az lab formula export-artifacts` pour exporter une structure d’artefact dans une formule de laboratoire.
* Ajout de commandes pour gérer les secrets dans un laboratoire.

### <a name="monitor"></a>Surveiller

* Correction de bogue : modélisation `--actions` de `az alert-rules create` pour consommer la chaîne JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))
* Correction de bogue : la création de paramètres de diagnostic n’accepte pas les métriques/journaux à partir des commandes d’affichage ([#2913](https://github.com/Azure/azure-cli/issues/2913))

### <a name="network"></a>Réseau

* Ajouter la commande `network watcher test-connectivity`.
* Ajouter la prise en charge du paramètre `--filters` pour `network watcher packet-capture create`.
* Ajouter la prise en charge pour le drainage de connexion Application Gateway.
* Ajouter la prise en charge pour la configuration du jeu de règles WAF d’Application Gateway.
* Ajouter la prise en charge des règles et des filtres de routage ExpressRoute.
* Ajouter la prise en charge pour le routage géographique TrafficManager.
* Ajouter la prise en charge des sélecteurs de trafic basés sur la stratégie de connexion VPN.
* Ajouter la prise en charge pour les stratégies IPSec de la connexion VPN.
* Corriger le bogue avec `vpn-connection create` lors de l’utilisation des paramètres `--no-wait` ou `--validate`.
* Ajouter la prise en charge des passerelles de réseau virtuel actif-actif
* Supprimer les valeurs NULL de la sortie des commandes `network vpn-connection list/show`.
* BC : résoudre un bogue dans la sortie de `vpn-connection create` 
* Corriger le bogue où l’argument « --key-length » de « vpn-connection create » n’était pas analysé correctement.
* Corriger le bogue dans `dns zone import` où les enregistrements n’étaient pas été importés correctement.
* Corriger le bogue où `traffic-manager endpoint update` ne fonctionnait pas.
* Ajouter des commandes d’aperçu « network watcher ».

### <a name="profile"></a>Profil

* Prendre en charge la connexion lorsqu’il n’y a aucun abonnement trouvé ([#2560](https://github.com/Azure/azure-cli/issues/2560))
* Prendre en charge un nom de paramètre court dans le jeu de comptes az --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))

### <a name="redis"></a>Redis

* Ajout d’une commande de mise à jour qui ajoute également la possibilité de mettre à l’échelle pour le cache redis
* Commande « update-settings » déconseillée.

### <a name="resource"></a>Ressource

* Ajouter managedapp et les commandes de définition managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985))
* Prendre en charge les commandes « provider operation » ([#2908](https://github.com/Azure/azure-cli/issues/2908))
* Prendre en charge la création de ressource générique ([#2606](https://github.com/Azure/azure-cli/issues/2606))
* Corriger l’analyse de ressource et la recherche de version d’API. ([#2781](https://github.com/Azure/azure-cli/issues/2781))
* Ajouter des documents pour mise à jour du verrou az. ([#2702](https://github.com/Azure/azure-cli/issues/2702))
* Sortie d’erreur si vous essayez de lister des ressources pour un groupe qui n’existe pas. ([#2769](https://github.com/Azure/azure-cli/issues/2769))
* [Compute] Résoudre les problèmes de mise à jour de VMSS et du groupe à haute disponibilité de machines virtuelles. ([#2773](https://github.com/Azure/azure-cli/issues/2773))
* Corriger le verrouillage des commandes créer et supprimer si parent-resource-path est None ([#2742](https://github.com/Azure/azure-cli/issues/2742))

### <a name="role"></a>Rôle

* create-for-rbac : vérifier que la date de fin du SP ne dépassera pas la date d’expiration du certificat ([#2989](https://github.com/Azure/azure-cli/issues/2989))
* RBAC : ajouter la prise en charge complète de « ad group » ([#2016](https://github.com/Azure/azure-cli/issues/2016))
* rôle : résoudre les problèmes de mise à jour de définition de rôle ([#2745](https://github.com/Azure/azure-cli/issues/2745))
* create-for-rbac : vérifier que le mot de passe fourni par l’utilisateur est accepté

### <a name="sql"></a>SQL

* Commandes az sql server list-usages et az sql db list-usages ajoutées.
* SQL : possibilité de se connecter directement au fournisseur de ressources ([#2832](https://github.com/Azure/azure-cli/issues/2832))

### <a name="storage"></a>Storage

* Définir l’emplacement par défaut sur l’emplacement du groupe de ressources pour `storage account create`.
* Ajouter la prise en charge de la copie incrémentielle d’objet blob
* Ajouter la prise en charge du chargement d’objet blob de blocs volumineux
* Modifier la taille de bloc à 100 Mo lorsque le fichier à charger est supérieur à 200 Go

### <a name="vm"></a>Machine virtuelle

* avail-set : rendre le compte de domaine UD&FD facultatif

  remarque : commandes de machine virtuelle dans clouds souverains Veuillez éviter les fonctionnalités liées au disque managé, notamment :
  1. az disk/snapshot/image
  2. az vm/vmss disk
  3. Dans « az vm/vmss create », utiliser « —use-unmanaged-disk » pour éviter le disque managé Les autres commandes devraient fonctionner
* vm/vmss : améliorer le texte d’avertissement lors de la génération de paires de clés ssh
* vm/vmss : prendre en charge la création à partir d’une image de la Place de marché qui requiert des informations sur le plan ([#1209](https://github.com/Azure/azure-cli/issues/1209))


## <a name="april-3-2017"></a>3 avril 2017

Version 2.0.2

Nous avons publié les composants ACR, Batch, KeyVault et SQL dans cette version.

```
azure-cli (2.0.2)
 
acr (2.0.0)
acs (2.0.2)
appservice (0.1.2)
batch (2.0.0)
cloud (2.0.0)
component (2.0.0)
configure (2.0.2)
container (0.1.2)
core (2.0.2)
documentdb (0.1.2)
feedback (2.0.0)
find (0.0.1b1)
iot (0.1.2)
keyvault (2.0.0)
lab (0.0.1)
monitor (0.0.1)
network (2.0.2)
nspkg (2.0.0)
profile (2.0.2)
redis (0.1.1b3)
resource (2.0.2)
role (2.0.1)
sql (2.0.0)
storage (2.0.2)
vm (2.0.2)
```

### <a name="core"></a>Principal

* Ajout des modules acr, lab, monitor et find à la liste par défaut.
* Connexion : ignorer les locataires erronés ([#2634](https://github.com/Azure/azure-cli/pull/2634))
* login : définition de l’abonnement par défaut à la valeur « un » avec l’état « Activé » ([#2575](https://github.com/Azure/azure-cli/pull/2575))
* Ajout de la prise en charge des commandes wait et de --no-wait à davantage de commandes ([#2524](https://github.com/Azure/azure-cli/pull/2524))
* core : prise en charge de la connexion à l’aide du principal du service avec un certificat ([#2457](https://github.com/Azure/azure-cli/pull/2457))
* Ajout d’une invite pour les paramètres de modèle manquants. ([#2364](https://github.com/Azure/azure-cli/pull/2364))
* Prise en charge de la définition de valeurs par défaut pour des arguments courants tels que le groupe de ressources par défaut, le site web par défaut et la machine virtuelle par défaut
* Prise en charge de la connexion à un locataire spécifique
 
### <a name="acs"></a>ACS

* [ACS] Ajout de la prise en charge de la configuration d’un cluster ACS par défaut ([#2554](https://github.com/Azure/azure-cli/pull/2554))
* Ajout de la prise en charge de l’invite de mot de passe de clé ssh. ([#2044](https://github.com/Azure/azure-cli/pull/2044))
* Ajout de la prise en charge des clusters Windows. ([#2211](https://github.com/Azure/azure-cli/pull/2211))
* Basculement du rôle Propriétaire au rôle Contributeur. ([#2321](https://github.com/Azure/azure-cli/pull/2321))
 
### <a name="appservice"></a>AppService

* appservice : prise en charge de l’obtention de l’adresse IP externe utilisée pour les enregistrements A DNS ([#2627](https://github.com/Azure/azure-cli/pull/2627))
* appservice : prise en charge de la liaison des certificats avec caractères génériques ([#2625](https://github.com/Azure/azure-cli/pull/2625))
* appservice : prise en charge des profils de publication de liste ([#2504](https://github.com/Azure/azure-cli/pull/2504))
* AppService : déclenchement de la synchronisation de contrôle de code source après la configuration ([#2326](https://github.com/Azure/azure-cli/pull/2326))
 
### <a name="datalake"></a>DataLake

* Version initiale du module Data Lake Analytics.
* Version initiale du module Data Lake Store.
 
### <a name="docuemntdb"></a>DocumentDB

* DocumentDB : ajout de la prise en charge de l’énumération des chaînes de connexion ([#2580](https://github.com/Azure/azure-cli/pull/2580))

### <a name="vm"></a>Machine virtuelle

* [Compute] Ajout de la prise en charge d’AppGateway à la création de groupe de machines virtuelles identiques ([#2570](https://github.com/Azure/azure-cli/pull/2570))
* [VM/VMSS] Amélioration de la prise en charge de la mise en cache de disque ([#2522](https://github.com/Azure/azure-cli/pull/2522))
* VM/VMSS : intégration de la logique de validation des informations d’identification utilisée par le portail ([#2537](https://github.com/Azure/azure-cli/pull/2537))
* Ajout de la prise en charge des commandes wait et de --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))
* Groupe de machines virtuelles identiques : prise en charge de * pour énumérer les vues d’instance parmi les machines virtuelles ([#2467](https://github.com/Azure/azure-cli/pull/2467))
* Ajout de --secrets pour les machines virtuelles et les groupes de machines virtuelles identiques ([#2212} (https://github.com/Azure/azure-cli/pull/2212))
* Autorisation de la création de machines virtuelles avec un disque dur virtuel spécialisé ([#2256](https://github.com/Azure/azure-cli/pull/2256))

## <a name="february-27-2017"></a>27 février 2017

Version 2.0.0

Cette version d’Azure CLI 2.0 est la première version en « Disponibilité générale ».
La disponibilité générale s’applique à ces modules de commande :
- Container Service (acs)
- Compute (notamment Resource Manager, machine virtuelle, groupes de machines virtuelles identiques, Managed Disks)
- Réseau
- Stockage

Ces modules de commande peuvent être utilisés en production et sont pris en charge par le contrat SLA Microsoft standard.
Vous pouvez ouvrir des incidents directement auprès du support technique de Microsoft ou dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/).
Vous pouvez poser des questions sur [StackOverflow à l’aide du mot clé azure-cli](http://stackoverflow.com/questions/tagged/azure-cli) ou contacter l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Vous pouvez fournir des commentaires à partir de la ligne de commande avec la commande `az feedback`.

Les commandes de ces modules sont stables et il n’est pas prévu que la syntaxe change dans les mises à jour ultérieures de cette version d’Azure CLI.

Pour vérifier la version de l’interface CLI, utilisez `az --version`.
La sortie indique la version de l’interface CLI proprement dite (2.0.0 dans cette version), les différents modules de commande et les versions de Python et de GCC que vous utilisez.

```
azure-cli (2.0.0)

acs (2.0.0)
appservice (0.1.1b5)
batch (0.1.1b4)
cloud (2.0.0)
component (2.0.0)
configure (2.0.0)
container (0.1.1b4)
core (2.0.0)
documentdb (0.1.1b2)
feedback (2.0.0)
iot (0.1.1b3)
keyvault (0.1.1b5)
network (2.0.0)
nspkg (2.0.0)
profile (2.0.0)
redis (0.1.1b3)
resource (2.0.0)
role (2.0.0)
sql (0.1.1b5)
storage (2.0.0)
vm (2.0.0)
 
Python (Darwin) 2.7.10 (default, Jul 30 2016, 19:40:32) 
[GCC 4.2.1 Compatible Apple LLVM 8.0.0 (clang-800.0.34)]
```

> [!Note]
> Certains des modules de commande ont un suffixe « b*n* » ou « rc*n* ».
> Ces modules de commande sont toujours en préversion et seront à la disposition générale ultérieurement.

Nous avons également des versions d’évaluation nocturnes de l’interface CLI.
Pour plus d’informations, consultez ces instructions sur [l’obtention des builds nocturnes](https://github.com/Azure/azure-cli#nightly-builds) et ces instructions sur [la contribution au code et la configuration d’un environnement de développement](https://github.com/Azure/azure-cli#developer-setup).

Vous pouvez signaler des problèmes liés aux versions d’évaluation nocturnes comme suit :
- Signalez des problèmes dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/)
- Contactez l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).
- Fournissez des commentaires à partir de la ligne de commande avec la commande `az feedback`.

