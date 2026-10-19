---
title: "FuzzySearchOptions"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Fornisce opzioni della ricerca fuzzy."
type: docs
weight: 900
url: /it/net/groupdocs.search.options/fuzzysearchoptions/
---
## FuzzySearchOptions class

Fornisce opzioni della ricerca fuzzy.

```csharp
public class FuzzySearchOptions
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [ConsiderTranspositions](../../groupdocs.search.options/fuzzysearchoptions/considertranspositions) { get; set; } | Ottiene o imposta un valore che indica se l'algoritmo di ricerca fuzzy deve considerare la trasposizione di due caratteri adiacenti come un unico errore. Il valore predefinito è `true`. |
| [Enabled](../../groupdocs.search.options/fuzzysearchoptions/enabled) { get; set; } | Ottiene o imposta un valore che indica se la funzionalità di ricerca fuzzy è abilitata. Il valore predefinito è `false`. |
| [FuzzyAlgorithm](../../groupdocs.search.options/fuzzysearchoptions/fuzzyalgorithm) { get; set; } | Ottiene o imposta l'algoritmo di ricerca fuzzy. Gli algoritmi di ricerca fuzzy attualmente disponibili sono [`SimilarityLevel`](../similaritylevel) e [`TableDiscreteFunction`](../tablediscretefunction). Il valore predefinito è un'istanza di [`SimilarityLevel`](../similaritylevel) con un valore di livello di similarità di `0.5`. |
| [OnlyBestResults](../../groupdocs.search.options/fuzzysearchoptions/onlybestresults) { get; set; } | Ottiene o imposta un valore che indica se verranno restituiti solo i risultati migliori. Il valore predefinito è `false`. |
| [OnlyBestResultsRange](../../groupdocs.search.options/fuzzysearchoptions/onlybestresultsrange) { get; set; } | Ottiene o imposta il superamento massimo del numero minimo di errori rilevati. Il valore predefinito è `0`. |

### Osservazioni

**Learn more**

* [Fuzzy search](https://docs.groupdocs.com/display/searchnet/Fuzzy+search)
* [Search options](https://docs.groupdocs.com/display/searchnet/Search+options)

### Vedi anche

* namespace [GroupDocs.Search.Options](../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
