---
title: "ExtractorSettings"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "包含文档数据提取器的设置。"
type: docs
weight: 19
url: /zh/java/com.groupdocs.search.common/extractorsettings/
---
**Inheritance:**
java.lang.Object
```
public abstract class ExtractorSettings
```

包含文档数据提取器的设置。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [ExtractorSettings()](#ExtractorSettings--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getIndexType()](#getIndexType--) | 获取提取器使用的索引类型。 |
|
|  | [setIndexType(IndexType value)](#setIndexType-com.groupdocs.search.options.IndexType-) | 设置提取器使用的索引类型。 |
|
### ExtractorSettings() {#ExtractorSettings--}
```
public ExtractorSettings()
```


### getIndexType() {#getIndexType--}
```
public abstract IndexType getIndexType()
```


获取提取器使用的索引类型。默认值为 GroupDocs.Search.Options.IndexType.NormalIndex。


**Returns:**
[IndexType](../../com.groupdocs.search.options/indextype) - The index type the extractor is used for.

### setIndexType(IndexType value) {#setIndexType-com.groupdocs.search.options.IndexType-}
```
public abstract void setIndexType(IndexType value)
```


设置提取器使用的索引类型。默认值为 GroupDocs.Search.Options.IndexType.NormalIndex。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | value | [IndexType](../../com.groupdocs.search.options/indextype) | 提取器使用的索引类型。 |
|

