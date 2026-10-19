---
title: "Evidenzia"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Genera testo formattato in HTML con i termini trovati evidenziati."
type: docs
weight: 210
url: /it/net/groupdocs.search/index/highlight/
---
## Highlight(FoundDocument, Highlighter) {#highlight}

Genera testo formattato in HTML con i termini trovati evidenziati.

```csharp
public void Highlight(FoundDocument document, Highlighter highlighter)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| document | FoundDocument | Il documento trovato. |
| evidenziatore | Evidenziatore | L'evidenziatore dei risultati di ricerca. |

### Esempi

L'esempio dimostra come evidenziare le occorrenze in testo formattato HTML.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentFolder = @"c:\MyDocuments\";

// Creazione di un indice
Index index = new Index(indexFolder);

// Indicizzazione dei documenti dalla cartella specificata
index.Add(documentFolder);

// Cerca la parola 'eternity'
SearchResult result = index.Search("eternity");

// Evidenziare le occorrenze nel testo
if (result.DocumentCount > 0)
{
    FoundDocument document = result.GetFoundDocument(0); // Getting the first found document
    OutputAdapter outputAdapter = new FileOutputAdapter(@"c:\Highlighted.html"); // Creating an output adapter to the file
    Highlighter highlighter = new HtmlHighlighter(outputAdapter); // Creating the highlighter object
    index.Highlight(document, highlighter); // Generating HTML formatted text with highlighted occurrences
}
```

### Vedi anche

* class [FoundDocument](../../../groupdocs.search.results/founddocument)
* class [Highlighter](../../../groupdocs.search.highlighters/highlighter)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Highlight(FoundDocument, Highlighter, HighlightOptions) {#highlight_1}

Genera testo formattato in HTML con i termini trovati evidenziati.

```csharp
public void Highlight(FoundDocument document, Highlighter highlighter, HighlightOptions options)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| document | FoundDocument | Il documento trovato. |
| evidenziatore | Evidenziatore | L'evidenziatore dei risultati di ricerca. |
| opzioni | HighlightOptions | Le opzioni di evidenziazione. |

### Esempi

L'esempio dimostra come evidenziare le occorrenze in testo formattato HTML.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentFolder = @"c:\MyDocuments\";

// Creazione di un indice
Index index = new Index(indexFolder);

// Indicizzazione dei documenti dalla cartella specificata
index.Add(documentFolder);

// Cerca la parola 'eternity'
SearchResult result = index.Search("eternity");

// Evidenziare le occorrenze nel testo
if (result.DocumentCount > 0)
{
    FoundDocument document = result.GetFoundDocument(0); // Getting the first found document
    OutputAdapter outputAdapter = new FileOutputAdapter(@"c:\Highlighted.html"); // Creating an output adapter to the file
    Highlighter highlighter = new HtmlHighlighter(outputAdapter); // Creating the highlighter object
    HighlightOptions options = new HighlightOptions(); // Creating the highlight options object
    options.TermsBefore = 5;
    options.TermsAfter = 5;
    options.TermsTotal = 15;
    index.Highlight(document, highlighter, options); // Generating HTML formatted text with highlighted occurrences
}
```

### Vedi anche

* class [FoundDocument](../../../groupdocs.search.results/founddocument)
* class [Highlighter](../../../groupdocs.search.highlighters/highlighter)
* class [HighlightOptions](../../../groupdocs.search.options/highlightoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
