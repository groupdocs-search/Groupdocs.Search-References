---
title: Highlight
second_title: GroupDocs.Search for .NET API Reference
description: Highlights the found terms in the text of the found document using the specified highlighter.
type: docs
weight: 210
url: /net/groupdocs.search/index/highlight/
---

## Highlight(FoundDocument, Highlighter) {#highlight}

Highlights the found terms in the text of the found document using the specified highlighter.

```csharp
public void Highlight(FoundDocument document, Highlighter highlighter)
```

| Parameter | Type | Description |
| --- | --- | --- |
| document | FoundDocument | The found document. |
| highlighter | Highlighter | The search result highlighter. |

### Exceptions

| exception | condition |
| --- | --- |
| ObjectDisposedException | The index is disposed. |

### Remarks

The text is read from the index if the index stores the texts of the documents; otherwise the document is extracted again from the file at its path. A document that the index does not contain is not highlighted, and the [`ErrorOccurred`](../../../groupdocs.search.events/eventhub/erroroccurred) event reports it. The found document must come from a search of this index or from a trusted source: an indexed document is highlighted by its path, so an application that gets found documents from its users must check that a user may read the document.

The text is divided into words by the built-in division: a document that was indexed with a custom word splitter is highlighted with the options that have the same splitter, see [`Highlight`](../highlight) and [`WordSplitter`](../../../groupdocs.search.options/textoptions/wordsplitter).

### Examples

The example demonstrates how to highlight occurrences in HTML formatted text.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentFolder = @"c:\MyDocuments\";

// Creating an index
Index index = new Index(indexFolder);

// Indexing documents from the specified folder
index.Add(documentFolder);

// Search for the word 'eternity'
SearchResult result = index.Search("eternity");

// Highlighting occurrences in text
if (result.DocumentCount > 0)
{
    FoundDocument document = result.GetFoundDocument(0); // Getting the first found document
    OutputAdapter outputAdapter = new FileOutputAdapter(OutputFormat.Html, @"c:\Highlighted.html"); // Creating an output adapter to the file
    Highlighter highlighter = new DocumentHighlighter(outputAdapter); // Creating the highlighter object
    index.Highlight(document, highlighter); // Generating HTML formatted text with highlighted occurrences
}
```

### See Also

* class [FoundDocument](../../../groupdocs.search.results/founddocument)
* class [Highlighter](../../../groupdocs.search.highlighters/highlighter)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Highlight(FoundDocument, Highlighter, HighlightOptions) {#highlight_1}

Highlights the found terms in the text of the found document using the specified highlighter.

```csharp
public void Highlight(FoundDocument document, Highlighter highlighter, HighlightOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| document | FoundDocument | The found document. |
| highlighter | Highlighter | The search result highlighter. |
| options | HighlightOptions | The highlight options. |

### Exceptions

| exception | condition |
| --- | --- |
| ObjectDisposedException | The index is disposed. |

### Remarks

The text is read from the index if the index stores the texts of the documents; otherwise the document is extracted again from the file at its path. A document that the index does not contain is not highlighted, and the [`ErrorOccurred`](../../../groupdocs.search.events/eventhub/erroroccurred) event reports it. The found document must come from a search of this index or from a trusted source: an indexed document is highlighted by its path, so an application that gets found documents from its users must check that a user may read the document.

A document that was indexed with a custom word splitter (see [`WordSplitter`](../../../groupdocs.search.events/fileindexingeventargs/wordsplitter)) is divided into words by the splitter of the options (see [`WordSplitter`](../../../groupdocs.search.options/textoptions/wordsplitter)): the options must have the same splitter, otherwise the words that the built-in division does not give are not highlighted.

### Examples

The example demonstrates how to highlight occurrences in HTML formatted text.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentFolder = @"c:\MyDocuments\";

// Creating an index
Index index = new Index(indexFolder);

// Indexing documents from the specified folder
index.Add(documentFolder);

// Search for the word 'eternity'
SearchResult result = index.Search("eternity");

// Highlighting occurrences in text
if (result.DocumentCount > 0)
{
    FoundDocument document = result.GetFoundDocument(0); // Getting the first found document
    OutputAdapter outputAdapter = new FileOutputAdapter(OutputFormat.Html, @"c:\Highlighted.html"); // Creating an output adapter to the file
    Highlighter highlighter = new DocumentHighlighter(outputAdapter); // Creating the highlighter object
    HighlightOptions options = new HighlightOptions(); // Creating the highlight options object
    options.HighlightColor = new Color(0, 255, 0); // Setting the highlight color
    index.Highlight(document, highlighter, options); // Generating HTML formatted text with highlighted occurrences
}
```

### See Also

* class [FoundDocument](../../../groupdocs.search.results/founddocument)
* class [Highlighter](../../../groupdocs.search.highlighters/highlighter)
* class [HighlightOptions](../../../groupdocs.search.options/highlightoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
