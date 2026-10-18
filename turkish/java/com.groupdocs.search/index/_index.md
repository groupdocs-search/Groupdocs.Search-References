---
title: "Dizin"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Belgeleri indekslemek ve içinde arama yapmak için ana sınıfı temsil eder."
type: docs
weight: 17
url: /tr/java/com.groupdocs.search/index/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable
```
public class Index implements Closeable
```

Belgeleri indekslemek ve içinde arama yapmak için ana sınıfı temsil eder.


**Learn more**

* [Creating an index](../https://docs.groupdocs.com/display/searchjava/Creating+an+index)
* [Indexing](../https://docs.groupdocs.com/display/searchjava/Indexing)
* [Searching](../https://docs.groupdocs.com/display/searchjava/Searching)


Örnek, sınıfın tipik bir kullanımını gösterir.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Belirtilen klasörde indeks oluşturma
index.add(documentsFolder); // Belirtilen klasörden belgeleri indeksleme
SearchResult result = index.search(query); // Dizin içinde arama
 
```
 
````


## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [Index()](#Index--) | Bellekte Index sınıfının yeni bir örneğini başlatır. |
|
|  | [Index(IndexSettings settings)](#Index-com.groupdocs.search.IndexSettings-) | Bellekte belirli dizin ayarlarıyla Index sınıfının yeni bir örneğini başlatır. |
|
|  | [Index(String indexFolder)](#Index-java.lang.String-) | Index sınıfının yeni bir örneğini başlatır. |
|
|  | [Index(String indexFolder, IndexSettings settings)](#Index-java.lang.String-com.groupdocs.search.IndexSettings-) | Yeni bir örnek başlatır |
Dizin
sınıf.
|
|  | [Index(String indexFolder, boolean overwriteIfExists)](#Index-java.lang.String-boolean-) | Yeni bir örnek başlatır |
Dizin
sınıf.
|
|  | [Index(String indexFolder, IndexSettings settings, boolean overwriteIfExists)](#Index-java.lang.String-com.groupdocs.search.IndexSettings-boolean-) | Yeni bir örnek başlatır |
Dizin
sınıf.
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getEvents()](#getEvents--) | Etkinliklere abone olmak için olay merkezini alır. |
|
|  | [getIndexInfo()](#getIndexInfo--) | Dizinle ilgili temel bilgileri alır. |
|
|  | [getRepository()](#getRepository--) | Dizin içinde bulunuyorsa dizin depo nesnesini alır. |
|
|  | [getIndexSettings()](#getIndexSettings--) | Dizin ayarlarını alır. |
|
|  | [getDictionaries()](#getDictionaries--) | Sözlük deposunu alır. |
|
|  | [close()](#close--) | Tarafından kullanılan tüm kaynakları serbest bırakır |
Dizin
.
|
|  | [add(String path)](#add-java.lang.String-) | Dizinleme işlemini gerçekleştirir. |
|
|  | [add(String path, IndexingOptions options)](#add-java.lang.String-com.groupdocs.search.options.IndexingOptions-) | Dizinleme işlemini gerçekleştirir. |
|
|  | [add(String[] paths)](#add-java.lang.String---) | Dizinleme işlemini gerçekleştirir. |
|
|  | [add(String[] paths, IndexingOptions options)](#add-java.lang.String---com.groupdocs.search.options.IndexingOptions-) | Dizinleme işlemini gerçekleştirir. |
|
|  | [add(Document[] documents, IndexingOptions options)](#add-com.groupdocs.search.Document---com.groupdocs.search.options.IndexingOptions-) | Dizinleme işlemini gerçekleştirir. |
|
|  | [add(ExtractedData[] data, IndexingOptions options)](#add-com.groupdocs.search.ExtractedData---com.groupdocs.search.options.IndexingOptions-) | Dizinleme işlemini gerçekleştirir. |
|
|  | [update()](#update--) | Son güncellemeden beri değiştirilen veya silinen belgeleri yeniden dizinler. |
|
|  | [update(UpdateOptions options)](#update-com.groupdocs.search.options.UpdateOptions-) | Son güncellemeden beri değiştirilen veya silinen belgeleri yeniden dizinler. |
|
|  | [getIndexingReports()](#getIndexingReports--) | Dizinleme işlemleriyle ilgili raporları alır. |
|
|  | [getSearchReports()](#getSearchReports--) | Arama işlemleriyle ilgili raporları alır. |
|
|  | [search(String query)](#search-java.lang.String-) | Dizinde arama yapar. |
|
|  | [search(String query, SearchOptions options)](#search-java.lang.String-com.groupdocs.search.options.SearchOptions-) | Dizinde arama yapar. |
|
|  | [search(SearchQuery query)](#search-com.groupdocs.search.SearchQuery-) | Dizinde arama yapar. |
|
|  | [search(SearchQuery query, SearchOptions options)](#search-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-) | Dizinde arama yapar. |
|
|  | [search(SearchImage image, ImageSearchOptions options)](#search-com.groupdocs.search.common.SearchImage-com.groupdocs.search.options.ImageSearchOptions-) | Dizinde ters görüntü araması gerçekleştirir. |
|
|  | [searchNext(ChunkSearchToken chunkSearchToken)](#searchNext-com.groupdocs.search.common.ChunkSearchToken-) | Search yöntemiyle başlatılan parça aramasına devam eder. |
|
|  | [searchNext(ChunkSearchToken chunkSearchToken, Cancellation cancellation)](#searchNext-com.groupdocs.search.common.ChunkSearchToken-com.groupdocs.search.common.Cancellation-) | Search yöntemiyle başlatılan parça aramasına devam eder. |
|
|  | [optimize()](#optimize--) | Dizin segmentlerinin sayısını birbiriyle birleştirerek azaltır. |
|
|  | [optimize(MergeOptions options)](#optimize-com.groupdocs.search.options.MergeOptions-) | Dizin segmentlerinin sayısını birbiriyle birleştirerek azaltır. |
|
|  | [merge(Index index, MergeOptions options)](#merge-com.groupdocs.search.Index-com.groupdocs.search.options.MergeOptions-) | Belirtilen dizini mevcut dizine birleştirir. |
|
|  | [merge(IndexRepository repository, MergeOptions options)](#merge-com.groupdocs.search.IndexRepository-com.groupdocs.search.options.MergeOptions-) | Belirtilen indeks deposundan indeksleri mevcut indekse birleştirir. |
|
|  | [highlight(FoundDocument document, Highlighter highlighter)](#highlight-com.groupdocs.search.results.FoundDocument-com.groupdocs.search.highlighters.Highlighter-) | Bulunan terimleri vurgulayan HTML biçimlendirilmiş metin oluşturur. |
|
|  | [highlight(FoundDocument document, Highlighter highlighter, HighlightOptions options)](#highlight-com.groupdocs.search.results.FoundDocument-com.groupdocs.search.highlighters.Highlighter-com.groupdocs.search.options.HighlightOptions-) | Bulunan terimleri vurgulayan HTML biçimlendirilmiş metin oluşturur. |
|
|  | [getIndexedDocuments()](#getIndexedDocuments--) | Tüm indekslenmiş belgelerin bir dizisini alır. |
|
|  | [getIndexedDocumentItems(DocumentInfo documentInfo)](#getIndexedDocumentItems-com.groupdocs.search.results.DocumentInfo-) | Belge öğelerinin bir dizisini alır. |
|
|  | [GetIndexedDocument(String documentKey)](#GetIndexedDocument-java.lang.String-) | Belge anahtarına göre indekslenmiş bir belge alır. |
|
|  | [getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter)](#getDocumentText-com.groupdocs.search.results.DocumentInfo-com.groupdocs.search.common.OutputAdapter-) | İndekslenmiş bir belgenin metnini oluşturur ve bir çıktı adaptörü aracılığıyla iletir. |
|
|  | [getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter, TextOptions options)](#getDocumentText-com.groupdocs.search.results.DocumentInfo-com.groupdocs.search.common.OutputAdapter-com.groupdocs.search.options.TextOptions-) | İndekslenmiş belge için HTML biçimlendirilmiş metin oluşturur ve çıktı adaptörü aracılığıyla aktarır. |
|
|  | [getIndexedPaths()](#getIndexedPaths--) | İndekslenmiş yolların - belgelerin veya klasörlerin - bir dizisini alır. |
|
|  | [delete(String[] paths, UpdateOptions options)](#delete-java.lang.String---com.groupdocs.search.options.UpdateOptions-) | İndeksten indekslenmiş dosya veya klasörleri siler. |
|
|  | [delete(UpdateOptions options, String[] documentKeys)](#delete-com.groupdocs.search.options.UpdateOptions-java.lang.String---) | Akışlardan veya yapılarından indekslenmiş belgeleri siler. |
|
|  | [notifyIndex(Notification notification)](#notifyIndex-com.groupdocs.search.Notification-) | Belirtilen bildirim nesnesini bildirimi gerçekleştirmek için indekse iletir. |
|
|  | [changeAttributes(AttributeChangeBatch batch)](#changeAttributes-com.groupdocs.search.common.AttributeChangeBatch-) | Güncelleme işlemi sırasında yeniden indeksleme yapmadan, belirtilen öznitelik değişiklikleri topluluğunu indekslenmiş belgelere uygular. |
|
|  | [getAttributes(String path)](#getAttributes-java.lang.String-) | Belirtilen indekslenmiş belgeyle ilişkili tüm öznitelikleri alır. |
|
|  | [loadIntoMemoryCompletely(String indexFolder)](#loadIntoMemoryCompletely-java.lang.String-) | Tam indeksi belleğe yükler. |
|
|  | [loadIntoMemoryCompletely(String indexFolder, IndexSettings settings)](#loadIntoMemoryCompletely-java.lang.String-com.groupdocs.search.IndexSettings-) | Tam indeksi belleğe yükler. |
|
### Index() {#Index--}
```
public Index()
```


Bellekte Index sınıfının yeni bir örneğini başlatır.


Bu örnek, dosyaları diske kaydetmeden bellekte indeks oluşturmanın nasıl yapılacağını gösterir.

````
 ```

Index index = new Index();
 
```
 
````



### Index(IndexSettings settings) {#Index-com.groupdocs.search.IndexSettings-}
```
public Index(IndexSettings settings)
```


Bellekte belirli dizin ayarlarıyla Index sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | İndeks ayarları nesnesi. |


Bu örnek, belirli indeks ayarlarıyla dosyaları diske kaydetmeden bellekte indeks oluşturmanın nasıl yapılacağını gösterir.

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


Index sınıfının yeni bir örneğini başlatır. Diskte yeni bir indeks oluşturur veya mevcut bir indeksi açar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | indexFolder | java.lang.String | İndeks klasör yolu. |


Bu örnek, bir diskte indeks oluşturmanın veya mevcut bir indeksi açmanın nasıl yapılacağını gösterir.

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


Yeni bir örnek başlatır
Dizin
sınıf.
Belirli ayarlarla yeni bir indeks oluşturur veya diskte mevcut bir indeksi açar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | indexFolder | java.lang.String | İndeks klasör yolu. |
|
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | İndeks ayarları nesnesi. |

Bu örnek, belirli indeks ayarlarıyla bir diskte indeks oluşturmanın nasıl yapılacağını gösterir.

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


Yeni bir örnek başlatır
Dizin
sınıf.
Varolan bir dizini diskten yüklüyor eğer
overwriteIfExists
değerdir
false
;
Aksi takdirde diskte yeni bir dizin oluşturur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | indexFolder | java.lang.String | İndeks klasör yolu. |
|
|  | overwriteIfExists | boolean | Dizin klasörünün üzerine yazma bayrağı. |

Örnek, zaten başka bir dizin içeren bir klasörde yeni bir dizin nasıl oluşturulacağını gösterir.

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


Yeni bir örnek başlatır
Dizin
sınıf.
Varolan bir dizini diskten yüklüyor eğer
overwriteIfExists
değerdir
false
;
Aksi takdirde belirli dizin ayarlarıyla diskte yeni bir dizin oluşturur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | indexFolder | java.lang.String | İndeks klasör yolu. |
|
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | İndeks ayarları nesnesi. |
|
|  | overwriteIfExists | boolean | Dizin klasörünün üzerine yazma bayrağı. |

Bu örnek, belirli indeks ayarlarıyla bir diskte indeks oluşturmanın nasıl yapılacağını gösterir.

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


Etkinliklere abone olmak için olay merkezini alır.


**Returns:**
[EventHub](../../com.groupdocs.search.events/eventhub) - The event hub for subscribing to events.

### getIndexInfo() {#getIndexInfo--}
```
public final IndexInfo getIndexInfo()
```


Dizinle ilgili temel bilgileri alır.


**Returns:**
[IndexInfo](../../com.groupdocs.search.common/indexinfo) - The basic information on the index.

### getRepository() {#getRepository--}
```
public final IndexRepository getRepository()
```


Dizin içinde bulunuyorsa dizin depo nesnesini alır.


**Returns:**
[IndexRepository](../../com.groupdocs.search/indexrepository) - The index repository object.

### getIndexSettings() {#getIndexSettings--}
```
public final IndexSettings getIndexSettings()
```


Dizin ayarlarını alır.


**Returns:**
[IndexSettings](../../com.groupdocs.search/indexsettings) - The index settings.

### getDictionaries() {#getDictionaries--}
```
public final DictionaryRepository getDictionaries()
```


Sözlük deposunu alır.


**Returns:**
[DictionaryRepository](../../com.groupdocs.search.dictionaries/dictionaryrepository) - The dictionary repository.

### close() {#close--}
```
public final void close()
```


Tarafından kullanılan tüm kaynakları serbest bırakır
Dizin
.


### add(String path) {#add-java.lang.String-}
```
public final void add(String path)
```


Dizinleme işlemini gerçekleştirir.
Mutlak ya da göreceli bir yol ile bir dosya ya da klasör ekler.
Tüm alt klasörlerden belgeler dizine eklenecek.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | path | java.lang.String | Dizine eklenecek bir dosya ya da klasörün yolu. |

Örnek, belgelere bir dizine nasıl ekleneceğini gösterir.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String folderPath = "c:\\MyDocuments\\";
String filePath = "c:\\Documents\\MyFile.txt";
Index index = new Index(indexFolder); // Belirtilen klasörde indeks oluşturma
index.add(folderPath); // Belirtilen klasördeki belgeleri dizine ekleme
index.add(filePath); // Belirtilen belgeyi dizine ekleme
 
```
 
````

|

### add(String path, IndexingOptions options) {#add-java.lang.String-com.groupdocs.search.options.IndexingOptions-}
```
public final void add(String path, IndexingOptions options)
```


Dizinleme işlemini gerçekleştirir.
Mutlak ya da göreceli bir yol ile bir dosya ya da klasör ekler.
Tüm alt klasörlerden belgeler dizine eklenecek.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | path | java.lang.String | Dizine eklenecek bir dosya ya da klasörün yolu. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | Dizinleme seçenekleri. |

Örnek, belirli dizinleme seçenekleriyle belgelere bir dizine nasıl ekleneceğini gösterir.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String folderPath = "c:\\MyDocuments\\";
String filePath = "c:\\Documents\\MyFile.txt";
Index index = new Index(indexFolder); // Belirtilen klasörde indeks oluşturma
IndexingOptions options = new IndexingOptions();
options.setThreads(2); // İndeksleme iş parçacığı sayısını ayarlama
index.add(folderPath, options); // Belirtilen klasördeki belgeleri dizine ekleme
index.add(filePath, options); // Belirtilen belgeyi dizine ekleme
 
```
 
````

|

### add(String[] paths) {#add-java.lang.String---}
```
public final void add(String[] paths)
```


Dizinleme işlemini gerçekleştirir.
Dosyaları veya klasörleri mutlak ya da göreceli bir yol ile ekler.
Tüm alt klasörlerden belgeler dizine eklenecek.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | yollar | java.lang.String[] | İndekslenmesi gereken dosya veya klasörlerin yolları. |

Örnek, belgelere bir dizine nasıl ekleneceğini gösterir.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String folderPath = "c:\\MyDocuments\\";
String filePath = "c:\\Documents\\MyFile.txt";
Index index = new Index(indexFolder); // Belirtilen klasörde indeks oluşturma
String[] paths = new String[] { folderPath, filePath };
index.add(paths); // Belirtilen yollar üzerindeki belgeleri indeksleme
 
```
 
````

|

### add(String[] paths, IndexingOptions options) {#add-java.lang.String---com.groupdocs.search.options.IndexingOptions-}
```
public final void add(String[] paths, IndexingOptions options)
```


Dizinleme işlemini gerçekleştirir.
Dosyaları veya klasörleri mutlak ya da göreceli bir yol ile ekler.
Tüm alt klasörlerden belgeler dizine eklenecek.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | yollar | java.lang.String[] | İndekslenmesi gereken dosya veya klasörlerin yolları. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | Dizinleme seçenekleri. |

Örnek, belirli dizinleme seçenekleriyle belgelere bir dizine nasıl ekleneceğini gösterir.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String folderPath = "c:\\MyDocuments\\";
String filePath = "c:\\Documents\\MyFile.txt";
Index index = new Index(indexFolder); // Belirtilen klasörde indeks oluşturma
IndexingOptions options = new IndexingOptions();
options.setThreads(2); // İndeksleme iş parçacığı sayısını ayarlama
String[] paths = new String[] { folderPath, filePath };
index.add(paths, options); // Belirtilen yollar üzerindeki belgeleri indeksleme
 
```
 
````

|

### add(Document[] documents, IndexingOptions options) {#add-com.groupdocs.search.Document---com.groupdocs.search.options.IndexingOptions-}
```
public final void add(Document[] documents, IndexingOptions options)
```


Dizinleme işlemini gerçekleştirir.
Dosya sisteminden, akıştan veya yapısal kaynaktan belgeler ekler.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | documents | [Document\[\]](../../com.groupdocs.search/document) | Dosya sisteminden, akıştan veya yapısal kaynaktan belgeler. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | Dizinleme seçenekleri. |
|

### add(ExtractedData[] data, IndexingOptions options) {#add-com.groupdocs.search.ExtractedData---com.groupdocs.search.options.IndexingOptions-}
```
public final void add(ExtractedData[] data, IndexingOptions options)
```


Dizinleme işlemini gerçekleştirir.
Çıkarılan verileri indekse ekler.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | data | [ExtractedData\[\]](../../com.groupdocs.search/extracteddata) | Çıkarılan veri. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | Dizinleme seçenekleri. |
|

### update() {#update--}
```
public final void update()
```


Son güncellemeden beri değiştirilen veya silinen belgeleri yeniden dizinler.
İndekslenen klasörlere eklenen yeni dosyaları ekler.

Örnek, bir indeksi nasıl güncelleyeceğini gösterir.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Belirtilen klasörde indeks oluşturma
index.add(documentsFolder); // Belirtilen klasörden belgeleri indeksleme
// Belgeleri belgeler klasöründen silin veya değiştirin veya klasöre yeni belgeler ekleyin
index.update(); // İndeksi güncelleme
 
```
 
````



### update(UpdateOptions options) {#update-com.groupdocs.search.options.UpdateOptions-}
```
public final void update(UpdateOptions options)
```


Son güncellemeden beri değiştirilen veya silinen belgeleri yeniden dizinler.
İndekslenen klasörlere eklenen yeni dosyaları ekler.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | options | [UpdateOptions](../../com.groupdocs.search.options/updateoptions) | Güncelleme seçenekleri. |

Örnek, belirli güncelleme seçenekleriyle bir indeksi nasıl güncelleyeceğini gösterir.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Belirtilen klasörde indeks oluşturma
index.add(documentsFolder); // Belirtilen klasörden belgeleri indeksleme
// Belgeleri belgeler klasöründen silin veya değiştirin veya klasöre yeni belgeler ekleyin
UpdateOptions options = new UpdateOptions();
options.setThreads(2); // İndeksleme iş parçacığı sayısını ayarlama
index.update(options); // İndeksi güncelleme
 
```
 
````

|

### getIndexingReports() {#getIndexingReports--}
```
public final IndexingReport[] getIndexingReports()
```


Dizinleme işlemleriyle ilgili raporları alır.


**Returns:**
com.groupdocs.search.common.IndexingReport[] - İndeksleme raporları.

Örnek, indeksleme raporlarını nasıl alacağını gösterir.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Belirtilen klasörde indeks oluşturma
index.add(documentsFolder); // Belirtilen klasörden belgeleri indeksleme
IndexingReport[] reports = index.getIndexingReports(); // İndeksleme raporlarını alıyor
 
```
 
````


### getSearchReports() {#getSearchReports--}
```
public final SearchReport[] getSearchReports()
```


Arama işlemleriyle ilgili raporları alır.


**Returns:**
com.groupdocs.search.common.SearchReport[] - Arama raporları.

Örnek, arama raporlarını nasıl alacağını gösterir.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query1 = "Einstein";
String query2 = "Newton";
Index index = new Index(indexFolder); // Belirtilen klasörde indeks oluşturma
index.add(documentsFolder); // Belirtilen klasörden belgeleri indeksleme
SearchResult result1 = index.search(query1); // Arama
SearchResult result2 = index.search(query2); // Arama
SearchResult result3 = index.search(query1 + " & " + query2);
SearchReport[] reports = index.getSearchReports(); // Arama raporlarını alıyor
 
```
 
````


### search(String query) {#search-java.lang.String-}
```
public final SearchResult search(String query)
```


Dizinde arama yapar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | query | java.lang.String | Arama sorgusu. |

Aşağıdaki örnek basit aramanın nasıl yapılacağını gösterir.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Belirtilen klasörde indeks oluşturma
index.add(documentsFolder); // Belirtilen klasörden belgeleri indeksleme
SearchResult result = index.search(query); // Arama yapıyor
 
```
 
````

Aşağıdaki örnek Regex aramasının nasıl yapılacağını gösterir.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Belirtilen klasörde indeks oluşturma
index.add(documentsFolder); // Belirtilen klasörden belgeleri indeksleme
String query = "^[0-9]{3,}"; // Arama sorgusunun başındaki caret (^) sembolü, indeksin bunun bir Regex sorgusu olduğunu belirtir
SearchResult result = index.search(query); // Arama yapıyor
 
```
 
````

Aşağıdaki örnek katmanlı aramanın nasıl yapılacağını gösterir.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Belirtilen klasörde indeks oluşturma
index.add(documentsFolder); // Belirtilen klasörden belgeleri indeksleme
String query = "content:Newton"; // Sorgudaki iki nokta üstünden önceki kelime, aranacak belge alanının adını ifade eder
SearchResult result = index.search(query); // Arama yapıyor
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(String query, SearchOptions options) {#search-java.lang.String-com.groupdocs.search.options.SearchOptions-}
```
public final SearchResult search(String query, SearchOptions options)
```


Dizinde arama yapar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | query | java.lang.String | Arama sorgusu. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | Arama seçenekleri. |

Aşağıdaki örnek bulanık aramanın nasıl yapılacağını gösterir.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Belirtilen klasörde indeks oluşturma
index.add(documentsFolder); // Belirtilen klasörden belgeleri indeksleme
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // Bulanık aramayı etkinleştiriyor
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1)); // Her kelime için olası fark sayısını ayarlıyor
// Başındaki ve sonundaki çift tırnaklar, indeksin bunun bir ifade arama sorgusu olduğunu söyler
String query = "\"The Pursuit of Happiness\"";
SearchResult result = index.search(query, options); // Arama
 
```
 
````

Aşağıdaki örnek eşanlamlı aramanın nasıl yapılacağını gösterir.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Belirtilen klasörde indeks oluşturma
index.add(documentsFolder); // Belirtilen klasörden belgeleri indeksleme
SearchOptions options = new SearchOptions();
options.setUseSynonymSearch(true); // Eşanlamlı aramayı etkinleştiriyor
String query = "cry";
SearchResult result = index.search(query, options); // Arama
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchQuery query) {#search-com.groupdocs.search.SearchQuery-}
```
public final SearchResult search(SearchQuery query)
```


Dizinde arama yapar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | Arama sorgusu. |

Aşağıdaki örnek sorguyu nesne biçiminde kullanarak aramanın nasıl yapılacağını gösterir.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Belirtilen klasörde indeks oluşturma
index.add(documentsFolder); // Belirtilen klasörden belgeleri indeksleme
// Alt sorgu 1 oluşturuluyor
SearchQuery subquery1 = SearchQuery.createWordQuery("accommodation");
subquery1.setSearchOptions(new SearchOptions()); // Yalnızca alt sorgu 1 için arama seçeneklerini ayarlama
subquery1.getSearchOptions().getFuzzySearch().setEnabled(true); // Bulanık aramayı etkinleştiriyor
subquery1.getSearchOptions().getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3)); // Azami fark sayısını ayarlama
// Alt sorgu 2 oluşturuluyor
SearchQuery subquery2 = SearchQuery.createNumericRangeQuery(1, 1000000);
// Alt sorgu 3 oluşturuluyor
SearchQuery subquery3 = SearchQuery.createRegexQuery("(.)\\1");
// Alt sorguları tek bir sorguya birleştirir.
SearchQuery query = SearchQuery.createPhraseSearchQuery(subquery1, subquery2, subquery3);
SearchResult result = index.search(query); // Arama yapıyor
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchQuery query, SearchOptions options) {#search-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-}
```
public final SearchResult search(SearchQuery query, SearchOptions options)
```


Dizinde arama yapar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | Arama sorgusu. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | Arama seçenekleri. |

Aşağıdaki örnek sorguyu nesne biçiminde kullanarak aramanın nasıl yapılacağını gösterir.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Belirtilen klasörde indeks oluşturma
index.add(documentsFolder); // Belirtilen klasörden belgeleri indeksleme
// Tarih aralığı araması için alt sorgu oluşturma
SearchQuery subquery1 = SearchQuery.createDateRangeQuery(new Date(2011, 6, 17), new Date(2013, 1, 1));
// 0 ile 2 arasındaki eksik kelime sayısıyla joker karakter alt sorgusu oluşturma
SearchQuery subquery2 = SearchQuery.createWildcardQuery(0, 2);
// Basit kelime alt sorgusu oluşturma
SearchQuery subquery3 = SearchQuery.createWordQuery("birth");
subquery3.setSearchOptions(new SearchOptions()); // Yalnızca alt sorgu 3 için arama seçeneklerini ayarlama
subquery3.getSearchOptions().getFuzzySearch().setEnabled(true);
subquery3.getSearchOptions().getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1));
// Alt sorguları tek bir sorguya birleştirir.
SearchQuery query = SearchQuery.createPhraseSearchQuery(subquery1, subquery2, subquery3);
// Bulunan oluşların artırılmış kapasitesiyle arama seçenekleri nesnesi oluşturuluyor
SearchOptions options = new SearchOptions(); // Genel arama seçenekleri
options.setMaxOccurrenceCountPerTerm(1000000);
options.setMaxTotalOccurrenceCount(10000000);
SearchResult result = index.search(query, options); // Arama
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchImage image, ImageSearchOptions options) {#search-com.groupdocs.search.common.SearchImage-com.groupdocs.search.options.ImageSearchOptions-}
```
public final ImageSearchResult search(SearchImage image, ImageSearchOptions options)
```


Dizinde ters görüntü araması gerçekleştirir.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | image | [SearchImage](../../com.groupdocs.search.common/searchimage) | Aranacak görüntü. |
|
|  | options | [ImageSearchOptions](../../com.groupdocs.search.options/imagesearchoptions) | Görüntü arama seçenekleri. |
|

**Returns:**
[ImageSearchResult](../../com.groupdocs.search.results/imagesearchresult) - The result of a reverse image search.

### searchNext(ChunkSearchToken chunkSearchToken) {#searchNext-com.groupdocs.search.common.ChunkSearchToken-}
```
public final SearchResult searchNext(ChunkSearchToken chunkSearchToken)
```


Search yöntemiyle başlatılan parça aramasına devam eder.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | chunkSearchToken | [ChunkSearchToken](../../com.groupdocs.search.common/chunksearchtoken) | Parça arama belirteci. |

Örnek, parça aramanın nasıl yapılacağını gösterir.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Belirtilen klasörde indeks oluşturma
index.add(documentsFolder); // Belirtilen klasörden belgeleri indeksleme
SearchOptions options = new SearchOptions();
options.setChunkSearch(true); // Parça aramayı etkinleştiriyor
SearchResult result = index.search(query, options); // Parça aramayı başlatıyor
System.out.println("Document count: " + result.getDocumentCount());
System.out.println("Occurrence count: " + result.getOccurrenceCount());
while (result.getNextChunkSearchToken() != null) {
result = index.searchNext(result.getNextChunkSearchToken()); // Parça aramayı sürdürüyor
System.out.println("Document count: " + result.getDocumentCount());
System.out.println("Occurrence count: " + result.getOccurrenceCount());
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


Search yöntemiyle başlatılan parça aramasına devam eder.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | chunkSearchToken | [ChunkSearchToken](../../com.groupdocs.search.common/chunksearchtoken) | Parça arama belirteci. |
|
|  | cancellation | [Cancellation](../../com.groupdocs.search.common/cancellation) | İptal nesnesi. |

Örnek, sorguyu nesne biçiminde kullanarak aramanın nasıl yapılacağını gösterir.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Belirtilen klasörde indeks oluşturma
index.add(documentsFolder); // Belirtilen klasörden belgeleri indeksleme
Cancellation cancellation = new Cancellation(); // Bu iptal nesnesi, iptal edildiğinde tüm arama devamlarını durdurur
SearchOptions options = new SearchOptions();
options.setChunkSearch(true); // Parça aramayı etkinleştiriyor
options.setCancellation(cancellation);
SearchResult result = index.search(query, options); // Parça aramayı başlatıyor
System.out.println("Document count: " + result.getDocumentCount());
System.out.println("Occurrence count: " + result.getOccurrenceCount());
while (result.getNextChunkSearchToken() != null) {
result = index.searchNext(result.getNextChunkSearchToken(), cancellation); // Parça aramayı sürdürüyor
System.out.println("Document count: " + result.getDocumentCount());
System.out.println("Occurrence count: " + result.getOccurrenceCount());
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


Dizin segmentlerinin sayısını birbiriyle birleştirerek azaltır.
Bu işlem arama performansını artırır.

Örnek, bir dizinin segmentlerini nasıl birleştireceğini gösterir.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
String documentsFolder3 = "c:\\MyDocuments3\\";
Index index = new Index(indexFolder); // Belirtilen klasörde indeks oluşturma
index.add(documentsFolder1); // Belirtilen klasörden belgeler indeksleniyor
index.add(documentsFolder2); // AddToIndex'e yapılan her çağrı dizinde en az bir yeni segment oluşturur
index.add(documentsFolder3);
// Dizinin segmentlerini birleştirme
index.optimize();
 
```
 
````



### optimize(MergeOptions options) {#optimize-com.groupdocs.search.options.MergeOptions-}
```
public final void optimize(MergeOptions options)
```


Dizin segmentlerinin sayısını birbiriyle birleştirerek azaltır.
Bu işlem arama performansını artırır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | options | [MergeOptions](../../com.groupdocs.search.options/mergeoptions) | Birleştirme seçenekleri. |

Bu örnek, bir dizinin bölümlerini belirli birleştirme seçenekleriyle nasıl birleştireceğinizi gösterir.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
String documentsFolder3 = "c:\\MyDocuments3\\";
Index index = new Index(indexFolder); // Belirtilen klasörde indeks oluşturma
index.add(documentsFolder1); // Belirtilen klasörden belgeler indeksleniyor
index.add(documentsFolder2); // AddToIndex'e yapılan her çağrı dizinde en az bir yeni segment oluşturur
index.add(documentsFolder3);
MergeOptions options = new MergeOptions();
options.setAsync(true); // Asenkron işlem
options.setCancellation(new Cancellation()); // İptal nesnesi oluşturuluyor
// Dizinin segmentlerini birleştirme
index.optimize(options); // Bu yöntem, işlem tamamlanmadan önce dönecektir
options.getCancellation().cancelAfter(10000); // İşlemin maksimum süresi 10 saniye olarak ayarlanıyor
 
```
 
````

|

### merge(Index index, MergeOptions options) {#merge-com.groupdocs.search.Index-com.groupdocs.search.options.MergeOptions-}
```
public final void merge(Index index, MergeOptions options)
```


Belirtilen dizini mevcut dizine birleştirir.
Diğer dizinin değişmeyeceğini unutmayın.


Diğer dizinin önceki bir sürümü varsa, birleştirmeden önce güncellenmelidir
IndexUpdater
.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | index | [Index](../../com.groupdocs.search/index) | Birleştirilecek dizin. |
|
|  | options | [MergeOptions](../../com.groupdocs.search.options/mergeoptions) | Birleştirme seçenekleri. |

Bu örnek, bir dizini mevcut dizine nasıl birleştireceğinizi gösterir.

````
 ```

String indexFolder1 = "c:\\MyIndex1\\";
String indexFolder2 = "c:\\MyIndex2\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
Index index1 = new Index(indexFolder1); // index1 oluşturuluyor
index1.add(documentsFolder1); // Belgeler indeksleniyor
Index index2 = new Index(indexFolder2); // index2 oluşturuluyor
index2.add(documentsFolder2); // Belgeler indeksleniyor
MergeOptions options = new MergeOptions();
options.setCancellation(new Cancellation()); // İptal nesnesi oluşturuluyor
// index2'yi index1'e birleştiriliyor. index2 dosyalarının değişmeyeceğini unutmayın.
index1.merge(index2, options);
 
```
 
````

|

### merge(IndexRepository repository, MergeOptions options) {#merge-com.groupdocs.search.IndexRepository-com.groupdocs.search.options.MergeOptions-}
```
public final void merge(IndexRepository repository, MergeOptions options)
```


Belirtilen indeks deposundan indeksleri mevcut indekse birleştirir.
Depodaki dizinlerin değişmeyeceğini unutmayın.


Diğer dizinlerin önceki bir sürümü varsa, birleştirmeden önce güncellenmelidir
IndexUpdater
.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | repository | [IndexRepository](../../com.groupdocs.search/indexrepository) | Birleştirilecek dizin deposu. |
|
|  | options | [MergeOptions](../../com.groupdocs.search.options/mergeoptions) | Birleştirme seçenekleri. |

Bu örnek, bir dizin deposunu mevcut dizine nasıl birleştireceğinizi gösterir.

````
 ```

String indexFolder1 = "c:\\MyIndex1\\";
String indexFolder2 = "c:\\MyIndex2\\";
String indexFolder3 = "c:\\MyIndex3\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
String documentsFolder3 = "c:\\MyDocuments3\\";
Index index1 = new Index(indexFolder1); // index1 oluşturuluyor
index1.add(documentsFolder1); // Belgeler indeksleniyor
IndexRepository repository = new IndexRepository(); // Dizin deposu oluşturuluyor
Index index2 = repository.create(indexFolder2); // index2 oluşturuluyor
index2.add(documentsFolder2); // Belgeler indeksleniyor
Index index3 = repository.create(indexFolder3); // index3 oluşturuluyor
index3.add(documentsFolder3); // Belgeler indeksleniyor
MergeOptions options = new MergeOptions();
options.setCancellation(new Cancellation()); // İptal nesnesi oluşturuluyor
// Tüm indeksleri indeks deposunda index1'e birleştiriliyor. Not: index2 ve index3 değiştirilmeyecek.
index1.merge(repository, options);
 
```
 
````

|

### highlight(FoundDocument document, Highlighter highlighter) {#highlight-com.groupdocs.search.results.FoundDocument-com.groupdocs.search.highlighters.Highlighter-}
```
public final void highlight(FoundDocument document, Highlighter highlighter)
```


Bulunan terimleri vurgulayan HTML biçimlendirilmiş metin oluşturur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | document | [FoundDocument](../../com.groupdocs.search.results/founddocument) | Bulunan belge. |
|
|  | highlighter | [Highlighter](../../com.groupdocs.search.highlighters/highlighter) | Arama sonucu vurgulayıcı. |

Bu örnek, HTML biçimlendirilmiş metindeki oluşumları nasıl vurgulayacağını gösterir.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentFolder = "c:\\MyDocuments\\";
// Bir indeks oluşturuluyor
Index index = new Index(indexFolder);
// Belirtilen klasörden belgeler indeksleniyor
index.add(documentFolder);
// 'eternity' kelimesini ara
SearchResult result = index.search("eternity");
// Metindeki oluşumları vurgulama
if (result.getDocumentCount() > 0) {
FoundDocument document = result.getFoundDocument(0); // İlk bulunan belge alınıyor
OutputAdapter outputAdapter = new FileOutputAdapter("c:\\Highlighted.html"); // Dosyaya bir çıktı adaptörü oluşturuluyor
Highlighter highlighter = new HtmlHighlighter(outputAdapter); // Vurgulayıcı nesnesi oluşturuluyor
index.highlight(document, highlighter); // Vurgulanan oluşumlarla HTML biçimlendirilmiş metin oluşturuluyor
}
 
```
 
````

|

### highlight(FoundDocument document, Highlighter highlighter, HighlightOptions options) {#highlight-com.groupdocs.search.results.FoundDocument-com.groupdocs.search.highlighters.Highlighter-com.groupdocs.search.options.HighlightOptions-}
```
public final void highlight(FoundDocument document, Highlighter highlighter, HighlightOptions options)
```


Bulunan terimleri vurgulayan HTML biçimlendirilmiş metin oluşturur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | document | [FoundDocument](../../com.groupdocs.search.results/founddocument) | Bulunan belge. |
|
|  | highlighter | [Highlighter](../../com.groupdocs.search.highlighters/highlighter) | Arama sonucu vurgulayıcı. |
|
|  | options | [HighlightOptions](../../com.groupdocs.search.options/highlightoptions) | Vurgulama seçenekleri. |

Bu örnek, HTML biçimlendirilmiş metindeki oluşumları nasıl vurgulayacağını gösterir.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentFolder = "c:\\MyDocuments\\";
// Bir indeks oluşturuluyor
Index index = new Index(indexFolder);
// Belirtilen klasörden belgeler indeksleniyor
index.add(documentFolder);
// 'eternity' kelimesini ara
SearchResult result = index.search("eternity");
// Metindeki oluşumları vurgulama
if (result.getDocumentCount() > 0) {
FoundDocument document = result.getFoundDocument(0); // İlk bulunan belge alınıyor
OutputAdapter outputAdapter = new FileOutputAdapter("c:\\Highlighted.html"); // Dosyaya bir çıktı adaptörü oluşturuluyor
Highlighter highlighter = new HtmlHighlighter(outputAdapter); // Vurgulayıcı nesnesi oluşturuluyor
HighlightOptions options = new HighlightOptions(); // Vurgulama seçenekleri nesnesi oluşturuluyor
options.setTermsBefore(5);
options.setTermsAfter(5);
options.setTermsTotal(15);
index.highlight(document, highlighter, options); // Vurgulanan oluşumlarla HTML biçimlendirilmiş metin oluşturma
}
 
```
 
````

|

### getIndexedDocuments() {#getIndexedDocuments--}
```
public final DocumentInfo[] getIndexedDocuments()
```


Tüm indekslenmiş belgelerin bir dizisini alır.


**Returns:**
com.groupdocs.search.results.DocumentInfo[] - Tüm indekslenmiş belgelerin bir dizisi.

Örnek, bir indeks'ten indekslenmiş belgelerin listesini nasıl alacağını gösterir.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Belirtilen klasörde bir indeks oluşturma
Index index = new Index(indexFolder);
// Belirtilen klasörden belgeler indeksleniyor
index.add(documentsFolder);
// İndekslenmiş belgelerin listesini alıyor
DocumentInfo[] documents = index.getIndexedDocuments();
 
```
 
````


### getIndexedDocumentItems(DocumentInfo documentInfo) {#getIndexedDocumentItems-com.groupdocs.search.results.DocumentInfo-}
```
public final DocumentInfo[] getIndexedDocumentItems(DocumentInfo documentInfo)
```


Belge öğelerinin bir dizisini alır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | documentInfo | [DocumentInfo](../../com.groupdocs.search.results/documentinfo) | Bir belge bilgisi. |

Örnek, bir indeks'ten indekslenmiş bir belgenin öğelerinin listesini nasıl alacağını gösterir.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Belirtilen klasörde bir indeks oluşturma
Index index = new Index(indexFolder);
// Belirtilen klasörden belgeler indeksleniyor
index.add(documentsFolder);
// İndekslenmiş belgelerin listesini alıyor
DocumentInfo[] documents = index.getIndexedDocuments();
for (int i = 0; i < documents.length; i++) {
DocumentInfo document = documents[i];
System.out.println(document.getFilePath());
DocumentInfo[] items = index.getIndexedDocumentItems(document); // Belge öğelerinin listesini alıyor
for (int j = 0; j < items.length; j++) {
DocumentInfo item = items[j];
System.out.println("\t" + item.getInnerPath());
}
}
 
```
 
````

|

**Returns:**
com.groupdocs.search.results.DocumentInfo[] - Bir belge öğesinin dizisi.

### GetIndexedDocument(String documentKey) {#GetIndexedDocument-java.lang.String-}
```
public DocumentInfo GetIndexedDocument(String documentKey)
```


Belge anahtarına göre indekslenmiş bir belge alır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | documentKey | java.lang.String | Belgenin anahtarı. |
|

**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - The indexed document.

### getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter) {#getDocumentText-com.groupdocs.search.results.DocumentInfo-com.groupdocs.search.common.OutputAdapter-}
```
public final void getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter)
```


İndekslenmiş bir belgenin metnini oluşturur ve bir çıktı adaptörü aracılığıyla iletir.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | documentInfo | [DocumentInfo](../../com.groupdocs.search.results/documentinfo) | İndekslenmiş belge bilgisi. |
|
|  | adapter | [OutputAdapter](../../com.groupdocs.search.common/outputadapter) | Çıktı adaptörü. |

Örnek, bir indeks'ten indekslenmiş bir belgenin metnini nasıl alacağını gösterir.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Belirtilen klasörde bir indeks oluşturma
Index index = new Index(indexFolder);
// Belirtilen klasörden belgeler indeksleniyor
index.add(documentsFolder);
// İndekslenmiş belgelerin listesini alıyor
DocumentInfo[] documents = index.getIndexedDocuments();
// Bir belge metni alınıyor
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


İndekslenmiş belge için HTML biçimlendirilmiş metin oluşturur ve çıktı adaptörü aracılığıyla aktarır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | documentInfo | [DocumentInfo](../../com.groupdocs.search.results/documentinfo) | İndekslenmiş belge bilgisi. |
|
|  | adapter | [OutputAdapter](../../com.groupdocs.search.common/outputadapter) | Çıktı adaptörü. |
|
|  | options | [TextOptions](../../com.groupdocs.search.options/textoptions) | Metin alma seçenekleri. |
|

### getIndexedPaths() {#getIndexedPaths--}
```
public final String[] getIndexedPaths()
```


İndekslenmiş yolların - belgelerin veya klasörlerin - bir dizisini alır.


**Returns:**
java.lang.String[] - İndekslenmiş yolların bir dizisi.

### delete(String[] paths, UpdateOptions options) {#delete-java.lang.String---com.groupdocs.search.options.UpdateOptions-}
```
public final DeleteResult delete(String[] paths, UpdateOptions options)
```


İndeksten indekslenmiş dosya veya klasörleri siler. Ardından silinen yollar olmadan indeksi günceller.
Bir belge, klasörün bir parçası olarak indekse eklenmişse, indeksten silinemeyeceğini unutmayın.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | yollar | java.lang.String[] | Silinecek dosya veya klasörlerin yolları. |
|
|  | options | [UpdateOptions](../../com.groupdocs.search.options/updateoptions) | Güncelleme seçenekleri. |

Bu örnek, bir indeksten indekslenmiş yolların nasıl silineceğini gösterir.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder1 = "c:\\MyDocuments\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
// Belirtilen klasörde bir indeks oluşturma
Index index = new Index(indexFolder);
// Belirtilen klasörlerden belgeleri indeksleme
index.add(documentsFolder1);
index.add(documentsFolder2);
// İndeksten indekslenmiş yolları alıyor
String[] indexedPaths1 = index.getIndexedPaths();
// İndekslenmiş yolları konsola yazdırma
System.out.println("İndekslenmiş yollar:");
for (String path : indexedPaths1) {
System.out.println("\t" + path);
}
// İndeksten indeks yolu silme
DeleteResult deleteResult = index.delete(new String[] { documentsFolder1 }, new UpdateOptions());
// Silme işleminden sonra indekslenmiş yolları alma
String[] indexedPaths2 = index.getIndexedPaths();
System.out.println("\nSilinen yollar: " + deleteResult.getSuccessCount());
System.out.println("\nİndekslenmiş yollar:");
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


Akışlardan veya yapılardan indekslenen belgeleri siler. Ardından silinen belgeler olmadan indeksi günceller.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | options | [UpdateOptions](../../com.groupdocs.search.options/updateoptions) | Güncelleme seçenekleri. |
|
|  | documentKeys | java.lang.String[] | Akışlardan veya yapılardan eklenen belgelerin anahtarları. |
|

**Returns:**
[DeleteResult](../../com.groupdocs.search.results/deleteresult) - An object describing the result of deleting documents from the index.

### notifyIndex(Notification notification) {#notifyIndex-com.groupdocs.search.Notification-}
```
public final boolean notifyIndex(Notification notification)
```


Belirtilen bildirim nesnesini bildirimi gerçekleştirmek için indekse iletir.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | notification | [Notification](../../com.groupdocs.search/notification) | Bildirim nesnesi. |
|

**Returns:**
boolean - Bildirimin başarıyla gerçekleştirildiği durumda  true  döner; aksi takdirinde  false .

### changeAttributes(AttributeChangeBatch batch) {#changeAttributes-com.groupdocs.search.common.AttributeChangeBatch-}
```
public final void changeAttributes(AttributeChangeBatch batch)
```


Güncelleme işlemi sırasında yeniden indeksleme yapmadan, belirtilen öznitelik değişiklikleri topluluğunu indekslenmiş belgelere uygular.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | batch | [AttributeChangeBatch](../../com.groupdocs.search.common/attributechangebatch) | Özellik değişim paketi. |
|

### getAttributes(String path) {#getAttributes-java.lang.String-}
```
public final String[] getAttributes(String path)
```


Belirtilen indekslenmiş belgeyle ilişkili tüm öznitelikleri alır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | path | java.lang.String | Belge yolu. |
|

**Returns:**
java.lang.String[] - Belgeyle ilişkili öznitelikler.

### loadIntoMemoryCompletely(String indexFolder) {#loadIntoMemoryCompletely-java.lang.String-}
```
public static Index loadIntoMemoryCompletely(String indexFolder)
```


Tam indeksi belleğe yükler.
Dizindeki herhangi bir değişiklik otomatik olarak orijinal klasöre kaydedilmez.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | indexFolder | java.lang.String | İndeks klasör yolu. |
|

**Returns:**
[Index](../../com.groupdocs.search/index) - The loaded in-memory index.

### loadIntoMemoryCompletely(String indexFolder, IndexSettings settings) {#loadIntoMemoryCompletely-java.lang.String-com.groupdocs.search.IndexSettings-}
```
public static Index loadIntoMemoryCompletely(String indexFolder, IndexSettings settings)
```


Tam indeksi belleğe yükler.
Dizindeki herhangi bir değişiklik otomatik olarak orijinal klasöre kaydedilmez.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | indexFolder | java.lang.String | İndeks klasör yolu. |
|
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | İndeks ayarları nesnesi. |
|

**Returns:**
[Index](../../com.groupdocs.search/index) - The loaded in-memory index.

