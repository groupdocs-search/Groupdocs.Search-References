---
title: "FuzzySearchOptions"
second_title: "GroupDocs.Search för Java API-referens"
description: "Tillhandahåller alternativ för fuzzy-sökning."
type: docs
weight: 21
url: /sv/java/com.groupdocs.search.options/fuzzysearchoptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class FuzzySearchOptions
```

Tillhandahåller alternativ för fuzzy-sökning.


**Learn more**

* [Fuzzy search](../https://docs.groupdocs.com/display/searchjava/Fuzzy+search)
* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [FuzzySearchOptions()](#FuzzySearchOptions--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getEnabled()](#getEnabled--) | Hämtar ett värde som indikerar om funktionen för fuzzy-sökning är aktiverad. |
|
|  | [setEnabled(boolean value)](#setEnabled-boolean-) | Ställer in ett värde som anger om fuzzy‑sökfunktionen är aktiverad. |
|
|  | [getFuzzyAlgorithm()](#getFuzzyAlgorithm--) | Hämtar fuzzy‑sökalgoritmen. |
|
|  | [setFuzzyAlgorithm(FuzzyAlgorithm value)](#setFuzzyAlgorithm-com.groupdocs.search.options.FuzzyAlgorithm-) | Ställer in fuzzy‑sökalgoritmen. |
|
|  | [getOnlyBestResults()](#getOnlyBestResults--) | Hämtar ett värde som indikerar om endast de bästa resultaten ska returneras. |
|
|  | [setOnlyBestResults(boolean value)](#setOnlyBestResults-boolean-) | Ställer in ett värde som indikerar om endast de bästa resultaten ska returneras. |
|
|  | [getOnlyBestResultsRange()](#getOnlyBestResultsRange--) | Hämtar det maximala överskridandet av det minsta antalet fel som hittas. |
|
|  | [setOnlyBestResultsRange(byte value)](#setOnlyBestResultsRange-byte-) | Ställer in det maximala överskridandet av det minsta antalet fel som hittas. |
|
|  | [getConsiderTranspositions()](#getConsiderTranspositions--) | Hämtar ett värde som anger om fuzzy‑sökalgoritmen måste betrakta transponering av två intilliggande tecken som ett enda fel. |
|
|  | [setConsiderTranspositions(boolean value)](#setConsiderTranspositions-boolean-) | Ställer in ett värde som anger om fuzzy‑sökalgoritmen måste betrakta transponering av två intilliggande tecken som ett enda fel. |
|
### FuzzySearchOptions() {#FuzzySearchOptions--}
```
public FuzzySearchOptions()
```


### getEnabled() {#getEnabled--}
```
public abstract boolean getEnabled()
```


Hämtar ett värde som anger om fuzzy‑sökfunktionen är aktiverad. Standardvärdet är falskt.


**Returns:**
boolesk - Ett värde som anger om fuzzy‑sökfunktionen är aktiverad.

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public abstract void setEnabled(boolean value)
```


Ställer in ett värde som anger om fuzzy‑sökfunktionen är aktiverad. Standardvärdet är falskt.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | boolean | Ett värde som anger om fuzzy‑sökfunktionen är aktiverad. |
|

### getFuzzyAlgorithm() {#getFuzzyAlgorithm--}
```
public abstract FuzzyAlgorithm getFuzzyAlgorithm()
```


Hämtar fuzzy‑sökalgoritmen. De för närvarande tillgängliga fuzzy‑sökalgoritmerna är SimilarityLevel och TableDiscreteFunction. Standardvärdet är en instans av SimilarityLevel med ett likhetsnivåvärde på 0,5.


**Returns:**
[FuzzyAlgorithm](../../com.groupdocs.search.options/fuzzyalgorithm) - The fuzzy search algorithm.


Exemplet visar hur man ställer in fuzzy‑sökalgoritmen.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Skapar ett index i den angivna mappen
index.add(documentsFolder); // Indexerar dokument från den angivna mappen
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // Aktiverar fuzzy-sökning
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1, new Step(5, 2), new Step(8, 3))); // Skapar fuzzy-sökalgoritmen
// Denna funktion anger 1 som maximalt antal fel för ord med 1 till 4 tecken.
// Den anger 2 som maximalt antal fel för ord med 5 till 7 tecken.
// Den anger 3 som maximalt antal fel för ord med 8 och fler tecken.
SearchResult result = index.search(query, options); // Sök i index
 
```
 
````


### setFuzzyAlgorithm(FuzzyAlgorithm value) {#setFuzzyAlgorithm-com.groupdocs.search.options.FuzzyAlgorithm-}
```
public abstract void setFuzzyAlgorithm(FuzzyAlgorithm value)
```


Ställer in fuzzy‑sökalgoritmen. De för närvarande tillgängliga fuzzy‑sökalgoritmerna är SimilarityLevel och TableDiscreteFunction. Standardvärdet är en instans av SimilarityLevel med ett likhetsnivåvärde på 0,5.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | value | [FuzzyAlgorithm](../../com.groupdocs.search.options/fuzzyalgorithm) | Fuzzy‑sökalgoritmen. |


Exemplet visar hur man ställer in fuzzy‑sökalgoritmen.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Skapar ett index i den angivna mappen
index.add(documentsFolder); // Indexerar dokument från den angivna mappen
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // Aktiverar fuzzy-sökning
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1, new Step(5, 2), new Step(8, 3))); // Skapar fuzzy-sökalgoritmen
// Denna funktion anger 1 som maximalt antal fel för ord med 1 till 4 tecken.
// Den anger 2 som maximalt antal fel för ord med 5 till 7 tecken.
// Den anger 3 som maximalt antal fel för ord med 8 och fler tecken.
SearchResult result = index.search(query, options); // Sök i index
 
```
 
````

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


Hämtar ett värde som anger om fuzzy‑sökalgoritmen måste betrakta transponering av två intilliggande tecken som ett enda fel. Standardvärdet är sant.


**Returns:**
boolesk - sant om fuzzy‑sökalgoritmen beaktar transponeringar; annars falskt.

### setConsiderTranspositions(boolean value) {#setConsiderTranspositions-boolean-}
```
public abstract void setConsiderTranspositions(boolean value)
```


Ställer in ett värde som anger om fuzzy‑sökalgoritmen måste betrakta transponering av två intilliggande tecken som ett enda fel. Standardvärdet är sant.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | boolean | : sant om fuzzy‑sökalgoritmen beaktar transponeringar; annars falskt. |
|

