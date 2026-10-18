---
title: "IndexSettings"
second_title: "GroupDocs.Search for Java API Referansı"
description: "İndeksleme işlemlerini özelleştirmeye izin veren indeks ayarlarını temsil eder."
type: docs
weight: 19
url: /tr/java/com.groupdocs.search/indexsettings/
---
**Inheritance:**
java.lang.Object
```
public class IndexSettings
```

İndeksleme işlemlerini özelleştirmeye izin veren indeks ayarlarını temsil eder.


**Learn more**

* [Search index settings](../https://docs.groupdocs.com/display/searchjava/Search+index+settings)


Örnek, sınıfın tipik bir kullanımını gösterir.

````
 ```

String indexFolder = "c:\\MyIndex\\";
IndexSettings settings = new IndexSettings();
settings.setIndexType(IndexType.CompactIndex); // Dizin türünü ayarlama
Index index = new Index(indexFolder, settings); // Bir dizin oluşturma
 
```
 
````


## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [IndexSettings()](#IndexSettings--) | IndexSettings sınıfının yeni bir örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getInMemoryIndex()](#getInMemoryIndex--) | Dizinin bellek içinde mi yoksa diskte mi saklandığını gösteren bir değeri alır. |
|
|  | [getUseStopWords()](#getUseStopWords--) | Durak kelimelerin kullanılıp kullanılmayacağını gösteren bir değeri alır. |
|
|  | [setUseStopWords(boolean value)](#setUseStopWords-boolean-) | Durak kelimelerin kullanılıp kullanılmayacağını gösteren bir değeri ayarlar. |
|
|  | [getMaxIndexingReportCount()](#getMaxIndexingReportCount--) | Azami indeksleme raporu sayısını alır. |
|
|  | [setMaxIndexingReportCount(int value)](#setMaxIndexingReportCount-int-) | Azami indeksleme raporu sayısını ayarlar. |
|
|  | [getMaxSearchReportCount()](#getMaxSearchReportCount--) | Azami arama raporu sayısını alır. |
|
|  | [setMaxSearchReportCount(int value)](#setMaxSearchReportCount-int-) | Azami arama raporu sayısını ayarlar. |
|
|  | [getUseCharacterReplacements()](#getUseCharacterReplacements--) | Karakter değişimlerinin kullanılıp kullanılmayacağını gösteren bir değeri alır. |
|
|  | [setUseCharacterReplacements(boolean value)](#setUseCharacterReplacements-boolean-) | Karakter değişimlerinin kullanılıp kullanılmayacağını gösteren bir değeri ayarlar. |
|
|  | [getDocumentFilter()](#getDocumentFilter--) | Bir belge filtresini alır. |
|
|  | [setDocumentFilter(DocumentFilter value)](#setDocumentFilter-com.groupdocs.search.DocumentFilter-) | Bir belge filtresini ayarlar. |
|
|  | [getTextStorageSettings()](#getTextStorageSettings--) | Metin depolama ayarlarını alır. |
|
|  | [setTextStorageSettings(TextStorageSettings value)](#setTextStorageSettings-com.groupdocs.search.options.TextStorageSettings-) | Metin depolama ayarlarını ayarlar. |
|
|  | [getIndexType()](#getIndexType--) | Dizin türünü alır. |
|
|  | [setIndexType(IndexType value)](#setIndexType-com.groupdocs.search.options.IndexType-) | Dizin türünü ayarlar. |
|
|  | [getSearchThreads()](#getSearchThreads--) | Arama için kullanılan iş parçacığı sayısını alır. |
|
|  | [setSearchThreads(NumberOfThreads value)](#setSearchThreads-com.groupdocs.search.options.NumberOfThreads-) | Arama için kullanılan iş parçacığı sayısını ayarlar. |
|
|  | [getCustomExtractors()](#getCustomExtractors--) | Özel çıkarıcı koleksiyonunu alır. |
|
|  | [getLogger()](#getLogger--) | Dizindeki olayları ve hataları kaydetmek için kullanılan bir günlükçüyü alır. |
|
|  | [setLogger(ILogger value)](#setLogger-com.groupdocs.search.common.ILogger-) | Dizindeki olayları ve hataları kaydetmek için kullanılan bir günlükçüyü ayarlar. |
|
### IndexSettings() {#IndexSettings--}
```
public IndexSettings()
```


IndexSettings sınıfının yeni bir örneğini başlatır.


### getInMemoryIndex() {#getInMemoryIndex--}
```
public final boolean getInMemoryIndex()
```


Dizinin bellek içinde mi yoksa diskte mi saklandığını gösteren bir değeri alır.


**Returns:**
boolean - Dizinin bellek içinde mi yoksa diskte mi saklandığını gösteren bir değer.

### getUseStopWords() {#getUseStopWords--}
```
public final boolean getUseStopWords()
```


Durak kelimelerin kullanılıp kullanılmayacağını gösteren bir değeri alır. Varsayılan değer true.


**Returns:**
boolean - Durdurma kelimelerinin kullanılıp kullanılmayacağını belirten bir değer.

### setUseStopWords(boolean value) {#setUseStopWords-boolean-}
```
public final void setUseStopWords(boolean value)
```


Durdurma kelimelerinin kullanılıp kullanılmayacağını belirten bir değer ayarlar. Varsayılan değer  true  dir.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | boolean | Durdurma kelimelerinin kullanılıp kullanılmayacağını belirten bir değer. |
|

### getMaxIndexingReportCount() {#getMaxIndexingReportCount--}
```
public final int getMaxIndexingReportCount()
```


Dizin raporlarının azami sayısını alır. Varsayılan değer  5  dir.


**Returns:**
int - Dizin raporlarının azami sayısı.

### setMaxIndexingReportCount(int value) {#setMaxIndexingReportCount-int-}
```
public final void setMaxIndexingReportCount(int value)
```


Dizin raporlarının azami sayısını ayarlar. Varsayılan değer  5  dir.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | int | Dizin raporlarının azami sayısı. |
|

### getMaxSearchReportCount() {#getMaxSearchReportCount--}
```
public final int getMaxSearchReportCount()
```


Arama raporlarının azami sayısını alır. Varsayılan değer  10  dir.


**Returns:**
int - Arama raporlarının azami sayısı.

### setMaxSearchReportCount(int value) {#setMaxSearchReportCount-int-}
```
public final void setMaxSearchReportCount(int value)
```


Arama raporlarının azami sayısını ayarlar. Varsayılan değer  10  dir.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | int | Arama raporlarının azami sayısı. |
|

### getUseCharacterReplacements() {#getUseCharacterReplacements--}
```
public final boolean getUseCharacterReplacements()
```


Karakter değiştirmelerinin kullanılıp kullanılmayacağını belirten bir değeri alır. Varsayılan değer  false  dir.


**Returns:**
boolean - Karakter değiştirmelerinin kullanılıp kullanılmayacağını belirten bir değer.

### setUseCharacterReplacements(boolean value) {#setUseCharacterReplacements-boolean-}
```
public final void setUseCharacterReplacements(boolean value)
```


Karakter değiştirmelerinin kullanılıp kullanılmayacağını belirten bir değeri ayarlar. Varsayılan değer  false  dir.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | boolean | Karakter değiştirmelerinin kullanılıp kullanılmayacağını belirten bir değer. |
|

### getDocumentFilter() {#getDocumentFilter--}
```
public final DocumentFilter getDocumentFilter()
```


Bir belge filtresi alır. DocumentFilter dahil etme mantığıyla çalışır. Bir belge filtresi örneği oluşturmak için DocumentFilter sınıfını kullanın. Varsayılan değer  null  dır, bu da tüm eklenen belgelerin indekslendiği anlamına gelir.


**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - The document filter.

Örnek, belge filtresinin nasıl ayarlanacağını gösterir.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// '.doc', '.docx', '.rtf' uzantılı belgeleri atlayan bir filtre oluşturma
IndexSettings settings = new IndexSettings();
DocumentFilter fileExtensionFilter = DocumentFilter.createFileExtension(".doc", ".docx", ".rtf"); // Dosya uzantısı filtresi oluşturma
DocumentFilter invertedFilter = DocumentFilter.createNot(fileExtensionFilter); // Dosya uzantısı filtresini tersine çevirme
settings.setDocumentFilter(invertedFilter);
// Belirtilen klasörde bir indeks oluşturma
Index index = new Index(indexFolder, settings);
// Belgeleri indeksleme
index.add(documentsFolder);
// Arama
SearchResult result = index.search("Einstein");
 
```
 
````


### setDocumentFilter(DocumentFilter value) {#setDocumentFilter-com.groupdocs.search.DocumentFilter-}
```
public final void setDocumentFilter(DocumentFilter value)
```


Bir belge filtresi ayarlar. DocumentFilter dahil etme mantığı üzerinde çalışır. Belge filtresi örnekleri oluşturmak için GroupDocs.Search.Options.DocumentFilter sınıfını kullanın. Varsayılan değer null'dur, bu da eklenen tüm belgelerin indekslendiği anlamına gelir.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | value | [DocumentFilter](../../com.groupdocs.search/documentfilter) | Belge filtresi. |

Örnek, belge filtresinin nasıl ayarlanacağını gösterir.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// '.doc', '.docx', '.rtf' uzantılı belgeleri atlayan bir filtre oluşturma
IndexSettings settings = new IndexSettings();
DocumentFilter fileExtensionFilter = DocumentFilter.createFileExtension(".doc", ".docx", ".rtf"); // Dosya uzantısı filtresi oluşturma
DocumentFilter invertedFilter = DocumentFilter.createNot(fileExtensionFilter); // Dosya uzantısı filtresini tersine çevirme
settings.setDocumentFilter(invertedFilter);
// Belirtilen klasörde bir indeks oluşturma
Index index = new Index(indexFolder, settings);
// Belgeleri indeksleme
index.add(documentsFolder);
// Arama
SearchResult result = index.search("Einstein");
 
```
 
````

|

### getTextStorageSettings() {#getTextStorageSettings--}
```
public final TextStorageSettings getTextStorageSettings()
```


Metin depolama ayarlarını alır. Varsayılan değer null'dur, bu da belge metinlerinin depolanmadığı anlamına gelir.


**Returns:**
[TextStorageSettings](../../com.groupdocs.search.options/textstoragesettings) - The text storage settings.

Örnek, metin depolama ayarlarının nasıl ayarlanacağını gösterir.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// İndeks ayarları örneği oluşturma
IndexSettings settings = new IndexSettings();
settings.setTextStorageSettings(new TextStorageSettings(Compression.High)); // İndeks metin depolaması için yüksek sıkıştırma seviyesini ayarlama
// Belirtilen klasörde bir indeks oluşturma
Index index = new Index(indexFolder, settings);
// Belgeleri indeksleme
index.add(documentsFolder);
// Arama
SearchResult result = index.search("Einstein");
 
```
 
````


### setTextStorageSettings(TextStorageSettings value) {#setTextStorageSettings-com.groupdocs.search.options.TextStorageSettings-}
```
public final void setTextStorageSettings(TextStorageSettings value)
```


Metin depolama ayarlarını ayarlar. Varsayılan değer null'dur, bu da belge metinlerinin depolanmadığı anlamına gelir.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | value | [TextStorageSettings](../../com.groupdocs.search.options/textstoragesettings) | Metin depolama ayarları. |

Örnek, metin depolama ayarlarının nasıl ayarlanacağını gösterir.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// İndeks ayarları örneği oluşturma
IndexSettings settings = new IndexSettings();
settings.setTextStorageSettings(new TextStorageSettings(Compression.High)); // İndeks metin depolaması için yüksek sıkıştırma seviyesini ayarlama
// Belirtilen klasörde bir indeks oluşturma
Index index = new Index(indexFolder, settings);
// Belgeleri indeksleme
index.add(documentsFolder);
// Arama
SearchResult result = index.search("Einstein");
 
```
 
````

|

### getIndexType() {#getIndexType--}
```
public final IndexType getIndexType()
```


İndeks tipini alır. Varsayılan değer GroupDocs.Search.Options.IndexType.NormalIndex'dir.


**Returns:**
[IndexType](../../com.groupdocs.search.options/indextype) - The index type.

### setIndexType(IndexType value) {#setIndexType-com.groupdocs.search.options.IndexType-}
```
public final void setIndexType(IndexType value)
```


İndeks tipini ayarlar. Varsayılan değer GroupDocs.Search.Options.IndexType.NormalIndex'dir.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | value | [IndexType](../../com.groupdocs.search.options/indextype) | İndeks tipi. |
|

### getSearchThreads() {#getSearchThreads--}
```
public final NumberOfThreads getSearchThreads()
```


Arama için kullanılan iş parçacığı sayısını alır. Varsayılan değer GroupDocs.Search.Options.NumberOfThreads.Default'tir, bu da aramanın işlemci çekirdek sayısına eşit sayıda iş parçacığı kullanılarak gerçekleştirileceği anlamına gelir.


**Returns:**
[NumberOfThreads](../../com.groupdocs.search.options/numberofthreads) - The number of threads used for the search.

### setSearchThreads(NumberOfThreads value) {#setSearchThreads-com.groupdocs.search.options.NumberOfThreads-}
```
public final void setSearchThreads(NumberOfThreads value)
```


Arama için kullanılan iş parçacığı sayısını ayarlar. Varsayılan değer GroupDocs.Search.Options.NumberOfThreads.Default'tir, bu da aramanın işlemci çekirdek sayısına eşit sayıda iş parçacığı kullanılarak gerçekleştirileceği anlamına gelir.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | value | [NumberOfThreads](../../com.groupdocs.search.options/numberofthreads) | Arama için kullanılan iş parçacığı sayısı. |
|

### getCustomExtractors() {#getCustomExtractors--}
```
public final CustomExtractorCollection getCustomExtractors()
```


Özel çıkarıcı koleksiyonunu alır. Özel bir çıkarıcı uygulamanın tam örneği, GroupDocs.Search.Common.IFieldExtractor arayüzü için belgelerde sunulmuştur.


**Returns:**
[CustomExtractorCollection](../../com.groupdocs.search.common/customextractorcollection) - The custom extractor collection.

### getLogger() {#getLogger--}
```
public final ILogger getLogger()
```


İndeks içinde olayları ve hataları kaydetmek için kullanılan bir günlükçüyü alır. Günlükçünün kaydedilmediğini ve indeks her oluşturulduğunda veya yüklendiğinde yeniden oluşturulup atanması gerektiğini unutmayın.


**Returns:**
[ILogger](../../com.groupdocs.search.common/ilogger) - A logger that is used for logging events and errors in the index.

### setLogger(ILogger value) {#setLogger-com.groupdocs.search.common.ILogger-}
```
public final void setLogger(ILogger value)
```


İndeks içinde olayları ve hataları kaydetmek için kullanılan bir günlükçüyü ayarlar. Günlükçünün kaydedilmediğini ve indeks her oluşturulduğunda veya yüklendiğinde yeniden oluşturulup atanması gerektiğini unutmayın.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | value | [ILogger](../../com.groupdocs.search.common/ilogger) | İndeks içinde olayları ve hataları kaydetmek için kullanılan bir günlükçü. |
|

