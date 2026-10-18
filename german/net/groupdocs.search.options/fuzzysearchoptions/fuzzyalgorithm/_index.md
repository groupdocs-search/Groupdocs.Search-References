---
title: "FuzzyAlgorithm"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Ruft den Fuzzy‑Suchalgorithmus ab oder legt ihn fest. Die derzeit verfügbaren Fuzzy‑Suchalgorithmen sind SimilarityLevelgroupdocs.search.options/similaritylevel und TableDiscreteFunctiongroupdocs.search.options/tablediscretefunction. Der Standardwert ist eine Instanz von SimilarityLevelgroupdocs.search.options/similaritylevel mit einem Ähnlichkeitsgrad von 0.5."
type: docs
weight: 30
url: /de/net/groupdocs.search.options/fuzzysearchoptions/fuzzyalgorithm/
---
## FuzzySearchOptions.FuzzyAlgorithm property

Ruft den Fuzzy‑Suchalgorithmus ab oder legt ihn fest. Die derzeit verfügbaren Fuzzy‑Suchalgorithmen sind [`SimilarityLevel`](../../similaritylevel) und [`TableDiscreteFunction`](../../tablediscretefunction). Der Standardwert ist eine Instanz von [`SimilarityLevel`](../../similaritylevel) mit einem Ähnlichkeitsgrad von `0.5`.

```csharp
public FuzzyAlgorithm FuzzyAlgorithm { get; set; }
```

### Property Value

Der Fuzzy‑Suchalgorithmus.

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | Wird ausgelöst, wenn *value* `null` ist. |

### Beispiele

Das Beispiel zeigt, wie der Fuzzy‑Suchalgorithmus festgelegt wird.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // Creating an index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

SearchOptions options = new SearchOptions();
options.FuzzySearch.Enabled = true; // Enabling the fuzzy search
options.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1, new Step(5, 2), new Step(8, 3)); // Creating the fuzzy search algorithm
// Diese Funktion legt 1 als maximale Fehlermenge für Wörter von 1 bis 4 Zeichen fest.
// Sie legt 2 als maximale Fehlermenge für Wörter von 5 bis 7 Zeichen fest.
// Sie legt 3 als maximale Fehlermenge für Wörter von 8 und mehr Zeichen fest.

SearchResult result = index.Search(query, options); // Search in index
```

### Siehe auch

* class [FuzzyAlgorithm](../../fuzzyalgorithm)
* class [FuzzySearchOptions](../../fuzzysearchoptions)
* namespace [GroupDocs.Search.Options](../../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
