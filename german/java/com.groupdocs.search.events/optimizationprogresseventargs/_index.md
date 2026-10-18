---
title: "OptimizationProgressEventArgs"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt Argumente für das Ereignis dar, wenn der Fortschritt des Indexierungsvorgangs aktualisiert wird."
type: docs
weight: 19
url: /de/java/com.groupdocs.search.events/optimizationprogresseventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class OptimizationProgressEventArgs extends BaseIndexEventArgs
```

Stellt Argumente für das Ereignis dar, wenn der Fortschritt des Indexierungsvorgangs aktualisiert wird.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getTotalSegments()](#getTotalSegments--) | Ermittelt die Gesamtzahl der zu verarbeitenden Segmente. |
|
|  | [getProcessedSegments()](#getProcessedSegments--) | Ermittelt die Anzahl der verarbeiteten Segmente. |
|
|  | [getProgressPercentage()](#getProgressPercentage--) | Liefert den Prozentsatz des Fortschritts. |
|
### getTotalSegments() {#getTotalSegments--}
```
public final int getTotalSegments()
```


Ermittelt die Gesamtzahl der zu verarbeitenden Segmente.


**Returns:**
int - Die Gesamtzahl der zu verarbeitenden Segmente.

### getProcessedSegments() {#getProcessedSegments--}
```
public final int getProcessedSegments()
```


Ermittelt die Anzahl der verarbeiteten Segmente.


**Returns:**
int - Die Anzahl der verarbeiteten Segmente.

### getProgressPercentage() {#getProgressPercentage--}
```
public final double getProgressPercentage()
```


Liefert den Prozentsatz des Fortschritts.


**Returns:**
double - Der Prozentsatz des Fortschritts.

