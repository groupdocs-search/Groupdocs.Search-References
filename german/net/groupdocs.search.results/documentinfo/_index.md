---
title: "DocumentInfo"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Stellt einen Deskriptor für ein indiziertes Dokument dar."
type: docs
weight: 1230
url: /de/net/groupdocs.search.results/documentinfo/
---
## DocumentInfo class

Stellt einen Deskriptor für ein indiziertes Dokument dar.

```csharp
public class DocumentInfo
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [DocumentSourceKind](../../groupdocs.search.results/documentinfo/documentsourcekind) { get; } | Liefert die Art der Dokumentquelle. |
| [FilePath](../../groupdocs.search.results/documentinfo/filepath) { get; } | Liefert den Dateipfad für indizierte Dateien oder den Dokumentschlüssel für indizierte Streams oder Strukturen. |
| [FileType](../../groupdocs.search.results/documentinfo/filetype) { get; } | Liefert den Dateityp. |
| [FormatFamily](../../groupdocs.search.results/documentinfo/formatfamily) { get; } | Ruft die Dokumentformatfamilie ab. |
| [IndexedWithError](../../groupdocs.search.results/documentinfo/indexedwitherror) { get; } | Liefert den Indikator für einen Indexierungsfehler. |
| [InnerPath](../../groupdocs.search.results/documentinfo/innerpath) { get; } | Liefert den inneren Pfad für das Container-Dokument-Element. |
| [InnerPathParts](../../groupdocs.search.results/documentinfo/innerpathparts) { get; } | Liefert die inneren Pfadteile für das Container-Dokument-Element. |
| [ModificationTime](../../groupdocs.search.results/documentinfo/modificationtime) { get; } | Liefert das Änderungsdatum. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| static [Deserialize](../../groupdocs.search.results/documentinfo/deserialize)(byte[]) | Deserialisiert eine Instanz aus einem Byte-Array. |
| [Serialize](../../groupdocs.search.results/documentinfo/serialize)() | Serialisiert die aktuelle Instanz in ein Byte-Array. |
| override [ToString](../../groupdocs.search.results/documentinfo/tostring)() | Gibt eine Zeichenkette zurück, die die aktuelle [`DocumentInfo`](../documentinfo) darstellt. |

### Hinweise

**Learn more**

* [Search results](https://docs.groupdocs.com/display/searchnet/Search+results)
* [Getting indexed documents](https://docs.groupdocs.com/display/searchnet/Getting+indexed+documents)

### Siehe auch

* namespace [GroupDocs.Search.Results](../../groupdocs.search.results)
* assembly [GroupDocs.Search](../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
