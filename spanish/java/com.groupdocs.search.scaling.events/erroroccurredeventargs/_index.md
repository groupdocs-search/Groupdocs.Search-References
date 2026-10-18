---
title: "ErrorOccurredEventArgs"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa los argumentos del evento de que ocurre un error en uno de los nodos de la red de búsqueda."
type: docs
weight: 13
url: /es/java/com.groupdocs.search.scaling.events/erroroccurredeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class ErrorOccurredEventArgs extends EventArgs
```

Representa los argumentos del evento de que ocurre un error en uno de los nodos de la red de búsqueda.

## Métodos

| Método | Descripción |
| --- | --- |
|  | [getNodeIndex()](#getNodeIndex--) | Obtiene el índice del nodo de la red de búsqueda. |
|
|  | [getServiceIndex()](#getServiceIndex--) | Obtiene el índice del servicio del nodo de la red de búsqueda. |
|
|  | [getMessage()](#getMessage--) | Obtiene el mensaje de error. |
|
### getNodeIndex() {#getNodeIndex--}
```
public final int getNodeIndex()
```


Obtiene el índice del nodo de la red de búsqueda.


**Returns:**
int - El índice del nodo de la red de búsqueda.

### getServiceIndex() {#getServiceIndex--}
```
public final int getServiceIndex()
```


Obtiene el índice del servicio del nodo de la red de búsqueda.


**Returns:**
int - El índice del servicio del nodo de la red de búsqueda.

### getMessage() {#getMessage--}
```
public final String getMessage()
```


Obtiene el mensaje de error.


**Returns:**
java.lang.String - El mensaje de error.

