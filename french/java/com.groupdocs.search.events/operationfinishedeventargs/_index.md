---
title: "OperationFinishedEventArgs"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente les arguments de l'événement de fin de l'opération d'indexation."
type: docs
weight: 17
url: /fr/java/com.groupdocs.search.events/operationfinishedeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class OperationFinishedEventArgs extends BaseIndexEventArgs
```

Représente les arguments de l'événement de fin de l'opération d'indexation.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getMessage()](#getMessage--) | Obtient le message. |
|
|  | [getOperationType()](#getOperationType--) | Obtient le type d'opération. |
|
### getMessage() {#getMessage--}
```
public final String getMessage()
```


Obtient le message.


**Returns:**
java.lang.String - Le message.

### getOperationType() {#getOperationType--}
```
public final OperationType getOperationType()
```


Obtient le type d'opération.


**Returns:**
[OperationType](../../com.groupdocs.search.events/operationtype) - The operation type.

