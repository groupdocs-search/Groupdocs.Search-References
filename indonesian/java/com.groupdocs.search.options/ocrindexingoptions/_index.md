---
title: "OcrIndexingOptions"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Menyediakan opsi untuk pemrosesan OCR dan pengindeksan teks yang dikenali."
type: docs
weight: 31
url: /id/java/com.groupdocs.search.options/ocrindexingoptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class OcrIndexingOptions
```

Menyediakan opsi untuk pemrosesan OCR dan pengindeksan teks yang dikenali.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [OcrIndexingOptions()](#OcrIndexingOptions--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getEnabledForSeparateImages()](#getEnabledForSeparateImages--) | Mendapatkan nilai yang menunjukkan apakah mengenali teks dalam file gambar terpisah. |
|
|  | [setEnabledForSeparateImages(boolean value)](#setEnabledForSeparateImages-boolean-) | Mengatur nilai yang menunjukkan apakah mengenali teks dalam file gambar terpisah. |
|
|  | [getEnabledForContainerItemImages()](#getEnabledForContainerItemImages--) | Mendapatkan nilai yang menunjukkan apakah mengenali teks dalam gambar yang merupakan item dalam sebuah kontainer (misalnya, gambar dalam arsip ZIP). |
|
|  | [setEnabledForContainerItemImages(boolean value)](#setEnabledForContainerItemImages-boolean-) | Mengatur nilai yang menunjukkan apakah mengenali teks dalam gambar yang merupakan item dalam sebuah kontainer (misalnya, gambar dalam arsip ZIP). |
|
|  | [getEnabledForEmbeddedImages()](#getEnabledForEmbeddedImages--) | Mendapatkan nilai yang menunjukkan apakah mengenali teks dalam gambar tersemat (misalnya, gambar dalam dokumen DOCX). |
|
|  | [setEnabledForEmbeddedImages(boolean value)](#setEnabledForEmbeddedImages-boolean-) | Mengatur nilai yang menunjukkan apakah mengenali teks dalam gambar tersemat (misalnya, gambar dalam dokumen DOCX). |
|
|  | [getOcrConnector()](#getOcrConnector--) | Mendapatkan konektor OCR yang digunakan untuk pemrosesan OCR. |
|
|  | [setOcrConnector(IOcrConnector value)](#setOcrConnector-com.groupdocs.search.options.IOcrConnector-) | Mengatur konektor OCR yang digunakan untuk pemrosesan OCR. |
|
### OcrIndexingOptions() {#OcrIndexingOptions--}
```
public OcrIndexingOptions()
```


### getEnabledForSeparateImages() {#getEnabledForSeparateImages--}
```
public abstract boolean getEnabledForSeparateImages()
```


Mendapatkan nilai yang menunjukkan apakah mengenali teks dalam file gambar terpisah. Nilai default adalah  false .


**Returns:**
boolean - Nilai yang menunjukkan apakah mengenali teks dalam file gambar terpisah.

### setEnabledForSeparateImages(boolean value) {#setEnabledForSeparateImages-boolean-}
```
public abstract void setEnabledForSeparateImages(boolean value)
```


Mengatur nilai yang menunjukkan apakah mengenali teks dalam file gambar terpisah. Nilai default adalah  false .


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | boolean | Nilai yang menunjukkan apakah mengenali teks dalam file gambar terpisah. |
|

### getEnabledForContainerItemImages() {#getEnabledForContainerItemImages--}
```
public abstract boolean getEnabledForContainerItemImages()
```


Mendapatkan nilai yang menunjukkan apakah mengenali teks dalam gambar yang merupakan item dalam sebuah kontainer (misalnya, gambar dalam arsip ZIP). Nilai default adalah  false .


**Returns:**
boolean - Nilai yang menunjukkan apakah mengenali teks dalam gambar yang merupakan item dalam sebuah kontainer.

### setEnabledForContainerItemImages(boolean value) {#setEnabledForContainerItemImages-boolean-}
```
public abstract void setEnabledForContainerItemImages(boolean value)
```


Mengatur nilai yang menunjukkan apakah mengenali teks dalam gambar yang merupakan item dalam sebuah kontainer (misalnya, gambar dalam arsip ZIP). Nilai default adalah  false .


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | boolean | Nilai yang menunjukkan apakah mengenali teks dalam gambar yang merupakan item dalam sebuah kontainer. |
|

### getEnabledForEmbeddedImages() {#getEnabledForEmbeddedImages--}
```
public abstract boolean getEnabledForEmbeddedImages()
```


Mendapatkan nilai yang menunjukkan apakah mengenali teks dalam gambar tersemat (misalnya, gambar dalam dokumen DOCX). Nilai default adalah  false .


**Returns:**
boolean - Nilai yang menunjukkan apakah mengenali teks dalam gambar tersemat.

### setEnabledForEmbeddedImages(boolean value) {#setEnabledForEmbeddedImages-boolean-}
```
public abstract void setEnabledForEmbeddedImages(boolean value)
```


Mengatur nilai yang menunjukkan apakah mengenali teks dalam gambar tersemat (misalnya, gambar dalam dokumen DOCX). Nilai default adalah  false .


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | boolean | Nilai yang menunjukkan apakah mengenali teks dalam gambar tersemat. |
|

### getOcrConnector() {#getOcrConnector--}
```
public abstract IOcrConnector getOcrConnector()
```


Mendapatkan konektor OCR yang digunakan untuk pemrosesan OCR. Nilai default adalah  null , yang berarti tidak ada OCR yang digunakan.


**Returns:**
[IOcrConnector](../../com.groupdocs.search.options/iocrconnector) - An OCR connector that is used for OCR processing.

### setOcrConnector(IOcrConnector value) {#setOcrConnector-com.groupdocs.search.options.IOcrConnector-}
```
public abstract void setOcrConnector(IOcrConnector value)
```


Mengatur konektor OCR yang digunakan untuk pemrosesan OCR. Nilai default adalah  null , yang berarti tidak ada OCR yang digunakan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | value | [IOcrConnector](../../com.groupdocs.search.options/iocrconnector) | Sebuah konektor OCR yang digunakan untuk pemrosesan OCR. |
|

