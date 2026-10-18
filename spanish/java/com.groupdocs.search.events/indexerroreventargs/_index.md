---
title: "IndexErrorEventArgs"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa los argumentos del evento de error de índice."
type: docs
weight: 16
url: /es/java/com.groupdocs.search.events/indexerroreventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class IndexErrorEventArgs extends BaseIndexEventArgs
```

Representa los argumentos del evento de error de índice.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Métodos

| Método | Descripción |
| --- | --- |
|  | [getMessage()](#getMessage--) | Obtiene el mensaje de error. |
|
|  | [isCritical()](#isCritical--) | Obtiene una bandera que indica que el error ocurrido es crítico y que el índice debe reiniciarse. |
|
### getMessage() {#getMessage--}
```
public final String getMessage()
```


Obtiene el mensaje de error.


**Returns:**
java.lang.String - El mensaje de error.

### isCritical() {#isCritical--}
```
public final boolean isCritical()
```


Obtiene una bandera que indica que el error ocurrido es crítico y que el índice debe reiniciarse.


**Returns:**
boolean - La bandera que indica que el error ocurrido es crítico y que el índice debe reiniciarse.

