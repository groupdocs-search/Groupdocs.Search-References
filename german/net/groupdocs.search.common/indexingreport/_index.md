---
title: "IndexingReport"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Stellt detaillierte Informationen zu einem Indexierungsvorgang dar."
type: docs
weight: 250
url: /de/net/groupdocs.search.common/indexingreport/
---
## IndexingReport class

Stellt detaillierte Informationen zu einem Indexierungsvorgang dar.

```csharp
public class IndexingReport
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [EndTime](../../groupdocs.search.common/indexingreport/endtime) { get; } | Ermittelt die Endzeit der Indexierung. |
| [Errors](../../groupdocs.search.common/indexingreport/errors) { get; } | Gibt die Liste der Fehler zurück. |
| [IndexedDocuments](../../groupdocs.search.common/indexingreport/indexeddocuments) { get; } | Gibt die Liste der indizierten Dokumente zurück. |
| [IndexedDocumentsSize](../../groupdocs.search.common/indexingreport/indexeddocumentssize) { get; } | Gibt die Gesamtlänge der indizierten Dokumente in MB zurück. |
| [IndexingTime](../../groupdocs.search.common/indexingreport/indexingtime) { get; } | Gibt die Dauer der Indizierung zurück. |
| [RemovedDocuments](../../groupdocs.search.common/indexingreport/removeddocuments) { get; } | Gibt die Liste der aus dem Index entfernten Dokumente zurück. |
| [SegmentCount](../../groupdocs.search.common/indexingreport/segmentcount) { get; } | Ruft die Anzahl der Indexsegmente ab. |
| [StartTime](../../groupdocs.search.common/indexingreport/starttime) { get; } | Gibt den Startzeitpunkt der Indizierung zurück. |
| [TotalDocumentsInIndex](../../groupdocs.search.common/indexingreport/totaldocumentsinindex) { get; } | Gibt die Gesamtzahl der Dokumente im Index zurück. |
| [TotalIndexSize](../../groupdocs.search.common/indexingreport/totalindexsize) { get; } | Gibt die gesamte Indexgröße in Bytes zurück. |
| [TotalTermCount](../../groupdocs.search.common/indexingreport/totaltermcount) { get; } | Gibt die Gesamtzahl der Begriffe im Index zurück. |
| [UpdatedDocuments](../../groupdocs.search.common/indexingreport/updateddocuments) { get; } | Gibt die Liste der aktualisierten Dokumente zurück. |

### Hinweise

**Learn more**

* [Indexing reports](https://docs.groupdocs.com/display/searchnet/Indexing+reports)

### Beispiele

Das Beispiel zeigt eine typische Verwendung der Klasse.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder1 = @"c:\MyDocuments1\";
string documentsFolder2 = @"c:\MyDocuments2\";

// Erstelle einen Index im angegebenen Ordner
Index index = new Index(indexFolder);

// Indiziere Dokumente
index.Add(documentsFolder1);
index.Add(documentsFolder2);

// Erhalte Indizierungsberichte
IndexingReport[] reports = index.GetIndexingReports();

// Drucke Berichte in die Konsole
foreach (IndexingReport report in reports)
{
    Console.WriteLine("Time: " + report.StartTime);
    Console.WriteLine("Duration: " + report.IndexingTime);
    Console.WriteLine("Documents total: " + report.TotalDocumentsInIndex);
    Console.WriteLine("Terms total: " + report.TotalTermCount);
    Console.WriteLine("Indexed documents size (MB): " + report.IndexedDocumentsSize);
    Console.WriteLine("Index size (MB): " + (report.TotalIndexSize / 1024.0 / 1024.0));
    Console.WriteLine();
}
```

### Siehe auch

* namespace [GroupDocs.Search.Common](../../groupdocs.search.common)
* assembly [GroupDocs.Search](../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
