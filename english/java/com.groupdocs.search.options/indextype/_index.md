---
title: IndexType
second_title: GroupDocs.Search for Java API Reference
description: Specifies an index type.
type: docs
weight: 45
url: /java/com.groupdocs.search.options/indextype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum IndexType extends Enum<IndexType>
```

Specifies an index type.

**Learn more**

 *  [Search index settings][]


[Search index settings]: https://docs.groupdocs.com/display/searchjava/Search+index+settings
## Fields

| Field | Description |
| --- | --- |
| [NormalIndex](#NormalIndex) | Normal index with documents metadata and documents content which supports all search features. |
| [MetadataIndex](#MetadataIndex) | Index that contains only metadata of documents, without content. |
| [CompactIndex](#CompactIndex) | Index type that takes much less disk space but does not support phrase search and date range search features. |
## Methods

| Method | Description |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### NormalIndex {#NormalIndex}
```
public static final IndexType NormalIndex
```


Normal index with documents metadata and documents content which supports all search features.

### MetadataIndex {#MetadataIndex}
```
public static final IndexType MetadataIndex
```


Index that contains only metadata of documents, without content.

### CompactIndex {#CompactIndex}
```
public static final IndexType CompactIndex
```


Index type that takes much less disk space but does not support phrase search and date range search features.

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
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[IndexType](../../com.groupdocs.search.options/indextype)
