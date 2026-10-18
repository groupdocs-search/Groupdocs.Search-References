---
title: "TableDiscreteFunction"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar fuzzy-sökalgoritmen som innehåller korrespondenser mellan ordlängder och antalet tillåtna fel."
type: docs
weight: 40
url: /sv/java/com.groupdocs.search.options/tablediscretefunction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.options.FuzzyAlgorithm](../../com.groupdocs.search.options/fuzzyalgorithm)
```
public class TableDiscreteFunction extends FuzzyAlgorithm
```

Representerar den fuzzy-sökalgoritmen som innehåller korrespondenser mellan ordlängder och antalet tillåtna fel. Denna algoritm kan specificeras med en tabell av utdatavärden eller med en stegfunktion.


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
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1, new Step(5, 2), new Step(8, 3))); // Skapar fuzzy-sökalgoritmen
// Denna funktion anger 1 som maximalt antal fel för ord med 1 till 4 tecken.
// Den anger 2 som maximalt antal fel för ord med 5 till 7 tecken.
// Den anger 3 som maximalt antal fel för ord med 8 och fler tecken.
SearchResult result = index.search(query, options); // Sök i index
 
```
 
````


## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [TableDiscreteFunction(int offsetOfInputs, int[] tableOfOutputs)](#TableDiscreteFunction-int-int---) | Initierar en ny instans av klassen  TableDiscreteFunction  . |
|
|  | [TableDiscreteFunction(int firstStepLevel, Step[] steps)](#TableDiscreteFunction-int-com.groupdocs.search.options.Step...-) | Initierar en ny instans av klassen  TableDiscreteFunction  . |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getSimilarityLevel(int termLength)](#getSimilarityLevel-int-) | Hämtar en likhetsnivå för angiven termlängd. |
|
|  | [getMaxMistakeCount(int termLength)](#getMaxMistakeCount-int-) | Hämtar ett maximalt tillåtet antal fel för angiven termlängd. |
|
### TableDiscreteFunction(int offsetOfInputs, int[] tableOfOutputs) {#TableDiscreteFunction-int-int---}
```
public TableDiscreteFunction(int offsetOfInputs, int[] tableOfOutputs)
```


Initierar en ny instans av klassen  TableDiscreteFunction  .


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | offsetOfInputs | int | Offset för tabellindexen relativt inmatningsvärdena. |
|
|  | tableOfOutputs | int[] | Tabellen med utdatavärden. |
|

### TableDiscreteFunction(int firstStepLevel, Step[] steps) {#TableDiscreteFunction-int-com.groupdocs.search.options.Step...-}
```
public TableDiscreteFunction(int firstStepLevel, Step[] steps)
```


Initierar en ny instans av klassen  TableDiscreteFunction  .


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | firstStepLevel | int | Nivån för det första steget i stegfunktionen. |
|
|  | steps | [Step\[\]](../../com.groupdocs.search.options/step) | De följande stegen i stegfunktionen. |
|

### getSimilarityLevel(int termLength) {#getSimilarityLevel-int-}
```
public double getSimilarityLevel(int termLength)
```


Hämtar en likhetsnivå för angiven termlängd.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | termLength | int | Termlängden. |
|

**Returns:**
double - En likhetsnivå.

### getMaxMistakeCount(int termLength) {#getMaxMistakeCount-int-}
```
public int getMaxMistakeCount(int termLength)
```


Hämtar ett maximalt tillåtet antal fel för angiven termlängd.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | termLength | int | Termlängden. |
|

**Returns:**
int - Ett maximalt tillåtet antal fel.

