---
title: "SimilarityLevel"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar en algoritm för fuzzy-sökning som specificerar likhetsnivån."
type: docs
weight: 35
url: /sv/java/com.groupdocs.search.options/similaritylevel/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.options.FuzzyAlgorithm](../../com.groupdocs.search.options/fuzzyalgorithm)
```
public class SimilarityLevel extends FuzzyAlgorithm
```

Representerar en algoritm för fuzzy-sökning som specificerar likhetsnivån. Algoritmen för likhetsnivå beräknar det maximala antalet fel för ett ord som omvänt proportionellt mot ordets längd.


**Learn more**

* [Fuzzy search](../https://docs.groupdocs.com/display/searchjava/Fuzzy+search)


Exemplet demonstrerar ett typiskt användningssätt av klassen.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Skapar ett index i den angivna mappen
index.add(documentsFolder); // Indexerar dokument från den angivna mappen
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // Aktiverar fuzzy-sökning
options.getFuzzySearch().setFuzzyAlgorithm(new SimilarityLevel(0.8)); // Skapar fuzzy-sökalgoritmen
// Denna funktion specificerar 0 som det maximala antalet fel för ord från 1 till 4 tecken.
// Den specificerar 1 som det maximala antalet fel för ord från 5 till 9 tecken.
// Den specificerar 2 som det maximala antalet fel för ord från 10 till 14 tecken. Och så vidare.
SearchResult result = index.search(query, options); // Sök i index
 
```
 
````


## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [SimilarityLevel(double value)](#SimilarityLevel-double-) | Initierar en ny instans av  SimilarityLevel  klassen. |
|
|  | [SimilarityLevel(Object data)](#SimilarityLevel-java.lang.Object-) | Initierar en ny instans av  SimilarityLevel  klassen. |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getSimilarityLevel(int termLength)](#getSimilarityLevel-int-) | Hämtar likhetsnivåvärdet för den angivna termlängden. |
|
|  | [getMaxMistakeCount(int termLength)](#getMaxMistakeCount-int-) | Hämtar det maximalt tillåtna antalet fel för den angivna termlängden. |
|
### SimilarityLevel(double value) {#SimilarityLevel-double-}
```
public SimilarityLevel(double value)
```


Initierar en ny instans av  SimilarityLevel  klassen.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | double | Likhetsnivåvärdet. |
|

### SimilarityLevel(Object data) {#SimilarityLevel-java.lang.Object-}
```
public SimilarityLevel(Object data)
```


Initierar en ny instans av  SimilarityLevel  klassen.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | data | java.lang.Object | Den serialiserade datan. |
|

### getSimilarityLevel(int termLength) {#getSimilarityLevel-int-}
```
public double getSimilarityLevel(int termLength)
```


Hämtar likhetsnivåvärdet för den angivna termlängden.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | termLength | int | Termlängden. |
|

**Returns:**
double - Likhetsnivåvärdet.

### getMaxMistakeCount(int termLength) {#getMaxMistakeCount-int-}
```
public int getMaxMistakeCount(int termLength)
```


Hämtar det maximalt tillåtna antalet fel för den angivna termlängden.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | termLength | int | Termlängden. |
|

**Returns:**
int - Det maximala tillåtna antalet misstag.

