---
title: "OperationProgressEventArgs"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta gli argomenti per l'evento di aggiornamento del progresso dell'operazione di indicizzazione."
type: docs
weight: 18
url: /it/java/com.groupdocs.search.events/operationprogresseventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class OperationProgressEventArgs extends BaseIndexEventArgs
```

Rappresenta gli argomenti per l'evento di aggiornamento del progresso dell'operazione di indicizzazione.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getTotalDocuments()](#getTotalDocuments--) | Ottiene il numero totale di documenti da elaborare. |
|
|  | [getProcessedDocuments()](#getProcessedDocuments--) | Restituisce il numero di documenti elaborati con successo. |
|
|  | [getSkippedDocuments()](#getSkippedDocuments--) | Restituisce il numero di documenti ignorati. |
|
|  | [getProgressPercentage()](#getProgressPercentage--) | Ottiene la percentuale di avanzamento. |
|
|  | [getLastDocumentKey()](#getLastDocumentKey--) | Restituisce la chiave dell'ultimo documento elaborato. |
|
|  | [getLastDocumentPath()](#getLastDocumentPath--) | Restituisce il percorso dell'ultimo documento elaborato. |
|
|  | [getLastDocumentStatus()](#getLastDocumentStatus--) | Restituisce lo stato dell'ultimo documento elaborato. |
|
### getTotalDocuments() {#getTotalDocuments--}
```
public final int getTotalDocuments()
```


Ottiene il numero totale di documenti da elaborare.


**Returns:**
int - Il numero totale di documenti da elaborare.

### getProcessedDocuments() {#getProcessedDocuments--}
```
public final int getProcessedDocuments()
```


Restituisce il numero di documenti elaborati con successo.


**Returns:**
int - Il numero di documenti elaborati con successo.

### getSkippedDocuments() {#getSkippedDocuments--}
```
public final int getSkippedDocuments()
```


Restituisce il numero di documenti ignorati.


**Returns:**
int - Il numero di documenti ignorati.

### getProgressPercentage() {#getProgressPercentage--}
```
public final double getProgressPercentage()
```


Ottiene la percentuale di avanzamento.


**Returns:**
double - La percentuale di avanzamento.

### getLastDocumentKey() {#getLastDocumentKey--}
```
public final String getLastDocumentKey()
```


Restituisce la chiave dell'ultimo documento elaborato.


**Returns:**
java.lang.String - La chiave dell'ultimo documento elaborato.

### getLastDocumentPath() {#getLastDocumentPath--}
```
public final String getLastDocumentPath()
```


Restituisce il percorso dell'ultimo documento elaborato.


**Returns:**
java.lang.String - Il percorso dell'ultimo documento elaborato.

### getLastDocumentStatus() {#getLastDocumentStatus--}
```
public final DocumentStatus getLastDocumentStatus()
```


Restituisce lo stato dell'ultimo documento elaborato.


**Returns:**
[DocumentStatus](../../com.groupdocs.search.common/documentstatus) - The last processed document status.

