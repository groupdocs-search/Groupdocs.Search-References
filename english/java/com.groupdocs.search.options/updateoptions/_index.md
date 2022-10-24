---
title: UpdateOptions
second_title: GroupDocs.Search for Java API Reference
description: Provides options for update operation.
type: docs
weight: 39
url: /java/com.groupdocs.search.options/updateoptions/
---
**Inheritance:**
java.lang.Object
```
public class UpdateOptions
```

Provides options for update operation.

**Learn more**

 *  [Update index][]
 *  [Delete indexed paths][]


[Update index]: https://docs.groupdocs.com/display/searchjava/Update+index
[Delete indexed paths]: https://docs.groupdocs.com/display/searchjava/Delete+indexed+paths
## Constructors

| Constructor | Description |
| --- | --- |
| [UpdateOptions()](#UpdateOptions--) | Initializes a new instance of the  UpdateOptions  class. |
## Methods

| Method | Description |
| --- | --- |
| [getThreads()](#getThreads--) | Gets the number of threads used for indexing. |
| [setThreads(int value)](#setThreads-int-) | Sets the number of threads used for indexing. |
| [isAsync()](#isAsync--) | Gets the flag of asynchronous performing the operation. |
| [setAsync(boolean value)](#setAsync-boolean-) | Sets the flag of asynchronous performing the operation. |
| [getCancellation()](#getCancellation--) | Gets the operation cancellation object. |
| [setCancellation(Cancellation value)](#setCancellation-com.groupdocs.search.common.Cancellation-) | Sets the operation cancellation object. |
| [getMetadataIndexingOptions()](#getMetadataIndexingOptions--) | Gets the options for indexing metadata fields. |
| [getOcrIndexingOptions()](#getOcrIndexingOptions--) | Gets the options for OCR processing and indexing recognized text. |
| [getImageIndexingOptions()](#getImageIndexingOptions--) | Gets the image indexing options for reverse image search. |
### UpdateOptions() {#UpdateOptions--}
```
public UpdateOptions()
```


Initializes a new instance of the  UpdateOptions  class.

### getThreads() {#getThreads--}
```
public final int getThreads()
```


Gets the number of threads used for indexing. The default value is  1 .

**Returns:**
int - The number of threads used for indexing.
### setThreads(int value) {#setThreads-int-}
```
public final void setThreads(int value)
```


Sets the number of threads used for indexing. The default value is  1 .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | The number of threads used for indexing. |

### isAsync() {#isAsync--}
```
public final boolean isAsync()
```


Gets the flag of asynchronous performing the operation. The default value is  false .

**Returns:**
boolean - The flag of asynchronous performing the operation.
### setAsync(boolean value) {#setAsync-boolean-}
```
public final void setAsync(boolean value)
```


Sets the flag of asynchronous performing the operation. The default value is  false .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The flag of asynchronous performing the operation. |

### getCancellation() {#getCancellation--}
```
public final Cancellation getCancellation()
```


Gets the operation cancellation object. The default value is  null .

**Returns:**
[Cancellation](../../com.groupdocs.search.common/cancellation) - The operation cancellation object.
### setCancellation(Cancellation value) {#setCancellation-com.groupdocs.search.common.Cancellation-}
```
public final void setCancellation(Cancellation value)
```


Sets the operation cancellation object. The default value is  null .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Cancellation](../../com.groupdocs.search.common/cancellation) | The operation cancellation object. |

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
