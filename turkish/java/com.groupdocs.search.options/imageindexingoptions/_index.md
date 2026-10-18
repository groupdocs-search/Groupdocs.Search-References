---
title: "ImageIndexingOptions"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Ters görüntü araması için görüntü indeksleme seçenekleri sağlar."
type: docs
weight: 23
url: /tr/java/com.groupdocs.search.options/imageindexingoptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class ImageIndexingOptions
```

Ters görüntü araması için görüntü indeksleme seçenekleri sağlar.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [ImageIndexingOptions()](#ImageIndexingOptions--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getEnabledForSeparateImages()](#getEnabledForSeparateImages--) | Ayrı görüntü dosyalarını indeksleyip indekslemeyeceğini gösteren bir değeri alır. |
|
|  | [setEnabledForSeparateImages(boolean value)](#setEnabledForSeparateImages-boolean-) | Ayrı görüntü dosyalarını indeksleyip indekslemeyeceğini gösteren bir değeri ayarlar. |
|
|  | [getEnabledForContainerItemImages()](#getEnabledForContainerItemImages--) | Konteynerdeki öğeler olan görüntüleri (örneğin, ZIP arşivindeki görüntüler) indeksleyip indekslemeyeceğini gösteren bir değeri alır. |
|
|  | [setEnabledForContainerItemImages(boolean value)](#setEnabledForContainerItemImages-boolean-) | Konteynerdeki öğeler olan görüntüleri (örneğin, ZIP arşivindeki görüntüler) indeksleyip indekslemeyeceğini gösteren bir değeri ayarlar. |
|
|  | [getEnabledForEmbeddedImages()](#getEnabledForEmbeddedImages--) | Gömülü görüntüleri (örneğin, DOCX belgesindeki görüntüler) indeksleyip indekslemeyeceğini gösteren bir değeri alır. |
|
|  | [setEnabledForEmbeddedImages(boolean value)](#setEnabledForEmbeddedImages-boolean-) | Gömülü görüntüleri (örneğin, DOCX belgesindeki görüntüler) indeksleyip indekslemeyeceğini gösteren bir değeri ayarlar. |
|
### ImageIndexingOptions() {#ImageIndexingOptions--}
```
public ImageIndexingOptions()
```


### getEnabledForSeparateImages() {#getEnabledForSeparateImages--}
```
public abstract boolean getEnabledForSeparateImages()
```


Ayrı görüntü dosyalarını indeksleyip indekslemeyeceğini gösteren bir değeri alır. Varsayılan değer false.


**Returns:**
boolean - Ayrı görüntü dosyalarını indeksleyip indekslemeyeceğini gösteren bir değer.

### setEnabledForSeparateImages(boolean value) {#setEnabledForSeparateImages-boolean-}
```
public abstract void setEnabledForSeparateImages(boolean value)
```


Ayrı görüntü dosyalarını indeksleyip indekslemeyeceğini gösteren bir değeri ayarlar. Varsayılan değer false.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | boolean | Ayrı görüntü dosyalarını indeksleyip indekslemeyeceğini gösteren bir değer. |
|

### getEnabledForContainerItemImages() {#getEnabledForContainerItemImages--}
```
public abstract boolean getEnabledForContainerItemImages()
```


Konteynerdeki öğeler olan görüntüleri (örneğin, ZIP arşivindeki görüntüler) indeksleyip indekslemeyeceğini gösteren bir değeri alır. Varsayılan değer false.


**Returns:**
boolean - Konteynerdeki öğeler olan görüntüleri indeksleyip indekslemeyeceğini gösteren bir değer.

### setEnabledForContainerItemImages(boolean value) {#setEnabledForContainerItemImages-boolean-}
```
public abstract void setEnabledForContainerItemImages(boolean value)
```


Konteynerdeki öğeler olan görüntüleri (örneğin, ZIP arşivindeki görüntüler) indeksleyip indekslemeyeceğini gösteren bir değeri ayarlar. Varsayılan değer false.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | boolean | Konteynerdeki öğeler olan görüntüleri indeksleyip indekslemeyeceğini gösteren bir değer. |
|

### getEnabledForEmbeddedImages() {#getEnabledForEmbeddedImages--}
```
public abstract boolean getEnabledForEmbeddedImages()
```


Gömülü görüntüleri (örneğin, DOCX belgesindeki görüntüler) indeksleyip indekslemeyeceğini gösteren bir değeri alır. Varsayılan değer false.


**Returns:**
boolean - Gömülü görüntüleri indeksleyip indekslemeyeceğini gösteren bir değer.

### setEnabledForEmbeddedImages(boolean value) {#setEnabledForEmbeddedImages-boolean-}
```
public abstract void setEnabledForEmbeddedImages(boolean value)
```


Gömülü görüntüleri (örneğin, DOCX belgesindeki görüntüler) indeksleyip indekslemeyeceğini gösteren bir değeri ayarlar. Varsayılan değer false.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | boolean | Gömülü görüntüleri indeksleyip indekslemeyeceğini gösteren bir değer. |
|

