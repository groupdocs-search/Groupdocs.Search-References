---
title: "NetworkIndexingProgressEventArgs"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt de argumenten voor het voortgangsveranderings‑evenement van de indexeringsbewerking voor."
type: docs
weight: 14
url: /nl/java/com.groupdocs.search.scaling.events/networkindexingprogresseventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class NetworkIndexingProgressEventArgs extends EventArgs
```

Stelt de argumenten voor het voortgangsveranderings‑evenement van de indexeringsbewerking voor.

## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getNodeIndex()](#getNodeIndex--) | Haalt de index van het zoeknetwerk‑knooppunt op. |
|
|  | [getServiceIndex()](#getServiceIndex--) | Haalt de index van de zoeknetwerk‑knooppuntservice op. |
|
|  | [getProcessedDocuments()](#getProcessedDocuments--) | Haalt het aantal verwerkte documenten op. |
|
|  | [getTotalDocuments()](#getTotalDocuments--) | Haalt het totale aantal documenten voor verwerking op. |
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

### getProcessedDocuments() {#getProcessedDocuments--}
```
public final int getProcessedDocuments()
```


Haalt het aantal verwerkte documenten op.


**Returns:**
int - Het aantal verwerkte documenten.

### getTotalDocuments() {#getTotalDocuments--}
```
public final int getTotalDocuments()
```


Haalt het totale aantal documenten voor verwerking op.


**Returns:**
int - Het totale aantal documenten voor verwerking.

### getProgressPercentage() {#getProgressPercentage--}
```
public final double getProgressPercentage()
```


Haalt het percentage van de voortgang op.


**Returns:**
double - Het percentage van de voortgang.

