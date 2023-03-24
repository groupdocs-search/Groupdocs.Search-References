---
title: TableDiscreteFunction
second_title: GroupDocs.Search for Java API Reference
description: Represents the fuzzy search algorithm that contains correspondences between word lengths and the number of allowed mistakes.
type: docs
weight: 36
url: /java/com.groupdocs.search.options/tablediscretefunction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.options.FuzzyAlgorithm](../../com.groupdocs.search.options/fuzzyalgorithm)
```
public class TableDiscreteFunction extends FuzzyAlgorithm
```

Represents the fuzzy search algorithm that contains correspondences between word lengths and the number of allowed mistakes. This algorithm can be specified by a table of output values or by a step function.

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
 options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1, new Step(5, 2), new Step(8, 3))); // Creating the fuzzy search algorithm
 // This function specifies 1 as the maximum number of mistakes for words from 1 to 4 characters.
 // It specifies 2 as the maximum number of mistakes for words from 5 to 7 characters.
 // It specifies 3 as the maximum number of mistakes for words from 8 and more characters.
 SearchResult result = index.search(query, options); // Search in index
 
```


[Fuzzy search]: https://docs.groupdocs.com/display/searchjava/Fuzzy+search
## Constructors

| Constructor | Description |
| --- | --- |
| [TableDiscreteFunction(int offsetOfInputs, int[] tableOfOutputs)](#TableDiscreteFunction-int-int---) | Initializes a new instance of the  TableDiscreteFunction  class. |
| [TableDiscreteFunction(int firstStepLevel, Step[] steps)](#TableDiscreteFunction-int-com.groupdocs.search.options.Step...-) | Initializes a new instance of the  TableDiscreteFunction  class. |
## Methods

| Method | Description |
| --- | --- |
| [getSimilarityLevel(int termLength)](#getSimilarityLevel-int-) | Gets a similarity level for specified term length. |
| [getMaxMistakeCount(int termLength)](#getMaxMistakeCount-int-) | Gets a maximum allowed number of mistakes for specified term length. |
### TableDiscreteFunction(int offsetOfInputs, int[] tableOfOutputs) {#TableDiscreteFunction-int-int---}
```
public TableDiscreteFunction(int offsetOfInputs, int[] tableOfOutputs)
```


Initializes a new instance of the  TableDiscreteFunction  class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| offsetOfInputs | int | The offset of the table indeces relative to the input values. |
| tableOfOutputs | int[] | The table of output values. |

### TableDiscreteFunction(int firstStepLevel, Step[] steps) {#TableDiscreteFunction-int-com.groupdocs.search.options.Step...-}
```
public TableDiscreteFunction(int firstStepLevel, Step[] steps)
```


Initializes a new instance of the  TableDiscreteFunction  class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| firstStepLevel | int | The level of the first step of the step function. |
| steps | [Step\[\]](../../com.groupdocs.search.options/step) | The next steps of the step function. |

### getSimilarityLevel(int termLength) {#getSimilarityLevel-int-}
```
public double getSimilarityLevel(int termLength)
```


Gets a similarity level for specified term length.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| termLength | int | The term length. |

**Returns:**
double - A similarity level.
### getMaxMistakeCount(int termLength) {#getMaxMistakeCount-int-}
```
public int getMaxMistakeCount(int termLength)
```


Gets a maximum allowed number of mistakes for specified term length.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| termLength | int | The term length. |

**Returns:**
int - A maximum allowed number of mistakes.
