---
title: "FuzzyAlgorithm"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt de basisklasse voor fuzzy-zoekalgoritmen voor."
type: docs
weight: 20
url: /nl/java/com.groupdocs.search.options/fuzzyalgorithm/
---
**Inheritance:**
java.lang.Object
```
public abstract class FuzzyAlgorithm
```

Stelt de basisklasse voor fuzzy-zoekalgoritmen voor.


**Learn more**

* [Fuzzy search](../https://docs.groupdocs.com/display/searchjava/Fuzzy+search)

## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getSimilarityLevel(int termLength)](#getSimilarityLevel-int-) | Haalt het gelijkenisniveau op voor de opgegeven termlengte. |
|
|  | [getMaxMistakeCount(int termLength)](#getMaxMistakeCount-int-) | Haalt het maximaal toegestane aantal fouten op voor de opgegeven termlengte. |
|
| [getCore()](#getCore--) |  |
### getSimilarityLevel(int termLength) {#getSimilarityLevel-int-}
```
public abstract double getSimilarityLevel(int termLength)
```


Haalt het gelijkenisniveau op voor de opgegeven termlengte.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | termLength | int | De termlengte. |
|

**Returns:**
double - Het gelijkenisniveau.

### getMaxMistakeCount(int termLength) {#getMaxMistakeCount-int-}
```
public abstract int getMaxMistakeCount(int termLength)
```


Haalt het maximaal toegestane aantal fouten op voor de opgegeven termlengte.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | termLength | int | De termlengte. |
|

**Returns:**
int - Het maximum toegestane aantal fouten.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
