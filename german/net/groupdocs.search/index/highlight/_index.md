---
title: "Highlight"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Erzeugt HTML-formatierten Text mit hervorgehobenen gefundenen Begriffen."
type: docs
weight: 210
url: /de/net/groupdocs.search/index/highlight/
---
## Highlight(FoundDocument, Highlighter) {#highlight}

Erzeugt HTML-formatierten Text mit hervorgehobenen gefundenen Begriffen.

```csharp
public void Highlight(FoundDocument document, Highlighter highlighter)
```

| Parameter | Type | Beschreibung |
| --- | --- | --- |
| document | FoundDocument | Das gefundene Dokument. |
| Markierer | Markierer | Der Suchergebnis‑Markierer. |

### Beispiele

Das Beispiel zeigt, wie Vorkommen in HTML‑formatiertem Text hervorgehoben werden.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentFolder = @"c:\MyDocuments\";

// Erstellen eines Index
Index index = new Index(indexFolder);

// Indizierung von Dokumenten aus dem angegebenen Ordner
index.Add(documentFolder);

// Suche nach dem Wort 'eternity'
SearchResult result = index.Search("eternity");

// Hervorheben von Vorkommen im Text
if (result.DocumentCount > 0)
{
    FoundDocument document = result.GetFoundDocument(0); // Getting the first found document
    OutputAdapter outputAdapter = new FileOutputAdapter(@"c:\Highlighted.html"); // Creating an output adapter to the file
    Highlighter highlighter = new HtmlHighlighter(outputAdapter); // Creating the highlighter object
    index.Highlight(document, highlighter); // Generating HTML formatted text with highlighted occurrences
}
```

### Siehe auch

* class [FoundDocument](../../../groupdocs.search.results/founddocument)
* class [Highlighter](../../../groupdocs.search.highlighters/highlighter)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Highlight(FoundDocument, Highlighter, HighlightOptions) {#highlight_1}

Erzeugt HTML-formatierten Text mit hervorgehobenen gefundenen Begriffen.

```csharp
public void Highlight(FoundDocument document, Highlighter highlighter, HighlightOptions options)
```

| Parameter | Type | Beschreibung |
| --- | --- | --- |
| document | FoundDocument | Das gefundene Dokument. |
| Markierer | Markierer | Der Suchergebnis‑Markierer. |
| Optionen | HighlightOptions | Die Hervorhebungsoptionen. |

### Beispiele

Das Beispiel zeigt, wie Vorkommen in HTML‑formatiertem Text hervorgehoben werden.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentFolder = @"c:\MyDocuments\";

// Erstellen eines Index
Index index = new Index(indexFolder);

// Indizierung von Dokumenten aus dem angegebenen Ordner
index.Add(documentFolder);

// Suche nach dem Wort 'eternity'
SearchResult result = index.Search("eternity");

// Hervorheben von Vorkommen im Text
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

### Siehe auch

* class [FoundDocument](../../../groupdocs.search.results/founddocument)
* class [Highlighter](../../../groupdocs.search.highlighters/highlighter)
* class [HighlightOptions](../../../groupdocs.search.options/highlightoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
