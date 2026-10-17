---
title: "OcrContext"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل سياق معالجة OCR."
type: docs
weight: 30
url: /ar/java/com.groupdocs.search.options/ocrcontext/
---
**Inheritance:**
java.lang.Object
```
public class OcrContext
```

يمثل سياق معالجة OCR.

## المنشئات

| منشئ | الوصف |
| --- | --- |
|  | [OcrContext(InputStream imageStream, ImageLocation imageLocation, String imageFileExtension)](#OcrContext-java.io.InputStream-com.groupdocs.search.options.ImageLocation-java.lang.String-) | يُنشئ مثيلاً جديدًا لـ |
OcrContext
الفئة.
|
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getImageStream()](#getImageStream--) | يسترجع الدفق الذي يحتوي على الصورة التي سيتم معالجتها. |
|
|  | [getImageLocation()](#getImageLocation--) | يسترجع موقع الصورة. |
|
|  | [getImageFileExtension()](#getImageFileExtension--) | يسترجع امتداد ملف الصورة. |
|
### OcrContext(InputStream imageStream, ImageLocation imageLocation, String imageFileExtension) {#OcrContext-java.io.InputStream-com.groupdocs.search.options.ImageLocation-java.lang.String-}
```
public OcrContext(InputStream imageStream, ImageLocation imageLocation, String imageFileExtension)
```


يُنشئ مثيلاً جديدًا لـ
OcrContext
الفئة.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | الدفق الذي يحتوي على الصورة التي سيتم معالجتها. |
|
|  | imageLocation | [ImageLocation](../../com.groupdocs.search.options/imagelocation) | موقع الصورة. |
|
|  | imageFileExtension | java.lang.String | امتداد ملف الصورة. |
|

### getImageStream() {#getImageStream--}
```
public final InputStream getImageStream()
```


يسترجع الدفق الذي يحتوي على الصورة التي سيتم معالجتها.


**Returns:**
java.io.InputStream - الدفق الذي يحتوي على الصورة التي سيتم معالجتها.

### getImageLocation() {#getImageLocation--}
```
public final ImageLocation getImageLocation()
```


يسترجع موقع الصورة.


**Returns:**
[ImageLocation](../../com.groupdocs.search.options/imagelocation) - The location of the image.

### getImageFileExtension() {#getImageFileExtension--}
```
public final String getImageFileExtension()
```


يسترجع امتداد ملف الصورة.
يمكن استخدام هذه القيمة لتحديد نوع الصورة.


**Returns:**
java.lang.String - امتداد ملف الصورة.

