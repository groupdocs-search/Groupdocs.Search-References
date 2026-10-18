---
title: "NetworkIndexingProgressEventArgs"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt die Argumente für das Fortschrittsänderungsereignis des Indexierungsvorgangs dar."
type: docs
weight: 14
url: /de/java/com.groupdocs.search.scaling.events/networkindexingprogresseventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class NetworkIndexingProgressEventArgs extends EventArgs
```

Stellt die Argumente für das Fortschrittsänderungsereignis des Indexierungsvorgangs dar.

## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getNodeIndex()](#getNodeIndex--) | Ermittelt den Index des Suchnetzwerk-Knotens. |
|
|  | [getServiceIndex()](#getServiceIndex--) | Ermittelt den Index des Suchnetzwerk-Knoten-Dienstes. |
|
|  | [getProcessedDocuments()](#getProcessedDocuments--) | Liefert die Anzahl der verarbeiteten Dokumente. |
|
|  | [getTotalDocuments()](#getTotalDocuments--) | Liefert die Gesamtzahl der zu verarbeitenden Dokumente. |
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

### getProcessedDocuments() {#getProcessedDocuments--}
```
public final int getProcessedDocuments()
```


Liefert die Anzahl der verarbeiteten Dokumente.


**Returns:**
int - Die Anzahl der verarbeiteten Dokumente.

### getTotalDocuments() {#getTotalDocuments--}
```
public final int getTotalDocuments()
```


Liefert die Gesamtzahl der zu verarbeitenden Dokumente.


**Returns:**
int - Die Gesamtzahl der zu verarbeitenden Dokumente.

### getProgressPercentage() {#getProgressPercentage--}
```
public final double getProgressPercentage()
```


Liefert den Prozentsatz des Fortschritts.


**Returns:**
double - Der Prozentsatz des Fortschritts.

