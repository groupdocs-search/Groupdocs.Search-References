---
title: "OcrContext"
second_title: "GroupDocs.Search for Java API Referansı"
description: "OCR işleme bağlamını temsil eder."
type: docs
weight: 30
url: /tr/java/com.groupdocs.search.options/ocrcontext/
---
**Inheritance:**
java.lang.Object
```
public class OcrContext
```

OCR işleme bağlamını temsil eder.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [OcrContext(InputStream imageStream, ImageLocation imageLocation, String imageFileExtension)](#OcrContext-java.io.InputStream-com.groupdocs.search.options.ImageLocation-java.lang.String-) | Yeni bir örnek başlatır |
OcrContext
sınıf.
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getImageStream()](#getImageStream--) | İşlenecek görüntüyü içeren akışı alır. |
|
|  | [getImageLocation()](#getImageLocation--) | Görüntünün konumunu alır. |
|
|  | [getImageFileExtension()](#getImageFileExtension--) | Görüntünün dosya uzantısını alır. |
|
### OcrContext(InputStream imageStream, ImageLocation imageLocation, String imageFileExtension) {#OcrContext-java.io.InputStream-com.groupdocs.search.options.ImageLocation-java.lang.String-}
```
public OcrContext(InputStream imageStream, ImageLocation imageLocation, String imageFileExtension)
```


Yeni bir örnek başlatır
OcrContext
sınıf.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | İşlenecek görüntüyü içeren akış. |
|
|  | imageLocation | [ImageLocation](../../com.groupdocs.search.options/imagelocation) | Görüntünün konumu. |
|
|  | imageFileExtension | java.lang.String | Görüntünün dosya uzantısı. |
|

### getImageStream() {#getImageStream--}
```
public final InputStream getImageStream()
```


İşlenecek görüntüyü içeren akışı alır.


**Returns:**
java.io.InputStream - İşlenecek görüntüyü içeren akış.

### getImageLocation() {#getImageLocation--}
```
public final ImageLocation getImageLocation()
```


Görüntünün konumunu alır.


**Returns:**
[ImageLocation](../../com.groupdocs.search.options/imagelocation) - The location of the image.

### getImageFileExtension() {#getImageFileExtension--}
```
public final String getImageFileExtension()
```


Görüntünün dosya uzantısını alır.
Bu değer, görüntünün türünü belirlemek için kullanılabilir.


**Returns:**
java.lang.String - Görüntünün dosya uzantısı.

