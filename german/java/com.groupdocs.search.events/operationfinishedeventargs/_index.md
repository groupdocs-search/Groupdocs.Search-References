---
title: "OperationFinishedEventArgs"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt Argumente für das Ereignis dar, wenn der Indexierungsvorgang abgeschlossen ist."
type: docs
weight: 17
url: /de/java/com.groupdocs.search.events/operationfinishedeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class OperationFinishedEventArgs extends BaseIndexEventArgs
```

Stellt Argumente für das Ereignis dar, wenn der Indexierungsvorgang abgeschlossen ist.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getMessage()](#getMessage--) | Gibt die Nachricht zurück. |
|
|  | [getOperationType()](#getOperationType--) | Gibt den Operationstyp zurück. |
|
### getMessage() {#getMessage--}
```
public final String getMessage()
```


Gibt die Nachricht zurück.


**Returns:**
java.lang.String - Die Nachricht.

### getOperationType() {#getOperationType--}
```
public final OperationType getOperationType()
```


Gibt den Operationstyp zurück.


**Returns:**
[OperationType](../../com.groupdocs.search.events/operationtype) - The operation type.

