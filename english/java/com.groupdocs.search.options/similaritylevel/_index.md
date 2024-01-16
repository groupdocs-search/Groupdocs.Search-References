---
title: SimilarityLevel
second_title: GroupDocs.Search for Java API Reference
description: Represents an algorithm of the fuzzy search that specifies the similarity level.
type: docs
weight: 32
url: /java/com.groupdocs.search.options/similaritylevel/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.options.FuzzyAlgorithm](../../com.groupdocs.search.options/fuzzyalgorithm)
```
public class SimilarityLevel extends FuzzyAlgorithm
```

Represents an algorithm of the fuzzy search that specifies the similarity level. The similarity level algorithm calculates the maximum number of mistakes for a word as inversely proportional to the word length.

**Learn more**

 *  [Fuzzy search][]

The example demonstrates a typical usage of the class.

```

 String indexFolder = "c:\\MyIndex\\";
 String documentsFolder = "c:\\MyDocuments\\";
 String query = "Einstein";
 Index index = new Index(indexFolder); // Creating an index in the specified folder
 index.add(documentsFolder); // Indexing documents from the specified folder
 SearchOptions options = new SearchOptions();
 options.getFuzzySearch().setEnabled(true); // Enabling the fuzzy search
 options.getFuzzySearch().setFuzzyAlgorithm(new SimilarityLevel(0.8)); // Creating the fuzzy search algorithm
 // This function specifies 0 as the maximum number of mistakes for words from 1 to 4 characters.
 // It specifies 1 as the maximum number of mistakes for words from 5 to 9 characters.
 // It specifies 2 as the maximum number of mistakes for words from 10 to 14 characters. And so on.
 SearchResult result = index.search(query, options); // Search in index
 
```


[Fuzzy search]: https://docs.groupdocs.com/display/searchjava/Fuzzy+search
## Constructors

| Constructor | Description |
| --- | --- |
| [SimilarityLevel(double value)](#SimilarityLevel-double-) | Initializes a new instance of the  SimilarityLevel  class. |
| [SimilarityLevel(Object data)](#SimilarityLevel-java.lang.Object-) | Initializes a new instance of the  SimilarityLevel  class. |
## Methods

| Method | Description |
| --- | --- |
| [getSimilarityLevel(int termLength)](#getSimilarityLevel-int-) | Gets the similarity level value for the specified term length. |
| [getMaxMistakeCount(int termLength)](#getMaxMistakeCount-int-) | Gets the maximum allowed number of mistakes for the specified term length. |
### SimilarityLevel(double value) {#SimilarityLevel-double-}
```
public SimilarityLevel(double value)
```


Initializes a new instance of the  SimilarityLevel  class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double | The similarity level value. |

### SimilarityLevel(Object data) {#SimilarityLevel-java.lang.Object-}
```
public SimilarityLevel(Object data)
```


Initializes a new instance of the  SimilarityLevel  class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| data | java.lang.Object | The serialized data. |

### getSimilarityLevel(int termLength) {#getSimilarityLevel-int-}
```
public double getSimilarityLevel(int termLength)
```


Gets the similarity level value for the specified term length.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| termLength | int | The term length. |

**Returns:**
double - The similarity level value.
### getMaxMistakeCount(int termLength) {#getMaxMistakeCount-int-}
```
public int getMaxMistakeCount(int termLength)
```


Gets the maximum allowed number of mistakes for the specified term length.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| termLength | int | The term length. |

**Returns:**
int - The maximum allowed number of mistakes.
