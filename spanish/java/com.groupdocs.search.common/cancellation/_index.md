---
title: "Cancellation"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa un objeto para solicitar la cancelación de una operación."
type: docs
weight: 11
url: /es/java/com.groupdocs.search.common/cancellation/
---
**Inheritance:**
java.lang.Object
```
public class Cancellation
```

Representa un objeto para solicitar la cancelación de una operación.


**Learn more**

* [Indexing options](../https://docs.groupdocs.com/display/searchjava/Indexing+options)
* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [Cancellation()](#Cancellation--) | Inicializa una nueva instancia de la |
Cancellation
clase.
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [isCancelled()](#isCancelled--) | Obtiene un valor que indica que se ha solicitado la cancelación. |
|
|  | [cancel()](#cancel--) | Realiza una solicitud de cancelación. |
|
|  | [cancelAfter(int milliseconds)](#cancelAfter-int-) | Realiza una solicitud de cancelación después de la expiración del número especificado de milisegundos. |
|
### Cancellation() {#Cancellation--}
```
public Cancellation()
```


Inicializa una nueva instancia de la
Cancellation
clase.


### isCancelled() {#isCancelled--}
```
public final boolean isCancelled()
```


Obtiene un valor que indica que se ha solicitado la cancelación.


**Returns:**
boolean - Un valor que indica que se ha solicitado la cancelación.

### cancel() {#cancel--}
```
public final void cancel()
```


Realiza una solicitud de cancelación.


### cancelAfter(int milliseconds) {#cancelAfter-int-}
```
public final void cancelAfter(int milliseconds)
```


Realiza una solicitud de cancelación después de la expiración del número especificado de milisegundos.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | milisegundos | int | El número de milisegundos después del cual se cancelará una operación. |
|

