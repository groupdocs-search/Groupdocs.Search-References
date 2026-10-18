---
title: "ImageSearchOptions"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Menyediakan opsi untuk operasi pencarian gambar terbalik."
type: docs
weight: 24
url: /id/java/com.groupdocs.search.options/imagesearchoptions/
---
**Inheritance:**
java.lang.Object
```
public class ImageSearchOptions
```

Menyediakan opsi untuk operasi pencarian gambar terbalik.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [ImageSearchOptions()](#ImageSearchOptions--) | Menginisialisasi instance baru dari kelas  ImageSearchOptions  . |
|
|  | [ImageSearchOptions(Object data)](#ImageSearchOptions-java.lang.Object-) | Menginisialisasi instance baru dari kelas  ImageSearchOptions  . |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getHashDifferences()](#getHashDifferences--) | Mendapatkan jumlah maksimum bit yang tidak cocok dalam hash gambar. |
|
|  | [setHashDifferences(int value)](#setHashDifferences-int-) | Mengatur jumlah maksimum bit yang tidak cocok dalam hash gambar. |
|
|  | [getMaxResultCount()](#getMaxResultCount--) | Mendapatkan jumlah maksimum gambar yang ditemukan untuk permintaan pencarian balik gambar. |
|
|  | [setMaxResultCount(int value)](#setMaxResultCount-int-) | Mengatur jumlah maksimum gambar yang ditemukan untuk permintaan pencarian balik gambar. |
|
|  | [getSearchDocumentFilter()](#getSearchDocumentFilter--) | Mendapatkan filter dokumen pencarian. |
|
|  | [setSearchDocumentFilter(ISearchDocumentFilter value)](#setSearchDocumentFilter-com.groupdocs.search.options.ISearchDocumentFilter-) | Mendapatkan atau mengatur filter dokumen pencarian. |
|
| [getCore()](#getCore--) |  |
### ImageSearchOptions() {#ImageSearchOptions--}
```
public ImageSearchOptions()
```


Menginisialisasi instance baru dari kelas  ImageSearchOptions  .


### ImageSearchOptions(Object data) {#ImageSearchOptions-java.lang.Object-}
```
public ImageSearchOptions(Object data)
```


Menginisialisasi instance baru dari kelas  ImageSearchOptions  .


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | data | java.lang.Object | Data yang diserialkan. |
|

### getHashDifferences() {#getHashDifferences--}
```
public int getHashDifferences()
```


Mendapatkan jumlah maksimum bit yang tidak cocok dalam hash gambar. Nilai defaultnya adalah  5 .


**Returns:**
int - Jumlah maksimum bit yang tidak cocok dalam hash gambar.

### setHashDifferences(int value) {#setHashDifferences-int-}
```
public void setHashDifferences(int value)
```


Mengatur jumlah maksimum bit yang tidak cocok dalam hash gambar. Nilai default adalah 5.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | int | Jumlah maksimum bit yang tidak cocok dalam hash gambar. |
|

### getMaxResultCount() {#getMaxResultCount--}
```
public int getMaxResultCount()
```


Menampilkan jumlah maksimum gambar yang ditemukan untuk permintaan pencarian balik gambar. Nilai default adalah 1000.


**Returns:**
int - Jumlah maksimum gambar yang ditemukan untuk permintaan pencarian balik gambar.

### setMaxResultCount(int value) {#setMaxResultCount-int-}
```
public void setMaxResultCount(int value)
```


Mengatur jumlah maksimum gambar yang ditemukan untuk permintaan pencarian balik gambar. Nilai default adalah 1000.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | int | Jumlah maksimum gambar yang ditemukan untuk permintaan pencarian balik gambar. |
|

### getSearchDocumentFilter() {#getSearchDocumentFilter--}
```
public ISearchDocumentFilter getSearchDocumentFilter()
```


Menampilkan filter dokumen pencarian. SearchDocumentFilter bekerja dengan logika inklusi. Gunakan kelas GroupDocs.Search.Options.SearchDocumentFilter untuk membuat instance filter dokumen pencarian. Nilai default adalah null, yang berarti semua dokumen yang ditemukan akan dikembalikan.


**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - The search document filter.

### setSearchDocumentFilter(ISearchDocumentFilter value) {#setSearchDocumentFilter-com.groupdocs.search.options.ISearchDocumentFilter-}
```
public void setSearchDocumentFilter(ISearchDocumentFilter value)
```


Menampilkan atau mengatur filter dokumen pencarian. SearchDocumentFilter bekerja dengan logika inklusi. Gunakan kelas GroupDocs.Search.Options.SearchDocumentFilter untuk membuat instance filter dokumen pencarian. Nilai default adalah null, yang berarti semua dokumen yang ditemukan akan dikembalikan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | value | [ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) | Filter dokumen pencarian. |
|

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
