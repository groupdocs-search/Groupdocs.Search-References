---
title: ExtractionOptions
second_title: GroupDocs.Search for Java API Reference
description: Provides options for extracting data from documents.
type: docs
weight: 18
url: /java/com.groupdocs.search.options/extractionoptions/
---
**Inheritance:**
java.lang.Object
```
public class ExtractionOptions
```

Provides options for extracting data from documents.
## Constructors

| Constructor | Description |
| --- | --- |
| [ExtractionOptions()](#ExtractionOptions--) | Initializes a new instance of the  ExtractionOptions  class. |
| [ExtractionOptions(Object data)](#ExtractionOptions-java.lang.Object-) | Initializes a new instance of the  ExtractionOptions  class. |
| [ExtractionOptions(IndexingOptions options, IFieldExtractor customExtractor, IOcrConnector ocrConnector)](#ExtractionOptions-com.groupdocs.search.options.IndexingOptions-com.groupdocs.search.common.IFieldExtractor-com.groupdocs.search.options.IOcrConnector-) | Initializes a new instance of the  ExtractionOptions  class. |
## Methods

| Method | Description |
| --- | --- |
| [getCustomExtractor()](#getCustomExtractor--) | Gets the custom text extractor. |
| [setCustomExtractor(IFieldExtractor value)](#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-) | Sets or sets the custom text extractor. |
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
### ExtractionOptions() {#ExtractionOptions--}
```
public ExtractionOptions()
```


Initializes a new instance of the  ExtractionOptions  class.

### ExtractionOptions(Object data) {#ExtractionOptions-java.lang.Object-}
```
public ExtractionOptions(Object data)
```


Initializes a new instance of the  ExtractionOptions  class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| data | java.lang.Object | The serialized data. |

### ExtractionOptions(IndexingOptions options, IFieldExtractor customExtractor, IOcrConnector ocrConnector) {#ExtractionOptions-com.groupdocs.search.options.IndexingOptions-com.groupdocs.search.common.IFieldExtractor-com.groupdocs.search.options.IOcrConnector-}
```
public ExtractionOptions(IndexingOptions options, IFieldExtractor customExtractor, IOcrConnector ocrConnector)
```


Initializes a new instance of the  ExtractionOptions  class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | The options. |
| customExtractor | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | The custom extractor. |
| ocrConnector | [IOcrConnector](../../com.groupdocs.search.options/iocrconnector) | The ocr connector. |

### getCustomExtractor() {#getCustomExtractor--}
```
public IFieldExtractor getCustomExtractor()
```


Gets the custom text extractor. The default value is  null .

**Returns:**
[IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) - The custom text extractor.
### setCustomExtractor(IFieldExtractor value) {#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-}
```
public void setCustomExtractor(IFieldExtractor value)
```


Sets or sets the custom text extractor. The default value is  null .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | The custom text extractor. |

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
