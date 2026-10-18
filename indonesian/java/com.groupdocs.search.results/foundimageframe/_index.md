---
title: "FoundImageFrame"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili bingkai gambar yang ditemukan."
type: docs
weight: 16
url: /id/java/com.groupdocs.search.results/foundimageframe/
---
**Inheritance:**
java.lang.Object
```
public abstract class FoundImageFrame
```

Mewakili bingkai gambar yang ditemukan.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [FoundImageFrame()](#FoundImageFrame--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getDocumentInfo()](#getDocumentInfo--) | Mendapatkan info dokumen. |
|
|  | [getImageIndex()](#getImageIndex--) | Mendapatkan nomor urut gambar dalam dokumen. |
|
|  | [getFrameIndex()](#getFrameIndex--) | Mendapatkan indeks bingkai dalam gambar. |
|
|  | [getHashDifferences()](#getHashDifferences--) | Mendapatkan jumlah bit yang tidak cocok dalam hash gambar. |
|
|  | [toString()](#toString--) | Mengembalikan sebuah System.String yang mewakili FoundImageFrame saat ini. |
|
### FoundImageFrame() {#FoundImageFrame--}
```
public FoundImageFrame()
```


### getDocumentInfo() {#getDocumentInfo--}
```
public abstract DocumentInfo getDocumentInfo()
```


Mendapatkan info dokumen.


**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - The document info.

### getImageIndex() {#getImageIndex--}
```
public abstract int getImageIndex()
```


Mendapatkan nomor urut gambar dalam dokumen.


**Returns:**
int - Nomor urut gambar dalam dokumen.

### getFrameIndex() {#getFrameIndex--}
```
public abstract int getFrameIndex()
```


Mendapatkan indeks bingkai dalam gambar.


**Returns:**
int - Indeks bingkai dalam gambar.

### getHashDifferences() {#getHashDifferences--}
```
public abstract int getHashDifferences()
```


Mendapatkan jumlah bit yang tidak cocok dalam hash gambar.


**Returns:**
int - Jumlah bit yang tidak cocok dalam hash gambar.

### toString() {#toString--}
```
public abstract String toString()
```


Mengembalikan sebuah System.String yang mewakili FoundImageFrame saat ini.


**Returns:**
java.lang.String - Sebuah System.String yang mewakili FoundImageFrame saat ini.

