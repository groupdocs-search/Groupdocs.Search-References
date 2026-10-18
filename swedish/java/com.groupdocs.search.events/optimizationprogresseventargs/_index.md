---
title: "OptimizationProgressEventArgs"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar argument för händelsen när framstegen för indexeringsoperationen uppdateras."
type: docs
weight: 19
url: /sv/java/com.groupdocs.search.events/optimizationprogresseventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class OptimizationProgressEventArgs extends BaseIndexEventArgs
```

Representerar argument för händelsen när framstegen för indexeringsoperationen uppdateras.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getTotalSegments()](#getTotalSegments--) | Hämtar det totala antalet segment för bearbetning. |
|
|  | [getProcessedSegments()](#getProcessedSegments--) | Hämtar antalet bearbetade segment. |
|
|  | [getProgressPercentage()](#getProgressPercentage--) | Hämtar procentandelen av framstegen. |
|
### getTotalSegments() {#getTotalSegments--}
```
public final int getTotalSegments()
```


Hämtar det totala antalet segment för bearbetning.


**Returns:**
int - Det totala antalet segment för bearbetning.

### getProcessedSegments() {#getProcessedSegments--}
```
public final int getProcessedSegments()
```


Hämtar antalet bearbetade segment.


**Returns:**
int - Antalet bearbetade segment.

### getProgressPercentage() {#getProgressPercentage--}
```
public final double getProgressPercentage()
```


Hämtar procentandelen av framstegen.


**Returns:**
double - Procentandelen av framstegen.

