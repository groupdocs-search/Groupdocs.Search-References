---
title: "ErrorOccurredEventArgs"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta gli argomenti per l'evento di errore che si verifica in uno dei nodi della rete di ricerca."
type: docs
weight: 13
url: /it/java/com.groupdocs.search.scaling.events/erroroccurredeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class ErrorOccurredEventArgs extends EventArgs
```

Rappresenta gli argomenti per l'evento di errore che si verifica in uno dei nodi della rete di ricerca.

## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getNodeIndex()](#getNodeIndex--) | Restituisce l'indice del nodo della rete di ricerca. |
|
|  | [getServiceIndex()](#getServiceIndex--) | Restituisce l'indice del servizio del nodo della rete di ricerca. |
|
|  | [getMessage()](#getMessage--) | Restituisce il messaggio di errore. |
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

### getMessage() {#getMessage--}
```
public final String getMessage()
```


Restituisce il messaggio di errore.


**Returns:**
java.lang.String - Il messaggio di errore.

