---
title: "ImageSearchResult"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili hasil pencarian gambar terbalik."
type: docs
weight: 17
url: /id/java/com.groupdocs.search.results/imagesearchresult/
---
**Inheritance:**
java.lang.Object
```
public abstract class ImageSearchResult
```

Mewakili hasil pencarian gambar terbalik.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [ImageSearchResult()](#ImageSearchResult--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getImageCount()](#getImageCount--) | Mendapatkan jumlah gambar yang ditemukan. |
|
|  | [getFoundImage(int index)](#getFoundImage-int-) | Mendapatkan gambar yang ditemukan berdasarkan indeks. |
|
### ImageSearchResult() {#ImageSearchResult--}
```
public ImageSearchResult()
```


### getImageCount() {#getImageCount--}
```
public abstract int getImageCount()
```


Mendapatkan jumlah gambar yang ditemukan.


**Returns:**
int - Jumlah gambar yang ditemukan.

### getFoundImage(int index) {#getFoundImage-int-}
```
public abstract FoundImageFrame getFoundImage(int index)
```


Mendapatkan gambar yang ditemukan berdasarkan indeks.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | indeks | int | Indeks gambar yang ditemukan. |
|

**Returns:**
[FoundImageFrame](../../com.groupdocs.search.results/foundimageframe) - The found image.

