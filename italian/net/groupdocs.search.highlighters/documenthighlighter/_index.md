---
title: "DocumentHighlighter"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Rappresenta un evidenziatore di risultati di ricerca che evidenzia i risultati di ricerca nell'intero testo del documento."
type: docs
weight: 670
url: /it/net/groupdocs.search.highlighters/documenthighlighter/
---
## DocumentHighlighter class

Rappresenta un evidenziatore di risultati di ricerca che evidenzia i risultati di ricerca nell'intero testo del documento.

```csharp
public class DocumentHighlighter : Highlighter
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [DocumentHighlighter](documenthighlighter)(OutputAdapter) | Inizializza una nuova istanza della classe [`DocumentHighlighter`](../documenthighlighter). |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [OutputAdapter](../../groupdocs.search.highlighters/documenthighlighter/outputadapter) { get; } | Ottiene l'adattatore di output passato nel costruttore. |
| [OutputFormat](../../groupdocs.search.common/resultbuilderfactory/outputformat) { get; } | Restituisce il formato di output. |

### Osservazioni

**Learn more**

* [Highlighting search results](https://docs.groupdocs.com/display/searchnet/Highlighting+search+results)

### Esempi

L'esempio dimostra un utilizzo tipico della classe.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

// Creazione di un indice
Index index = new Index(indexFolder);

// Indicizzazione dei documenti dalla cartella specificata
index.Add(documentsFolder);

// Cerca la fase 'Theory of Relativity'
SearchResult result = index.Search("\"Theory of Relativity\"");

// Evidenzia le parole trovate nel testo di un documento
FoundDocument document = result.GetFoundDocument(0);
OutputAdapter outputAdapter = new FileOutputAdapter(OutputFormat.Html, "Highlighted.html");
Highlighter highlighter = new DocumentHighlighter(outputAdapter);
index.Highlight(document, highlighter);
```

### Vedi anche

* class [Highlighter](../highlighter)
* namespace [GroupDocs.Search.Highlighters](../../groupdocs.search.highlighters)
* assembly [GroupDocs.Search](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
