---
title: "SearchReport"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Rappresenta informazioni dettagliate su un'operazione di ricerca."
type: docs
weight: 300
url: /it/net/groupdocs.search.common/searchreport/
---
## SearchReport class

Rappresenta informazioni dettagliate su un'operazione di ricerca.

```csharp
public class SearchReport
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [DocumentCount](../../groupdocs.search.common/searchreport/documentcount) { get; } | Ottiene il numero di documenti trovati. |
| [EndTime](../../groupdocs.search.common/searchreport/endtime) { get; } | Ottiene l'ora di fine della ricerca. |
| [ObjectQuery](../../groupdocs.search.common/searchreport/objectquery) { get; } | Ottiene la query di ricerca in forma di oggetto. |
| [OccurrenceCount](../../groupdocs.search.common/searchreport/occurrencecount) { get; } | Ottiene il numero totale di occorrenze trovate. |
| [SearchDuration](../../groupdocs.search.common/searchreport/searchduration) { get; } | Ottiene la durata della ricerca. |
| [SearchOptions](../../groupdocs.search.common/searchreport/searchoptions) { get; } | Ottiene le opzioni di ricerca. |
| [StartTime](../../groupdocs.search.common/searchreport/starttime) { get; } | Ottiene l'ora di inizio della ricerca. |
| [TextQuery](../../groupdocs.search.common/searchreport/textquery) { get; } | Ottiene la query di ricerca in forma di testo. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| override [ToString](../../groupdocs.search.common/searchreport/tostring)() | Restituisce una String che rappresenta l'attuale [`SearchReport`](../searchreport). |

### Osservazioni

**Learn more**

* [Search reports](https://docs.groupdocs.com/display/searchnet/Search+reports)

### Esempi

L'esempio dimostra un utilizzo tipico della classe.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

// Creazione di un indice nella cartella specificata
Index index = new Index(indexFolder);

// Indicizzazione dei documenti dalla cartella specificata
index.Add(documentsFolder);

// Ricerca nell'indice
SearchResult result1 = index.Search("Einstein");
SearchResult result2 = index.Search("\"Theory of Relativity\"");

// Recupero dei report di ricerca
SearchReport[] reports = index.GetSearchReports();

// Stampa dei report sulla console
foreach (SearchReport report in reports)
{
    Console.WriteLine("Query: " + report.TextQuery);
    Console.WriteLine("Time: " + report.StartTime);
    Console.WriteLine("Duration: " + report.SearchDuration);
    Console.WriteLine("Documents: " + report.DocumentCount);
    Console.WriteLine("Occurrences: " + report.OccurrenceCount);
    Console.WriteLine();
}
```

### Vedi anche

* namespace [GroupDocs.Search.Common](../../groupdocs.search.common)
* assembly [GroupDocs.Search](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
