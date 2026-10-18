---
title: "SpellingCorrectorOptions"
second_title: "GroupDocs.Search för Java API-referens"
description: "Tillhandahåller alternativ för stavningskorrigeringen."
type: docs
weight: 36
url: /sv/java/com.groupdocs.search.options/spellingcorrectoroptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class SpellingCorrectorOptions
```

Tillhandahåller alternativ för stavningskorrigeringen.


**Learn more**

* [Spell checking](../https://docs.groupdocs.com/display/searchjava/Spell+checking)
* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [SpellingCorrectorOptions()](#SpellingCorrectorOptions--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getEnabled()](#getEnabled--) | Hämtar ett värde som indikerar om stavningskorrigeringen är aktiverad. |
|
|  | [setEnabled(boolean value)](#setEnabled-boolean-) | Ställer in ett värde som indikerar om stavningskorrigeringen är aktiverad. |
|
|  | [getMaxMistakeCount()](#getMaxMistakeCount--) | Hämtar det maximala antalet fel. |
|
|  | [setMaxMistakeCount(int value)](#setMaxMistakeCount-int-) | Ställer in det maximala antalet fel. |
|
|  | [getOnlyBestResults()](#getOnlyBestResults--) | Hämtar ett värde som indikerar om endast de bästa resultaten ska returneras. |
|
|  | [setOnlyBestResults(boolean value)](#setOnlyBestResults-boolean-) | Ställer in ett värde som indikerar om endast de bästa resultaten ska returneras. |
|
|  | [getOnlyBestResultsRange()](#getOnlyBestResultsRange--) | Hämtar det maximala överskridandet av det minsta antalet fel som hittas. |
|
|  | [setOnlyBestResultsRange(byte value)](#setOnlyBestResultsRange-byte-) | Ställer in det maximala överskridandet av det minsta antalet fel som hittas. |
|
|  | [getConsiderTranspositions()](#getConsiderTranspositions--) | Hämtar ett värde som indikerar om algoritmen ska betrakta transponering av två intilliggande tecken som ett enda fel. |
|
|  | [setConsiderTranspositions(boolean value)](#setConsiderTranspositions-boolean-) | Ställer in ett värde som indikerar om algoritmen ska betrakta transponering av två intilliggande tecken som ett enda fel. |
|
### SpellingCorrectorOptions() {#SpellingCorrectorOptions--}
```
public SpellingCorrectorOptions()
```


### getEnabled() {#getEnabled--}
```
public abstract boolean getEnabled()
```


Hämtar ett värde som indikerar om stavningskorrigeringen är aktiverad. Standardvärdet är false.


**Returns:**
boolean - Ett värde som indikerar om stavningskorrigeringen är aktiverad.

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public abstract void setEnabled(boolean value)
```


Ställer in ett värde som indikerar om stavningskorrigeringen är aktiverad. Standardvärdet är false.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | boolean | Ett värde som indikerar om stavningskorrigeringen är aktiverad. |
|

### getMaxMistakeCount() {#getMaxMistakeCount--}
```
public abstract int getMaxMistakeCount()
```


Hämtar det maximala antalet fel. Standardvärdet är 2.


**Returns:**
int - Det maximala antalet misstag.

### setMaxMistakeCount(int value) {#setMaxMistakeCount-int-}
```
public abstract void setMaxMistakeCount(int value)
```


Ställer in det maximala antalet misstag. Standardvärdet är  2 .


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | int | Det maximala antalet misstag. |
|

### getOnlyBestResults() {#getOnlyBestResults--}
```
public abstract boolean getOnlyBestResults()
```


Hämtar ett värde som indikerar om endast de bästa resultaten ska returneras. Standardvärdet är  false .


**Returns:**
boolean -  true  om endast de bästa resultaten ska returneras; annars  false .

### setOnlyBestResults(boolean value) {#setOnlyBestResults-boolean-}
```
public abstract void setOnlyBestResults(boolean value)
```


Ställer in ett värde som indikerar om endast de bästa resultaten ska returneras. Standardvärdet är  false .


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | boolean | true  om endast de bästa resultaten ska returneras; annars  false . |
|

### getOnlyBestResultsRange() {#getOnlyBestResultsRange--}
```
public abstract byte getOnlyBestResultsRange()
```


Hämtar det maximala överskridandet av det minsta antalet misstag som hittas. Standardvärdet är  0 .


**Returns:**
byte - Det maximala överskridandet av det minsta antalet misstag som hittas.

### setOnlyBestResultsRange(byte value) {#setOnlyBestResultsRange-byte-}
```
public abstract void setOnlyBestResultsRange(byte value)
```


Ställer in det maximala överskridandet av det minsta antalet misstag som hittas. Standardvärdet är  0 .


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | byte | Det maximala överskridandet av det minsta antalet misstag som hittas. |
|

### getConsiderTranspositions() {#getConsiderTranspositions--}
```
public abstract boolean getConsiderTranspositions()
```


Hämtar ett värde som indikerar om algoritmen måste betrakta transposition av två intilliggande tecken som ett enda fel. Standardvärdet är  true .


**Returns:**
boolean -  true  om stavningskorrigeringsalgoritmen betraktar transpositioner; annars  false .

### setConsiderTranspositions(boolean value) {#setConsiderTranspositions-boolean-}
```
public abstract void setConsiderTranspositions(boolean value)
```


Ställer in ett värde som indikerar om algoritmen måste betrakta transposition av två intilliggande tecken som ett enda fel. Standardvärdet är  true .


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | boolean | true  om stavningskorrigeringsalgoritmen betraktar transpositioner; annars  false . |
|

