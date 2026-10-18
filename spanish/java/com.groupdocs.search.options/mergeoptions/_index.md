---
title: "MergeOptions"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Proporciona opciones para la operación de fusión."
type: docs
weight: 28
url: /es/java/com.groupdocs.search.options/mergeoptions/
---
**Inheritance:**
java.lang.Object
```
public class MergeOptions
```

Proporciona opciones para la operación de fusión.


**Learn more**

* [Merge indexes](../https://docs.groupdocs.com/display/searchjava/Merge+indexes)
* [Optimize index](../https://docs.groupdocs.com/display/searchjava/Optimize+index)

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [MergeOptions()](#MergeOptions--) | Inicializa una nueva instancia de la  MergeOptions  clase. |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [isAsync()](#isAsync--) | Obtiene la bandera de ejecución asíncrona de la operación. |
|
|  | [setAsync(boolean value)](#setAsync-boolean-) | Establece la bandera de ejecución asíncrona de la operación. |
|
|  | [getCancellation()](#getCancellation--) | Obtiene el objeto de cancelación de la operación. |
|
|  | [setCancellation(Cancellation value)](#setCancellation-com.groupdocs.search.common.Cancellation-) | Establece el objeto de cancelación de la operación. |
|
### MergeOptions() {#MergeOptions--}
```
public MergeOptions()
```


Inicializa una nueva instancia de la  MergeOptions  clase.


### isAsync() {#isAsync--}
```
public final boolean isAsync()
```


Obtiene la bandera de ejecución asíncrona de la operación. El valor predeterminado es  false .


**Returns:**
boolean - La bandera de ejecución asíncrona de la operación.

### setAsync(boolean value) {#setAsync-boolean-}
```
public final void setAsync(boolean value)
```


Establece la bandera de ejecución asíncrona de la operación. El valor predeterminado es  false .


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | boolean | La bandera de ejecución asíncrona de la operación. |
|

### getCancellation() {#getCancellation--}
```
public final Cancellation getCancellation()
```


Obtiene el objeto de cancelación de la operación. El valor predeterminado es  null .


**Returns:**
[Cancellation](../../com.groupdocs.search.common/cancellation) - The operation cancellation object.

### setCancellation(Cancellation value) {#setCancellation-com.groupdocs.search.common.Cancellation-}
```
public final void setCancellation(Cancellation value)
```


Establece el objeto de cancelación de la operación. El valor predeterminado es  null .


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | value | [Cancellation](../../com.groupdocs.search.common/cancellation) | El objeto de cancelación de la operación. |
|

