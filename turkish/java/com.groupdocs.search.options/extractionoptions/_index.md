---
title: "ExtractionOptions"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Belgelerden veri çıkarmak için seçenekler sağlar."
type: docs
weight: 18
url: /tr/java/com.groupdocs.search.options/extractionoptions/
---
**Inheritance:**
java.lang.Object
```
public class ExtractionOptions
```

Belgelerden veri çıkarmak için seçenekler sağlar.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [ExtractionOptions()](#ExtractionOptions--) | ExtractionOptions sınıfının yeni bir örneğini başlatır. |
|
|  | [ExtractionOptions(Object data)](#ExtractionOptions-java.lang.Object-) | ExtractionOptions sınıfının yeni bir örneğini başlatır. |
|
|  | [ExtractionOptions(IndexingOptions options, IFieldExtractor customExtractor, IOcrConnector ocrConnector)](#ExtractionOptions-com.groupdocs.search.options.IndexingOptions-com.groupdocs.search.common.IFieldExtractor-com.groupdocs.search.options.IOcrConnector-) | ExtractionOptions sınıfının yeni bir örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getCustomExtractor()](#getCustomExtractor--) | Özel metin çıkarıcıyı alır. |
|
|  | [setCustomExtractor(IFieldExtractor value)](#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-) | Ayarlayan veya ayarlayan özel metin çıkarıcıyı ayarlar. |
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
### ExtractionOptions() {#ExtractionOptions--}
```
public ExtractionOptions()
```


ExtractionOptions sınıfının yeni bir örneğini başlatır.


### ExtractionOptions(Object data) {#ExtractionOptions-java.lang.Object-}
```
public ExtractionOptions(Object data)
```


ExtractionOptions sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | veri | java.lang.Object | Serileştirilmiş veri. |
|

### ExtractionOptions(IndexingOptions options, IFieldExtractor customExtractor, IOcrConnector ocrConnector) {#ExtractionOptions-com.groupdocs.search.options.IndexingOptions-com.groupdocs.search.common.IFieldExtractor-com.groupdocs.search.options.IOcrConnector-}
```
public ExtractionOptions(IndexingOptions options, IFieldExtractor customExtractor, IOcrConnector ocrConnector)
```


ExtractionOptions sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | Seçenekler. |
|
|  | customExtractor | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | Özel çıkarıcı. |
|
|  | ocrConnector | [IOcrConnector](../../com.groupdocs.search.options/iocrconnector) | ocr bağlayıcısı. |
|

### getCustomExtractor() {#getCustomExtractor--}
```
public IFieldExtractor getCustomExtractor()
```


Özel metin çıkarıcıyı alır. Varsayılan değer null.


**Returns:**
[IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) - The custom text extractor.

### setCustomExtractor(IFieldExtractor value) {#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-}
```
public void setCustomExtractor(IFieldExtractor value)
```


Özel metin çıkarıcıyı ayarlar. Varsayılan değer null.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | value | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | Özel metin çıkarıcı. |
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
