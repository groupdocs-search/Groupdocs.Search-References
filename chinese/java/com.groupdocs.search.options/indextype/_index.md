---
title: "IndexType"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "指定索引类型。"
type: docs
weight: 49
url: /zh/java/com.groupdocs.search.options/indextype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum IndexType extends Enum<IndexType>
```

指定索引类型。


**Learn more**

* [Search index settings](../https://docs.groupdocs.com/display/searchjava/Search+index+settings)

## Fields

| Field | 描述 |
| --- | --- |
|  | [NormalIndex](#NormalIndex) | 包含文档元数据和文档内容的普通索引，支持所有搜索功能。 |
|
|  | [MetadataIndex](#MetadataIndex) | 仅包含文档元数据而不包含内容的索引。 |
|
|  | [CompactIndex](#CompactIndex) | 占用更少磁盘空间的索引类型，但不支持短语搜索和日期范围搜索功能。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### NormalIndex {#NormalIndex}
```
public static final IndexType NormalIndex
```


包含文档元数据和文档内容的普通索引，支持所有搜索功能。


### MetadataIndex {#MetadataIndex}
```
public static final IndexType MetadataIndex
```


仅包含文档元数据而不包含内容的索引。


### CompactIndex {#CompactIndex}
```
public static final IndexType CompactIndex
```


占用更少磁盘空间的索引类型，但不支持短语搜索和日期范围搜索功能。


### values() {#values--}
```
public static IndexType[] values()
```




**Returns:**
com.groupdocs.search.options.IndexType[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static IndexType valueOf(String name)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String |  |

**Returns:**
[IndexType](../../com.groupdocs.search.options/indextype)
