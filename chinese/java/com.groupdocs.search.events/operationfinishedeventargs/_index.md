---
title: "OperationFinishedEventArgs"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示索引操作完成事件的参数。"
type: docs
weight: 17
url: /zh/java/com.groupdocs.search.events/operationfinishedeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class OperationFinishedEventArgs extends BaseIndexEventArgs
```

表示索引操作完成事件的参数。


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getMessage()](#getMessage--) | 获取消息。 |
|
|  | [getOperationType()](#getOperationType--) | 获取操作类型。 |
|
### getMessage() {#getMessage--}
```
public final String getMessage()
```


获取消息。


**Returns:**
java.lang.String - 消息。

### getOperationType() {#getOperationType--}
```
public final OperationType getOperationType()
```


获取操作类型。


**Returns:**
[OperationType](../../com.groupdocs.search.events/operationtype) - The operation type.

