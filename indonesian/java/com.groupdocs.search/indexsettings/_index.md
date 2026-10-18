---
title: "IndexSettings"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili pengaturan indeks yang memungkinkan penyesuaian operasi pengindeksan."
type: docs
weight: 19
url: /id/java/com.groupdocs.search/indexsettings/
---
**Inheritance:**
java.lang.Object
```
public class IndexSettings
```

Mewakili pengaturan indeks yang memungkinkan penyesuaian operasi pengindeksan.


**Learn more**

* [Search index settings](../https://docs.groupdocs.com/display/searchjava/Search+index+settings)


Contoh ini menunjukkan penggunaan tipikal kelas tersebut.

````
 ```

String indexFolder = "c:\\MyIndex\\";
IndexSettings settings = new IndexSettings();
settings.setIndexType(IndexType.CompactIndex); // Mengatur tipe indeks
Index index = new Index(indexFolder, settings); // Membuat sebuah indeks
 
```
 
````


## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [IndexSettings()](#IndexSettings--) | Menginisialisasi sebuah instance baru dari kelas IndexSettings. |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getInMemoryIndex()](#getInMemoryIndex--) | Mendapatkan nilai yang menunjukkan apakah indeks disimpan di memori atau di disk. |
|
|  | [getUseStopWords()](#getUseStopWords--) | Mendapatkan nilai yang menunjukkan apakah akan menggunakan kata berhenti atau tidak. |
|
|  | [setUseStopWords(boolean value)](#setUseStopWords-boolean-) | Mengatur nilai yang menunjukkan apakah akan menggunakan kata berhenti atau tidak. |
|
|  | [getMaxIndexingReportCount()](#getMaxIndexingReportCount--) | Mendapatkan jumlah maksimum laporan pengindeksan. |
|
|  | [setMaxIndexingReportCount(int value)](#setMaxIndexingReportCount-int-) | Mengatur jumlah maksimum laporan pengindeksan. |
|
|  | [getMaxSearchReportCount()](#getMaxSearchReportCount--) | Mendapatkan jumlah maksimum laporan pencarian. |
|
|  | [setMaxSearchReportCount(int value)](#setMaxSearchReportCount-int-) | Mengatur jumlah maksimum laporan pencarian. |
|
|  | [getUseCharacterReplacements()](#getUseCharacterReplacements--) | Mendapatkan nilai yang menunjukkan apakah akan menggunakan penggantian karakter atau tidak. |
|
|  | [setUseCharacterReplacements(boolean value)](#setUseCharacterReplacements-boolean-) | Mengatur nilai yang menunjukkan apakah akan menggunakan penggantian karakter atau tidak. |
|
|  | [getDocumentFilter()](#getDocumentFilter--) | Mendapatkan filter dokumen. |
|
|  | [setDocumentFilter(DocumentFilter value)](#setDocumentFilter-com.groupdocs.search.DocumentFilter-) | Mengatur filter dokumen. |
|
|  | [getTextStorageSettings()](#getTextStorageSettings--) | Mendapatkan pengaturan penyimpanan teks. |
|
|  | [setTextStorageSettings(TextStorageSettings value)](#setTextStorageSettings-com.groupdocs.search.options.TextStorageSettings-) | Mengatur pengaturan penyimpanan teks. |
|
|  | [getIndexType()](#getIndexType--) | Mendapatkan tipe indeks. |
|
|  | [setIndexType(IndexType value)](#setIndexType-com.groupdocs.search.options.IndexType-) | Mengatur tipe indeks. |
|
|  | [getSearchThreads()](#getSearchThreads--) | Mendapatkan jumlah thread yang digunakan untuk pencarian. |
|
|  | [setSearchThreads(NumberOfThreads value)](#setSearchThreads-com.groupdocs.search.options.NumberOfThreads-) | Mengatur jumlah thread yang digunakan untuk pencarian. |
|
|  | [getCustomExtractors()](#getCustomExtractors--) | Mendapatkan koleksi ekstraktor khusus. |
|
|  | [getLogger()](#getLogger--) | Mendapatkan logger yang digunakan untuk mencatat peristiwa dan kesalahan dalam indeks. |
|
|  | [setLogger(ILogger value)](#setLogger-com.groupdocs.search.common.ILogger-) | Mengatur logger yang digunakan untuk mencatat peristiwa dan kesalahan dalam indeks. |
|
### IndexSettings() {#IndexSettings--}
```
public IndexSettings()
```


Menginisialisasi sebuah instance baru dari kelas IndexSettings.


### getInMemoryIndex() {#getInMemoryIndex--}
```
public final boolean getInMemoryIndex()
```


Mendapatkan nilai yang menunjukkan apakah indeks disimpan di memori atau di disk.


**Returns:**
boolean - Nilai yang menunjukkan apakah indeks disimpan di memori atau di disk.

### getUseStopWords() {#getUseStopWords--}
```
public final boolean getUseStopWords()
```


Mendapatkan nilai yang menunjukkan apakah menggunakan stop words atau tidak. Nilai default adalah  true .


**Returns:**
boolean - Nilai yang menunjukkan apakah menggunakan stop words atau tidak.

### setUseStopWords(boolean value) {#setUseStopWords-boolean-}
```
public final void setUseStopWords(boolean value)
```


Mengatur nilai yang menunjukkan apakah menggunakan stop words atau tidak. Nilai default adalah  true .


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | boolean | Nilai yang menunjukkan apakah menggunakan stop words atau tidak. |
|

### getMaxIndexingReportCount() {#getMaxIndexingReportCount--}
```
public final int getMaxIndexingReportCount()
```


Mendapatkan jumlah maksimum laporan pengindeksan. Nilai default adalah  5 .


**Returns:**
int - Jumlah maksimum laporan pengindeksan.

### setMaxIndexingReportCount(int value) {#setMaxIndexingReportCount-int-}
```
public final void setMaxIndexingReportCount(int value)
```


Mengatur jumlah maksimum laporan pengindeksan. Nilai default adalah  5 .


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | int | Jumlah maksimum laporan pengindeksan. |
|

### getMaxSearchReportCount() {#getMaxSearchReportCount--}
```
public final int getMaxSearchReportCount()
```


Mendapatkan jumlah maksimum laporan pencarian. Nilai default adalah  10 .


**Returns:**
int - Jumlah maksimum laporan pencarian.

### setMaxSearchReportCount(int value) {#setMaxSearchReportCount-int-}
```
public final void setMaxSearchReportCount(int value)
```


Mengatur jumlah maksimum laporan pencarian. Nilai default adalah  10 .


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | int | Jumlah maksimum laporan pencarian. |
|

### getUseCharacterReplacements() {#getUseCharacterReplacements--}
```
public final boolean getUseCharacterReplacements()
```


Mendapatkan nilai yang menunjukkan apakah menggunakan penggantian karakter atau tidak. Nilai default adalah  false .


**Returns:**
boolean - Nilai yang menunjukkan apakah menggunakan penggantian karakter atau tidak.

### setUseCharacterReplacements(boolean value) {#setUseCharacterReplacements-boolean-}
```
public final void setUseCharacterReplacements(boolean value)
```


Mengatur nilai yang menunjukkan apakah menggunakan penggantian karakter atau tidak. Nilai default adalah  false .


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | boolean | Nilai yang menunjukkan apakah menggunakan penggantian karakter atau tidak. |
|

### getDocumentFilter() {#getDocumentFilter--}
```
public final DocumentFilter getDocumentFilter()
```


Mendapatkan filter dokumen. DocumentFilter bekerja pada logika inklusi. Gunakan kelas DocumentFilter untuk membuat instance filter dokumen. Nilai default adalah null, yang berarti semua dokumen yang ditambahkan diindeks.


**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - The document filter.

Contoh ini menunjukkan cara mengatur filter dokumen.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Membuat filter yang melewati dokumen dengan ekstensi '.doc', '.docx', '.rtf'
IndexSettings settings = new IndexSettings();
DocumentFilter fileExtensionFilter = DocumentFilter.createFileExtension(".doc", ".docx", ".rtf"); // Membuat filter ekstensi file
DocumentFilter invertedFilter = DocumentFilter.createNot(fileExtensionFilter); // Membalikkan filter ekstensi file
settings.setDocumentFilter(invertedFilter);
// Membuat indeks di folder yang ditentukan
Index index = new Index(indexFolder, settings);
// Mengindeks dokumen
index.add(documentsFolder);
// Mencari
SearchResult result = index.search("Einstein");
 
```
 
````


### setDocumentFilter(DocumentFilter value) {#setDocumentFilter-com.groupdocs.search.DocumentFilter-}
```
public final void setDocumentFilter(DocumentFilter value)
```


Menetapkan filter dokumen. DocumentFilter bekerja pada logika inklusi. Gunakan kelas GroupDocs.Search.Options.DocumentFilter untuk membuat instance filter dokumen. Nilai default adalah null, yang berarti semua dokumen yang ditambahkan diindeks.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | value | [DocumentFilter](../../com.groupdocs.search/documentfilter) | Filter dokumen. |

Contoh ini menunjukkan cara mengatur filter dokumen.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Membuat filter yang melewati dokumen dengan ekstensi '.doc', '.docx', '.rtf'
IndexSettings settings = new IndexSettings();
DocumentFilter fileExtensionFilter = DocumentFilter.createFileExtension(".doc", ".docx", ".rtf"); // Membuat filter ekstensi file
DocumentFilter invertedFilter = DocumentFilter.createNot(fileExtensionFilter); // Membalikkan filter ekstensi file
settings.setDocumentFilter(invertedFilter);
// Membuat indeks di folder yang ditentukan
Index index = new Index(indexFolder, settings);
// Mengindeks dokumen
index.add(documentsFolder);
// Mencari
SearchResult result = index.search("Einstein");
 
```
 
````

|

### getTextStorageSettings() {#getTextStorageSettings--}
```
public final TextStorageSettings getTextStorageSettings()
```


Mendapatkan pengaturan penyimpanan teks. Nilai default adalah null, yang berarti teks dokumen tidak disimpan.


**Returns:**
[TextStorageSettings](../../com.groupdocs.search.options/textstoragesettings) - The text storage settings.

Contoh ini menunjukkan cara mengatur pengaturan penyimpanan teks.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Membuat instance pengaturan indeks
IndexSettings settings = new IndexSettings();
settings.setTextStorageSettings(new TextStorageSettings(Compression.High)); // Mengatur tingkat kompresi tinggi untuk penyimpanan teks indeks
// Membuat indeks di folder yang ditentukan
Index index = new Index(indexFolder, settings);
// Mengindeks dokumen
index.add(documentsFolder);
// Mencari
SearchResult result = index.search("Einstein");
 
```
 
````


### setTextStorageSettings(TextStorageSettings value) {#setTextStorageSettings-com.groupdocs.search.options.TextStorageSettings-}
```
public final void setTextStorageSettings(TextStorageSettings value)
```


Menetapkan pengaturan penyimpanan teks. Nilai default adalah null, yang berarti teks dokumen tidak disimpan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | value | [TextStorageSettings](../../com.groupdocs.search.options/textstoragesettings) | Pengaturan penyimpanan teks. |

Contoh ini menunjukkan cara mengatur pengaturan penyimpanan teks.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Membuat instance pengaturan indeks
IndexSettings settings = new IndexSettings();
settings.setTextStorageSettings(new TextStorageSettings(Compression.High)); // Mengatur tingkat kompresi tinggi untuk penyimpanan teks indeks
// Membuat indeks di folder yang ditentukan
Index index = new Index(indexFolder, settings);
// Mengindeks dokumen
index.add(documentsFolder);
// Mencari
SearchResult result = index.search("Einstein");
 
```
 
````

|

### getIndexType() {#getIndexType--}
```
public final IndexType getIndexType()
```


Mendapatkan tipe indeks. Nilai default adalah GroupDocs.Search.Options.IndexType.NormalIndex.


**Returns:**
[IndexType](../../com.groupdocs.search.options/indextype) - The index type.

### setIndexType(IndexType value) {#setIndexType-com.groupdocs.search.options.IndexType-}
```
public final void setIndexType(IndexType value)
```


Menetapkan tipe indeks. Nilai default adalah GroupDocs.Search.Options.IndexType.NormalIndex.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | value | [IndexType](../../com.groupdocs.search.options/indextype) | Tipe indeks. |
|

### getSearchThreads() {#getSearchThreads--}
```
public final NumberOfThreads getSearchThreads()
```


Mengetahui jumlah thread yang digunakan untuk pencarian. Nilai default adalah GroupDocs.Search.Options.NumberOfThreads.Default, yang berarti pencarian akan dilakukan menggunakan jumlah thread yang sama dengan jumlah core prosesor.


**Returns:**
[NumberOfThreads](../../com.groupdocs.search.options/numberofthreads) - The number of threads used for the search.

### setSearchThreads(NumberOfThreads value) {#setSearchThreads-com.groupdocs.search.options.NumberOfThreads-}
```
public final void setSearchThreads(NumberOfThreads value)
```


Menetapkan jumlah thread yang digunakan untuk pencarian. Nilai default adalah GroupDocs.Search.Options.NumberOfThreads.Default, yang berarti pencarian akan dilakukan menggunakan jumlah thread yang sama dengan jumlah core prosesor.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | value | [NumberOfThreads](../../com.groupdocs.search.options/numberofthreads) | Jumlah thread yang digunakan untuk pencarian. |
|

### getCustomExtractors() {#getCustomExtractors--}
```
public final CustomExtractorCollection getCustomExtractors()
```


Mendapatkan koleksi ekstraktor kustom. Contoh lengkap implementasi ekstraktor kustom disajikan dalam dokumentasi untuk antarmuka GroupDocs.Search.Common.IFieldExtractor.


**Returns:**
[CustomExtractorCollection](../../com.groupdocs.search.common/customextractorcollection) - The custom extractor collection.

### getLogger() {#getLogger--}
```
public final ILogger getLogger()
```


Mendapatkan logger yang digunakan untuk mencatat peristiwa dan kesalahan dalam indeks. Perhatikan bahwa logger tidak disimpan dan harus dibuat serta ditetapkan setiap kali indeks dibuat atau dimuat.


**Returns:**
[ILogger](../../com.groupdocs.search.common/ilogger) - A logger that is used for logging events and errors in the index.

### setLogger(ILogger value) {#setLogger-com.groupdocs.search.common.ILogger-}
```
public final void setLogger(ILogger value)
```


Mengatur logger yang digunakan untuk mencatat peristiwa dan kesalahan dalam indeks. Perhatikan bahwa logger tidak disimpan dan harus dibuat serta ditetapkan setiap kali indeks dibuat atau dimuat.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | value | [ILogger](../../com.groupdocs.search.common/ilogger) | Logger yang digunakan untuk mencatat peristiwa dan kesalahan dalam indeks. |
|

