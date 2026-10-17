---
title: "TextOptions"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "提供从索引检索文档文本的选项。"
type: docs
weight: 41
url: /zh/java/com.groupdocs.search.options/textoptions/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.search.options.ITextOptions](../../com.groupdocs.search.options/itextoptions)
```
public class TextOptions implements ITextOptions
```

提供从索引检索文档文本的选项。


**Learn more**

* [Getting indexed documents](../https://docs.groupdocs.com/display/searchjava/Getting+indexed+documents)
* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [TextOptions()](#TextOptions--) | 初始化 TextOptions 类的新实例。 |
|
|  | [TextOptions(Object data)](#TextOptions-java.lang.Object-) | 初始化 TextOptions 类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getCustomExtractor()](#getCustomExtractor--) | 获取用于索引的自定义文本提取器。 |
|
|  | [setCustomExtractor(IFieldExtractor value)](#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-) | 设置用于索引的自定义文本提取器。 |
|
|  | [getAdditionalFields()](#getAdditionalFields--) | 获取用于索引的附加文档字段。 |
|
|  | [setAdditionalFields(DocumentField[] value)](#setAdditionalFields-com.groupdocs.search.common.DocumentField---) | 设置用于索引的附加文档字段。 |
|
|  | [getCancellation()](#getCancellation--) | 获取取消对象。 |
|
|  | [setCancellation(Cancellation value)](#setCancellation-com.groupdocs.search.common.Cancellation-) | 设置取消对象。 |
|
|  | [getGenerateHead()](#getGenerateHead--) | 获取指示是否在输出 HTML 中生成 Head 标记的值。 |
|
|  | [setGenerateHead(boolean value)](#setGenerateHead-boolean-) | 设置指示是否在输出 HTML 中生成 Head 标记的值。 |
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
### TextOptions() {#TextOptions--}
```
public TextOptions()
```


初始化 TextOptions 类的新实例。


### TextOptions(Object data) {#TextOptions-java.lang.Object-}
```
public TextOptions(Object data)
```


初始化 TextOptions 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 数据 | java.lang.Object | 序列化的数据。 |
|

### getCustomExtractor() {#getCustomExtractor--}
```
public IFieldExtractor getCustomExtractor()
```


获取用于索引的自定义文本提取器。默认值为 null。请注意，仅在文档文本未保存到索引时才使用此值。


**Returns:**
[IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) - The custom text extractor that was used for indexing.

### setCustomExtractor(IFieldExtractor value) {#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-}
```
public void setCustomExtractor(IFieldExtractor value)
```


设置用于索引的自定义文本提取器。默认值为 null。请注意，仅在文档文本未保存到索引时才使用此值。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | value | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | 用于索引的自定义文本提取器。 |
|

### getAdditionalFields() {#getAdditionalFields--}
```
public DocumentField[] getAdditionalFields()
```


获取用于索引的附加文档字段。默认值为 null。请注意，仅在文档文本未保存到索引时才使用此值。


**Returns:**
com.groupdocs.search.common.DocumentField[] - 用于索引的附加文档字段。

### setAdditionalFields(DocumentField[] value) {#setAdditionalFields-com.groupdocs.search.common.DocumentField---}
```
public void setAdditionalFields(DocumentField[] value)
```


设置用于索引的附加文档字段。默认值为 null。请注意，仅在文档文本未保存到索引时才使用此值。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | value | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | 用于索引的附加文档字段。 |
|

### getCancellation() {#getCancellation--}
```
public Cancellation getCancellation()
```


获取取消对象。默认值为 null。


**Returns:**
[Cancellation](../../com.groupdocs.search.common/cancellation) - The cancellation object.

### setCancellation(Cancellation value) {#setCancellation-com.groupdocs.search.common.Cancellation-}
```
public void setCancellation(Cancellation value)
```


设置取消对象。默认值为 null。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | value | [Cancellation](../../com.groupdocs.search.common/cancellation) | 取消对象。 |
|

### getGenerateHead() {#getGenerateHead--}
```
public boolean getGenerateHead()
```


获取指示是否在输出 HTML 中生成 Head 标记的值。默认值为 true。


**Returns:**
boolean - 指示是否在输出 HTML 中生成 Head 标记的值。

### setGenerateHead(boolean value) {#setGenerateHead-boolean-}
```
public void setGenerateHead(boolean value)
```


设置指示是否在输出 HTML 中生成 Head 标记的值。默认值为 true。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | boolean | 指示是否在输出 HTML 中生成 Head 标记的值。 |
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
