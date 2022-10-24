---
title: ExtractionOptions
second_title: GroupDocs.Search for Java API Reference
description: Provides options for extracting data from documents.
type: docs
weight: 16
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
## Methods

| Method | Description |
| --- | --- |
| [getCustomExtractor()](#getCustomExtractor--) | Gets or sets the custom text extractor. |
| [setCustomExtractor(IFieldExtractor value)](#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-) | Gets or sets the custom text extractor. |
| [getEncoding()](#getEncoding--) | Gets or sets the encoding used to extract from text documents. |
| [setEncoding(String value)](#setEncoding-java.lang.String-) | Gets or sets the encoding used to extract from text documents. |
| [getUseRawTextExtraction()](#getUseRawTextExtraction--) | Gets or sets a value indicating whether the raw mode is used for text extraction if possible. |
| [setUseRawTextExtraction(boolean value)](#setUseRawTextExtraction-boolean-) | Gets or sets a value indicating whether the raw mode is used for text extraction if possible. |
| [getMetadataIndexingOptions()](#getMetadataIndexingOptions--) | Gets the options for indexing metadata fields. |
| [getOcrIndexingOptions()](#getOcrIndexingOptions--) | Gets the options for OCR processing and indexing recognized text. |
| [getImageIndexingOptions()](#getImageIndexingOptions--) | Gets the image indexing options for reverse image search. |
### ExtractionOptions() {#ExtractionOptions--}
```
public ExtractionOptions()
```


Initializes a new instance of the  ExtractionOptions  class.

### getCustomExtractor() {#getCustomExtractor--}
```
public final IFieldExtractor getCustomExtractor()
```


Gets or sets the custom text extractor. The default value is  null .

Value: The custom text extractor.

**Returns:**
[IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor)
### setCustomExtractor(IFieldExtractor value) {#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-}
```
public final void setCustomExtractor(IFieldExtractor value)
```


Gets or sets the custom text extractor. The default value is  null .

Value: The custom text extractor.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) |  |

### getEncoding() {#getEncoding--}
```
public final String getEncoding()
```


Gets or sets the encoding used to extract from text documents.

Value: The encoding used to extract from text documents.

**Returns:**
java.lang.String
### setEncoding(String value) {#setEncoding-java.lang.String-}
```
public final void setEncoding(String value)
```


Gets or sets the encoding used to extract from text documents.

Value: The encoding used to extract from text documents.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### getUseRawTextExtraction() {#getUseRawTextExtraction--}
```
public final boolean getUseRawTextExtraction()
```


Gets or sets a value indicating whether the raw mode is used for text extraction if possible. The default value is  true . The raw mode can significantly increase the indexing speed, but normal mode improves the formatting of the extracted text.

Value: A value indicating whether the raw mode is used for text extraction if possible.

**Returns:**
boolean
### setUseRawTextExtraction(boolean value) {#setUseRawTextExtraction-boolean-}
```
public final void setUseRawTextExtraction(boolean value)
```


Gets or sets a value indicating whether the raw mode is used for text extraction if possible. The default value is  true . The raw mode can significantly increase the indexing speed, but normal mode improves the formatting of the extracted text.

Value: A value indicating whether the raw mode is used for text extraction if possible.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### getMetadataIndexingOptions() {#getMetadataIndexingOptions--}
```
public final MetadataIndexingOptions getMetadataIndexingOptions()
```


Gets the options for indexing metadata fields.

Value: The options for indexing metadata fields.

**Returns:**
[MetadataIndexingOptions](../../com.groupdocs.search.options/metadataindexingoptions)
### getOcrIndexingOptions() {#getOcrIndexingOptions--}
```
public final OcrIndexingOptions getOcrIndexingOptions()
```


Gets the options for OCR processing and indexing recognized text.

Value: The options for OCR processing and indexing recognized text.

**Returns:**
[OcrIndexingOptions](../../com.groupdocs.search.options/ocrindexingoptions)
### getImageIndexingOptions() {#getImageIndexingOptions--}
```
public final ImageIndexingOptions getImageIndexingOptions()
```


Gets the image indexing options for reverse image search.

Value: The image indexing options for reverse image search.

**Returns:**
[ImageIndexingOptions](../../com.groupdocs.search.options/imageindexingoptions)
