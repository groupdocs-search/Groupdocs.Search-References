---
title: "TableDiscreteFunction"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Rappresenta l'algoritmo di ricerca fuzzy che contiene corrispondenze tra le lunghezze delle parole e il numero di errori consentiti. Questo algoritmo può essere specificato tramite una tabella di valori di output o mediante una funzione a gradini."
type: docs
weight: 1170
url: /it/net/groupdocs.search.options/tablediscretefunction/
---
## TableDiscreteFunction class

Rappresenta l'algoritmo di ricerca fuzzy che contiene corrispondenze tra le lunghezze delle parole e il numero di errori consentiti. Questo algoritmo può essere specificato tramite una tabella di valori di output o mediante una funzione a gradini.

```csharp
public class TableDiscreteFunction : FuzzyAlgorithm
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [TableDiscreteFunction](tablediscretefunction#constructor_1)(int, int[]) | Inizializza una nuova istanza della classe [`TableDiscreteFunction`](../tablediscretefunction). |
| [TableDiscreteFunction](tablediscretefunction#constructor)(int, params Step[]) | Inizializza una nuova istanza della classe [`TableDiscreteFunction`](../tablediscretefunction). |

## Metodi

| Nome | Descrizione |
| --- | --- |
| override [GetMaxMistakeCount](../../groupdocs.search.options/tablediscretefunction/getmaxmistakecount)(int) | Ottiene il numero massimo consentito di errori per la lunghezza del termine specificata. |
| override [GetSimilarityLevel](../../groupdocs.search.options/tablediscretefunction/getsimilaritylevel)(int) | Ottiene il livello di somiglianza per la lunghezza del termine specificata. |

### Osservazioni

**Learn more**

* [Fuzzy search](https://docs.groupdocs.com/display/searchnet/Fuzzy+search)

### Esempi

L'esempio dimostra un utilizzo tipico della classe.

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

* class [FuzzyAlgorithm](../fuzzyalgorithm)
* namespace [GroupDocs.Search.Options](../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
