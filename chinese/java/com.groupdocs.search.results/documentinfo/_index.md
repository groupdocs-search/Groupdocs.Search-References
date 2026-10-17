---
title: "DocumentInfo"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示已索引文档的描述符。"
type: docs
weight: 11
url: /zh/java/com.groupdocs.search.results/documentinfo/
---
**Inheritance:**
java.lang.Object
```
public abstract class DocumentInfo
```

表示已索引文档的描述符。


**Learn more**

* [Search results](../https://docs.groupdocs.com/display/searchjava/Search+results)
* [Getting indexed documents](../https://docs.groupdocs.com/display/searchjava/Getting+indexed+documents)

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [DocumentInfo()](#DocumentInfo--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [toString()](#toString--) | 返回一个  System.String ，它表示当前的  DocumentInfo 。 |
|
|  | [getFilePath()](#getFilePath--) | 获取从文件索引的文件路径或从流或结构索引的文档键。 |
|
|  | [getFileType()](#getFileType--) | 获取文件类型。 |
|
|  | [getFormatFamily()](#getFormatFamily--) | 获取文档格式系列。 |
|
|  | [getInnerPath()](#getInnerPath--) | 获取容器文档项的内部路径。 |
|
|  | [getInnerPathParts()](#getInnerPathParts--) | 获取容器文档项的内部路径部分。 |
|
|  | [getDocumentSourceKind()](#getDocumentSourceKind--) | 获取文档来源类型。 |
|
|  | [getIndexedWithError()](#getIndexedWithError--) | 获取索引错误的指示器。 |
|
|  | [serialize()](#serialize--) | 将当前实例序列化为字节数组。 |
|
|  | [deserialize(byte[] array)](#deserialize-byte---) | 从字节数组反序列化实例。 |
|
### DocumentInfo() {#DocumentInfo--}
```
public DocumentInfo()
```


### toString() {#toString--}
```
public abstract String toString()
```


返回一个  System.String ，它表示当前的  DocumentInfo 。


**Returns:**
java.lang.String - 一个  System.String ，它表示当前的  DocumentInfo 。

### getFilePath() {#getFilePath--}
```
public abstract String getFilePath()
```


获取从文件索引的文件路径或从流或结构索引的文档键。


**Returns:**
java.lang.String - 文件路径或文档键。

### getFileType() {#getFileType--}
```
public abstract FileType getFileType()
```


获取文件类型。


**Returns:**
[FileType](../../com.groupdocs.search.results/filetype) - The file type.

### getFormatFamily() {#getFormatFamily--}
```
public abstract FormatFamily getFormatFamily()
```


获取文档格式系列。


**Returns:**
[FormatFamily](../../com.groupdocs.search.results/formatfamily) - The document format family.

### getInnerPath() {#getInnerPath--}
```
public abstract String getInnerPath()
```


获取容器文档项的内部路径。


**Returns:**
java.lang.String - 内部路径。

### getInnerPathParts() {#getInnerPathParts--}
```
public abstract String[] getInnerPathParts()
```


获取容器文档项的内部路径部分。


**Returns:**
java.lang.String[] - 内部路径部分。

### getDocumentSourceKind() {#getDocumentSourceKind--}
```
public abstract DocumentSourceKind getDocumentSourceKind()
```


获取文档来源类型。


**Returns:**
[DocumentSourceKind](../../com.groupdocs.search.common/documentsourcekind) - The document source kind.

### getIndexedWithError() {#getIndexedWithError--}
```
public abstract boolean getIndexedWithError()
```


获取索引错误的指示器。


**Returns:**
boolean - 索引错误的指示器。

### serialize() {#serialize--}
```
public abstract byte[] serialize()
```


将当前实例序列化为字节数组。


**Returns:**
byte[] - 表示当前实例的字节数组。

### deserialize(byte[] array) {#deserialize-byte---}
```
public static DocumentInfo deserialize(byte[] array)
```


从字节数组反序列化实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 数组 | byte[] | 用于反序列化的字节数组。 |
|

**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - An instance deserialized from a byte array.

