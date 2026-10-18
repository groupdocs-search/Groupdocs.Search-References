---
title: "SearchImage"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili gambar untuk pencarian."
type: docs
weight: 29
url: /id/java/com.groupdocs.search.common/searchimage/
---
**Inheritance:**
java.lang.Object
```
public abstract class SearchImage
```

Mewakili gambar untuk pencarian.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [SearchImage()](#SearchImage--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [create(String filePath)](#create-java.lang.String-) | Membuat gambar dari file untuk pencarian. |
|
|  | [create(String filePath, int imageIndex)](#create-java.lang.String-int-) | Membuat gambar dari file untuk pencarian. |
|
|  | [create(InputStream stream)](#create-java.io.InputStream-) | Membuat gambar dari aliran untuk pencarian. |
|
|  | [create(InputStream stream, int imageIndex)](#create-java.io.InputStream-int-) | Membuat gambar dari aliran untuk pencarian. |
|
### SearchImage() {#SearchImage--}
```
public SearchImage()
```


### create(String filePath) {#create-java.lang.String-}
```
public static SearchImage create(String filePath)
```


Membuat gambar dari file untuk pencarian.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | filePath | java.lang.String | Path file gambar. |
|

**Returns:**
[SearchImage](../../com.groupdocs.search.common/searchimage) - An image to search.

### create(String filePath, int imageIndex) {#create-java.lang.String-int-}
```
public static SearchImage create(String filePath, int imageIndex)
```


Membuat gambar dari file untuk pencarian.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | filePath | java.lang.String | Path file gambar. |
|
|  | imageIndex | int | Indeks gambar dalam gambar multipage. |
|

**Returns:**
[SearchImage](../../com.groupdocs.search.common/searchimage) - An image to search.

### create(InputStream stream) {#create-java.io.InputStream-}
```
public static SearchImage create(InputStream stream)
```


Membuat gambar dari aliran untuk pencarian.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | stream | java.io.InputStream | Aliran gambar. |
|

**Returns:**
[SearchImage](../../com.groupdocs.search.common/searchimage) - An image to search.

### create(InputStream stream, int imageIndex) {#create-java.io.InputStream-int-}
```
public static SearchImage create(InputStream stream, int imageIndex)
```


Membuat gambar dari aliran untuk pencarian.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | stream | java.io.InputStream | Aliran gambar. |
|
|  | imageIndex | int | Indeks gambar dalam gambar multipage. |
|

**Returns:**
[SearchImage](../../com.groupdocs.search.common/searchimage) - An image to search.

