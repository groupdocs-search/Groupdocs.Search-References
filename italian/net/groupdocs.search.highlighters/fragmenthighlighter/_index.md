---
title: "FragmentHighlighter"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Rappresenta un evidenziatore di risultati di ricerca che evidenzia i risultati di ricerca in frammenti di testo."
type: docs
weight: 680
url: /it/net/groupdocs.search.highlighters/fragmenthighlighter/
---
## FragmentHighlighter class

Rappresenta un evidenziatore di risultati di ricerca che evidenzia i risultati di ricerca in frammenti di testo.

```csharp
public class FragmentHighlighter : Highlighter
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [FragmentHighlighter](fragmenthighlighter)(OutputFormat) | Inizializza una nuova istanza della classe [`FragmentHighlighter`](../fragmenthighlighter). |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [OutputFormat](../../groupdocs.search.common/resultbuilderfactory/outputformat) { get; } | Restituisce il formato di output. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [GetResult](../../groupdocs.search.highlighters/fragmenthighlighter/getresult)() | Ottiene un array di contenitori di frammenti risultanti. |

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

// Cerca la parola 'Einstein'
SearchResult result = index.Search("Einstein");

// Assegnazione delle opzioni di evidenziazione
HighlightOptions options = new HighlightOptions();
options.TermsBefore = 5;
options.TermsAfter = 5;
options.TermsTotal = 15;

// Evidenzia le parole trovate nel testo di un documento
FoundDocument document = result.GetFoundDocument(0);
FragmentHighlighter highlighter = new FragmentHighlighter(OutputFormat.Html);
index.Highlight(document, highlighter, options);

// Ottenere il risultato
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
            // Stampa il markup HTML sulla console
            Console.WriteLine(fragments[j]);
            Console.WriteLine();
        }
    }
}
```

### Vedi anche

* class [Highlighter](../highlighter)
* namespace [GroupDocs.Search.Highlighters](../../groupdocs.search.highlighters)
* assembly [GroupDocs.Search](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
