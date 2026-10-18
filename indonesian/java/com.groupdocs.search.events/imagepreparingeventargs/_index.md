---
title: "ImagePreparingEventArgs"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili argumen untuk peristiwa ketika persiapan gambar dimulai."
type: docs
weight: 15
url: /id/java/com.groupdocs.search.events/imagepreparingeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class ImagePreparingEventArgs extends BaseIndexEventArgs
```

Mewakili argumen untuk peristiwa ketika persiapan gambar dimulai.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getDocumentKey()](#getDocumentKey--) | Mendapatkan kunci dokumen. |
|
|  | [getInnerPath()](#getInnerPath--) | Mendapatkan jalur dalam dari dokumen bersarang. |
|
|  | [getImageIndex()](#getImageIndex--) | Mendapatkan nomor urut gambar dalam dokumen. |
|
|  | [getImageFrames()](#getImageFrames--) | Mendapatkan frame gambar. |
|
|  | [getImageStream()](#getImageStream--) | Mendapatkan aliran gambar. |
|
### getDocumentKey() {#getDocumentKey--}
```
public final String getDocumentKey()
```


Mendapatkan kunci dokumen.


**Returns:**
java.lang.String - Kunci dokumen.

### getInnerPath() {#getInnerPath--}
```
public final String[] getInnerPath()
```


Mendapatkan jalur dalam dari dokumen bersarang.


**Returns:**
java.lang.String[] - Jalur dalam dari dokumen bersarang.

### getImageIndex() {#getImageIndex--}
```
public final int getImageIndex()
```


Mendapatkan nomor urut gambar dalam dokumen.


**Returns:**
int - Nomor urut gambar dalam dokumen.

### getImageFrames() {#getImageFrames--}
```
public final ImageFrame[] getImageFrames()
```


Mendapatkan frame gambar.


**Returns:**
com.groupdocs.search.common.ImageFrame[] - Frame gambar.

### getImageStream() {#getImageStream--}
```
public final InputStream getImageStream()
```


Mendapatkan aliran gambar.


**Returns:**
java.io.InputStream - Aliran gambar.

