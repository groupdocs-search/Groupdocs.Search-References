---
title: "FileIndexingEventArgs"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示文档索引开始事件的参数。"
type: docs
weight: 14
url: /zh/java/com.groupdocs.search.events/fileindexingeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class FileIndexingEventArgs extends BaseIndexEventArgs
```

表示文档索引开始事件的参数。


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getDocument()](#getDocument--) | 获取文档。 |
|
|  | [getDocumentFullPath()](#getDocumentFullPath--) | 获取文档的完整路径。 |
|
|  | [getDocumentKey()](#getDocumentKey--) | 获取文档键。 |
|
|  | [getSkipIndexing()](#getSkipIndexing--) | 获取一个值，指示应跳过文档的索引。 |
|
|  | [setSkipIndexing(boolean value)](#setSkipIndexing-boolean-) | 设置一个值，指示应跳过文档的索引。 |
|
|  | [getEncoding()](#getEncoding--) | 获取文档的编码。 |
|
|  | [setEncoding(String value)](#setEncoding-java.lang.String-) | 设置文档的编码。 |
|
|  | [getCustomExtractor()](#getCustomExtractor--) | 获取自定义文本提取器。 |
|
|  | [setCustomExtractor(IFieldExtractor value)](#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-) | 设置自定义文本提取器。 |
|
|  | [getAdditionalFields()](#getAdditionalFields--) | 获取文档的附加字段。 |
|
|  | [setAdditionalFields(DocumentField[] value)](#setAdditionalFields-com.groupdocs.search.common.DocumentField---) | 设置文档的附加字段。 |
|
|  | [getAttributes()](#getAttributes--) | 获取文档的属性。 |
|
|  | [setAttributes(String[] value)](#setAttributes-java.lang.String---) | 设置文档的属性。 |
|
### getDocument() {#getDocument--}
```
public final Document getDocument()
```


获取文档。


**Returns:**
[Document](../../com.groupdocs.search/document) - The document.

### getDocumentFullPath() {#getDocumentFullPath--}
```
public final String getDocumentFullPath()
```


获取文档的完整路径。


**Returns:**
java.lang.String - 文档的完整路径。

### getDocumentKey() {#getDocumentKey--}
```
public final String getDocumentKey()
```


获取文档键。


**Returns:**
java.lang.String - 文档键。

### getSkipIndexing() {#getSkipIndexing--}
```
public final boolean getSkipIndexing()
```


获取一个值，指示应跳过文档的索引。


**Returns:**
boolean - 一个指示应跳过文档索引的值。

### setSkipIndexing(boolean value) {#setSkipIndexing-boolean-}
```
public final void setSkipIndexing(boolean value)
```


设置一个值，指示应跳过文档的索引。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | boolean | 一个指示应跳过文档索引的值。 |
|

### getEncoding() {#getEncoding--}
```
public final String getEncoding()
```


获取文档的编码。


**Returns:**
java.lang.String - 文档的编码。

### setEncoding(String value) {#setEncoding-java.lang.String-}
```
public final void setEncoding(String value)
```


设置文档的编码。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | java.lang.String | 文档的编码。 |
|

### getCustomExtractor() {#getCustomExtractor--}
```
public final IFieldExtractor getCustomExtractor()
```


获取自定义文本提取器。


**Returns:**
[IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) - The custom text extractor.

### setCustomExtractor(IFieldExtractor value) {#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-}
```
public final void setCustomExtractor(IFieldExtractor value)
```


设置自定义文本提取器。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | value | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | 自定义文本提取器。 |
|

### getAdditionalFields() {#getAdditionalFields--}
```
public final DocumentField[] getAdditionalFields()
```


获取文档的附加字段。


**Returns:**
com.groupdocs.search.common.DocumentField[] - 文档的附加字段。

### setAdditionalFields(DocumentField[] value) {#setAdditionalFields-com.groupdocs.search.common.DocumentField---}
```
public final void setAdditionalFields(DocumentField[] value)
```


设置文档的附加字段。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | value | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | 文档的附加字段。 |
|

### getAttributes() {#getAttributes--}
```
public final String[] getAttributes()
```


获取文档的属性。


**Returns:**
java.lang.String[] - 文档的属性。

### setAttributes(String[] value) {#setAttributes-java.lang.String---}
```
public final void setAttributes(String[] value)
```


设置文档的属性。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | java.lang.String[] | 文档的属性。 |
|

