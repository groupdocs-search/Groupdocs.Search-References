---
title: HtmlFragmentHighlighter
second_title: GroupDocs.Search efter .NET API Reference
description: Representerar en överstrykning av sökresultat som framhäver sökresultat i HTMLformaterade textfragment.
type: docs
weight: 630
url: /sv/net/groupdocs.search.highlighters/htmlfragmenthighlighter/
---
## HtmlFragmentHighlighter class

Representerar en överstrykning av sökresultat som framhäver sökresultat i HTML-formaterade textfragment.

```csharp
public class HtmlFragmentHighlighter : Highlighter
```

## Konstruktörer

| namn | Beskrivning |
| --- | --- |
| [HtmlFragmentHighlighter](htmlfragmenthighlighter)() | Initierar en ny instans av[`HtmlFragmentHighlighter`](../htmlfragmenthighlighter) class. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| [GetResult](../../groupdocs.search.highlighters/htmlfragmenthighlighter/getresult)() | Får en array av resulterande fragmentbehållare. |

### Anmärkningar

**Läs mer**

* [Markera sökresultat](https://docs.groupdocs.com/display/searchnet/Highlighting+search+results)

### Exempel

Exemplet visar en typisk användning av klassen.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

// Skapa ett index
Index index = new Index(indexFolder);

// Indexering av dokument från den angivna mappen
index.Add(documentsFolder);

// Sök efter ordet 'Einstein'
SearchResult result = index.Search("Einstein");

// Tilldela markeringsalternativ
HighlightOptions options = new HighlightOptions();
options.TermsBefore = 5;
options.TermsAfter = 5;
options.TermsTotal = 15;

// Markera hittade ord i texten i ett dokument
FoundDocument document = result.GetFoundDocument(0);
HtmlFragmentHighlighter highlighter = new HtmlFragmentHighlighter();
index.Highlight(document, highlighter, options);

// Får resultatet
FragmentContainer[] fragmentContainers = highlighter.GetResult();
for (int i = 0; i < fragmentContainers.Length; i++)
{
    FragmentContainer container = fragmentContainers[i];
    string[] fragments = container.GetFragments();
    if (fragments.Length > 0)
    {
        Console.WriteLine(container.FieldName);
        Console.WriteLine();
        for (int j = 0; j < fragments.Length; j++)
        {
            // Skriver ut HTML-kod till konsolen
            Console.WriteLine(fragments[j]);
            Console.WriteLine();
        }
    }
}
```

### Se även

* class [Highlighter](../highlighter)
* namnutrymme [GroupDocs.Search.Highlighters](../../groupdocs.search.highlighters)
* hopsättning [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->