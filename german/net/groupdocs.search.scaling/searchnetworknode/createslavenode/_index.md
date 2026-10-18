---
title: "CreateSlaveNode"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Erstellt einen Slave-Knoten des Suchnetzwerks."
type: docs
weight: 20
url: /de/net/groupdocs.search.scaling/searchnetworknode/createslavenode/
---
## CreateSlaveNode(int, string, INetworkSettings) {#createslavenode}

Erstellt einen Slave-Knoten des Suchnetzwerks.

```csharp
public static SearchNetworkNode CreateSlaveNode(int nodeIndex, string storagePath, 
    INetworkSettings networkSettings)
```

| Parameter | Type | Beschreibung |
| --- | --- | --- |
| nodeIndex | Int32 | Der Knotenindex. |
| storagePath | String | Der Speicherpfad. |
| networkSettings | INetworkSettings | Die Netzwerkeinstellungen. |

### Rückgabewert

Der Slave-Knoten.

### Siehe auch

* interface [INetworkSettings](../../../groupdocs.search.scaling.configuring/inetworksettings)
* class [SearchNetworkNode](../../searchnetworknode)
* namespace [GroupDocs.Search.Scaling](../../../groupdocs.search.scaling)
* assembly [GroupDocs.Search](../../../)

---

## CreateSlaveNode(int, string, INetworkSettings, ILogger) {#createslavenode_1}

Erstellt einen Slave-Knoten des Suchnetzwerks.

```csharp
public static SearchNetworkNode CreateSlaveNode(int nodeIndex, string storagePath, 
    INetworkSettings networkSettings, ILogger logger)
```

| Parameter | Type | Beschreibung |
| --- | --- | --- |
| nodeIndex | Int32 | Der Knotenindex. |
| storagePath | String | Der Speicherpfad. |
| networkSettings | INetworkSettings | Die Netzwerkeinstellungen. |
| logger | ILogger | Der Logger. |

### Rückgabewert

Der Slave-Knoten.

### Siehe auch

* interface [INetworkSettings](../../../groupdocs.search.scaling.configuring/inetworksettings)
* interface [ILogger](../../../groupdocs.search.common/ilogger)
* class [SearchNetworkNode](../../searchnetworknode)
* namespace [GroupDocs.Search.Scaling](../../../groupdocs.search.scaling)
* assembly [GroupDocs.Search](../../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
