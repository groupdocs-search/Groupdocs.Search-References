---
title: "NetworkOptimizationProgressEventArgs"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt de argumenten voor het voortgangsveranderings‑evenement van de optimalisatiebewerking voor."
type: docs
weight: 15
url: /nl/java/com.groupdocs.search.scaling.events/networkoptimizationprogresseventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class NetworkOptimizationProgressEventArgs extends EventArgs
```

Stelt de argumenten voor het voortgangsveranderings‑evenement van de optimalisatiebewerking voor.

## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getNodeIndex()](#getNodeIndex--) | Haalt de index van het zoeknetwerk‑knooppunt op. |
|
|  | [getServiceIndex()](#getServiceIndex--) | Haalt de index van de zoeknetwerk‑knooppuntservice op. |
|
|  | [getProcessedSegments()](#getProcessedSegments--) | Haalt het aantal verwerkte segmenten op. |
|
|  | [getTotalSegments()](#getTotalSegments--) | Haalt het totale aantal segmenten voor verwerking op. |
|
|  | [getProgressPercentage()](#getProgressPercentage--) | Haalt het percentage van de voortgang op. |
|
### getNodeIndex() {#getNodeIndex--}
```
public final int getNodeIndex()
```


Haalt de index van het zoeknetwerk‑knooppunt op.


**Returns:**
int - De index van het zoeknetwerk‑knooppunt.

### getServiceIndex() {#getServiceIndex--}
```
public final int getServiceIndex()
```


Haalt de index van de zoeknetwerk‑knooppuntservice op.


**Returns:**
int - De index van de zoeknetwerk‑knooppuntservice.

### getProcessedSegments() {#getProcessedSegments--}
```
public final int getProcessedSegments()
```


Haalt het aantal verwerkte segmenten op.


**Returns:**
int - Het aantal verwerkte segmenten.

### getTotalSegments() {#getTotalSegments--}
```
public final int getTotalSegments()
```


Haalt het totale aantal segmenten voor verwerking op.


**Returns:**
int - Het totale aantal segmenten voor verwerking.

### getProgressPercentage() {#getProgressPercentage--}
```
public final double getProgressPercentage()
```


Haalt het percentage van de voortgang op.


**Returns:**
double - Het percentage van de voortgang.

