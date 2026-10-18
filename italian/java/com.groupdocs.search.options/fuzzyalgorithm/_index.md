---
title: "FuzzyAlgorithm"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta la classe base per gli algoritmi di ricerca fuzzy."
type: docs
weight: 20
url: /it/java/com.groupdocs.search.options/fuzzyalgorithm/
---
**Inheritance:**
java.lang.Object
```
public abstract class FuzzyAlgorithm
```

Rappresenta la classe base per gli algoritmi di ricerca fuzzy.


**Learn more**

* [Fuzzy search](../https://docs.groupdocs.com/display/searchjava/Fuzzy+search)

## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getSimilarityLevel(int termLength)](#getSimilarityLevel-int-) | Ottiene il livello di similarità per la lunghezza del termine specificata. |
|
|  | [getMaxMistakeCount(int termLength)](#getMaxMistakeCount-int-) | Ottiene il numero massimo consentito di errori per la lunghezza del termine specificata. |
|
| [getCore()](#getCore--) |  |
### getSimilarityLevel(int termLength) {#getSimilarityLevel-int-}
```
public abstract double getSimilarityLevel(int termLength)
```


Ottiene il livello di similarità per la lunghezza del termine specificata.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | termLength | int | La lunghezza del termine. |
|

**Returns:**
double - Il livello di similarità.

### getMaxMistakeCount(int termLength) {#getMaxMistakeCount-int-}
```
public abstract int getMaxMistakeCount(int termLength)
```


Ottiene il numero massimo consentito di errori per la lunghezza del termine specificata.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | termLength | int | La lunghezza del termine. |
|

**Returns:**
int - Il numero massimo consentito di errori.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
