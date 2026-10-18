---
title: "NetworkIndexingProgressEventArgs"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar argumenten för framstegsändringshändelsen för indexeringsoperationen."
type: docs
weight: 14
url: /sv/java/com.groupdocs.search.scaling.events/networkindexingprogresseventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class NetworkIndexingProgressEventArgs extends EventArgs
```

Representerar argumenten för framstegsändringshändelsen för indexeringsoperationen.

## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getNodeIndex()](#getNodeIndex--) | Hämtar index för söknätsnod. |
|
|  | [getServiceIndex()](#getServiceIndex--) | Hämtar index för söknätsnodtjänst. |
|
|  | [getProcessedDocuments()](#getProcessedDocuments--) | Hämtar antalet bearbetade dokument. |
|
|  | [getTotalDocuments()](#getTotalDocuments--) | Hämtar det totala antalet dokument för bearbetning. |
|
|  | [getProgressPercentage()](#getProgressPercentage--) | Hämtar procentandelen av framstegen. |
|
### getNodeIndex() {#getNodeIndex--}
```
public final int getNodeIndex()
```


Hämtar index för söknätsnod.


**Returns:**
int - Index för söknätsnod.

### getServiceIndex() {#getServiceIndex--}
```
public final int getServiceIndex()
```


Hämtar index för söknätsnodtjänst.


**Returns:**
int - Index för söknätsnodtjänst.

### getProcessedDocuments() {#getProcessedDocuments--}
```
public final int getProcessedDocuments()
```


Hämtar antalet bearbetade dokument.


**Returns:**
int - Antalet bearbetade dokument.

### getTotalDocuments() {#getTotalDocuments--}
```
public final int getTotalDocuments()
```


Hämtar det totala antalet dokument för bearbetning.


**Returns:**
int - Det totala antalet dokument för bearbetning.

### getProgressPercentage() {#getProgressPercentage--}
```
public final double getProgressPercentage()
```


Hämtar procentandelen av framstegen.


**Returns:**
double - Procentandelen av framstegen.

