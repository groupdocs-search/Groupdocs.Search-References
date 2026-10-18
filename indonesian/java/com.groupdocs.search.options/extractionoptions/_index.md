---
title: "ExtractionOptions"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Menyediakan opsi untuk mengekstrak data dari dokumen."
type: docs
weight: 18
url: /id/java/com.groupdocs.search.options/extractionoptions/
---
**Inheritance:**
java.lang.Object
```
public class ExtractionOptions
```

Menyediakan opsi untuk mengekstrak data dari dokumen.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [ExtractionOptions()](#ExtractionOptions--) | Menginisialisasi instance baru dari kelas  ExtractionOptions  . |
|
|  | [ExtractionOptions(Object data)](#ExtractionOptions-java.lang.Object-) | Menginisialisasi instance baru dari kelas  ExtractionOptions  . |
|
|  | [ExtractionOptions(IndexingOptions options, IFieldExtractor customExtractor, IOcrConnector ocrConnector)](#ExtractionOptions-com.groupdocs.search.options.IndexingOptions-com.groupdocs.search.common.IFieldExtractor-com.groupdocs.search.options.IOcrConnector-) | Menginisialisasi instance baru dari kelas  ExtractionOptions  . |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getCustomExtractor()](#getCustomExtractor--) | Mendapatkan pengekstrak teks khusus. |
|
|  | [setCustomExtractor(IFieldExtractor value)](#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-) | Mengatur atau mengatur pengekstrak teks khusus. |
|
|  | [getAutoDetectEncoding()](#getAutoDetectEncoding--) | Mendapatkan nilai yang menunjukkan apakah akan mendeteksi encoding secara otomatis atau tidak. |
|
|  | [setAutoDetectEncoding(boolean value)](#setAutoDetectEncoding-boolean-) | Mengatur nilai yang menunjukkan apakah akan mendeteksi encoding secara otomatis atau tidak. |
|
|  | [getEncoding()](#getEncoding--) | Mendapatkan encoding yang digunakan untuk mengekstrak teks dari dokumen teks. |
|
|  | [setEncoding(String value)](#setEncoding-java.lang.String-) | Mengatur enkoding yang digunakan untuk mengekstrak teks dari dokumen teks. |
|
|  | [getUseRawTextExtraction()](#getUseRawTextExtraction--) | Mendapatkan nilai yang menunjukkan apakah mode mentah digunakan untuk ekstraksi teks jika memungkinkan. |
|
|  | [setUseRawTextExtraction(boolean value)](#setUseRawTextExtraction-boolean-) | Mengatur nilai yang menunjukkan apakah mode mentah digunakan untuk ekstraksi teks jika memungkinkan. |
|
|  | [getMetadataIndexingOptions()](#getMetadataIndexingOptions--) | Mendapatkan opsi untuk mengindeks bidang metadata. |
|
|  | [getOcrIndexingOptions()](#getOcrIndexingOptions--) | Mendapatkan opsi untuk pemrosesan OCR dan pengindeksan teks yang dikenali. |
|
|  | [getImageIndexingOptions()](#getImageIndexingOptions--) | Mendapatkan opsi pengindeksan gambar untuk pencarian gambar terbalik. |
|
| [getCore()](#getCore--) |  |
### ExtractionOptions() {#ExtractionOptions--}
```
public ExtractionOptions()
```


Menginisialisasi instance baru dari kelas  ExtractionOptions  .


### ExtractionOptions(Object data) {#ExtractionOptions-java.lang.Object-}
```
public ExtractionOptions(Object data)
```


Menginisialisasi instance baru dari kelas  ExtractionOptions  .


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | data | java.lang.Object | Data yang diserialkan. |
|

### ExtractionOptions(IndexingOptions options, IFieldExtractor customExtractor, IOcrConnector ocrConnector) {#ExtractionOptions-com.groupdocs.search.options.IndexingOptions-com.groupdocs.search.common.IFieldExtractor-com.groupdocs.search.options.IOcrConnector-}
```
public ExtractionOptions(IndexingOptions options, IFieldExtractor customExtractor, IOcrConnector ocrConnector)
```


Menginisialisasi instance baru dari kelas  ExtractionOptions  .


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | Opsi. |
|
|  | customExtractor | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | Pengekstrak khusus. |
|
|  | ocrConnector | [IOcrConnector](../../com.groupdocs.search.options/iocrconnector) | Konektor ocr. |
|

### getCustomExtractor() {#getCustomExtractor--}
```
public IFieldExtractor getCustomExtractor()
```


Mendapatkan pengekstrak teks khusus. Nilai default adalah  null .


**Returns:**
[IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) - The custom text extractor.

### setCustomExtractor(IFieldExtractor value) {#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-}
```
public void setCustomExtractor(IFieldExtractor value)
```


Mengatur atau mengatur pengekstrak teks khusus. Nilai default adalah  null .


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | value | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | Pengekstrak teks khusus. |
|

### getAutoDetectEncoding() {#getAutoDetectEncoding--}
```
public boolean getAutoDetectEncoding()
```


Mendapatkan nilai yang menunjukkan apakah mendeteksi enkoding secara otomatis atau tidak. Nilai defaultnya adalah false.


**Returns:**
boolean - Nilai yang menunjukkan apakah mendeteksi enkoding secara otomatis atau tidak.

### setAutoDetectEncoding(boolean value) {#setAutoDetectEncoding-boolean-}
```
public void setAutoDetectEncoding(boolean value)
```


Mengatur nilai yang menunjukkan apakah mendeteksi enkoding secara otomatis atau tidak. Nilai defaultnya adalah false.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | boolean | Nilai yang menunjukkan apakah mendeteksi enkoding secara otomatis atau tidak. |
|

### getEncoding() {#getEncoding--}
```
public String getEncoding()
```


Mendapatkan enkoding yang digunakan untuk mengekstrak teks dari dokumen teks. Nilai defaultnya adalah null, yang berarti enkoding default UTF-8 digunakan. Jika AutoDetectEncoding adalah true maka nilai ini digunakan sebagai enkoding default.


**Returns:**
java.lang.String - Enkoding yang digunakan untuk mengekstrak teks dari dokumen teks.

### setEncoding(String value) {#setEncoding-java.lang.String-}
```
public void setEncoding(String value)
```


Mengatur enkoding yang digunakan untuk mengekstrak teks dari dokumen teks. Nilai defaultnya adalah null, yang berarti enkoding default UTF-8 digunakan. Jika AutoDetectEncoding adalah true maka nilai ini digunakan sebagai enkoding default.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | java.lang.String | Enkoding yang digunakan untuk mengekstrak teks dari dokumen teks. |
|

### getUseRawTextExtraction() {#getUseRawTextExtraction--}
```
public boolean getUseRawTextExtraction()
```


Mendapatkan nilai yang menunjukkan apakah mode mentah digunakan untuk ekstraksi teks jika memungkinkan. Nilai default adalah  true . Mode mentah dapat secara signifikan meningkatkan kecepatan pengindeksan, tetapi mode normal meningkatkan pemformatan teks yang diekstrak.


**Returns:**
boolean - Nilai yang menunjukkan apakah mode mentah digunakan untuk ekstraksi teks jika memungkinkan.

### setUseRawTextExtraction(boolean value) {#setUseRawTextExtraction-boolean-}
```
public void setUseRawTextExtraction(boolean value)
```


Mengatur nilai yang menunjukkan apakah mode mentah digunakan untuk ekstraksi teks jika memungkinkan. Nilai default adalah  true . Mode mentah dapat secara signifikan meningkatkan kecepatan pengindeksan, tetapi mode normal meningkatkan pemformatan teks yang diekstrak.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | boolean | Nilai yang menunjukkan apakah mode mentah digunakan untuk ekstraksi teks jika memungkinkan. |
|

### getMetadataIndexingOptions() {#getMetadataIndexingOptions--}
```
public MetadataIndexingOptions getMetadataIndexingOptions()
```


Mendapatkan opsi untuk mengindeks bidang metadata.


**Returns:**
[MetadataIndexingOptions](../../com.groupdocs.search.options/metadataindexingoptions) - The options for indexing metadata fields.

### getOcrIndexingOptions() {#getOcrIndexingOptions--}
```
public OcrIndexingOptions getOcrIndexingOptions()
```


Mendapatkan opsi untuk pemrosesan OCR dan pengindeksan teks yang dikenali.


**Returns:**
[OcrIndexingOptions](../../com.groupdocs.search.options/ocrindexingoptions) - The options for OCR processing and indexing recognized text.

### getImageIndexingOptions() {#getImageIndexingOptions--}
```
public ImageIndexingOptions getImageIndexingOptions()
```


Mendapatkan opsi pengindeksan gambar untuk pencarian gambar terbalik.


**Returns:**
[ImageIndexingOptions](../../com.groupdocs.search.options/imageindexingoptions) - The image indexing options for reverse image search.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
