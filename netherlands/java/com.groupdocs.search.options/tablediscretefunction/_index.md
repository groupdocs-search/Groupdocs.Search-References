---
title: "TableDiscreteFunction"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt het fuzzy-zoekalgoritme voor dat overeenkomsten bevat tussen woordlengtes en het aantal toegestane fouten."
type: docs
weight: 40
url: /nl/java/com.groupdocs.search.options/tablediscretefunction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.options.FuzzyAlgorithm](../../com.groupdocs.search.options/fuzzyalgorithm)
```
public class TableDiscreteFunction extends FuzzyAlgorithm
```

Stelt het fuzzy-zoekalgoritme voor dat overeenkomsten bevat tussen woordlengtes en het aantal toegestane fouten. Dit algoritme kan worden gespecificeerd door een tabel met uitvoerwaarden of door een stapfunctie.


**Learn more**

* [Fuzzy search](../https://docs.groupdocs.com/display/searchjava/Fuzzy+search)


Het voorbeeld toont een typisch gebruik van de klasse.

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


## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [TableDiscreteFunction(int offsetOfInputs, int[] tableOfOutputs)](#TableDiscreteFunction-int-int---) | Initialiseert een nieuw exemplaar van de  TableDiscreteFunction  klasse. |
|
|  | [TableDiscreteFunction(int firstStepLevel, Step[] steps)](#TableDiscreteFunction-int-com.groupdocs.search.options.Step...-) | Initialiseert een nieuw exemplaar van de  TableDiscreteFunction  klasse. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getSimilarityLevel(int termLength)](#getSimilarityLevel-int-) | Haalt een similariteitsniveau op voor de opgegeven termlengte. |
|
|  | [getMaxMistakeCount(int termLength)](#getMaxMistakeCount-int-) | Haalt het maximaal toegestane aantal fouten op voor opgegeven termlengte. |
|
### TableDiscreteFunction(int offsetOfInputs, int[] tableOfOutputs) {#TableDiscreteFunction-int-int---}
```
public TableDiscreteFunction(int offsetOfInputs, int[] tableOfOutputs)
```


Initialiseert een nieuw exemplaar van de  TableDiscreteFunction  klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | offsetOfInputs | int | De offset van de tabelindexen ten opzichte van de invoerwaarden. |
|
|  | tableOfOutputs | int[] | De tabel met uitvoerwaarden. |
|

### TableDiscreteFunction(int firstStepLevel, Step[] steps) {#TableDiscreteFunction-int-com.groupdocs.search.options.Step...-}
```
public TableDiscreteFunction(int firstStepLevel, Step[] steps)
```


Initialiseert een nieuw exemplaar van de  TableDiscreteFunction  klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | firstStepLevel | int | Het niveau van de eerste stap van de stapfunctie. |
|
|  | steps | [Step\[\]](../../com.groupdocs.search.options/step) | De volgende stappen van de stapfunctie. |
|

### getSimilarityLevel(int termLength) {#getSimilarityLevel-int-}
```
public double getSimilarityLevel(int termLength)
```


Haalt een similariteitsniveau op voor de opgegeven termlengte.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | termLength | int | De termlengte. |
|

**Returns:**
double - Een similariteitsniveau.

### getMaxMistakeCount(int termLength) {#getMaxMistakeCount-int-}
```
public int getMaxMistakeCount(int termLength)
```


Haalt het maximaal toegestane aantal fouten op voor opgegeven termlengte.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | termLength | int | De termlengte. |
|

**Returns:**
int - Een maximaal toegestaan aantal fouten.

