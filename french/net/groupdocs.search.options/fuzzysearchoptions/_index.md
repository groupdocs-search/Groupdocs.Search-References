---
title: "FuzzySearchOptions"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Fournit des options de la recherche floue."
type: docs
weight: 900
url: /fr/net/groupdocs.search.options/fuzzysearchoptions/
---
## FuzzySearchOptions class

Fournit des options de la recherche floue.

```csharp
public class FuzzySearchOptions
```

## Propriétés

| Nom | Description |
| --- | --- |
| [ConsiderTranspositions](../../groupdocs.search.options/fuzzysearchoptions/considertranspositions) { get; set; } | Obtient ou définit une valeur indiquant si l'algorithme de recherche floue doit considérer la transposition de deux caractères adjacents comme une seule erreur. La valeur par défaut est `true`. |
| [Enabled](../../groupdocs.search.options/fuzzysearchoptions/enabled) { get; set; } | Obtient ou définit une valeur indiquant si la fonction de recherche floue est activée. La valeur par défaut est `false`. |
| [FuzzyAlgorithm](../../groupdocs.search.options/fuzzysearchoptions/fuzzyalgorithm) { get; set; } | Obtient ou définit l'algorithme de recherche floue. Les algorithmes de recherche floue actuellement disponibles sont [`SimilarityLevel`](../similaritylevel) et [`TableDiscreteFunction`](../tablediscretefunction). La valeur par défaut est une instance de [`SimilarityLevel`](../similaritylevel) avec une valeur de niveau de similarité de `0.5`. |
| [OnlyBestResults](../../groupdocs.search.options/fuzzysearchoptions/onlybestresults) { get; set; } | Obtient ou définit une valeur indiquant si seuls les meilleurs résultats seront renvoyés. La valeur par défaut est `false`. |
| [OnlyBestResultsRange](../../groupdocs.search.options/fuzzysearchoptions/onlybestresultsrange) { get; set; } | Obtient ou définit le dépassement maximal du nombre minimum d'erreurs qui sont trouvées. La valeur par défaut est `0`. |

### Remarques

**Learn more**

* [Fuzzy search](https://docs.groupdocs.com/display/searchnet/Fuzzy+search)
* [Search options](https://docs.groupdocs.com/display/searchnet/Search+options)

### Voir aussi

* namespace [GroupDocs.Search.Options](../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
