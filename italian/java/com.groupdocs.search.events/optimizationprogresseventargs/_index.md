---
title: "OptimizationProgressEventArgs"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta gli argomenti per l'evento di aggiornamento del progresso dell'operazione di indicizzazione."
type: docs
weight: 19
url: /it/java/com.groupdocs.search.events/optimizationprogresseventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class OptimizationProgressEventArgs extends BaseIndexEventArgs
```

Rappresenta gli argomenti per l'evento di aggiornamento del progresso dell'operazione di indicizzazione.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getTotalSegments()](#getTotalSegments--) | Restituisce il numero totale di segmenti da elaborare. |
|
|  | [getProcessedSegments()](#getProcessedSegments--) | Restituisce il numero di segmenti elaborati. |
|
|  | [getProgressPercentage()](#getProgressPercentage--) | Ottiene la percentuale di avanzamento. |
|
### getTotalSegments() {#getTotalSegments--}
```
public final int getTotalSegments()
```


Restituisce il numero totale di segmenti da elaborare.


**Returns:**
int - Il numero totale di segmenti da elaborare.

### getProcessedSegments() {#getProcessedSegments--}
```
public final int getProcessedSegments()
```


Restituisce il numero di segmenti elaborati.


**Returns:**
int - Il numero di segmenti elaborati.

### getProgressPercentage() {#getProgressPercentage--}
```
public final double getProgressPercentage()
```


Ottiene la percentuale di avanzamento.


**Returns:**
double - La percentuale di avanzamento.

