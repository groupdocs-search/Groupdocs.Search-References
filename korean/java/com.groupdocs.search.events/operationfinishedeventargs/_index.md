---
title: "OperationFinishedEventArgs"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "인덱싱 작업이 완료되는 이벤트에 대한 인수를 나타냅니다."
type: docs
weight: 17
url: /ko/java/com.groupdocs.search.events/operationfinishedeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class OperationFinishedEventArgs extends BaseIndexEventArgs
```

인덱싱 작업이 완료되는 이벤트에 대한 인수를 나타냅니다.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getMessage()](#getMessage--) | 메시지를 가져옵니다. |
|
|  | [getOperationType()](#getOperationType--) | 작업 유형을 가져옵니다. |
|
### getMessage() {#getMessage--}
```
public final String getMessage()
```


메시지를 가져옵니다.


**Returns:**
java.lang.String - 메시지.

### getOperationType() {#getOperationType--}
```
public final OperationType getOperationType()
```


작업 유형을 가져옵니다.


**Returns:**
[OperationType](../../com.groupdocs.search.events/operationtype) - The operation type.

