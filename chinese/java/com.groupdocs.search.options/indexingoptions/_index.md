---
title: "IndexingOptions"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "提供索引操作的选项。"
type: docs
weight: 25
url: /zh/java/com.groupdocs.search.options/indexingoptions/
---
**Inheritance:**
java.lang.Object
```
public class IndexingOptions
```

提供索引操作的选项。


**Learn more**

* [Indexing options](../https://docs.groupdocs.com/display/searchjava/Indexing+options)

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [IndexingOptions()](#IndexingOptions--) | 初始化 IndexingOptions 类的新实例。 |
|
|  | [IndexingOptions(Object data)](#IndexingOptions-java.lang.Object-) | 初始化 IndexingOptions 类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getThreads()](#getThreads--) | 获取用于索引的线程数。 |
|
|  | [setThreads(int value)](#setThreads-int-) | 设置用于索引的线程数。 |
|
|  | [isAsync()](#isAsync--) | 获取异步执行操作的标志。 |
|
|  | [setAsync(boolean value)](#setAsync-boolean-) | 设置异步执行操作的标志。 |
|
|  | [getCancellation()](#getCancellation--) | 获取操作取消对象。 |
|
|  | [setCancellation(Cancellation value)](#setCancellation-com.groupdocs.search.common.Cancellation-) | 设置操作取消对象。 |
|
|  | [getAutoDetectEncoding()](#getAutoDetectEncoding--) | 获取指示是否自动检测编码的值。 |
|
|  | [setAutoDetectEncoding(boolean value)](#setAutoDetectEncoding-boolean-) | 设置指示是否自动检测编码的值。 |
|
|  | [getEncoding()](#getEncoding--) | 获取用于从文本文件中提取文本的编码。 |
|
|  | [setEncoding(String value)](#setEncoding-java.lang.String-) | 设置用于从文本文件中提取文本的编码。 |
|
|  | [getUseRawTextExtraction()](#getUseRawTextExtraction--) | 获取一个值，指示是否在可能的情况下使用原始模式进行文本提取。 |
|
|  | [setUseRawTextExtraction(boolean value)](#setUseRawTextExtraction-boolean-) | 设置一个值，指示是否在可能的情况下使用原始模式进行文本提取。 |
|
|  | [getMetadataIndexingOptions()](#getMetadataIndexingOptions--) | 获取用于索引元数据字段的选项。 |
|
|  | [getOcrIndexingOptions()](#getOcrIndexingOptions--) | 获取 OCR 处理和已识别文本索引的选项。 |
|
|  | [getImageIndexingOptions()](#getImageIndexingOptions--) | 获取用于反向图像搜索的图像索引选项。 |
|
| [getCore()](#getCore--) |  |
### IndexingOptions() {#IndexingOptions--}
```
public IndexingOptions()
```


初始化 IndexingOptions 类的新实例。


### IndexingOptions(Object data) {#IndexingOptions-java.lang.Object-}
```
public IndexingOptions(Object data)
```


初始化 IndexingOptions 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 数据 | java.lang.Object | 序列化的数据。 |
|

### getThreads() {#getThreads--}
```
public int getThreads()
```


获取用于索引的线程数。默认值为 1。


**Returns:**
int - 用于索引的线程数。

### setThreads(int value) {#setThreads-int-}
```
public void setThreads(int value)
```


设置用于索引的线程数。默认值为 1。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | int | 用于索引的线程数。 |
|

### isAsync() {#isAsync--}
```
public boolean isAsync()
```


获取异步执行操作的标志。默认值为 false。


**Returns:**
boolean - 异步执行操作的标志。

### setAsync(boolean value) {#setAsync-boolean-}
```
public void setAsync(boolean value)
```


设置异步执行操作的标志。默认值为 false。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | boolean | 异步执行操作的标志。 |
|

### getCancellation() {#getCancellation--}
```
public Cancellation getCancellation()
```


获取操作取消对象。默认值为 null。


**Returns:**
[Cancellation](../../com.groupdocs.search.common/cancellation) - The operation cancellation object.

### setCancellation(Cancellation value) {#setCancellation-com.groupdocs.search.common.Cancellation-}
```
public void setCancellation(Cancellation value)
```


设置操作取消对象。默认值为 null。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | value | [Cancellation](../../com.groupdocs.search.common/cancellation) | 操作取消对象。 |
|

### getAutoDetectEncoding() {#getAutoDetectEncoding--}
```
public boolean getAutoDetectEncoding()
```


获取一个值，指示是否自动检测编码。默认值为 false。


**Returns:**
boolean - 指示是否自动检测编码的值。

### setAutoDetectEncoding(boolean value) {#setAutoDetectEncoding-boolean-}
```
public void setAutoDetectEncoding(boolean value)
```


设置一个值，指示是否自动检测编码。默认值为 false。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | boolean | 指示是否自动检测编码的值。 |
|

### getEncoding() {#getEncoding--}
```
public String getEncoding()
```


获取用于从文本文件中提取文本的编码。默认值为 null，这意味着使用默认编码 UTF-8。如果 AutoDetectEncoding 为 true，则此值用作默认编码。


**Returns:**
java.lang.String - 用于从文本文件中提取文本的编码。

### setEncoding(String value) {#setEncoding-java.lang.String-}
```
public void setEncoding(String value)
```


设置用于从文本文件中提取文本的编码。默认值为 null，这意味着使用默认编码 UTF-8。如果 AutoDetectEncoding 为 true，则此值用作默认编码。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | java.lang.String | 用于从文本文件中提取文本的编码。 |
|

### getUseRawTextExtraction() {#getUseRawTextExtraction--}
```
public boolean getUseRawTextExtraction()
```


获取一个值，指示是否在可能的情况下使用原始模式进行文本提取。默认值为 true。原始模式可以显著提高索引速度，但普通模式可以改善提取文本的格式。


**Returns:**
布尔型 - 指示是否在可能的情况下使用原始模式进行文本提取的值。

### setUseRawTextExtraction(boolean value) {#setUseRawTextExtraction-boolean-}
```
public void setUseRawTextExtraction(boolean value)
```


设置一个值，指示是否在可能的情况下使用原始模式进行文本提取。默认值为 true。原始模式可以显著提高索引速度，但普通模式可以改善提取文本的格式。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | boolean | 指示是否在可能的情况下使用原始模式进行文本提取的值。 |
|

### getMetadataIndexingOptions() {#getMetadataIndexingOptions--}
```
public MetadataIndexingOptions getMetadataIndexingOptions()
```


获取用于索引元数据字段的选项。


**Returns:**
[MetadataIndexingOptions](../../com.groupdocs.search.options/metadataindexingoptions) - The options for indexing metadata fields.

### getOcrIndexingOptions() {#getOcrIndexingOptions--}
```
public OcrIndexingOptions getOcrIndexingOptions()
```


获取 OCR 处理和已识别文本索引的选项。


**Returns:**
[OcrIndexingOptions](../../com.groupdocs.search.options/ocrindexingoptions) - The options for OCR processing and indexing recognized text.

### getImageIndexingOptions() {#getImageIndexingOptions--}
```
public ImageIndexingOptions getImageIndexingOptions()
```


获取用于反向图像搜索的图像索引选项。


**Returns:**
[ImageIndexingOptions](../../com.groupdocs.search.options/imageindexingoptions) - The image indexing options for reverse image search.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
