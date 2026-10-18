---
title: "SearchResult"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Stellt ein Suchergebnis dar, das zu einer Suchanfrage passt."
type: docs
weight: 1310
url: /de/net/groupdocs.search.results/searchresult/
---
## SearchResult class

Stellt ein Suchergebnis dar, das zu einer Suchanfrage passt.

```csharp
public class SearchResult : IEnumerable<FoundDocument>
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [DocumentCount](../../groupdocs.search.results/searchresult/documentcount) { get; } | Ruft die Anzahl gefundener Dokumente ab. |
| [EndTime](../../groupdocs.search.results/searchresult/endtime) { get; } | Ruft die Endzeit der Suche ab. |
| [NextChunkSearchToken](../../groupdocs.search.results/searchresult/nextchunksearchtoken) { get; } | Gibt ein Chunk‑Suche‑Token zum Suchen des nächsten Chunks zurück. |
| [OccurrenceCount](../../groupdocs.search.results/searchresult/occurrencecount) { get; } | Ruft die Gesamtzahl gefundener Vorkommen ab. |
| [SearchDuration](../../groupdocs.search.results/searchresult/searchduration) { get; } | Ruft die Suchdauer ab. |
| [StartTime](../../groupdocs.search.results/searchresult/starttime) { get; } | Ruft die Startzeit der Suche ab. |
| [Truncated](../../groupdocs.search.results/searchresult/truncated) { get; } | Gibt einen Wert zurück, der anzeigt, dass das Ergebnis abgeschnitten ist. |
| [Warnings](../../groupdocs.search.results/searchresult/warnings) { get; } | Gibt eine Warnung zurück, die das Ergebnis beschreibt. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [GetEnumerator](../../groupdocs.search.results/searchresult/getenumerator)() | Gibt einen Enumerator zurück, der durch die Sammlung der gefundenen Dokumente iteriert. |
| [GetFoundDocument](../../groupdocs.search.results/searchresult/getfounddocument)(int) | Gibt das gefundene Dokument nach Index zurück. |

### Hinweise

**Learn more**

* [Searching](https://docs.groupdocs.com/display/searchnet/Searching)
* [Search results](https://docs.groupdocs.com/display/searchnet/Search+results)

### Beispiele

Das Beispiel zeigt eine typische Verwendung der Klasse.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentFolder = @"c:\MyDocuments\";

// Erstellen eines Index
Index index = new Index(indexFolder);

// Indizierung von Dokumenten aus dem angegebenen Ordner
index.Add(documentFolder);

// Festlegen von Suchoptionen
SearchOptions options = new SearchOptions();
options.FuzzySearch.Enabled = true; // Enabling the fuzzy search
options.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(3); // Setting the maximum number of differences to 3

// Suche nach Dokumenten, die das Wort 'Einstein' oder die Phrase 'Theory of Relativity' enthalten
SearchResult result = index.Search("Einstein OR \"Theory of Relativity\"", options);

// Ausgabe des Ergebnisses
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
        // Ausgabe gefundener Begriffe
        if (field.Terms != null)
        {
            for (int k = 0; k < field.Terms.Length; k++)
            {
                Console.WriteLine("\t\t\t" + field.Terms[k].PadRight(20) + field.TermsOccurrences[k]);
            }
        }
        // Ausgabe gefundener Phrasen
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

### Siehe auch

* class [FoundDocument](../founddocument)
* namespace [GroupDocs.Search.Results](../../groupdocs.search.results)
* assembly [GroupDocs.Search](../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
