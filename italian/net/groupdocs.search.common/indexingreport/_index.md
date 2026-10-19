---
title: "IndexingReport"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Rappresenta informazioni dettagliate su un'operazione di indicizzazione."
type: docs
weight: 250
url: /it/net/groupdocs.search.common/indexingreport/
---
## IndexingReport class

Rappresenta informazioni dettagliate su un'operazione di indicizzazione.

```csharp
public class IndexingReport
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [EndTime](../../groupdocs.search.common/indexingreport/endtime) { get; } | Ottiene l'ora di fine dell'indicizzazione. |
| [Errors](../../groupdocs.search.common/indexingreport/errors) { get; } | Ottiene l'elenco degli errori. |
| [IndexedDocuments](../../groupdocs.search.common/indexingreport/indexeddocuments) { get; } | Ottiene l'elenco dei documenti indicizzati. |
| [IndexedDocumentsSize](../../groupdocs.search.common/indexingreport/indexeddocumentssize) { get; } | Ottiene la lunghezza totale dei documenti indicizzati in MB. |
| [IndexingTime](../../groupdocs.search.common/indexingreport/indexingtime) { get; } | Ottiene la durata dell'indicizzazione. |
| [RemovedDocuments](../../groupdocs.search.common/indexingreport/removeddocuments) { get; } | Ottiene l'elenco dei documenti rimossi dall'indice. |
| [SegmentCount](../../groupdocs.search.common/indexingreport/segmentcount) { get; } | Ottiene il numero di segmenti dell'indice. |
| [StartTime](../../groupdocs.search.common/indexingreport/starttime) { get; } | Ottiene l'ora di inizio dell'indicizzazione. |
| [TotalDocumentsInIndex](../../groupdocs.search.common/indexingreport/totaldocumentsinindex) { get; } | Ottiene il numero totale di documenti nell'indice. |
| [TotalIndexSize](../../groupdocs.search.common/indexingreport/totalindexsize) { get; } | Ottiene la dimensione totale dell'indice in byte. |
| [TotalTermCount](../../groupdocs.search.common/indexingreport/totaltermcount) { get; } | Ottiene il numero totale di termini nell'indice. |
| [UpdatedDocuments](../../groupdocs.search.common/indexingreport/updateddocuments) { get; } | Ottiene l'elenco dei documenti aggiornati. |

### Osservazioni

**Learn more**

* [Indexing reports](https://docs.groupdocs.com/display/searchnet/Indexing+reports)

### Esempi

L'esempio dimostra un utilizzo tipico della classe.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder1 = @"c:\MyDocuments1\";
string documentsFolder2 = @"c:\MyDocuments2\";

// Creazione di un indice nella cartella specificata
Index index = new Index(indexFolder);

// Indicizzazione dei documenti
index.Add(documentsFolder1);
index.Add(documentsFolder2);

// Recupero dei report di indicizzazione
IndexingReport[] reports = index.GetIndexingReports();

// Stampa dei report sulla console
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

### Vedi anche

* namespace [GroupDocs.Search.Common](../../groupdocs.search.common)
* assembly [GroupDocs.Search](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
