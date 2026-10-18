---
title: "NetworkOptimizationProgressEventArgs"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt die Argumente für das Fortschrittsänderungsereignis des Optimierungsvorgangs dar."
type: docs
weight: 15
url: /de/java/com.groupdocs.search.scaling.events/networkoptimizationprogresseventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class NetworkOptimizationProgressEventArgs extends EventArgs
```

Stellt die Argumente für das Fortschrittsänderungsereignis des Optimierungsvorgangs dar.

## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getNodeIndex()](#getNodeIndex--) | Ermittelt den Index des Suchnetzwerk-Knotens. |
|
|  | [getServiceIndex()](#getServiceIndex--) | Ermittelt den Index des Suchnetzwerk-Knoten-Dienstes. |
|
|  | [getProcessedSegments()](#getProcessedSegments--) | Ermittelt die Anzahl der verarbeiteten Segmente. |
|
|  | [getTotalSegments()](#getTotalSegments--) | Ermittelt die Gesamtzahl der zu verarbeitenden Segmente. |
|
|  | [getProgressPercentage()](#getProgressPercentage--) | Liefert den Prozentsatz des Fortschritts. |
|
### getNodeIndex() {#getNodeIndex--}
```
public final int getNodeIndex()
```


Ermittelt den Index des Suchnetzwerk-Knotens.


**Returns:**
int - Der Index des Suchnetzwerk-Knotens.

### getServiceIndex() {#getServiceIndex--}
```
public final int getServiceIndex()
```


Ermittelt den Index des Suchnetzwerk-Knoten-Dienstes.


**Returns:**
int - Der Index des Suchnetzwerk-Knoten-Dienstes.

### getProcessedSegments() {#getProcessedSegments--}
```
public final int getProcessedSegments()
```


Ermittelt die Anzahl der verarbeiteten Segmente.


**Returns:**
int - Die Anzahl der verarbeiteten Segmente.

### getTotalSegments() {#getTotalSegments--}
```
public final int getTotalSegments()
```


Ermittelt die Gesamtzahl der zu verarbeitenden Segmente.


**Returns:**
int - Die Gesamtzahl der zu verarbeitenden Segmente.

### getProgressPercentage() {#getProgressPercentage--}
```
public final double getProgressPercentage()
```


Liefert den Prozentsatz des Fortschritts.


**Returns:**
double - Der Prozentsatz des Fortschritts.

