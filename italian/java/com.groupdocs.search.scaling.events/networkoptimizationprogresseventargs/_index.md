---
title: "NetworkOptimizationProgressEventArgs"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta gli argomenti per l'evento di cambiamento di avanzamento dell'operazione di ottimizzazione."
type: docs
weight: 15
url: /it/java/com.groupdocs.search.scaling.events/networkoptimizationprogresseventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class NetworkOptimizationProgressEventArgs extends EventArgs
```

Rappresenta gli argomenti per l'evento di cambiamento di avanzamento dell'operazione di ottimizzazione.

## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getNodeIndex()](#getNodeIndex--) | Restituisce l'indice del nodo della rete di ricerca. |
|
|  | [getServiceIndex()](#getServiceIndex--) | Restituisce l'indice del servizio del nodo della rete di ricerca. |
|
|  | [getProcessedSegments()](#getProcessedSegments--) | Restituisce il numero di segmenti elaborati. |
|
|  | [getTotalSegments()](#getTotalSegments--) | Restituisce il numero totale di segmenti da elaborare. |
|
|  | [getProgressPercentage()](#getProgressPercentage--) | Ottiene la percentuale di avanzamento. |
|
### getNodeIndex() {#getNodeIndex--}
```
public final int getNodeIndex()
```


Restituisce l'indice del nodo della rete di ricerca.


**Returns:**
int - L'indice del nodo della rete di ricerca.

### getServiceIndex() {#getServiceIndex--}
```
public final int getServiceIndex()
```


Restituisce l'indice del servizio del nodo della rete di ricerca.


**Returns:**
int - L'indice del servizio del nodo della rete di ricerca.

### getProcessedSegments() {#getProcessedSegments--}
```
public final int getProcessedSegments()
```


Restituisce il numero di segmenti elaborati.


**Returns:**
int - Il numero di segmenti elaborati.

### getTotalSegments() {#getTotalSegments--}
```
public final int getTotalSegments()
```


Restituisce il numero totale di segmenti da elaborare.


**Returns:**
int - Il numero totale di segmenti da elaborare.

### getProgressPercentage() {#getProgressPercentage--}
```
public final double getProgressPercentage()
```


Ottiene la percentuale di avanzamento.


**Returns:**
double - La percentuale di avanzamento.

