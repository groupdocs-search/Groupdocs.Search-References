---
title: "TableDiscreteFunction"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt den Algorithmus der unscharfen Suche dar, der Zuordnungen zwischen Wortlängen und der Anzahl zulässiger Fehler enthält."
type: docs
weight: 40
url: /de/java/com.groupdocs.search.options/tablediscretefunction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.options.FuzzyAlgorithm](../../com.groupdocs.search.options/fuzzyalgorithm)
```
public class TableDiscreteFunction extends FuzzyAlgorithm
```

Stellt den Fuzzy‑Suchalgorithmus dar, der Zuordnungen zwischen Wortlängen und der Anzahl zulässiger Fehler enthält. Dieser Algorithmus kann durch eine Tabelle von Ausgabewerten oder durch eine Stufenfunktion angegeben werden.


**Learn more**

* [Fuzzy search](../https://docs.groupdocs.com/display/searchjava/Fuzzy+search)


Das Beispiel demonstriert eine typische Verwendung der Klasse.

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


## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [TableDiscreteFunction(int offsetOfInputs, int[] tableOfOutputs)](#TableDiscreteFunction-int-int---) | Initialisiert eine neue Instanz der Klasse TableDiscreteFunction. |
|
|  | [TableDiscreteFunction(int firstStepLevel, Step[] steps)](#TableDiscreteFunction-int-com.groupdocs.search.options.Step...-) | Initialisiert eine neue Instanz der Klasse TableDiscreteFunction. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getSimilarityLevel(int termLength)](#getSimilarityLevel-int-) | Ermittelt einen Ähnlichkeitsgrad für die angegebene Termlänge. |
|
|  | [getMaxMistakeCount(int termLength)](#getMaxMistakeCount-int-) | Ermittelt die maximal zulässige Anzahl von Fehlern für die angegebene Termlänge. |
|
### TableDiscreteFunction(int offsetOfInputs, int[] tableOfOutputs) {#TableDiscreteFunction-int-int---}
```
public TableDiscreteFunction(int offsetOfInputs, int[] tableOfOutputs)
```


Initialisiert eine neue Instanz der Klasse TableDiscreteFunction.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | offsetOfInputs | int | Der Versatz der Tabellenindizes relativ zu den Eingabewerten. |
|
|  | tableOfOutputs | int[] | Die Tabelle der Ausgabewerte. |
|

### TableDiscreteFunction(int firstStepLevel, Step[] steps) {#TableDiscreteFunction-int-com.groupdocs.search.options.Step...-}
```
public TableDiscreteFunction(int firstStepLevel, Step[] steps)
```


Initialisiert eine neue Instanz der Klasse TableDiscreteFunction.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | firstStepLevel | int | Der Level des ersten Schritts der Stufenfunktion. |
|
|  | steps | [Step\[\]](../../com.groupdocs.search.options/step) | Die nächsten Schritte der Stufenfunktion. |
|

### getSimilarityLevel(int termLength) {#getSimilarityLevel-int-}
```
public double getSimilarityLevel(int termLength)
```


Ermittelt einen Ähnlichkeitsgrad für die angegebene Termlänge.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | termLength | int | Die Termlänge. |
|

**Returns:**
double - Ein Ähnlichkeitsgrad.

### getMaxMistakeCount(int termLength) {#getMaxMistakeCount-int-}
```
public int getMaxMistakeCount(int termLength)
```


Ermittelt die maximal zulässige Anzahl von Fehlern für die angegebene Termlänge.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | termLength | int | Die Termlänge. |
|

**Returns:**
int - Eine maximal zulässige Anzahl von Fehlern.

