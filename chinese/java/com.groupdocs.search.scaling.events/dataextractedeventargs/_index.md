---
title: "DataExtractedEventArgs"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示文档数据提取完成事件的参数。"
type: docs
weight: 10
url: /zh/java/com.groupdocs.search.scaling.events/dataextractedeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class DataExtractedEventArgs extends EventArgs
```

表示文档数据提取完成事件的参数。

## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getExtractorIndex()](#getExtractorIndex--) | 获取提取器索引。 |
|
|  | [getDocumentKey()](#getDocumentKey--) | 获取文档键。 |
|
### getExtractorIndex() {#getExtractorIndex--}
```
public final int getExtractorIndex()
```


获取提取器索引。


**Returns:**
int - 提取器索引。

### getDocumentKey() {#getDocumentKey--}
```
public final String getDocumentKey()
```


获取文档键。


**Returns:**
java.lang.String - 文档键。

