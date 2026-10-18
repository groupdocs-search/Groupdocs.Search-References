---
title: "OperationFinishedEventArgs"
second_title: "GroupDocs.Search for Java API Referansı"
description: "İndeksleme işlemi tamamlandığında olayın argümanlarını temsil eder."
type: docs
weight: 17
url: /tr/java/com.groupdocs.search.events/operationfinishedeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class OperationFinishedEventArgs extends BaseIndexEventArgs
```

İndeksleme işlemi tamamlandığında olayın argümanlarını temsil eder.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getMessage()](#getMessage--) | Mesajı alır. |
|
|  | [getOperationType()](#getOperationType--) | İşlem türünü alır. |
|
### getMessage() {#getMessage--}
```
public final String getMessage()
```


Mesajı alır.


**Returns:**
java.lang.String - Mesaj.

### getOperationType() {#getOperationType--}
```
public final OperationType getOperationType()
```


İşlem türünü alır.


**Returns:**
[OperationType](../../com.groupdocs.search.events/operationtype) - The operation type.

