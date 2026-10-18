---
title: "BaseIndexEventArgs"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa la clase base de los argumentos de eventos."
type: docs
weight: 10
url: /es/java/com.groupdocs.search.events/baseindexeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class BaseIndexEventArgs extends EventArgs
```

Representa la clase base de los argumentos de eventos.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Métodos

| Método | Descripción |
| --- | --- |
|  | [getTime()](#getTime--) | Obtiene la hora de un evento. |
|
|  | [getIndexId()](#getIndexId--) | Obtiene el ID del índice. |
|
|  | [getIndexFolder()](#getIndexFolder--) | Obtiene la carpeta del índice. |
|
|  | [getStatus()](#getStatus--) | Obtiene el estado del índice. |
|
### getTime() {#getTime--}
```
public final Date getTime()
```


Obtiene la hora de un evento.


**Returns:**
java.util.Date - La hora de un evento.

### getIndexId() {#getIndexId--}
```
public final UUID getIndexId()
```


Obtiene el ID del índice.


**Returns:**
java.util.UUID - El ID del índice.

### getIndexFolder() {#getIndexFolder--}
```
public final String getIndexFolder()
```


Obtiene la carpeta del índice.


**Returns:**
java.lang.String - La carpeta del índice.

### getStatus() {#getStatus--}
```
public final IndexStatus getStatus()
```


Obtiene el estado del índice.


**Returns:**
[IndexStatus](../../com.groupdocs.search.common/indexstatus) - The index status.

