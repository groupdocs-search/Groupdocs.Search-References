---
title: "SearchNetworkNode"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Représente un nœud du réseau de recherche qui peut contenir des services tels que extractor, indexer, searcher, shard."
type: docs
weight: 1550
url: /fr/net/groupdocs.search.scaling/searchnetworknode/
---
## SearchNetworkNode class

Représente un nœud du réseau de recherche qui peut contenir des services tels que l'extracteur, l'indexeur, le chercheur, le fragment.

```csharp
public class SearchNetworkNode : IDisposable
```

## Propriétés

| Nom | Description |
| --- | --- |
| [CustomExtractors](../../groupdocs.search.scaling/searchnetworknode/customextractors) { get; } | Obtient la collection d'extracteurs personnalisés. |
| [Events](../../groupdocs.search.scaling/searchnetworknode/events) { get; } | Obtient le hub d'événements pour s'abonner aux événements. |
| [Indexer](../../groupdocs.search.scaling/searchnetworknode/indexer) { get; } | Obtient l'indexeur. |
| [NodeIndex](../../groupdocs.search.scaling/searchnetworknode/nodeindex) { get; } | Obtient l'indice du nœud du réseau de recherche. |
| [Searcher](../../groupdocs.search.scaling/searchnetworknode/searcher) { get; } | Obtient le chercheur. |

## Méthodes

| Nom | Description |
| --- | --- |
| static [CreateMasterNode](../../groupdocs.search.scaling/searchnetworknode/createmasternode)(int, string, INetworkSettings, ILogger, Configuration) | Crée un nœud maître du réseau de recherche. |
| static [CreateSlaveNode](../../groupdocs.search.scaling/searchnetworknode/createslavenode#createslavenode)(int, string, INetworkSettings) | Crée un nœud esclave du réseau de recherche. |
| static [CreateSlaveNode](../../groupdocs.search.scaling/searchnetworknode/createslavenode#createslavenode_1)(int, string, INetworkSettings, ILogger) | Crée un nœud esclave du réseau de recherche. |
| [ConfigureAllNodes](../../groupdocs.search.scaling/searchnetworknode/configureallnodes)() | Configure tous les nœuds du réseau de recherche. |
| [ConfigureNode](../../groupdocs.search.scaling/searchnetworknode/configurenode)(int) | Configure le nœud spécifié du réseau de recherche. |
| [Dispose](../../groupdocs.search.scaling/searchnetworknode/dispose)() | Libère toutes les ressources utilisées par le [`SearchNetworkNode`](../searchnetworknode). |
| [GetNodeIndex](../../groupdocs.search.scaling/searchnetworknode/getnodeindex)(int) | Obtient l'index du nœud où le service est situé. |
| [GetShardIndices](../../groupdocs.search.scaling/searchnetworknode/getshardindices)() | Obtient un tableau de tous les indices de fragments dans le réseau de recherche. |
| [SetOcrConnector](../../groupdocs.search.scaling/searchnetworknode/setocrconnector)(IOcrConnector) | Définit un connecteur OCR utilisé pour le traitement OCR. |
| [SetWordFormsProvider](../../groupdocs.search.scaling/searchnetworknode/setwordformsprovider)(IWordFormsProvider) | Définit un fournisseur de formes de mots. |
| [Start](../../groupdocs.search.scaling/searchnetworknode/start)() | Démarre le fonctionnement du nœud du réseau de recherche. |

### Voir aussi

* namespace [GroupDocs.Search.Scaling](../../groupdocs.search.scaling)
* assembly [GroupDocs.Search](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
