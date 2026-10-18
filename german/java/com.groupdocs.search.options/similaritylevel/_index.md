---
title: "SimilarityLevel"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt einen Algorithmus der unscharfen Suche dar, der das Ähnlichkeitsniveau festlegt."
type: docs
weight: 35
url: /de/java/com.groupdocs.search.options/similaritylevel/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.options.FuzzyAlgorithm](../../com.groupdocs.search.options/fuzzyalgorithm)
```
public class SimilarityLevel extends FuzzyAlgorithm
```

Stellt einen Algorithmus der unscharfen Suche dar, der den Ähnlichkeitsgrad festlegt. Der Ähnlichkeitsgrad-Algorithmus berechnet die maximale Anzahl von Fehlern für ein Wort, die umgekehrt proportional zur Wortlänge ist.


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
options.getFuzzySearch().setFuzzyAlgorithm(new SimilarityLevel(0.8)); // Erstellen des Fuzzy-Suchalgorithmus
// Diese Funktion legt 0 als maximale Fehlermenge für Wörter von 1 bis 4 Zeichen fest.
// Sie legt 1 als maximale Fehlermenge für Wörter von 5 bis 9 Zeichen fest.
// Sie legt 2 als maximale Fehlermenge für Wörter von 10 bis 14 Zeichen fest. Und so weiter.
SearchResult result = index.search(query, options); // Suche im Index
 
```
 
````


## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [SimilarityLevel(double value)](#SimilarityLevel-double-) | Initialisiert eine neue Instanz der Klasse SimilarityLevel. |
|
|  | [SimilarityLevel(Object data)](#SimilarityLevel-java.lang.Object-) | Initialisiert eine neue Instanz der Klasse SimilarityLevel. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getSimilarityLevel(int termLength)](#getSimilarityLevel-int-) | Gibt den Ähnlichkeitsgradwert für die angegebene Begriffslänge zurück. |
|
|  | [getMaxMistakeCount(int termLength)](#getMaxMistakeCount-int-) | Gibt die maximal zulässige Anzahl von Fehlern für die angegebene Begriffslänge zurück. |
|
### SimilarityLevel(double value) {#SimilarityLevel-double-}
```
public SimilarityLevel(double value)
```


Initialisiert eine neue Instanz der Klasse SimilarityLevel.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | double | Der Ähnlichkeitsgradwert. |
|

### SimilarityLevel(Object data) {#SimilarityLevel-java.lang.Object-}
```
public SimilarityLevel(Object data)
```


Initialisiert eine neue Instanz der Klasse SimilarityLevel.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Daten | java.lang.Object | Die serialisierten Daten. |
|

### getSimilarityLevel(int termLength) {#getSimilarityLevel-int-}
```
public double getSimilarityLevel(int termLength)
```


Gibt den Ähnlichkeitsgradwert für die angegebene Begriffslänge zurück.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | termLength | int | Die Termlänge. |
|

**Returns:**
double - Der Ähnlichkeitsgradwert.

### getMaxMistakeCount(int termLength) {#getMaxMistakeCount-int-}
```
public int getMaxMistakeCount(int termLength)
```


Gibt die maximal zulässige Anzahl von Fehlern für die angegebene Begriffslänge zurück.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | termLength | int | Die Termlänge. |
|

**Returns:**
int - Die maximal zulässige Anzahl von Fehlern.

