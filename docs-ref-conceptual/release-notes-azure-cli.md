---
title: "Notes de publication d’Azure CLI 2.0"
description: "En savoir plus sur les dernières mises à jour d’Azure CLI 2.0"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 02/13/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 480b646b7230c8fb22f10b28a9204287cd0acc19
ms.sourcegitcommit: b93a19222e116d5880bbe64c03507c64e190331e
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/15/2018
---
# <a name="azure-cli-20-release-notes"></a>Notes de publication d’Azure CLI 2.0

## <a name="february-13-2018"></a>13 février 2018

Version 2.0.27

### <a name="core"></a>Principal

* Modification de l’authentification pour passer au système de clé sur l’ID d’abonnement et le nom sur la connexion MSI

### <a name="acs"></a>ACS

* [CHANGEMENT] `aks get-versions` renommé en `aks get-upgrades` pour des raisons de précision
* Modification de `aks get-versions` pour afficher les versions Kubernetes disponibles pour `aks create`
* Modification des valeurs par défaut de `aks create` de manière à laisser le serveur choisir la version de Kubernetes
* Mise à jour des messages d’aide faisant référence au principal du service généré par AKS
* Modification des tailles de nœud par défaut pour `aks create` pour passer de « Standard\_D1\_v2 » à « Standard\_DS1\_v2 »
* Meilleure fiabilité lors de la localisation du pod de tableau de bord pour `az aks browse`
* Correction de `aks get-credentials` pour gérer les erreurs Unicode lors du chargement des fichiers de configuration Kubernetes
* Ajout d’un message à `az aks install-cli` pour aider à l’obtention de `kubectl` dans `$PATH`

### <a name="appservice"></a>AppService

* Résolution du problème dans lequel `webapp [backup|restore]` a échoué en raison d’une référence null
* Ajout de la prise en charge supplémentaire des plans App Service par défaut via `az configure --defaults appserviceplan=my-asp`

### <a name="cdn"></a>CDN

* Ajout des commandes `cdn custom-domain [enable-https|disable-https]`

### <a name="container"></a>Conteneur

* Ajout de l’option `--follow` à `az container logs` pour les journaux de diffusion en continu
* Ajout de la commande `container attach` qui associe les flux d’erreur et de sortie standard locaux à un conteneur d’un groupe de conteneur

### <a name="cosmosdb"></a>CosmosDB

* Ajout de la prise en charge de la définition de fonctionnalités

### <a name="extension"></a>Extension

* Ajout de la prise en charge du paramètre `--pip-proxy` pour les commandes `az extension [add|update]`
* Ajout de la prise en charge de l’argument `--pip-extra-index-urls` pour les commandes `az extension [add|update]`

### <a name="feedback"></a>Commentaires

* Ajout d’informations d’extension aux données de télémétrie

### <a name="interactive"></a>Interactive

* Résolution du problème dans lequel l’utilisateur est invité à se connecter à l’aide du mode interactif dans Cloud Shell
* Correction de la régression avec les listes de saisie semi-automatique des paramètres manquants

### <a name="iot"></a>IoT

* Résolution du problème dans lequel `iot dps access policy [create|update]` renvoie une erreur « introuvable » en cas de réussite.
* Résolution du problème dans lequel `iot dps linked-hub [create|update]` renvoie une erreur « introuvable » en cas de réussite.
* Ajout de la prise en charge de `--no-wait` pour `iot dps access policy [create|update]` et `iot dps linked-hub [create|update]`
* Modification de `iot hub create` pour autoriser la spécification du nombre de partitions

### <a name="monitor"></a>Surveiller

* Correction de la commande `az monitor log-profiles create`

### <a name="network"></a>Réseau

* Correction de l’option `--tags` pour les commandes suivantes :
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a>Profil

* Activation `az login` à partir du mode interactif

### <a name="resource"></a>Ressource

* Rajout de `feature show`

### <a name="role"></a>Rôle

* Ajout de l’argument `--available-to-other-tenants` à `ad app update`

### <a name="sql"></a>SQL

* Ajout des commandes `sql server dns-alias`
* Ajout de `sql db rename`
* Ajout de la prise en charge de l’argument `--ids` pour toutes les commandes sql

### <a name="storage"></a>Stockage

* Ajout des commandes `storage blob service-properties delete-policy` et `storage blob undelete` pour permettre une suppression réversible

### <a name="vm"></a>Machine virtuelle

* Correction d’un incident lorsque le chiffrement de la machine virtuelle ne peut pas être initialisé entièrement
* Ajout de la sortie d’ID du principal lors de l’activation de MSI
* `vm boot-diagnostics get-boot-log` fixe


## <a name="january-31-2018"></a>31 janvier 2018

Version 2.0.26

### <a name="core"></a>Principal

* Ajout de la prise en charge de la récupération du jeton brut dans le contexte MSI
* Suppression de la chaîne de l’indicateur d’interrogation après la fin de LRO sur le fichier cmd.exe de Windows
* Ajout d’un avertissement qui s’affiche lorsque l’utilisation d’une valeur par défaut configurée a été remplacée par une entrée de niveau INFO. Utilisation de `--verbose` pour voir
* Ajouter un indicateur de progression pour les commandes wait

### <a name="acs"></a>ACS

* Clarification de l’argument `--disable-browser`
* Amélioration de la touche TAB pour les arguments `--vm-size`

### <a name="appservice"></a>AppService

* `webapp log [tail|download]` fixe
* Suppression de la vérification de `kind` sur les fonctions et les applications web

### <a name="cdn"></a>CDN

* Résolution du problème de client manquant avec `cdn custom-domain create`

### <a name="cosmosdb"></a>CosmosDB

* Correction de la description du paramètre pour les stratégies de basculement

### <a name="interactive"></a>Interactive

* Résolution du problème dans lequel les listes de saisie semi-automatique d’option de commande ne s’affichent plus

### <a name="network"></a>Réseau

* Ajout de la protection pour `--cert-password` à `application-gateway create`
* Résolution du problème lié à `application-gateway update` où `--sku` a appliqué par erreur une valeur par défaut
* Ajout de la protection pour `--shared-key` et `--authorization-key` à `vpn-connection create`
* Résolution du problème de client manquant avec `asg create`
* Ajout du paramètre `--file-name / -f` pour les noms exportés à `dns zone export`
* Les problèmes suivants liés à `dns zone export` ont été résolus :
  * Résolution du problème dans lequel des enregistrements TXT longs ont été mal exportés
  * Résolution du problème dans lequel des enregistrements TXT entre guillemets ont été mal exportés sans guillemets placés dans une séquence d’échappement.
* Résolution du problème où certains enregistrements ont été importés à deux reprises avec `dns zone import` 
* Restauration des commandes `vnet-gateway root-cert` et `vnet-gateway revoked-cert`

### <a name="profile"></a>Profil

* Correction de `get-access-token` pour qu’il fonctionne à l’intérieur d’une machine virtuelle avec l’identité

### <a name="resource"></a>Ressource

* Correction du bogue lié à `deployment [create|validate]` où un avertissement ne s’est pas affiché correctement quand un champ ’type’ du modèle contient des valeurs en majuscules

### <a name="storage"></a>Stockage

* Résolution du problème lié à la migration des comptes Storage V1 vers Storage V2
* Ajout de la création progressive de rapports pour toutes les commandes de chargement/téléchargement
* Résolution du bogue empêchant l’option d’argument « -n » avec `storage account check-name`  
* Ajout de la colonne de « snapshot » ajouté à la sortie de table pour `blob [list|show]`
* Résolution des bogues dans lesquels différents paramètres devaient être analysés en tant qu’entiers

### <a name="vm"></a>Machine virtuelle

* Ajout de la commande `vm image accept-terms` pour autoriser la création de machines virtuelles à partir d’images moyennant des frais supplémentaires
* Correction de `[vm|vmss create]` pour garantir l’exécution des commandes sous un proxy avec des certificats non signés
* [APERÇU] Ajout de la prise en charge de la priorité « faible» au groupe de machines virtuelles identiques
* Ajout de la protection pour `--admin-password` à `[vm|vmss] create`


## <a name="january-17-2018"></a>17 janvier 2018

Version 2.0.25

### <a name="acr"></a>ACR

* Ajout d’une connexion acr de secours en cas d’erreurs d’informations d’identification Windows
* Activation des journaux du Registre

### <a name="acs"></a>ACS

* Correction de la commande `get-credentials`
* Suppression de l’exigence de rôle SPN

### <a name="appservice"></a>AppService

* Correction du bogue avec `config ssl upload` où `hosting_environment_profile` avait la valeur null
* Ajout de la prise en charge des URL personnalisées pour `browse`
* Prise en charge de l’emplacement fixe pour `log tail`

### <a name="backup"></a>Sauvegarde

* Modification de l’option `--container-name` de `backup item list` désormais facultative
* Ajout d’options de compte de stockage à `backup restore restore-disks`
* Correction de la vérification de l’emplacement dans `backup protection enable-for-vm`, ne tient désormais plus compte de la casse
* Correction d’un problème qui causait l’échec des commandes avec un nom de conteneur non valide
* Modification de `backup item list` pour inclure « État d’intégrité » par défaut

### <a name="batch"></a>Batch

* Modification de `batch login` pour retourner des détails d’authentification

### <a name="cloud"></a>Cloud

* Ne requiert plus de points de terminaison lors de la définition de `--profile` sur un cloud

### <a name="consumption"></a>Consommation

* Ajout de nouvelles commandes pour les réservations : `consumption reservations summaries` et `consumption reservations details`

### <a name="event-grid"></a>Event Grid

* [MODIFICATION CRITIQUE] Déplacement des commandes `az eventgrid topic event-subscription` vers `eventgrid event-subscription`
* [MODIFICATION CRITIQUE] Déplacement des commandes `az eventgrid resource event-subscription` vers `eventgrid event-subscription`
* [MODIFICATION CRITIQUE] Suppression de la commande `eventgrid event-subscription show-endpoint-url`. Utilisation de `eventgrid event-subscription show --include-full-endpoint-url` à la place
* Ajout de la commande `eventgrid topic update`
* Ajout de la commande `eventgrid event-subscription update`
* Ajout du paramètre `--ids` pour les commandes `eventgrid topic`
* Ajout de la prise en charge de la saisie semi-automatique via la touche TAB pour les noms de rubrique

### <a name="interactive"></a>Interactive

* Correction d’un problème qui empêchait le fonctionnement du mode interactif avec Python 2.x
* Corrections d’erreurs au démarrage
* Correction du problème de commandes ne s’exécutant pas en mode interactif

### <a name="iot"></a>IoT

* Ajout de la prise en charge du service de provisionnement des appareils
* Ajout de messages de désapprobation dans les commandes et l’aide relative aux commandes
* Ajout de la vérification IoT pour informer les utilisateurs de l’extension IoT

### <a name="monitor"></a>Surveiller

* Ajout de la prise en charge des paramètres multi diagnostic. Le paramètre `--name` est désormais requis pour `az monitor diagnostic-settings create`
* Ajout de la commande `monitor diagnostic-settings categories` pour obtenir la catégorie des paramètres de diagnostic

### <a name="network"></a>Réseau

* Résolution du problème se produisant lors de la tentative de passage au mode actif-passif, ou depuis ce dernier, avec `vnet-gateway update`
* Ajout de la prise en charge de HTTP2 vers `application-gateway [create|update]`

### <a name="profile"></a>Profil

* Ajout de la prise en charge pour la connexion à l’aide d’identités affectées aux utilisateurs

### <a name="role"></a>Rôle

* Ajout de l’argument `--assignee-object-id` à `role assignment create` pour ignorer les requêtes de graphique

### <a name="service-fabric"></a>Service Fabric

* Ajout d’erreurs détaillées à la réponse de validation lors de la création du cluster
* Résolution du problème concernant le client manquant avec plusieurs commandes

### <a name="vm"></a>Machine virtuelle

* [PRÉVERSION] Prise en charge interzone pour `vmss`
* [MODIFICATION CRITIQUE] Modification de zone unique `vmss` par défaut en équilibreur de charge « Standard »
* [MODIFICATION CRITIQUE] Modification de `externalIdentities` en `userAssignedIdentities` pour EMSI
* [PRÉVERSION] Ajout de la prise en charge de l’échange de disque du système d’exploitation
* Ajout de la prise en charge de l’utilisation des images de machine virtuelle à partir d’autres abonnements
* Ajout des arguments `--plan-name`, `--plan-product`, `--plan-promotion-code` et `--plan-publisher` à `[vm|vmss] create`
* Correction des problèmes d’erreur avec `[vm|vmss] create`
* Correction de l’utilisation excessive des ressources due à `vm image list --all`

## <a name="december-19-2017"></a>19 décembre 2017

Version 2.0.23

* Ajout de la prise en charge pour la connexion à l’aide d’identités affectées aux utilisateurs

### <a name="container"></a>Conteneur

* Correction de l’ordre incorrect des paramètres pour les journaux du conteneur

### <a name="network"></a>Réseau

* Ajout de l’argument `--disable-bgp-route-propagation` à `route-table [create|update]`
* Ajout de l’argument `--ip-tags` à `public-ip [create|update]`

### <a name="storage"></a>Stockage

* Ajout de la prise en charge du stockage V2

### <a name="vm"></a>Machine virtuelle

* [APERÇU] Ajout de la prise en charge des identités affectées aux utilisateurs pour les machines virtuelles et les VMSS


## <a name="december-5-2017"></a>5 décembre 2017

Version 2.0.22

* Suppression des commandes `az component`. Utilisation de `az extension` à la place

### <a name="core"></a>Principal
* Modification du point de terminaison de l’autorité AAD `AZURE_US_GOV_CLOUD` pour le faire passer de login.microsoftonline.com à login.microsoftonline.us
* Résolution du problème au cours duquel les données de télémétrie étaient constamment renvoyées

### <a name="acs"></a>ACS

* Ajout des commandes `aks install-connector` et `aks remove-connector`
* Amélioration des rapports d’erreurs pour `acs create`
* Correction de l’utilisation de `aks get-credentials -f` sans chemin d’accès complet

### <a name="advisor"></a>Advisor

* Version initiale

### <a name="appservice"></a>AppService

* Correction de la génération du nom de certificat avec `webapp config ssl upload`
* Correction de `webapp [list|show]` et `functionapp [list|show]` de manière à afficher les applications correctes
* Ajout de la valeur par défaut pour `WEBSITE_NODE_DEFAULT_VERSION`

### <a name="consumption"></a>Consommation

* Ajout de la prise en charge de l’API version 2017-11-30

### <a name="container"></a>Conteneur

* Correction de la régression des ports par défaut

### <a name="monitor"></a>Surveiller

* Ajout de la prise en charge de plusieurs dimensions à la commande des mesures

### <a name="resource"></a>Ressource

* Ajout de l’argument `--include-response-body` à `resource show`

### <a name="role"></a>Rôle

* Ajout de l’affichage des affectations par défaut pour les administrateurs « classiques » à `role assignment list`
* Ajout de la prise en charge à `ad sp reset-credentials` pour l’ajout d’informations d’identification au lieu de leur remplacement
* Amélioration des rapports d’erreurs pour `ad sp create-for-rbac`

### <a name="sql"></a>SQL

* Ajout des commandes `sql db list-usages` et `sql db show-usage`
* Ajout des commandes `sql server conn-policy show` et `sql server conn-policy update`

### <a name="vm"></a>Machine virtuelle

* Ajout des informations de zone à `az vm list-skus`


## <a name="november-14-2017"></a>14 novembre 2017

Version 2.0.21

### <a name="acr"></a>ACR

* Ajout de la prise en charge pour la création de webhooks dans les régions de réplication


### <a name="acs"></a>ACS

* Modification de toutes les mentions « agent » en « nœud » dans AKS
* Option `--orchestrator-release` déconseillée pour `acs create`
* Changement de la taille de machine virtuelle par défaut pour AKS à `Standard_D1_v2`
* Résolution de `az aks browse` sur Windows
* Résolution de `az aks get-credentials` sur Windows

### <a name="appservice"></a>AppService

* Ajout de la source de déploiement `config-zip` pour les applications Web et de fonction
* Ajout de l’option `--docker-container-logging` à `az webapp log config`
* Suppression de l’option `storage` du paramètre `--web-server-logging` de `az webapp log config`
* Amélioration des messages d’erreur pour `deployment user set`
* Ajout de la prise en charge pour la création d’applications de fonction Linux
* `list-locations` fixe

### <a name="batch"></a>Batch

* Correction du bogue dans la commande de création de pool lorsqu’un ID ressource a été utilisé avec l’indicateur `--image`

### <a name="batchai"></a>Batchai

* Ajout de l’option courte, `-s`, pour `--vm-size` quand la taille de machine virtuelle est fournie dans la commande `file-server create`
* Ajout du nom de compte de stockage et des arguments de clé dans les paramètres `cluster create`
* Résolution de la documentation pour `job list-files` et `job stream-file`
* Ajout de l’option courte, `-r`, pour `--cluster-name` quand le nom du cluster est fourni dans la commande `job create`

### <a name="cloud"></a>Cloud

* Modification de `cloud [register|update]` pour empêcher l’inscription des clouds qui ne disposent pas de tous les points de terminaison requis

### <a name="container"></a>Conteneur

* Ajout de la prise en charge pour ouvrir plusieurs ports
* Ajout de la stratégie de redémarrage du groupe de conteneurs
* Ajout de la prise en charge pour monter le partage de fichier Azure en tant que volume
* Mise à jour des documents d’assistance

### <a name="data-lake-analytics"></a>Data Lake Analytics

* Modification de `[job|account] list` pour retourner des informations plus concises

### <a name="data-lake-store"></a>Data Lake Store

* Modification de `account list` pour retourner des informations plus concises

### <a name="extension"></a>Extension

* Ajout de `extension list-available` pour permettre l’affichage de la liste des extensions officielles Microsoft
* Ajout de `--name` à `extension [add|update]` pour permettre l’installation des extensions par nom

### <a name="iot"></a>IoT

* Ajout de la prise en charge pour les autorités de certification (CA) et les chaînes d’approbation

### <a name="monitor"></a>Surveiller

* Ajout des commandes `activity-log alert`

### <a name="network"></a>Réseau

* Ajout de la prise en charge pour les enregistrements DNS CAA
* Résolution d’un problème empêchant la mise à jour des points de terminaison avec `traffic-manager profile update`
* Résolution d’un problème où `vnet update --dns-servers` ne fonctionnait pas, en fonction de la façon dont avait été créé le réseau virtuel
* Résolution d’un problème où les noms DNS relatifs n’étaient pas importés correctement par `dns zone import`

### <a name="reservations"></a>Réservations

* Version préliminaire initiale

### <a name="resource"></a>Ressource

* Ajout de la prise en charge pour les ID de ressource au paramètre `--resource` et pour les verrous au niveau des ressources

### <a name="sql"></a>SQL

* Ajout du paramètre `--ignore-missing-vnet-service-endpoint` pour `sql server vnet-rule [create|update]`

### <a name="storage"></a>Stockage

* Modification de `storage account create` pour utiliser la référence SKU `Standard_RAGRS` par défaut
* Correction du bogue lors du traitement des noms d’objets blob/de fichier qui incluent des caractères non-ascii
* Correction du bogue qui empêchait l’utilisation de `--source-uri` avec `storage [blob|file] copy start-batch`
* Ajout de commandes pour paramétrer et supprimer plusieurs objets avec `storage [blob|file] delete-batch`
* Résolution du problème de l’activation des métriques avec `storage metrics update`
* Résolution du problème des fichiers de plus de 200 Go lors de l’utilisation de `storage blob upload-batch`
* Résolution du problème où `--bypass` et `--default-action` étaient ignorés par `storage account [create|update]`

### <a name="vm"></a>Machine virtuelle

* Correction d’un bogue avec `vmss create` qui empêchait l’utilisation du niveau de taille `Basic`
* Ajout d’arguments `--plan` à `[vm|vmss] create` pour les images personnalisées avec des informations de facturation
* Ajout des commandes `vm secret `[add|remove|list]
* Renommage de `vm format-secret` en `vm secret format`
* Ajout de l’argument `--encrypt format` à `vm encryption enable`

## <a name="october-24-2017"></a>24 octobre 2017

Version 2.0.20

### <a name="core"></a>Principal

* Mise à jour de `2017-03-09-profile` pour consommer l’API `MGMT_STORAGE` version `2016-01-01`

### <a name="acr"></a>ACR

* Mise à jour de la gestion des ressources pour pointer vers la version d’API `2017-10-01`
* Modification de la référence SKU « Bring Your Own Storage » en Classique
* Changement des noms des références SKU de registre en De base, Standard, et Premium

### <a name="acs"></a>ACS

* [PRÉVERSION] Ajout des commandes `az aks`
* Réparation de Kubernetes `get-credentials`

### <a name="appservice"></a>AppService

* Résolution d’une erreur où le téléchargement des journaux `webapp` était incorrect

### <a name="component"></a>Composant

* Ajout de clarté dans les messages visant à déconseiller de tous les programmes d’installation et des invites de confirmation

### <a name="monitor"></a>Surveiller

* Ajout des commandes `action-group`

### <a name="resource"></a>Ressource

* Résolution d’une incompatibilité de la dépendance msrest dans `group export` avec les versions les plus récentes
* Résolution de `policy assignment create` pour qu’il fonctionne avec les définitions de stratégie et les définitions d’ensemble de stratégie intégrées

### <a name="vm"></a>Machine virtuelle

* Ajout de l’argument `--accelerated-networking` à `vmss create`


## <a name="october-9-2017"></a>9 octobre 2017

Version 2.0.19

### <a name="core"></a>Principal

* Ajout de la gestion des URL d’autorisation AD FS avec une barre oblique à Azure Stack

### <a name="appservice"></a>AppService

* Ajout de la mise à jour générique avec la nouvelle commande `webapp update`

### <a name="batch"></a>Batch

* Mis à jour du kit de développement logiciel (SDK) à la version 4.0.0
* Mise à jour de l’option `--image` de VirtualMachineConfiguration pour prendre en charge les références d’image ARM en plus de publish:offre:sku:version
* Ajout de la prise en charge du nouveau modèle d’extension CLI pour les commandes d’extension Batch
* Suppression de la prise en charge Batch des modèles de composants

### <a name="batchai"></a>Batchai

* Version initiale du module Batch AI

### <a name="keyvault"></a>KeyVault

* Résolution du problème d’authentification Key Vault lors de l’utilisation d’AD FS sur Azure Stack. [(#4448)](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a>Réseau

* La modification de l’argument `--server` de `application-gateway address-pool create` devient facultative, permettant les pools d’adresses vides
* Mise à jour de `traffic-manager` pour prendre en charge les fonctionnalités les plus récentes

### <a name="resource"></a>Ressource

* Ajout de la prise en charge des options `--resource-group/-g` pour le nom du groupe de ressources dans `group`
* Ajout des commandes à `account lock` pour travailler avec des verrous au niveau de l’abonnement
* Ajout des commandes à `group lock` pour travailler avec des verrous au niveau du groupe
* Ajout des commandes à `resource lock` pour travailler avec des verrous au niveau des ressources

### <a name="sql"></a>SQL

* Ajout de la prise en charge pour le Chiffrement transparent des données (TDE) SQL et le chiffrement transparent des données avec Bring Your Own Key
* Ajout de la commande `db list-deleted` et du paramètre `db restore --deleted-time`, ce qui offre la possibilité de rechercher et de restaurer les bases de données supprimées
* Ajout de `db op list` et `db op cancel`, ce qui offre la capacité de répertorier et d’annuler des opérations en cours sur la base de données

### <a name="storage"></a>Stockage

* Ajout de la prise en charge d’instantané de partage de fichiers

### <a name="vm"></a>Machine virtuelle

* Correction d’un bogue dans `vm show` où l’utilisation de `-d` a provoqué un incident dans les adresses IP privées manquantes
* [VERSION PRÉLIMINAIRE] Ajout de la prise en charge de la mise à niveau propagée pour `vmss create`
* Ajout de la prise en charge de la mise à jour des paramètres de chiffrement avec `vm encryption enable`
* Ajout du paramètre `--os-disk-size-gb` pour `vm create`
* Ajout du paramètre `--license-type` de Windows pour `vmss create`


## <a name="september-22-2017"></a>22 septembre 2017

Version 2.0.18

### <a name="resource"></a>Ressource

* Ajout de la prise en charge de l’affichage des définitions de stratégie intégrée
* Ajout de la prise en charge du paramètre de mode pour la création de définitions de stratégie
* Ajout de la prise en charge des définitions d’interface utilisateur et des modèles pour `managedapp definition create`
* [CHANGEMENT RÉCENT] Modification du type de ressource `managedapp` de `appliances` en `applications` et de `applianceDefinitions` en `applicationDefinitions`

### <a name="network"></a>Réseau

* Ajout de la prise en charge de la zone de disponibilité aux sous-commandes `network lb` et `network public-ip`
* Ajout de la prise en charge de l’homologation Microsoft IPv6 pour `express-route`
* Ajout des commandes du groupe de sécurité d’application `asg`
* Ajout de l’argument `--application-security-groups` à `nic [create|ip-config create|ip-config update]`
* Ajout des arguments `--source-asgs` et `--destination-asgs` à `nsg rule [create|update]`
* Ajout des arguments `--ddos-protection` et `--vm-protection` à `vnet [create|update]`
* Ajout des commandes `network [vnet-gateway|vpn-client|show-url]`

### <a name="storage"></a>Stockage

* Résolution d’un problème qui pouvait causer l’échec des commandes `storage account network-rule` après la mise à jour du Kit de développement logiciel (SDK)

### <a name="eventgrid"></a>Événement

* Mise à jour du Kit de développement logiciel (SDK) Python Azure Event Grid afin d’utiliser une version plus récente de l’API « 2017-09-15-preview »

### <a name="sql"></a>SQL

* La modification de l’`sql server list`argument`--resource-group` devient facultative. En l’absence de précisions, tous les serveurs SQL dans l’abonnement seront retournés
* Ajout du paramètre `--no-wait` à `db [create|copy|restore|update|replica create|create|update]` et `dw [create|update]`

### <a name="keyvault"></a>KeyVault

* Ajout de la prise en charge des commandes Keyvault derrière un proxy

### <a name="vm"></a>Machine virtuelle

* Ajout de la prise en charge de zone de disponibilité pour `[vm|vmss|disk] create`
* Résolution d’un problème à cause duquel l’utilisation de `--app-gateway ID` avec `vmss create` entraînait un échec
* Ajout de l’argument `--asgs` à `vm create`
* Ajout de la prise en charge des commandes en cours d’exécution sur des machines virtuelles avec `vm run-command`
* [PRÉVERSION] Ajout de la prise en charge du chiffrement de disque VMSS avec `vmss encryption`
* Ajout de la prise en charge de la réalisation de la maintenance sur des machines virtuelles avec `vm perform-maintenance`

### <a name="acs"></a>ACS

* [PRÉVERSION] Ajout de l’argument `--orchestrator-release` à `acs create` pour les régions ACS en préversion

### <a name="appservice"></a>AppService

* Ajout de la capacité à mettre à jour et à afficher les paramètres d’authentification avec `webapp auth [update|show]`

### <a name="backup"></a>Sauvegarde

* Version préliminaire


## <a name="september-11-2017"></a>11 septembre 2017

Version 2.0.17

### <a name="core"></a>Principal

* Module de commande activé pour définir son propre ID de corrélation dans la télémétrie
* Résolution du problème de vidage JSON lorsque la télémétrie est définie en mode diagnostics

### <a name="acs"></a>Acs

* Ajout de la commande `acs list-locations`
* Faire en sorte que `ssh-key-file` soit fourni avec la valeur par défaut attendu

### <a name="appservice"></a>AppService

* Ajout de la possibilité de créer une application web dans un groupe de ressources autre que celui du plan de service actif

### <a name="cdn"></a>CDN

* Correction du bogue « CustomDomain n’est pas itérable » pour `cdn custom-domain create`.

### <a name="extension"></a>Extension

* Version initiale.

### <a name="keyvault"></a>KeyVault

* Résolution du problème, où les autorisations étaient sensibles à la casse pour `keyvault set-policy`.

### <a name="network"></a>Réseau

* Renommage de `vnet list-private-access-services` en `vnet list-endpoint-services`
* Argument `--private-access-services` renommé en `--service-endpoints` pour`vnet subnet create/update`
* Ajout de la prise en charge de plusieurs plages IP et de ports à `nsg rule create/update`
* Ajout de la prise en charge de la référence (SKU) pour `lb create`
* Ajout de la prise en charge de la référence (SKU) pour `public-ip create`

### <a name="resource"></a>Ressource

* Autoriser le passage dans les définitions de paramètres de stratégie de ressource dans `policy definition create`, et`policy definition update`
* Autoriser le passage dans les valeurs de paramètres pour `policy assignment create`
* Autoriser le passage de JSON ou d’un fichier pour tous les paramètres
* Incrémentation de la version de l’API

### <a name="sql"></a>SQL

* Ajout des commandes `sql server vnet-rule`

### <a name="vm"></a>Machine virtuelle

* Résolu : n’affecte aucun accès tant que `--scope` n’est pas indiqué
* Résolu : utilisation de la même dénomination d’extension que celle du portail
* Suppression de `subscription` de la sortie `[vm|vmss] create`
* Résolu : la référence SKU de stockage `[vm|vmss] create` n’est pas appliquée sur les disques de données avec une image
* Résolu : `vm format-secret --secrets` n’accepte pas d’ID séparés par un saut de ligne

## <a name="august-31-2017"></a>31 août 2017

Version 2.0.16

### <a name="keyvault"></a>KeyVault

* Correction d’un bogue à cause duquel vous tentez de résoudre automatiquement l’encodage secret avec `secret download`

### <a name="sf"></a>Sf

* Déconseiller toutes les commandes en faveur de Service Fabric CLI (sfctl)

### <a name="storage"></a>Stockage

* Résolution du problème dans lequel la création de comptes de stockage dans les régions ne prenant pas en charge la fonctionnalité NetworkACLs était impossible
* Déterminer le type de contenu et l’encodage du contenu lors du chargement d’objets blob et de fichiers si aucun type de contenu et d’encodage n’est spécifié.

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

### <a name="storage"></a>Stockage

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

### <a name="storage"></a>Stockage

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
* Ajout de `dla job recurrence list`

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

### <a name="storage"></a>Stockage

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

### <a name="storage"></a>Stockage

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

