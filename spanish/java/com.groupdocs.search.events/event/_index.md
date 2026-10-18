---
title: "Evento"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Esta clase está destinada a ser heredada al suscribirse a eventos."
type: docs
weight: 11
url: /es/java/com.groupdocs.search.events/event/
---
**Inheritance:**
java.lang.Object
```
public abstract class Event<T>
```

Esta clase está destinada a ser heredada al suscribirse a eventos.

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [Event()](#Event--) | Inicializa una nueva instancia de la clase  Event  . |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [add(T delegate)](#add-T-) | Agrega un escuchador para el evento. |
|
|  | [remove(T delegate)](#remove-T-) | Elimina un escuchador para el evento. |
|
|  | [isEmpty()](#isEmpty--) | Comprueba la presencia de al menos un escuchador. |
|
### Event() {#Event--}
```
public Event()
```


Inicializa una nueva instancia de la clase  Event  .


### add(T delegate) {#add-T-}
```
public final synchronized void add(T delegate)
```


Agrega un escuchador para el evento.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | delegado | T | Un escuchador para el evento a agregar. |
|

### remove(T delegate) {#remove-T-}
```
public final synchronized void remove(T delegate)
```


Elimina un escuchador para el evento.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | delegado | T | Un escuchador para el evento a eliminar. |
|

### isEmpty() {#isEmpty--}
```
public synchronized boolean isEmpty()
```


Comprueba la presencia de al menos un escuchador.


**Returns:**
boolean - Un valor que indica que al menos un escuchador se ha agregado para el evento.

