---
title: "PathDeleteResult"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa el resultado de la operación de eliminar un archivo o carpeta indexado del índice."
type: docs
weight: 18
url: /es/java/com.groupdocs.search.results/pathdeleteresult/
---
**Inheritance:**
java.lang.Object
```
public class PathDeleteResult
```

Representa el resultado de la operación de eliminar un archivo o carpeta indexado del índice.


**Learn more**

* [Delete indexed paths](../https://docs.groupdocs.com/display/searchjava/Delete+indexed+paths)

## Métodos

| Método | Descripción |
| --- | --- |
|  | [isSuccess()](#isSuccess--) | Devuelve el indicador de éxito de la operación de eliminación. |
|
|  | [getError()](#getError--) | Devuelve una descripción del error de eliminación. |
|
|  | [getPath()](#getPath--) | Devuelve la ruta al archivo o carpeta a eliminar. |
|
### isSuccess() {#isSuccess--}
```
public final boolean isSuccess()
```


Devuelve el indicador de éxito de la operación de eliminación.


**Returns:**
boolean -  true  si la operación de eliminación fue exitosa; de lo contrario, devuelve  false .

### getError() {#getError--}
```
public final String getError()
```


Devuelve una descripción del error de eliminación.


**Returns:**
java.lang.String - Una descripción del error de eliminación.

### getPath() {#getPath--}
```
public final String getPath()
```


Devuelve la ruta al archivo o carpeta a eliminar.


**Returns:**
java.lang.String - La ruta al archivo o carpeta a eliminar.

