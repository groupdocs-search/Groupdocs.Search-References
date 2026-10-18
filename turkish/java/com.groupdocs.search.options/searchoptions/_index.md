---
title: "SearchOptions"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Arama işlemi için seçenekler sağlar."
type: docs
weight: 34
url: /tr/java/com.groupdocs.search.options/searchoptions/
---
**Inheritance:**
java.lang.Object
```
public class SearchOptions
```

Arama işlemi için seçenekler sağlar.


**Learn more**

* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [SearchOptions()](#SearchOptions--) | SearchOptions sınıfının yeni bir örneğini başlatır. |
|
|  | [SearchOptions(Object data)](#SearchOptions-java.lang.Object-) | SearchOptions sınıfının yeni bir örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getUseSynonymSearch()](#getUseSynonymSearch--) | Aramada eşanlamlıların kullanım bayrağını alır. |
|
|  | [setUseSynonymSearch(boolean value)](#setUseSynonymSearch-boolean-) | Aramada eşanlamlıların kullanım bayrağını ayarlar. |
|
|  | [getUseHomophoneSearch()](#getUseHomophoneSearch--) | Aramada aynı sesli kelimelerin kullanım bayrağını alır. |
|
|  | [setUseHomophoneSearch(boolean value)](#setUseHomophoneSearch-boolean-) | Aramada aynı sesli kelimelerin kullanım bayrağını ayarlar. |
|
|  | [getUseWordFormsSearch()](#getUseWordFormsSearch--) | Aramada farklı kelime biçimlerinin kullanım bayrağını alır. |
|
|  | [setUseWordFormsSearch(boolean value)](#setUseWordFormsSearch-boolean-) | Aramada farklı kelime biçimlerinin kullanım bayrağını ayarlar. |
|
|  | [getRetrieveAttributes()](#getRetrieveAttributes--) | Bulunan belgelerle ilişkili özniteliklerin alınması bayrağını alır. |
|
|  | [setRetrieveAttributes(boolean value)](#setRetrieveAttributes-boolean-) | Bulunan belgelerle ilişkili özniteliklerin alınması bayrağını ayarlar. |
|
|  | [getFuzzySearch()](#getFuzzySearch--) | Bulanık arama seçeneklerini alır. |
|
|  | [getSpellingCorrector()](#getSpellingCorrector--) | Yazım düzeltici seçeneklerini alır. |
|
|  | [getKeyboardLayoutCorrector()](#getKeyboardLayoutCorrector--) | Klavye düzeni düzeltici seçeneklerini alır. |
|
|  | [getUseCaseSensitiveSearch()](#getUseCaseSensitiveSearch--) | Büyük/küçük harfe duyarlı arama bayrağını alır. |
|
|  | [setUseCaseSensitiveSearch(boolean value)](#setUseCaseSensitiveSearch-boolean-) | Büyük/küçük harfe duyarlı arama bayrağını ayarlar. |
|
|  | [getMaxTotalOccurrenceCount()](#getMaxTotalOccurrenceCount--) | Bir arama sorgusundaki tüm terimlerin maksimum toplam tekrar sayısını alır. |
|
|  | [setMaxTotalOccurrenceCount(int value)](#setMaxTotalOccurrenceCount-int-) | Arama sorgusundaki tüm terimlerin toplam en fazla oluş sayısını ayarlar. |
|
|  | [getMaxOccurrenceCountPerTerm()](#getMaxOccurrenceCountPerTerm--) | Arama sorgusundaki her terimin en fazla oluş sayısını alır. |
|
|  | [setMaxOccurrenceCountPerTerm(int value)](#setMaxOccurrenceCountPerTerm-int-) | Arama sorgusundaki her terimin en fazla oluş sayısını ayarlar. |
|
|  | [getDateFormats()](#getDateFormats--) | Tarih aralığı araması için tarih biçimleri koleksiyonunu alır. |
|
|  | [isChunkSearch()](#isChunkSearch--) | Parçalarla arama bayrağını alır. |
|
|  | [setChunkSearch(boolean value)](#setChunkSearch-boolean-) | Parçalarla arama bayrağını ayarlar. |
|
|  | [getSearchDocumentFilter()](#getSearchDocumentFilter--) | Arama belge filtresini alır. |
|
|  | [setSearchDocumentFilter(ISearchDocumentFilter value)](#setSearchDocumentFilter-com.groupdocs.search.options.ISearchDocumentFilter-) | Arama belge filtresini ayarlar. |
|
|  | [getCancellation()](#getCancellation--) | İşlem iptal nesnesini alır. |
|
|  | [setCancellation(Cancellation value)](#setCancellation-com.groupdocs.search.common.Cancellation-) | İşlem iptal nesnesini ayarlar. |
|
| [getCore()](#getCore--) |  |
### SearchOptions() {#SearchOptions--}
```
public SearchOptions()
```


SearchOptions sınıfının yeni bir örneğini başlatır.


### SearchOptions(Object data) {#SearchOptions-java.lang.Object-}
```
public SearchOptions(Object data)
```


SearchOptions sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | veri | java.lang.Object | Serileştirilmiş veri. |
|

### getUseSynonymSearch() {#getUseSynonymSearch--}
```
public boolean getUseSynonymSearch()
```


Aramada eşanlamlıların kullanım bayrağını alır. Varsayılan değer false.


**Returns:**
boolean - Aramada eşanlamlıların kullanım bayrağı.

### setUseSynonymSearch(boolean value) {#setUseSynonymSearch-boolean-}
```
public void setUseSynonymSearch(boolean value)
```


Aramada eşanlamlıların kullanım bayrağını ayarlar. Varsayılan değer false.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | boolean | Aramada eşanlamlıların kullanım bayrağı. |
|

### getUseHomophoneSearch() {#getUseHomophoneSearch--}
```
public boolean getUseHomophoneSearch()
```


Aramada homofonların kullanım bayrağını alır. Varsayılan değer false.


**Returns:**
boolean - Aramada homofonların kullanım bayrağı.

### setUseHomophoneSearch(boolean value) {#setUseHomophoneSearch-boolean-}
```
public void setUseHomophoneSearch(boolean value)
```


Aramada homofonların kullanım bayrağını ayarlar. Varsayılan değer false.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | boolean | Aramada homofonların kullanım bayrağı. |
|

### getUseWordFormsSearch() {#getUseWordFormsSearch--}
```
public boolean getUseWordFormsSearch()
```


Aramada farklı kelime biçimlerinin kullanım bayrağını alır. Varsayılan değer false.


**Returns:**
boolean - Aramada farklı kelime biçimlerinin kullanım bayrağı.

### setUseWordFormsSearch(boolean value) {#setUseWordFormsSearch-boolean-}
```
public void setUseWordFormsSearch(boolean value)
```


Aramada farklı kelime biçimlerinin kullanım bayrağını ayarlar. Varsayılan değer false.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | boolean | Aramada farklı kelime biçimlerinin kullanım bayrağı. |
|

### getRetrieveAttributes() {#getRetrieveAttributes--}
```
public boolean getRetrieveAttributes()
```


Bulunan belgelerle ilişkili özniteliklerin alınması bayrağını alır. Varsayılan değer false.


**Returns:**
boolean - Bulunan belgelerle ilişkili özniteliklerin alınması bayrağı.

### setRetrieveAttributes(boolean value) {#setRetrieveAttributes-boolean-}
```
public void setRetrieveAttributes(boolean value)
```


Bulunan belgelerle ilişkili özniteliklerin alınması bayrağını ayarlar. Varsayılan değer false.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | boolean | Bulunan belgelerle ilişkili özniteliklerin alınması bayrağı. |
|

### getFuzzySearch() {#getFuzzySearch--}
```
public FuzzySearchOptions getFuzzySearch()
```


Bulanık arama seçeneklerini alır.


**Returns:**
[FuzzySearchOptions](../../com.groupdocs.search.options/fuzzysearchoptions) - The fuzzy search options.

### getSpellingCorrector() {#getSpellingCorrector--}
```
public SpellingCorrectorOptions getSpellingCorrector()
```


Yazım düzeltici seçeneklerini alır.


**Returns:**
[SpellingCorrectorOptions](../../com.groupdocs.search.options/spellingcorrectoroptions) - The spelling corrector options.

### getKeyboardLayoutCorrector() {#getKeyboardLayoutCorrector--}
```
public KeyboardLayoutCorrectorOptions getKeyboardLayoutCorrector()
```


Klavye düzeni düzeltici seçeneklerini alır.


**Returns:**
[KeyboardLayoutCorrectorOptions](../../com.groupdocs.search.options/keyboardlayoutcorrectoroptions) - The keyboard layout corrector options.

### getUseCaseSensitiveSearch() {#getUseCaseSensitiveSearch--}
```
public boolean getUseCaseSensitiveSearch()
```


Büyük/küçük harfe duyarlı arama bayrağını alır. Varsayılan değer false.


**Returns:**
boolean - Büyük/küçük harfe duyarlı arama bayrağı.

### setUseCaseSensitiveSearch(boolean value) {#setUseCaseSensitiveSearch-boolean-}
```
public void setUseCaseSensitiveSearch(boolean value)
```


Büyük/küçük harfe duyarlı arama bayrağını ayarlar. Varsayılan değer false.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | boolean | Büyük/küçük harfe duyarlı arama bayrağı. |
|

### getMaxTotalOccurrenceCount() {#getMaxTotalOccurrenceCount--}
```
public int getMaxTotalOccurrenceCount()
```


Bir arama sorgusundaki tüm terimlerin maksimum toplam oluşum sayısını alır. Varsayılan değer 500000.


**Returns:**
int - Maksimum toplam oluşum sayısı.

### setMaxTotalOccurrenceCount(int value) {#setMaxTotalOccurrenceCount-int-}
```
public void setMaxTotalOccurrenceCount(int value)
```


Bir arama sorgusundaki tüm terimlerin maksimum toplam oluşum sayısını ayarlar. Varsayılan değer 500000.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | int | Maksimum toplam oluşum sayısı. |
|

### getMaxOccurrenceCountPerTerm() {#getMaxOccurrenceCountPerTerm--}
```
public int getMaxOccurrenceCountPerTerm()
```


Bir arama sorgusundaki her terimin maksimum oluşum sayısını alır. Varsayılan değer 100000.


**Returns:**
int - Bir arama sorgusundaki her terimin maksimum oluşum sayısı.

### setMaxOccurrenceCountPerTerm(int value) {#setMaxOccurrenceCountPerTerm-int-}
```
public void setMaxOccurrenceCountPerTerm(int value)
```


Bir arama sorgusundaki her terimin maksimum oluşum sayısını ayarlar. Varsayılan değer 100000.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | int | Bir arama sorgusundaki her terimin maksimum oluşum sayısı. |
|

### getDateFormats() {#getDateFormats--}
```
public DateFormatCollection getDateFormats()
```


Tarih aralığı araması için tarih formatları koleksiyonunu alır. Varsayılan tarih formatları 'dd.MM.yyyy', 'MM/dd/yyyy' ve 'yyyy-MM-dd' dir.


**Returns:**
[DateFormatCollection](../../com.groupdocs.search.options/dateformatcollection) - The collection of date formats for date range search.


Örnek, arama için tarih formatlarını nasıl ayarlayacağınızı gösterir.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Belirtilen klasörde bir indeks oluşturuluyor
index.add(documentsFolder); // Belirtilen klasörden belgeleri indeksleme
SearchOptions options = new SearchOptions();
options.getDateFormats().clear(); // Varsayılan tarih formatlarını kaldırma
DateFormatElement[] elements = new DateFormatElement[] {
DateFormatElement.getMonthTwoDigits(),
DateFormatElement.getDayOfMonthTwoDigits(),
DateFormatElement.getYearFourDigits(),
};
// 'MM/dd/yyyy' tarih formatı deseni oluşturma
com.groupdocs.search.DateFormat dateFormat = new com.groupdocs.search.DateFormat(elements, "/");
options.getDateFormats().addItem(dateFormat);
SearchResult result = index.search(query, options); // İndekste arama
 
```
 
````


### isChunkSearch() {#isChunkSearch--}
```
public boolean isChunkSearch()
```


Parçalarla arama bayrağını alır. Varsayılan değer false.


**Returns:**
boolean - Parçalarla arama bayrağı.

### setChunkSearch(boolean value) {#setChunkSearch-boolean-}
```
public void setChunkSearch(boolean value)
```


Parçalarla arama bayrağını ayarlar. Varsayılan değer false.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | boolean | Parçalarla arama bayrağı. |
|

### getSearchDocumentFilter() {#getSearchDocumentFilter--}
```
public ISearchDocumentFilter getSearchDocumentFilter()
```


Arama belge filtresini alır. SearchDocumentFilter dahil etme mantığıyla çalışır. Arama belge filtresi örnekleri oluşturmak için SearchDocumentFilter sınıfını kullanın. Varsayılan değer null'dır, bu da bulunan tüm belgelerin döndürüleceği anlamına gelir.


**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - The search document filter.


Örnek, belge filtresinin nasıl ayarlanacağını gösterir.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments1\\";
// Belirtilen klasörde bir indeks oluşturma
Index index = new Index(indexFolder);
// Belgeleri indeksleme
index.add(documentsFolder);
// '.doc', '.docx', '.rtf' uzantılı belgeleri atlayan bir arama belge filtresi oluşturma
SearchOptions options = new SearchOptions();
ISearchDocumentFilter fileExtensionFilter = SearchDocumentFilter.createFileExtension(".doc", ".docx", ".rtf"); // Dosya uzantısı filtresi oluşturma
ISearchDocumentFilter invertedFilter = SearchDocumentFilter.createNot(fileExtensionFilter); // Dosya uzantısı filtresini tersine çevirme
options.setSearchDocumentFilter(invertedFilter);
// Dizin içinde ara
SearchResult result = index.search("Einstein", options);
 
```
 
````


### setSearchDocumentFilter(ISearchDocumentFilter value) {#setSearchDocumentFilter-com.groupdocs.search.options.ISearchDocumentFilter-}
```
public void setSearchDocumentFilter(ISearchDocumentFilter value)
```


Arama belge filtresini ayarlar. SearchDocumentFilter dahil etme mantığıyla çalışır. Arama belge filtresi örnekleri oluşturmak için SearchDocumentFilter sınıfını kullanın. Varsayılan değer null'dır, bu da bulunan tüm belgelerin döndürüleceği anlamına gelir.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | value | [ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) | Arama belge filtresi. |


Örnek, belge filtresinin nasıl ayarlanacağını gösterir.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments1\\";
// Belirtilen klasörde bir indeks oluşturma
Index index = new Index(indexFolder);
// Belgeleri indeksleme
index.add(documentsFolder);
// '.doc', '.docx', '.rtf' uzantılı belgeleri atlayan bir arama belge filtresi oluşturma
SearchOptions options = new SearchOptions();
ISearchDocumentFilter fileExtensionFilter = SearchDocumentFilter.createFileExtension(".doc", ".docx", ".rtf"); // Dosya uzantısı filtresi oluşturma
ISearchDocumentFilter invertedFilter = SearchDocumentFilter.createNot(fileExtensionFilter); // Dosya uzantısı filtresini tersine çevirme
options.setSearchDocumentFilter(invertedFilter);
// Dizin içinde ara
SearchResult result = index.search("Einstein", options);
 
```
 
````

|

### getCancellation() {#getCancellation--}
```
public Cancellation getCancellation()
```


İşlem iptal nesnesini alır. Varsayılan değer  null .


**Returns:**
[Cancellation](../../com.groupdocs.search.common/cancellation) - The operation cancellation object.

### setCancellation(Cancellation value) {#setCancellation-com.groupdocs.search.common.Cancellation-}
```
public void setCancellation(Cancellation value)
```


İşlem iptal nesnesini ayarlar. Varsayılan değer  null .


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | value | [Cancellation](../../com.groupdocs.search.common/cancellation) | İşlem iptal nesnesi. |
|

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
