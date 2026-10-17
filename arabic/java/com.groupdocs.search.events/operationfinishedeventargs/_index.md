---
title: "OperationFinishedEventArgs"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل المعلمات لحدث انتهاء عملية الفهرسة."
type: docs
weight: 17
url: /ar/java/com.groupdocs.search.events/operationfinishedeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class OperationFinishedEventArgs extends BaseIndexEventArgs
```

يمثل المعلمات لحدث انتهاء عملية الفهرسة.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getMessage()](#getMessage--) | يحصل على الرسالة. |
|
|  | [getOperationType()](#getOperationType--) | يحصل على نوع العملية. |
|
### getMessage() {#getMessage--}
```
public final String getMessage()
```


يحصل على الرسالة.


**Returns:**
java.lang.String - الرسالة.

### getOperationType() {#getOperationType--}
```
public final OperationType getOperationType()
```


يحصل على نوع العملية.


**Returns:**
[OperationType](../../com.groupdocs.search.events/operationtype) - The operation type.

