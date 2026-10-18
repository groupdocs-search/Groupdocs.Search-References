---
title: "OcrContext"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili konteks pemrosesan OCR."
type: docs
weight: 30
url: /id/java/com.groupdocs.search.options/ocrcontext/
---
**Inheritance:**
java.lang.Object
```
public class OcrContext
```

Mewakili konteks pemrosesan OCR.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [OcrContext(InputStream imageStream, ImageLocation imageLocation, String imageFileExtension)](#OcrContext-java.io.InputStream-com.groupdocs.search.options.ImageLocation-java.lang.String-) | Menginisialisasi instance baru dari |
OcrContext
kelas.
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getImageStream()](#getImageStream--) | Mendapatkan aliran yang berisi gambar yang akan diproses. |
|
|  | [getImageLocation()](#getImageLocation--) | Mendapatkan lokasi gambar. |
|
|  | [getImageFileExtension()](#getImageFileExtension--) | Mendapatkan ekstensi file gambar. |
|
### OcrContext(InputStream imageStream, ImageLocation imageLocation, String imageFileExtension) {#OcrContext-java.io.InputStream-com.groupdocs.search.options.ImageLocation-java.lang.String-}
```
public OcrContext(InputStream imageStream, ImageLocation imageLocation, String imageFileExtension)
```


Menginisialisasi instance baru dari
OcrContext
kelas.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | Aliran yang berisi gambar yang akan diproses. |
|
|  | imageLocation | [ImageLocation](../../com.groupdocs.search.options/imagelocation) | Lokasi gambar. |
|
|  | imageFileExtension | java.lang.String | Ekstensi file gambar. |
|

### getImageStream() {#getImageStream--}
```
public final InputStream getImageStream()
```


Mendapatkan aliran yang berisi gambar yang akan diproses.


**Returns:**
java.io.InputStream - Aliran yang berisi gambar yang akan diproses.

### getImageLocation() {#getImageLocation--}
```
public final ImageLocation getImageLocation()
```


Mendapatkan lokasi gambar.


**Returns:**
[ImageLocation](../../com.groupdocs.search.options/imagelocation) - The location of the image.

### getImageFileExtension() {#getImageFileExtension--}
```
public final String getImageFileExtension()
```


Mendapatkan ekstensi file gambar.
Nilai ini dapat digunakan untuk menentukan tipe gambar.


**Returns:**
java.lang.String - Ekstensi file gambar.

