---
title: "OperationProgressEventArgs"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示索引操作进度更新事件的参数。"
type: docs
weight: 18
url: /zh/java/com.groupdocs.search.events/operationprogresseventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class OperationProgressEventArgs extends BaseIndexEventArgs
```

表示索引操作进度更新事件的参数。


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getTotalDocuments()](#getTotalDocuments--) | 获取待处理文档的总数。 |
|
|  | [getProcessedDocuments()](#getProcessedDocuments--) | 获取成功处理的文档数量。 |
|
|  | [getSkippedDocuments()](#getSkippedDocuments--) | 获取被跳过的文档数量。 |
|
|  | [getProgressPercentage()](#getProgressPercentage--) | 获取进度的百分比。 |
|
|  | [getLastDocumentKey()](#getLastDocumentKey--) | 获取最后处理的文档键。 |
|
|  | [getLastDocumentPath()](#getLastDocumentPath--) | 获取最后处理的文档路径。 |
|
|  | [getLastDocumentStatus()](#getLastDocumentStatus--) | 获取最后处理的文档状态。 |
|
### getTotalDocuments() {#getTotalDocuments--}
```
public final int getTotalDocuments()
```


获取待处理文档的总数。


**Returns:**
int - 待处理文档的总数。

### getProcessedDocuments() {#getProcessedDocuments--}
```
public final int getProcessedDocuments()
```


获取成功处理的文档数量。


**Returns:**
int - 成功处理的文档数量。

### getSkippedDocuments() {#getSkippedDocuments--}
```
public final int getSkippedDocuments()
```


获取被跳过的文档数量。


**Returns:**
int - 被跳过的文档数量。

### getProgressPercentage() {#getProgressPercentage--}
```
public final double getProgressPercentage()
```


获取进度的百分比。


**Returns:**
double - 进度的百分比。

### getLastDocumentKey() {#getLastDocumentKey--}
```
public final String getLastDocumentKey()
```


获取最后处理的文档键。


**Returns:**
java.lang.String - 最后处理的文档键。

### getLastDocumentPath() {#getLastDocumentPath--}
```
public final String getLastDocumentPath()
```


获取最后处理的文档路径。


**Returns:**
java.lang.String - 最后处理的文档路径。

### getLastDocumentStatus() {#getLastDocumentStatus--}
```
public final DocumentStatus getLastDocumentStatus()
```


获取最后处理的文档状态。


**Returns:**
[DocumentStatus](../../com.groupdocs.search.common/documentstatus) - The last processed document status.

