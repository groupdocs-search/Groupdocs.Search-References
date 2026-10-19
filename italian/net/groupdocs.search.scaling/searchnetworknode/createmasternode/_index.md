---
title: "CreateMasterNode"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Crea un nodo master della rete di ricerca."
type: docs
weight: 10
url: /it/net/groupdocs.search.scaling/searchnetworknode/createmasternode/
---
## SearchNetworkNode.CreateMasterNode method

Crea un nodo master della rete di ricerca.

```csharp
public static SearchNetworkNode CreateMasterNode(int nodeIndex, string storagePath, 
    INetworkSettings networkSettings, ILogger logger, Configuration configuration)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| indiceNodo | Int32 | L'indice del nodo. |
| percorsoArchiviazione | String | Il percorso di archiviazione. |
| networkSettings | INetworkSettings | Le impostazioni di rete. |
| logger | ILogger | Il logger. |
| configurazione | Configurazione | La configurazione. |

### Valore di ritorno

Il nodo master.

### Vedi anche

* interface [INetworkSettings](../../../groupdocs.search.scaling.configuring/inetworksettings)
* interface [ILogger](../../../groupdocs.search.common/ilogger)
* class [Configuration](../../../groupdocs.search.scaling.configuring/configuration)
* class [SearchNetworkNode](../../searchnetworknode)
* namespace [GroupDocs.Search.Scaling](../../../groupdocs.search.scaling)
* assembly [GroupDocs.Search](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
