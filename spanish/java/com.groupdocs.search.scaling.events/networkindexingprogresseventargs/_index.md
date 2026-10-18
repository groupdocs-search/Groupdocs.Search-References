---
title: "NetworkIndexingProgressEventArgs"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa los argumentos del evento de cambio de progreso de la operación de indexado."
type: docs
weight: 14
url: /es/java/com.groupdocs.search.scaling.events/networkindexingprogresseventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class NetworkIndexingProgressEventArgs extends EventArgs
```

Representa los argumentos del evento de cambio de progreso de la operación de indexado.

## Métodos

| Método | Descripción |
| --- | --- |
|  | [getNodeIndex()](#getNodeIndex--) | Obtiene el índice del nodo de la red de búsqueda. |
|
|  | [getServiceIndex()](#getServiceIndex--) | Obtiene el índice del servicio del nodo de la red de búsqueda. |
|
|  | [getProcessedDocuments()](#getProcessedDocuments--) | Obtiene el número de documentos procesados. |
|
|  | [getTotalDocuments()](#getTotalDocuments--) | Obtiene el número total de documentos para procesar. |
|
|  | [getProgressPercentage()](#getProgressPercentage--) | Obtiene el porcentaje del progreso. |
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

### getProcessedDocuments() {#getProcessedDocuments--}
```
public final int getProcessedDocuments()
```


Obtiene el número de documentos procesados.


**Returns:**
int - El número de documentos procesados.

### getTotalDocuments() {#getTotalDocuments--}
```
public final int getTotalDocuments()
```


Obtiene el número total de documentos para procesar.


**Returns:**
int - El número total de documentos para procesar.

### getProgressPercentage() {#getProgressPercentage--}
```
public final double getProgressPercentage()
```


Obtiene el porcentaje del progreso.


**Returns:**
double - El porcentaje del progreso.

