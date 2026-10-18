---
title: "SimilarityLevel"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Représente un algorithme de recherche floue qui spécifie le niveau de similarité. L'algorithme de niveau de similarité calcule le nombre maximal d'erreurs pour un mot proportionnellement inverse à la longueur du mot."
type: docs
weight: 1120
url: /fr/net/groupdocs.search.options/similaritylevel/
---
## SimilarityLevel class

Représente un algorithme de recherche floue qui spécifie le niveau de similarité. L'algorithme de niveau de similarité calcule le nombre maximal d'erreurs pour un mot proportionnellement inverse à la longueur du mot.

```csharp
public class SimilarityLevel : FuzzyAlgorithm
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [SimilarityLevel](similaritylevel)(double) | Initialise une nouvelle instance de la classe [`SimilarityLevel`](../similaritylevel). |

## Méthodes

| Nom | Description |
| --- | --- |
| override [GetMaxMistakeCount](../../groupdocs.search.options/similaritylevel/getmaxmistakecount)(int) | Obtient le nombre maximal d'erreurs autorisées pour la longueur de terme spécifiée. |
| override [GetSimilarityLevel](../../groupdocs.search.options/similaritylevel/getsimilaritylevel)(int) | Obtient la valeur du niveau de similarité pour la longueur de terme spécifiée. |

### Remarques

**Learn more**

* [Fuzzy search](https://docs.groupdocs.com/display/searchnet/Fuzzy+search)

### Exemples

L'exemple montre une utilisation typique de la classe.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // Creating an index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

SearchOptions options = new SearchOptions();
options.FuzzySearch.Enabled = true; // Enabling the fuzzy search
options.FuzzySearch.FuzzyAlgorithm = new SimilarityLevel(0.8); // Creating the fuzzy search algorithm
// Cette fonction spécifie 0 comme nombre maximal d'erreurs pour les mots de 1 à 4 caractères.
// Elle spécifie 1 comme nombre maximal d'erreurs pour les mots de 5 à 9 caractères.
// Elle spécifie 2 comme nombre maximal d'erreurs pour les mots de 10 à 14 caractères. Et ainsi de suite.

SearchResult result = index.Search(query, options); // Search in index
```

### Voir aussi

* class [FuzzyAlgorithm](../fuzzyalgorithm)
* namespace [GroupDocs.Search.Options](../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
