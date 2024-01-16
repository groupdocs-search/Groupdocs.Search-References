---
title: ImageIndexingOptions
second_title: GroupDocs.Search for Java API Reference
description: Provides image indexing options for reverse image search.
type: docs
weight: 21
url: /java/com.groupdocs.search.options/imageindexingoptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class ImageIndexingOptions
```

Provides image indexing options for reverse image search.
## Constructors

| Constructor | Description |
| --- | --- |
| [ImageIndexingOptions()](#ImageIndexingOptions--) |  |
## Methods

| Method | Description |
| --- | --- |
| [getEnabledForSeparateImages()](#getEnabledForSeparateImages--) | Gets a value indicating whether to index separate image files. |
| [setEnabledForSeparateImages(boolean value)](#setEnabledForSeparateImages-boolean-) | Sets a value indicating whether to index separate image files. |
| [getEnabledForContainerItemImages()](#getEnabledForContainerItemImages--) | Gets a value indicating whether to index images that are items in a container (for example, images in a ZIP archive). |
| [setEnabledForContainerItemImages(boolean value)](#setEnabledForContainerItemImages-boolean-) | Sets a value indicating whether to index images that are items in a container (for example, images in a ZIP archive). |
| [getEnabledForEmbeddedImages()](#getEnabledForEmbeddedImages--) | Gets a value indicating whether to index embedded images (for example, images in a DOCX document). |
| [setEnabledForEmbeddedImages(boolean value)](#setEnabledForEmbeddedImages-boolean-) | Sets a value indicating whether to index embedded images (for example, images in a DOCX document). |
### ImageIndexingOptions() {#ImageIndexingOptions--}
```
public ImageIndexingOptions()
```


### getEnabledForSeparateImages() {#getEnabledForSeparateImages--}
```
public abstract boolean getEnabledForSeparateImages()
```


Gets a value indicating whether to index separate image files. The default value is  false .

**Returns:**
boolean - A value indicating whether to index separate image files.
### setEnabledForSeparateImages(boolean value) {#setEnabledForSeparateImages-boolean-}
```
public abstract void setEnabledForSeparateImages(boolean value)
```


Sets a value indicating whether to index separate image files. The default value is  false .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | A value indicating whether to index separate image files. |

### getEnabledForContainerItemImages() {#getEnabledForContainerItemImages--}
```
public abstract boolean getEnabledForContainerItemImages()
```


Gets a value indicating whether to index images that are items in a container (for example, images in a ZIP archive). The default value is  false .

**Returns:**
boolean - A value indicating whether to index images that are items in a container.
### setEnabledForContainerItemImages(boolean value) {#setEnabledForContainerItemImages-boolean-}
```
public abstract void setEnabledForContainerItemImages(boolean value)
```


Sets a value indicating whether to index images that are items in a container (for example, images in a ZIP archive). The default value is  false .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | A value indicating whether to index images that are items in a container. |

### getEnabledForEmbeddedImages() {#getEnabledForEmbeddedImages--}
```
public abstract boolean getEnabledForEmbeddedImages()
```


Gets a value indicating whether to index embedded images (for example, images in a DOCX document). The default value is  false .

**Returns:**
boolean - A value indicating whether to index embedded images.
### setEnabledForEmbeddedImages(boolean value) {#setEnabledForEmbeddedImages-boolean-}
```
public abstract void setEnabledForEmbeddedImages(boolean value)
```


Sets a value indicating whether to index embedded images (for example, images in a DOCX document). The default value is  false .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | A value indicating whether to index embedded images. |

