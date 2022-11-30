---
title: TableDiscreteFunction
second_title: GroupDocs.Search efter .NET API Reference
description: Representerar den otydliga sökalgoritmen som innehåller överensstämmelse mellan ordlängder och antalet tillåtna misstag. Denna algoritm kan specificeras av en tabell med utdatavärden eller av en stegfunktion.
type: docs
weight: 1050
url: /sv/net/groupdocs.search.options/tablediscretefunction/
---
## TableDiscreteFunction class

Representerar den otydliga sökalgoritmen som innehåller överensstämmelse mellan ordlängder och antalet tillåtna misstag. Denna algoritm kan specificeras av en tabell med utdatavärden eller av en stegfunktion.

```csharp
public class TableDiscreteFunction : FuzzyAlgorithm
```

## Konstruktörer

| namn | Beskrivning |
| --- | --- |
| [TableDiscreteFunction](tablediscretefunction#constructor_1)(int, int[]) | Initierar en ny instans av[`TableDiscreteFunction`](../tablediscretefunction) class. |
| [TableDiscreteFunction](tablediscretefunction#constructor)(int, params Step[]) | Initierar en ny instans av[`TableDiscreteFunction`](../tablediscretefunction) class. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| override [GetMaxMistakeCount](../../groupdocs.search.options/tablediscretefunction/getmaxmistakecount)(int) | Får ett maximalt tillåtet antal misstag för angiven termlängd. |
| override [GetSimilarityLevel](../../groupdocs.search.options/tablediscretefunction/getsimilaritylevel)(int) | Får en likhetsnivå för angiven termlängd. |

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
options.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1, new Step(5, 2), new Step(8, 3)); // Skapar den suddiga sökalgoritmen
// Denna funktion anger 1 som det maximala antalet misstag för ord från 1 till 4 tecken.
// Den anger 2 som det maximala antalet misstag för ord från 5 till 7 tecken.
// Den anger 3 som det maximala antalet misstag för ord från 8 eller fler tecken.

SearchResult result = index.Search(query, options); // Sök i index
```

### Se även

* class [FuzzyAlgorithm](../fuzzyalgorithm)
* namnutrymme [GroupDocs.Search.Options](../../groupdocs.search.options)
* hopsättning [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->