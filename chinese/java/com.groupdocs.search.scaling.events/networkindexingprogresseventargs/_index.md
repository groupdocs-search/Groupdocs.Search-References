---
title: "NetworkIndexingProgressEventArgs"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示索引操作进度更改事件的参数。"
type: docs
weight: 14
url: /zh/java/com.groupdocs.search.scaling.events/networkindexingprogresseventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class NetworkIndexingProgressEventArgs extends EventArgs
```

表示索引操作进度更改事件的参数。

## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getNodeIndex()](#getNodeIndex--) | 获取搜索网络节点的索引。 |
|
|  | [getServiceIndex()](#getServiceIndex--) | 获取搜索网络节点服务的索引。 |
|
|  | [getProcessedDocuments()](#getProcessedDocuments--) | 获取已处理文档的数量。 |
|
|  | [getTotalDocuments()](#getTotalDocuments--) | 获取待处理文档的总数。 |
|
|  | [getProgressPercentage()](#getProgressPercentage--) | 获取进度的百分比。 |
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

### getProcessedDocuments() {#getProcessedDocuments--}
```
public final int getProcessedDocuments()
```


获取已处理文档的数量。


**Returns:**
int - 已处理文档的数量。

### getTotalDocuments() {#getTotalDocuments--}
```
public final int getTotalDocuments()
```


获取待处理文档的总数。


**Returns:**
int - 待处理文档的总数。

### getProgressPercentage() {#getProgressPercentage--}
```
public final double getProgressPercentage()
```


获取进度的百分比。


**Returns:**
double - 进度的百分比。

