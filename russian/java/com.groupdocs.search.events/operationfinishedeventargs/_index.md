---
title: "OperationFinishedEventArgs"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет аргументы события завершения операции индексации."
type: docs
weight: 17
url: /ru/java/com.groupdocs.search.events/operationfinishedeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class OperationFinishedEventArgs extends BaseIndexEventArgs
```

Представляет аргументы события завершения операции индексации.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Методы

| Метод | Описание |
| --- | --- |
|  | [getMessage()](#getMessage--) | Возвращает сообщение. |
|
|  | [getOperationType()](#getOperationType--) | Возвращает тип операции. |
|
### getMessage() {#getMessage--}
```
public final String getMessage()
```


Возвращает сообщение.


**Returns:**
java.lang.String - Сообщение.

### getOperationType() {#getOperationType--}
```
public final OperationType getOperationType()
```


Возвращает тип операции.


**Returns:**
[OperationType](../../com.groupdocs.search.events/operationtype) - The operation type.

