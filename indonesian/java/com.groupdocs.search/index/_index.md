---
title: "Index"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili kelas utama untuk mengindeks dokumen dan mencari di dalamnya."
type: docs
weight: 17
url: /id/java/com.groupdocs.search/index/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable
```
public class Index implements Closeable
```

Mewakili kelas utama untuk mengindeks dokumen dan mencari di dalamnya.


**Learn more**

* [Creating an index](../https://docs.groupdocs.com/display/searchjava/Creating+an+index)
* [Indexing](../https://docs.groupdocs.com/display/searchjava/Indexing)
* [Searching](../https://docs.groupdocs.com/display/searchjava/Searching)


Contoh ini menunjukkan penggunaan tipikal kelas tersebut.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Membuat indeks di folder yang ditentukan
index.add(documentsFolder); // Mengindeks dokumen dari folder yang ditentukan
SearchResult result = index.search(query); // Mencari dalam indeks
 
```
 
````


## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [Index()](#Index--) | Menginisialisasi sebuah instance baru dari kelas  Index  dalam memori. |
|
|  | [Index(IndexSettings settings)](#Index-com.groupdocs.search.IndexSettings-) | Menginisialisasi sebuah instance baru dari kelas  Index  dalam memori dengan pengaturan indeks tertentu. |
|
|  | [Index(String indexFolder)](#Index-java.lang.String-) | Menginisialisasi sebuah instance baru dari kelas  Index  . |
|
|  | [Index(String indexFolder, IndexSettings settings)](#Index-java.lang.String-com.groupdocs.search.IndexSettings-) | Menginisialisasi instance baru dari |
Index
kelas.
|
|  | [Index(String indexFolder, boolean overwriteIfExists)](#Index-java.lang.String-boolean-) | Menginisialisasi instance baru dari |
Index
kelas.
|
|  | [Index(String indexFolder, IndexSettings settings, boolean overwriteIfExists)](#Index-java.lang.String-com.groupdocs.search.IndexSettings-boolean-) | Menginisialisasi instance baru dari |
Index
kelas.
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getEvents()](#getEvents--) | Mendapatkan hub acara untuk berlangganan ke acara. |
|
|  | [getIndexInfo()](#getIndexInfo--) | Mendapatkan informasi dasar tentang indeks. |
|
|  | [getRepository()](#getRepository--) | Mendapatkan objek repositori indeks jika indeks berada di dalamnya. |
|
|  | [getIndexSettings()](#getIndexSettings--) | Mendapatkan pengaturan indeks. |
|
|  | [getDictionaries()](#getDictionaries--) | Mendapatkan repositori kamus. |
|
|  | [close()](#close--) | Melepaskan semua sumber daya yang digunakan oleh |
Index
.
|
|  | [add(String path)](#add-java.lang.String-) | Melakukan operasi pengindeksan. |
|
|  | [add(String path, IndexingOptions options)](#add-java.lang.String-com.groupdocs.search.options.IndexingOptions-) | Melakukan operasi pengindeksan. |
|
|  | [add(String[] paths)](#add-java.lang.String---) | Melakukan operasi pengindeksan. |
|
|  | [add(String[] paths, IndexingOptions options)](#add-java.lang.String---com.groupdocs.search.options.IndexingOptions-) | Melakukan operasi pengindeksan. |
|
|  | [add(Document[] documents, IndexingOptions options)](#add-com.groupdocs.search.Document---com.groupdocs.search.options.IndexingOptions-) | Melakukan operasi pengindeksan. |
|
|  | [add(ExtractedData[] data, IndexingOptions options)](#add-com.groupdocs.search.ExtractedData---com.groupdocs.search.options.IndexingOptions-) | Melakukan operasi pengindeksan. |
|
|  | [update()](#update--) | Mengindeks ulang dokumen yang telah diubah atau dihapus sejak pembaruan terakhir. |
|
|  | [update(UpdateOptions options)](#update-com.groupdocs.search.options.UpdateOptions-) | Mengindeks ulang dokumen yang telah diubah atau dihapus sejak pembaruan terakhir. |
|
|  | [getIndexingReports()](#getIndexingReports--) | Mendapatkan laporan tentang operasi pengindeksan. |
|
|  | [getSearchReports()](#getSearchReports--) | Mendapatkan laporan tentang operasi pencarian. |
|
|  | [search(String query)](#search-java.lang.String-) | Mencari dalam indeks. |
|
|  | [search(String query, SearchOptions options)](#search-java.lang.String-com.groupdocs.search.options.SearchOptions-) | Mencari dalam indeks. |
|
|  | [search(SearchQuery query)](#search-com.groupdocs.search.SearchQuery-) | Mencari dalam indeks. |
|
|  | [search(SearchQuery query, SearchOptions options)](#search-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-) | Mencari dalam indeks. |
|
|  | [search(SearchImage image, ImageSearchOptions options)](#search-com.groupdocs.search.common.SearchImage-com.groupdocs.search.options.ImageSearchOptions-) | Melakukan pencarian gambar terbalik dalam indeks. |
|
|  | [searchNext(ChunkSearchToken chunkSearchToken)](#searchNext-com.groupdocs.search.common.ChunkSearchToken-) | Melanjutkan pencarian potongan yang dimulai dengan metode Search. |
|
|  | [searchNext(ChunkSearchToken chunkSearchToken, Cancellation cancellation)](#searchNext-com.groupdocs.search.common.ChunkSearchToken-com.groupdocs.search.common.Cancellation-) | Melanjutkan pencarian potongan yang dimulai dengan metode Search. |
|
|  | [optimize()](#optimize--) | Meminimalkan jumlah segmen indeks dengan menggabungkannya satu dengan yang lain. |
|
|  | [optimize(MergeOptions options)](#optimize-com.groupdocs.search.options.MergeOptions-) | Meminimalkan jumlah segmen indeks dengan menggabungkannya satu dengan yang lain. |
|
|  | [merge(Index index, MergeOptions options)](#merge-com.groupdocs.search.Index-com.groupdocs.search.options.MergeOptions-) | Menggabungkan indeks yang ditentukan ke dalam indeks saat ini. |
|
|  | [merge(IndexRepository repository, MergeOptions options)](#merge-com.groupdocs.search.IndexRepository-com.groupdocs.search.options.MergeOptions-) | Menggabungkan indeks dari repositori indeks yang ditentukan ke dalam indeks saat ini. |
|
|  | [highlight(FoundDocument document, Highlighter highlighter)](#highlight-com.groupdocs.search.results.FoundDocument-com.groupdocs.search.highlighters.Highlighter-) | Menghasilkan teks berformat HTML dengan istilah yang ditemukan disorot. |
|
|  | [highlight(FoundDocument document, Highlighter highlighter, HighlightOptions options)](#highlight-com.groupdocs.search.results.FoundDocument-com.groupdocs.search.highlighters.Highlighter-com.groupdocs.search.options.HighlightOptions-) | Menghasilkan teks berformat HTML dengan istilah yang ditemukan disorot. |
|
|  | [getIndexedDocuments()](#getIndexedDocuments--) | Mendapatkan array semua dokumen yang diindeks. |
|
|  | [getIndexedDocumentItems(DocumentInfo documentInfo)](#getIndexedDocumentItems-com.groupdocs.search.results.DocumentInfo-) | Mendapatkan array item dokumen. |
|
|  | [GetIndexedDocument(String documentKey)](#GetIndexedDocument-java.lang.String-) | Mendapatkan dokumen yang diindeks berdasarkan kunci dokumen. |
|
|  | [getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter)](#getDocumentText-com.groupdocs.search.results.DocumentInfo-com.groupdocs.search.common.OutputAdapter-) | Menghasilkan teks dokumen yang diindeks dan melewatkannya melalui adaptor output. |
|
|  | [getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter, TextOptions options)](#getDocumentText-com.groupdocs.search.results.DocumentInfo-com.groupdocs.search.common.OutputAdapter-com.groupdocs.search.options.TextOptions-) | Menghasilkan teks berformat HTML untuk dokumen yang diindeks dan mentransfernya melalui adaptor output. |
|
|  | [getIndexedPaths()](#getIndexedPaths--) | Mendapatkan array jalur yang diindeks - dokumen atau folder. |
|
|  | [delete(String[] paths, UpdateOptions options)](#delete-java.lang.String---com.groupdocs.search.options.UpdateOptions-) | Menghapus file atau folder yang diindeks dari indeks. |
|
|  | [delete(UpdateOptions options, String[] documentKeys)](#delete-com.groupdocs.search.options.UpdateOptions-java.lang.String---) | Menghapus dokumen yang diindeks dari aliran atau struktur. |
|
|  | [notifyIndex(Notification notification)](#notifyIndex-com.groupdocs.search.Notification-) | Melewatkan objek notifikasi yang ditentukan ke indeks untuk melakukan notifikasi. |
|
|  | [changeAttributes(AttributeChangeBatch batch)](#changeAttributes-com.groupdocs.search.common.AttributeChangeBatch-) | Menerapkan batch perubahan atribut yang ditentukan ke dokumen yang diindeks tanpa melakukan pengindeksan ulang selama operasi pembaruan. |
|
|  | [getAttributes(String path)](#getAttributes-java.lang.String-) | Mendapatkan semua atribut yang terkait dengan dokumen yang diindeks yang ditentukan. |
|
|  | [loadIntoMemoryCompletely(String indexFolder)](#loadIntoMemoryCompletely-java.lang.String-) | Memuat seluruh indeks ke memori. |
|
|  | [loadIntoMemoryCompletely(String indexFolder, IndexSettings settings)](#loadIntoMemoryCompletely-java.lang.String-com.groupdocs.search.IndexSettings-) | Memuat seluruh indeks ke memori. |
|
### Index() {#Index--}
```
public Index()
```


Menginisialisasi sebuah instance baru dari kelas  Index  dalam memori.


Contoh ini menunjukkan cara membuat indeks di memori tanpa menyimpan file ke disk.

````
 ```

Index index = new Index();
 
```
 
````



### Index(IndexSettings settings) {#Index-com.groupdocs.search.IndexSettings-}
```
public Index(IndexSettings settings)
```


Menginisialisasi sebuah instance baru dari kelas  Index  dalam memori dengan pengaturan indeks tertentu.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | Objek pengaturan indeks. |


Contoh ini menunjukkan cara membuat indeks di memori tanpa menyimpan file ke disk dengan pengaturan indeks tertentu.

````
 ```

IndexSettings settings = new IndexSettings();
settings.setIndexType(IndexType.CompactIndex);
Index index = new Index(settings);
 
```
 
````

|

### Index(String indexFolder) {#Index-java.lang.String-}
```
public Index(String indexFolder)
```


Menginisialisasi sebuah instance baru dari kelas  Index . Membuat indeks baru atau membuka indeks yang sudah ada di disk.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | indexFolder | java.lang.String | Jalur folder indeks. |


Contoh ini menunjukkan cara membuat indeks di disk atau membuka indeks yang sudah ada.

````
 ```

String indexFolder = "c:\\MyIndex\\";
Index index = new Index(indexFolder);
 
```
 
````

|

### Index(String indexFolder, IndexSettings settings) {#Index-java.lang.String-com.groupdocs.search.IndexSettings-}
```
public Index(String indexFolder, IndexSettings settings)
```


Menginisialisasi instance baru dari
Index
kelas.
Membuat indeks baru dengan pengaturan tertentu atau membuka indeks yang sudah ada di disk.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | indexFolder | java.lang.String | Jalur folder indeks. |
|
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | Objek pengaturan indeks. |

Contoh ini menunjukkan cara membuat indeks di disk dengan pengaturan indeks tertentu.

````
 ```

String indexFolder = "c:\\MyIndex\\";
IndexSettings settings = new IndexSettings();
settings.setIndexType(IndexType.CompactIndex);
Index index = new Index(indexFolder, settings);
 
```
 
````

|

### Index(String indexFolder, boolean overwriteIfExists) {#Index-java.lang.String-boolean-}
```
public Index(String indexFolder, boolean overwriteIfExists)
```


Menginisialisasi instance baru dari
Index
kelas.
Muat indeks yang sudah ada dari disk jika
overwriteIfExists
is
false
;
membuat indeks baru di disk sebaliknya.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | indexFolder | java.lang.String | Jalur folder indeks. |
|
|  | overwriteIfExists | boolean | Bendera untuk menimpa folder indeks. |

Contoh ini menunjukkan cara membuat indeks baru dalam folder yang sudah berisi indeks lain.

````
 ```

String indexFolder = "c:\\MyIndex\\";
Index index = new Index(indexFolder, true);
 
```
 
````

|

### Index(String indexFolder, IndexSettings settings, boolean overwriteIfExists) {#Index-java.lang.String-com.groupdocs.search.IndexSettings-boolean-}
```
public Index(String indexFolder, IndexSettings settings, boolean overwriteIfExists)
```


Menginisialisasi instance baru dari
Index
kelas.
Muat indeks yang sudah ada dari disk jika
overwriteIfExists
is
false
;
membuat indeks baru di disk dengan pengaturan indeks tertentu sebaliknya.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | indexFolder | java.lang.String | Jalur folder indeks. |
|
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | Objek pengaturan indeks. |
|
|  | overwriteIfExists | boolean | Bendera untuk menimpa folder indeks. |

Contoh ini menunjukkan cara membuat indeks di disk dengan pengaturan indeks tertentu.

````
 ```

String indexFolder = "c:\\MyIndex\\";
IndexSettings settings = new IndexSettings();
settings.setIndexType(IndexType.CompactIndex);
Index index = new Index(indexFolder, settings, true);
 
```
 
````

|

### getEvents() {#getEvents--}
```
public final EventHub getEvents()
```


Mendapatkan hub acara untuk berlangganan ke acara.


**Returns:**
[EventHub](../../com.groupdocs.search.events/eventhub) - The event hub for subscribing to events.

### getIndexInfo() {#getIndexInfo--}
```
public final IndexInfo getIndexInfo()
```


Mendapatkan informasi dasar tentang indeks.


**Returns:**
[IndexInfo](../../com.groupdocs.search.common/indexinfo) - The basic information on the index.

### getRepository() {#getRepository--}
```
public final IndexRepository getRepository()
```


Mendapatkan objek repositori indeks jika indeks berada di dalamnya.


**Returns:**
[IndexRepository](../../com.groupdocs.search/indexrepository) - The index repository object.

### getIndexSettings() {#getIndexSettings--}
```
public final IndexSettings getIndexSettings()
```


Mendapatkan pengaturan indeks.


**Returns:**
[IndexSettings](../../com.groupdocs.search/indexsettings) - The index settings.

### getDictionaries() {#getDictionaries--}
```
public final DictionaryRepository getDictionaries()
```


Mendapatkan repositori kamus.


**Returns:**
[DictionaryRepository](../../com.groupdocs.search.dictionaries/dictionaryrepository) - The dictionary repository.

### close() {#close--}
```
public final void close()
```


Melepaskan semua sumber daya yang digunakan oleh
Index
.


### add(String path) {#add-java.lang.String-}
```
public final void add(String path)
```


Melakukan operasi pengindeksan.
Menambahkan file atau folder dengan jalur absolut atau relatif.
Dokumen dari semua subfolder akan diindeks.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | path | java.lang.String | Jalur ke file atau folder yang akan diindeks. |

Contoh ini menunjukkan cara menambahkan dokumen ke indeks.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String folderPath = "c:\\MyDocuments\\";
String filePath = "c:\\Documents\\MyFile.txt";
Index index = new Index(indexFolder); // Membuat indeks di folder yang ditentukan
index.add(folderPath); // Mengindeks dokumen di folder yang ditentukan
index.add(filePath); // Mengindeks dokumen yang ditentukan
 
```
 
````

|

### add(String path, IndexingOptions options) {#add-java.lang.String-com.groupdocs.search.options.IndexingOptions-}
```
public final void add(String path, IndexingOptions options)
```


Melakukan operasi pengindeksan.
Menambahkan file atau folder dengan jalur absolut atau relatif.
Dokumen dari semua subfolder akan diindeks.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | path | java.lang.String | Jalur ke file atau folder yang akan diindeks. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | Opsi pengindeksan. |

Contoh ini menunjukkan cara menambahkan dokumen ke indeks dengan opsi pengindeksan tertentu.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String folderPath = "c:\\MyDocuments\\";
String filePath = "c:\\Documents\\MyFile.txt";
Index index = new Index(indexFolder); // Membuat indeks di folder yang ditentukan
IndexingOptions options = new IndexingOptions();
options.setThreads(2); // Mengatur jumlah thread pengindeksan
index.add(folderPath, options); // Mengindeks dokumen di folder yang ditentukan
index.add(filePath, options); // Mengindeks dokumen yang ditentukan
 
```
 
````

|

### add(String[] paths) {#add-java.lang.String---}
```
public final void add(String[] paths)
```


Melakukan operasi pengindeksan.
Menambahkan file atau folder dengan jalur absolut atau relatif.
Dokumen dari semua subfolder akan diindeks.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | jalur | java.lang.String[] | Jalur ke file atau folder yang akan diindeks. |

Contoh ini menunjukkan cara menambahkan dokumen ke indeks.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String folderPath = "c:\\MyDocuments\\";
String filePath = "c:\\Documents\\MyFile.txt";
Index index = new Index(indexFolder); // Membuat indeks di folder yang ditentukan
String[] paths = new String[] { folderPath, filePath };
index.add(paths); // Mengindeks dokumen pada jalur yang ditentukan
 
```
 
````

|

### add(String[] paths, IndexingOptions options) {#add-java.lang.String---com.groupdocs.search.options.IndexingOptions-}
```
public final void add(String[] paths, IndexingOptions options)
```


Melakukan operasi pengindeksan.
Menambahkan file atau folder dengan jalur absolut atau relatif.
Dokumen dari semua subfolder akan diindeks.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | jalur | java.lang.String[] | Jalur ke file atau folder yang akan diindeks. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | Opsi pengindeksan. |

Contoh ini menunjukkan cara menambahkan dokumen ke indeks dengan opsi pengindeksan tertentu.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String folderPath = "c:\\MyDocuments\\";
String filePath = "c:\\Documents\\MyFile.txt";
Index index = new Index(indexFolder); // Membuat indeks di folder yang ditentukan
IndexingOptions options = new IndexingOptions();
options.setThreads(2); // Mengatur jumlah thread pengindeksan
String[] paths = new String[] { folderPath, filePath };
index.add(paths, options); // Mengindeks dokumen pada jalur yang ditentukan
 
```
 
````

|

### add(Document[] documents, IndexingOptions options) {#add-com.groupdocs.search.Document---com.groupdocs.search.options.IndexingOptions-}
```
public final void add(Document[] documents, IndexingOptions options)
```


Melakukan operasi pengindeksan.
Menambahkan dokumen dari sistem file, aliran, atau struktur.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | documents | [Document\[\]](../../com.groupdocs.search/document) | Dokumen dari sistem file, aliran, atau struktur. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | Opsi pengindeksan. |
|

### add(ExtractedData[] data, IndexingOptions options) {#add-com.groupdocs.search.ExtractedData---com.groupdocs.search.options.IndexingOptions-}
```
public final void add(ExtractedData[] data, IndexingOptions options)
```


Melakukan operasi pengindeksan.
Menambahkan data yang diekstrak ke indeks.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | data | [ExtractedData\[\]](../../com.groupdocs.search/extracteddata) | Data yang diekstrak. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | Opsi pengindeksan. |
|

### update() {#update--}
```
public final void update()
```


Mengindeks ulang dokumen yang telah diubah atau dihapus sejak pembaruan terakhir.
Menambahkan file baru yang telah ditambahkan ke folder yang diindeks.

Contoh ini menunjukkan cara memperbarui indeks.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Membuat indeks di folder yang ditentukan
index.add(documentsFolder); // Mengindeks dokumen dari folder yang ditentukan
// Hapus dokumen dari folder dokumen atau ubah mereka atau tambahkan dokumen baru ke folder
index.update(); // Memperbarui indeks
 
```
 
````



### update(UpdateOptions options) {#update-com.groupdocs.search.options.UpdateOptions-}
```
public final void update(UpdateOptions options)
```


Mengindeks ulang dokumen yang telah diubah atau dihapus sejak pembaruan terakhir.
Menambahkan file baru yang telah ditambahkan ke folder yang diindeks.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | options | [UpdateOptions](../../com.groupdocs.search.options/updateoptions) | Opsi pembaruan. |

Contoh ini menunjukkan cara memperbarui indeks dengan opsi pembaruan tertentu.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Membuat indeks di folder yang ditentukan
index.add(documentsFolder); // Mengindeks dokumen dari folder yang ditentukan
// Hapus dokumen dari folder dokumen atau ubah mereka atau tambahkan dokumen baru ke folder
UpdateOptions options = new UpdateOptions();
options.setThreads(2); // Mengatur jumlah thread pengindeksan
index.update(options); // Memperbarui indeks
 
```
 
````

|

### getIndexingReports() {#getIndexingReports--}
```
public final IndexingReport[] getIndexingReports()
```


Mendapatkan laporan tentang operasi pengindeksan.


**Returns:**
com.groupdocs.search.common.IndexingReport[] - Laporan pengindeksan.

Contoh ini menunjukkan cara mendapatkan laporan pengindeksan.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Membuat indeks di folder yang ditentukan
index.add(documentsFolder); // Mengindeks dokumen dari folder yang ditentukan
IndexingReport[] reports = index.getIndexingReports(); // Mendapatkan laporan pengindeksan
 
```
 
````


### getSearchReports() {#getSearchReports--}
```
public final SearchReport[] getSearchReports()
```


Mendapatkan laporan tentang operasi pencarian.


**Returns:**
com.groupdocs.search.common.SearchReport[] - Laporan pencarian.

Contoh ini menunjukkan cara mendapatkan laporan pencarian.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query1 = "Einstein";
String query2 = "Newton";
Index index = new Index(indexFolder); // Membuat indeks di folder yang ditentukan
index.add(documentsFolder); // Mengindeks dokumen dari folder yang ditentukan
SearchResult result1 = index.search(query1); // Mencari
SearchResult result2 = index.search(query2);
SearchResult result3 = index.search(query1 + " & " + query2);
SearchReport[] reports = index.getSearchReports(); // Mendapatkan laporan pencarian
 
```
 
````


### search(String query) {#search-java.lang.String-}
```
public final SearchResult search(String query)
```


Mencari dalam indeks.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | query | java.lang.String | Kueri pencarian. |

Contoh berikut menunjukkan cara melakukan pencarian sederhana.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Membuat indeks di folder yang ditentukan
index.add(documentsFolder); // Mengindeks dokumen dari folder yang ditentukan
SearchResult result = index.search(query); // Mencari
 
```
 
````

Contoh berikut menunjukkan cara melakukan pencarian Regex.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Membuat indeks di folder yang ditentukan
index.add(documentsFolder); // Mengindeks dokumen dari folder yang ditentukan
String query = "^[0-9]{3,}"; // Simbol caret di awal kueri pencarian memberi tahu indeks bahwa itu adalah kueri Regex
SearchResult result = index.search(query); // Mencari
 
```
 
````

Contoh berikut menunjukkan cara melakukan pencarian berfaset.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Membuat indeks di folder yang ditentukan
index.add(documentsFolder); // Mengindeks dokumen dari folder yang ditentukan
String query = "content:Newton"; // Kata sebelum titik dua dalam kueri berarti nama bidang dokumen yang akan dicari
SearchResult result = index.search(query); // Mencari
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(String query, SearchOptions options) {#search-java.lang.String-com.groupdocs.search.options.SearchOptions-}
```
public final SearchResult search(String query, SearchOptions options)
```


Mencari dalam indeks.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | query | java.lang.String | Kueri pencarian. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | Opsi pencarian. |

Contoh berikut menunjukkan cara melakukan pencarian fuzzy.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Membuat indeks di folder yang ditentukan
index.add(documentsFolder); // Mengindeks dokumen dari folder yang ditentukan
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // Mengaktifkan pencarian fuzzy
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1)); // Mengatur jumlah perbedaan yang mungkin untuk setiap kata
// Tanda kutip ganda di awal dan akhir memberi tahu indeks bahwa itu adalah kueri pencarian frasa
String query = "\"The Pursuit of Happiness\"";
SearchResult result = index.search(query, options); // Mencari
 
```
 
````

Contoh berikut menunjukkan cara melakukan pencarian sinonim.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Membuat indeks di folder yang ditentukan
index.add(documentsFolder); // Mengindeks dokumen dari folder yang ditentukan
SearchOptions options = new SearchOptions();
options.setUseSynonymSearch(true); // Mengaktifkan pencarian sinonim
String query = "cry";
SearchResult result = index.search(query, options); // Mencari
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchQuery query) {#search-com.groupdocs.search.SearchQuery-}
```
public final SearchResult search(SearchQuery query)
```


Mencari dalam indeks.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | Kueri pencarian. |

Contoh berikut menunjukkan cara melakukan pencarian menggunakan kueri dalam bentuk objek.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Membuat indeks di folder yang ditentukan
index.add(documentsFolder); // Mengindeks dokumen dari folder yang ditentukan
// Membuat subkueri 1
SearchQuery subquery1 = SearchQuery.createWordQuery("accommodation");
subquery1.setSearchOptions(new SearchOptions()); // Mengatur opsi pencarian hanya untuk subquery 1
subquery1.getSearchOptions().getFuzzySearch().setEnabled(true); // Mengaktifkan pencarian fuzzy
subquery1.getSearchOptions().getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3)); // Mengatur jumlah perbedaan maksimum
// Membuat subquery 2
SearchQuery subquery2 = SearchQuery.createNumericRangeQuery(1, 1000000);
// Membuat subquery 3
SearchQuery subquery3 = SearchQuery.createRegexQuery(\"(.)\\\\1\");
// Menggabungkan subquery menjadi satu kueri
SearchQuery query = SearchQuery.createPhraseSearchQuery(subquery1, subquery2, subquery3);
SearchResult result = index.search(query); // Mencari
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchQuery query, SearchOptions options) {#search-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-}
```
public final SearchResult search(SearchQuery query, SearchOptions options)
```


Mencari dalam indeks.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | Kueri pencarian. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | Opsi pencarian. |

Contoh berikut menunjukkan cara melakukan pencarian menggunakan kueri dalam bentuk objek.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Membuat indeks di folder yang ditentukan
index.add(documentsFolder); // Mengindeks dokumen dari folder yang ditentukan
// Membuat subquery pencarian rentang tanggal
SearchQuery subquery1 = SearchQuery.createDateRangeQuery(new Date(2011, 6, 17), new Date(2013, 1, 1));
// Membuat subquery wildcard dengan jumlah kata yang terlewat dari 0 hingga 2
SearchQuery subquery2 = SearchQuery.createWildcardQuery(0, 2);
// Membuat subquery kata sederhana
SearchQuery subquery3 = SearchQuery.createWordQuery("birth");
subquery3.setSearchOptions(new SearchOptions()); // Mengatur opsi pencarian hanya untuk subquery 3
subquery3.getSearchOptions().getFuzzySearch().setEnabled(true);
subquery3.getSearchOptions().getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1));
// Menggabungkan subquery menjadi satu kueri
SearchQuery query = SearchQuery.createPhraseSearchQuery(subquery1, subquery2, subquery3);
// Membuat objek opsi pencarian dengan kapasitas temuan yang meningkat
SearchOptions options = new SearchOptions(); // Opsi pencarian keseluruhan
options.setMaxOccurrenceCountPerTerm(1000000);
options.setMaxTotalOccurrenceCount(10000000);
SearchResult result = index.search(query, options); // Mencari
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchImage image, ImageSearchOptions options) {#search-com.groupdocs.search.common.SearchImage-com.groupdocs.search.options.ImageSearchOptions-}
```
public final ImageSearchResult search(SearchImage image, ImageSearchOptions options)
```


Melakukan pencarian gambar terbalik dalam indeks.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | image | [SearchImage](../../com.groupdocs.search.common/searchimage) | Gambar yang akan dicari. |
|
|  | options | [ImageSearchOptions](../../com.groupdocs.search.options/imagesearchoptions) | Opsi pencarian gambar. |
|

**Returns:**
[ImageSearchResult](../../com.groupdocs.search.results/imagesearchresult) - The result of a reverse image search.

### searchNext(ChunkSearchToken chunkSearchToken) {#searchNext-com.groupdocs.search.common.ChunkSearchToken-}
```
public final SearchResult searchNext(ChunkSearchToken chunkSearchToken)
```


Melanjutkan pencarian potongan yang dimulai dengan metode Search.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | chunkSearchToken | [ChunkSearchToken](../../com.groupdocs.search.common/chunksearchtoken) | Token pencarian chunk. |

Contoh ini menunjukkan cara melakukan pencarian chunk.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Membuat indeks di folder yang ditentukan
index.add(documentsFolder); // Mengindeks dokumen dari folder yang ditentukan
SearchOptions options = new SearchOptions();
options.setChunkSearch(true); // Mengaktifkan pencarian chunk
SearchResult result = index.search(query, options); // Memulai pencarian chunk
System.out.println(\"Jumlah dokumen: \" + result.getDocumentCount());
System.out.println(\"Jumlah kemunculan: \" + result.getOccurrenceCount());
while (result.getNextChunkSearchToken() != null) {
result = index.searchNext(result.getNextChunkSearchToken()); // Melanjutkan pencarian chunk
System.out.println(\"Jumlah dokumen: \" + result.getDocumentCount());
System.out.println(\"Jumlah kemunculan: \" + result.getOccurrenceCount());
}
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### searchNext(ChunkSearchToken chunkSearchToken, Cancellation cancellation) {#searchNext-com.groupdocs.search.common.ChunkSearchToken-com.groupdocs.search.common.Cancellation-}
```
public final SearchResult searchNext(ChunkSearchToken chunkSearchToken, Cancellation cancellation)
```


Melanjutkan pencarian potongan yang dimulai dengan metode Search.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | chunkSearchToken | [ChunkSearchToken](../../com.groupdocs.search.common/chunksearchtoken) | Token pencarian chunk. |
|
|  | cancellation | [Cancellation](../../com.groupdocs.search.common/cancellation) | Objek pembatalan. |

Contoh ini menunjukkan cara melakukan pencarian menggunakan query dalam bentuk objek.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Membuat indeks di folder yang ditentukan
index.add(documentsFolder); // Mengindeks dokumen dari folder yang ditentukan
Cancellation cancellation = new Cancellation(); // Objek pembatalan ini menghentikan semua kelanjutan pencarian jika dibatalkan
SearchOptions options = new SearchOptions();
options.setChunkSearch(true); // Mengaktifkan pencarian chunk
options.setCancellation(cancellation);
SearchResult result = index.search(query, options); // Memulai pencarian chunk
System.out.println(\"Jumlah dokumen: \" + result.getDocumentCount());
System.out.println(\"Jumlah kemunculan: \" + result.getOccurrenceCount());
while (result.getNextChunkSearchToken() != null) {
result = index.searchNext(result.getNextChunkSearchToken(), cancellation); // Melanjutkan pencarian chunk
System.out.println(\"Jumlah dokumen: \" + result.getDocumentCount());
System.out.println(\"Jumlah kemunculan: \" + result.getOccurrenceCount());
}
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### optimize() {#optimize--}
```
public final void optimize()
```


Meminimalkan jumlah segmen indeks dengan menggabungkannya satu dengan yang lain.
Operasi ini meningkatkan kinerja pencarian.

Contoh ini menunjukkan cara menggabungkan segmen indeks.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder1 = \"c:\\\\MyDocuments1\\\\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
String documentsFolder3 = "c:\\MyDocuments3\\";
Index index = new Index(indexFolder); // Membuat indeks di folder yang ditentukan
index.add(documentsFolder1); // Mengindeks dokumen dari folder yang ditentukan
index.add(documentsFolder2); // Setiap pemanggilan AddToIndex membuat setidaknya satu segmen baru dalam indeks
index.add(documentsFolder3);
// Menggabungkan segmen indeks
index.optimize();
 
```
 
````



### optimize(MergeOptions options) {#optimize-com.groupdocs.search.options.MergeOptions-}
```
public final void optimize(MergeOptions options)
```


Meminimalkan jumlah segmen indeks dengan menggabungkannya satu dengan yang lain.
Operasi ini meningkatkan kinerja pencarian.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | options | [MergeOptions](../../com.groupdocs.search.options/mergeoptions) | Opsi penggabungan. |

Contoh ini menunjukkan cara menggabungkan segmen indeks dengan opsi penggabungan tertentu.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder1 = \"c:\\\\MyDocuments1\\\\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
String documentsFolder3 = "c:\\MyDocuments3\\";
Index index = new Index(indexFolder); // Membuat indeks di folder yang ditentukan
index.add(documentsFolder1); // Mengindeks dokumen dari folder yang ditentukan
index.add(documentsFolder2); // Setiap pemanggilan AddToIndex membuat setidaknya satu segmen baru dalam indeks
index.add(documentsFolder3);
MergeOptions options = new MergeOptions();
options.setAsync(true); // Operasi asinkron
options.setCancellation(new Cancellation()); // Membuat objek pembatalan
// Menggabungkan segmen indeks
index.optimize(options); // Metode ini akan mengembalikan kontrol sebelum operasi selesai
options.getCancellation().cancelAfter(10000); // Menetapkan durasi maksimum operasi menjadi 10 detik
 
```
 
````

|

### merge(Index index, MergeOptions options) {#merge-com.groupdocs.search.Index-com.groupdocs.search.options.MergeOptions-}
```
public final void merge(Index index, MergeOptions options)
```


Menggabungkan indeks yang ditentukan ke dalam indeks saat ini.
Catatan bahwa indeks lain tidak akan diubah.


Jika indeks lain memiliki versi sebelumnya, harus diperbarui sebelum digabungkan dengan
IndexUpdater
.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | index | [Index](../../com.groupdocs.search/index) | Indeks yang akan digabungkan ke dalamnya. |
|
|  | options | [MergeOptions](../../com.groupdocs.search.options/mergeoptions) | Opsi penggabungan. |

Contoh ini menunjukkan cara menggabungkan sebuah indeks ke dalam indeks saat ini.

````
 ```

String indexFolder1 = "c:\\MyIndex1\\";
String indexFolder2 = "c:\\MyIndex2\\";
String documentsFolder1 = \"c:\\\\MyDocuments1\\\\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
Index index1 = new Index(indexFolder1); // Membuat index1
index1.add(documentsFolder1); // Mengindeks dokumen
Index index2 = new Index(indexFolder2); // Membuat index2
index2.add(documentsFolder2); // Mengindeks dokumen
MergeOptions options = new MergeOptions();
options.setCancellation(new Cancellation()); // Membuat objek pembatalan
// Menggabungkan index2 ke index1. Catatan bahwa berkas index2 tidak akan diubah.
index1.merge(index2, options);
 
```
 
````

|

### merge(IndexRepository repository, MergeOptions options) {#merge-com.groupdocs.search.IndexRepository-com.groupdocs.search.options.MergeOptions-}
```
public final void merge(IndexRepository repository, MergeOptions options)
```


Menggabungkan indeks dari repositori indeks yang ditentukan ke dalam indeks saat ini.
Catatan bahwa indeks dalam repositori tidak akan diubah.


Jika indeks lain memiliki versi sebelumnya, mereka harus diperbarui sebelum digabungkan dengan
IndexUpdater
.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | repository | [IndexRepository](../../com.groupdocs.search/indexrepository) | Repositori indeks untuk digabungkan ke dalam. |
|
|  | options | [MergeOptions](../../com.groupdocs.search.options/mergeoptions) | Opsi penggabungan. |

Contoh ini menunjukkan cara menggabungkan repositori indeks ke dalam indeks saat ini.

````
 ```

String indexFolder1 = "c:\\MyIndex1\\";
String indexFolder2 = "c:\\MyIndex2\\";
String indexFolder3 = "c:\\MyIndex3\\";
String documentsFolder1 = \"c:\\\\MyDocuments1\\\\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
String documentsFolder3 = "c:\\MyDocuments3\\";
Index index1 = new Index(indexFolder1); // Membuat index1
index1.add(documentsFolder1); // Mengindeks dokumen
IndexRepository repository = new IndexRepository(); // Membuat repositori indeks
Index index2 = repository.create(indexFolder2); // Membuat index2
index2.add(documentsFolder2); // Mengindeks dokumen
Index index3 = repository.create(indexFolder3); // Membuat index3
index3.add(documentsFolder3); // Mengindeks dokumen
MergeOptions options = new MergeOptions();
options.setCancellation(new Cancellation()); // Membuat objek pembatalan
// Menggabungkan semua indeks dalam repositori indeks ke index1. Catatan bahwa index2 dan index3 tidak akan diubah.
index1.merge(repository, options);
 
```
 
````

|

### highlight(FoundDocument document, Highlighter highlighter) {#highlight-com.groupdocs.search.results.FoundDocument-com.groupdocs.search.highlighters.Highlighter-}
```
public final void highlight(FoundDocument document, Highlighter highlighter)
```


Menghasilkan teks berformat HTML dengan istilah yang ditemukan disorot.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | document | [FoundDocument](../../com.groupdocs.search.results/founddocument) | Dokumen yang ditemukan. |
|
|  | highlighter | [Highlighter](../../com.groupdocs.search.highlighters/highlighter) | Penyorot hasil pencarian. |

Contoh ini menunjukkan cara menyorot kemunculan dalam teks berformat HTML.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentFolder = "c:\\MyDocuments\\";
// Membuat sebuah indeks
Index index = new Index(indexFolder);
// Mengindeks dokumen dari folder yang ditentukan
index.add(documentFolder);
// Mencari kata 'eternity'
SearchResult result = index.search("eternity");
// Menyorot kemunculan dalam teks
if (result.getDocumentCount() > 0) {
FoundDocument document = result.getFoundDocument(0); // Mendapatkan dokumen pertama yang ditemukan
OutputAdapter outputAdapter = new FileOutputAdapter("c:\\Highlighted.html"); // Membuat adapter output ke file
Highlighter highlighter = new HtmlHighlighter(outputAdapter); // Membuat objek penyorot
index.highlight(document, highlighter); // Menghasilkan teks berformat HTML dengan kemunculan yang disorot
}
 
```
 
````

|

### highlight(FoundDocument document, Highlighter highlighter, HighlightOptions options) {#highlight-com.groupdocs.search.results.FoundDocument-com.groupdocs.search.highlighters.Highlighter-com.groupdocs.search.options.HighlightOptions-}
```
public final void highlight(FoundDocument document, Highlighter highlighter, HighlightOptions options)
```


Menghasilkan teks berformat HTML dengan istilah yang ditemukan disorot.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | document | [FoundDocument](../../com.groupdocs.search.results/founddocument) | Dokumen yang ditemukan. |
|
|  | highlighter | [Highlighter](../../com.groupdocs.search.highlighters/highlighter) | Penyorot hasil pencarian. |
|
|  | options | [HighlightOptions](../../com.groupdocs.search.options/highlightoptions) | Opsi sorotan. |

Contoh ini menunjukkan cara menyorot kemunculan dalam teks berformat HTML.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentFolder = "c:\\MyDocuments\\";
// Membuat sebuah indeks
Index index = new Index(indexFolder);
// Mengindeks dokumen dari folder yang ditentukan
index.add(documentFolder);
// Mencari kata 'eternity'
SearchResult result = index.search("eternity");
// Menyorot kemunculan dalam teks
if (result.getDocumentCount() > 0) {
FoundDocument document = result.getFoundDocument(0); // Mendapatkan dokumen pertama yang ditemukan
OutputAdapter outputAdapter = new FileOutputAdapter("c:\\Highlighted.html"); // Membuat adapter output ke file
Highlighter highlighter = new HtmlHighlighter(outputAdapter); // Membuat objek penyorot
HighlightOptions options = new HighlightOptions(); // Membuat objek opsi sorotan
options.setTermsBefore(5);
options.setTermsAfter(5);
options.setTermsTotal(15);
index.highlight(document, highlighter, options); // Menghasilkan teks berformat HTML dengan kemunculan yang disorot
}
 
```
 
````

|

### getIndexedDocuments() {#getIndexedDocuments--}
```
public final DocumentInfo[] getIndexedDocuments()
```


Mendapatkan array semua dokumen yang diindeks.


**Returns:**
com.groupdocs.search.results.DocumentInfo[] - Sebuah array dari semua dokumen yang diindeks.

Contoh ini menunjukkan cara mendapatkan daftar dokumen yang diindeks dari sebuah indeks.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Membuat indeks di folder yang ditentukan
Index index = new Index(indexFolder);
// Mengindeks dokumen dari folder yang ditentukan
index.add(documentsFolder);
// Mendapatkan daftar dokumen yang diindeks
DocumentInfo[] documents = index.getIndexedDocuments();
 
```
 
````


### getIndexedDocumentItems(DocumentInfo documentInfo) {#getIndexedDocumentItems-com.groupdocs.search.results.DocumentInfo-}
```
public final DocumentInfo[] getIndexedDocumentItems(DocumentInfo documentInfo)
```


Mendapatkan array item dokumen.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | documentInfo | [DocumentInfo](../../com.groupdocs.search.results/documentinfo) | Sebuah info dokumen. |

Contoh ini menunjukkan cara mendapatkan daftar item dari sebuah dokumen yang diindeks dari sebuah indeks.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Membuat indeks di folder yang ditentukan
Index index = new Index(indexFolder);
// Mengindeks dokumen dari folder yang ditentukan
index.add(documentsFolder);
// Mendapatkan daftar dokumen yang diindeks
DocumentInfo[] documents = index.getIndexedDocuments();
for (int i = 0; i < documents.length; i++) {
DocumentInfo document = documents[i];
System.out.println(document.getFilePath());
DocumentInfo[] items = index.getIndexedDocumentItems(document); // Mendapatkan daftar item dokumen
for (int j = 0; j < items.length; j++) {
DocumentInfo item = items[j];
System.out.println("\t" + item.getInnerPath());
}
}
 
```
 
````

|

**Returns:**
com.groupdocs.search.results.DocumentInfo[] - Sebuah array dari item dokumen.

### GetIndexedDocument(String documentKey) {#GetIndexedDocument-java.lang.String-}
```
public DocumentInfo GetIndexedDocument(String documentKey)
```


Mendapatkan dokumen yang diindeks berdasarkan kunci dokumen.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | documentKey | java.lang.String | Kunci dokumen. |
|

**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - The indexed document.

### getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter) {#getDocumentText-com.groupdocs.search.results.DocumentInfo-com.groupdocs.search.common.OutputAdapter-}
```
public final void getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter)
```


Menghasilkan teks dokumen yang diindeks dan melewatkannya melalui adaptor output.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | documentInfo | [DocumentInfo](../../com.groupdocs.search.results/documentinfo) | Info dokumen yang diindeks. |
|
|  | adapter | [OutputAdapter](../../com.groupdocs.search.common/outputadapter) | Adapter output. |

Contoh ini menunjukkan cara mendapatkan teks dari sebuah dokumen yang diindeks dari sebuah indeks.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Membuat indeks di folder yang ditentukan
Index index = new Index(indexFolder);
// Mengindeks dokumen dari folder yang ditentukan
index.add(documentsFolder);
// Mendapatkan daftar dokumen yang diindeks
DocumentInfo[] documents = index.getIndexedDocuments();
// Mendapatkan teks dokumen
if (documents.length > 0) {
FileOutputAdapter outputAdapter = new FileOutputAdapter("C:\\Text.html");
index.getDocumentText(documents[0], outputAdapter);
}
 
```
 
````

|

### getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter, TextOptions options) {#getDocumentText-com.groupdocs.search.results.DocumentInfo-com.groupdocs.search.common.OutputAdapter-com.groupdocs.search.options.TextOptions-}
```
public final void getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter, TextOptions options)
```


Menghasilkan teks berformat HTML untuk dokumen yang diindeks dan mentransfernya melalui adaptor output.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | documentInfo | [DocumentInfo](../../com.groupdocs.search.results/documentinfo) | Info dokumen yang diindeks. |
|
|  | adapter | [OutputAdapter](../../com.groupdocs.search.common/outputadapter) | Adapter output. |
|
|  | options | [TextOptions](../../com.groupdocs.search.options/textoptions) | Opsi pengambilan teks. |
|

### getIndexedPaths() {#getIndexedPaths--}
```
public final String[] getIndexedPaths()
```


Mendapatkan array jalur yang diindeks - dokumen atau folder.


**Returns:**
java.lang.String[] - Sebuah array dari jalur terindeks.

### delete(String[] paths, UpdateOptions options) {#delete-java.lang.String---com.groupdocs.search.options.UpdateOptions-}
```
public final DeleteResult delete(String[] paths, UpdateOptions options)
```


Menghapus file atau folder yang terindeks dari indeks. Kemudian memperbarui indeks tanpa jalur yang dihapus.
Catatan bahwa dokumen individu tidak dapat dihapus dari indeks jika ditambahkan ke indeks sebagai bagian dari folder.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | jalur | java.lang.String[] | Jalur ke file atau folder yang akan dihapus. |
|
|  | options | [UpdateOptions](../../com.groupdocs.search.options/updateoptions) | Opsi pembaruan. |

Contoh ini menunjukkan cara menghapus jalur terindeks dari indeks.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder1 = "c:\\MyDocuments\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
// Membuat indeks di folder yang ditentukan
Index index = new Index(indexFolder);
// Mengindeks dokumen dari folder yang ditentukan
index.add(documentsFolder1);
index.add(documentsFolder2);
// Mendapatkan jalur terindeks dari indeks
String[] indexedPaths1 = index.getIndexedPaths();
// Menulis jalur terindeks ke konsol
System.out.println("Jalur terindeks:");
for (String path : indexedPaths1) {
System.out.println("\t" + path);
}
// Menghapus jalur indeks dari indeks
DeleteResult deleteResult = index.delete(new String[] { documentsFolder1 }, new UpdateOptions());
// Mendapatkan jalur terindeks setelah penghapusan
String[] indexedPaths2 = index.getIndexedPaths();
System.out.println("\nJalur yang dihapus: " + deleteResult.getSuccessCount());
System.out.println("\nJalur terindeks:");
for (String path : indexedPaths2) {
System.out.println("\t" + path);
}
 
```
 
````

|

**Returns:**
[DeleteResult](../../com.groupdocs.search.results/deleteresult) - An object describing the result of deleting files or folders from the index.

### delete(UpdateOptions options, String[] documentKeys) {#delete-com.groupdocs.search.options.UpdateOptions-java.lang.String---}
```
public final DeleteResult delete(UpdateOptions options, String[] documentKeys)
```


Menghapus dokumen yang diindeks dari aliran atau struktur. Kemudian memperbarui indeks tanpa dokumen yang dihapus.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | options | [UpdateOptions](../../com.groupdocs.search.options/updateoptions) | Opsi pembaruan. |
|
|  | documentKeys | java.lang.String[] | Kunci dokumen yang ditambahkan dari aliran atau struktur. |
|

**Returns:**
[DeleteResult](../../com.groupdocs.search.results/deleteresult) - An object describing the result of deleting documents from the index.

### notifyIndex(Notification notification) {#notifyIndex-com.groupdocs.search.Notification-}
```
public final boolean notifyIndex(Notification notification)
```


Melewatkan objek notifikasi yang ditentukan ke indeks untuk melakukan notifikasi.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | notification | [Notification](../../com.groupdocs.search/notification) | Objek notifikasi. |
|

**Returns:**
boolean - Mengembalikan  true  jika notifikasi berhasil dilakukan; sebaliknya  false .

### changeAttributes(AttributeChangeBatch batch) {#changeAttributes-com.groupdocs.search.common.AttributeChangeBatch-}
```
public final void changeAttributes(AttributeChangeBatch batch)
```


Menerapkan batch perubahan atribut yang ditentukan ke dokumen yang diindeks tanpa melakukan pengindeksan ulang selama operasi pembaruan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | batch | [AttributeChangeBatch](../../com.groupdocs.search.common/attributechangebatch) | Batch perubahan atribut. |
|

### getAttributes(String path) {#getAttributes-java.lang.String-}
```
public final String[] getAttributes(String path)
```


Mendapatkan semua atribut yang terkait dengan dokumen yang diindeks yang ditentukan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | path | java.lang.String | Jalur dokumen. |
|

**Returns:**
java.lang.String[] - Atribut yang terkait dengan dokumen.

### loadIntoMemoryCompletely(String indexFolder) {#loadIntoMemoryCompletely-java.lang.String-}
```
public static Index loadIntoMemoryCompletely(String indexFolder)
```


Memuat seluruh indeks ke memori.
Setiap perubahan pada indeks tidak secara otomatis disimpan ke folder asli.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | indexFolder | java.lang.String | Jalur folder indeks. |
|

**Returns:**
[Index](../../com.groupdocs.search/index) - The loaded in-memory index.

### loadIntoMemoryCompletely(String indexFolder, IndexSettings settings) {#loadIntoMemoryCompletely-java.lang.String-com.groupdocs.search.IndexSettings-}
```
public static Index loadIntoMemoryCompletely(String indexFolder, IndexSettings settings)
```


Memuat seluruh indeks ke memori.
Setiap perubahan pada indeks tidak secara otomatis disimpan ke folder asli.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | indexFolder | java.lang.String | Jalur folder indeks. |
|
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | Objek pengaturan indeks. |
|

**Returns:**
[Index](../../com.groupdocs.search/index) - The loaded in-memory index.

