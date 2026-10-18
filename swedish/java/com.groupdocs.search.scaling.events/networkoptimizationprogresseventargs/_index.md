---
title: "NetworkOptimizationProgressEventArgs"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar argumenten för framstegsändringshändelsen för optimeringsoperationen."
type: docs
weight: 15
url: /sv/java/com.groupdocs.search.scaling.events/networkoptimizationprogresseventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class NetworkOptimizationProgressEventArgs extends EventArgs
```

Representerar argumenten för framstegsändringshändelsen för optimeringsoperationen.

## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getNodeIndex()](#getNodeIndex--) | Hämtar index för söknätsnod. |
|
|  | [getServiceIndex()](#getServiceIndex--) | Hämtar index för söknätsnodtjänst. |
|
|  | [getProcessedSegments()](#getProcessedSegments--) | Hämtar antalet bearbetade segment. |
|
|  | [getTotalSegments()](#getTotalSegments--) | Hämtar det totala antalet segment för bearbetning. |
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

### getProcessedSegments() {#getProcessedSegments--}
```
public final int getProcessedSegments()
```


Hämtar antalet bearbetade segment.


**Returns:**
int - Antalet bearbetade segment.

### getTotalSegments() {#getTotalSegments--}
```
public final int getTotalSegments()
```


Hämtar det totala antalet segment för bearbetning.


**Returns:**
int - Det totala antalet segment för bearbetning.

### getProgressPercentage() {#getProgressPercentage--}
```
public final double getProgressPercentage()
```


Hämtar procentandelen av framstegen.


**Returns:**
double - Procentandelen av framstegen.

