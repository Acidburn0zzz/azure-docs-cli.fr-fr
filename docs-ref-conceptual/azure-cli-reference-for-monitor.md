---
title: Références Azure CLI pour Azure Monitor
description: Page de destination des références Azure CLI pour Azure Monitor
author: dbradish-microsoft
manager: barbkess
ms.devlang: azurecli
ms.topic: reference
ms.date: 06/30/2020
ms.author: dbradish
ms.service: azure-cli
ms.reviewer: robb
ms.custom: devx-track-azurecli
ms.openlocfilehash: d16c745656b3d92942e66cfbcb6764d219d971ec
ms.sourcegitcommit: 5d29362589078b66d15f5cd494fe903a5195658d
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/25/2020
ms.locfileid: "91225437"
---
# <a name="azure-cli-for-azure-monitor"></a>Azure CLI pour Azure Monitor

L'interface de ligne de commande Azure ([Azure CLI](./what-is-azure-cli.md)) est un ensemble de commandes utilisées pour créer et gérer des ressources Azure.  Elle est disponible sur de nombreux services Azure, notamment Azure Monitor.  Il existe plus de 100 références pour Azure Monitor vous permettant de travailler efficacement avec les services Monitor à partir d’une ligne de commande.

## <a name="references-for-azure-monitor"></a>Références pour Azure Monitor

L’expérience CLI d’[Azure Monitor](/azure/azure-monitor/) est composée de deux parties : Azure CLI (communément appelée **noyau** CLI) et l’**extension** Azure Monitor CLI.  Les références d’extension Azure CLI doivent être installées avant d’être utilisées. La commande [az extension add](/cli/azure/extension?view=azure-cli-latest#az-extension-add) installe une référence d’extension par nom.

> [!IMPORTANT]
>
> Azure Monitor comprend désormais Application Insights et Log Analytics. Vous devez donc installer les extensions pour chaque sous-zone quand vous utilisez l’interface CLI d’Azure Monitor.

### <a name="references"></a>References

| Informations de référence | Installer l’extension | Description | Pour plus d’informations, consultez
|-|-|-|-|
| [az monitor](/cli/azure/monitor) | | Groupe de commandes de niveau supérieur pour toutes les commandes Azure CLI pour Azure Monitor. | [Vue d’ensemble d’Azure Monitor](/azure/azure-monitor/overview)
| [az monitor action-group](/cli/azure/monitor/action-group) | | Gérer les groupes d’actions, qui sont liés aux notifications après le déclenchement d’une alerte. | [Alertes Azure Monitor](/azure/azure-monitor/platform/alerts-overview)
| [az monitor activity-log](/cli/azure/monitor/activity-log) | | Gérer le journal d’activité, notamment les alertes du journal d’activité. | [Journaux d’activité Azure](/azure/azure-monitor/platform/activity-log)
| [az monitor alert](/cli/azure/monitor/alert) | | NE PAS L’UTILISER pour les nouveaux développements.  Cette commande gère les anciennes règles d’alerte basées sur des métriques classiques, qui à part quelques exceptions, ont été migrées vers les types d’alerte de métriques plus récents. Utilisez [az monitor metrics alert](/cli/azure/monitor/metrics/alert) à la place. |
| [az monitor app-insights](/cli/azure/ext/application-insights/monitor/app-insights) | Oui | Gérer Application Insights pour la supervision des applications. | [Vue d’ensemble d’Application Insights](/azure/azure-monitor/app/app-insights-overview)
| [az monitor autoscale](/cli/azure/monitor/autoscale) | | Gérer les paramètres de mise à l’échelle automatique. | [Vue d’ensemble de la mise à l’échelle automatique](/azure/azure-monitor/platform/autoscale-overview)
| [az monitor diagnostic-settings](/cli/azure/monitor/diagnostic-settings) | | Gérer les paramètres de diagnostic de service, qui configurent la collecte et le routage de nombreux types de métriques et de journaux de plateforme. | [Créer des paramètres de diagnostic](/azure/azure-monitor/platform/diagnostic-settings)
| [az monitor log-analytics](/cli/azure/monitor/log-analytics) | | Gérer les clusters de journaux et les espaces de travail. | [Conception de votre déploiement de journaux Azure Monitor](/azure/azure-monitor/platform/design-logs-deployment)
| [az monitor log-analytics query](/cli/azure/ext/log-analytics/monitor/log-analytics#ext-log-analytics-az-monitor-log-analytics-query) | Oui | Commandes permettant d’interroger les données dans des espaces de travail Log Analytics.  | [Bien démarrer avec les requêtes Log Analytics](/azure/azure-monitor/log-query/get-started-portal)
| [az monitor log-profiles](/cli/azure/monitor/log-profiles) | | NE PAS L’UTILISER pour les nouveaux développements.  Cette commande était précédemment utilisée pour router les journaux d’activité vers les journaux Azure Monitor et Log Analytics.  Utilisez les [paramètres de diagnostic](/azure/azure-monitor/platform/diagnostic-settings) à la place.  | [Envoyer le journal d’activité à un espace de travail Log Analytics](/azure/azure-monitor/platform/activity-log#send-to-log-analytics-workspace)
| [az monitor metrics](/cli/azure/monitor/metrics) | | Gérer les métriques de plateforme et les règles d’alerte des métriques en quasi-temps réel. | [Vue d’ensemble des mesures dans Azure Monitor](/azure/azure-monitor/platform/data-platform-metrics) et [Comprendre le fonctionnement des alertes de métrique](/azure/azure-monitor/platform/alerts-metric-overview)
| [az monitor private-link-scope](/cli/azure/monitor/private-link-scope) | | Gérer la ressource d’étendue de liaison privée d’Azure Monitor. | [Utiliser Azure Private Link pour connecter en toute sécurité des réseaux à Azure Monitor](/azure/azure-monitor/platform/private-link-security)

### <a name="installing-extension-references"></a>Installation des références d’extension

Les références d’extension Azure CLI doivent être installées avant d’être utilisées.  La commande [az extension add](./azure-cli-extensions-overview.md) installe une référence d’extension par nom.

```azurecli
# install the extension for az monitor app-insights
az extension add --name application-insights

# install the extension for az monitor log-analytics
az extension add --name log-analytics
```

## <a name="popular-monitor-articles-using-the-azure-cli"></a>Articles Azure Monitor populaires utilisant l’interface Azure CLI

- [Exemples d’interface CLI Azure Monitor](/azure/azure-monitor/samples/cli-samples)
- [Créer un espace de travail Log Analytics avec Azure CLI 2.0](/azure/azure-monitor/learn/quick-create-workspace-cli)

## <a name="azure-cli-reference-examples"></a>Exemples de référence Azure CLI

Des exemples sont fournis avec chaque référence Azure CLI. Vous pouvez également effectuer ces tâches via le portail Azure, mais l'utilisation d'Azure CLI ne nécessite qu'une seule ligne de commande.  Les exemples de code suivants vous donneront une idée de la facilité d’utilisation d’Azure CLI.

Pour utiliser Azure Monitor, vous devez d’abord disposer d’un groupe de ressources.  Les groupes de ressources Azure sont faciles à créer et à gérer avec Azure CLI.  

```azurecli
#create a resource group
az group create -location westus -name MyResourceGroup

#get a list of resource groups for a subscription
az group list --subscription MySubscription --output table
```

La création d’une alerte de journal Azure Monitor est tout aussi simple.

```azurecli
#create an Azure Monitor activity log alert
az monitor activity-log alert create --name MyAlertName --resource-group MyResourceGroup
```

## <a name="see-also"></a>Voir aussi

- [Prise en main d'Azure CLI](./get-started-with-azure-cli.md) pour en savoir plus sur l'installation et la connexion.

- Découvrez des références [publiées](/cli/azure/reference-index) et [d’extension](./azure-cli-extensions-list.md) supplémentaires dans la documentation Azure CLI.

- Découvrez-en plus sur les références des extensions dans [Utiliser des extensions avec Azure CLI](./azure-cli-extensions-overview.md).