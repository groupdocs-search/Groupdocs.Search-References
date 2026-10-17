---
title: "ErrorOccurredEventArgs"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示搜索网络中某个节点发生错误事件的参数。"
type: docs
weight: 13
url: /zh/java/com.groupdocs.search.scaling.events/erroroccurredeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class ErrorOccurredEventArgs extends EventArgs
```

表示搜索网络中某个节点发生错误事件的参数。

## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getNodeIndex()](#getNodeIndex--) | 获取搜索网络节点的索引。 |
|
|  | [getServiceIndex()](#getServiceIndex--) | 获取搜索网络节点服务的索引。 |
|
|  | [getMessage()](#getMessage--) | 获取错误信息。 |
|
### getNodeIndex() {#getNodeIndex--}
```
public final int getNodeIndex()
```


获取搜索网络节点的索引。


**Returns:**
int - 搜索网络节点的索引。

### getServiceIndex() {#getServiceIndex--}
```
public final int getServiceIndex()
```


获取搜索网络节点服务的索引。


**Returns:**
int - 搜索网络节点服务的索引。

### getMessage() {#getMessage--}
```
public final String getMessage()
```


获取错误信息。


**Returns:**
java.lang.String - 错误信息。

