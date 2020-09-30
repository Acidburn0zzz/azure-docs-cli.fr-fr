---
title: Références Azure CLI pour Azure Network
description: Page de destination des références Azure CLI pour Azure Network
author: dbradish-microsoft
manager: barbkess
ms.devlang: azurecli
ms.topic: reference
ms.date: 06/30/2020
ms.author: dbradish
ms.service: azure-cli
ms.reviewer: mohnader
ms.custom: devx-track-azurecli
ms.openlocfilehash: 2155be0bca6b6aa297e4be07a685a379892523c6
ms.sourcegitcommit: 5d29362589078b66d15f5cd494fe903a5195658d
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/25/2020
ms.locfileid: "91225913"
---
# <a name="azure-cli-for-azure-network"></a>Azure CLI pour Azure Network

L'interface de ligne de commande Azure ([Azure CLI](./what-is-azure-cli.md)) est un ensemble de commandes utilisées pour créer et gérer des ressources Azure.  L’interface de ligne de commande est disponible dans de nombreux services Azure, dont Azure Network, ce qui vous permet de gérer les services de mise en réseau à partir d’une ligne de commande.

## <a name="references-for-azure-network"></a>Références pour Azure Network

L’expérience d’interface de ligne de commande Azure Network est composée de deux parties : **principale** et **extension**.  Les commandes d’interface de ligne de commande Azure principales sont fournies dans le cadre de l’interface CLI et sont entièrement prises en charge.  Une extension vous donne accès à des commandes expérimentales et disponibles en préversion, et doit être installée avant d’être utilisée.  Des exemples de scripts d’installation sont fournis dans [Installation des références d’extension](#installing-extension-references).

Pour obtenir la liste complète des références principales d’interface de ligne de commande Azure pour Azure Network, consultez [az network](/cli/azure/network).  Suivez les liens ci-dessous pour les références d’extension.

### <a name="virtual-network"></a>Réseau virtuel

| Sous-groupe | Informations de référence | Utilisation | Est une extension
|-|-|-|-|
| Appliance | [az network virtual-appliance](/cli/azure/network/virtual-appliance) | Gérer l’appliance virtuelle Azure Network.
| DNS | [az network private-dns](/cli/azure/network/private-dns) | Gérer les domaines DNS privés dans Azure. |
| Point de terminaison | [az network service-endpoint](/cli/azure/network/service-endpoint) | Gérer les stratégies liées aux points de terminaison de service. |
| NAT | [az network nat](/cli/azure/network/nat) | Gérer les ressources de traduction d’adresses réseau. |
| Carte d’interface réseau | [az network nic](/cli/azure/network/nic) | Gérer des interfaces réseau. |
| Peering | [az peering](/cli/azure/ext/peering/peering) | Gérer le peering. | Oui
| Profil | [az network profile](/cli/azure/network/profile) | Gérer les profils réseau. |
| Routage | [az network route-filter](/cli/azure/network/route-filter) | Gérer les filtres de routage. |
| Routage | [az network route-table](/cli/azure/network/route-table) | Gérer les tables de routage. |
| VMware | [az network vmware](/cli/azure/ext/vmware/vmware) | Commandes pour gérer Azure VMware Solutions. | Oui
| Réseau virtuel | [az network vnet](/cli/azure/network/vnet) | Gérer les réseaux virtuels Azure. |
| Réseau virtuel | [az network vnet-tap](/cli/azure/ext/virtual-network-tap/network/vnet/tap) | Gérer les taps de réseau virtuel. | Oui
| Réseau virtuel | [az network vnet-gateway](/cli/azure/network/vnet-gateway) | Utiliser une passerelle de réseau virtuel Azure pour établir une connectivité entre sites sécurisée. |

### <a name="wan-and-on-premise-connectivity"></a>Connectivité WAN et locale

| Sous-groupe | Informations de référence | Utilisation | Est une extension
|-|-|-|-|
| Connexion croisée | [az network cross-connection](/cli/azure/ext/express-route-cross-connection/network/cross-connection) | Gérer les ressources Azure Network. | Oui
| ExpressRoute | [az network express-route](/cli/azure/network/express-route) | Gérer les hubs Azure IoT. |
| vHub | [az network vhub](/cli/azure/ext/virtual-wan/network/vhub) | Gérer les hubs virtuels. | Oui
| VPN | [az network vpn-connection](/cli/azure/network/vpn-connection) | Gérer les connexions VPN. |
| VPN | [az network vpn-gateway](/cli/azure/ext/virtual-wan/network/vpn-gateway) | Gérer les passerelles VPN. | Oui
| VPN | [az network vpn-site](/cli/azure/ext/virtual-wan/network/vpn-site) | Gérer les configurations de site VPN. | Oui
| vRouter | [az network vrouter](/cli/azure/network/vrouter) | Gérer le routeur virtuel. |
| vWAN | [az network vwan](/cli/azure/ext/virtual-wan/network/vwan) | Gérer des WAN virtuels. | Oui

### <a name="load-balancing-and-ip"></a>Équilibrage de charge et adresses IP

| Sous-groupe | Informations de référence | Utilisation | Est une extension
|-|-|-|-|
| Application Gateway | [az network application-gateway](/cli/azure/network/application-gateway) | Gérer les services de routage et d’équilibrage de charge au niveau de l’application. |
| Équilibrer la charge | [az network lb](/cli/azure/network/lb) | Gérer et configurer les équilibreurs de charge. |
| IP | [az network ip-group](/cli/azure/ext/ip-group/network/ip-group) | Gérer les ipGroups. | Oui
| IP | [az network public-ip](/cli/azure/network/public-ip) | Gérer les adresses IP publiques. |
| Front Door | [az network front-door](/cli/azure/ext/front-door/network/front-door) | Gérer les ressources Front Door de mise en réseau. | Oui
| Passerelle locale | [az network local-gateway](/cli/azure/network/local-gateway) | Gérer les passerelles locales. |
| Traffic Manager | [az network traffic-manager](/cli/azure/network/traffic-manager) | Gérer le routage du trafic entrant. |

### <a name="security"></a>Sécurité

| Sous-groupe | Informations de référence | Utilisation | Est une extension
|-|-|-|-|
| ASG | [az asg](/cli/azure/network/asg) | Gérer les groupes de sécurité d’application. |
| Bastion | [az network bastion](/cli/azure/network/bastion) | Gérer l’hôte bastion Azure. |
| DDoS | [az network ddos-protection](/cli/azure/network/ddos-protection) | Gérer les plans de protection DDoS. |
| Pare-feu | [az network firewall](/cli/azure/ext/azure-firewall/network/firewall) | Gérer et configurer les pare-feu Azure. | Oui
| Pare-feu | [az network security-partner-provider](/cli/azure/network/security-partner-provider) | Gérer un fournisseur de partenaire de sécurité Azure. |
| Groupe de sécurité réseau | [az network nsg](/cli/azure/network/nsg)| Gérer les groupes de sécurité réseau Azure. |
| Point de terminaison privé | [az network private-endpoint](/cli/azure/network/private-endpoint) | Gérer les points de terminaison privés. |
| Point de terminaison privé | [az network private-endpoint-connection](/cli/azure/network/private-endpoint-connection) | Gérer les connexions de point de terminaison privé. |
| Liaison privée | [az network private-link-resource](/cli/azure/network/private-link-resource) | Gérer les ressources de liaison privée. |
| Liaison privée | [az network private-link-service](/cli/azure/network/private-link-service) | Gérer les services de liaison privée. |

### <a name="monitoring"></a>Supervision

| Sous-groupe | Informations de référence | Utilisation | Est une extension
|-|-|-|-|
| Observateur | [az network watcher](/cli/azure/network/watcher) | Gérer Azure Network Watcher. |

### <a name="list"></a>List

| Sous-groupe | Informations de référence | Utilisation | Est une extension
|-|-|-|-|
| Service | [az network list-service-aliases](/cli/azure/network#az-network-list-service-aliases) | Lister les alias de service disponibles dans la région qui peuvent être utilisés pour les stratégies de point de terminaison de service. |
| Service | [az network list-service-tags](/cli/azure/network#az-network-list-service-tags) | Lister toutes les étiquettes de service qui appartiennent à des ressources différentes. |
| Usage | [az network list-usages](/cli/azure/network#az-network-list-usages) | Lister le nombre de ressources réseau dans une région utilisées par rapport à un quota d’abonnement. |

## <a name="installing-extension-references"></a>Installation des références d’extension

Les références d’extension Azure CLI doivent être installées avant d’être utilisées.  La commande [az extension add](./azure-cli-extensions-overview.md) installe une référence d’extension par nom.  Découvrez-en plus sur les références des extensions dans [Utiliser des extensions avec Azure CLI](./azure-cli-extensions-overview.md).

```azurecli
## get a list of available Azure CLI extensions
az extension list-available --output table

# install the extension for az network express-route-cross-connection
az extension add --name express-route-cross-connection

# install the extension for az network front-door
az extension add --name front-door

# install the extension for az network virtual-wan
az extension add --name virtual-wan

# install the extension for az network vm-repair
az extension add --name virtual-network-tap

# install the extension for az network vmware
az extension add --name vmware

# install the extension for az peering
az extension add --name peering
```

## <a name="popular-network-articles-using-the-azure-cli"></a>Articles Azure Network populaires utilisant l’interface Azure CLI

- [Créer des machines virtuelles](/cli/azure/azure-cli-vm-tutorial)
- [Création d'un réseau virtuel](/azure/virtual-network/quick-create-cli)
- [Exemples Azure CLI pour machines virtuelles Windows](/azure/virtual-machines/windows/cli-samples?toc=%2Fcli%2Fazure%2Ftoc.json&bc=%2Fcli%2Fazure%2Fbreadcrumb%2Ftoc.json)
- [Créer un groupe de machines virtuelles identiques](/azure/virtual-machine-scale-sets/quick-create-cli)
- [Exécuter Azure IoT Edge sur des machines virtuelles Ubuntu](/azure/iot-edge/how-to-install-iot-edge-ubuntuvm#deploy-from-azure-cli)
- [Équilibrer la charge des machines virtuelles Linux dans Azure](/azure/virtual-machines/linux/tutorial-load-balancer)
- [Créer et gérer des réseaux virtuels Azure pour des machines virtuelles Linux](/azure/virtual-machines/linux/tutorial-virtual-network)
- [Configurer un point de terminaison de service pour Cosmos DB](/azure/cosmos-db/how-to-configure-vnet-service-endpoint#configure-using-cli)

## <a name="see-also"></a>Voir aussi

- [Prise en main d'Azure CLI](./get-started-with-azure-cli.md) pour en savoir plus sur l'installation et la connexion.

- Découvrez des références [principales](/cli/azure/reference-index) et [d'extension](./azure-cli-extensions-list.md) supplémentaires dans la documentation Azure CLI.

- Gérer des machines virtuelles Linux ou Windows avec [az vm](/cli/azure/vm).