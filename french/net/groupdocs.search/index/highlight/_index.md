---
title: "Surlignage"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Génère du texte formaté en HTML avec les termes trouvés mis en évidence."
type: docs
weight: 210
url: /fr/net/groupdocs.search/index/highlight/
---
## Highlight(FoundDocument, Highlighter) {#highlight}

Génère du texte formaté en HTML avec les termes trouvés mis en évidence.

```csharp
public void Highlight(FoundDocument document, Highlighter highlighter)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| document | FoundDocument | Le document trouvé. |
| surligneur | Surligneur | Le surligneur de résultats de recherche. |

### Exemples

L'exemple montre comment surligner les occurrences dans du texte formaté en HTML.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentFolder = @"c:\MyDocuments\";

// Création d'un index
Index index = new Index(indexFolder);

// Indexation des documents depuis le dossier spécifié
index.Add(documentFolder);

// Rechercher le mot 'eternity'
SearchResult result = index.Search("eternity");

// Surlignage des occurrences dans le texte
if (result.DocumentCount > 0)
{
    FoundDocument document = result.GetFoundDocument(0); // Getting the first found document
    OutputAdapter outputAdapter = new FileOutputAdapter(@"c:\Highlighted.html"); // Creating an output adapter to the file
    Highlighter highlighter = new HtmlHighlighter(outputAdapter); // Creating the highlighter object
    index.Highlight(document, highlighter); // Generating HTML formatted text with highlighted occurrences
}
```

### Voir aussi

* class [FoundDocument](../../../groupdocs.search.results/founddocument)
* class [Highlighter](../../../groupdocs.search.highlighters/highlighter)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Highlight(FoundDocument, Highlighter, HighlightOptions) {#highlight_1}

Génère du texte formaté en HTML avec les termes trouvés mis en évidence.

```csharp
public void Highlight(FoundDocument document, Highlighter highlighter, HighlightOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| document | FoundDocument | Le document trouvé. |
| surligneur | Surligneur | Le surligneur de résultats de recherche. |
| options | HighlightOptions | Les options de surlignage. |

### Exemples

L'exemple montre comment surligner les occurrences dans du texte formaté en HTML.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentFolder = @"c:\MyDocuments\";

// Création d'un index
Index index = new Index(indexFolder);

// Indexation des documents depuis le dossier spécifié
index.Add(documentFolder);

// Rechercher le mot 'eternity'
SearchResult result = index.Search("eternity");

// Surlignage des occurrences dans le texte
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

### Voir aussi

* class [FoundDocument](../../../groupdocs.search.results/founddocument)
* class [Highlighter](../../../groupdocs.search.highlighters/highlighter)
* class [HighlightOptions](../../../groupdocs.search.options/highlightoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
