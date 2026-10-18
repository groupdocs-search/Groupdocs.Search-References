---
title: "CreateMasterNode"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Erstellt einen Master-Knoten des Suchnetzwerks."
type: docs
weight: 10
url: /de/net/groupdocs.search.scaling/searchnetworknode/createmasternode/
---
## SearchNetworkNode.CreateMasterNode method

Erstellt einen Master-Knoten des Suchnetzwerks.

```csharp
public static SearchNetworkNode CreateMasterNode(int nodeIndex, string storagePath, 
    INetworkSettings networkSettings, ILogger logger, Configuration configuration)
```

| Parameter | Type | Beschreibung |
| --- | --- | --- |
| nodeIndex | Int32 | Der Knotenindex. |
| storagePath | String | Der Speicherpfad. |
| networkSettings | INetworkSettings | Die Netzwerkeinstellungen. |
| logger | ILogger | Der Logger. |
| configuration | Konfiguration | Die Konfiguration. |

### Rückgabewert

Der Master‑Knoten.

### Siehe auch

* interface [INetworkSettings](../../../groupdocs.search.scaling.configuring/inetworksettings)
* interface [ILogger](../../../groupdocs.search.common/ilogger)
* class [Configuration](../../../groupdocs.search.scaling.configuring/configuration)
* class [SearchNetworkNode](../../searchnetworknode)
* namespace [GroupDocs.Search.Scaling](../../../groupdocs.search.scaling)
* assembly [GroupDocs.Search](../../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
