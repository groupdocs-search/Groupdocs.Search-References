---
title: SpellingCorrectorOptions
second_title: GroupDocs.Search for Java API Reference
description: Provides options for the spelling corrector.
type: docs
weight: 36
url: /java/com.groupdocs.search.options/spellingcorrectoroptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class SpellingCorrectorOptions
```

Provides options for the spelling corrector.

**Learn more**

 *  [Spell checking][]
 *  [Search options][]


[Spell checking]: https://docs.groupdocs.com/display/searchjava/Spell+checking
[Search options]: https://docs.groupdocs.com/display/searchjava/Search+options
## Constructors

| Constructor | Description |
| --- | --- |
| [SpellingCorrectorOptions()](#SpellingCorrectorOptions--) |  |
## Methods

| Method | Description |
| --- | --- |
| [getEnabled()](#getEnabled--) | Gets a value indicating whether the spelling corrector is enabled. |
| [setEnabled(boolean value)](#setEnabled-boolean-) | Sets a value indicating whether the spelling corrector is enabled. |
| [getMaxMistakeCount()](#getMaxMistakeCount--) | Gets the maximum number of mistakes. |
| [setMaxMistakeCount(int value)](#setMaxMistakeCount-int-) | Sets the maximum number of mistakes. |
| [getOnlyBestResults()](#getOnlyBestResults--) | Gets a value indicating whether only the best results will be returned. |
| [setOnlyBestResults(boolean value)](#setOnlyBestResults-boolean-) | Sets a value indicating whether only the best results will be returned. |
| [getOnlyBestResultsRange()](#getOnlyBestResultsRange--) | Gets the maximum exceeding of the minimum number of mistakes that are found. |
| [setOnlyBestResultsRange(byte value)](#setOnlyBestResultsRange-byte-) | Sets the maximum exceeding of the minimum number of mistakes that are found. |
| [getConsiderTranspositions()](#getConsiderTranspositions--) | Gets a value indicating whether the algorithm must consider transposition of two adjacent characters as a single mistake. |
| [setConsiderTranspositions(boolean value)](#setConsiderTranspositions-boolean-) | Sets a value indicating whether the algorithm must consider transposition of two adjacent characters as a single mistake. |
### SpellingCorrectorOptions() {#SpellingCorrectorOptions--}
```
public SpellingCorrectorOptions()
```


### getEnabled() {#getEnabled--}
```
public abstract boolean getEnabled()
```


Gets a value indicating whether the spelling corrector is enabled. The default value is  false .

**Returns:**
boolean - A value indicating whether the spelling corrector is enabled.
### setEnabled(boolean value) {#setEnabled-boolean-}
```
public abstract void setEnabled(boolean value)
```


Sets a value indicating whether the spelling corrector is enabled. The default value is  false .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | A value indicating whether the spelling corrector is enabled. |

### getMaxMistakeCount() {#getMaxMistakeCount--}
```
public abstract int getMaxMistakeCount()
```


Gets the maximum number of mistakes. The default value is  2 .

**Returns:**
int - The maximum number of mistakes.
### setMaxMistakeCount(int value) {#setMaxMistakeCount-int-}
```
public abstract void setMaxMistakeCount(int value)
```


Sets the maximum number of mistakes. The default value is  2 .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | The maximum number of mistakes. |

### getOnlyBestResults() {#getOnlyBestResults--}
```
public abstract boolean getOnlyBestResults()
```


Gets a value indicating whether only the best results will be returned. The default value is  false .

**Returns:**
boolean -  true  if only the best results will be returned; otherwise  false .
### setOnlyBestResults(boolean value) {#setOnlyBestResults-boolean-}
```
public abstract void setOnlyBestResults(boolean value)
```


Sets a value indicating whether only the best results will be returned. The default value is  false .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  true  if only the best results will be returned; otherwise  false . |

### getOnlyBestResultsRange() {#getOnlyBestResultsRange--}
```
public abstract byte getOnlyBestResultsRange()
```


Gets the maximum exceeding of the minimum number of mistakes that are found. The default value is  0 .

**Returns:**
byte - The maximum exceeding of the minimum number of mistakes found.
### setOnlyBestResultsRange(byte value) {#setOnlyBestResultsRange-byte-}
```
public abstract void setOnlyBestResultsRange(byte value)
```


Sets the maximum exceeding of the minimum number of mistakes that are found. The default value is  0 .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | byte | The maximum exceeding of the minimum number of mistakes found. |

### getConsiderTranspositions() {#getConsiderTranspositions--}
```
public abstract boolean getConsiderTranspositions()
```


Gets a value indicating whether the algorithm must consider transposition of two adjacent characters as a single mistake. The default value is  true .

**Returns:**
boolean -  true  if the spelling corrector algorithm considers transpositions; otherwise  false .
### setConsiderTranspositions(boolean value) {#setConsiderTranspositions-boolean-}
```
public abstract void setConsiderTranspositions(boolean value)
```


Sets a value indicating whether the algorithm must consider transposition of two adjacent characters as a single mistake. The default value is  true .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  true  if the spelling corrector algorithm considers transpositions; otherwise  false . |

