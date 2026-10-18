---
title: "ImageIndexingOptions"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Menyediakan opsi pengindeksan gambar untuk pencarian gambar terbalik."
type: docs
weight: 23
url: /id/java/com.groupdocs.search.options/imageindexingoptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class ImageIndexingOptions
```

Menyediakan opsi pengindeksan gambar untuk pencarian gambar terbalik.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [ImageIndexingOptions()](#ImageIndexingOptions--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getEnabledForSeparateImages()](#getEnabledForSeparateImages--) | Mendapatkan nilai yang menunjukkan apakah akan mengindeks file gambar terpisah. |
|
|  | [setEnabledForSeparateImages(boolean value)](#setEnabledForSeparateImages-boolean-) | Mengatur nilai yang menunjukkan apakah akan mengindeks file gambar terpisah. |
|
|  | [getEnabledForContainerItemImages()](#getEnabledForContainerItemImages--) | Mendapatkan nilai yang menunjukkan apakah akan mengindeks gambar yang merupakan item dalam sebuah kontainer (misalnya, gambar dalam arsip ZIP). |
|
|  | [setEnabledForContainerItemImages(boolean value)](#setEnabledForContainerItemImages-boolean-) | Mengatur nilai yang menunjukkan apakah akan mengindeks gambar yang merupakan item dalam sebuah kontainer (misalnya, gambar dalam arsip ZIP). |
|
|  | [getEnabledForEmbeddedImages()](#getEnabledForEmbeddedImages--) | Mendapatkan nilai yang menunjukkan apakah akan mengindeks gambar tersemat (misalnya, gambar dalam dokumen DOCX). |
|
|  | [setEnabledForEmbeddedImages(boolean value)](#setEnabledForEmbeddedImages-boolean-) | Mengatur nilai yang menunjukkan apakah akan mengindeks gambar tersemat (misalnya, gambar dalam dokumen DOCX). |
|
### ImageIndexingOptions() {#ImageIndexingOptions--}
```
public ImageIndexingOptions()
```


### getEnabledForSeparateImages() {#getEnabledForSeparateImages--}
```
public abstract boolean getEnabledForSeparateImages()
```


Mendapatkan nilai yang menunjukkan apakah akan mengindeks file gambar terpisah. Nilai default adalah  false .


**Returns:**
boolean - Nilai yang menunjukkan apakah akan mengindeks file gambar terpisah.

### setEnabledForSeparateImages(boolean value) {#setEnabledForSeparateImages-boolean-}
```
public abstract void setEnabledForSeparateImages(boolean value)
```


Mengatur nilai yang menunjukkan apakah akan mengindeks file gambar terpisah. Nilai default adalah  false .


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | boolean | Nilai yang menunjukkan apakah akan mengindeks file gambar terpisah. |
|

### getEnabledForContainerItemImages() {#getEnabledForContainerItemImages--}
```
public abstract boolean getEnabledForContainerItemImages()
```


Mendapatkan nilai yang menunjukkan apakah akan mengindeks gambar yang merupakan item dalam sebuah kontainer (misalnya, gambar dalam arsip ZIP). Nilai default adalah  false .


**Returns:**
boolean - Nilai yang menunjukkan apakah akan mengindeks gambar yang merupakan item dalam sebuah kontainer.

### setEnabledForContainerItemImages(boolean value) {#setEnabledForContainerItemImages-boolean-}
```
public abstract void setEnabledForContainerItemImages(boolean value)
```


Mengatur nilai yang menunjukkan apakah akan mengindeks gambar yang merupakan item dalam sebuah kontainer (misalnya, gambar dalam arsip ZIP). Nilai default adalah false.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | boolean | Nilai yang menunjukkan apakah akan mengindeks gambar yang merupakan item dalam sebuah kontainer. |
|

### getEnabledForEmbeddedImages() {#getEnabledForEmbeddedImages--}
```
public abstract boolean getEnabledForEmbeddedImages()
```


Mendapatkan nilai yang menunjukkan apakah akan mengindeks gambar tersemat (misalnya, gambar dalam dokumen DOCX). Nilai default adalah false.


**Returns:**
boolean - Nilai yang menunjukkan apakah akan mengindeks gambar tersemat.

### setEnabledForEmbeddedImages(boolean value) {#setEnabledForEmbeddedImages-boolean-}
```
public abstract void setEnabledForEmbeddedImages(boolean value)
```


Mengatur nilai yang menunjukkan apakah akan mengindeks gambar tersemat (misalnya, gambar dalam dokumen DOCX). Nilai default adalah false.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | boolean | Nilai yang menunjukkan apakah akan mengindeks gambar tersemat. |
|

