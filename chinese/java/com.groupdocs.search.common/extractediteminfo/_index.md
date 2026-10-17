---
title: "ExtractedItemInfo"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示容器项信息。"
type: docs
weight: 18
url: /zh/java/com.groupdocs.search.common/extractediteminfo/
---
**Inheritance:**
java.lang.Object
```
public class ExtractedItemInfo
```

表示容器项信息。


**Learn more**

* [Custom text extractors](../https://docs.groupdocs.com/display/searchjava/Custom+text+extractors)

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [ExtractedItemInfo(FormatFamily formatFamily, DocumentField[] fields, String itemInfo, String innerPath)](#ExtractedItemInfo-com.groupdocs.search.results.FormatFamily-com.groupdocs.search.common.DocumentField---java.lang.String-java.lang.String-) | 初始化 ExtractedItemInfo 类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getFormatFamily()](#getFormatFamily--) | 获取文档类型。 |
|
|  | [getFields()](#getFields--) | 获取提取的字段。 |
|
|  | [getItemInfo()](#getItemInfo--) | 获取项目信息。 |
|
|  | [getInnerPath()](#getInnerPath--) | 获取内部路径。 |
|
### ExtractedItemInfo(FormatFamily formatFamily, DocumentField[] fields, String itemInfo, String innerPath) {#ExtractedItemInfo-com.groupdocs.search.results.FormatFamily-com.groupdocs.search.common.DocumentField---java.lang.String-java.lang.String-}
```
public ExtractedItemInfo(FormatFamily formatFamily, DocumentField[] fields, String itemInfo, String innerPath)
```


初始化 ExtractedItemInfo 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | formatFamily | [FormatFamily](../../com.groupdocs.search.results/formatfamily) | 文档格式系列。 |
|
|  | fields | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | 提取的字段。 |
|
|  | itemInfo | java.lang.String | 项目信息。 |
|
|  | innerPath | java.lang.String | 容器中项的路径。 |
|

### getFormatFamily() {#getFormatFamily--}
```
public final FormatFamily getFormatFamily()
```


获取文档类型。


**Returns:**
[FormatFamily](../../com.groupdocs.search.results/formatfamily) - The document type.

### getFields() {#getFields--}
```
public final DocumentField[] getFields()
```


获取提取的字段。


**Returns:**
com.groupdocs.search.common.DocumentField[] - 提取的字段。

### getItemInfo() {#getItemInfo--}
```
public final String getItemInfo()
```


获取项目信息。


**Returns:**
java.lang.String - 项目信息。

### getInnerPath() {#getInnerPath--}
```
public final String getInnerPath()
```


获取内部路径。


**Returns:**
java.lang.String - 内部路径。

