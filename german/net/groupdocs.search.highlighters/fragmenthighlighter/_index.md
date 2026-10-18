---
title: "FragmentHighlighter"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Stellt einen Suchergebnis‑Highlighter dar, der Suchergebnisse in Textfragmenten hervorhebt."
type: docs
weight: 680
url: /de/net/groupdocs.search.highlighters/fragmenthighlighter/
---
## FragmentHighlighter class

Stellt einen Suchergebnis‑Highlighter dar, der Suchergebnisse in Textfragmenten hervorhebt.

```csharp
public class FragmentHighlighter : Highlighter
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [FragmentHighlighter](fragmenthighlighter)(OutputFormat) | Initialisiert eine neue Instanz der Klasse [`FragmentHighlighter`](../fragmenthighlighter). |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [OutputFormat](../../groupdocs.search.common/resultbuilderfactory/outputformat) { get; } | Liefert das Ausgabeformat. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [GetResult](../../groupdocs.search.highlighters/fragmenthighlighter/getresult)() | Liefert ein Array der resultierenden Fragmentcontainer. |

### Hinweise

**Learn more**

* [Highlighting search results](https://docs.groupdocs.com/display/searchnet/Highlighting+search+results)

### Beispiele

Das Beispiel zeigt eine typische Verwendung der Klasse.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

// Erstellen eines Index
Index index = new Index(indexFolder);

// Indizierung von Dokumenten aus dem angegebenen Ordner
index.Add(documentsFolder);

// Suche nach dem Wort 'Einstein'
SearchResult result = index.Search("Einstein");

// Zuweisen von Hervorhebungsoptionen
HighlightOptions options = new HighlightOptions();
options.TermsBefore = 5;
options.TermsAfter = 5;
options.TermsTotal = 15;

// Markieren gefundener Wörter im Text eines Dokuments
FoundDocument document = result.GetFoundDocument(0);
FragmentHighlighter highlighter = new FragmentHighlighter(OutputFormat.Html);
index.Highlight(document, highlighter, options);

// Abrufen des Ergebnisses
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
            // Ausgabe von HTML-Markup in die Konsole
            Console.WriteLine(fragments[j]);
            Console.WriteLine();
        }
    }
}
```

### Siehe auch

* class [Highlighter](../highlighter)
* namespace [GroupDocs.Search.Highlighters](../../groupdocs.search.highlighters)
* assembly [GroupDocs.Search](../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
