---
title: "OptimizationProgressEventArgs"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa los argumentos del evento de actualización del progreso de la operación de indexado."
type: docs
weight: 19
url: /es/java/com.groupdocs.search.events/optimizationprogresseventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class OptimizationProgressEventArgs extends BaseIndexEventArgs
```

Representa los argumentos del evento de actualización del progreso de la operación de indexado.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Métodos

| Método | Descripción |
| --- | --- |
|  | [getTotalSegments()](#getTotalSegments--) | Obtiene el número total de segmentos para procesar. |
|
|  | [getProcessedSegments()](#getProcessedSegments--) | Obtiene el número de segmentos procesados. |
|
|  | [getProgressPercentage()](#getProgressPercentage--) | Obtiene el porcentaje del progreso. |
|
### getTotalSegments() {#getTotalSegments--}
```
public final int getTotalSegments()
```


Obtiene el número total de segmentos para procesar.


**Returns:**
int - El número total de segmentos para procesar.

### getProcessedSegments() {#getProcessedSegments--}
```
public final int getProcessedSegments()
```


Obtiene el número de segmentos procesados.


**Returns:**
int - El número de segmentos procesados.

### getProgressPercentage() {#getProgressPercentage--}
```
public final double getProgressPercentage()
```


Obtiene el porcentaje del progreso.


**Returns:**
double - El porcentaje del progreso.

