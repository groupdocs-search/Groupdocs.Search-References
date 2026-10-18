---
title: "FuzzySearchOptions"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Fornisce opzioni per la ricerca fuzzy."
type: docs
weight: 21
url: /it/java/com.groupdocs.search.options/fuzzysearchoptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class FuzzySearchOptions
```

Fornisce opzioni per la ricerca fuzzy.


**Learn more**

* [Fuzzy search](../https://docs.groupdocs.com/display/searchjava/Fuzzy+search)
* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [FuzzySearchOptions()](#FuzzySearchOptions--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getEnabled()](#getEnabled--) | Restituisce un valore che indica se la funzionalità di ricerca fuzzy è abilitata. |
|
|  | [setEnabled(boolean value)](#setEnabled-boolean-) | Imposta un valore che indica se la funzionalità di ricerca fuzzy è abilitata. |
|
|  | [getFuzzyAlgorithm()](#getFuzzyAlgorithm--) | Ottiene l'algoritmo di ricerca fuzzy. |
|
|  | [setFuzzyAlgorithm(FuzzyAlgorithm value)](#setFuzzyAlgorithm-com.groupdocs.search.options.FuzzyAlgorithm-) | Imposta l'algoritmo di ricerca fuzzy. |
|
|  | [getOnlyBestResults()](#getOnlyBestResults--) | Restituisce un valore che indica se verranno restituiti solo i risultati migliori. |
|
|  | [setOnlyBestResults(boolean value)](#setOnlyBestResults-boolean-) | Imposta un valore che indica se verranno restituiti solo i risultati migliori. |
|
|  | [getOnlyBestResultsRange()](#getOnlyBestResultsRange--) | Restituisce il superamento massimo del numero minimo di errori trovati. |
|
|  | [setOnlyBestResultsRange(byte value)](#setOnlyBestResultsRange-byte-) | Imposta il superamento massimo del numero minimo di errori trovati. |
|
|  | [getConsiderTranspositions()](#getConsiderTranspositions--) | Ottiene un valore che indica se l'algoritmo di ricerca fuzzy deve considerare la trasposizione di due caratteri adiacenti come un unico errore. |
|
|  | [setConsiderTranspositions(boolean value)](#setConsiderTranspositions-boolean-) | Imposta un valore che indica se l'algoritmo di ricerca fuzzy deve considerare la trasposizione di due caratteri adiacenti come un unico errore. |
|
### FuzzySearchOptions() {#FuzzySearchOptions--}
```
public FuzzySearchOptions()
```


### getEnabled() {#getEnabled--}
```
public abstract boolean getEnabled()
```


Ottiene un valore che indica se la funzionalità di ricerca fuzzy è abilitata. Il valore predefinito è  false .


**Returns:**
boolean - Un valore che indica se la funzionalità di ricerca fuzzy è abilitata.

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public abstract void setEnabled(boolean value)
```


Imposta un valore che indica se la funzionalità di ricerca fuzzy è abilitata. Il valore predefinito è  false .


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | boolean | Un valore che indica se la funzionalità di ricerca fuzzy è abilitata. |
|

### getFuzzyAlgorithm() {#getFuzzyAlgorithm--}
```
public abstract FuzzyAlgorithm getFuzzyAlgorithm()
```


Ottiene l'algoritmo di ricerca fuzzy. Gli algoritmi di ricerca fuzzy attualmente disponibili sono  SimilarityLevel  e  TableDiscreteFunction . Il valore predefinito è un'istanza di  SimilarityLevel  con un valore di livello di similarità di  0.5 .


**Returns:**
[FuzzyAlgorithm](../../com.groupdocs.search.options/fuzzyalgorithm) - The fuzzy search algorithm.


L'esempio dimostra come impostare l'algoritmo di ricerca fuzzy.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Creazione di un indice nella cartella specificata
index.add(documentsFolder); // Indicizzazione dei documenti dalla cartella specificata
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // Abilitazione della ricerca fuzzy
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1, new Step(5, 2), new Step(8, 3))); // Creazione dell'algoritmo di ricerca fuzzy
// Questa funzione specifica 1 come numero massimo di errori per parole da 1 a 4 caratteri.
// Specifica 2 come numero massimo di errori per parole da 5 a 7 caratteri.
// Specifica 3 come numero massimo di errori per parole da 8 caratteri in su.
SearchResult result = index.search(query, options); // Cerca nell'indice
 
```
 
````


### setFuzzyAlgorithm(FuzzyAlgorithm value) {#setFuzzyAlgorithm-com.groupdocs.search.options.FuzzyAlgorithm-}
```
public abstract void setFuzzyAlgorithm(FuzzyAlgorithm value)
```


Imposta l'algoritmo di ricerca fuzzy. Gli algoritmi di ricerca fuzzy attualmente disponibili sono  SimilarityLevel  e  TableDiscreteFunction . Il valore predefinito è un'istanza di  SimilarityLevel  con un valore di livello di similarità di  0.5 .


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | value | [FuzzyAlgorithm](../../com.groupdocs.search.options/fuzzyalgorithm) | L'algoritmo di ricerca fuzzy. |


L'esempio dimostra come impostare l'algoritmo di ricerca fuzzy.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Creazione di un indice nella cartella specificata
index.add(documentsFolder); // Indicizzazione dei documenti dalla cartella specificata
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // Abilitazione della ricerca fuzzy
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1, new Step(5, 2), new Step(8, 3))); // Creazione dell'algoritmo di ricerca fuzzy
// Questa funzione specifica 1 come numero massimo di errori per parole da 1 a 4 caratteri.
// Specifica 2 come numero massimo di errori per parole da 5 a 7 caratteri.
// Specifica 3 come numero massimo di errori per parole da 8 caratteri in su.
SearchResult result = index.search(query, options); // Cerca nell'indice
 
```
 
````

|

### getOnlyBestResults() {#getOnlyBestResults--}
```
public abstract boolean getOnlyBestResults()
```


Ottiene un valore che indica se verranno restituiti solo i risultati migliori. Il valore predefinito è  false .


**Returns:**
boolean -  true  se verranno restituiti solo i risultati migliori; altrimenti  false .

### setOnlyBestResults(boolean value) {#setOnlyBestResults-boolean-}
```
public abstract void setOnlyBestResults(boolean value)
```


Imposta un valore che indica se verranno restituiti solo i risultati migliori. Il valore predefinito è  false .


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | boolean | true  se verranno restituiti solo i risultati migliori; altrimenti  false . |
|

### getOnlyBestResultsRange() {#getOnlyBestResultsRange--}
```
public abstract byte getOnlyBestResultsRange()
```


Ottiene il superamento massimo del numero minimo di errori trovato. Il valore predefinito è  0 .


**Returns:**
byte - Il superamento massimo del numero minimo di errori trovato.

### setOnlyBestResultsRange(byte value) {#setOnlyBestResultsRange-byte-}
```
public abstract void setOnlyBestResultsRange(byte value)
```


Imposta il superamento massimo del numero minimo di errori trovato. Il valore predefinito è  0 .


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | byte | Il superamento massimo del numero minimo di errori trovato. |
|

### getConsiderTranspositions() {#getConsiderTranspositions--}
```
public abstract boolean getConsiderTranspositions()
```


Ottiene un valore che indica se l'algoritmo di ricerca fuzzy deve considerare la trasposizione di due caratteri adiacenti come un unico errore. Il valore predefinito è  true .


**Returns:**
boolean -  true  se l'algoritmo di ricerca fuzzy considera le trasposizioni; altrimenti  false .

### setConsiderTranspositions(boolean value) {#setConsiderTranspositions-boolean-}
```
public abstract void setConsiderTranspositions(boolean value)
```


Imposta un valore che indica se l'algoritmo di ricerca fuzzy deve considerare la trasposizione di due caratteri adiacenti come un unico errore. Il valore predefinito è  true .


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | boolean | :  true  se l'algoritmo di ricerca fuzzy considera le trasposizioni; altrimenti  false . |
|

