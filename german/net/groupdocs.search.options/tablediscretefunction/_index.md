---
title: "TableDiscreteFunction"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Stellt den Fuzzy-Suchalgorithmus dar, der Zuordnungen zwischen Wortlängen und der Anzahl zulässiger Fehler enthält. Dieser Algorithmus kann durch eine Tabelle von Ausgabewerten oder durch eine Stufenfunktion angegeben werden."
type: docs
weight: 1170
url: /de/net/groupdocs.search.options/tablediscretefunction/
---
## TableDiscreteFunction class

Stellt den Fuzzy-Suchalgorithmus dar, der Zuordnungen zwischen Wortlängen und der Anzahl zulässiger Fehler enthält. Dieser Algorithmus kann durch eine Tabelle von Ausgabewerten oder durch eine Stufenfunktion angegeben werden.

```csharp
public class TableDiscreteFunction : FuzzyAlgorithm
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [TableDiscreteFunction](tablediscretefunction#constructor_1)(int, int[]) | Initialisiert eine neue Instanz der Klasse [`TableDiscreteFunction`](../tablediscretefunction). |
| [TableDiscreteFunction](tablediscretefunction#constructor)(int, params Step[]) | Initialisiert eine neue Instanz der Klasse [`TableDiscreteFunction`](../tablediscretefunction). |

## Methoden

| Name | Beschreibung |
| --- | --- |
| override [GetMaxMistakeCount](../../groupdocs.search.options/tablediscretefunction/getmaxmistakecount)(int) | Gibt die maximal zulässige Anzahl von Fehlern für die angegebene Begriffslänge zurück. |
| override [GetSimilarityLevel](../../groupdocs.search.options/tablediscretefunction/getsimilaritylevel)(int) | Gibt das Ähnlichkeitsniveau für die angegebene Begriffslänge zurück. |

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
options.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1, new Step(5, 2), new Step(8, 3)); // Creating the fuzzy search algorithm
// Diese Funktion legt 1 als maximale Fehlermenge für Wörter von 1 bis 4 Zeichen fest.
// Sie legt 2 als maximale Fehlermenge für Wörter von 5 bis 7 Zeichen fest.
// Sie legt 3 als maximale Fehlermenge für Wörter von 8 und mehr Zeichen fest.

SearchResult result = index.Search(query, options); // Search in index
```

### Siehe auch

* class [FuzzyAlgorithm](../fuzzyalgorithm)
* namespace [GroupDocs.Search.Options](../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
