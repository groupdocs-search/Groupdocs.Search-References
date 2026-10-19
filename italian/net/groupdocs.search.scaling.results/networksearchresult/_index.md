---
title: "NetworkSearchResult"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Rappresenta un risultato di ricerca corrispondente a una query di ricerca."
type: docs
weight: 1530
url: /it/net/groupdocs.search.scaling.results/networksearchresult/
---
## NetworkSearchResult class

Rappresenta un risultato di ricerca corrispondente a una query di ricerca.

```csharp
public class NetworkSearchResult : IEnumerable<NetworkFoundDocument>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [DocumentCount](../../groupdocs.search.scaling.results/networksearchresult/documentcount) { get; } | Ottiene il numero di documenti trovati. |
| [EndTime](../../groupdocs.search.scaling.results/networksearchresult/endtime) { get; } | Ottiene l'ora di fine della ricerca. |
| [NextChunkSearchToken](../../groupdocs.search.scaling.results/networksearchresult/nextchunksearchtoken) { get; } | Ottiene un token di ricerca a blocchi per cercare il blocco successivo. |
| [NodeIndex](../../groupdocs.search.scaling.results/networksearchresult/nodeindex) { get; } | Ottiene l'indice del nodo da cui è stato ricevuto il risultato. |
| [OccurrenceCount](../../groupdocs.search.scaling.results/networksearchresult/occurrencecount) { get; } | Ottiene il numero totale di occorrenze trovate. |
| [SearchDuration](../../groupdocs.search.scaling.results/networksearchresult/searchduration) { get; } | Ottiene la durata della ricerca. |
| [StartTime](../../groupdocs.search.scaling.results/networksearchresult/starttime) { get; } | Ottiene l'ora di inizio della ricerca. |
| [Truncated](../../groupdocs.search.scaling.results/networksearchresult/truncated) { get; } | Ottiene un valore che indica che il risultato è troncato. |
| [Warnings](../../groupdocs.search.scaling.results/networksearchresult/warnings) { get; } | Ottiene gli avvisi che descrivono il risultato. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [GetEnumerator](../../groupdocs.search.scaling.results/networksearchresult/getenumerator)() | Restituisce un enumeratore che itera attraverso la raccolta dei documenti trovati. |
| [GetFoundDocument](../../groupdocs.search.scaling.results/networksearchresult/getfounddocument)(int) | Ottiene il documento trovato per indice. |

### Vedi anche

* class [NetworkFoundDocument](../networkfounddocument)
* namespace [GroupDocs.Search.Scaling.Results](../../groupdocs.search.scaling.results)
* assembly [GroupDocs.Search](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
