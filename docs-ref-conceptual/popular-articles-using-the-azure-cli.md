---
title: Liens entre les services pour une utilisation avec l’interface Azure CLI
description: Liens vers des tutoriels populaires, des guides de démarrage rapide, des exemples, des concepts et des guides de procédures, Azure CLI, des machines virtuelles, Azure Kubernetes Service (AKS), Batch, Azure CLI (Core), Azure Resource Manager, Key Vault, Azure Stack Hub, Functions, Database, Event Hubs, App Configuration, App Config, , Allemagne, Sécurité, Gouvernance, Insights, IoT, Internet des objets, DevOps, Réseau Virtuel, Compute, Networking, Outils de développement, Bases de données, Analytique, Gestion et gouvernance, Hybride, Stockage, Sécurité, IA, IA + Machine Learning, Linux, Windows, Ubuntu, Automation, application, application web, script
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 03/01/2020
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: 42e9de630530568a15bc6f9f05d2442d790d8b68
ms.sourcegitcommit: 2da241715d25407ed22c1065c0c793acfd865996
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/09/2020
ms.locfileid: "89563142"
---
# <a name="popular-articles-using-the-azure-cli"></a>Articles populaires utilisant l’interface Azure CLI

L’interface Azure CLI est utilisée dans de nombreux services Azure, ce qui donne lieu à la diffusion d’articles dans les référentiels de documents.  Cette page fournit des liens permettant de sélectionner des articles populaires.  

## <a name="compute"></a>Calcul

| | | | |
|-|-|-|-|
|Machines Virtuelles | Tutoriel : Linux | [Créer une machine virtuelle Linux avec Azure CLI](azure-cli-vm-tutorial.yml) | Création d’une machine virtuelle  Découvrez les requêtes de sortie et la définition de variables d’environnement.
|Virtual Machines | Démarrage rapide : Linux | [Créer une machine virtuelle Linux en utilisant Azure CLI](/azure/virtual-machines/linux/quick-create-cli) | Créez et déployez une machine virtuelle Linux.  Ouvrez un port pour le trafic web et installez un serveur web.
|Virtual Machines | Guide pratique : Linux |[Créer une image Linux d’une machine virtuelle ou d’un disque dur virtuel](/azure/virtual-machines/linux/capture-image) | Déprovisionnez une machine virtuelle existante, créer une image, puis créez une nouvelle machine virtuelle à partir de l’image capturée.
|Virtual Machines | Guide pratique : Linux | [Charger un disque dur virtuel sur Azure à l’aide d’Azure CLI](/azure/virtual-machines/linux/disks-upload-vhd-to-managed-disk-cli) | Créez un disque managé vide, chargez votre fichier VHD local, puis copiez un disque managé.
|Virtual Machines | Guide pratique : Linux | [Créer une galerie d’images partagées à l’aide d’Azure CLI](/azure/virtual-machines/linux/shared-images) | Créez une galerie d’images partagées contenant des images de machine virtuelle personnalisées avec d’autres personnes de votre organisation, dans ou entre différentes régions, ou dans un locataire Azure Active Directory.
|Virtual Machines | Guide pratique : Linux | [Déployer des machines virtuelles Spot avec Azure CLI (préversion)](/azure/virtual-machines/linux/spot-cli) | Déployez une machine virtuelle Spot Linux qui ne sera pas supprimée en fonction du prix.
|Virtual Machines | Démarrage rapide : Windows | [Créer une machine virtuelle Windows à l’aide d’Azure CLI](/azure/virtual-machines/windows/quick-create-cli) | Déployez dans Azure une machine virtuelle qui exécute Windows Server 2016.
|Virtual Machines | Module d’apprentissage | [Gérer des machines virtuelles à l’aide d’Azure CLI](https://docs.microsoft.com/learn/modules/manage-virtual-machines-with-azure-cli/) | Créez, démarrez, arrêtez des machines virtuelles, et effectuez d’autres tâches de gestion liées à ces dernières.
|Azure Kubernetes Service (AKS)| Démarrage rapide | [Déployer un cluster AKS (Azure Kubernetes Service) à l’aide d’Azure CLI](/azure/aks/kubernetes-walkthrough) | Déployez et gérez des clusters AKS.  Découvrez comment superviser l’intégrité du cluster et des pods qui exécutent votre application.
|Azure Batch|Exemple | [Exécuter un travail et des tâches avec Azure Batch à l’aide d’Azure CLI](/azure/batch/scripts/batch-cli-sample-run-job) | Créez un travail Batch et ajoutez une série de tâches au travail. Supervisez un travail et ses tâches.
|Azure Batch|Exemple | [Créer et gérer un pool Windows dans Azure Batch à l’aide d’Azure CLI](/azure/batch/scripts/batch-cli-sample-manage-windows-pool) | Créez et gérez un pool de nœuds de calcul Windows avec une configuration des services cloud.
|Azure Container Instance|Démarrage rapide | [Déployer un instance de conteneur à l’aide d’Azure CLI](/azure/container-instances/container-instances-quickstart) | Déployez un conteneur Docker isolé et mettez son application à disposition avec un nom de domaine complet (FQDN). Exécutez une seule commande de déploiement, puis accédez à l’application en cours d’exécution dans le conteneur.
|Fonction Azure|Démarrage rapide |  [Créer dans Azure une fonction qui répond à des requêtes HTTP à l’aide d’Azure CLI](/azure/azure-functions/functions-create-first-azure-function-azure-cli) | Utilisez des outils en ligne de commande pour créer une fonction qui répond à des requêtes HTTP. Après avoir testé le code localement, déployez la fonction dans l’environnement serverless d’Azure Functions.

## <a name="networking"></a>Mise en réseau

| | | | |
|-|-|-|-|
|Réseau virtuel|Démarrage rapide | [Créer un réseau virtuel à l’aide d’Azure CLI](/azure/virtual-network/quick-create-cli) | Créez un réseau virtuel, déployez deux machines virtuelles dans le réseau virtuel, puis connectez-vous aux machines virtuelles à partir d’Internet.
|Réseau virtuel|Guide pratique | [Activer l’accélération réseau sur une machine virtuelle existante à l’aide d’Azure CLI](/azure/virtual-network/create-vm-accelerated-networking-cli) | Créez une machine virtuelle Linux, gérez la liaison dynamique et la révocation de la fonction virtuelle, puis activez l’accélération réseau.

## <a name="internet-of-things"></a>Internet des Objets

| | | | |
|-|-|-|-|
|IoT Hub|Didacticiel | [Configurer le routage des messages IoT Hub à l’aide d’Azure CLI](/azure/iot-hub/tutorial-routing) | Configurez et utilisez des requêtes de routage personnalisées avec IoT Hub.

## <a name="developer-tools"></a>Outils de développement

| | | | |
|-|-|-|-|
|Azure App Configuration|Exemples |[Exemples Azure CLI pour Azure App Configuration](/azure/azure-app-configuration/cli-samples) | Obtenez des liens vers des scripts Bash qui utilisent l’interface Azure CLI pour Azure App Configuration.
|Azure DevOps| Bien démarrer : Pipeline DevOps |[Créer votre premier pipeline Azure à l’aide d’Azure CLI](/azure/devops/pipelines/create-first-pipeline-cli) | Créez un pipeline dans un répertoire GitHub cloné, et gérez et exécutez vos pipelines.
|Azure DevOps| Guide pratique : Pipeline DevOps |[Tâches de déploiement de pipeline Azure à l’aide d’Azure CLI](/azure/devops/pipelines/tasks/deploy/azure-cli?view=azure-devops) | Dans un pipeline de build ou de mise en service, exécutez un script shell ou de commandes par lot contenant Azure CLI.  Les commandes s’exécutent sur des agents multiplateformes qui, eux-mêmes, s’exécutent sur des systèmes d’exploitation Linux, macOS ou Windows.
|Azure DevOps| Tutoriel : Pipeline Jenkins |[Déployer dans Azure App Service avec Jenkins à l’aide d’Azure CLI](/azure/jenkins/execute-cli-jenkins-pipeline) | Créez et configurez une machine virtuelle Jenkins, créez une application web dans Azure, puis préparez un dépôt GitHub.  Créez et exécutez le pipeline Jenkins.

## <a name="databases"></a>Bases de données

| | | | |
|-|-|-|-|
|SQL Database| Exemple |[Configurer Azure SQL Database à l’aide d’Azure CLI](/azure/sql-database/sql-database-cli-samples?tabs=single-database) | Exemples Azure CLI pour Azure SQL Database.
|MySQL|Démarrage rapide |[Créer un serveur Azure Database pour MySQL à l’aide d’Azure CLI](/azure/mysql/quickstart-create-mysql-server-database-using-azure-cli) | Créez un serveur de base de données Azure pour MySQL.  Configurez une règle de pare-feu et des paramètres SL.  Obtenez et utilisez des informations de connexion.
|Cosmos DB |Guide pratique |[Gérer les ressources Azure Cosmos à l’aide d’Azure CLI](/azure/cosmos-db/manage-with-cli) | Utilisez des commandes courantes pour automatiser la gestion de vos comptes, bases de données et conteneurs Azure Cosmos DB.
|Cosmos DB |Exemple |[Exemples Azure CLI pour l’API SQL (Core) Azure Cosmos DB](/azure/cosmos-db/cli-samples) | Obtenez des liens vers des exemples de scripts Azure CLI pour l’API SQL (Core) Azure Cosmos DB.

## <a name="analytics"></a>Analytics

| | | | |
|-|-|-|-|
Azure Event Hub |Démarrage rapide |[Créer un hub d’événements à l’aide d’Azure CLI](/azure/event-hubs/event-hubs-quickstart-cli) | Créez un espace de noms Event Hubs et un hub d’événements.
HDInsight |Guide pratique |[Créer des clusters HDInsight à l’aide de l’interface de ligne de commande Azure](/azure/hdinsight/hdinsight-hadoop-create-linux-clusters-azure-cli) | Créez un cluster HDInsight 3.6.
HDInsight |Didacticiel |[Gérer des clusters Azure HDInsight à l’aide d’Azure CLI](/azure/hdinsight/hdinsight-administer-use-command-line) | Listez, affichez, supprimez et mettez à l’échelle des clusters HDInsight.

## <a name="management-and-governance"></a>Gestion et gouvernance

| | | | |
|-|-|-|-|
Modèles de Gestionnaire des ressources |Guide pratique |[Déployer des ressources avec des modèles Azure Resource Manager et Azure CLI](/azure/azure-resource-manager/templates/deploy-cli) | Déployez vos ressources dans Azure à l’aide de modèles.
Groupes Resource Manager |Guide pratique |[Gérer des groupes de ressources Azure Resource Manager à l’aide d’Azure CLI](/azure/azure-resource-manager/management/manage-resource-groups-cli) | Utilisez Azure Resource Manager pour gérer vos groupes de ressources Azure.
Resource Graph |Démarrage rapide |[Exécuter votre première requête Resource Graph à l’aide d’Azure CLI](/azure/governance/resource-graph/first-query-azurecli) | Ajoutez Azure Resource Graph à votre installation d’Azure CLI, puis exécutez votre première requête Resource Graph.
Attribution de stratégie |Démarrage rapide |[Créer une attribution de stratégie pour identifier les ressources non conformes à l’aide d’Azure CLI](/azure/governance/policy/assign-policy-azurecli) | Créez une attribution de stratégie pour identifier les machines virtuelles qui n’utilisent pas de disques managés.

## <a name="hybrid"></a>Hybride

| | | | |
|-|-|-|-|
Azure Stack Hub| Démarrage rapide : Machine virtuelle Linux |[Créer une machine virtuelle de serveur Linux dans Azure Stack Hub à l’aide d’Azure CLI](/azure-stack/user/azure-stack-quick-create-vm-linux-cli) | Créez une machine virtuelle Ubuntu Server 16.04 LTS, connectez-vous à la machine virtuelle avec un client distant, puis installez un serveur web NGINX.
Azure Stack Hub| Démarrage rapide : Machine virtuelle Windows |[Créer une machine virtuelle Windows Server dans Azure Stack Hub à l’aide d’Azure CLI](/azure-stack/user/azure-stack-quick-create-vm-windows-cli) |Créez une machine virtuelle Windows Server 2016, connectez la machine virtuelle avec un client distant, puis installez un serveur web IIS.
Azure Stack Hub| Guide pratique : Ressources ASDK |[Gérer et déployer des ressources sur Azure Stack Hub à l’aide d’Azure CLI](/azure-stack/user/azure-stack-version-profiles-azurecli2) | Configurez l’interface de ligne de commande (CLI) Azure pour gérer les ressources du Kit de développement Azure Stack (ASDK) à partir des plateformes clientes Linux, Mac et Windows.

## <a name="storage"></a>Stockage

| | | | |
|-|-|-|-|
Stockage d’objets BLOB |Démarrage rapide |  [Créer, charger et lister des objets blob à l’aide d’Azure CLI](/azure/storage/blobs/storage-quickstart-blobs-cli) | Chargez et téléchargez des données vers et depuis le Stockage Blob Azure.
Stockage d’objets BLOB |Guide pratique |[Autoriser l’accès à des données d’objet blob ou de file d’attente à l’aide d’Azure CLI](/azure/storage/common/authorize-data-operations-cli) | Spécifiez la façon dont les opérations de données sont autorisées et définissez des variables d’environnement pour les paramètres.
Stockage d’objets BLOB |Guide pratique |[Utiliser Azure CLI pour gérer des répertoires, des fichiers et des listes de contrôle d’accès dans Azure Data Lake Storage Gen2 (préversion)](/azure/storage/blobs/data-lake-storage-directory-file-acl-cli) | Créez et gérez des répertoires, des fichiers et des autorisations dans des comptes de stockage dotés d’un espace de noms hiérarchique.
Stockage Fichier |Démarrage rapide |[Créer et gérer des partages de fichiers Azure à l’aide d’Azure CLI](/azure/storage/files/storage-how-to-use-files-cli) | Créez et utilisez des partages de fichiers Azure.  Créez et gérez des captures instantanées de partage.

## <a name="security"></a>Sécurité

| | | | |
|-|-|-|-|
Principal du service |Guide pratique |[Créer un principal du service Azure à l’aide d’Azure CLI](/cli/azure/create-an-azure-service-principal-azure-cli) | Créez un principal de service, obtenez les informations s’y rapportant et réinitialisez-le avec Azure CLI.
RBAC |Guide pratique |[Ajouter ou supprimer des attributions de rôles avec le contrôle d’accès en fonction du rôle (RBAC) Azure et Azure CLI](/azure/role-based-access-control/role-assignments-cli) | Attribuez des rôles au contrôle d’accès en fonction du rôle Azure.
Key Vault |Guide pratique |[Gérer Key Vault à l’aide de l’interface de ligne de commande Azure](/azure/key-vault/key-vault-manage-with-cli2) | Créez et gérez Azure Key Vault.  Inscrivez et autorisez une application, définissez des stratégies d’accès avancées et découvrez les commandes d’interface de ligne de commande multiplateformes.
Key Vault |Didacticiel |[Gérer les clés de compte de stockage avec Key Vault et l’interface de ligne de commande Azure](/azure/key-vault/key-vault-ovw-storage-keys) | Gérez les clés de compte de stockage et générez des jetons de signature d’accès partagé.

## <a name="ai--machine-learning"></a>IA + Machine Learning

| | | | |
|-|-|-|-|
Machine Learning |Référence |[Utiliser l’extension Azure CLI pour Azure Machine Learning](/azure/machine-learning/reference-azure-machine-learning-cli) | Exécutez des expériences pour créer et inscrire des modèles Machine Learning à destination des clients.  Empaquetez, déployez et suivez le cycle de vie de vos modèles Machine Learning.
Cognitive Services |Guide pratique |[Créer une ressource Cognitive Services avec Azure CLI](/azure/cognitive-services/cognitive-services-apis-create-account-cli) | Inscrivez-vous à Azure Cognitive Services et créez un compte disposant d’un abonnement monoservice ou multiservice.  Utilisez les clés et le point de terminaison générés automatiquement pour authentifier vos applications.
Azure Monitor |Guide pratique |[Créer un espace de travail Log Analytics dans Azure CLI](/azure/azure-monitor/learn/quick-create-workspace-cli) | Créez et déployez un espace de travail Log Analytics.

## <a name="geographies"></a>Zones géographiques

| | | | |
|-|-|-|-|
Azure Allemagne |Découvrir |[Se connecter à Azure Allemagne à l’aide d’Azure CLI](/azure/germany/germany-get-started-connect-with-cli) | À l’aide d’Azure Allemagne, gérez un grand abonnement par le biais de scripts et accédez à des fonctionnalités qui ne sont actuellement pas disponibles dans le portail Azure global.
Azure Government|Découvrir |[Connexion à Azure Government avec l’interface de ligne de commande Azure](/azure/azure-government/documentation-government-get-started-connect-with-cli)|Accédez à des ressources dans Azure Government et commencez à les gérer.

## <a name="see-also"></a>Voir aussi

* [Prise en main de l’interface Azure CLI](get-started-with-azure-cli.md)
* [Liste de référence complète des commandes pour Azure CLI](/cli/azure/reference-index)
* [Services pouvant être gérés par l’interface Azure CLI](azure-services-the-azure-cli-can-manage.md)
