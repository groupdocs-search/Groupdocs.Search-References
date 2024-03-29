---
title: SimilarityLevel
second_title: GroupDocs.Search efter .NET API Reference
description: Representerar en algoritm för den otydliga sökningen som anger likhetsnivån. Likhetsnivåalgoritmen beräknar det maximala antalet misstag för ett ord som omvänt proportionell mot ordlängden.
type: docs
weight: 1050
url: /sv/net/groupdocs.search.options/similaritylevel/
---
## SimilarityLevel class

Representerar en algoritm för den otydliga sökningen som anger likhetsnivån. Likhetsnivåalgoritmen beräknar det maximala antalet misstag för ett ord som omvänt proportionell mot ordlängden.

```csharp
public class SimilarityLevel : FuzzyAlgorithm
```

## Konstruktörer

| namn | Beskrivning |
| --- | --- |
| [SimilarityLevel](similaritylevel)(double) | Initierar en ny instans av[`SimilarityLevel`](../similaritylevel) class. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| override [GetMaxMistakeCount](../../groupdocs.search.options/similaritylevel/getmaxmistakecount)(int) | Får det högsta tillåtna antalet misstag för den angivna termlängden. |
| override [GetSimilarityLevel](../../groupdocs.search.options/similaritylevel/getsimilaritylevel)(int) | Hämtar likhetsnivåvärdet för den angivna termlängden. |

### Anmärkningar

**Läs mer**

* [Luddrig sökning](https://docs.groupdocs.com/display/searchnet/Fuzzy+search)

### Exempel

Exemplet visar en typisk användning av klassen.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // Skapar ett index i den angivna mappen
index.Add(documentsFolder); // Indexering av dokument från den angivna mappen

SearchOptions options = new SearchOptions();
options.FuzzySearch.Enabled = true; // Aktiverar den otydliga sökningen
options.FuzzySearch.FuzzyAlgorithm = new SimilarityLevel(0.8); // Skapar den suddiga sökalgoritmen
// Denna funktion anger 0 som det maximala antalet misstag för ord från 1 till 4 tecken.
// Den anger 1 som det maximala antalet misstag för ord från 5 till 9 tecken.
// Den anger 2 som det maximala antalet misstag för ord från 10 till 14 tecken. Och så vidare.

SearchResult result = index.Search(query, options); // Sök i index
```

### Se även

* class [FuzzyAlgorithm](../fuzzyalgorithm)
* namnutrymme [GroupDocs.Search.Options](../../groupdocs.search.options)
* hopsättning [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
