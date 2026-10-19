---
title: "FuzzyAlgorithm"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Ottiene o imposta l'algoritmo di ricerca fuzzy. Gli algoritmi di ricerca fuzzy attualmente disponibili sono SimilarityLevelgroupdocs.search.options/similaritylevel e TableDiscreteFunctiongroupdocs.search.options/tablediscretefunction. Il valore predefinito è un'istanza di SimilarityLevelgroupdocs.search.options/similaritylevel con un valore di livello di similarità di 0.5."
type: docs
weight: 30
url: /it/net/groupdocs.search.options/fuzzysearchoptions/fuzzyalgorithm/
---
## FuzzySearchOptions.FuzzyAlgorithm property

Ottiene o imposta l'algoritmo di ricerca fuzzy. Gli algoritmi di ricerca fuzzy attualmente disponibili sono [`SimilarityLevel`](../../similaritylevel) e [`TableDiscreteFunction`](../../tablediscretefunction). Il valore predefinito è un'istanza di [`SimilarityLevel`](../../similaritylevel) con un valore di livello di similarità di `0.5`.

```csharp
public FuzzyAlgorithm FuzzyAlgorithm { get; set; }
```

### Property Value

L'algoritmo di ricerca fuzzy.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | Generata quando *value* è `null`. |

### Esempi

L'esempio dimostra come impostare l'algoritmo di ricerca fuzzy.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // Creating an index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

SearchOptions options = new SearchOptions();
options.FuzzySearch.Enabled = true; // Enabling the fuzzy search
options.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1, new Step(5, 2), new Step(8, 3)); // Creating the fuzzy search algorithm
// Questa funzione specifica 1 come numero massimo di errori per parole da 1 a 4 caratteri.
// Specifica 2 come numero massimo di errori per parole da 5 a 7 caratteri.
// Specifica 3 come numero massimo di errori per parole di 8 o più caratteri.

SearchResult result = index.Search(query, options); // Search in index
```

### Vedi anche

* class [FuzzyAlgorithm](../../fuzzyalgorithm)
* class [FuzzySearchOptions](../../fuzzysearchoptions)
* namespace [GroupDocs.Search.Options](../../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
