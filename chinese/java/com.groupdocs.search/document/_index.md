---
title: "文档"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示从文件系统流或结构添加到索引的文档的基类。"
type: docs
weight: 13
url: /zh/java/com.groupdocs.search/document/
---
**Inheritance:**
java.lang.Object
```
public abstract class Document
```

表示从文件系统、流或结构添加到索引的文档的基类。包含用于从不同类型来源创建文档的静态方法。


**Learn more**

* [Indexing from different sources](../https://docs.groupdocs.com/search/java/indexing-from-different-sources/)

## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getDocumentSourceKind()](#getDocumentSourceKind--) | 获取文档来源类型。 |
|
|  | [getDocumentKey()](#getDocumentKey--) | 获取用于在索引中标识文档的文档键。 |
|
|  | [isLazy()](#isLazy--) | 获取指示文档是否按需加载的值。 |
|
|  | [getModificationDate()](#getModificationDate--) | 获取文档的最后修改日期。 |
|
|  | [getExtension()](#getExtension--) | 获取此文档类型使用的扩展名。 |
|
|  | [getAdditionalFields()](#getAdditionalFields--) | 获取文档的附加字段。 |
|
|  | [setAdditionalFields(DocumentField[] value)](#setAdditionalFields-com.groupdocs.search.common.DocumentField---) | 设置文档的附加字段。 |
|
|  | [getAttributes()](#getAttributes--) | 获取文档的属性。 |
|
|  | [setAttributes(String[] value)](#setAttributes-java.lang.String---) | 设置文档的属性。 |
|
|  | [createFromFile(String filePath)](#createFromFile-java.lang.String-) | 从文件创建文档。 |
|
|  | [createFromStream(String documentKey, Date modificationDate, String extension, InputStream stream)](#createFromStream-java.lang.String-java.util.Date-java.lang.String-java.io.InputStream-) | 从流创建文档。 |
|
|  | [createFromStructure(String documentKey, Date modificationDate, DocumentField[] fields)](#createFromStructure-java.lang.String-java.util.Date-com.groupdocs.search.common.DocumentField---) | 从结构（文本字段数组）创建文档。 |
|
|  | [createLazy(DocumentSourceKind documentSourceKind, String documentKey, IDocumentLoader documentLoader)](#createLazy-com.groupdocs.search.common.DocumentSourceKind-java.lang.String-com.groupdocs.search.common.IDocumentLoader-) | 创建延迟加载的文档。 |
|
|  | [toString()](#toString--) | 返回一个  java.lang.String  表示当前的  文档 。 |
|
### getDocumentSourceKind() {#getDocumentSourceKind--}
```
public abstract DocumentSourceKind getDocumentSourceKind()
```


获取文档来源类型。


**Returns:**
[DocumentSourceKind](../../com.groupdocs.search.common/documentsourcekind) - The document source kind.

### getDocumentKey() {#getDocumentKey--}
```
public abstract String getDocumentKey()
```


获取用于在索引中标识文档的文档键。


**Returns:**
java.lang.String - 用于在索引中标识文档的文档键。

### isLazy() {#isLazy--}
```
public abstract boolean isLazy()
```


获取指示文档是否按需加载的值。


**Returns:**
boolean - 指示文档是否按需加载的值。

### getModificationDate() {#getModificationDate--}
```
public abstract Date getModificationDate()
```


获取文档的最后修改日期。


**Returns:**
java.util.Date - 文档的最后修改日期。

### getExtension() {#getExtension--}
```
public abstract String getExtension()
```


获取此文档类型使用的扩展名。


**Returns:**
java.lang.String - 此文档类型使用的扩展名。

### getAdditionalFields() {#getAdditionalFields--}
```
public DocumentField[] getAdditionalFields()
```


获取文档的附加字段。


**Returns:**
com.groupdocs.search.common.DocumentField[] - 文档的附加字段。

### setAdditionalFields(DocumentField[] value) {#setAdditionalFields-com.groupdocs.search.common.DocumentField---}
```
public void setAdditionalFields(DocumentField[] value)
```


设置文档的附加字段。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | value | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | 文档的附加字段。 |
|

### getAttributes() {#getAttributes--}
```
public String[] getAttributes()
```


获取文档的属性。


**Returns:**
java.lang.String[] - 文档的属性。

### setAttributes(String[] value) {#setAttributes-java.lang.String---}
```
public void setAttributes(String[] value)
```


设置文档的属性。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | java.lang.String[] | 文档的属性。 |
|

### createFromFile(String filePath) {#createFromFile-java.lang.String-}
```
public static Document createFromFile(String filePath)
```


从文件创建文档。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 文件路径 | java.lang.String | 文档文件路径。 |
|

**Returns:**
[Document](../../com.groupdocs.search/document) - The created document.

### createFromStream(String documentKey, Date modificationDate, String extension, InputStream stream) {#createFromStream-java.lang.String-java.util.Date-java.lang.String-java.io.InputStream-}
```
public static Document createFromStream(String documentKey, Date modificationDate, String extension, InputStream stream)
```


从流创建文档。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 文档键 | java.lang.String | 文档键。 |
|
|  | 修改日期 | java.util.Date | 文档修改日期。 |
|
|  | 扩展名 | java.lang.String | 文档扩展名。 |
|
|  | 流 | java.io.InputStream | 文档流。 |
|

**Returns:**
[Document](../../com.groupdocs.search/document) - The created document.

### createFromStructure(String documentKey, Date modificationDate, DocumentField[] fields) {#createFromStructure-java.lang.String-java.util.Date-com.groupdocs.search.common.DocumentField---}
```
public static Document createFromStructure(String documentKey, Date modificationDate, DocumentField[] fields)
```


从结构（文本字段数组）创建文档。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 文档键 | java.lang.String | 文档键。 |
|
|  | 修改日期 | java.util.Date | 文档修改日期。 |
|
|  | fields | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | 文档字段。 |
|

**Returns:**
[Document](../../com.groupdocs.search/document) - The created document.

### createLazy(DocumentSourceKind documentSourceKind, String documentKey, IDocumentLoader documentLoader) {#createLazy-com.groupdocs.search.common.DocumentSourceKind-java.lang.String-com.groupdocs.search.common.IDocumentLoader-}
```
public static Document createLazy(DocumentSourceKind documentSourceKind, String documentKey, IDocumentLoader documentLoader)
```


创建延迟加载的文档。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | documentSourceKind | [DocumentSourceKind](../../com.groupdocs.search.common/documentsourcekind) | 文档来源类型。此值必须与加载的文档类型匹配。 |
|
|  | 文档键 | java.lang.String | 文档键。此值必须与加载的文档键匹配。 |
|
|  | documentLoader | [IDocumentLoader](../../com.groupdocs.search.common/idocumentloader) | 文档加载器。 |
|

**Returns:**
[Document](../../com.groupdocs.search/document) - The created document.

### toString() {#toString--}
```
public String toString()
```


返回一个  java.lang.String  表示当前的  文档 。


**Returns:**
java.lang.String - 一个 java.lang.String，表示当前的 Document。

