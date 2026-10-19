---
title: "SearchResult"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Rappresenta un risultato di ricerca corrispondente a una query di ricerca."
type: docs
weight: 1310
url: /it/net/groupdocs.search.results/searchresult/
---
## SearchResult class

Rappresenta un risultato di ricerca corrispondente a una query di ricerca.

```csharp
public class SearchResult : IEnumerable<FoundDocument>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [DocumentCount](../../groupdocs.search.results/searchresult/documentcount) { get; } | Ottiene il numero di documenti trovati. |
| [EndTime](../../groupdocs.search.results/searchresult/endtime) { get; } | Ottiene l'ora di fine della ricerca. |
| [NextChunkSearchToken](../../groupdocs.search.results/searchresult/nextchunksearchtoken) { get; } | Ottiene un token di ricerca a blocchi per cercare il blocco successivo. |
| [OccurrenceCount](../../groupdocs.search.results/searchresult/occurrencecount) { get; } | Ottiene il numero totale di occorrenze trovate. |
| [SearchDuration](../../groupdocs.search.results/searchresult/searchduration) { get; } | Ottiene la durata della ricerca. |
| [StartTime](../../groupdocs.search.results/searchresult/starttime) { get; } | Ottiene l'ora di inizio della ricerca. |
| [Truncated](../../groupdocs.search.results/searchresult/truncated) { get; } | Ottiene un valore che indica che il risultato è troncato. |
| [Warnings](../../groupdocs.search.results/searchresult/warnings) { get; } | Ottiene gli avvisi che descrivono il risultato. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [GetEnumerator](../../groupdocs.search.results/searchresult/getenumerator)() | Restituisce un enumeratore che itera attraverso la raccolta dei documenti trovati. |
| [GetFoundDocument](../../groupdocs.search.results/searchresult/getfounddocument)(int) | Ottiene il documento trovato per indice. |

### Osservazioni

**Learn more**

* [Searching](https://docs.groupdocs.com/display/searchnet/Searching)
* [Search results](https://docs.groupdocs.com/display/searchnet/Search+results)

### Esempi

L'esempio dimostra un utilizzo tipico della classe.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentFolder = @"c:\MyDocuments\";

// Creazione di un indice
Index index = new Index(indexFolder);

// Indicizzazione dei documenti dalla cartella specificata
index.Add(documentFolder);

// Impostazione delle opzioni di ricerca
SearchOptions options = new SearchOptions();
options.FuzzySearch.Enabled = true; // Enabling the fuzzy search
options.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(3); // Setting the maximum number of differences to 3

// Cerca documenti contenenti la parola 'Einstein' o la frase 'Theory of Relativity'
SearchResult result = index.Search("Einstein OR \"Theory of Relativity\"", options);

// Stampa del risultato
Console.WriteLine("Documents: " + result.DocumentCount);
Console.WriteLine("Total occurrences: " + result.OccurrenceCount);
for (int i = 0; i < result.DocumentCount; i++)
{
    FoundDocument document = result.GetFoundDocument(i);
    Console.WriteLine("\tDocument: " + document.DocumentInfo.FilePath);
    Console.WriteLine("\tOccurrences: " + document.OccurrenceCount);
    for (int j = 0; j < document.FoundFields.Length; j++)
    {
        FoundDocumentField field = document.FoundFields[j];
        Console.WriteLine("\t\tField: " + field.FieldName);
        Console.WriteLine("\t\tOccurrences: " + document.OccurrenceCount);
        // Stampa dei termini trovati
        if (field.Terms != null)
        {
            for (int k = 0; k < field.Terms.Length; k++)
            {
                Console.WriteLine("\t\t\t" + field.Terms[k].PadRight(20) + field.TermsOccurrences[k]);
            }
        }
        // Stampa delle frasi trovate
        if (field.TermSequences != null)
        {
            for (int k = 0; k < field.TermSequences.Length; k++)
            {
                string sequence = string.Join(" ", field.TermSequences[k]);
                Console.WriteLine("\t\t\t" + sequence.PadRight(30) + field.TermSequencesOccurrences[k]);
            }
        }
    }
}
```

### Vedi anche

* class [FoundDocument](../founddocument)
* namespace [GroupDocs.Search.Results](../../groupdocs.search.results)
* assembly [GroupDocs.Search](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
