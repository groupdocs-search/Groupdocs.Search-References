---
title: "SimilarityLevel"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt een algoritme van de fuzzy-zoekopdracht voor dat het gelijkenisniveau specificeert."
type: docs
weight: 35
url: /nl/java/com.groupdocs.search.options/similaritylevel/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.options.FuzzyAlgorithm](../../com.groupdocs.search.options/fuzzyalgorithm)
```
public class SimilarityLevel extends FuzzyAlgorithm
```

Stelt een algoritme van de fuzzy-zoekopdracht voor dat het similariteitsniveau specificeert. Het similariteitsniveau-algoritme berekent het maximale aantal fouten voor een woord als omgekeerd evenredig met de lengte van het woord.


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
options.getFuzzySearch().setFuzzyAlgorithm(new SimilarityLevel(0.8)); // Het maken van het fuzzy-zoekalgoritme
// Deze functie specificeert 0 als het maximale aantal fouten voor woorden van 1 tot 4 tekens.
// Het specificeert 1 als het maximale aantal fouten voor woorden van 5 tot 9 tekens.
// Het specificeert 2 als het maximale aantal fouten voor woorden van 10 tot 14 tekens. En zo verder.
SearchResult result = index.search(query, options); // Zoeken in index
 
```
 
````


## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [SimilarityLevel(double value)](#SimilarityLevel-double-) | Initialiseert een nieuw exemplaar van de  SimilarityLevel  klasse. |
|
|  | [SimilarityLevel(Object data)](#SimilarityLevel-java.lang.Object-) | Initialiseert een nieuw exemplaar van de  SimilarityLevel  klasse. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getSimilarityLevel(int termLength)](#getSimilarityLevel-int-) | Haalt de similariteitsniveau-waarde op voor de opgegeven termlengte. |
|
|  | [getMaxMistakeCount(int termLength)](#getMaxMistakeCount-int-) | Haalt het maximaal toegestane aantal fouten op voor de opgegeven termlengte. |
|
### SimilarityLevel(double value) {#SimilarityLevel-double-}
```
public SimilarityLevel(double value)
```


Initialiseert een nieuw exemplaar van de  SimilarityLevel  klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | double | De similariteitsniveau-waarde. |
|

### SimilarityLevel(Object data) {#SimilarityLevel-java.lang.Object-}
```
public SimilarityLevel(Object data)
```


Initialiseert een nieuw exemplaar van de  SimilarityLevel  klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | gegevens | java.lang.Object | De geserialiseerde gegevens. |
|

### getSimilarityLevel(int termLength) {#getSimilarityLevel-int-}
```
public double getSimilarityLevel(int termLength)
```


Haalt de similariteitsniveau-waarde op voor de opgegeven termlengte.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | termLength | int | De termlengte. |
|

**Returns:**
double - De similariteitsniveau-waarde.

### getMaxMistakeCount(int termLength) {#getMaxMistakeCount-int-}
```
public int getMaxMistakeCount(int termLength)
```


Haalt het maximaal toegestane aantal fouten op voor de opgegeven termlengte.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | termLength | int | De termlengte. |
|

**Returns:**
int - Het maximum toegestane aantal fouten.

