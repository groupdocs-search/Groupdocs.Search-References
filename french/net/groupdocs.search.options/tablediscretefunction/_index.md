---
title: "TableDiscreteFunction"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Représente l'algorithme de recherche floue qui contient des correspondances entre les longueurs de mots et le nombre d'erreurs autorisées. Cet algorithme peut être spécifié par un tableau de valeurs de sortie ou par une fonction d'étape."
type: docs
weight: 1170
url: /fr/net/groupdocs.search.options/tablediscretefunction/
---
## TableDiscreteFunction class

Représente l'algorithme de recherche floue qui contient des correspondances entre les longueurs de mots et le nombre d'erreurs autorisées. Cet algorithme peut être spécifié par un tableau de valeurs de sortie ou par une fonction d'étape.

```csharp
public class TableDiscreteFunction : FuzzyAlgorithm
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [TableDiscreteFunction](tablediscretefunction#constructor_1)(int, int[]) | Initialise une nouvelle instance de la classe [`TableDiscreteFunction`](../tablediscretefunction). |
| [TableDiscreteFunction](tablediscretefunction#constructor)(int, params Step[]) | Initialise une nouvelle instance de la classe [`TableDiscreteFunction`](../tablediscretefunction). |

## Méthodes

| Nom | Description |
| --- | --- |
| override [GetMaxMistakeCount](../../groupdocs.search.options/tablediscretefunction/getmaxmistakecount)(int) | Obtient le nombre maximal d'erreurs autorisé pour la longueur de terme spécifiée. |
| override [GetSimilarityLevel](../../groupdocs.search.options/tablediscretefunction/getsimilaritylevel)(int) | Obtient le niveau de similarité pour la longueur de terme spécifiée. |

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
options.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1, new Step(5, 2), new Step(8, 3)); // Creating the fuzzy search algorithm
// Cette fonction spécifie 1 comme nombre maximal d'erreurs pour les mots de 1 à 4 caractères.
// Elle spécifie 2 comme nombre maximal d'erreurs pour les mots de 5 à 7 caractères.
// Elle spécifie 3 comme nombre maximal d'erreurs pour les mots de 8 caractères et plus.

SearchResult result = index.Search(query, options); // Search in index
```

### Voir aussi

* class [FuzzyAlgorithm](../fuzzyalgorithm)
* namespace [GroupDocs.Search.Options](../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
