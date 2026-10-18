---
title: "TextOptions"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Menyediakan opsi untuk mengambil teks dokumen dari indeks."
type: docs
weight: 41
url: /id/java/com.groupdocs.search.options/textoptions/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.search.options.ITextOptions](../../com.groupdocs.search.options/itextoptions)
```
public class TextOptions implements ITextOptions
```

Menyediakan opsi untuk mengambil teks dokumen dari indeks.


**Learn more**

* [Getting indexed documents](../https://docs.groupdocs.com/display/searchjava/Getting+indexed+documents)
* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [TextOptions()](#TextOptions--) | Menginisialisasi instance baru dari kelas TextOptions. |
|
|  | [TextOptions(Object data)](#TextOptions-java.lang.Object-) | Menginisialisasi instance baru dari kelas TextOptions. |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getCustomExtractor()](#getCustomExtractor--) | Mengambil pengekstrak teks khusus yang digunakan untuk pengindeksan. |
|
|  | [setCustomExtractor(IFieldExtractor value)](#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-) | Mengatur pengekstrak teks khusus yang digunakan untuk pengindeksan. |
|
|  | [getAdditionalFields()](#getAdditionalFields--) | Mendapatkan bidang dokumen tambahan yang digunakan untuk pengindeksan. |
|
|  | [setAdditionalFields(DocumentField[] value)](#setAdditionalFields-com.groupdocs.search.common.DocumentField---) | Mengatur bidang dokumen tambahan yang digunakan untuk pengindeksan. |
|
|  | [getCancellation()](#getCancellation--) | Mendapatkan objek pembatalan. |
|
|  | [setCancellation(Cancellation value)](#setCancellation-com.groupdocs.search.common.Cancellation-) | Mengatur objek pembatalan. |
|
|  | [getGenerateHead()](#getGenerateHead--) | Mendapatkan nilai yang menunjukkan apakah tag Head dihasilkan dalam HTML output. |
|
|  | [setGenerateHead(boolean value)](#setGenerateHead-boolean-) | Mengatur nilai yang menunjukkan apakah tag Head dihasilkan dalam HTML output. |
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
### TextOptions() {#TextOptions--}
```
public TextOptions()
```


Menginisialisasi instance baru dari kelas TextOptions.


### TextOptions(Object data) {#TextOptions-java.lang.Object-}
```
public TextOptions(Object data)
```


Menginisialisasi instance baru dari kelas TextOptions.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | data | java.lang.Object | Data yang diserialkan. |
|

### getCustomExtractor() {#getCustomExtractor--}
```
public IFieldExtractor getCustomExtractor()
```


Mendapatkan ekstraktor teks khusus yang digunakan untuk pengindeksan. Nilai default adalah null. Perhatikan bahwa nilai ini hanya digunakan jika teks dokumen tidak disimpan ke dalam indeks.


**Returns:**
[IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) - The custom text extractor that was used for indexing.

### setCustomExtractor(IFieldExtractor value) {#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-}
```
public void setCustomExtractor(IFieldExtractor value)
```


Mengatur ekstraktor teks khusus yang digunakan untuk pengindeksan. Nilai default adalah null. Perhatikan bahwa nilai ini hanya digunakan jika teks dokumen tidak disimpan ke dalam indeks.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | value | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | Ekstraktor teks khusus yang digunakan untuk pengindeksan. |
|

### getAdditionalFields() {#getAdditionalFields--}
```
public DocumentField[] getAdditionalFields()
```


Mendapatkan bidang dokumen tambahan yang digunakan untuk pengindeksan. Nilai default adalah null. Perhatikan bahwa nilai ini hanya digunakan jika teks dokumen tidak disimpan ke dalam indeks.


**Returns:**
com.groupdocs.search.common.DocumentField[] - Bidang dokumen tambahan yang digunakan untuk pengindeksan.

### setAdditionalFields(DocumentField[] value) {#setAdditionalFields-com.groupdocs.search.common.DocumentField---}
```
public void setAdditionalFields(DocumentField[] value)
```


Mengatur bidang dokumen tambahan yang digunakan untuk pengindeksan. Nilai default adalah null. Perhatikan bahwa nilai ini hanya digunakan jika teks dokumen tidak disimpan ke dalam indeks.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | value | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | Bidang dokumen tambahan yang digunakan untuk pengindeksan. |
|

### getCancellation() {#getCancellation--}
```
public Cancellation getCancellation()
```


Mendapatkan objek pembatalan. Nilai default adalah null.


**Returns:**
[Cancellation](../../com.groupdocs.search.common/cancellation) - The cancellation object.

### setCancellation(Cancellation value) {#setCancellation-com.groupdocs.search.common.Cancellation-}
```
public void setCancellation(Cancellation value)
```


Mengatur objek pembatalan. Nilai default adalah null.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | value | [Cancellation](../../com.groupdocs.search.common/cancellation) | Objek pembatalan. |
|

### getGenerateHead() {#getGenerateHead--}
```
public boolean getGenerateHead()
```


Mendapatkan nilai yang menunjukkan apakah tag Head dihasilkan dalam HTML output. Nilai default adalah true.


**Returns:**
boolean - Nilai yang menunjukkan apakah tag Head dihasilkan dalam HTML output.

### setGenerateHead(boolean value) {#setGenerateHead-boolean-}
```
public void setGenerateHead(boolean value)
```


Mengatur nilai yang menunjukkan apakah tag Head dihasilkan dalam HTML output. Nilai default adalah true.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | boolean | Nilai yang menunjukkan apakah tag Head dihasilkan dalam HTML output. |
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
