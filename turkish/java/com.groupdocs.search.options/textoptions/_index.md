---
title: "TextOptions"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Bir indeksten belge metnini alma için seçenekler sağlar."
type: docs
weight: 41
url: /tr/java/com.groupdocs.search.options/textoptions/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.search.options.ITextOptions](../../com.groupdocs.search.options/itextoptions)
```
public class TextOptions implements ITextOptions
```

Bir indeksten belge metnini alma için seçenekler sağlar.


**Learn more**

* [Getting indexed documents](../https://docs.groupdocs.com/display/searchjava/Getting+indexed+documents)
* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [TextOptions()](#TextOptions--) | TextOptions sınıfının yeni bir örneğini başlatır. |
|
|  | [TextOptions(Object data)](#TextOptions-java.lang.Object-) | TextOptions sınıfının yeni bir örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getCustomExtractor()](#getCustomExtractor--) | Dizinleme için kullanılan özel metin çıkarıcıyı alır. |
|
|  | [setCustomExtractor(IFieldExtractor value)](#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-) | Dizinleme için kullanılan özel metin çıkarıcıyı ayarlar. |
|
|  | [getAdditionalFields()](#getAdditionalFields--) | Dizinleme için kullanılan ek belge alanlarını alır. |
|
|  | [setAdditionalFields(DocumentField[] value)](#setAdditionalFields-com.groupdocs.search.common.DocumentField---) | Dizinleme için kullanılan ek belge alanlarını ayarlar. |
|
|  | [getCancellation()](#getCancellation--) | İptal nesnesini alır. |
|
|  | [setCancellation(Cancellation value)](#setCancellation-com.groupdocs.search.common.Cancellation-) | İptal nesnesini ayarlar. |
|
|  | [getGenerateHead()](#getGenerateHead--) | Head etiketinin çıktı HTML'de oluşturulup oluşturulmadığını gösteren bir değer alır. |
|
|  | [setGenerateHead(boolean value)](#setGenerateHead-boolean-) | Head etiketinin çıktı HTML'de oluşturulup oluşturulmadığını gösteren bir değer ayarlar. |
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
### TextOptions() {#TextOptions--}
```
public TextOptions()
```


TextOptions sınıfının yeni bir örneğini başlatır.


### TextOptions(Object data) {#TextOptions-java.lang.Object-}
```
public TextOptions(Object data)
```


TextOptions sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | veri | java.lang.Object | Serileştirilmiş veri. |
|

### getCustomExtractor() {#getCustomExtractor--}
```
public IFieldExtractor getCustomExtractor()
```


Dizinleme için kullanılan özel metin çıkarıcıyı alır. Varsayılan değer null. Bu değerin yalnızca belge metni indeks'e kaydedilmemişse kullanıldığını unutmayın.


**Returns:**
[IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) - The custom text extractor that was used for indexing.

### setCustomExtractor(IFieldExtractor value) {#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-}
```
public void setCustomExtractor(IFieldExtractor value)
```


Dizinleme için kullanılan özel metin çıkarıcıyı ayarlar. Varsayılan değer null'dır. Bu değerin yalnızca belge metni dizine kaydedilmemişse kullanıldığını unutmayın.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | value | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | Dizinleme için kullanılan özel metin çıkarıcı. |
|

### getAdditionalFields() {#getAdditionalFields--}
```
public DocumentField[] getAdditionalFields()
```


Dizinleme için kullanılan ek belge alanlarını alır. Varsayılan değer null'dir. Bu değerin yalnızca belge metni dizine kaydedilmemişse kullanıldığını unutmayın.


**Returns:**
com.groupdocs.search.common.DocumentField[] - Dizinleme için kullanılan ek belge alanları.

### setAdditionalFields(DocumentField[] value) {#setAdditionalFields-com.groupdocs.search.common.DocumentField---}
```
public void setAdditionalFields(DocumentField[] value)
```


Dizinleme için kullanılan ek belge alanlarını ayarlar. Varsayılan değer null'dir. Bu değerin yalnızca belge metni dizine kaydedilmemişse kullanıldığını unutmayın.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | value | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | Dizinleme için kullanılan ek belge alanları. |
|

### getCancellation() {#getCancellation--}
```
public Cancellation getCancellation()
```


İptal nesnesini alır. Varsayılan değer null'dır.


**Returns:**
[Cancellation](../../com.groupdocs.search.common/cancellation) - The cancellation object.

### setCancellation(Cancellation value) {#setCancellation-com.groupdocs.search.common.Cancellation-}
```
public void setCancellation(Cancellation value)
```


İptal nesnesini ayarlar. Varsayılan değer null'dir.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | value | [Cancellation](../../com.groupdocs.search.common/cancellation) | İptal nesnesi. |
|

### getGenerateHead() {#getGenerateHead--}
```
public boolean getGenerateHead()
```


Çıktı HTML'sinde Head etiketinin oluşturulup oluşturulmadığını gösteren bir değeri alır. Varsayılan değer true'dur.


**Returns:**
boolean - Çıktı HTML'sinde Head etiketinin oluşturulup oluşturulmadığını gösteren bir değer.

### setGenerateHead(boolean value) {#setGenerateHead-boolean-}
```
public void setGenerateHead(boolean value)
```


Çıktı HTML'sinde Head etiketinin oluşturulup oluşturulmadığını gösteren bir değeri ayarlar. Varsayılan değer true'dur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | boolean | Çıktı HTML'sinde Head etiketinin oluşturulup oluşturulmadığını gösteren bir değer. |
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
