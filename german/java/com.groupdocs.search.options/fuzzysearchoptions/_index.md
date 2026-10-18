---
title: "FuzzySearchOptions"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Bietet Optionen für die Fuzzy‑Suche."
type: docs
weight: 21
url: /de/java/com.groupdocs.search.options/fuzzysearchoptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class FuzzySearchOptions
```

Bietet Optionen für die Fuzzy‑Suche.


**Learn more**

* [Fuzzy search](../https://docs.groupdocs.com/display/searchjava/Fuzzy+search)
* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [FuzzySearchOptions()](#FuzzySearchOptions--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getEnabled()](#getEnabled--) | Gibt einen Wert zurück, der angibt, ob die Fuzzy‑Suche‑Funktion aktiviert ist. |
|
|  | [setEnabled(boolean value)](#setEnabled-boolean-) | Legt einen Wert fest, der angibt, ob die Fuzzy‑Suche aktiviert ist. |
|
|  | [getFuzzyAlgorithm()](#getFuzzyAlgorithm--) | Ruft den Fuzzy‑Suchalgorithmus ab. |
|
|  | [setFuzzyAlgorithm(FuzzyAlgorithm value)](#setFuzzyAlgorithm-com.groupdocs.search.options.FuzzyAlgorithm-) | Legt den Fuzzy‑Suchalgorithmus fest. |
|
|  | [getOnlyBestResults()](#getOnlyBestResults--) | Gibt einen Wert zurück, der angibt, ob nur die besten Ergebnisse zurückgegeben werden. |
|
|  | [setOnlyBestResults(boolean value)](#setOnlyBestResults-boolean-) | Legt einen Wert fest, der angibt, ob nur die besten Ergebnisse zurückgegeben werden. |
|
|  | [getOnlyBestResultsRange()](#getOnlyBestResultsRange--) | Gibt das maximale Überschreiten der minimal gefundenen Fehleranzahl zurück. |
|
|  | [setOnlyBestResultsRange(byte value)](#setOnlyBestResultsRange-byte-) | Legt das maximale Überschreiten der minimal gefundenen Fehleranzahl fest. |
|
|  | [getConsiderTranspositions()](#getConsiderTranspositions--) | Ruft einen Wert ab, der angibt, ob der Fuzzy‑Suchalgorithmus die Vertauschung zweier benachbarter Zeichen als einen einzelnen Fehler berücksichtigen muss. |
|
|  | [setConsiderTranspositions(boolean value)](#setConsiderTranspositions-boolean-) | Legt einen Wert fest, der angibt, ob der Fuzzy‑Suchalgorithmus die Vertauschung zweier benachbarter Zeichen als einen einzelnen Fehler berücksichtigen muss. |
|
### FuzzySearchOptions() {#FuzzySearchOptions--}
```
public FuzzySearchOptions()
```


### getEnabled() {#getEnabled--}
```
public abstract boolean getEnabled()
```


Ruft einen Wert ab, der angibt, ob die Fuzzy‑Suche aktiviert ist. Der Standardwert ist false.


**Returns:**
boolean – Ein Wert, der angibt, ob die Fuzzy‑Suche aktiviert ist.

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public abstract void setEnabled(boolean value)
```


Legt einen Wert fest, der angibt, ob die Fuzzy‑Suche aktiviert ist. Der Standardwert ist false.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | boolean | Ein Wert, der angibt, ob die Fuzzy‑Suche aktiviert ist. |
|

### getFuzzyAlgorithm() {#getFuzzyAlgorithm--}
```
public abstract FuzzyAlgorithm getFuzzyAlgorithm()
```


Ruft den Fuzzy‑Suchalgorithmus ab. Die derzeit verfügbaren Fuzzy‑Suchalgorithmen sind SimilarityLevel und TableDiscreteFunction. Der Standardwert ist eine Instanz von SimilarityLevel mit einem Ähnlichkeitsgrad von 0.5.


**Returns:**
[FuzzyAlgorithm](../../com.groupdocs.search.options/fuzzyalgorithm) - The fuzzy search algorithm.


Das Beispiel zeigt, wie der Fuzzy‑Suchalgorithmus festgelegt wird.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Erstellen eines Index im angegebenen Ordner
index.add(documentsFolder); // Indizieren von Dokumenten aus dem angegebenen Ordner
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // Aktivieren der unscharfen Suche
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1, new Step(5, 2), new Step(8, 3))); // Erstellen des Fuzzy‑Suchalgorithmus
// Diese Funktion legt 1 als maximale Fehleranzahl für Wörter von 1 bis 4 Zeichen fest.
// Sie legt 2 als maximale Fehleranzahl für Wörter von 5 bis 7 Zeichen fest.
// Sie legt 3 als maximale Fehleranzahl für Wörter von 8 und mehr Zeichen fest.
SearchResult result = index.search(query, options); // Suche im Index
 
```
 
````


### setFuzzyAlgorithm(FuzzyAlgorithm value) {#setFuzzyAlgorithm-com.groupdocs.search.options.FuzzyAlgorithm-}
```
public abstract void setFuzzyAlgorithm(FuzzyAlgorithm value)
```


Legt den Fuzzy‑Suchalgorithmus fest. Die derzeit verfügbaren Fuzzy‑Suchalgorithmen sind SimilarityLevel und TableDiscreteFunction. Der Standardwert ist eine Instanz von SimilarityLevel mit einem Ähnlichkeitsgrad von 0.5.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | value | [FuzzyAlgorithm](../../com.groupdocs.search.options/fuzzyalgorithm) | Der Fuzzy‑Suchalgorithmus. |


Das Beispiel zeigt, wie der Fuzzy‑Suchalgorithmus festgelegt wird.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Erstellen eines Index im angegebenen Ordner
index.add(documentsFolder); // Indizieren von Dokumenten aus dem angegebenen Ordner
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // Aktivieren der unscharfen Suche
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1, new Step(5, 2), new Step(8, 3))); // Erstellen des Fuzzy‑Suchalgorithmus
// Diese Funktion legt 1 als maximale Fehleranzahl für Wörter von 1 bis 4 Zeichen fest.
// Sie legt 2 als maximale Fehleranzahl für Wörter von 5 bis 7 Zeichen fest.
// Sie legt 3 als maximale Fehleranzahl für Wörter von 8 und mehr Zeichen fest.
SearchResult result = index.search(query, options); // Suche im Index
 
```
 
````

|

### getOnlyBestResults() {#getOnlyBestResults--}
```
public abstract boolean getOnlyBestResults()
```


Gibt einen Wert zurück, der angibt, ob nur die besten Ergebnisse zurückgegeben werden. Der Standardwert ist false.


**Returns:**
boolean - true, wenn nur die besten Ergebnisse zurückgegeben werden; andernfalls false.

### setOnlyBestResults(boolean value) {#setOnlyBestResults-boolean-}
```
public abstract void setOnlyBestResults(boolean value)
```


Legt einen Wert fest, der angibt, ob nur die besten Ergebnisse zurückgegeben werden. Der Standardwert ist false.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | boolean | true, wenn nur die besten Ergebnisse zurückgegeben werden; andernfalls false. |
|

### getOnlyBestResultsRange() {#getOnlyBestResultsRange--}
```
public abstract byte getOnlyBestResultsRange()
```


Gibt die maximale Überschreitung der minimal gefundenen Fehleranzahl zurück. Der Standardwert ist 0.


**Returns:**
byte - Die maximale Überschreitung der minimal gefundenen Fehleranzahl.

### setOnlyBestResultsRange(byte value) {#setOnlyBestResultsRange-byte-}
```
public abstract void setOnlyBestResultsRange(byte value)
```


Legt die maximale Überschreitung der minimal gefundenen Fehleranzahl fest. Der Standardwert ist 0.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | byte | Die maximale Überschreitung der minimal gefundenen Fehleranzahl. |
|

### getConsiderTranspositions() {#getConsiderTranspositions--}
```
public abstract boolean getConsiderTranspositions()
```


Ruft einen Wert ab, der angibt, ob der Fuzzy‑Suchalgorithmus die Vertauschung zweier benachbarter Zeichen als einen einzelnen Fehler berücksichtigen muss. Der Standardwert ist true.


**Returns:**
boolean – true, wenn der Fuzzy‑Suchalgorithmus Vertauschungen berücksichtigt; andernfalls false.

### setConsiderTranspositions(boolean value) {#setConsiderTranspositions-boolean-}
```
public abstract void setConsiderTranspositions(boolean value)
```


Legt einen Wert fest, der angibt, ob der Fuzzy‑Suchalgorithmus die Vertauschung zweier benachbarter Zeichen als einen einzelnen Fehler berücksichtigen muss. Der Standardwert ist true.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | boolean | : true, wenn der Fuzzy‑Suchalgorithmus Vertauschungen berücksichtigt; andernfalls false. |
|

