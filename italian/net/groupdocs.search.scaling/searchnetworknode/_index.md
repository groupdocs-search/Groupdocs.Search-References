---
title: "SearchNetworkNode"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Rappresenta un nodo della rete di ricerca che può contenere servizi come estrattore, indicizzatore, ricercatore e shard."
type: docs
weight: 1550
url: /it/net/groupdocs.search.scaling/searchnetworknode/
---
## SearchNetworkNode class

Rappresenta un nodo della rete di ricerca che può contenere servizi come estrattore, indicizzatore, ricercatore, frammento.

```csharp
public class SearchNetworkNode : IDisposable
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [CustomExtractors](../../groupdocs.search.scaling/searchnetworknode/customextractors) { get; } | Ottiene la raccolta di estrattori personalizzati. |
| [Events](../../groupdocs.search.scaling/searchnetworknode/events) { get; } | Ottiene il hub degli eventi per l'iscrizione agli eventi. |
| [Indexer](../../groupdocs.search.scaling/searchnetworknode/indexer) { get; } | Ottiene l'indicizzatore. |
| [NodeIndex](../../groupdocs.search.scaling/searchnetworknode/nodeindex) { get; } | Ottiene l'indice del nodo di rete di ricerca. |
| [Searcher](../../groupdocs.search.scaling/searchnetworknode/searcher) { get; } | Ottiene il ricercatore. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| static [CreateMasterNode](../../groupdocs.search.scaling/searchnetworknode/createmasternode)(int, string, INetworkSettings, ILogger, Configuration) | Crea un nodo master della rete di ricerca. |
| static [CreateSlaveNode](../../groupdocs.search.scaling/searchnetworknode/createslavenode#createslavenode)(int, string, INetworkSettings) | Crea un nodo slave della rete di ricerca. |
| static [CreateSlaveNode](../../groupdocs.search.scaling/searchnetworknode/createslavenode#createslavenode_1)(int, string, INetworkSettings, ILogger) | Crea un nodo slave della rete di ricerca. |
| [ConfigureAllNodes](../../groupdocs.search.scaling/searchnetworknode/configureallnodes)() | Configura tutti i nodi nella rete di ricerca. |
| [ConfigureNode](../../groupdocs.search.scaling/searchnetworknode/configurenode)(int) | Configura il nodo specificato nella rete di ricerca. |
| [Dispose](../../groupdocs.search.scaling/searchnetworknode/dispose)() | Rilascia tutte le risorse utilizzate da [`SearchNetworkNode`](../searchnetworknode). |
| [GetNodeIndex](../../groupdocs.search.scaling/searchnetworknode/getnodeindex)(int) | Ottiene l'indice del nodo in cui si trova il servizio. |
| [GetShardIndices](../../groupdocs.search.scaling/searchnetworknode/getshardindices)() | Ottiene un array di tutti gli indici di shard nella rete di ricerca. |
| [SetOcrConnector](../../groupdocs.search.scaling/searchnetworknode/setocrconnector)(IOcrConnector) | Imposta un connettore OCR utilizzato per l'elaborazione OCR. |
| [SetWordFormsProvider](../../groupdocs.search.scaling/searchnetworknode/setwordformsprovider)(IWordFormsProvider) | Imposta un provider di forme di parole. |
| [Start](../../groupdocs.search.scaling/searchnetworknode/start)() | Avvia il funzionamento del nodo della rete di ricerca. |

### Vedi anche

* namespace [GroupDocs.Search.Scaling](../../groupdocs.search.scaling)
* assembly [GroupDocs.Search](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
