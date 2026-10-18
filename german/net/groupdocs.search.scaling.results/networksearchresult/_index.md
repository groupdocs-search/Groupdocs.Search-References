---
title: "NetworkSearchResult"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Stellt ein Suchergebnis dar, das zu einer Suchanfrage passt."
type: docs
weight: 1530
url: /de/net/groupdocs.search.scaling.results/networksearchresult/
---
## NetworkSearchResult class

Stellt ein Suchergebnis dar, das zu einer Suchanfrage passt.

```csharp
public class NetworkSearchResult : IEnumerable<NetworkFoundDocument>
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [DocumentCount](../../groupdocs.search.scaling.results/networksearchresult/documentcount) { get; } | Ruft die Anzahl gefundener Dokumente ab. |
| [EndTime](../../groupdocs.search.scaling.results/networksearchresult/endtime) { get; } | Ruft die Endzeit der Suche ab. |
| [NextChunkSearchToken](../../groupdocs.search.scaling.results/networksearchresult/nextchunksearchtoken) { get; } | Gibt ein Chunk‑Suche‑Token zum Suchen des nächsten Chunks zurück. |
| [NodeIndex](../../groupdocs.search.scaling.results/networksearchresult/nodeindex) { get; } | Ruft den Index des Knotens ab, von dem das Ergebnis empfangen wurde. |
| [OccurrenceCount](../../groupdocs.search.scaling.results/networksearchresult/occurrencecount) { get; } | Ruft die Gesamtzahl gefundener Vorkommen ab. |
| [SearchDuration](../../groupdocs.search.scaling.results/networksearchresult/searchduration) { get; } | Ruft die Suchdauer ab. |
| [StartTime](../../groupdocs.search.scaling.results/networksearchresult/starttime) { get; } | Ruft die Startzeit der Suche ab. |
| [Truncated](../../groupdocs.search.scaling.results/networksearchresult/truncated) { get; } | Gibt einen Wert zurück, der anzeigt, dass das Ergebnis abgeschnitten ist. |
| [Warnings](../../groupdocs.search.scaling.results/networksearchresult/warnings) { get; } | Gibt eine Warnung zurück, die das Ergebnis beschreibt. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [GetEnumerator](../../groupdocs.search.scaling.results/networksearchresult/getenumerator)() | Gibt einen Enumerator zurück, der durch die Sammlung der gefundenen Dokumente iteriert. |
| [GetFoundDocument](../../groupdocs.search.scaling.results/networksearchresult/getfounddocument)(int) | Gibt das gefundene Dokument nach Index zurück. |

### Siehe auch

* class [NetworkFoundDocument](../networkfounddocument)
* namespace [GroupDocs.Search.Scaling.Results](../../groupdocs.search.scaling.results)
* assembly [GroupDocs.Search](../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
