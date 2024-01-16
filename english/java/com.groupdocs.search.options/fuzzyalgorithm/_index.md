---
title: FuzzyAlgorithm
second_title: GroupDocs.Search for Java API Reference
description: Represents the base class for fuzzy search algorithms.
type: docs
weight: 18
url: /java/com.groupdocs.search.options/fuzzyalgorithm/
---
**Inheritance:**
java.lang.Object
```
public abstract class FuzzyAlgorithm
```

Represents the base class for fuzzy search algorithms.

**Learn more**

 *  [Fuzzy search][]


[Fuzzy search]: https://docs.groupdocs.com/display/searchjava/Fuzzy+search
## Methods

| Method | Description |
| --- | --- |
| [getSimilarityLevel(int termLength)](#getSimilarityLevel-int-) | Gets the similarity level for the specified term length. |
| [getMaxMistakeCount(int termLength)](#getMaxMistakeCount-int-) | Gets the maximum allowed number of mistakes for the specified term length. |
| [getCore()](#getCore--) |  |
### getSimilarityLevel(int termLength) {#getSimilarityLevel-int-}
```
public abstract double getSimilarityLevel(int termLength)
```


Gets the similarity level for the specified term length.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| termLength | int | The term length. |

**Returns:**
double - The similarity level.
### getMaxMistakeCount(int termLength) {#getMaxMistakeCount-int-}
```
public abstract int getMaxMistakeCount(int termLength)
```


Gets the maximum allowed number of mistakes for the specified term length.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| termLength | int | The term length. |

**Returns:**
int - The maximum allowed number of mistakes.
### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
