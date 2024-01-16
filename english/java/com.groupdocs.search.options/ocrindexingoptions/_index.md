---
title: OcrIndexingOptions
second_title: GroupDocs.Search for Java API Reference
description: Provides options for OCR processing and indexing recognized text.
type: docs
weight: 29
url: /java/com.groupdocs.search.options/ocrindexingoptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class OcrIndexingOptions
```

Provides options for OCR processing and indexing recognized text.
## Constructors

| Constructor | Description |
| --- | --- |
| [OcrIndexingOptions()](#OcrIndexingOptions--) |  |
## Methods

| Method | Description |
| --- | --- |
| [getEnabledForSeparateImages()](#getEnabledForSeparateImages--) | Gets a value indicating whether to recognize text in separate image files. |
| [setEnabledForSeparateImages(boolean value)](#setEnabledForSeparateImages-boolean-) | Sets a value indicating whether to recognize text in separate image files. |
| [getEnabledForContainerItemImages()](#getEnabledForContainerItemImages--) | Gets a value indicating whether to recognize text in images that are items in a container (for example, images in a ZIP archive). |
| [setEnabledForContainerItemImages(boolean value)](#setEnabledForContainerItemImages-boolean-) | Sets a value indicating whether to recognize text in images that are items in a container (for example, images in a ZIP archive). |
| [getEnabledForEmbeddedImages()](#getEnabledForEmbeddedImages--) | Gets a value indicating whether to recognize text in embedded images (for example, images in a DOCX document). |
| [setEnabledForEmbeddedImages(boolean value)](#setEnabledForEmbeddedImages-boolean-) | Sets a value indicating whether to recognize text in embedded images (for example, images in a DOCX document). |
| [getOcrConnector()](#getOcrConnector--) | Gets an OCR connector that is used for OCR processing. |
| [setOcrConnector(IOcrConnector value)](#setOcrConnector-com.groupdocs.search.options.IOcrConnector-) | Sets an OCR connector that is used for OCR processing. |
### OcrIndexingOptions() {#OcrIndexingOptions--}
```
public OcrIndexingOptions()
```


### getEnabledForSeparateImages() {#getEnabledForSeparateImages--}
```
public abstract boolean getEnabledForSeparateImages()
```


Gets a value indicating whether to recognize text in separate image files. The default value is  false .

**Returns:**
boolean - A value indicating whether to recognize text in separate image files.
### setEnabledForSeparateImages(boolean value) {#setEnabledForSeparateImages-boolean-}
```
public abstract void setEnabledForSeparateImages(boolean value)
```


Sets a value indicating whether to recognize text in separate image files. The default value is  false .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | A value indicating whether to recognize text in separate image files. |

### getEnabledForContainerItemImages() {#getEnabledForContainerItemImages--}
```
public abstract boolean getEnabledForContainerItemImages()
```


Gets a value indicating whether to recognize text in images that are items in a container (for example, images in a ZIP archive). The default value is  false .

**Returns:**
boolean - A value indicating whether to recognize text in images that are items in a container.
### setEnabledForContainerItemImages(boolean value) {#setEnabledForContainerItemImages-boolean-}
```
public abstract void setEnabledForContainerItemImages(boolean value)
```


Sets a value indicating whether to recognize text in images that are items in a container (for example, images in a ZIP archive). The default value is  false .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | A value indicating whether to recognize text in images that are items in a container. |

### getEnabledForEmbeddedImages() {#getEnabledForEmbeddedImages--}
```
public abstract boolean getEnabledForEmbeddedImages()
```


Gets a value indicating whether to recognize text in embedded images (for example, images in a DOCX document). The default value is  false .

**Returns:**
boolean - A value indicating whether to recognize text in embedded images.
### setEnabledForEmbeddedImages(boolean value) {#setEnabledForEmbeddedImages-boolean-}
```
public abstract void setEnabledForEmbeddedImages(boolean value)
```


Sets a value indicating whether to recognize text in embedded images (for example, images in a DOCX document). The default value is  false .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | A value indicating whether to recognize text in embedded images. |

### getOcrConnector() {#getOcrConnector--}
```
public abstract IOcrConnector getOcrConnector()
```


Gets an OCR connector that is used for OCR processing. The default value is  null , which means no OCR is used.

**Returns:**
[IOcrConnector](../../com.groupdocs.search.options/iocrconnector) - An OCR connector that is used for OCR processing.
### setOcrConnector(IOcrConnector value) {#setOcrConnector-com.groupdocs.search.options.IOcrConnector-}
```
public abstract void setOcrConnector(IOcrConnector value)
```


Sets an OCR connector that is used for OCR processing. The default value is  null , which means no OCR is used.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IOcrConnector](../../com.groupdocs.search.options/iocrconnector) | An OCR connector that is used for OCR processing. |

