---
title: "FuzzyAlgorithm"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Obtient ou définit l'algorithme de recherche floue. Les algorithmes de recherche floue actuellement disponibles sont SimilarityLevelgroupdocs.search.options/similaritylevel et TableDiscreteFunctiongroupdocs.search.options/tablediscretefunction. La valeur par défaut est une instance de SimilarityLevelgroupdocs.search.options/similaritylevel avec une valeur de niveau de similarité de 0.5."
type: docs
weight: 30
url: /fr/net/groupdocs.search.options/fuzzysearchoptions/fuzzyalgorithm/
---
## FuzzySearchOptions.FuzzyAlgorithm property

Obtient ou définit l'algorithme de recherche floue. Les algorithmes de recherche floue actuellement disponibles sont [`SimilarityLevel`](../../similaritylevel) et [`TableDiscreteFunction`](../../tablediscretefunction). La valeur par défaut est une instance de [`SimilarityLevel`](../../similaritylevel) avec une valeur de niveau de similarité de `0.5`.

```csharp
public FuzzyAlgorithm FuzzyAlgorithm { get; set; }
```

### Property Value

L'algorithme de recherche floue.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | Lancé lorsque *value* est `null`. |

### Exemples

L'exemple montre comment définir l'algorithme de recherche floue.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // Creating an index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

SearchOptions options = new SearchOptions();
options.FuzzySearch.Enabled = true; // Enabling the fuzzy search
options.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1, new Step(5, 2), new Step(8, 3)); // Creating the fuzzy search algorithm
// Cette fonction spécifie 1 comme nombre maximal d'erreurs pour les mots de 1 à 4 caractères.
// Elle spécifie 2 comme nombre maximal d'erreurs pour les mots de 5 à 7 caractères.
// Elle spécifie 3 comme nombre maximal d'erreurs pour les mots de 8 caractères et plus.

SearchResult result = index.Search(query, options); // Search in index
```

### Voir aussi

* class [FuzzyAlgorithm](../../fuzzyalgorithm)
* class [FuzzySearchOptions](../../fuzzysearchoptions)
* namespace [GroupDocs.Search.Options](../../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
