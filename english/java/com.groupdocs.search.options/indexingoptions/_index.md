---
title: IndexingOptions
second_title: GroupDocs.Search for Java API Reference
description: Provides options for indexing operation.
type: docs
weight: 25
url: /java/com.groupdocs.search.options/indexingoptions/
---
**Inheritance:**
java.lang.Object
```
public class IndexingOptions
```

Provides options for indexing operation.

**Learn more**

 *  [Indexing options][]


[Indexing options]: https://docs.groupdocs.com/display/searchjava/Indexing+options
## Constructors

| Constructor | Description |
| --- | --- |
| [IndexingOptions()](#IndexingOptions--) | Initializes a new instance of the  IndexingOptions  class. |
| [IndexingOptions(Object data)](#IndexingOptions-java.lang.Object-) | Initializes a new instance of the  IndexingOptions  class. |
## Methods

| Method | Description |
| --- | --- |
| [getThreads()](#getThreads--) | Gets the number of threads used for indexing. |
| [setThreads(int value)](#setThreads-int-) | Sets the number of threads used for indexing. |
| [isAsync()](#isAsync--) | Gets the flag of asynchronous performing the operation. |
| [setAsync(boolean value)](#setAsync-boolean-) | Sets the flag of asynchronous performing the operation. |
| [getCancellation()](#getCancellation--) | Gets the operation cancellation object. |
| [setCancellation(Cancellation value)](#setCancellation-com.groupdocs.search.common.Cancellation-) | Sets the operation cancellation object. |
| [getAutoDetectEncoding()](#getAutoDetectEncoding--) | Gets a value indicating whether to detect encoding automatically or not. |
| [setAutoDetectEncoding(boolean value)](#setAutoDetectEncoding-boolean-) | Sets a value indicating whether to detect encoding automatically or not. |
| [getEncoding()](#getEncoding--) | Gets the encoding used to extract text from text documents. |
| [setEncoding(String value)](#setEncoding-java.lang.String-) | Sets the encoding used to extract text from text documents. |
| [getUseRawTextExtraction()](#getUseRawTextExtraction--) | Gets a value indicating whether the raw mode is used for text extraction if possible. |
| [setUseRawTextExtraction(boolean value)](#setUseRawTextExtraction-boolean-) | Sets a value indicating whether the raw mode is used for text extraction if possible. |
| [getMetadataIndexingOptions()](#getMetadataIndexingOptions--) | Gets the options for indexing metadata fields. |
| [getOcrIndexingOptions()](#getOcrIndexingOptions--) | Gets the options for OCR processing and indexing recognized text. |
| [getImageIndexingOptions()](#getImageIndexingOptions--) | Gets the image indexing options for reverse image search. |
| [getCore()](#getCore--) |  |
### IndexingOptions() {#IndexingOptions--}
```
public IndexingOptions()
```


Initializes a new instance of the  IndexingOptions  class.

### IndexingOptions(Object data) {#IndexingOptions-java.lang.Object-}
```
public IndexingOptions(Object data)
```


Initializes a new instance of the  IndexingOptions  class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| data | java.lang.Object | The serialized data. |

### getThreads() {#getThreads--}
```
public int getThreads()
```


Gets the number of threads used for indexing. The default value is  1 .

**Returns:**
int - The number of threads used for indexing.
### setThreads(int value) {#setThreads-int-}
```
public void setThreads(int value)
```


Sets the number of threads used for indexing. The default value is  1 .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | The number of threads used for indexing. |

### isAsync() {#isAsync--}
```
public boolean isAsync()
```


Gets the flag of asynchronous performing the operation. The default value is  false .

**Returns:**
boolean - The flag of asynchronous performing the operation.
### setAsync(boolean value) {#setAsync-boolean-}
```
public void setAsync(boolean value)
```


Sets the flag of asynchronous performing the operation. The default value is  false .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The flag of asynchronous performing the operation. |

### getCancellation() {#getCancellation--}
```
public Cancellation getCancellation()
```


Gets the operation cancellation object. The default value is  null .

**Returns:**
[Cancellation](../../com.groupdocs.search.common/cancellation) - The operation cancellation object.
### setCancellation(Cancellation value) {#setCancellation-com.groupdocs.search.common.Cancellation-}
```
public void setCancellation(Cancellation value)
```


Sets the operation cancellation object. The default value is  null .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Cancellation](../../com.groupdocs.search.common/cancellation) | The operation cancellation object. |

### getAutoDetectEncoding() {#getAutoDetectEncoding--}
```
public boolean getAutoDetectEncoding()
```


Gets a value indicating whether to detect encoding automatically or not. The default value is  false .

**Returns:**
boolean - A value indicating whether to detect encoding automatically or not.
### setAutoDetectEncoding(boolean value) {#setAutoDetectEncoding-boolean-}
```
public void setAutoDetectEncoding(boolean value)
```


Sets a value indicating whether to detect encoding automatically or not. The default value is  false .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | A value indicating whether to detect encoding automatically or not. |

### getEncoding() {#getEncoding--}
```
public String getEncoding()
```


Gets the encoding used to extract text from text documents. The default value is  null , which means that the default encoding UTF-8 is used. If AutoDetectEncoding is  true  then this value is used as the default encoding.

**Returns:**
java.lang.String - The encoding used to extract text from text documents.
### setEncoding(String value) {#setEncoding-java.lang.String-}
```
public void setEncoding(String value)
```


Sets the encoding used to extract text from text documents. The default value is  null , which means that the default encoding UTF-8 is used. If AutoDetectEncoding is  true  then this value is used as the default encoding.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | The encoding used to extract text from text documents. |

### getUseRawTextExtraction() {#getUseRawTextExtraction--}
```
public boolean getUseRawTextExtraction()
```


Gets a value indicating whether the raw mode is used for text extraction if possible. The default value is  true . The raw mode can significantly increase the indexing speed, but normal mode improves the formatting of the extracted text.

**Returns:**
boolean - A value indicating whether the raw mode is used for text extraction if possible.
### setUseRawTextExtraction(boolean value) {#setUseRawTextExtraction-boolean-}
```
public void setUseRawTextExtraction(boolean value)
```


Sets a value indicating whether the raw mode is used for text extraction if possible. The default value is  true . The raw mode can significantly increase the indexing speed, but normal mode improves the formatting of the extracted text.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | A value indicating whether the raw mode is used for text extraction if possible. |

### getMetadataIndexingOptions() {#getMetadataIndexingOptions--}
```
public MetadataIndexingOptions getMetadataIndexingOptions()
```


Gets the options for indexing metadata fields.

**Returns:**
[MetadataIndexingOptions](../../com.groupdocs.search.options/metadataindexingoptions) - The options for indexing metadata fields.
### getOcrIndexingOptions() {#getOcrIndexingOptions--}
```
public OcrIndexingOptions getOcrIndexingOptions()
```


Gets the options for OCR processing and indexing recognized text.

**Returns:**
[OcrIndexingOptions](../../com.groupdocs.search.options/ocrindexingoptions) - The options for OCR processing and indexing recognized text.
### getImageIndexingOptions() {#getImageIndexingOptions--}
```
public ImageIndexingOptions getImageIndexingOptions()
```


Gets the image indexing options for reverse image search.

**Returns:**
[ImageIndexingOptions](../../com.groupdocs.search.options/imageindexingoptions) - The image indexing options for reverse image search.
### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
