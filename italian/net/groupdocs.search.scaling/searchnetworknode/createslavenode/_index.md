---
title: "CreateSlaveNode"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Crea un nodo slave della rete di ricerca."
type: docs
weight: 20
url: /it/net/groupdocs.search.scaling/searchnetworknode/createslavenode/
---
## CreateSlaveNode(int, string, INetworkSettings) {#createslavenode}

Crea un nodo slave della rete di ricerca.

```csharp
public static SearchNetworkNode CreateSlaveNode(int nodeIndex, string storagePath, 
    INetworkSettings networkSettings)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| indiceNodo | Int32 | L'indice del nodo. |
| percorsoArchiviazione | String | Il percorso di archiviazione. |
| networkSettings | INetworkSettings | Le impostazioni di rete. |

### Valore di ritorno

Il nodo slave.

### Vedi anche

* interface [INetworkSettings](../../../groupdocs.search.scaling.configuring/inetworksettings)
* class [SearchNetworkNode](../../searchnetworknode)
* namespace [GroupDocs.Search.Scaling](../../../groupdocs.search.scaling)
* assembly [GroupDocs.Search](../../../)

---

## CreateSlaveNode(int, string, INetworkSettings, ILogger) {#createslavenode_1}

Crea un nodo slave della rete di ricerca.

```csharp
public static SearchNetworkNode CreateSlaveNode(int nodeIndex, string storagePath, 
    INetworkSettings networkSettings, ILogger logger)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| indiceNodo | Int32 | L'indice del nodo. |
| percorsoArchiviazione | String | Il percorso di archiviazione. |
| networkSettings | INetworkSettings | Le impostazioni di rete. |
| logger | ILogger | Il logger. |

### Valore di ritorno

Il nodo slave.

### Vedi anche

* interface [INetworkSettings](../../../groupdocs.search.scaling.configuring/inetworksettings)
* interface [ILogger](../../../groupdocs.search.common/ilogger)
* class [SearchNetworkNode](../../searchnetworknode)
* namespace [GroupDocs.Search.Scaling](../../../groupdocs.search.scaling)
* assembly [GroupDocs.Search](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
