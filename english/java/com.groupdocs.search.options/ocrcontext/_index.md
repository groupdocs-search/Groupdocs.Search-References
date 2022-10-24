---
title: OcrContext
second_title: GroupDocs.Search for Java API Reference
description: Represents the OCR processing context.
type: docs
weight: 28
url: /java/com.groupdocs.search.options/ocrcontext/
---
**Inheritance:**
java.lang.Object
```
public class OcrContext
```

Represents the OCR processing context.
## Constructors

| Constructor | Description |
| --- | --- |
| [OcrContext(InputStream imageStream, ImageLocation imageLocation, String imageFileExtension)](#OcrContext-java.io.InputStream-com.groupdocs.search.options.ImageLocation-java.lang.String-) | Initializes a new instance of the  OcrContext  class. |
## Methods

| Method | Description |
| --- | --- |
| [getImageStream()](#getImageStream--) | Gets the stream containing the image to be processed. |
| [getImageLocation()](#getImageLocation--) | Gets the location of the image. |
| [getImageFileExtension()](#getImageFileExtension--) | Gets the file extension of the image. |
### OcrContext(InputStream imageStream, ImageLocation imageLocation, String imageFileExtension) {#OcrContext-java.io.InputStream-com.groupdocs.search.options.ImageLocation-java.lang.String-}
```
public OcrContext(InputStream imageStream, ImageLocation imageLocation, String imageFileExtension)
```


Initializes a new instance of the  OcrContext  class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| imageStream | java.io.InputStream | The stream containing the image to be processed. |
| imageLocation | [ImageLocation](../../com.groupdocs.search.options/imagelocation) | The location of the image. |
| imageFileExtension | java.lang.String | The file extension of the image. |

### getImageStream() {#getImageStream--}
```
public final InputStream getImageStream()
```


Gets the stream containing the image to be processed.

**Returns:**
java.io.InputStream - The stream containing the image to be processed.
### getImageLocation() {#getImageLocation--}
```
public final ImageLocation getImageLocation()
```


Gets the location of the image.

**Returns:**
[ImageLocation](../../com.groupdocs.search.options/imagelocation) - The location of the image.
### getImageFileExtension() {#getImageFileExtension--}
```
public final String getImageFileExtension()
```


Gets the file extension of the image. This value can be used to determine the type of the image.

**Returns:**
java.lang.String - The file extension of the image.
