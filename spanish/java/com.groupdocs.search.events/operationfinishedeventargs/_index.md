---
title: "OperationFinishedEventArgs"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa los argumentos del evento de finalización de la operación de indexado."
type: docs
weight: 17
url: /es/java/com.groupdocs.search.events/operationfinishedeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class OperationFinishedEventArgs extends BaseIndexEventArgs
```

Representa los argumentos del evento de finalización de la operación de indexado.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Métodos

| Método | Descripción |
| --- | --- |
|  | [getMessage()](#getMessage--) | Obtiene el mensaje. |
|
|  | [getOperationType()](#getOperationType--) | Obtiene el tipo de operación. |
|
### getMessage() {#getMessage--}
```
public final String getMessage()
```


Obtiene el mensaje.


**Returns:**
java.lang.String - El mensaje.

### getOperationType() {#getOperationType--}
```
public final OperationType getOperationType()
```


Obtiene el tipo de operación.


**Returns:**
[OperationType](../../com.groupdocs.search.events/operationtype) - The operation type.

