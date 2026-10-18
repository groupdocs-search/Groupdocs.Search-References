---
title: "FuzzySearchOptions"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Stellt Optionen für die Fuzzy-Suche bereit."
type: docs
weight: 900
url: /de/net/groupdocs.search.options/fuzzysearchoptions/
---
## FuzzySearchOptions class

Stellt Optionen für die Fuzzy-Suche bereit.

```csharp
public class FuzzySearchOptions
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [ConsiderTranspositions](../../groupdocs.search.options/fuzzysearchoptions/considertranspositions) { get; set; } | Ruft den Wert ab oder legt ihn fest, der angibt, ob der Fuzzy-Search-Algorithmus die Vertauschung zweier benachbarter Zeichen als einen einzigen Fehler berücksichtigen muss. Der Standardwert ist `true`. |
| [Enabled](../../groupdocs.search.options/fuzzysearchoptions/enabled) { get; set; } | Ruft den Wert ab oder legt ihn fest, der angibt, ob die Fuzzy-Search-Funktion aktiviert ist. Der Standardwert ist `false`. |
| [FuzzyAlgorithm](../../groupdocs.search.options/fuzzysearchoptions/fuzzyalgorithm) { get; set; } | Ruft den Fuzzy-Search-Algorithmus ab oder legt ihn fest. Die derzeit verfügbaren Fuzzy-Search-Algorithmen sind [`SimilarityLevel`](../similaritylevel) und [`TableDiscreteFunction`](../tablediscretefunction). Der Standardwert ist eine Instanz von [`SimilarityLevel`](../similaritylevel) mit einem Ähnlichkeitsgrad von `0.5`. |
| [OnlyBestResults](../../groupdocs.search.options/fuzzysearchoptions/onlybestresults) { get; set; } | Liest oder setzt einen Wert, der angibt, ob nur die besten Ergebnisse zurückgegeben werden. Der Standardwert ist `false`. |
| [OnlyBestResultsRange](../../groupdocs.search.options/fuzzysearchoptions/onlybestresultsrange) { get; set; } | Liest oder setzt die maximale Überschreitung der minimal gefundenen Fehleranzahl. Der Standardwert ist `0`. |

### Hinweise

**Learn more**

* [Fuzzy search](https://docs.groupdocs.com/display/searchnet/Fuzzy+search)
* [Search options](https://docs.groupdocs.com/display/searchnet/Search+options)

### Siehe auch

* namespace [GroupDocs.Search.Options](../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
