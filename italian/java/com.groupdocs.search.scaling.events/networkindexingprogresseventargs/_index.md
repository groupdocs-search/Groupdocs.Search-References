---
title: "NetworkIndexingProgressEventArgs"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta gli argomenti per l'evento di cambiamento di avanzamento dell'operazione di indicizzazione."
type: docs
weight: 14
url: /it/java/com.groupdocs.search.scaling.events/networkindexingprogresseventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class NetworkIndexingProgressEventArgs extends EventArgs
```

Rappresenta gli argomenti per l'evento di cambiamento di avanzamento dell'operazione di indicizzazione.

## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getNodeIndex()](#getNodeIndex--) | Restituisce l'indice del nodo della rete di ricerca. |
|
|  | [getServiceIndex()](#getServiceIndex--) | Restituisce l'indice del servizio del nodo della rete di ricerca. |
|
|  | [getProcessedDocuments()](#getProcessedDocuments--) | Ottiene il numero di documenti elaborati. |
|
|  | [getTotalDocuments()](#getTotalDocuments--) | Ottiene il numero totale di documenti da elaborare. |
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

### getProcessedDocuments() {#getProcessedDocuments--}
```
public final int getProcessedDocuments()
```


Ottiene il numero di documenti elaborati.


**Returns:**
int - Il numero di documenti elaborati.

### getTotalDocuments() {#getTotalDocuments--}
```
public final int getTotalDocuments()
```


Ottiene il numero totale di documenti da elaborare.


**Returns:**
int - Il numero totale di documenti da elaborare.

### getProgressPercentage() {#getProgressPercentage--}
```
public final double getProgressPercentage()
```


Ottiene la percentuale di avanzamento.


**Returns:**
double - La percentuale di avanzamento.

