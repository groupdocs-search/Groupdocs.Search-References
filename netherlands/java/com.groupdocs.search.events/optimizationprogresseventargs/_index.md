---
title: "OptimizationProgressEventArgs"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt de argumenten voor het evenement voor wanneer de voortgang van de indexeringsbewerking wordt bijgewerkt."
type: docs
weight: 19
url: /nl/java/com.groupdocs.search.events/optimizationprogresseventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class OptimizationProgressEventArgs extends BaseIndexEventArgs
```

Stelt de argumenten voor het evenement voor wanneer de voortgang van de indexeringsbewerking wordt bijgewerkt.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getTotalSegments()](#getTotalSegments--) | Haalt het totale aantal segmenten voor verwerking op. |
|
|  | [getProcessedSegments()](#getProcessedSegments--) | Haalt het aantal verwerkte segmenten op. |
|
|  | [getProgressPercentage()](#getProgressPercentage--) | Haalt het percentage van de voortgang op. |
|
### getTotalSegments() {#getTotalSegments--}
```
public final int getTotalSegments()
```


Haalt het totale aantal segmenten voor verwerking op.


**Returns:**
int - Het totale aantal segmenten voor verwerking.

### getProcessedSegments() {#getProcessedSegments--}
```
public final int getProcessedSegments()
```


Haalt het aantal verwerkte segmenten op.


**Returns:**
int - Het aantal verwerkte segmenten.

### getProgressPercentage() {#getProgressPercentage--}
```
public final double getProgressPercentage()
```


Haalt het percentage van de voortgang op.


**Returns:**
double - Het percentage van de voortgang.

