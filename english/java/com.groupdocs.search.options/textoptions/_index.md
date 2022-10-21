---
title: TextOptions
second_title: GroupDocs.Search for Java API Reference
description: Provides options for retrieving document text from an index.
type: docs
weight: 37
url: /java/com.groupdocs.search.options/textoptions/
---
**Inheritance:**
java.lang.Object
```
public class TextOptions
```

Provides options for retrieving document text from an index.

**Learn more**

 *  [Getting indexed documents][]
 *  [Highlighting search results][]


[Getting indexed documents]: https://docs.groupdocs.com/display/searchjava/Getting+indexed+documents
[Highlighting search results]: https://docs.groupdocs.com/display/searchjava/Highlighting+search+results
## Constructors

| Constructor | Description |
| --- | --- |
| [TextOptions()](#TextOptions--) | Initializes a new instance of the  TextOptions  class. |
## Methods

| Method | Description |
| --- | --- |
| [getCustomExtractor()](#getCustomExtractor--) | Gets the custom text extractor that was used for indexing. |
| [setCustomExtractor(IFieldExtractor value)](#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-) | Sets the custom text extractor that was used for indexing. |
| [getAdditionalFields()](#getAdditionalFields--) | Gets the additional document fields that was used for indexing. |
| [setAdditionalFields(DocumentField[] value)](#setAdditionalFields-com.groupdocs.search.common.DocumentField---) | Sets the additional document fields that was used for indexing. |
| [getCancellation()](#getCancellation--) | Gets the cancellation object. |
| [setCancellation(Cancellation value)](#setCancellation-com.groupdocs.search.common.Cancellation-) | Sets the cancellation object. |
| [getGenerateHead()](#getGenerateHead--) | Gets a value indicating whether the Head tag is generated in the output HTML. |
| [setGenerateHead(boolean value)](#setGenerateHead-boolean-) | Sets a value indicating whether the Head tag is generated in the output HTML. |
| [getMetadataIndexingOptions()](#getMetadataIndexingOptions--) | Gets the options for indexing metadata fields. |
| [getOcrIndexingOptions()](#getOcrIndexingOptions--) | Gets the options for OCR processing and indexing recognized text. |
| [getImageIndexingOptions()](#getImageIndexingOptions--) | Gets the image indexing options for reverse image search. |
### TextOptions() {#TextOptions--}
```
public TextOptions()
```


Initializes a new instance of the  TextOptions  class.

### getCustomExtractor() {#getCustomExtractor--}
```
public final IFieldExtractor getCustomExtractor()
```


Gets the custom text extractor that was used for indexing. The default value is  null . Note that this value is used only if document text was not saved into the index.

**Returns:**
[IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) - The custom text extractor that was used for indexing.
### setCustomExtractor(IFieldExtractor value) {#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-}
```
public final void setCustomExtractor(IFieldExtractor value)
```


Sets the custom text extractor that was used for indexing. The default value is  null . Note that this value is used only if document text was not saved into the index.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | The custom text extractor that was used for indexing. |

### getAdditionalFields() {#getAdditionalFields--}
```
public final DocumentField[] getAdditionalFields()
```


Gets the additional document fields that was used for indexing. The default value is  null . Note that this value is used only if document text was not saved into the index.

**Returns:**
com.groupdocs.search.common.DocumentField[] - The additional document fields that was used for indexing.
### setAdditionalFields(DocumentField[] value) {#setAdditionalFields-com.groupdocs.search.common.DocumentField---}
```
public final void setAdditionalFields(DocumentField[] value)
```


Sets the additional document fields that was used for indexing. The default value is  null . Note that this value is used only if document text was not saved into the index.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | The additional document fields that was used for indexing. |

### getCancellation() {#getCancellation--}
```
public final Cancellation getCancellation()
```


Gets the cancellation object. The default value is  null .

**Returns:**
[Cancellation](../../com.groupdocs.search.common/cancellation) - The cancellation object.
### setCancellation(Cancellation value) {#setCancellation-com.groupdocs.search.common.Cancellation-}
```
public final void setCancellation(Cancellation value)
```


Sets the cancellation object. The default value is  null .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Cancellation](../../com.groupdocs.search.common/cancellation) | The cancellation object. |

### getGenerateHead() {#getGenerateHead--}
```
public final boolean getGenerateHead()
```


Gets a value indicating whether the Head tag is generated in the output HTML. The default value is  true .

**Returns:**
boolean - A value indicating whether the Head tag is generated in the output HTML.
### setGenerateHead(boolean value) {#setGenerateHead-boolean-}
```
public final void setGenerateHead(boolean value)
```


Sets a value indicating whether the Head tag is generated in the output HTML. The default value is  true .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | A value indicating whether the Head tag is generated in the output HTML. |

### getMetadataIndexingOptions() {#getMetadataIndexingOptions--}
```
public final MetadataIndexingOptions getMetadataIndexingOptions()
```


Gets the options for indexing metadata fields.

**Returns:**
[MetadataIndexingOptions](../../com.groupdocs.search.options/metadataindexingoptions) - The options for indexing metadata fields.
### getOcrIndexingOptions() {#getOcrIndexingOptions--}
```
public final OcrIndexingOptions getOcrIndexingOptions()
```


Gets the options for OCR processing and indexing recognized text.

**Returns:**
[OcrIndexingOptions](../../com.groupdocs.search.options/ocrindexingoptions) - The options for OCR processing and indexing recognized text.
### getImageIndexingOptions() {#getImageIndexingOptions--}
```
public final ImageIndexingOptions getImageIndexingOptions()
```


Gets the image indexing options for reverse image search.

**Returns:**
[ImageIndexingOptions](../../com.groupdocs.search.options/imageindexingoptions) - The image indexing options for reverse image search.
