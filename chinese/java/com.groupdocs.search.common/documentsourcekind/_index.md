---
title: "DocumentSourceKind"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "定义文档来源的类型。"
type: docs
weight: 39
url: /zh/java/com.groupdocs.search.common/documentsourcekind/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum DocumentSourceKind extends Enum<DocumentSourceKind>
```

定义文档来源的类型。

## Fields

| Field | 描述 |
| --- | --- |
|  | [File](#File) | 文件文档源。 |
|
|  | [Stream](#Stream) | 流文档源。 |
|
|  | [Structure](#Structure) | 结构文档源。 |
|
|  | [ExtractedData](#ExtractedData) | 先前提取数据的文档源。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### File {#File}
```
public static final DocumentSourceKind File
```


文件文档源。


### Stream {#Stream}
```
public static final DocumentSourceKind Stream
```


流文档源。


### Structure {#Structure}
```
public static final DocumentSourceKind Structure
```


结构文档源。


### ExtractedData {#ExtractedData}
```
public static final DocumentSourceKind ExtractedData
```


先前提取数据的文档源。


### values() {#values--}
```
public static DocumentSourceKind[] values()
```




**Returns:**
com.groupdocs.search.common.DocumentSourceKind[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static DocumentSourceKind valueOf(String name)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String |  |

**Returns:**
[DocumentSourceKind](../../com.groupdocs.search.common/documentsourcekind)
