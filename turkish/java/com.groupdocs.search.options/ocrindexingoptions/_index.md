---
title: "OcrIndexingOptions"
second_title: "GroupDocs.Search for Java API Referansı"
description: "OCR işleme ve tanınan metni indeksleme için seçenekler sağlar."
type: docs
weight: 31
url: /tr/java/com.groupdocs.search.options/ocrindexingoptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class OcrIndexingOptions
```

OCR işleme ve tanınan metni indeksleme için seçenekler sağlar.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [OcrIndexingOptions()](#OcrIndexingOptions--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getEnabledForSeparateImages()](#getEnabledForSeparateImages--) | Ayrı görüntü dosyalarında metni tanıyıp tanımadığını gösteren bir değeri alır. |
|
|  | [setEnabledForSeparateImages(boolean value)](#setEnabledForSeparateImages-boolean-) | Ayrı görüntü dosyalarında metni tanıyıp tanımadığını gösteren bir değeri ayarlar. |
|
|  | [getEnabledForContainerItemImages()](#getEnabledForContainerItemImages--) | Bir konteynerdeki öğe olan görüntülerde (örneğin, bir ZIP arşivindeki görüntüler) metni tanıyıp tanımadığını gösteren bir değeri alır. |
|
|  | [setEnabledForContainerItemImages(boolean value)](#setEnabledForContainerItemImages-boolean-) | Bir konteynerdeki öğe olan görüntülerde (örneğin, bir ZIP arşivindeki görüntüler) metni tanıyıp tanımadığını gösteren bir değeri ayarlar. |
|
|  | [getEnabledForEmbeddedImages()](#getEnabledForEmbeddedImages--) | Gömülü görüntülerde metin tanıma yapılıp yapılmayacağını gösteren bir değer alır (örneğin, bir DOCX belgesindeki görseller). |
|
|  | [setEnabledForEmbeddedImages(boolean value)](#setEnabledForEmbeddedImages-boolean-) | Gömülü görüntülerde metin tanıma yapılıp yapılmayacağını gösteren bir değeri ayarlar (örneğin, bir DOCX belgesindeki görseller). |
|
|  | [getOcrConnector()](#getOcrConnector--) | OCR işleme için kullanılan bir OCR bağlayıcısını alır. |
|
|  | [setOcrConnector(IOcrConnector value)](#setOcrConnector-com.groupdocs.search.options.IOcrConnector-) | OCR işleme için kullanılan bir OCR bağlayıcısını ayarlar. |
|
### OcrIndexingOptions() {#OcrIndexingOptions--}
```
public OcrIndexingOptions()
```


### getEnabledForSeparateImages() {#getEnabledForSeparateImages--}
```
public abstract boolean getEnabledForSeparateImages()
```


Ayrı görüntü dosyalarında metin tanıma yapılıp yapılmayacağını gösteren bir değer alır. Varsayılan değer  false  .


**Returns:**
boolean - Ayrı görüntü dosyalarında metin tanıma yapılıp yapılmayacağını gösteren bir değer.

### setEnabledForSeparateImages(boolean value) {#setEnabledForSeparateImages-boolean-}
```
public abstract void setEnabledForSeparateImages(boolean value)
```


Ayrı görüntü dosyalarında metin tanıma yapılıp yapılmayacağını gösteren bir değeri ayarlar. Varsayılan değer  false  .


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | boolean | Ayrı görüntü dosyalarında metin tanıma yapılıp yapılmayacağını gösteren bir değer. |
|

### getEnabledForContainerItemImages() {#getEnabledForContainerItemImages--}
```
public abstract boolean getEnabledForContainerItemImages()
```


Konteynerdeki öğeler olan görüntülerde (örneğin, bir ZIP arşivindeki görseller) metin tanıma yapılıp yapılmayacağını gösteren bir değer alır. Varsayılan değer  false  .


**Returns:**
boolean - Konteynerdeki öğeler olan görüntülerde metin tanıma yapılıp yapılmayacağını gösteren bir değer.

### setEnabledForContainerItemImages(boolean value) {#setEnabledForContainerItemImages-boolean-}
```
public abstract void setEnabledForContainerItemImages(boolean value)
```


Konteynerdeki öğeler olan görüntülerde (örneğin, bir ZIP arşivindeki görseller) metin tanıma yapılıp yapılmayacağını gösteren bir değeri ayarlar. Varsayılan değer  false  .


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | boolean | Konteynerdeki öğeler olan görüntülerde metin tanıma yapılıp yapılmayacağını gösteren bir değer. |
|

### getEnabledForEmbeddedImages() {#getEnabledForEmbeddedImages--}
```
public abstract boolean getEnabledForEmbeddedImages()
```


Gömülü görüntülerde (örneğin, bir DOCX belgesindeki görseller) metin tanıma yapılıp yapılmayacağını gösteren bir değer alır. Varsayılan değer  false  .


**Returns:**
boolean - Gömülü görüntülerde metin tanıma yapılıp yapılmayacağını gösteren bir değer.

### setEnabledForEmbeddedImages(boolean value) {#setEnabledForEmbeddedImages-boolean-}
```
public abstract void setEnabledForEmbeddedImages(boolean value)
```


Gömülü görüntülerde (örneğin, bir DOCX belgesindeki görseller) metin tanıma yapılıp yapılmayacağını gösteren bir değeri ayarlar. Varsayılan değer  false  .


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | boolean | Gömülü görüntülerde metin tanıma yapılıp yapılmayacağını gösteren bir değer. |
|

### getOcrConnector() {#getOcrConnector--}
```
public abstract IOcrConnector getOcrConnector()
```


OCR işleme için kullanılan bir OCR bağlayıcısını alır. Varsayılan değer  null  , bu da OCR kullanılmadığı anlamına gelir.


**Returns:**
[IOcrConnector](../../com.groupdocs.search.options/iocrconnector) - An OCR connector that is used for OCR processing.

### setOcrConnector(IOcrConnector value) {#setOcrConnector-com.groupdocs.search.options.IOcrConnector-}
```
public abstract void setOcrConnector(IOcrConnector value)
```


OCR işleme için kullanılan bir OCR bağlayıcısını ayarlar. Varsayılan değer  null  , bu da OCR kullanılmadığı anlamına gelir.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | value | [IOcrConnector](../../com.groupdocs.search.options/iocrconnector) | OCR işleme için kullanılan bir OCR bağlayıcısı. |
|

