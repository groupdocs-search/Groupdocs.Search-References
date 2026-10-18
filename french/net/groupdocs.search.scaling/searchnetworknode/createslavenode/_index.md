---
title: "CreateSlaveNode"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Crée un nœud esclave du réseau de recherche."
type: docs
weight: 20
url: /fr/net/groupdocs.search.scaling/searchnetworknode/createslavenode/
---
## CreateSlaveNode(int, string, INetworkSettings) {#createslavenode}

Crée un nœud esclave du réseau de recherche.

```csharp
public static SearchNetworkNode CreateSlaveNode(int nodeIndex, string storagePath, 
    INetworkSettings networkSettings)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| nodeIndex | Int32 | L'index du nœud. |
| storagePath | String | Le chemin de stockage. |
| networkSettings | INetworkSettings | Les paramètres du réseau. |

### Valeur de retour

Le nœud esclave.

### Voir aussi

* interface [INetworkSettings](../../../groupdocs.search.scaling.configuring/inetworksettings)
* class [SearchNetworkNode](../../searchnetworknode)
* namespace [GroupDocs.Search.Scaling](../../../groupdocs.search.scaling)
* assembly [GroupDocs.Search](../../../)

---

## CreateSlaveNode(int, string, INetworkSettings, ILogger) {#createslavenode_1}

Crée un nœud esclave du réseau de recherche.

```csharp
public static SearchNetworkNode CreateSlaveNode(int nodeIndex, string storagePath, 
    INetworkSettings networkSettings, ILogger logger)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| nodeIndex | Int32 | L'index du nœud. |
| storagePath | String | Le chemin de stockage. |
| networkSettings | INetworkSettings | Les paramètres du réseau. |
| logger | ILogger | Le logger. |

### Valeur de retour

Le nœud esclave.

### Voir aussi

* interface [INetworkSettings](../../../groupdocs.search.scaling.configuring/inetworksettings)
* interface [ILogger](../../../groupdocs.search.common/ilogger)
* class [SearchNetworkNode](../../searchnetworknode)
* namespace [GroupDocs.Search.Scaling](../../../groupdocs.search.scaling)
* assembly [GroupDocs.Search](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
