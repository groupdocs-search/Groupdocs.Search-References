---
title: "NetworkOptimizationProgressEventArgs"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示优化操作进度更改事件的参数。"
type: docs
weight: 15
url: /zh/java/com.groupdocs.search.scaling.events/networkoptimizationprogresseventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class NetworkOptimizationProgressEventArgs extends EventArgs
```

表示优化操作进度更改事件的参数。

## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getNodeIndex()](#getNodeIndex--) | 获取搜索网络节点的索引。 |
|
|  | [getServiceIndex()](#getServiceIndex--) | 获取搜索网络节点服务的索引。 |
|
|  | [getProcessedSegments()](#getProcessedSegments--) | 获取已处理段的数量。 |
|
|  | [getTotalSegments()](#getTotalSegments--) | 获取待处理段的总数。 |
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

### getProcessedSegments() {#getProcessedSegments--}
```
public final int getProcessedSegments()
```


获取已处理段的数量。


**Returns:**
int - 已处理段的数量。

### getTotalSegments() {#getTotalSegments--}
```
public final int getTotalSegments()
```


获取待处理段的总数。


**Returns:**
int - 用于处理的段总数。

### getProgressPercentage() {#getProgressPercentage--}
```
public final double getProgressPercentage()
```


获取进度的百分比。


**Returns:**
double - 进度的百分比。

