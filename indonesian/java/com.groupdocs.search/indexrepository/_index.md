---
title: "IndexRepository"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili wadah untuk menggabungkan beberapa indeks dan melakukan operasi umum pada mereka."
type: docs
weight: 18
url: /id/java/com.groupdocs.search/indexrepository/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable
```
public class IndexRepository implements Closeable
```

Mewakili wadah untuk menggabungkan beberapa indeks dan melakukan operasi umum pada mereka.


**Learn more**

* [Search index repository](../https://docs.groupdocs.com/display/searchjava/Search+index+repository)


Contoh ini menunjukkan penggunaan tipikal kelas tersebut.

````
 ```

String indexFolder1 = "c:\\MyIndex\\";
String indexFolder2 = "c:\\MyIndex\\";
String query = "Einstein";
IndexRepository repository = new IndexRepository();
repository.addToRepository(indexFolder1); // Memuat indeks yang ada
repository.addToRepository(indexFolder2); // Memuat indeks lain yang ada
SearchResult result = repository.search(query); // Mencari dalam indeks repositori
 
```
 
````


## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [IndexRepository()](#IndexRepository--) | Menginisialisasi instance baru dari |
IndexRepository
kelas.
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getEvents()](#getEvents--) | Mendapatkan hub acara untuk berlangganan ke acara. |
|
|  | [getIndexes()](#getIndexes--) | Mendapatkan indeks yang terkandung di dalam ini |
IndexRepository
.
|
|  | [close()](#close--) | Melepaskan semua sumber daya yang digunakan oleh |
IndexRepository
.
|
|  | [create()](#create--) | Membuat indeks baru di memori. |
|
|  | [create(IndexSettings settings)](#create-com.groupdocs.search.IndexSettings-) | Membuat indeks baru di memori. |
|
|  | [create(String indexFolder)](#create-java.lang.String-) | Membuat indeks baru di disk. |
|
|  | [create(String indexFolder, IndexSettings settings)](#create-java.lang.String-com.groupdocs.search.IndexSettings-) | Membuat indeks baru di disk. |
|
|  | [addToRepository(Index index)](#addToRepository-com.groupdocs.search.Index-) | Menambahkan indeks ke repositori indeks. |
|
|  | [addToRepository(String indexFolder)](#addToRepository-java.lang.String-) | Membuka dan menambahkan indeks ke repositori indeks. |
|
|  | [update()](#update--) | Memperbarui semua indeks dalam repositori. |
|
|  | [update(UpdateOptions options)](#update-com.groupdocs.search.options.UpdateOptions-) | Memperbarui semua indeks dalam repositori. |
|
|  | [search(String query)](#search-java.lang.String-) | Mencari di semua indeks repositori. |
|
|  | [search(String query, SearchOptions options)](#search-java.lang.String-com.groupdocs.search.options.SearchOptions-) | Mencari di semua indeks repositori. |
|
|  | [search(SearchQuery query)](#search-com.groupdocs.search.SearchQuery-) | Mencari di semua indeks repositori. |
|
|  | [search(SearchQuery query, SearchOptions options)](#search-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-) | Mencari di semua indeks repositori. |
|
### IndexRepository() {#IndexRepository--}
```
public IndexRepository()
```


Menginisialisasi instance baru dari
IndexRepository
kelas.


### getEvents() {#getEvents--}
```
public final EventHub getEvents()
```


Mendapatkan hub acara untuk berlangganan ke acara.


**Returns:**
[EventHub](../../com.groupdocs.search.events/eventhub) - The event hub for subscribing to events.

### getIndexes() {#getIndexes--}
```
public final Index[] getIndexes()
```


Mendapatkan indeks yang terkandung di dalam ini
IndexRepository
.


**Returns:**
com.groupdocs.search.Index[] - Indeks-indeks.

### close() {#close--}
```
public final void close()
```


Melepaskan semua sumber daya yang digunakan oleh
IndexRepository
.


### create() {#create--}
```
public final Index create()
```


Membuat indeks baru di memori.


**Returns:**
[Index](../../com.groupdocs.search/index) - The created index.

Contoh ini menunjukkan cara membuat indeks di memori melalui repositori indeks.

````
 ```

IndexRepository indexRepository = new IndexRepository();
Index index = indexRepository.create();
 
```
 
````


### create(IndexSettings settings) {#create-com.groupdocs.search.IndexSettings-}
```
public final Index create(IndexSettings settings)
```


Membuat indeks baru di memori.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | Pengaturan indeks. |

Contoh ini menunjukkan cara membuat indeks di memori melalui repositori indeks.

````
 ```

IndexRepository indexRepository = new IndexRepository();
IndexSettings settings = new IndexSettings();
settings.setUseStopWords(false); // Menonaktifkan penggunaan kata berhenti selama pengindeksan
Index index = indexRepository.create(settings);
 
```
 
````

|

**Returns:**
[Index](../../com.groupdocs.search/index) - The created index.

### create(String indexFolder) {#create-java.lang.String-}
```
public final Index create(String indexFolder)
```


Membuat indeks baru di disk.
Folder indeks akan dibersihkan sebelum pembuatan indeks.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | indexFolder | java.lang.String | Folder indeks. |

Contoh ini menunjukkan cara membuat indeks di disk melalui repositori indeks.

````
 ```

String indexFolder = "c:\\MyIndex\\";
IndexRepository indexRepository = new IndexRepository();
Index index = indexRepository.create(indexFolder);
 
```
 
````

|

**Returns:**
[Index](../../com.groupdocs.search/index) - The created index.

### create(String indexFolder, IndexSettings settings) {#create-java.lang.String-com.groupdocs.search.IndexSettings-}
```
public final Index create(String indexFolder, IndexSettings settings)
```


Membuat indeks baru di disk.
Folder indeks akan dibersihkan sebelum pembuatan indeks.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | indexFolder | java.lang.String | Folder indeks. |
|
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | Pengaturan indeks. |

Contoh ini menunjukkan cara membuat indeks di disk melalui repositori indeks.

````
 ```

String indexFolder = "c:\\MyIndex\\";
IndexRepository indexRepository = new IndexRepository();
IndexSettings settings = new IndexSettings();
settings.setUseStopWords(false); // Menonaktifkan penggunaan kata berhenti selama pengindeksan
Index index = indexRepository.create(indexFolder, settings);
 
```
 
````

|

**Returns:**
[Index](../../com.groupdocs.search/index) - The created index.

### addToRepository(Index index) {#addToRepository-com.groupdocs.search.Index-}
```
public final void addToRepository(Index index)
```


Menambahkan indeks ke repositori indeks.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | index | [Index](../../com.groupdocs.search/index) | Indeks yang akan ditambahkan. |

Contoh ini menunjukkan cara menambahkan indeks ke repositori indeks.

````
 ```

Index index = new Index();
IndexRepository indexRepository = new IndexRepository();
indexRepository.addToRepository(index);
 
```
 
````

|

### addToRepository(String indexFolder) {#addToRepository-java.lang.String-}
```
public final void addToRepository(String indexFolder)
```


Membuka dan menambahkan indeks ke repositori indeks.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | indexFolder | java.lang.String | Folder indeks. |

Contoh ini menunjukkan cara menambahkan indeks ke repositori indeks.

````
 ```

String indexFolder = "c:\\MyIndex\\";
IndexRepository indexRepository = new IndexRepository();
indexRepository.addToRepository(indexFolder);
 
```
 
````

|

### update() {#update--}
```
public final void update()
```


Memperbarui semua indeks dalam repositori.

Contoh ini menunjukkan cara memperbarui indeks dalam repositori.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // Membuat indeks
index.add(documentsFolder); // Mengindeks dokumen
// Hapus dokumen dari folder dokumen atau ubah mereka atau tambahkan dokumen baru ke folder
repository.update();
 
```
 
````



### update(UpdateOptions options) {#update-com.groupdocs.search.options.UpdateOptions-}
```
public final void update(UpdateOptions options)
```


Memperbarui semua indeks dalam repositori.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | options | [UpdateOptions](../../com.groupdocs.search.options/updateoptions) | Opsi pembaruan. |

Contoh ini menunjukkan cara memperbarui indeks dalam repositori.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // Membuat indeks
index.add(documentsFolder); // Mengindeks dokumen
// Hapus dokumen dari folder dokumen atau ubah mereka atau tambahkan dokumen baru ke folder
UpdateOptions options = new UpdateOptions();
options.setThreads(2); // Mengatur jumlah thread pengindeksan
repository.update(options);
 
```
 
````

|

### search(String query) {#search-java.lang.String-}
```
public final SearchResult search(String query)
```


Mencari di semua indeks repositori.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | query | java.lang.String | Kueri pencarian. |

Contoh ini menunjukkan cara melakukan pencarian dalam repositori indeks.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // Membuat indeks
index.add(documentsFolder); // Mengindeks dokumen
SearchResult result = repository.search(query); // Mencari
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(String query, SearchOptions options) {#search-java.lang.String-com.groupdocs.search.options.SearchOptions-}
```
public final SearchResult search(String query, SearchOptions options)
```


Mencari di semua indeks repositori.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | query | java.lang.String | Kueri pencarian. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | Opsi pencarian. |

Contoh ini menunjukkan cara melakukan pencarian dalam repositori indeks.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // Membuat indeks
index.add(documentsFolder); // Mengindeks dokumen
SearchOptions options = new SearchOptions();
options.setUseCaseSensitiveSearch(true); // Mengatur flag pencarian yang sensitif huruf
SearchResult result = repository.search(query, options); // Mencari
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchQuery query) {#search-com.groupdocs.search.SearchQuery-}
```
public final SearchResult search(SearchQuery query)
```


Mencari di semua indeks repositori.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | Kueri pencarian. |

Contoh ini menunjukkan cara melakukan pencarian dalam repositori indeks.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // Membuat indeks
index.add(documentsFolder); // Mengindeks dokumen
SearchQuery query = SearchQuery.createWordQuery("Einstein"); // Membuat kueri pencarian dalam bentuk objek
SearchResult result = repository.search(query); // Mencari
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchQuery query, SearchOptions options) {#search-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-}
```
public final SearchResult search(SearchQuery query, SearchOptions options)
```


Mencari di semua indeks repositori.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | Kueri pencarian. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | Opsi pencarian. |

Contoh ini menunjukkan cara melakukan pencarian dalam repositori indeks.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // Membuat indeks
index.add(documentsFolder); // Mengindeks dokumen
SearchOptions options = new SearchOptions();
options.setUseCaseSensitiveSearch(true); // Mengatur flag pencarian yang sensitif huruf
SearchQuery query = SearchQuery.createWordQuery("Einstein"); // Membuat kueri pencarian dalam bentuk objek
SearchResult result = repository.search(query, options); // Mencari
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

