---
title: "DeleteResult"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa el resultado de la operación para eliminar archivos o carpetas indexados de un índice."
type: docs
weight: 10
url: /es/java/com.groupdocs.search.results/deleteresult/
---
**Inheritance:**
java.lang.Object
```
public class DeleteResult
```

Representa el resultado de la operación para eliminar archivos o carpetas indexados de un índice.


**Learn more**

* [Delete indexed paths](../https://docs.groupdocs.com/display/searchjava/Delete+indexed+paths)

## Métodos

| Método | Descripción |
| --- | --- |
|  | [getItemResults()](#getItemResults--) | Devuelve los resultados de eliminar cada ruta. |
|
|  | [getTotalCount()](#getTotalCount--) | Devuelve el número total de rutas a eliminar. |
|
|  | [getSuccessCount()](#getSuccessCount--) | Devuelve el número de rutas eliminadas con éxito. |
|
|  | [getFailedCount()](#getFailedCount--) | Devuelve el número de rutas no eliminadas debido a errores. |
|
|  | [getErrors()](#getErrors--) | Devuelve descripciones de los errores de eliminación. |
|
### getItemResults() {#getItemResults--}
```
public final PathDeleteResult[] getItemResults()
```


Devuelve los resultados de eliminar cada ruta.


**Returns:**
com.groupdocs.search.results.PathDeleteResult[] - Los resultados de eliminar cada ruta.

### getTotalCount() {#getTotalCount--}
```
public final int getTotalCount()
```


Devuelve el número total de rutas a eliminar.


**Returns:**
int - El número total de rutas a eliminar.

### getSuccessCount() {#getSuccessCount--}
```
public final int getSuccessCount()
```


Devuelve el número de rutas eliminadas con éxito.


**Returns:**
int - El número de rutas eliminadas con éxito.

### getFailedCount() {#getFailedCount--}
```
public final int getFailedCount()
```


Devuelve el número de rutas no eliminadas debido a errores.


**Returns:**
int - El número de rutas no eliminadas debido a errores.

### getErrors() {#getErrors--}
```
public final String[] getErrors()
```


Devuelve descripciones de los errores de eliminación.


**Returns:**
java.lang.String[] - Descripciones de errores de eliminación.

