---
title: "IndexingOptions"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Menyediakan opsi untuk operasi pengindeksan."
type: docs
weight: 25
url: /id/java/com.groupdocs.search.options/indexingoptions/
---
**Inheritance:**
java.lang.Object
```
public class IndexingOptions
```

Menyediakan opsi untuk operasi pengindeksan.


**Learn more**

* [Indexing options](../https://docs.groupdocs.com/display/searchjava/Indexing+options)

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [IndexingOptions()](#IndexingOptions--) | Menginisialisasi instance baru dari kelas  IndexingOptions  . |
|
|  | [IndexingOptions(Object data)](#IndexingOptions-java.lang.Object-) | Menginisialisasi instance baru dari kelas  IndexingOptions  . |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getThreads()](#getThreads--) | Mendapatkan jumlah thread yang digunakan untuk pengindeksan. |
|
|  | [setThreads(int value)](#setThreads-int-) | Mengatur jumlah thread yang digunakan untuk pengindeksan. |
|
|  | [isAsync()](#isAsync--) | Mendapatkan flag pelaksanaan operasi secara asinkron. |
|
|  | [setAsync(boolean value)](#setAsync-boolean-) | Mengatur flag pelaksanaan operasi secara asinkron. |
|
|  | [getCancellation()](#getCancellation--) | Mendapatkan objek pembatalan operasi. |
|
|  | [setCancellation(Cancellation value)](#setCancellation-com.groupdocs.search.common.Cancellation-) | Mengatur objek pembatalan operasi. |
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
### IndexingOptions() {#IndexingOptions--}
```
public IndexingOptions()
```


Menginisialisasi instance baru dari kelas  IndexingOptions  .


### IndexingOptions(Object data) {#IndexingOptions-java.lang.Object-}
```
public IndexingOptions(Object data)
```


Menginisialisasi instance baru dari kelas  IndexingOptions  .


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | data | java.lang.Object | Data yang diserialkan. |
|

### getThreads() {#getThreads--}
```
public int getThreads()
```


Mendapatkan jumlah thread yang digunakan untuk pengindeksan. Nilai defaultnya adalah 1.


**Returns:**
int - Jumlah thread yang digunakan untuk pengindeksan.

### setThreads(int value) {#setThreads-int-}
```
public void setThreads(int value)
```


Mengatur jumlah thread yang digunakan untuk pengindeksan. Nilai defaultnya adalah 1.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | int | Jumlah thread yang digunakan untuk pengindeksan. |
|

### isAsync() {#isAsync--}
```
public boolean isAsync()
```


Mendapatkan flag pelaksanaan operasi secara asynchronous. Nilai defaultnya adalah false.


**Returns:**
boolean - Flag pelaksanaan operasi secara asynchronous.

### setAsync(boolean value) {#setAsync-boolean-}
```
public void setAsync(boolean value)
```


Mengatur flag pelaksanaan operasi secara asynchronous. Nilai defaultnya adalah false.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | boolean | Flag pelaksanaan operasi secara asynchronous. |
|

### getCancellation() {#getCancellation--}
```
public Cancellation getCancellation()
```


Mendapatkan objek pembatalan operasi. Nilai defaultnya adalah null.


**Returns:**
[Cancellation](../../com.groupdocs.search.common/cancellation) - The operation cancellation object.

### setCancellation(Cancellation value) {#setCancellation-com.groupdocs.search.common.Cancellation-}
```
public void setCancellation(Cancellation value)
```


Mengatur objek pembatalan operasi. Nilai defaultnya adalah null.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | value | [Cancellation](../../com.groupdocs.search.common/cancellation) | Objek pembatalan operasi. |
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
