---
title: FuzzySearchOptions
second_title: GroupDocs.Search for Java API Reference
description: Provides options of the fuzzy search.
type: docs
weight: 19
url: /java/com.groupdocs.search.options/fuzzysearchoptions/
---
**Inheritance:**
java.lang.Object
```
public class FuzzySearchOptions
```

Provides options of the fuzzy search.

**Learn more**

 *  [Fuzzy search][]
 *  [Search options][]


[Fuzzy search]: https://docs.groupdocs.com/display/searchjava/Fuzzy+search
[Search options]: https://docs.groupdocs.com/display/searchjava/Search+options
## Methods

| Method | Description |
| --- | --- |
| [getEnabled()](#getEnabled--) | Gets a value indicating whether fuzzy search feature is enabled. |
| [setEnabled(boolean value)](#setEnabled-boolean-) | Sets a value indicating whether fuzzy search feature is enabled. |
| [getFuzzyAlgorithm()](#getFuzzyAlgorithm--) | Gets the fuzzy search algorithm. |
| [setFuzzyAlgorithm(FuzzyAlgorithm value)](#setFuzzyAlgorithm-com.groupdocs.search.options.FuzzyAlgorithm-) | Sets the fuzzy search algorithm. |
| [getOnlyBestResults()](#getOnlyBestResults--) | Gets a value indicating whether only the best results will be returned. |
| [setOnlyBestResults(boolean value)](#setOnlyBestResults-boolean-) | Sets a value indicating whether only the best results will be returned. |
| [getOnlyBestResultsRange()](#getOnlyBestResultsRange--) | Gets the maximum exceeding of the minimum number of mistakes that are found. |
| [setOnlyBestResultsRange(byte value)](#setOnlyBestResultsRange-byte-) | Sets the maximum exceeding of the minimum number of mistakes that are found. |
| [getConsiderTranspositions()](#getConsiderTranspositions--) | Gets a value indicating whether the fuzzy search algorithm must consider transposition of two adjacent characters as a single mistake. |
| [setConsiderTranspositions(boolean value)](#setConsiderTranspositions-boolean-) | Sets a value indicating whether the fuzzy search algorithm must consider transposition of two adjacent characters as a single mistake. |
### getEnabled() {#getEnabled--}
```
public final boolean getEnabled()
```


Gets a value indicating whether fuzzy search feature is enabled. The default value is  false .

**Returns:**
boolean - A value indicating whether fuzzy search feature is enabled.
### setEnabled(boolean value) {#setEnabled-boolean-}
```
public final void setEnabled(boolean value)
```


Sets a value indicating whether fuzzy search feature is enabled. The default value is  false .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | A value indicating whether fuzzy search feature is enabled. |

### getFuzzyAlgorithm() {#getFuzzyAlgorithm--}
```
public final FuzzyAlgorithm getFuzzyAlgorithm()
```


Gets the fuzzy search algorithm. The currently available fuzzy search algorithms are  SimilarityLevel  and  TableDiscreteFunction . The default value is an instance of  SimilarityLevel  with a similarity level value of  0.5 .

**Returns:**
[FuzzyAlgorithm](../../com.groupdocs.search.options/fuzzyalgorithm) - The fuzzy search algorithm.

The example demonstrates how to set the fuzzy search algorithm.

```
String indexFolder = "c:\\MyIndex\\";
 String documentsFolder = "c:\\MyDocuments\\";
 String query = "Einstein";
 Index index = new Index(indexFolder); // Creating an index in the specified folder
 index.add(documentsFolder); // Indexing documents from the specified folder
 SearchOptions options = new SearchOptions();
 options.getFuzzySearch().setEnabled(true); // Enabling the fuzzy search
 options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1, new Step(5, 2), new Step(8, 3))); // Creating the fuzzy search algorithm
 // This function specifies 1 as the maximum number of mistakes for words from 1 to 4 characters.
 // It specifies 2 as the maximum number of mistakes for words from 5 to 7 characters.
 // It specifies 3 as the maximum number of mistakes for words from 8 and more characters.
 SearchResult result = index.search(query, options); // Search in index
```
### setFuzzyAlgorithm(FuzzyAlgorithm value) {#setFuzzyAlgorithm-com.groupdocs.search.options.FuzzyAlgorithm-}
```
public final void setFuzzyAlgorithm(FuzzyAlgorithm value)
```


Sets the fuzzy search algorithm. The currently available fuzzy search algorithms are  SimilarityLevel  and  TableDiscreteFunction . The default value is an instance of  SimilarityLevel  with a similarity level value of  0.5 .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [FuzzyAlgorithm](../../com.groupdocs.search.options/fuzzyalgorithm) | The fuzzy search algorithm.

The example demonstrates how to set the fuzzy search algorithm.

```
String indexFolder = "c:\\MyIndex\\";
 String documentsFolder = "c:\\MyDocuments\\";
 String query = "Einstein";
 Index index = new Index(indexFolder); // Creating an index in the specified folder
 index.add(documentsFolder); // Indexing documents from the specified folder
 SearchOptions options = new SearchOptions();
 options.getFuzzySearch().setEnabled(true); // Enabling the fuzzy search
 options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1, new Step(5, 2), new Step(8, 3))); // Creating the fuzzy search algorithm
 // This function specifies 1 as the maximum number of mistakes for words from 1 to 4 characters.
 // It specifies 2 as the maximum number of mistakes for words from 5 to 7 characters.
 // It specifies 3 as the maximum number of mistakes for words from 8 and more characters.
 SearchResult result = index.search(query, options); // Search in index
``` |

### getOnlyBestResults() {#getOnlyBestResults--}
```
public final boolean getOnlyBestResults()
```


Gets a value indicating whether only the best results will be returned. The default value is  false .

**Returns:**
boolean -  true  if only the best results will be returned; otherwise  false .
### setOnlyBestResults(boolean value) {#setOnlyBestResults-boolean-}
```
public final void setOnlyBestResults(boolean value)
```


Sets a value indicating whether only the best results will be returned. The default value is  false .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  true  if only the best results will be returned; otherwise  false . |

### getOnlyBestResultsRange() {#getOnlyBestResultsRange--}
```
public final byte getOnlyBestResultsRange()
```


Gets the maximum exceeding of the minimum number of mistakes that are found. The default value is  0 .

**Returns:**
byte - The maximum exceeding of the minimum number of mistakes found.
### setOnlyBestResultsRange(byte value) {#setOnlyBestResultsRange-byte-}
```
public final void setOnlyBestResultsRange(byte value)
```


Sets the maximum exceeding of the minimum number of mistakes that are found. The default value is  0 .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | byte | The maximum exceeding of the minimum number of mistakes found. |

### getConsiderTranspositions() {#getConsiderTranspositions--}
```
public final boolean getConsiderTranspositions()
```


Gets a value indicating whether the fuzzy search algorithm must consider transposition of two adjacent characters as a single mistake. The default value is  true .

**Returns:**
boolean -  true  if the fuzzy search algorithm considers transpositions; otherwise  false .
### setConsiderTranspositions(boolean value) {#setConsiderTranspositions-boolean-}
```
public final void setConsiderTranspositions(boolean value)
```


Sets a value indicating whether the fuzzy search algorithm must consider transposition of two adjacent characters as a single mistake. The default value is  true .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | :  true  if the fuzzy search algorithm considers transpositions; otherwise  false . |

