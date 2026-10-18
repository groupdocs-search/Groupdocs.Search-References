---
title: "SimilarityLevel"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Stellt einen Algorithmus der Fuzzy-Suche dar, der den Ähnlichkeitsgrad festlegt. Der Ähnlichkeitsgrad-Algorithmus berechnet die maximale Anzahl von Fehlern für ein Wort als umgekehrt proportional zur Wortlänge."
type: docs
weight: 1120
url: /de/net/groupdocs.search.options/similaritylevel/
---
## SimilarityLevel class

Stellt einen Algorithmus der Fuzzy-Suche dar, der den Ähnlichkeitsgrad festlegt. Der Ähnlichkeitsgrad-Algorithmus berechnet die maximale Anzahl von Fehlern für ein Wort als umgekehrt proportional zur Wortlänge.

```csharp
public class SimilarityLevel : FuzzyAlgorithm
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [SimilarityLevel](similaritylevel)(double) | Initialisiert eine neue Instanz der [`SimilarityLevel`](../similaritylevel)-Klasse. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| override [GetMaxMistakeCount](../../groupdocs.search.options/similaritylevel/getmaxmistakecount)(int) | Liest die maximal zulässige Anzahl von Fehlern für die angegebene Begriffslänge. |
| override [GetSimilarityLevel](../../groupdocs.search.options/similaritylevel/getsimilaritylevel)(int) | Liest den Ähnlichkeitsgradwert für die angegebene Begriffslänge. |

### Hinweise

**Learn more**

* [Fuzzy search](https://docs.groupdocs.com/display/searchnet/Fuzzy+search)

### Beispiele

Das Beispiel zeigt eine typische Verwendung der Klasse.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // Creating an index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

SearchOptions options = new SearchOptions();
options.FuzzySearch.Enabled = true; // Enabling the fuzzy search
options.FuzzySearch.FuzzyAlgorithm = new SimilarityLevel(0.8); // Creating the fuzzy search algorithm
// Diese Funktion legt 0 als maximale Fehleranzahl für Wörter von 1 bis 4 Zeichen fest.
// Sie legt 1 als maximale Fehleranzahl für Wörter von 5 bis 9 Zeichen fest.
// Sie legt 2 als maximale Fehleranzahl für Wörter von 10 bis 14 Zeichen fest. Und so weiter.

SearchResult result = index.Search(query, options); // Search in index
```

### Siehe auch

* class [FuzzyAlgorithm](../fuzzyalgorithm)
* namespace [GroupDocs.Search.Options](../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
