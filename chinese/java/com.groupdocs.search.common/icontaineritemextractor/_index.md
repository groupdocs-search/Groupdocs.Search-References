---
title: "IContainerItemExtractor"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "提供从容器文档中提取项目的方法。"
type: docs
weight: 35
url: /zh/java/com.groupdocs.search.common/icontaineritemextractor/
---
**All Implemented Interfaces:**
[com.groupdocs.search.common.IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor)
```
public interface IContainerItemExtractor extends IFieldExtractor
```

提供从容器文档中提取项目的方法。


**Learn more**

* [Custom text extractors](../https://docs.groupdocs.com/display/searchjava/Custom+text+extractors)

## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getFormatFamily()](#getFormatFamily--) | 获取文档格式系列。 |
|
|  | [getContainerItems(String filePath)](#getContainerItems-java.lang.String-) | 从容器文档中提取项目。 |
|
|  | [getContainerItems(InputStream stream)](#getContainerItems-java.io.InputStream-) | 从容器文档中提取项目。 |
|
### getFormatFamily() {#getFormatFamily--}
```
public abstract FormatFamily getFormatFamily()
```


获取文档格式系列。


**Returns:**
[FormatFamily](../../com.groupdocs.search.results/formatfamily) - The document format family.

### getContainerItems(String filePath) {#getContainerItems-java.lang.String-}
```
public abstract ExtractedItemInfo[] getContainerItems(String filePath)
```


从容器文档中提取项目。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 文件路径 | java.lang.String | 文件路径。 |
|

**Returns:**
com.groupdocs.search.common.ExtractedItemInfo[] - 提取项目的数组。

### getContainerItems(InputStream stream) {#getContainerItems-java.io.InputStream-}
```
public abstract ExtractedItemInfo[] getContainerItems(InputStream stream)
```


从容器文档中提取项目。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 流 | java.io.InputStream | 文档流。 |
|

**Returns:**
com.groupdocs.search.common.ExtractedItemInfo[] - 提取项目的数组。

