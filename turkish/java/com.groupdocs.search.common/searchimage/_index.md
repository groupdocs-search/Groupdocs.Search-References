---
title: "SearchImage"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Arama yapılacak bir görüntüyü temsil eder."
type: docs
weight: 29
url: /tr/java/com.groupdocs.search.common/searchimage/
---
**Inheritance:**
java.lang.Object
```
public abstract class SearchImage
```

Arama yapılacak bir görüntüyü temsil eder.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [SearchImage()](#SearchImage--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [create(String filePath)](#create-java.lang.String-) | Arama için bir dosyadan görüntü oluşturur. |
|
|  | [create(String filePath, int imageIndex)](#create-java.lang.String-int-) | Arama için bir dosyadan görüntü oluşturur. |
|
|  | [create(InputStream stream)](#create-java.io.InputStream-) | Arama için bir akıştan görüntü oluşturur. |
|
|  | [create(InputStream stream, int imageIndex)](#create-java.io.InputStream-int-) | Arama için bir akıştan görüntü oluşturur. |
|
### SearchImage() {#SearchImage--}
```
public SearchImage()
```


### create(String filePath) {#create-java.lang.String-}
```
public static SearchImage create(String filePath)
```


Arama için bir dosyadan görüntü oluşturur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | filePath | java.lang.String | Görüntü dosya yolu. |
|

**Returns:**
[SearchImage](../../com.groupdocs.search.common/searchimage) - An image to search.

### create(String filePath, int imageIndex) {#create-java.lang.String-int-}
```
public static SearchImage create(String filePath, int imageIndex)
```


Arama için bir dosyadan görüntü oluşturur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | filePath | java.lang.String | Görüntü dosya yolu. |
|
|  | imageIndex | int | Çok sayfalı görüntülerdeki görüntü indeksi. |
|

**Returns:**
[SearchImage](../../com.groupdocs.search.common/searchimage) - An image to search.

### create(InputStream stream) {#create-java.io.InputStream-}
```
public static SearchImage create(InputStream stream)
```


Arama için bir akıştan görüntü oluşturur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | stream | java.io.InputStream | Görüntü akışı. |
|

**Returns:**
[SearchImage](../../com.groupdocs.search.common/searchimage) - An image to search.

### create(InputStream stream, int imageIndex) {#create-java.io.InputStream-int-}
```
public static SearchImage create(InputStream stream, int imageIndex)
```


Arama için bir akıştan görüntü oluşturur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | stream | java.io.InputStream | Görüntü akışı. |
|
|  | imageIndex | int | Çok sayfalı görüntülerdeki görüntü indeksi. |
|

**Returns:**
[SearchImage](../../com.groupdocs.search.common/searchimage) - An image to search.

