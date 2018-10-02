---
title: Notes de publication d’Azure CLI
description: En savoir plus sur les dernières mises à jour d’Azure CLI
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/21/2018
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: f0ee84c3f70cf168818de447289d6c7ab5a40c9e
ms.sourcegitcommit: c4462456dfb17993f098d47c37bc19f4d78b8179
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/25/2018
ms.locfileid: "47178080"
---
# <a name="azure-cli-release-notes"></a>Notes de publication d’Azure CLI

## <a name="september-21-2018"></a>21 septembre 2018

Version 20.46

### <a name="acr"></a>ACR
* Ajout de commandes de tâche ACR
* Ajout de la commande d’exécution rapide
* Groupe de commandes `build-task` déconseillé
* Ajout du groupe de commandes `helm` pour prendre en charge la gestion des graphiques Helm avec ACR
* Ajout de la prise en charge de la création idempotent pour les registres managés
* Ajout d’un indicateur de non-format pour l’affichage des journaux de génération

### <a name="acs"></a>ACS
* Modification de la commande `install-connector` pour configurer le nom de domaine complet maître AKS
* Correction de la création d’attribution de rôle pour vnet-subnet-id lorsque le principal de service n’est pas spécifié, et pour skip-role-assignemnt

### <a name="appservice"></a>AppService

* Ajout de la prise en charge de la gestion des opérations (continues et déclenchées) des Webjobs
* az webapp config set prend en charge la propriété FTS-state. Aussi ajout de la prise en charge de az functionapp config set & show
* Ajout de la prise en charge de Bring Your Own Storage pour les applications web
* Ajout de la prise en charge du référencement et de la restauration des applications web supprimées

### <a name="batch"></a>Batch
* Modification de l’ajout des tâches via `--json-file` pour prendre en charge la syntaxe AddTaskCollectionParameter
* Mise à jour de la documentation des formats `--json-file` acceptés
* Ajout de `--max-tasks-per-node-option` à `batch pool create`
* Modification du comportement de `batch account` pour afficher la connexion au compte si aucune option n’est spécifiée

### <a name="batch-ai"></a>Batch AI 
* Correction de l’échec de création de compte de stockage automatique dans la commande `batchai cluster create`

### <a name="cognitive-services"></a>Cognitive Services
* Ajout de Completer pour les arguments `--sku`, `--kind` et `--location`
* Ajout de la commande `cognitiveservices account list-usage`
* Ajout de la commande `cognitiveservices account list-kinds`
* Ajout de la commande `cognitiveservices account list`
* `cognitiveservices list` déconseillé
* Modification de `--name` afin de le rendre facultatif pour `cognitiveservices account list-skus`

### <a name="container"></a>Conteneur
* Ajout de la possibilité de redémarrer et d’arrêter un groupe de conteneurs en cours d’exécution
* Ajout de `--network-profile` pour autoriser le passage dans un profil réseau
* Ajout de `--subnet` et `--vnet_name` pour autoriser la création de groupes de conteneurs dans un réseau virtuel
* Modification de la sortie de table pour afficher l’état du groupe de conteneurs

### <a name="datalake"></a>DataLake
* Ajout de commandes pour les règles de réseau virtuel

### <a name="interactive-shell"></a>Shell interactif
* Correction des erreurs sur Windows où les commandes ne s’exécutent pas correctement
* Correction du problème de chargement de commande dans le Shell interactif provoqué par les objets déconseillés

### <a name="iot"></a>IoT
* Ajout de la prise en charge du routage des hubs IoT

### <a name="key-vault"></a>Key Vault
* Correction de l’importation de la clé Key Vault pour les clés RSA

### <a name="network"></a>Réseau
* Ajout des commandes `network public-ip prefix` pour prendre en charge les fonctionnalités de préfixes d’adresses IP publiques
* Ajout des commandes `network service-endpoint` pour prendre en charge les fonctionnalités de stratégie de point de terminaison de service
* Ajout des commandes `network lb outbound-rule` pour prendre en charge la création de règles de trafic sortant d’un équilibreur de charge standard
* Ajout de `--public-ip-prefix` à `network lb frontend-ip create/update` pour prendre en charge les configurations IP frontales à l’aide de préfixes d’adresses IP publiques
* Ajout de `--enable-tcp-reset` à `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`
* Ajout de `--disable-outbound-snat` à `network lb rule create/update`
* Autoriser `network watcher flow-log show/configure` à être utilisé avec des groupes de sécurité réseau classiques
* Ajouter la commande `network watcher run-configuration-diagnostic`
* Correction de la commande `network watcher test-connectivity` et ajout des propriétés `--method`, `--valid-status-codes` et `--headers`
* `network express-route create/update` : ajout de l’indicateur `--allow-global-reach`
* `network vnet subnet create/update` : ajout de la prise en charge de `--delegation`
* Ajout de la commande `network vnet subnet list-available-delegations`
* `network traffic-manager profile create/update` : ajout de la prise en charge de `--interval`, `--timeout` et `--max-failures` pour les options Deprecated de configuration du moniteur `--monitor-path`, `--monitor-port` et `--monitor-protocol` en faveur de `--path`, `--port`, `--protocol`
* `network lb frontend-ip create/update` : correction de la logique de réglage de la méthode d’allocation d’adresses IP privées. Si une adresse IP privée est fournie, l’allocation sera statique. Si aucune adresse IP privée n’est fournie, ou qu’une chaîne vide est fournie pour l’adresse IP privée, l’allocation est dynamique.
* `dns record-set * create/update` : ajout de la prise en charge de `--target-resource`
* Ajout des commandes `network interface-endpoint` pour interroger les objets de point de terminaison de l’interface
* Ajout de `network profile show/list/delete` pour la gestion partielle des profils de réseau
* Ajout des commandes `network express-route peering connection` pour gérer les connexions d’appairage entre les routes ExpressRoutes

### <a name="rdbms"></a>SGBDR
* Ajout de la prise en charge du service MariaDB

### <a name="reservation"></a>Réservation
* Ajout de CosmosDb dans le type d’énumération des ressources réservées
* Ajout de la propriété de nom dans un modèle Patch

### <a name="manage-app"></a>Gérer l’application
* Correction du bogue dans `managedapp create --kind MarketPlace` à l’origine du blocage de la création d’instance d’une application Marketplace gérée
* Modification des commandes `feature` afin qu’elles soient limitées aux profils pris en charge

### <a name="role"></a>Rôle
* Ajout de la prise en charge pour répertorier les appartenances de l’utilisateur à des groupes

### <a name="signalr"></a>SignalR
* Première version

### <a name="storage"></a>Stockage
* Ajout du paramètre `--auth-mode login` pour l’utilisation des informations d’identification de l’utilisateur pour autoriser les objets blob et les files d’attente
* Ajout de `storage container immutability-policy/legal-hold` pour gérer le stockage immuable

### <a name="vm"></a>Machine virtuelle
* Correction d’un problème `vm create --generate-ssh-keys` qui remplace le fichier de clé privée si le fichier de clé publique est manquant (#4725, #6780)
* Ajout de la prise en charge pour la galerie d’images partagée via `az sig`

## <a name="august-28-2018"></a>28 Août 2018

Version 2.0.45

### <a name="core"></a>Principal

* Résolution du problème de chargement de fichier de configuration vide
* Ajout de la prise en charge du profil `2018-03-01-hybrid` pour Azure Stack

### <a name="acr"></a>ACR

* Ajout d’une solution pour les opérations d’exécution sans les requêtes ARM
* Exclusion des fichiers de contrôle de version (par exemple, .git, .gitignore) chargés par défaut dans les fichiers tar dans la commande `build`

### <a name="acs"></a>ACS

* Modification de `aks create` à la valeur par défaut sur les machines virtuelles `Standard_DS2_v2`
* Modification de `aks get-credentials` afin d’appeler de nouvelles API pour l’obtention des informations d’identification des clusters

### <a name="appservice"></a>AppService

* Prise en charge de CORS sur functionapp et webapp
* Ajout de la prise en charge de la balise ARM sur les commandes de création
* Modification de `[webapp|functionapp] identity show` permettant de quitter avec le code 3 en cas de ressource manquante

### <a name="backup"></a>Sauvegarde

* Modification de `backup vault backup-properties show` permettant de quitter avec le code 3 en cas de ressource manquante

### <a name="bot-service"></a>Service de robot

* Version initiale de l’interface CLI de Bot Service

### <a name="cognitive-services"></a>Cognitive Services

* Ajout du nouveau paramètre `--api-properties,` requis pour la création de certains services

### <a name="iot"></a>IoT

* Résolution du problème relatif à l’association de hubs liés

### <a name="monitor"></a>Surveiller

* Ajout des commandes `monitor metrics alert` permettant de recevoir des alertes sur les métriques quasiment en temps réel
* Commandes `monitor alert` déconseillées

### <a name="network"></a>Réseau

* Modification de `network application-gateway ssl-policy predefined show` permettant de quitter avec le code 3 en cas de ressource manquante

### <a name="resource"></a>Ressource

* Modification de `provider operation show` permettant de quitter avec le code 3 en cas de ressource manquante

### <a name="storage"></a>Stockage

* Modification de `storage share policy show` permettant de quitter avec le code 3 en cas de ressource manquante

### <a name="vm"></a>Machine virtuelle

* Modification de `vm/vmss identity show` permettant de quitter avec le code 3 en cas de ressource manquante 
* Remplacement de `--storage-caching` pour `vm create`

## <a name="auguest-14-2018"></a>14 août 2018

Version 2.0.44

### <a name="core"></a>Principal

* Correction de l’affichage numérique dans la sortie `table`
* Ajout du format de sortie YAML

### <a name="telemetry"></a>Télémétrie

* Amélioration des rapports de télémétrie

### <a name="acr"></a>ACR

* Ajout des commandes `content-trust policy`
* Résolution du problème où `.dockerignore` n’était pas honorée

### <a name="acs"></a>ACS

* Modification de `az acs/aks install-cli` afin d’effectuer l’installation sous `%USERPROFILE%\.azure-kubectl` sur Windows
* Modification de `az aks install-connector` afin de détecter si le cluster dispose du contrôle RBAC et de configurer le connecteur ACI correctement
* Remplacement par l’attribution de rôle au sous-réseau lorsque l’attribution est fournie
* Ajout de l’option nouveau « ignorer attribution de rôle » pour le sous-réseau lorsque l’attribution est fournie                                 
* Modification ignorant l’attribution de rôle au sous-réseau lorsque l’attribution existe déjà                

### <a name="appservice"></a>AppService

* Correction d’un bogue empêchant de créer une application de fonction à l’aide de comptes de stockage dans les groupes de ressources externes
* Correction d’un incident lors du déploiement de dossier zip

### <a name="batchai"></a>Batch AI

* Modification de la sortie de l’enregistreur d’événements pour la création du compte de stockage automatique afin de spécifier l’information « ressource *groupe*».        

### <a name="container"></a>Conteneur

* Ajout de `--secure-environment-variables` pour transmettre des variables d’environnement sécurisées vers un conteneur      

### <a name="iot"></a>IoT

* [CHANGEMENT CASSANT] Suppression des commandes obsolètes déplacées vers l’extension iot
* Mise à jour des éléments afin de ne pas prendre en compte le domaine `azure-devices.net`

### <a name="iot-central"></a>Iot Central

* Version initiale du module IoT Central

### <a name="keyvault"></a>KeyVault


* Ajout des commandes pour la gestion des comptes de stockage et les définitions SAS
* Ajout de commandes pour les règles réseau                                                           
* Ajout du paramètre `--id` aux opérations relatives au mots de passe confidentiels, clés et certificats
* Ajout de la prise en charge pour la version multi-api avec gestion des coffres de clés
* Ajout de la prise en charge pour la version multi-api avec plan de données des coffres de clés

### <a name="relay"></a>Relais

* Version initiale

### <a name="sql"></a>SQL

* Ajout des commandes `sql failover-group`

### <a name="storage"></a>Stockage

* [CHANGEMENT CASSANT] Modification de `storage account show-usage` afin d’exiger le paramètre `--location` et de répertorier par région
* Modification du paramètre `--resource-group` afin de le rendre facultatif pour les commandes `storage account`
* Suppression des avertissements concernant l’échec de la condition préalable pour les défaillances isolées dans les commandes batch pour les messages agrégés uniques
* Modification des commandes `[blob|file] delete-batch` afin de ne plus produire des tableaux ayant la valeur null
* Modification des commandes `blob [download|upload|delete-batch]` afin de lire le jeton de SAS à partir de l’url du conteneur

### <a name="vm"></a>Machine virtuelle

* Ajout des filtres courants à `vm list-skus` pour une plus grande simplicité d’utilisation

## <a name="july-31-2018"></a>31 juillet 2018

Version 2.0.43

### <a name="acr"></a>ACR

* Ajout de l’indicateur `--with-secure-properties` à la commande `acr build-task show`
* Ajout de la commande `acr build-task update-build`

### <a name="acs"></a>ACS

* Retour au return 0 (réussite) à la fin de `az aks browse` en appuyant sur [Ctrl + C]

### <a name="batch"></a>Batch

* Correction du bug lors de l’affichage des jetons AAD dans le Cloud Shell

### <a name="container"></a>Conteneur

* Suppression de l’exigence pour `--log-analytics-workspace-key` pour le nom ou l’identifiant lors de l’abonnement standard

### <a name="network"></a>Réseau

* Ajout du serveur DNS au profil du 09/03/2017 pour Azure Stack 

### <a name="resource"></a>Ressource

* Ajout de `--rollback-on-error` à `group deployment create` pour exécuter un déploiement correct et connu en cas d’erreur
* Correction d’un problème où `--parameters {}` avec `group deployment create` entraînait une erreur

### <a name="role"></a>Rôle

* Ajout de la prise en charge du profil stack du 09/03/2017
* Correction d’un problème où les paramètres de mise à jour génériques à `app update` ne fonctionnaient pas correctement

### <a name="search"></a>Recherche

* Ajout de commandes pour le service de recherches d’Azure

### <a name="service-bus"></a>Service Bus

* Ajout d’un groupe de commandes de migration pour migrer un espace de noms d’un Service Bus Standard à un Premium
* Ajout de nouvelles propriétés facultatives à la file d’attente du Service Bus et à l’abonnement
  *  `--enable-batched-operations` et `--enable-dead-lettering-on-message-expiration` dans `queue`
  *  `--dead-letter-on-filter-exceptions` dans `subscriptions`

### <a name="storage"></a>Stockage

* Ajout de la prise en charge du téléchargement de fichiers volumineux à l’aide d’une connexion unique
* Conversion des commandes `show` qui manquaient d’échouer avec le code de sortie 3 sur une ressource manquante

### <a name="vm"></a>Machine virtuelle

* Ajout d’une prise en charge pour lister les groupes disponibles par abonnement
* Ajout de la prise en charge de `StandardSSD_LRS`
* Ajout d’une prise en charge des groupes de sécurité d’application dans la création du groupe identique de machines virtuelles
* [CHANGEMENT CASSANT] Changement de `[vm|vmss] create`, `[vm|vmss] identity assign`, et `[vm|vmss] identity remove` pour sortir les identités des utilisateurs au format de dictionnaire

## <a name="july-18-2018"></a>18 juillet 2018

Version 2.0.42

### <a name="core"></a>Principal

* Ajout de la prise en charge de la connexion basée sur le navigateur dans la fenêtre d’interpréteur de commandes Windows pour Linux
* Ajout de l’indicateur `--force-string` pour toutes les commandes de mise à jour générique
* [CHANGEMENT CASSANT] Modification des commandes « d’affichage » pour connecter le message d’erreur et échec avec un code de sortie de 3 sur une ressource manquante

### <a name="acr"></a>ACR

* [CHANGEMENT CASSANT] Mise à jour de « --no-push » vers un indicateur pur dans la commande « ACR Build »
* Ajout des commandes `show` et `update` sous le groupe `acr repository`
* Ajout de l’indicateur `--detail` à `show-manifests` et `show-tags` pour afficher des informations plus détaillées
* Ajout du paramètre `--image` pour prendre en charge l’obtention des détails de build ou des journaux par une image

### <a name="acs"></a>ACS

* Modification de `az aks create` en sortie d’erreur si `--max-pods` est inférieur à 5

### <a name="appservice"></a>AppService

* Ajout de la prise en charge pour les références (SKU) PremiumV2

### <a name="batch"></a>Batch

* Correction d’un bogue relatif à l’utilisation des informations d’identification de jeton dans le mode Cloud Shell
* Modification de l’entrée JSON pour respecter la casse

### <a name="batch-ai"></a>Batch AI

* Correction de la commande `az batchai job exec`

### <a name="container"></a>Conteneur

* Suppression des exigences pour le nom d’utilisateur et le mot de passe pour les registres non dockerhub
* Correction de l’erreur lors de la création de groupes de conteneur à partir du fichier yaml

### <a name="network"></a>Réseau

* Ajout de la prise en charge de `--no-wait` pour `network nic [create|update|delete]` 
* Ajout de `network nic wait`
* Argument `--ids` déconseillé pour `network vnet [subnet|peering] list`
* Ajout de l’indicateur `--include-default` pour inclure les règles de sécurité par défaut dans la sortie de `network nsg rule list`  

### <a name="resource"></a>Ressource

* Ajout de la prise en charge de `--no-wait` pour `group deployment delete`
* Ajout de la prise en charge de `--no-wait` pour `deployment delete`
* Ajout de la commande `deployment wait`
* Résolution du problème qui causait l’affichage par erreur des commandes `az deployment` du niveau de l’abonnement pour le profil 2017-03-09-profile

### <a name="sql"></a>SQL

* Résolution de l’erreur « Le nom du groupe de ressources fourni ne correspond pas au nom de l’URL » lors de la spécification du nom du pool élastique pour les commandes `sql db copy` et `sql db replica create`
* Autoriser la configuration de SQL Server par défaut en exécutant `az configure --defaults sql-server=<name>`
* Implémentation de formateurs de table pour les commandes `sql server`, `sql server firewall-rule`, `sql list-usages` et `sql show-usage`

### <a name="storage"></a>Stockage

* Ajout de la propriété `pageRanges` à la sortie `storage blob show` qui sera renseignée pour les objets blob de pages

### <a name="vm"></a>Machine virtuelle

* [CHANGEMENT CASSANT] Modification de `vmss create` pour utiliser `Standard_DS1_v2` comme taille d’instance par défaut
* Ajout de la prise en charge de `--no-wait` pour `vm extension [set|delete]` et `vmss extension [set|delete]`
* Ajout de `vm extension wait`

## <a name="july-3-2018"></a>3 juillet 2018

Version 2.0.41

### <a name="aks"></a>AKS

* Modification de la surveillance pour utiliser l’ID d’abonnement

## <a name="july-3-2018"></a>3 juillet 2018

Version 2.0.40

### <a name="core"></a>Principal

* Ajout d’un nouveau flux de code d’autorisation pour une connexion interactive

### <a name="acr"></a>ACR

* Ajout de l’interrogation de l’état du build
* Ajout de la prise en charge des valeurs d’énumération ne respectant pas la casse
* Ajout des paramètres `--top` et `--orderby` pour `show-manifests`

### <a name="acs"></a>ACS

* [CHANGEMENT CASSANT] Active le contrôle d’accès en fonction du rôle Kubernetes par défaut
* Ajout de l’argument `--disable-rbac` et dépréciation de `--enable-rbac` dans la mesure où il s’agit actuellement de la valeur par défaut
* Mise à jour des options de la commande `aks browse`. Ajout de la prise en charge de `--listen-port`
* Mise à jour du package de graphique Helm par défaut pour la commande `aks install-connector`. Use virtual-kubelet-for-aks-latest.tgz
* Ajout des commandes `aks enable-addons` et `aks disable-addons` pour mettre à jour un cluster existant

### <a name="appservice"></a>AppService

* Ajout de la prise en charge de la désactivation d’identité via `webapp identity remove`
* Suppression de la balise `preview` pour la fonctionnalité Identité

### <a name="backup"></a>Sauvegarde

* Mise à jour de la définition du module

### <a name="batchai"></a>Batch AI

* Correction de la sortie de table pour les commandes `batchai cluster node list` et `batchai job node list`

### <a name="cloud"></a>Cloud

* Ajout du suffixe de serveur `acr login` à la configuration du cloud

### <a name="container"></a>Conteneur

* Modification de `container create` sur valeur par défaut en opération à long terme
* Ajout des paramètres Log Analytics `--log-analytics-workspace` et `--log-analytics-workspace-key`
* Ajout du paramètre `--protocol` pour spécifier le protocole réseau à utiliser

### <a name="extension"></a>Extension

* Modification de `extension list-available` pour afficher uniquement les extensions compatibles avec la version CLI

### <a name="network"></a>Réseau

* Résolution du problème où les types d’enregistrement étaient sensibles à la casse pour ([#6602](https://github.com/Azure/azure-cli/issues/6602))

### <a name="rdbms"></a>Rdbms

* Ajout des commandes `[postgres|myql] server vnet-rule`

### <a name="resource"></a>Ressource

* Ajout d’un nouveau groupe d’opérations `deployment`

### <a name="vm"></a>Machine virtuelle

* Ajout de la prise en charge de la suppression de l’identité affectée au système

## <a name="june-25-2018"></a>25 juin 2018

Version 2.0.39

### <a name="cli"></a>Interface de ligne de commande

* Mise à jour de la suppression du fichier dans le programme d’installation MSI pour résoudre le problème d’installation de l’extension

## <a name="june-19-2018"></a>19 juin 2018

Version 2.0.38

### <a name="core"></a>Principal

* Ajout de la prise en charge globale de `--subscription` pour la plupart des commandes

### <a name="acr"></a>ACR

* Ajout de `azure-storage-blob` comme dépendance
* Modification de la configuration de l’UC par défaut avec `acr build-task create` pour utiliser 2 cœurs

### <a name="acs"></a>ACS

* Mise à jour des options de la commande `aks use-dev-spaces`. Ajout de la prise en charge de `--update`
* Modification de `aks get-credentials --admin` pour ne pas remplacer le contexte utilisateur dans `$HOME/.kube/config`
* Exposition de la propriété en lecture seule `nodeResourceGroup` sur les clusters managés
* Correction de l’erreur de commande `acs browse`
* `--connector-name` rendu facultatif pour `aks install-connector`, `aks upgrade-connector` et `aks remove-connector`
* Ajout de nouvelles régions Azure Container Instance pour `aks install-connector`
* Ajout de l’emplacement normalisé dans le nom de mise en production Helm et le nom du nœud pour `aks install-connector`

### <a name="appservice"></a>AppService

* Ajout de la prise en charge des versions urllib plus récentes
* Ajout de la prise en charge pour `functionapp create` pour utiliser un plan App Service à partir de groupes de ressources externes

### <a name="batch"></a>Batch

* Suppression de la dépendance `azure-batch-extensions`

### <a name="batch-ai"></a>Batch AI

* Ajout de la prise en charge des espaces de travail. Les espaces de travail permettent de regrouper les clusters, serveurs de fichiers et expériences, supprimant la limitation du nombre de ressources qui peuvent être créées
* Ajout de la prise en charge des expériences. Les expériences permettent de regrouper les tâches dans des collections, supprimant la limitation du nombre de tâches créées
* Ajout de la prise en charge pour configurer `/dev/shm` pour les travaux en cours d’exécution dans un conteneur docker
* Ajout des commandes `batchai cluster node exec` et `batchai job node exec`. Ces commandes permettent d’exécuter des commandes directement sur les nœuds et fournissent la fonctionnalité de réacheminement de port.
* Ajout de la prise en charge des commandes `--ids` et `batchai`
* [CHANGEMENT CASSANT] Tous les clusters et serveurs de fichiers doivent être créés dans des espaces de travail
* [CHANGEMENT CASSANT] Les travaux doivent être créés dans des expériences
* [CHANGEMENT CASSANT] Suppression de `--nfs-resource-group` des commandes `cluster create` et `job create`. Pour monter un NFS appartenant à un autre espace de travail/groupe de ressources, indiquez l’ID ARM du serveur de fichiers via l’option `--nfs`
* [CHANGEMENT CASSANT] Suppression de `--cluster-resource-group` de la commande `job create`. Pour soumettre un travail sur un cluster appartenant à un autre espace de travail/groupe de ressources, indiquez l’ID ARM du cluster via l’option `--cluster`
* [CHANGEMENT CASSANT] Suppression de l’attribut `location` des travaux, clusters et serveurs de fichiers. L’emplacement est maintenant un attribut d’espace de travail.
* [CHANGEMENT CASSANT] Suppression de `--location` des commandes `job create`, `cluster create` et `file-server create`
* [CHANGEMENT CASSANT] Modification des noms des options courtes pour rendre l’interface plus cohérente :
 - [`--config`, `-c`] renommé en [`--config-file`, `-f`]
 - [`--cluster`, `-r`] renommé en [`--cluster`, `-c`]
 - [`--cluster`, `-n`] renommé en [`--cluster`, `-c`]
 - [`--job`, `-n`] renommé en [`--job`, `-j`]

### <a name="maps"></a>Cartes

* [CHANGEMENT CASSANT] Modification de `maps account create` pour accepter les Conditions d’utilisation, soit par l’invite interactive ou par l’indicateur `--accept-tos`

### <a name="network"></a>Réseau

* Ajout de la prise en charge de `https` à `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)
* Correction d’un problème où `--endpoint-status` était sensible à la casse. [#6502](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a>Réservations

* [CHANGEMENT CASSANT] Ajout du paramètre obligatoire `ReservedResourceType` à `reservations catalog show`
* Ajout du paramètre `Location` à `reservations catalog show`
* [CHANGEMENT CASSANT] Suppression de `kind` de `ReservationProperties`
* [CHANGEMENT CASSANT] `capabilities` renommé en `sku_properties` dans `Catalog`
* [CHANGEMENT CASSANT] Suppression des propriétés `size` et `tier` de `Catalog`
* Ajout du paramètre `InstanceFlexibility` à `reservations reservation update`

### <a name="role"></a>Rôle

* Amélioration de la gestion des erreurs

### <a name="sql"></a>SQL

* Correction de l’erreur déroutante lors de l’exécution de `az sql db list-editions` pour un emplacement qui n’est pas disponible pour votre abonnement

### <a name="storage"></a>Stockage

* Modification de la sortie de table pour que `storage blob download` soit plus lisible

### <a name="vm"></a>Machine virtuelle

* Amélioration de la vérification de la taille de la machine virtuelle pour la prise en charge de la mise en réseau accélérée dans `vm create`
* Ajout d’un avertissement pour `vmss create` indiquant que la taille de la machine virtuelle par défaut va passer de `Standard_D1_v2` à `Standard_DS1_v2`
* Ajout de `--force-update` à `[vm|vmss] extension set` pour mettre à jour l’extension, même lorsque la configuration n’a pas changé

## <a name="june-13-2018"></a>13 juin 2018

Version 2.0.37

### <a name="core"></a>Principal

* Amélioration de la télémétrie interactive

## <a name="june-13-2018"></a>13 juin 2018

Version 2.0.36

### <a name="aks"></a>AKS

* Ajout d’options réseau avancées à `aks create`
* Ajout d’arguments à `aks create` pour permettre la surveillance et le routage HTTP
* Ajout de l’argument `--no-ssh-key` à `aks create`
* Ajout de l’argument `--enable-rbac` à `aks create`
* [PRÉVERSION] Ajout de la prise en charge pour l’authentification basée sur Azure Active Directory à `aks create`

### <a name="appservice"></a>AppService

* Résolution d’un problème lié à des versions urllib incompatibles

## <a name="june-5-2018"></a>5 juin 2018

Version 2.0.35

### <a name="interactive"></a>Interactive

* Ajout de limites aux dépendances du mode interactif

## <a name="june-5-2018"></a>5 juin 2018

Version 2.0.34

### <a name="core"></a>Principal

* Prise en charge supplémentaire pour les références de ressources inter-client
* Amélioration de la fiabilité de téléchargement des données de télémétrie

### <a name="acr"></a>ACR

* Prise en charge supplémentaire pour VSTS en tant qu’emplacement source distant
* Ajout de la commande `acr import`

### <a name="aks"></a>AKS

* `aks get-credentials` a été modifié pour créer le fichier de configuration kube avec des autorisations de système de fichiers plus sécurisées

### <a name="batch"></a>Batch

* Résolution du bogue concernant la mise en forme dans la table de liste de pool [[problème #4378](https://github.com/Azure/azure-cli/issues/4378)]

### <a name="iot"></a>IOT

* Prise en charge ajoutée pour la création de IoT Hubs de niveau de base

### <a name="network"></a>Réseau

* `network vnet peering` amélioré

### <a name="policy-insights"></a>Policy Insights

* Version initiale

### <a name="arm"></a>ARM

* Ajout des commandes `account management-group`.

### <a name="sql"></a>SQL

* Ajout de nouvelles commandes d’instance gérée :
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* Ajout de nouvelles commandes de base de données gérée :
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a>Stockage

* Ajout de types MimeTypes supplémentaires pour les formats json et javascript pour être déduit à partir des extensions de fichier

### <a name="vm"></a>Machine virtuelle

* `vm list-skus` a été modifié pour utiliser des colonnes corrigées et ajouter l’avertissement que `Tier` et `Size` seront supprimés
* Ajout de l’option `--accelerated-networking` à `vm create`
* Ajout de `--tags` à `identity create`

## <a name="may-22-2018"></a>22 mai 2018

Version 2.0.33

### <a name="core"></a>Principal

* Ajout de la prise en charge pour le développement de `@` dans les noms de fichiers

### <a name="acs"></a>ACS

* Ajout de nouvelles commandes Dev Spaces `aks use-dev-spaces` et `aks remove-dev-spaces`
* Faute de frappe corrigée dans un message d’aide

### <a name="appservice"></a>AppService

* Amélioration des commandes de mise à jour générique
* Ajout de la prise en charge asynchrone pour `webapp deployment source config-zip`

### <a name="container"></a>Conteneur

* Prise en charge ajoutée pour l’exportation d’un groupe de conteneurs au format yaml
* Prise en charge ajoutée pour l’utilisation d’un fichier yaml afin de créer/mettre à jour un groupe de conteneurs

### <a name="extension"></a>Extension

* Amélioration de la suppression des extensions

### <a name="interactive"></a>Interactive

* La journalisation a été modifiée pour désactiver l’analyseur pour les saisies semi-automatiques
* Gestion améliorée des caches d’aide incorrects

### <a name="keyvault"></a>KeyVault

* Commandes keyvault corrigées afin de fonctionner dans Cloud Shell ou dans des machines virtuelles avec l’identité

### <a name="network"></a>Réseau

* Résolution d’un problème où `network watcher show-topology` ne fonctionnait pas avec le nom de réseau virtuel et/ou de sous-réseau [#6326](https://github.com/Azure/azure-cli/issues/6326)
* Correction d’un problème où certaines commandes `network watcher` revendiquaient que Network Watcher n’était pas activé pour certaines régions alors qu’il l’était [#6264](https://github.com/Azure/azure-cli/issues/6264)

### <a name="sql"></a>SQL

* [CHANGEMENT CASSANT] Objets de réponse retournés modifiés à partir des commandes `db` et `dw`
    * Propriété `serviceLevelObjective` renommée en `currentServiceObjectiveName`
    * Suppression des propriétés `currentServiceObjectiveId` et `requestedServiceObjectiveId`
    * Propriété `maxSizeBytes` modifiée en valeur entière au lieu d’une chaîne
* [CHANGEMENT CASSANT] Les propriétés `db` et `dw` suivantes ont été modifiées pour être en lecture seule :
    * `requestedServiceObjectiveName`.  Pour mettre à jour, utilisez le paramètre `--service-objective` ou définissez la propriété `sku.name`
    * `edition`. Pour mettre à jour, utilisez le paramètre `--edition` ou définissez la propriété `sku.tier`
    * `elasticPoolName`. Pour mettre à jour, utilisez le paramètre `--elastic-pool` ou définissez la propriété `elasticPoolId`
* [CHANGEMENT CASSANT] Les propriétés `elastic-pool` suivantes ont été modifiées pour être en lecture seule :
    * `edition`. Pour mettre à jour, utilisez le paramètre `--edition`
    * `dtu`. Pour mettre à jour, utilisez le paramètre `--capacity`
    *  `databaseDtuMin`. Pour mettre à jour, utilisez le paramètre `--db-min-capacity`
    *  `databaseDtuMax`. Pour mettre à jour, utilisez le paramètre `--db-max-capacity`
* Ajout des paramètres `--family` et `--capacity` aux commandes `db`, `dw` et `elastic-pool`
* Ajout de formateurs de table aux commandes `db`, `dw` et `elastic-pool`

### <a name="storage"></a>Stockage

* Ajout d’un compléteur pour l’argument `--account-name`
* Correction d’un problème avec `storage entity query`

### <a name="vm"></a>Machine virtuelle

* [CHANGEMENT CASSANT] Suppression de `--write-accelerator` de `vm create`. La même prise en charge est accessible via `vm update` ou `vm disk attach`
* Correction de l’image de l’extension efficace dans `[vm|vmss] extension`
* Ajout de`--boot-diagnostics-storage` à `vm create` pour capturer le journal de démarrage
* Ajout de `--license-type` à `[vm|vmss] update`

## <a name="may-7-2018"></a>7 mai 2018

Version 2.0.32

### <a name="core"></a>Principal

* Correction d’une exception non gérée lors de la récupération des clés secrètes à partir d’un compte de principal de service avec certificat
* Nouvelle prise en charge limitée pour les arguments positionnels
* Correction d’un problème où `--query` ne pouvait pas être utilisé avec `--ids`. [#5591](https://github.com/Azure/azure-cli/issues/5591)
* Amélioration des scénarios de redirection à partir des commandes en utilisant `--ids`. Prend en charge `-o tsv` avec une requête spécifiée ou `-o json` sans spécification de requête
* Ajout de suggestions de commande en cas d’erreur engendrées par des fautes de frappe des utilisateurs dans les commandes
* Amélioration de l’erreur lorsque les utilisateurs entrent `az ''`
* Ajout de la prise en charge des types de ressources personnalisés pour les modules et les extensions de commande

### <a name="acr"></a>ACR

* Ajout de commandes de build de l’ACR
* Améliorations des messages d’erreur dus aux ressources introuvables
* Amélioration des performances de création de ressources et de la gestion des erreurs
* Amélioration de la connexion ACR dans des consoles non standards et des WSL
* Amélioration des messages d’erreur dus aux commandes de dépôt
* Mise à jour des colonnes de la table et du classement

### <a name="acs"></a>ACS

* Ajout d’un avertissement indiquant que `az aks` est un service en préversion
* Résolution du problème d’autorisation dans `aks install-connector` lorsque `--aci-resource-group` n’est pas spécifié

### <a name="ams"></a>AMS

* Version initiale - Gérer des ressources Azure Media Services

### <a name="appservice"></a>AppService

* Correction d’un bogue dans `webapp delete` lorsque `--slot` est fourni
* `--runtime-version` retiré de `webapp auth update`
* Ajout de la prise en charge de min\_tls\_version & https2.0
* Ajout de la prise en charge pour les multiconteneurs

### <a name="batch-ai"></a>Batch AI

* `batchai create cluster` modifié pour respecter la priorité de machine virtuelle configurée dans le fichier de configuration du cluster

### <a name="cognitive-services"></a>Cognitive Services

* Faute de frappe corrigée dans l’exemple de `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)

### <a name="consumption"></a>Consommation

* Ajout de nouvelles commandes pour l’API Budget

### <a name="container"></a>Conteneur

* Suppression de l’exigence pour `--registry-server` pour `container create` lorsqu’un serveur de registre est inclus dans le nom de l’image

### <a name="cosmos-db"></a>Cosmos DB

* Présentation de la prise en charge d’un réseau virtuel pour Azure CLI - Cosmos DB

### <a name="dms"></a>DMS

* Version initiale - Ajoute la prise en charge de l’instruction SQL pour le scénario de migration de SQL Azure

### <a name="extension"></a>Extension

* Correction d’un bogue où les métadonnées d’extension cessaient d’être affichées

### <a name="interactive"></a>Interactive

* Autorise le fonctionnement de compléments interactifs avec des arguments positionnel
* Sortie plus conviviale lorsque les utilisateurs entrent \'
* Achèvements corrigés pour les paramètres sans aide
* Descriptions corrigées pour les groupes de commandes

### <a name="lab"></a>Laboratoire

* Régressions corrigées de conversion Knack

### <a name="network"></a>Réseau

* [CHANGEMENT CASSANT] Suppression du paramètre `--ids` pour :
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a>Profil

* Correction de la détection de source `disk create`
* [CHANGEMENT CASSANT] Suppression de `--msi-port` et `--identity-port` car ils ne sont plus utilisés
* Correction d’une faute de frappe dans le bref résumé de `account get-access-token`

### <a name="redis"></a>Redis

* `redis patch-schedule patch-schedule show` déconseillé en faveur de `redis patch-schedule show`
* `redis list-all` déconseillé. Cette fonctionnalité a été pliée dans `redis list`
* `redis import-method` déconseillé en faveur de `redis import`
* Ajout de la prise en charge de `--ids` pour diverses commandes

### <a name="role"></a>Rôle

* [CHANGEMENT CASSANT] Suppression de `ad sp reset-credentials` déconseillé

### <a name="storage"></a>Stockage

* Autorise l’application du jeton SAS de destination pour une copie d’objets blob si le SAS source et la clé de compte ne sont pas spécifiés
* Exposé--délai d’expiration de socket pour les chargements et téléchargements d’objets blob
* Traite les noms d’objets blob commençant par des séparateurs de chemin d’accès comme des chemins d’accès relatifs
* Autorise `storage blob copy --source-sas` avec le caractère de démarrage de requête, « ? »
* `storage entity query --marker` corrigé pour accepter une liste de clé =valeurs

### <a name="vm"></a>Machine virtuelle

* Correction d’une logique de détection invalide sur l’URI de l’objet blob non gérée
* Ajout de la prise en charge du chiffrement de disque sans principaux de service fournis par l’utilisateur
* [CHANGEMENT CASSANT] Ne pas utiliser « ManagedIdentityExtension » de machine virtuelle pour la prise en charge de MSI
* Ajout de la prise en charge pour la stratégie d’éviction vers `vmss`
* [CHANGEMENT CASSANT] Suppression de `--ids` de :
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* Ajout de la prise en charge des accélérateurs d’écriture
* Ajout de `vmss perform-maintenance`
* Correction de `vm diagnostics set` pour détecter la fiabilité du type de système d’exploitation de la machine virtuelle
* Modification de `vm resize` pour vérifier si la taille demandée est différente de celle actuellement définie et pour mettre à jour uniquement en cas de modifications


## <a name="april-10-2018"></a>10 avril 2018

Version 2.0.31

### <a name="acr"></a>ACR

* Gestion améliorée des erreurs de secours wincred

### <a name="acs"></a>ACS

* Modification de la durée de validité des SPN créés par AKS à 5 ans

### <a name="appservice"></a>AppService

* [CHANGEMENT CASSANT]: Removed `assign-identity`
* Correction d’une exception non interceptée pour les plans webapp inexistants

### <a name="batchai"></a>Batch AI

* Ajout de la prise en charge de l’API 2018-03-01

 - Montage au niveau du travail
 - Variables d’environnement avec les valeurs des secrets
 - Paramètres des compteurs de performances
 - Création de rapports de segments de ligne spécifiques à un travail
 - Prise en charge des sous-dossiers dans les listes de fichiers de l’API
 - Création de rapports d’utilisation et de limites
 - Autorisation de la spécification du type de mise en cache pour les serveurs NFS
 - Prise en charge des images personnalisées
 - Ajout de la prise en charge de la boîte à outils pyTorch

* Ajout de la commande `job wait` qui permet d’attendre la fin du travail et d’obtenir le code de sortie du travail
* Ajout de la commande `usage show` pour répertorier l’utilisation actuelle des ressources Batch AI et les limites pour les différentes régions
* Prise en charge des clouds nationaux
* Ajout d’arguments de ligne de commande de travail pour monter des systèmes de fichiers au niveau du travail en plus des fichiers de configuration
* Ajout de plus d’options pour personnaliser les clusters : priorité des machines virtuelles, sous-réseau, nombre de nœuds initial pour les clusters avec mise à l’échelle automatique, spécification d’une image personnalisée
* Ajout d’une option de ligne de commande pour spécifier le type de mise en cache pour les NFS gérés par Batch AI
* Simplification de la spécification du montage du système de fichiers dans les fichiers config. Il est désormais possible d’omettre les informations d’identification pour les partages de fichiers Azure et les conteneurs d’objets blob Azure : CLI remplira les informations d’identification manquantes à l’aide de la clé du compte de stockage fournie par le biais des paramètres de ligne de commande ou spécifiée via la variable d’environnement, ou interrogera la clé à partir du stockage Azure (si le compte de stockage appartient à l’abonnement actuel)
* La commande de flux de fichiers de travail se remplit désormais automatiquement lorsque le travail est terminé (réussite, échec, terminé ou supprimé)
* Amélioration de la sortie `table` pour les opérations `show`
* Ajout de l’option `--use-auto-storage` pour la création du cluster. Cette option simplifie la gestion des comptes de stockage et le montage de partages de fichiers Azure et de conteneurs d’objets blob Azure vers des clusters
* Ajout de l’option `--generate-ssh-keys` à `cluster create` et `file-server create`
* Ajout de la possibilité de fournir la tâche de configuration de nœud via la ligne de commande
* [CHANGEMENT CASSANT] Déplacement des commandes `job stream-file` et `job list-files` sous le groupe `job file`
* [CHANGEMENT CASSANT] Renommage de `--admin-user-name` en `--user-name` dans la commande `file-server create` pour être cohérent avec la commande `cluster create`

### <a name="billing"></a>Facturation

* Ajout de commandes d’inscription de compte

### <a name="consumption"></a>Consommation

* Ajout des commandes `marketplace`
* [CHANGEMENT CASSANT] Renommage de `reservations summaries` en `reservation summary`
* [CHANGEMENT CASSANT] Renommage de `reservations details` en `reservation detail`
* [CHANGEMENT CASSANT] Suppression des options abrégées de `--reservation-order-id` et `--reservation-id` pour les commandes `reservation`
* [CHANGEMENT CASSANT] Suppression des options abrégées de `--grain` pour les commandes `reservation summary`
* [CHANGEMENT CASSANT] Suppression des options abrégées de `--include-meter-details` pour les commandes `pricesheet`

### <a name="container"></a>Conteneur

* Ajout des paramètres de montage de volume de référentiel Git `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` et `--gitrepo-mount-path`
* Résolution de [#5926](https://github.com/Azure/azure-cli/issues/5926) : `az container exec` échoue lorsque le nom du conteneur -- est spécifié

### <a name="extension"></a>Extension

* Modification du message de vérification de distribution pour qu’il soit au niveau du débogage

### <a name="interactive"></a>Interactive

* Modification pour arrêter la saisie semi-automatique sur les commandes non reconnues
* Ajout d’événements de raccordement avant et après la création du sous-arbre de commande
* Ajout de la saisie semi-automatique pour les paramètres `--ids`

### <a name="network"></a>Réseau

* Résolution de [#5936](https://github.com/Azure/azure-cli/issues/5936) : les balises `application-gateway create` n’ont pas pu déterminer l’ensemble
* Ajout de l’argument `--auth-certs` pour joindre des certificats d’authentification pour `application-gateway http-settings [create|update]`. [#4910](https://github.com/Azure/azure-cli/issues/4910)
* Ajout de commandes `ddos-protection` pour créer des plans de protection DDoS
* Prise en charge de `--ddos-protection-plan` pour `vnet [create|update]` pour associer un réseau virtuel à un plan de protection DDoS
* Résolution du problème avec l’ indicateur `--disable-bgp-route-propagation` dans `network route-table [create|update]`
* Suppression des arguments factices `--public-ip-address-type` et `--subnet-type` pour `network lb [create|update]`
* Ajout de la prise en charge des enregistrements TXT avec les séquences d’échappement RFC 1035 à `network dns zone [import|export]` et `network dns record-set txt add-record`

### <a name="profile"></a>Profil

* Ajout de la prise en charge des comptes Azure Classic dans `account list`
* [CHANGEMENT CASSANT] Suppression des arguments `--msi` & `--msi-port`

### <a name="rdbms"></a>SGBDR

* Ajout de la commande `georestore`
* Suppression de la restriction de taille de stockage de la commande `create`

### <a name="resource"></a>Ressource

* Ajout de la prise en charge de `--metadata` pour `policy definition create`
* Ajout de la prise en charge de `--metadata`, `--set`, `--add` et `--remove` à `policy definition update`

### <a name="sql"></a>SQL

* Ajout de `sql elastic-pool op list` et `sql elastic-pool op cancel`

### <a name="storage"></a>Stockage

* Amélioration des messages d’erreur pour les chaînes de connexion incorrectes

### <a name="vm"></a>Machine virtuelle

* Ajout de la prise en charge pour configurer le nombre de domaines d’erreur de plateforme sur `vmss create`
* Modification de `vmss create` sur la valeur par défaut de l’équilibreur de charge Standard pour les groupes identiques désactivés zonaux, grands ou avec un seul groupe de placement
* [CHANGEMENT CASSANT]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret`
* Ajout de la prise en charge des références SKU d’IP public à `vm create`
* Ajout des arguments `--keyvault` et `--resource-group` à `vm secret format` pour prendre en charge des scénarios où la commande ne parvient pas à résoudre l’ID de coffre. [#5718](https://github.com/Azure/azure-cli/issues/5718)
* Amélioration des erreurs pour `[vm|vmss create]` lorsque l’emplacement d’un groupe de ressources ne possède aucune prise en charge de zone


## <a name="march-27-2018"></a>27 mars 2018

Version 2.0.30

### <a name="core"></a>Principal

* Afficher le message pour les extensions marquées en tant que préversions dans l’aide

### <a name="acs"></a>ACS

* Corriger l’erreur de vérification de certificat SSL pour `aks install-cli` dans Cloud Shell

### <a name="appservice"></a>AppService

* Ajout de la prise en charge HTTPS exclusive à `webapp update`
* Ajout de la prise en charge des emplacements à `az webapp identity [assign|show]` et `az functionapp identity [assign|show]`

### <a name="backup"></a>Sauvegarde

* Ajout de la commande `az backup protection isenabled-for-vm` Cette commande peut être utilisée pour vérifier si une machine virtuelle est sauvegardée par un coffre dans l’abonnement
* Activation des ID d’objet Azure pour les paramètres `--resource-group` et `--vault-name`, pour les commandes suivantes :
  * `backup container show`
  * `backup item set-policy`
  * `backup item show`
  * `backup job show`
  * `backup job stop`
  * `backup job wait`
  * `backup policy delete`
  * `backup policy get-default-for-vm`
  * `backup policy list-associated-items`
  * `backup policy set`
  * `backup policy show`
  * `backup protection backup-now`
  * `backup protection disable`
  * `backup protection enable-for-vm`
  * `backup recoverypoint show`
  * `backup restore files mount-rp`
  * `backup restore files unmount-rp`
  * `backup restore restore-disks`
  * `backup vault delete`
  * `backup vault show`
* Modification des paramètres `--name` pour accepter le format de sortie des commandes `backup ... show`

### <a name="container"></a>Conteneur

* Ajout de la commande `container exec` Exécute les commandes dans un conteneur, pour un groupe de conteneurs en exécution.
* Autoriser la sortie de table pour la création et la mise à jour d’un groupe de conteneurs

### <a name="extension"></a>Extension

* Ajout d’un message pour `extension add` si l’extension est en préversion
* Modification de `extension list-available` afin d’afficher les données complètes d’extension avec `--show-details`
* [CHANGEMENT CASSANT] Modification de `extension list-available` afin d’afficher les données simplifiées d’extension par défaut

### <a name="interactive"></a>Interactive

* Modification des saisies semi-automatiques pour procéder à l’activation dès le chargement de la table de commande
* Correction du bogue par l’exécution du paramètre `--style`
* Analyseur lexical interactif instancié après le vidage de la table de commande, si manquant
* Amélioration de la prise en charge de Completer

### <a name="lab"></a>Laboratoire

* Correction des bogues avec la commande `create environment`

### <a name="monitor"></a>Surveiller

* Ajout de la prise en charge de `--top`, `--orderby` et `--namespace` à `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)
* Résolution de [#4529](https://github.com/Azure/azure-cli/issues/5785) : `metrics list` Accepte une liste de mesures séparées par des espaces à récupérer
* Ajout de la prise en charge de `--namespace` à `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)

### <a name="network"></a>Réseau

* Ajout de la prise en charge des zones de DNS privé

### <a name="profile"></a>Profil

* Ajout d’un avertissement pour `--identity-port` et `--msi-port` à `login`

### <a name="rdbms"></a>SGBDR

* Ajout de la version d’API mise à la disposition générale du modèle d’entreprise 2017-12-01

### <a name="resource"></a>Ressource

* [CHANGEMENT CASSANT]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a>Rôle

* Ajout de la prise en charge des configurations d’accès et des clients natifs requis à `az ad app create`
* Modification des commandes `rbac` afin de renvoyer moins de 1 000 ID sur la résolution d’objet
* Ajout des commandes de gestion des informations d’identification `ad sp credential [reset|list|delete]`
* [CHANGEMENT CASSANT] Suppression des propriétés de la sortie `az role assignment [list|show]`
* Ajout de la prise en charge des autorisations `dataActions` et `notDataActions` à `role definition`

### <a name="storage"></a>Stockage

* Résolution du problème lié au chargement des fichiers présentant une taille comprise entre 195 Go et 200 Go
* Résolution de [#4049](https://github.com/Azure/azure-cli/issues/4049) : Problèmes avec les chargements d’objets blob d’ajout ignorant les paramètres de condition

### <a name="vm"></a>Machine virtuelle

* Ajout d’un avertissement à `vmss create` concernant les changements cassants à venir pour les ensembles comprenant plus de 100 instances
* Ajout de la prise en charge de la résilience dans la zone à `vm [snapshot|image]`
* Modification de la vue d’instance de disque pour signaler un meilleur état de chiffrement
* [CHANGEMENT CASSANT] Modification de `vm extension delete` afin d’annuler la capacité de génération de sortie

## <a name="march-13-2018"></a>13 mars 2018

Version 2.0.29

### <a name="acr"></a>ACR

* Ajout de la prise en charge du paramètre `--image` pour `repository delete`
* Paramètres `--manifest` et `--tag` de la commande `repository delete` déconseillés
* Ajout de la commande `repository untag` pour supprimer une balise sans supprimer les données

### <a name="acs"></a>ACS

* Ajout de la commande `aks upgrade-connector` pour mettre à niveau un connecteur existant
* Modification des fichiers de configuration `kubectl` pour utiliser un YAML de style bloc plus lisible

### <a name="advisor"></a>Advisor

* [CHANGEMENT CASSANT] Renommage de `advisor configuration get` en `advisor configuration list`
* [CHANGEMENT CASSANT] Renommage de `advisor configuration set` en `advisor configuration update`
* [CHANGEMENT CASSANT] Suppression de `advisor recommendation generate`
* Ajout du paramètre `--refresh` pour `advisor recommendation list`
* Ajout de la commande `advisor recommendation show`

### <a name="appservice"></a>AppService

* `[webapp|functionapp] assign-identity` déconseillé
* Ajout des commandes d’identité gérée `webapp identity [assign|show]` et `functionapp identity [assign|show]`

### <a name="eventhubs"></a>Eventhubs

* Version initiale

### <a name="extension"></a>Extension

* Ajout d’un contrôle supplémentaire pour avertir l’utilisateur si le distributeur utilisé est différent de celui stocké dans le fichier source du package, car cela peut entraîner des erreurs

### <a name="interactive"></a>Interactive

* Résolu [#5625](https://github.com/Azure/azure-cli/issues/5625) : conservation de l’historique entre différentes sessions
* Résolu [#3016](https://github.com/Azure/azure-cli/issues/3016) : historique non enregistré alors qu’il était dans la portée
* Résolu [#5688](https://github.com/Azure/azure-cli/issues/5688) : la saisie automatique n’apparaît pas si le chargement de la table de commande a rencontré une exception
* Résolu : indicateur de progression pour les opérations à long terme

### <a name="monitor"></a>Surveiller

* Les commandes `monitor autoscale-settings` ont été déconseillées
* Ajout des commandes `monitor autoscale`
* Ajout des commandes `monitor autoscale profile`
* Ajout des commandes `monitor autoscale rule`

### <a name="network"></a>Réseau

* [CHANGEMENT CASSANT] Suppression du paramètre `--tags` de `route-filter rule create`
* Suppression de certaines valeurs par défaut erronées pour les commandes suivantes :
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* Ajout des commandes `network watcher connection-monitor`
* Ajout des paramètres `--vnet` et `--subnet` à `network watcher show-topology`

### <a name="profile"></a>Profil

* Paramètre `--msi` déconseillé pour `az login`
* Ajout du paramètre `--identity` pour `az login` afin de remplacer `--msi`

### <a name="rdbms"></a>SGBDR

* [PRÉVERSION] Modifiée pour utiliser l’API 2017-12-01-préversion

### <a name="service-bus"></a>Service Bus

* Version initiale

### <a name="storage"></a>Stockage

* Résolution de [#4971](https://github.com/Azure/azure-cli/issues/4971) : `storage blob copy` prend désormais en charge les autres clouds Azure
* Résolu [#5286](https://github.com/Azure/azure-cli/issues/5286) : Les lots de commandes `storage blob [delete-batch|download-batch|upload-batch]` ne génèrent plus une erreur lors d’échecs de la condition préalable

### <a name="vm"></a>Machine virtuelle

* Ajout de prise en charge de `[vm|vmss] create` pour attacher des disques de données non gérées et configurer la mise en cache
* `[vm|vmss] assign-identity` et `[vm|vmss] remove-identity` sont déconseillés
* Ajout des commandes `vm identity [assign|remove|show]` et `vmss identity [assign|remove|show]` pour remplacer des commandes déconseillées
* Modification de la priorité par défaut dans `vmss create` à None

## <a name="february-27-2018"></a>27 février 2018

Version 2.0.28

### <a name="core"></a>Principal

* Résolu [#5184](https://github.com/Azure/azure-cli/issues/5184) : Problème d’installation d’Homebrew
* Ajout de la prise en charge de télémétrie d’extension avec des clés personnalisées
* Ajout de la connexion HTTP à `--debug`

### <a name="acs"></a>ACS

* Modification pour utiliser le graphique Helm `virtual-kubelet-for-aks` pour `aks install-connector` par défaut
* Problème résolu : autorisation insuffisante des principaux de service à créer des groupes de conteneur ACI
* Ajout des paramètres `--aci-container-group`, `--location` et `--image-tag` à `aks install-connector`
* Suppression de l’avis de désapprobation de `aks get-versions`

### <a name="appservice"></a>AppService

* Mises à jour pour la nouvelle version du kit de développement logiciel (SDK) (azure-mgmt-web 0.35.0)
* Résolu [#5538](https://github.com/Azure/azure-cli/issues/5538) : `Free` défini comme une SKU invalide

### <a name="cognitive-services"></a>Cognitive Services

* Mise à jour de l’avis lors de la création d’un compte Cognitive Services

### <a name="consumption"></a>Consommation

* Ajout de nouvelles commandes pour l’API priceSheet
* Mise à jour des formats existants Détails d’utilisations et Détails de la réservation

### <a name="container"></a>Conteneur

* Ajout des arguments `--secrets` et `--secrets-mount-path` à `container create` pour utiliser des secrets dans ACI

### <a name="network"></a>Réseau

* Résolu [#5559](https://github.com/Azure/azure-cli/issues/5559) : client manquant dans `network vnet-gateway vpn-client generate`

### <a name="resource"></a>Ressource

* Modification de `group deployment export` pour afficher un modèle et des erreurs partiels sur échec

### <a name="role"></a>Rôle

* Ajout de `role assignment list-changelogs` pour permettre l’audit des rôles du principal de service

### <a name="sql"></a>SQL

* Ajout de la prise en charge de la redondance de zone pour les bases de données et les pools élastiques lors de création et mise à jour

### <a name="storage"></a>Stockage

* Activation de la spécification de préfixe/destination pour `storage blob [upload-batch|download-batch]`

### <a name="vm"></a>Machine virtuelle

* Ajout de prise en charge de jonction / séparation de disques sur une instance de groupe de machines virtuelles identiques uniques


## <a name="february-13-2018"></a>13 février 2018

Version 2.0.27

### <a name="core"></a>Principal

* Modification de l’authentification pour passer au système de clé sur l’ID d’abonnement et le nom sur la connexion MSI

### <a name="acs"></a>ACS

* [CHANGEMENT CASSANT] Renommage de `aks get-versions` en `aks get-upgrades` pour des raisons de précision
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

* Résolution du problème dans lequel `iot dps access policy [create|update]` renvoie une erreur « introuvable » en cas de réussite
* Résolution du problème dans lequel `iot dps linked-hub [create|update]` renvoie une erreur « introuvable » en cas de réussite
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

* [CHANGEMENT CASSANT] Déplacement des commandes `az eventgrid topic event-subscription` vers `eventgrid event-subscription`
* [CHANGEMENT CASSANT] Déplacement des commandes `az eventgrid resource event-subscription` vers `eventgrid event-subscription`
* [CHANGEMENT CASSANT] Suppression de la commande `eventgrid event-subscription show-endpoint-url` Utilisation de `eventgrid event-subscription show --include-full-endpoint-url` à la place
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
* [CHANGEMENT CASSANT] Modification de la valeur par défaut `vmss` de zone unique en équilibreur de charge « Standard »
* [CHANGEMENT CASSANT] Modification de `externalIdentities` en `userAssignedIdentities` pour EMSI
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
* [CHANGEMENT CASSANT] Modification du type de ressource `managedapp` de `appliances` en `applications` et de `applianceDefinitions` en `applicationDefinitions`

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

* Correction du bogue « CustomDomain n’est pas itérable » pour `cdn custom-domain create`

### <a name="extension"></a>Extension

* Version initiale

### <a name="keyvault"></a>KeyVault

* Résolution du problème où les autorisations étaient sensibles à la casse pour `keyvault set-policy`

### <a name="network"></a>Réseau

* Renommage de `vnet list-private-access-services` en `vnet list-endpoint-services`
* Argument `--private-access-services` renommé en `--service-endpoints` pour`vnet subnet create/update`
* Ajout de la prise en charge de plusieurs plages IP et de ports à `nsg rule create/update`
* Ajout de la prise en charge de la référence (SKU) pour `lb create`
* Ajout de la prise en charge de la référence (SKU) pour `public-ip create`

### <a name="resource"></a>Ressource

* Autoriser le passages dans les définitions de paramètres de stratégie de ressource dans `policy definition create`, et`policy definition update`
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

* Ajout d’une remarque juridique pour `--version`

### <a name="acs"></a>ACS

* Correction des régions d’aperçu
* Mise en forme par défaut `dns_name_prefix` correctement
* Optimisation de la sortie de commande des services ACS

### <a name="appservice"></a>AppService

* [CHANGEMENT CASSANT] Fixation des incohérences dans la sortie de `az webapp config appsettings [delete|set]`
* Ajout d’un nouvel alias de `-i` pour `az webapp config container set --docker-custom-image-name`
* Exposé `az webapp log show`
* Exposition de nouveaux arguments à partir de `az webapp delete` pour conserver le plan de service d'application, les métriques ou l’inscription DNS
* Problème résolu : Détecter les paramètres d’emplacement correctement

### <a name="iot"></a>IoT

* Résolu #3934 : La création de la stratégie n’efface plus les stratégies existantes

### <a name="network"></a>Réseau

* [CHANGEMENT CASSANT] Renommage de `vnet list-private-access-services` en `vnet list-endpoint-services`
* [CHANGEMENT CASSANT] Renommage de l’option `--private-access-services` en `--service-endpoints` pour `vnet subnet [create|update]`
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
* [CHANGEMENT CASSANT] Renommage de l’option `--encryption` en `--encryption-services` pour la commande `az storage account create and az storage account update`
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

```text
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

* Fourniture d’un meilleur message d’erreur pour `cdn endpoint list` quand le profil spécifié par `--profile-name` n’existe pas

### <a name="cloud"></a>Cloud

* Modification de la version de l’API du point de terminaison de métadonnées du cloud au format AAAA-MM-JJ
* Le point de terminaison de la galerie n’est pas nécessaire
* Prise en charge de l’inscription du cloud, avec le point de terminaison ARM resource manager
* Ajout d’une option pour `cloud set` permettant de choisir le profil lors de la sélection du cloud actuel
* Exposé `endpoint_vm_image_alias_doc`

### <a name="cosmosdb"></a>CosmosDB

* Correction relative à la permission de la création de collection avec une clé de partition personnalisée
* Ajout de la prise en charge de la durée de vie par défaut de la collection

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
* Correction d’un problème à cause duquel `cmss create` avec un équilibreur de charge existant exigeait `--backend-pool-name`
* Les disques de données créés avec le numéro d’unité logique `vm image create` commencent à 0


## <a name="may-10-2017"></a>10 mai 2017

Version 2.0.6

* documentdb renommé en cosmosdb
* Ajouter rdbms (mysql, postgres)
* Inclure les modules Data Lake Analytics et Data Lake Store
* Inclure le module Cognitive Services
* Inclure le module Service Fabric
* Inclure le module Interactive (az-shell renommé)
* Ajouter la prise en charge des commandes CDN
* Supprimer le module Container
* Ajouter « az -v » comme raccourci pour « az --version » ([#2926](https://github.com/Azure/azure-cli/issues/2926))
* Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))

```text
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

* Renommer le module documentdb en cosmosdb
* Prise en charge ajoutée pour les API de plan de données documentdb : gestion de base de données et de collecte
* Prise en charge ajoutée pour activer le basculement automatique sur les comptes de base de données
* Prise en charge ajoutée pour la nouvelle stratégie de cohérence ConsistentPrefix

### <a name="data-lake-analytics"></a>Data Lake Analytics

* Corriger un bogue dans lequel le filtrage sur le résultat et l’état des listes de travaux lève une erreur
* Ajouter la prise en charge d’un nouveau type d’élément de catalogue : paquet. accessible via : `az dla catalog package`
* A rendu possible le fait de répertorier les éléments de catalogue suivants à partir d’une base de données (aucune spécification de schéma requise) :

  * Table
  * Fonction table
  * Affichage
  * Statistiques de table. Cela peut également être répertorié avec un schéma, mais sans spécifier un nom de table

### <a name="data-lake-store"></a>Data Lake Store

* Mettre à jour la version du Kit de développement logiciel (SDK) du système de fichiers sous-jacent, qui offre une meilleure prise en charge pour gérer les scénarios de limitation côté serveur
* Améliorer les performances de chargement de paquet et d’exécution de commande ([#2819](https://github.com/Azure/azure-cli/issues/2819))
* aide manquante pour afficher l’accès. ajout en cours. ([#2743](https://github.com/Azure/azure-cli/issues/2743))

### <a name="find"></a>Rechercher

* résultats de la recherche améliorés et autorisation du contrôle de version de l’index de recherche

### <a name="keyvault"></a>KeyVault

* BC : `az keyvault certificate download` remplacer -e dans chaîne ou élément binaire par PEM ou DER afin de mieux représenter les options
* BC : Supprimer --expires et --not-before dans `keyvault certificate create` car ces paramètres ne sont pas pris en charge par le service
* Ajoute le paramètre --validity à `keyvault certificate create` pour substituer de manière sélective la valeur dans --policy
* Résout le problème dans `keyvault certificate get-default-policy` où « expires » et « not_before » étaient exposés mais « validity_in_months » ne l’était pas
* correction de keyvault pour l’importation de pem et pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))

### <a name="lab"></a>Laboratoire

* Ajout des commandes créer, afficher, supprimer et liste pour l’environnement dans le laboratoire
* Ajout des commandes afficher et liste pour afficher les modèles ARM dans le laboratoire
* Ajout de l’indicateur --environment dans `az lab vm list` pour filtrer les machines virtuelles selon l’environnement du laboratoire
* Ajout de la commande pratique `az lab formula export-artifacts` pour exporter une structure d’artefact dans une formule de laboratoire
* Ajout de commandes pour gérer les secrets dans un laboratoire

### <a name="monitor"></a>Surveiller

* Correction de bogue : modélisation `--actions` de `az alert-rules create` pour consommer la chaîne JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))
* Correction de bogue : la création de paramètres de diagnostic n’accepte pas les métriques/journaux à partir des commandes d’affichage ([#2913](https://github.com/Azure/azure-cli/issues/2913))

### <a name="network"></a>Réseau

* Ajouter la commande `network watcher test-connectivity`
* Ajouter la prise en charge du paramètre `--filters` pour `network watcher packet-capture create`
* Ajouter la prise en charge pour le drainage de connexion Application Gateway
* Ajouter la prise en charge pour la configuration du jeu de règles WAF d’Application Gateway
* Ajouter la prise en charge des règles et des filtres de routage ExpressRoute
* Ajouter la prise en charge pour le routage géographique TrafficManager
* Ajouter la prise en charge des sélecteurs de trafic basés sur la stratégie de connexion VPN
* Ajouter la prise en charge pour les stratégies IPSec de la connexion VPN
* Corriger le bogue avec `vpn-connection create` lors de l’utilisation des paramètres `--no-wait` ou `--validate`
* Ajouter la prise en charge des passerelles de réseau virtuel actif-actif
* Supprimer les valeurs NULL de la sortie des commandes `network vpn-connection list/show`
* BC : résoudre un bogue dans la sortie de `vpn-connection create`
* Corriger le bogue où l’argument « --key-length » de « vpn-connection create » n’était pas analysé correctement
* Corriger le bogue dans `dns zone import` où les enregistrements n’étaient pas été importés correctement
* Corriger le bogue où `traffic-manager endpoint update` ne fonctionnait pas
* Ajouter des commandes d’aperçu « network watcher »

### <a name="profile"></a>Profil

* Prendre en charge la connexion lorsqu’il n’y a aucun abonnement trouvé ([#2560](https://github.com/Azure/azure-cli/issues/2560))
* Prendre en charge un nom de paramètre court dans le jeu de comptes az --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))

### <a name="redis"></a>Redis

* Ajout d’une commande de mise à jour qui ajoute également la possibilité de mettre à l’échelle pour le cache redis
* Commande « update-settings » déconseillée

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

* Ajout des commandes az sql server list-usages et az sql db list-usages
* SQL : possibilité de se connecter directement au fournisseur de ressources ([#2832](https://github.com/Azure/azure-cli/issues/2832))

### <a name="storage"></a>Stockage

* Définir l’emplacement par défaut sur l’emplacement du groupe de ressources pour `storage account create`
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

Nous avons publié les composants ACR, Batch, KeyVault et SQL dans cette version

```text
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

* Ajout des modules acr, lab, monitor et find à la liste par défaut
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

* Version initiale du module Data Lake Analytics
* Version initiale du module Data Lake Store

### <a name="docuemntdb"></a>DocumentDB

* DocumentDB : ajout de la prise en charge de l’énumération des chaînes de connexion ([#2580](https://github.com/Azure/azure-cli/pull/2580))

### <a name="vm"></a>Machine virtuelle

* [Compute] Ajout de la prise en charge d’AppGateway à la création de groupe de machines virtuelles identiques ([#2570](https://github.com/Azure/azure-cli/pull/2570))
* [VM/VMSS] Amélioration de la prise en charge de la mise en cache de disque ([#2522](https://github.com/Azure/azure-cli/pull/2522))
* VM/VMSS : intégration de la logique de validation des informations d’identification utilisée par le portail ([#2537](https://github.com/Azure/azure-cli/pull/2537))
* Ajout de la prise en charge des commandes wait et de --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))
* Groupe de machines virtuelles identiques : prise en charge de * pour énumérer les vues d’instance parmi les machines virtuelles ([#2467](https://github.com/Azure/azure-cli/pull/2467))
* Ajout --secrets pour machine virtuelle et groupe de machines virtuelles identiques ([#2212}(https://github.com/Azure/azure-cli/pull/2212))
* Autorisation de la création de machines virtuelles avec un disque dur virtuel spécialisé ([#2256](https://github.com/Azure/azure-cli/pull/2256))

## <a name="february-27-2017"></a>27 février 2017

Version 2.0.0

Cette version d’Azure CLI 2.0 est la première instance mise à la disposition générale. La disponibilité générale s’applique à ces modules de commande :
- Container Service (acs)
- Compute (notamment Resource Manager, machine virtuelle, groupes de machines virtuelles identiques, Managed Disks)
- Réseau
- Stockage

Ces modules de commande, pouvant être utilisés en production, sont pris en charge par le contrat de niveau de service (SLA) Microsoft standard. Vous pouvez ouvrir des incidents directement auprès du support technique Microsoft ou dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/). Vous pouvez poser des questions sur [StackOverflow à l’aide du mot-clé azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), ou contacter l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Vous pouvez fournir des commentaires à partir de la ligne de commande avec la commande `az feedback`.

Les commandes de ces modules sont stables et il n’est pas prévu que la syntaxe change dans les mises à jour ultérieures de cette version d’Azure CLI.

Pour vérifier la version de l’interface CLI, utilisez `az --version`. La sortie indique la version de l’interface CLI proprement dite (2.0.0 dans cette version), les différents modules de commande et les versions de Python et de GCC que vous utilisez.

```text
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
> Certains de ces modules de commande présentent un suffixe « b*n* » ou « rc*n* ». Ces modules de commande, encore en préversion, seront mis à la disposition générale à l’avenir.

Nous avons également des versions d’évaluation nocturnes de l’interface CLI. Pour plus d’informations, consultez ces instructions sur l’[obtention des builds nocturnes](https://github.com/Azure/azure-cli#nightly-builds), ainsi que ces instructions sur [la contribution au code et la configuration d’un environnement de développement](https://github.com/Azure/azure-cli#developer-setup).

Vous pouvez signaler des problèmes liés aux versions d’évaluation nocturnes comme suit :
- Signalez des problèmes dans notre [liste d’incidents github](https://github.com/azure/azure-cli/issues/)
- Contactez l’équipe produit à l’adresse [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).
- Fournissez des commentaires à partir de la ligne de commande avec la commande `az feedback`.

