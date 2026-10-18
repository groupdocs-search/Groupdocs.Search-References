---
title: "OperationFinishedEventArgs"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar argument för händelsen när indexeringsoperationen är slutförd."
type: docs
weight: 17
url: /sv/java/com.groupdocs.search.events/operationfinishedeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class OperationFinishedEventArgs extends BaseIndexEventArgs
```

Representerar argument för händelsen när indexeringsoperationen är slutförd.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getMessage()](#getMessage--) | Hämtar meddelandet. |
|
|  | [getOperationType()](#getOperationType--) | Hämtar operationstypen. |
|
### getMessage() {#getMessage--}
```
public final String getMessage()
```


Hämtar meddelandet.


**Returns:**
java.lang.String - Meddelandet.

### getOperationType() {#getOperationType--}
```
public final OperationType getOperationType()
```


Hämtar operationstypen.


**Returns:**
[OperationType](../../com.groupdocs.search.events/operationtype) - The operation type.

