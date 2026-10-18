---
title: "IndexRepository"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Birden çok indeksi birleştirmek ve onlarda ortak işlemler gerçekleştirmek için bir kapsayıcıyı temsil eder."
type: docs
weight: 18
url: /tr/java/com.groupdocs.search/indexrepository/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable
```
public class IndexRepository implements Closeable
```

Birden çok indeksi birleştirmek ve onlarda ortak işlemler gerçekleştirmek için bir kapsayıcıyı temsil eder.


**Learn more**

* [Search index repository](../https://docs.groupdocs.com/display/searchjava/Search+index+repository)


Örnek, sınıfın tipik bir kullanımını gösterir.

````
 ```

String indexFolder1 = "c:\\MyIndex\\";
String indexFolder2 = "c:\\MyIndex\\";
String query = "Einstein";
IndexRepository repository = new IndexRepository();
repository.addToRepository(indexFolder1); // Mevcut bir dizini yüklüyor
repository.addToRepository(indexFolder2); // Başka bir mevcut dizini yüklüyor
SearchResult result = repository.search(query); // Depodaki dizinlerde arama yapıyor
 
```
 
````


## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [IndexRepository()](#IndexRepository--) | Yeni bir örnek başlatır |
IndexRepository
sınıf.
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getEvents()](#getEvents--) | Etkinliklere abone olmak için olay merkezini alır. |
|
|  | [getIndexes()](#getIndexes--) | Bu içinde bulunan dizinleri alır |
IndexRepository
.
|
|  | [close()](#close--) | Tarafından kullanılan tüm kaynakları serbest bırakır |
IndexRepository
.
|
|  | [create()](#create--) | Bellekte yeni bir dizin oluşturur. |
|
|  | [create(IndexSettings settings)](#create-com.groupdocs.search.IndexSettings-) | Bellekte yeni bir dizin oluşturur. |
|
|  | [create(String indexFolder)](#create-java.lang.String-) | Diskte yeni bir dizin oluşturur. |
|
|  | [create(String indexFolder, IndexSettings settings)](#create-java.lang.String-com.groupdocs.search.IndexSettings-) | Diskte yeni bir dizin oluşturur. |
|
|  | [addToRepository(Index index)](#addToRepository-com.groupdocs.search.Index-) | Bir dizini indeks deposuna ekler. |
|
|  | [addToRepository(String indexFolder)](#addToRepository-java.lang.String-) | Bir dizini açar ve indeks deposuna ekler. |
|
|  | [update()](#update--) | Depodaki tüm dizinleri günceller. |
|
|  | [update(UpdateOptions options)](#update-com.groupdocs.search.options.UpdateOptions-) | Depodaki tüm dizinleri günceller. |
|
|  | [search(String query)](#search-java.lang.String-) | Depodaki tüm indekslerde arama yapar. |
|
|  | [search(String query, SearchOptions options)](#search-java.lang.String-com.groupdocs.search.options.SearchOptions-) | Depodaki tüm indekslerde arama yapar. |
|
|  | [search(SearchQuery query)](#search-com.groupdocs.search.SearchQuery-) | Depodaki tüm indekslerde arama yapar. |
|
|  | [search(SearchQuery query, SearchOptions options)](#search-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-) | Depodaki tüm indekslerde arama yapar. |
|
### IndexRepository() {#IndexRepository--}
```
public IndexRepository()
```


Yeni bir örnek başlatır
IndexRepository
sınıf.


### getEvents() {#getEvents--}
```
public final EventHub getEvents()
```


Etkinliklere abone olmak için olay merkezini alır.


**Returns:**
[EventHub](../../com.groupdocs.search.events/eventhub) - The event hub for subscribing to events.

### getIndexes() {#getIndexes--}
```
public final Index[] getIndexes()
```


Bu içinde bulunan dizinleri alır
IndexRepository
.


**Returns:**
com.groupdocs.search.Index[] - İndeksler.

### close() {#close--}
```
public final void close()
```


Tarafından kullanılan tüm kaynakları serbest bırakır
IndexRepository
.


### create() {#create--}
```
public final Index create()
```


Bellekte yeni bir dizin oluşturur.


**Returns:**
[Index](../../com.groupdocs.search/index) - The created index.

Örnek, indeks deposu aracılığıyla bellekte bir indeks oluşturmayı gösterir.

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


Bellekte yeni bir dizin oluşturur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | İndeks ayarları. |

Örnek, indeks deposu aracılığıyla bellekte bir indeks oluşturmayı gösterir.

````
 ```

IndexRepository indexRepository = new IndexRepository();
IndexSettings settings = new IndexSettings();
settings.setUseStopWords(false); // İndeksleme sırasında durak kelimelerinin kullanımını devre dışı bırakma
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


Diskte yeni bir dizin oluşturur.
İndeks klasörü, indeks oluşturulmadan önce temizlenecek.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | indexFolder | java.lang.String | İndeks klasörü. |

Örnek, indeks deposu aracılığıyla diskte bir indeks oluşturmayı gösterir.

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


Diskte yeni bir dizin oluşturur.
İndeks klasörü, indeks oluşturulmadan önce temizlenecek.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | indexFolder | java.lang.String | İndeks klasörü. |
|
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | İndeks ayarları. |

Örnek, indeks deposu aracılığıyla diskte bir indeks oluşturmayı gösterir.

````
 ```

String indexFolder = "c:\\MyIndex\\";
IndexRepository indexRepository = new IndexRepository();
IndexSettings settings = new IndexSettings();
settings.setUseStopWords(false); // İndeksleme sırasında durak kelimelerinin kullanımını devre dışı bırakma
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


Bir dizini indeks deposuna ekler.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | index | [Index](../../com.groupdocs.search/index) | Eklenecek indeks. |

Örnek, bir indeksi indeks deposuna eklemeyi gösterir.

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


Bir dizini açar ve indeks deposuna ekler.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | indexFolder | java.lang.String | İndeks klasörü. |

Örnek, bir indeksi indeks deposuna eklemeyi gösterir.

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


Depodaki tüm dizinleri günceller.

Örnek, depodaki indeksleri güncellemeyi gösterir.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // İndeks oluşturuluyor
index.add(documentsFolder); // Belgeleri indeksleme
// Belgeleri belgeler klasöründen silin veya değiştirin veya klasöre yeni belgeler ekleyin
repository.update();
 
```
 
````



### update(UpdateOptions options) {#update-com.groupdocs.search.options.UpdateOptions-}
```
public final void update(UpdateOptions options)
```


Depodaki tüm dizinleri günceller.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | options | [UpdateOptions](../../com.groupdocs.search.options/updateoptions) | Güncelleme seçenekleri. |

Örnek, depodaki indeksleri güncellemeyi gösterir.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // İndeks oluşturuluyor
index.add(documentsFolder); // Belgeleri indeksleme
// Belgeleri belgeler klasöründen silin veya değiştirin veya klasöre yeni belgeler ekleyin
UpdateOptions options = new UpdateOptions();
options.setThreads(2); // İndeksleme iş parçacığı sayısını ayarlama
repository.update(options);
 
```
 
````

|

### search(String query) {#search-java.lang.String-}
```
public final SearchResult search(String query)
```


Depodaki tüm indekslerde arama yapar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | query | java.lang.String | Arama sorgusu. |

Örnek, indeks deposunda arama nasıl yapılacağını gösterir.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // İndeks oluşturuluyor
index.add(documentsFolder); // Belgeleri indeksleme
SearchResult result = repository.search(query); // Arama
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(String query, SearchOptions options) {#search-java.lang.String-com.groupdocs.search.options.SearchOptions-}
```
public final SearchResult search(String query, SearchOptions options)
```


Depodaki tüm indekslerde arama yapar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | query | java.lang.String | Arama sorgusu. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | Arama seçenekleri. |

Örnek, indeks deposunda arama nasıl yapılacağını gösterir.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // İndeks oluşturuluyor
index.add(documentsFolder); // Belgeleri indeksleme
SearchOptions options = new SearchOptions();
options.setUseCaseSensitiveSearch(true); // Büyük/küçük harfe duyarlı arama bayrağını ayarlama
SearchResult result = repository.search(query, options); // Arama
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchQuery query) {#search-com.groupdocs.search.SearchQuery-}
```
public final SearchResult search(SearchQuery query)
```


Depodaki tüm indekslerde arama yapar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | Arama sorgusu. |

Örnek, indeks deposunda arama nasıl yapılacağını gösterir.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // İndeks oluşturuluyor
index.add(documentsFolder); // Belgeleri indeksleme
SearchQuery query = SearchQuery.createWordQuery("Einstein"); // Nesne biçiminde arama sorgusu oluşturma
SearchResult result = repository.search(query); // Arama
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchQuery query, SearchOptions options) {#search-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-}
```
public final SearchResult search(SearchQuery query, SearchOptions options)
```


Depodaki tüm indekslerde arama yapar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | Arama sorgusu. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | Arama seçenekleri. |

Örnek, indeks deposunda arama nasıl yapılacağını gösterir.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // İndeks oluşturuluyor
index.add(documentsFolder); // Belgeleri indeksleme
SearchOptions options = new SearchOptions();
options.setUseCaseSensitiveSearch(true); // Büyük/küçük harfe duyarlı arama bayrağını ayarlama
SearchQuery query = SearchQuery.createWordQuery("Einstein"); // Nesne biçiminde arama sorgusu oluşturma
SearchResult result = repository.search(query, options); // Arama
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

