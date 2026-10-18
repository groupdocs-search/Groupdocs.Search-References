---
title: "NetworkOptimizationProgressEventArgs"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa los argumentos del evento de cambio de progreso de la operación de optimización."
type: docs
weight: 15
url: /es/java/com.groupdocs.search.scaling.events/networkoptimizationprogresseventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class NetworkOptimizationProgressEventArgs extends EventArgs
```

Representa los argumentos del evento de cambio de progreso de la operación de optimización.

## Métodos

| Método | Descripción |
| --- | --- |
|  | [getNodeIndex()](#getNodeIndex--) | Obtiene el índice del nodo de la red de búsqueda. |
|
|  | [getServiceIndex()](#getServiceIndex--) | Obtiene el índice del servicio del nodo de la red de búsqueda. |
|
|  | [getProcessedSegments()](#getProcessedSegments--) | Obtiene el número de segmentos procesados. |
|
|  | [getTotalSegments()](#getTotalSegments--) | Obtiene el número total de segmentos para procesar. |
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

### getProcessedSegments() {#getProcessedSegments--}
```
public final int getProcessedSegments()
```


Obtiene el número de segmentos procesados.


**Returns:**
int - El número de segmentos procesados.

### getTotalSegments() {#getTotalSegments--}
```
public final int getTotalSegments()
```


Obtiene el número total de segmentos para procesar.


**Returns:**
int - El número total de segmentos para procesar.

### getProgressPercentage() {#getProgressPercentage--}
```
public final double getProgressPercentage()
```


Obtiene el porcentaje del progreso.


**Returns:**
double - El porcentaje del progreso.

