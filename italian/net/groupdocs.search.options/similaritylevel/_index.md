---
title: SimilarityLevel
second_title: GroupDocs.Cerca il riferimento dell'API .NET
description: Rappresenta un algoritmo della ricerca fuzzy che specifica il livello di somiglianza. Lalgoritmo del livello di somiglianza calcola il numero massimo di errori per una parola come inversamente proporzionale alla lunghezza della parola.
type: docs
weight: 1050
url: /it/net/groupdocs.search.options/similaritylevel/
---
## SimilarityLevel class

Rappresenta un algoritmo della ricerca fuzzy che specifica il livello di somiglianza. L'algoritmo del livello di somiglianza calcola il numero massimo di errori per una parola come inversamente proporzionale alla lunghezza della parola.

```csharp
public class SimilarityLevel : FuzzyAlgorithm
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [SimilarityLevel](similaritylevel)(double) | Inizializza una nuova istanza di[`SimilarityLevel`](../similaritylevel) classe. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| override [GetMaxMistakeCount](../../groupdocs.search.options/similaritylevel/getmaxmistakecount)(int) | Ottiene il numero massimo consentito di errori per la lunghezza del termine specificata. |
| override [GetSimilarityLevel](../../groupdocs.search.options/similaritylevel/getsimilaritylevel)(int) | Ottiene il valore del livello di somiglianza per la lunghezza del termine specificata. |

### Osservazioni

**Saperne di più**

* [Ricerca sfocata](https://docs.groupdocs.com/display/searchnet/Fuzzy+search)

### Esempi

L'esempio mostra un utilizzo tipico della classe.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // Creazione di un indice nella cartella specificata
index.Add(documentsFolder); // Indicizzazione dei documenti dalla cartella specificata

SearchOptions options = new SearchOptions();
options.FuzzySearch.Enabled = true; // Abilitazione della ricerca fuzzy
options.FuzzySearch.FuzzyAlgorithm = new SimilarityLevel(0.8); // Creazione dell'algoritmo di ricerca fuzzy
// Questa funzione specifica 0 come numero massimo di errori per parole da 1 a 4 caratteri.
// Specifica 1 come numero massimo di errori per parole da 5 a 9 caratteri.
// Specifica 2 come numero massimo di errori per parole da 10 a 14 caratteri. E così via.

SearchResult result = index.Search(query, options); // Cerca nell'indice
```

### Guarda anche

* class [FuzzyAlgorithm](../fuzzyalgorithm)
* spazio dei nomi [GroupDocs.Search.Options](../../groupdocs.search.options)
* assemblea [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
