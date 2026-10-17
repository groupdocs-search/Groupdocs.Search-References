---
title: "OptimizationProgressEventArgs"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示索引操作进度更新事件的参数。"
type: docs
weight: 19
url: /zh/java/com.groupdocs.search.events/optimizationprogresseventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class OptimizationProgressEventArgs extends BaseIndexEventArgs
```

表示索引操作进度更新事件的参数。


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getTotalSegments()](#getTotalSegments--) | 获取待处理段的总数。 |
|
|  | [getProcessedSegments()](#getProcessedSegments--) | 获取已处理段的数量。 |
|
|  | [getProgressPercentage()](#getProgressPercentage--) | 获取进度的百分比。 |
|
### getTotalSegments() {#getTotalSegments--}
```
public final int getTotalSegments()
```


获取待处理段的总数。


**Returns:**
int - 用于处理的段总数。

### getProcessedSegments() {#getProcessedSegments--}
```
public final int getProcessedSegments()
```


获取已处理段的数量。


**Returns:**
int - 已处理段的数量。

### getProgressPercentage() {#getProgressPercentage--}
```
public final double getProgressPercentage()
```


获取进度的百分比。


**Returns:**
double - 进度的百分比。

