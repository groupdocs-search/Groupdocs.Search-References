---
title: "UpdateOptions"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Güncelleme işlemi için seçenekler sağlar."
type: docs
weight: 43
url: /tr/java/com.groupdocs.search.options/updateoptions/
---
**Inheritance:**
java.lang.Object
```
public class UpdateOptions
```

Güncelleme işlemi için seçenekler sağlar.


**Learn more**

* [Update index](../https://docs.groupdocs.com/display/searchjava/Update+index)
* [Delete indexed paths](../https://docs.groupdocs.com/display/searchjava/Delete+indexed+paths)

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [UpdateOptions()](#UpdateOptions--) |   UpdateOptions  sınıfının yeni bir örneğini başlatır. |
|
|  | [UpdateOptions(Object data)](#UpdateOptions-java.lang.Object-) |   UpdateOptions  sınıfının yeni bir örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getThreads()](#getThreads--) | Dizinleme için kullanılan iş parçacığı sayısını alır. |
|
|  | [setThreads(int value)](#setThreads-int-) | Dizinleme için kullanılan iş parçacığı sayısını ayarlar. |
|
|  | [isAsync()](#isAsync--) | İşlemin asenkron olarak gerçekleştirilme bayrağını alır. |
|
|  | [setAsync(boolean value)](#setAsync-boolean-) | İşlemin asenkron olarak gerçekleştirilme bayrağını ayarlar. |
|
|  | [getCancellation()](#getCancellation--) | İşlem iptal nesnesini alır. |
|
|  | [setCancellation(Cancellation value)](#setCancellation-com.groupdocs.search.common.Cancellation-) | İşlem iptal nesnesini ayarlar. |
|
|  | [getAutoDetectEncoding()](#getAutoDetectEncoding--) | Kodlamanın otomatik olarak algılanıp algılanmayacağını gösteren bir değeri alır. |
|
|  | [setAutoDetectEncoding(boolean value)](#setAutoDetectEncoding-boolean-) | Kodlamanın otomatik olarak algılanıp algılanmayacağını gösteren bir değeri ayarlar. |
|
|  | [getEncoding()](#getEncoding--) | Metin belgelerinden metin çıkarmak için kullanılan kodlamayı alır. |
|
|  | [setEncoding(String value)](#setEncoding-java.lang.String-) | Metin belgelerinden metin çıkarmak için kullanılan kodlamayı ayarlar. |
|
|  | [getUseRawTextExtraction()](#getUseRawTextExtraction--) | Mümkünse metin çıkarma için ham modun kullanılıp kullanılmadığını gösteren bir değeri alır. |
|
|  | [setUseRawTextExtraction(boolean value)](#setUseRawTextExtraction-boolean-) | Mümkünse metin çıkarma için ham modun kullanılıp kullanılmadığını gösteren bir değeri ayarlar. |
|
|  | [getMetadataIndexingOptions()](#getMetadataIndexingOptions--) | Meta veri alanlarını indeksleme seçeneklerini alır. |
|
|  | [getOcrIndexingOptions()](#getOcrIndexingOptions--) | OCR işleme ve tanınan metni indeksleme seçeneklerini alır. |
|
|  | [getImageIndexingOptions()](#getImageIndexingOptions--) | Ters görsel arama için görsel indeksleme seçeneklerini alır. |
|
| [getCore()](#getCore--) |  |
### UpdateOptions() {#UpdateOptions--}
```
public UpdateOptions()
```


  UpdateOptions  sınıfının yeni bir örneğini başlatır.


### UpdateOptions(Object data) {#UpdateOptions-java.lang.Object-}
```
public UpdateOptions(Object data)
```


  UpdateOptions  sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | veri | java.lang.Object | Serileştirilmiş veri. |
|

### getThreads() {#getThreads--}
```
public int getThreads()
```


Dizinleme için kullanılan iş parçacığı sayısını alır. Varsayılan değer  1  dir.


**Returns:**
int - İndeksleme için kullanılan iş parçacığı sayısı.

### setThreads(int value) {#setThreads-int-}
```
public void setThreads(int value)
```


İndeksleme için kullanılan iş parçacığı sayısını ayarlar. Varsayılan değer  1 .


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | int | İndeksleme için kullanılan iş parçacığı sayısı. |
|

### isAsync() {#isAsync--}
```
public boolean isAsync()
```


İşlemin asenkron olarak gerçekleştirilmesinin bayrağını alır. Varsayılan değer  false .


**Returns:**
boolean - İşlemin asenkron olarak gerçekleştirilmesinin bayrağı.

### setAsync(boolean value) {#setAsync-boolean-}
```
public void setAsync(boolean value)
```


İşlemin asenkron olarak gerçekleştirilmesinin bayrağını ayarlar. Varsayılan değer  false .


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | boolean | İşlemin asenkron olarak gerçekleştirilmesinin bayrağı. |
|

### getCancellation() {#getCancellation--}
```
public Cancellation getCancellation()
```


İşlem iptal nesnesini alır. Varsayılan değer  null .


**Returns:**
[Cancellation](../../com.groupdocs.search.common/cancellation) - The operation cancellation object.

### setCancellation(Cancellation value) {#setCancellation-com.groupdocs.search.common.Cancellation-}
```
public void setCancellation(Cancellation value)
```


İşlem iptal nesnesini ayarlar. Varsayılan değer  null .


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | value | [Cancellation](../../com.groupdocs.search.common/cancellation) | İşlem iptal nesnesi. |
|

### getAutoDetectEncoding() {#getAutoDetectEncoding--}
```
public boolean getAutoDetectEncoding()
```


Kodlamayı otomatik olarak algılayıp algılamayacağını gösteren bir değeri alır. Varsayılan değer  false .


**Returns:**
boolean - Kodlamayı otomatik olarak algılayıp algılamayacağını gösteren bir değer.

### setAutoDetectEncoding(boolean value) {#setAutoDetectEncoding-boolean-}
```
public void setAutoDetectEncoding(boolean value)
```


Kodlamayı otomatik olarak algılayıp algılamayacağını gösteren bir değeri ayarlar. Varsayılan değer  false .


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | boolean | Kodlamayı otomatik olarak algılayıp algılamayacağını gösteren bir değer. |
|

### getEncoding() {#getEncoding--}
```
public String getEncoding()
```


Metin belgelerinden metin çıkarmak için kullanılan kodlamayı alır. Varsayılan değer  null , bu da varsayılan kodlamanın UTF-8 olduğu anlamına gelir. AutoDetectEncoding true ise bu değer varsayılan kodlama olarak kullanılır.


**Returns:**
java.lang.String - Metin belgelerinden metin çıkarmak için kullanılan kodlama.

### setEncoding(String value) {#setEncoding-java.lang.String-}
```
public void setEncoding(String value)
```


Metin belgelerinden metin çıkarmak için kullanılan kodlamayı ayarlar. Varsayılan değer  null , bu da varsayılan kodlamanın UTF-8 olduğu anlamına gelir. AutoDetectEncoding true ise bu değer varsayılan kodlama olarak kullanılır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | java.lang.String | Metin belgelerinden metin çıkarmak için kullanılan kodlama. |
|

### getUseRawTextExtraction() {#getUseRawTextExtraction--}
```
public boolean getUseRawTextExtraction()
```


Mümkünse ham modun metin çıkarma için kullanılıp kullanılmadığını gösteren bir değeri alır. Varsayılan değer  true . Ham mod indeksleme hızını önemli ölçüde artırabilir, ancak normal mod çıkarılan metnin biçimlendirmesini iyileştirir.


**Returns:**
boolean - Mümkünse ham modun metin çıkarma için kullanılıp kullanılmadığını gösteren bir değer.

### setUseRawTextExtraction(boolean value) {#setUseRawTextExtraction-boolean-}
```
public void setUseRawTextExtraction(boolean value)
```


Mümkünse ham modun metin çıkarma için kullanılıp kullanılmadığını gösteren bir değeri ayarlar. Varsayılan değer  true . Ham mod indeksleme hızını önemli ölçüde artırabilir, ancak normal mod çıkarılan metnin biçimlendirmesini iyileştirir.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | boolean | Mümkünse ham modun metin çıkarma için kullanılıp kullanılmadığını gösteren bir değer. |
|

### getMetadataIndexingOptions() {#getMetadataIndexingOptions--}
```
public MetadataIndexingOptions getMetadataIndexingOptions()
```


Meta veri alanlarını indeksleme seçeneklerini alır.


**Returns:**
[MetadataIndexingOptions](../../com.groupdocs.search.options/metadataindexingoptions) - The options for indexing metadata fields.

### getOcrIndexingOptions() {#getOcrIndexingOptions--}
```
public OcrIndexingOptions getOcrIndexingOptions()
```


OCR işleme ve tanınan metni indeksleme seçeneklerini alır.


**Returns:**
[OcrIndexingOptions](../../com.groupdocs.search.options/ocrindexingoptions) - The options for OCR processing and indexing recognized text.

### getImageIndexingOptions() {#getImageIndexingOptions--}
```
public ImageIndexingOptions getImageIndexingOptions()
```


Ters görsel arama için görsel indeksleme seçeneklerini alır.


**Returns:**
[ImageIndexingOptions](../../com.groupdocs.search.options/imageindexingoptions) - The image indexing options for reverse image search.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
