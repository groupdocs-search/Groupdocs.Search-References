---
title: "FuzzyAlgorithm"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar basklassen för fuzzy-sökalgoritmer."
type: docs
weight: 20
url: /sv/java/com.groupdocs.search.options/fuzzyalgorithm/
---
**Inheritance:**
java.lang.Object
```
public abstract class FuzzyAlgorithm
```

Representerar basklassen för fuzzy-sökalgoritmer.


**Learn more**

* [Fuzzy search](../https://docs.groupdocs.com/display/searchjava/Fuzzy+search)

## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getSimilarityLevel(int termLength)](#getSimilarityLevel-int-) | Hämtar likhetsnivån för den angivna termlängden. |
|
|  | [getMaxMistakeCount(int termLength)](#getMaxMistakeCount-int-) | Hämtar det maximalt tillåtna antalet fel för den angivna termlängden. |
|
| [getCore()](#getCore--) |  |
### getSimilarityLevel(int termLength) {#getSimilarityLevel-int-}
```
public abstract double getSimilarityLevel(int termLength)
```


Hämtar likhetsnivån för den angivna termlängden.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | termLength | int | Termlängden. |
|

**Returns:**
double - Likhetsnivån.

### getMaxMistakeCount(int termLength) {#getMaxMistakeCount-int-}
```
public abstract int getMaxMistakeCount(int termLength)
```


Hämtar det maximalt tillåtna antalet fel för den angivna termlängden.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | termLength | int | Termlängden. |
|

**Returns:**
int - Det maximala tillåtna antalet misstag.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
