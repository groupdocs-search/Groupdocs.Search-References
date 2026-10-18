---
title: "SimilarityLevel"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta un algoritmo di ricerca fuzzy che specifica il livello di somiglianza."
type: docs
weight: 35
url: /it/java/com.groupdocs.search.options/similaritylevel/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.options.FuzzyAlgorithm](../../com.groupdocs.search.options/fuzzyalgorithm)
```
public class SimilarityLevel extends FuzzyAlgorithm
```

Rappresenta un algoritmo di ricerca fuzzy che specifica il livello di similarità. L'algoritmo del livello di similarità calcola il numero massimo di errori per una parola in modo inversamente proporzionale alla lunghezza della parola.


**Learn more**

* [Fuzzy search](../https://docs.groupdocs.com/display/searchjava/Fuzzy+search)


L'esempio dimostra un utilizzo tipico della classe.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Creazione di un indice nella cartella specificata
index.add(documentsFolder); // Indicizzazione dei documenti dalla cartella specificata
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // Abilitazione della ricerca fuzzy
options.getFuzzySearch().setFuzzyAlgorithm(new SimilarityLevel(0.8)); // Creazione dell'algoritmo di ricerca fuzzy
// Questa funzione specifica 0 come numero massimo di errori per parole da 1 a 4 caratteri.
// Specifica 1 come numero massimo di errori per parole da 5 a 9 caratteri.
// Specifica 2 come numero massimo di errori per parole da 10 a 14 caratteri. E così via.
SearchResult result = index.search(query, options); // Cerca nell'indice
 
```
 
````


## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [SimilarityLevel(double value)](#SimilarityLevel-double-) | Inizializza una nuova istanza della classe SimilarityLevel. |
|
|  | [SimilarityLevel(Object data)](#SimilarityLevel-java.lang.Object-) | Inizializza una nuova istanza della classe SimilarityLevel. |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getSimilarityLevel(int termLength)](#getSimilarityLevel-int-) | Ottiene il valore del livello di similarità per la lunghezza del termine specificata. |
|
|  | [getMaxMistakeCount(int termLength)](#getMaxMistakeCount-int-) | Ottiene il numero massimo consentito di errori per la lunghezza del termine specificata. |
|
### SimilarityLevel(double value) {#SimilarityLevel-double-}
```
public SimilarityLevel(double value)
```


Inizializza una nuova istanza della classe SimilarityLevel.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | double | Il valore del livello di similarità. |
|

### SimilarityLevel(Object data) {#SimilarityLevel-java.lang.Object-}
```
public SimilarityLevel(Object data)
```


Inizializza una nuova istanza della classe SimilarityLevel.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | dati | java.lang.Object | I dati serializzati. |
|

### getSimilarityLevel(int termLength) {#getSimilarityLevel-int-}
```
public double getSimilarityLevel(int termLength)
```


Ottiene il valore del livello di similarità per la lunghezza del termine specificata.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | termLength | int | La lunghezza del termine. |
|

**Returns:**
double - Il valore del livello di similarità.

### getMaxMistakeCount(int termLength) {#getMaxMistakeCount-int-}
```
public int getMaxMistakeCount(int termLength)
```


Ottiene il numero massimo consentito di errori per la lunghezza del termine specificata.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | termLength | int | La lunghezza del termine. |
|

**Returns:**
int - Il numero massimo consentito di errori.

