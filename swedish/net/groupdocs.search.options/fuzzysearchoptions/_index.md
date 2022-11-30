---
title: FuzzySearchOptions
second_title: GroupDocs.Search efter .NET API Reference
description: Ger alternativ för suddig sökning.
type: docs
weight: 820
url: /sv/net/groupdocs.search.options/fuzzysearchoptions/
---
## FuzzySearchOptions class

Ger alternativ för suddig sökning.

```csharp
public class FuzzySearchOptions
```

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [ConsiderTranspositions](../../groupdocs.search.options/fuzzysearchoptions/considertranspositions) { get; set; } | Hämtar eller ställer in ett värde som indikerar om den suddiga sökalgoritmen måste betrakta transponering av två intilliggande tecken som ett enda misstag. Standardvärdet är`Sann` . |
| [Enabled](../../groupdocs.search.options/fuzzysearchoptions/enabled) { get; set; } | Hämtar eller ställer in ett värde som anger om fuzzy search-funktionen är aktiverad. Standardvärdet är`falsk` . |
| [FuzzyAlgorithm](../../groupdocs.search.options/fuzzysearchoptions/fuzzyalgorithm) { get; set; } | Hämtar eller ställer in fuzzy sökalgoritmen. De för närvarande tillgängliga fuzzy sökalgoritmerna är[`SimilarityLevel`](../similaritylevel) och[`TableDiscreteFunction`](../tablediscretefunction) . Standardvärdet är en instans av[`SimilarityLevel`](../similaritylevel) med ett likhetsnivåvärde på`0,5` . |
| [OnlyBestResults](../../groupdocs.search.options/fuzzysearchoptions/onlybestresults) { get; set; } | Hämtar eller ställer in ett värde som anger om endast de bästa resultaten kommer att returneras. Standardvärdet är`falsk` . |
| [OnlyBestResultsRange](../../groupdocs.search.options/fuzzysearchoptions/onlybestresultsrange) { get; set; } | Hämtar eller ställer in det maximala överskridandet av det minsta antalet misstag som hittas. Standardvärdet är`0` . |

### Anmärkningar

**Läs mer**

* [Luddrig sökning](https://docs.groupdocs.com/display/searchnet/Fuzzy+search)
* [sökmöjligheter](https://docs.groupdocs.com/display/searchnet/Search+options)

### Se även

* namnutrymme [GroupDocs.Search.Options](../../groupdocs.search.options)
* hopsättning [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->