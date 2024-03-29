---
title: HtmlHighlighter
second_title: GroupDocs. Zoek naar .NET API-referentie
description: Vertegenwoordigt een markeerstift voor zoekresultaten die zoekresultaten markeert in een volledige documenttekst die is opgemaakt in HTML.
type: docs
weight: 670
url: /nl/net/groupdocs.search.highlighters/htmlhighlighter/
---
## HtmlHighlighter class

Vertegenwoordigt een markeerstift voor zoekresultaten die zoekresultaten markeert in een volledige documenttekst die is opgemaakt in HTML.

```csharp
[Obsolete("Please, use the DocumentHighlighter class instead.")]
public class HtmlHighlighter : Highlighter
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [OutputFormat](../../groupdocs.search.common/resultbuilderfactory/outputformat) { get; } | Haalt het uitvoerformaat op. |

### Opmerkingen

**Kom meer te weten**

* [Zoekresultaten markeren](https://docs.groupdocs.com/display/searchnet/Highlighting+search+results)

### Voorbeelden

Het voorbeeld demonstreert een typisch gebruik van de klasse.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

// Een index maken
Index index = new Index(indexFolder);

// Documenten uit de opgegeven map indexeren
index.Add(documentsFolder);

// Zoek naar de fase 'Relativiteitstheorie'
SearchResult result = index.Search("\"Theory of Relativity\"");

// Gevonden woorden in de tekst van een document markeren
FoundDocument document = result.GetFoundDocument(0);
OutputAdapter outputAdapter = new FileOutputAdapter(OutputFormat.Html, "Highlighted.html");
Highlighter highlighter = new HtmlHighlighter(outputAdapter);
index.Highlight(document, highlighter);
```

### Zie ook

* class [Highlighter](../highlighter)
* naamruimte [GroupDocs.Search.Highlighters](../../groupdocs.search.highlighters)
* montage [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
