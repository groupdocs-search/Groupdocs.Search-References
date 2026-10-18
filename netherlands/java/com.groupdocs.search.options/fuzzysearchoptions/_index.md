---
title: "FuzzySearchOptions"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Biedt opties voor de fuzzy-zoekopdracht."
type: docs
weight: 21
url: /nl/java/com.groupdocs.search.options/fuzzysearchoptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class FuzzySearchOptions
```

Biedt opties voor de fuzzy-zoekopdracht.


**Learn more**

* [Fuzzy search](../https://docs.groupdocs.com/display/searchjava/Fuzzy+search)
* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [FuzzySearchOptions()](#FuzzySearchOptions--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getEnabled()](#getEnabled--) | Haalt een waarde op die aangeeft of de fuzzy search-functie is ingeschakeld. |
|
|  | [setEnabled(boolean value)](#setEnabled-boolean-) | Stelt een waarde in die aangeeft of de fuzzy search-functie is ingeschakeld. |
|
|  | [getFuzzyAlgorithm()](#getFuzzyAlgorithm--) | Haalt het fuzzy search-algoritme op. |
|
|  | [setFuzzyAlgorithm(FuzzyAlgorithm value)](#setFuzzyAlgorithm-com.groupdocs.search.options.FuzzyAlgorithm-) | Stelt het fuzzy search-algoritme in. |
|
|  | [getOnlyBestResults()](#getOnlyBestResults--) | Haalt een waarde op die aangeeft of alleen de beste resultaten worden geretourneerd. |
|
|  | [setOnlyBestResults(boolean value)](#setOnlyBestResults-boolean-) | Stelt een waarde in die aangeeft of alleen de beste resultaten worden geretourneerd. |
|
|  | [getOnlyBestResultsRange()](#getOnlyBestResultsRange--) | Haalt de maximale overschrijding van het minimum aantal gevonden fouten op. |
|
|  | [setOnlyBestResultsRange(byte value)](#setOnlyBestResultsRange-byte-) | Stelt de maximale overschrijding van het minimum aantal gevonden fouten in. |
|
|  | [getConsiderTranspositions()](#getConsiderTranspositions--) | Haalt een waarde op die aangeeft of het fuzzy search-algoritme transpositie van twee aangrenzende tekens moet beschouwen als één fout. |
|
|  | [setConsiderTranspositions(boolean value)](#setConsiderTranspositions-boolean-) | Stelt een waarde in die aangeeft of het fuzzy search-algoritme transpositie van twee aangrenzende tekens moet beschouwen als één fout. |
|
### FuzzySearchOptions() {#FuzzySearchOptions--}
```
public FuzzySearchOptions()
```


### getEnabled() {#getEnabled--}
```
public abstract boolean getEnabled()
```


Haalt een waarde op die aangeeft of de fuzzy search-functie is ingeschakeld. De standaardwaarde is  false .


**Returns:**
boolean - Een waarde die aangeeft of de fuzzy search-functie is ingeschakeld.

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public abstract void setEnabled(boolean value)
```


Stelt een waarde in die aangeeft of de fuzzy search-functie is ingeschakeld. De standaardwaarde is  false .


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | boolean | Een waarde die aangeeft of de fuzzy search-functie is ingeschakeld. |
|

### getFuzzyAlgorithm() {#getFuzzyAlgorithm--}
```
public abstract FuzzyAlgorithm getFuzzyAlgorithm()
```


Haalt het fuzzy search-algoritme op. De momenteel beschikbare fuzzy search-algoritmen zijn  SimilarityLevel  en  TableDiscreteFunction . De standaardwaarde is een instantie van  SimilarityLevel  met een similariteitsniveau van  0.5 .


**Returns:**
[FuzzyAlgorithm](../../com.groupdocs.search.options/fuzzyalgorithm) - The fuzzy search algorithm.


Het voorbeeld laat zien hoe het fuzzy search-algoritme moet worden ingesteld.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Een index maken in de opgegeven map
index.add(documentsFolder); // Documenten indexeren vanuit de opgegeven map
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // Fuzzy-zoekopdracht inschakelen
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1, new Step(5, 2), new Step(8, 3))); // Het fuzzy-zoekalgoritme maken
// Deze functie specificeert 1 als het maximale aantal fouten voor woorden van 1 tot 4 tekens.
// Het specificeert 2 als het maximale aantal fouten voor woorden van 5 tot 7 tekens.
// Het specificeert 3 als het maximale aantal fouten voor woorden van 8 en meer tekens.
SearchResult result = index.search(query, options); // Zoeken in index
 
```
 
````


### setFuzzyAlgorithm(FuzzyAlgorithm value) {#setFuzzyAlgorithm-com.groupdocs.search.options.FuzzyAlgorithm-}
```
public abstract void setFuzzyAlgorithm(FuzzyAlgorithm value)
```


Stelt het fuzzy search-algoritme in. De momenteel beschikbare fuzzy search-algoritmen zijn  SimilarityLevel  en  TableDiscreteFunction . De standaardwaarde is een instantie van  SimilarityLevel  met een similariteitsniveau van  0.5 .


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | value | [FuzzyAlgorithm](../../com.groupdocs.search.options/fuzzyalgorithm) | Het fuzzy search-algoritme. |


Het voorbeeld laat zien hoe het fuzzy search-algoritme moet worden ingesteld.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Een index maken in de opgegeven map
index.add(documentsFolder); // Documenten indexeren vanuit de opgegeven map
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // Fuzzy-zoekopdracht inschakelen
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1, new Step(5, 2), new Step(8, 3))); // Het fuzzy-zoekalgoritme maken
// Deze functie specificeert 1 als het maximale aantal fouten voor woorden van 1 tot 4 tekens.
// Het specificeert 2 als het maximale aantal fouten voor woorden van 5 tot 7 tekens.
// Het specificeert 3 als het maximale aantal fouten voor woorden van 8 en meer tekens.
SearchResult result = index.search(query, options); // Zoeken in index
 
```
 
````

|

### getOnlyBestResults() {#getOnlyBestResults--}
```
public abstract boolean getOnlyBestResults()
```


Haalt een waarde op die aangeeft of alleen de beste resultaten worden geretourneerd. De standaardwaarde is  false .


**Returns:**
boolean -  true  als alleen de beste resultaten worden geretourneerd; anders  false .

### setOnlyBestResults(boolean value) {#setOnlyBestResults-boolean-}
```
public abstract void setOnlyBestResults(boolean value)
```


Stelt een waarde in die aangeeft of alleen de beste resultaten worden geretourneerd. De standaardwaarde is  false .


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | boolean | true  als alleen de beste resultaten worden geretourneerd; anders  false . |
|

### getOnlyBestResultsRange() {#getOnlyBestResultsRange--}
```
public abstract byte getOnlyBestResultsRange()
```


Haalt het maximale overschrijding van het minimum aantal gevonden fouten op. De standaardwaarde is  0 .


**Returns:**
byte - Het maximale overschrijding van het minimum aantal gevonden fouten.

### setOnlyBestResultsRange(byte value) {#setOnlyBestResultsRange-byte-}
```
public abstract void setOnlyBestResultsRange(byte value)
```


Stelt het maximale overschrijding van het minimum aantal gevonden fouten in. De standaardwaarde is  0 .


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | byte | Het maximale overschrijding van het minimum aantal gevonden fouten. |
|

### getConsiderTranspositions() {#getConsiderTranspositions--}
```
public abstract boolean getConsiderTranspositions()
```


Haalt een waarde op die aangeeft of het fuzzy search-algoritme transpositie van twee aangrenzende tekens moet beschouwen als één fout. De standaardwaarde is  true .


**Returns:**
boolean -  true  als het fuzzy search-algoritme transposities beschouwt; anders  false .

### setConsiderTranspositions(boolean value) {#setConsiderTranspositions-boolean-}
```
public abstract void setConsiderTranspositions(boolean value)
```


Stelt een waarde in die aangeeft of het fuzzy search-algoritme transpositie van twee aangrenzende tekens moet beschouwen als één fout. De standaardwaarde is  true .


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | boolean | :  true  als het fuzzy search-algoritme transposities beschouwt; anders  false . |
|

