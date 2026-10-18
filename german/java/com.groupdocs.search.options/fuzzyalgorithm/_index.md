---
title: "FuzzyAlgorithm"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt die Basisklasse für Fuzzy‑Suchalgorithmen dar."
type: docs
weight: 20
url: /de/java/com.groupdocs.search.options/fuzzyalgorithm/
---
**Inheritance:**
java.lang.Object
```
public abstract class FuzzyAlgorithm
```

Stellt die Basisklasse für Fuzzy‑Suchalgorithmen dar.


**Learn more**

* [Fuzzy search](../https://docs.groupdocs.com/display/searchjava/Fuzzy+search)

## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getSimilarityLevel(int termLength)](#getSimilarityLevel-int-) | Ermittelt den Ähnlichkeitsgrad für die angegebene Begriffslänge. |
|
|  | [getMaxMistakeCount(int termLength)](#getMaxMistakeCount-int-) | Gibt die maximal zulässige Anzahl von Fehlern für die angegebene Begriffslänge zurück. |
|
| [getCore()](#getCore--) |  |
### getSimilarityLevel(int termLength) {#getSimilarityLevel-int-}
```
public abstract double getSimilarityLevel(int termLength)
```


Ermittelt den Ähnlichkeitsgrad für die angegebene Begriffslänge.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | termLength | int | Die Termlänge. |
|

**Returns:**
double - Der Ähnlichkeitsgrad.

### getMaxMistakeCount(int termLength) {#getMaxMistakeCount-int-}
```
public abstract int getMaxMistakeCount(int termLength)
```


Gibt die maximal zulässige Anzahl von Fehlern für die angegebene Begriffslänge zurück.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | termLength | int | Die Termlänge. |
|

**Returns:**
int - Die maximal zulässige Anzahl von Fehlern.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
