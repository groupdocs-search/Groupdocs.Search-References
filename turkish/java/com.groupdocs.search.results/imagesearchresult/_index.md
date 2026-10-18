---
title: "ImageSearchResult"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Ters görüntü aramasının sonucunu temsil eder."
type: docs
weight: 17
url: /tr/java/com.groupdocs.search.results/imagesearchresult/
---
**Inheritance:**
java.lang.Object
```
public abstract class ImageSearchResult
```

Ters görüntü aramasının sonucunu temsil eder.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [ImageSearchResult()](#ImageSearchResult--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getImageCount()](#getImageCount--) | Bulunan resim sayısını alır. |
|
|  | [getFoundImage(int index)](#getFoundImage-int-) | Bulunan resmi indeksine göre alır. |
|
### ImageSearchResult() {#ImageSearchResult--}
```
public ImageSearchResult()
```


### getImageCount() {#getImageCount--}
```
public abstract int getImageCount()
```


Bulunan resim sayısını alır.


**Returns:**
int - Bulunan görüntü sayısı.

### getFoundImage(int index) {#getFoundImage-int-}
```
public abstract FoundImageFrame getFoundImage(int index)
```


Bulunan resmi indeksine göre alır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | indeks | int | Bulunan bir görüntünün indeksi. |
|

**Returns:**
[FoundImageFrame](../../com.groupdocs.search.results/foundimageframe) - The found image.

