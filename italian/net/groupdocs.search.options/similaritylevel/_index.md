---
title: "SimilarityLevel"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Rappresenta un algoritmo di ricerca fuzzy che specifica il livello di similarità. L'algoritmo del livello di similarità calcola il numero massimo di errori per una parola in modo inversamente proporzionale alla lunghezza della parola."
type: docs
weight: 1120
url: /it/net/groupdocs.search.options/similaritylevel/
---
## SimilarityLevel class

Rappresenta un algoritmo di ricerca fuzzy che specifica il livello di similarità. L'algoritmo del livello di similarità calcola il numero massimo di errori per una parola in modo inversamente proporzionale alla lunghezza della parola.

```csharp
public class SimilarityLevel : FuzzyAlgorithm
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [SimilarityLevel](similaritylevel)(double) | Inizializza una nuova istanza della classe [`SimilarityLevel`](../similaritylevel). |

## Metodi

| Nome | Descrizione |
| --- | --- |
| override [GetMaxMistakeCount](../../groupdocs.search.options/similaritylevel/getmaxmistakecount)(int) | Ottiene il numero massimo consentito di errori per la lunghezza del termine specificata. |
| override [GetSimilarityLevel](../../groupdocs.search.options/similaritylevel/getsimilaritylevel)(int) | Ottiene il valore del livello di similarità per la lunghezza del termine specificata. |

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
options.FuzzySearch.FuzzyAlgorithm = new SimilarityLevel(0.8); // Creating the fuzzy search algorithm
// Questa funzione specifica 0 come numero massimo di errori per parole da 1 a 4 caratteri.
// Specifica 1 come numero massimo di errori per parole da 5 a 9 caratteri.
// Specifica 2 come numero massimo di errori per parole da 10 a 14 caratteri. E così via.

SearchResult result = index.Search(query, options); // Search in index
```

### Vedi anche

* class [FuzzyAlgorithm](../fuzzyalgorithm)
* namespace [GroupDocs.Search.Options](../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
