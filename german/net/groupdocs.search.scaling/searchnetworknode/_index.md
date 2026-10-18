---
title: "SearchNetworkNode"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Stellt einen Suchnetzwerkknoten dar, der Dienste wie extractor, indexer, searcher und shard enthalten kann."
type: docs
weight: 1550
url: /de/net/groupdocs.search.scaling/searchnetworknode/
---
## SearchNetworkNode class

Stellt einen Knoten des Suchnetzwerks dar, der Dienste wie Extraktor, Indexierer, Sucher, Shard enthalten kann.

```csharp
public class SearchNetworkNode : IDisposable
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [CustomExtractors](../../groupdocs.search.scaling/searchnetworknode/customextractors) { get; } | Ruft die benutzerdefinierte Extraktor‑Sammlung ab. |
| [Events](../../groupdocs.search.scaling/searchnetworknode/events) { get; } | Liefert den Ereignis-Hub zum Abonnieren von Ereignissen. |
| [Indexer](../../groupdocs.search.scaling/searchnetworknode/indexer) { get; } | Liest den Indexer. |
| [NodeIndex](../../groupdocs.search.scaling/searchnetworknode/nodeindex) { get; } | Gibt den Index des Suchnetzwerkknotens zurück. |
| [Searcher](../../groupdocs.search.scaling/searchnetworknode/searcher) { get; } | Liest den Searcher. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| static [CreateMasterNode](../../groupdocs.search.scaling/searchnetworknode/createmasternode)(int, string, INetworkSettings, ILogger, Configuration) | Erstellt einen Master-Knoten des Suchnetzwerks. |
| static [CreateSlaveNode](../../groupdocs.search.scaling/searchnetworknode/createslavenode#createslavenode)(int, string, INetworkSettings) | Erstellt einen Slave-Knoten des Suchnetzwerks. |
| static [CreateSlaveNode](../../groupdocs.search.scaling/searchnetworknode/createslavenode#createslavenode_1)(int, string, INetworkSettings, ILogger) | Erstellt einen Slave-Knoten des Suchnetzwerks. |
| [ConfigureAllNodes](../../groupdocs.search.scaling/searchnetworknode/configureallnodes)() | Konfiguriert alle Knoten im Suchnetzwerk. |
| [ConfigureNode](../../groupdocs.search.scaling/searchnetworknode/configurenode)(int) | Konfiguriert den angegebenen Knoten im Suchnetzwerk. |
| [Dispose](../../groupdocs.search.scaling/searchnetworknode/dispose)() | Gibt alle von dem [`SearchNetworkNode`](../searchnetworknode) verwendeten Ressourcen frei. |
| [GetNodeIndex](../../groupdocs.search.scaling/searchnetworknode/getnodeindex)(int) | Ermittelt den Index des Knotens, an dem der Dienst befindet. |
| [GetShardIndices](../../groupdocs.search.scaling/searchnetworknode/getshardindices)() | Ermittelt ein Array aller Shard-Indizes im Suchnetzwerk. |
| [SetOcrConnector](../../groupdocs.search.scaling/searchnetworknode/setocrconnector)(IOcrConnector) | Legt einen OCR‑Connector fest, der für die OCR‑Verarbeitung verwendet wird. |
| [SetWordFormsProvider](../../groupdocs.search.scaling/searchnetworknode/setwordformsprovider)(IWordFormsProvider) | Legt einen Anbieter für Wortformen fest. |
| [Start](../../groupdocs.search.scaling/searchnetworknode/start)() | Startet die Funktionsweise des Suchnetzwerk‑Knotens. |

### Siehe auch

* namespace [GroupDocs.Search.Scaling](../../groupdocs.search.scaling)
* assembly [GroupDocs.Search](../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
