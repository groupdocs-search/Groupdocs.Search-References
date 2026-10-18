---
title: "SearchQuery"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Nesne biçiminde bir arama sorgusunu temsil eder."
type: docs
weight: 25
url: /tr/java/com.groupdocs.search/searchquery/
---
**Inheritance:**
java.lang.Object
```
public abstract class SearchQuery
```

Nesne biçiminde bir arama sorgusunu temsil eder.


**Learn more**

* [Searching](../https://docs.groupdocs.com/display/searchjava/Searching)
* [Queries in text and object form](../https://docs.groupdocs.com/display/searchjava/Queries+in+text+and+object+form)
* [Nesting search queries in object form](../https://docs.groupdocs.com/display/searchjava/Nesting+search+queries+in+object+form)


Örnek, sınıfın tipik bir kullanımını gösterir.

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


## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getFieldName()](#getFieldName--) | Alan adını alır. |
|
|  | [getChildCount()](#getChildCount--) | Alt sorgu sayısını alır. |
|
|  | [getFirstChild()](#getFirstChild--) | İlk alt sorguyu alır. |
|
|  | [getSecondChild()](#getSecondChild--) | İkinci alt sorguyu alır. |
|
|  | [getChild(int index)](#getChild-int-) | Bir indeksle bir alt sorgu alır. |
|
|  | [getSearchOptions()](#getSearchOptions--) | Bu arama sorgusunun arama seçeneklerini alır veya ayarlar. |
|
|  | [setSearchOptions(SearchOptions value)](#setSearchOptions-com.groupdocs.search.options.SearchOptions-) | Bu arama sorgusunun arama seçeneklerini alır veya ayarlar. |
|
|  | [toString()](#toString--) | Geçerli  SearchQuery  örneğini temsil eden bir  System.String  döndürür. |
|
|  | [createWordQuery(String term)](#createWordQuery-java.lang.String-) | Basit bir kelime sorgusu oluşturur. |
|
|  | [createWordPatternQuery(WordPattern pattern)](#createWordPatternQuery-com.groupdocs.search.common.WordPattern-) | Kelime deseni sorgusu oluşturur. |
|
|  | [createRegexQuery(String pattern)](#createRegexQuery-java.lang.String-) | Düzenli ifade sorgusu oluşturur. |
|
|  | [createRegexQuery(String pattern, int options)](#createRegexQuery-java.lang.String-int-) | Düzenli ifade sorgusu oluşturur. |
|
|  | [createNumericRangeQuery(long start, long end)](#createNumericRangeQuery-long-long-) | Sayısal aralık sorgusu oluşturur. |
|
|  | [createDateRangeQuery(Date start, Date end)](#createDateRangeQuery-java.util.Date-java.util.Date-) | Tarih aralık sorgusu oluşturur. |
|
|  | [createPhraseSearchQuery(SearchQuery[] queries)](#createPhraseSearchQuery-com.groupdocs.search.SearchQuery...-) | İfade arama sorgusu oluşturur. |
|
|  | [createAndQuery(SearchQuery[] queries)](#createAndQuery-com.groupdocs.search.SearchQuery---) | Her orijinal sorgu için bulunacak belgeleri yalnızca bulacak bir birleşik sorgu oluşturur. |
|
|  | [createFieldQuery(String fieldName, SearchQuery query)](#createFieldQuery-java.lang.String-com.groupdocs.search.SearchQuery-) | Belirtilen sorguya bir alan ekler. |
|
|  | [createNotQuery(SearchQuery query)](#createNotQuery-com.groupdocs.search.SearchQuery-) | Orijinal sorgu için bulunacak belgelerin tersine, indeksdeki kalan belgeleri bulacak bir ters sorgu oluşturur. |
|
|  | [createAndQuery(SearchQuery leftQuery, SearchQuery rightQuery)](#createAndQuery-com.groupdocs.search.SearchQuery-com.groupdocs.search.SearchQuery-) | Her orijinal sorgu için bulunacak belgeleri yalnızca bulacak bir birleşik sorgu oluşturur. |
|
|  | [createOrQuery(SearchQuery leftQuery, SearchQuery rightQuery)](#createOrQuery-com.groupdocs.search.SearchQuery-com.groupdocs.search.SearchQuery-) | Orijinal sorgulardan en az birinde bulunacak tüm belgeleri bulacak bir birleşik sorgu oluşturur. |
|
|  | [createOrQuery(SearchQuery[] queries)](#createOrQuery-com.groupdocs.search.SearchQuery---) | Orijinal sorgulardan en az birinde bulunacak tüm belgeleri bulacak bir birleşik sorgu oluşturur. |
|
|  | [createWildcardQuery(int count)](#createWildcardQuery-int-) | İfade araması için bir joker karakter oluşturur. |
|
|  | [createWildcardQuery(int minCount, int maxCount)](#createWildcardQuery-int-int-) | İfade araması için bir joker karakter oluşturur. |
|
### getFieldName() {#getFieldName--}
```
public String getFieldName()
```


Alan adını alır.


**Returns:**
java.lang.String - Alan adı.

### getChildCount() {#getChildCount--}
```
public int getChildCount()
```


Alt sorgu sayısını alır.


**Returns:**
int - Alt sorgu sayısı.

### getFirstChild() {#getFirstChild--}
```
public SearchQuery getFirstChild()
```


İlk alt sorguyu alır.


**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - The first child query.

### getSecondChild() {#getSecondChild--}
```
public SearchQuery getSecondChild()
```


İkinci alt sorguyu alır.


**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - The second child query.

### getChild(int index) {#getChild-int-}
```
public abstract SearchQuery getChild(int index)
```


Bir indeksle bir alt sorgu alır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | indeks | int | İndeks. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A child query corresponding the specified index.

### getSearchOptions() {#getSearchOptions--}
```
public final SearchOptions getSearchOptions()
```


Bu arama sorgusunun arama seçeneklerini alır veya ayarlar.


**Returns:**
[SearchOptions](../../com.groupdocs.search.options/searchoptions) - The search options.

### setSearchOptions(SearchOptions value) {#setSearchOptions-com.groupdocs.search.options.SearchOptions-}
```
public final void setSearchOptions(SearchOptions value)
```


Bu arama sorgusunun arama seçeneklerini alır veya ayarlar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | value | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | Arama seçenekleri. |
|

### toString() {#toString--}
```
public abstract String toString()
```


Geçerli  SearchQuery  örneğini temsil eden bir  System.String  döndürür.


**Returns:**
java.lang.String - Geçerli SearchQuery örneğini temsil eden bir System.String.

### createWordQuery(String term) {#createWordQuery-java.lang.String-}
```
public static SearchQuery createWordQuery(String term)
```


Basit bir kelime sorgusu oluşturur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | terim | java.lang.String | Aranacak terim. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A simple word query.

### createWordPatternQuery(WordPattern pattern) {#createWordPatternQuery-com.groupdocs.search.common.WordPattern-}
```
public static SearchQuery createWordPatternQuery(WordPattern pattern)
```


Kelime deseni sorgusu oluşturur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | pattern | [WordPattern](../../com.groupdocs.search.common/wordpattern) | Kelime deseni. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A word pattern query.

### createRegexQuery(String pattern) {#createRegexQuery-java.lang.String-}
```
public static SearchQuery createRegexQuery(String pattern)
```


Düzenli ifade sorgusu oluşturur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | pattern | java.lang.String | Eşleşecek düzenli ifade deseni. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A regular expression query.

### createRegexQuery(String pattern, int options) {#createRegexQuery-java.lang.String-int-}
```
public static SearchQuery createRegexQuery(String pattern, int options)
```


Düzenli ifade sorgusu oluşturur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | pattern | java.lang.String | Eşleşecek düzenli ifade deseni. |
|
|  | options | int | Düzenli ifadeyi değiştiren enum değerlerinin bit düzeyinde birleşimi. Bu değer RegexOptions.IgnoreCase bayrağını içermelidir. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A regular expression query.

### createNumericRangeQuery(long start, long end) {#createNumericRangeQuery-long-long-}
```
public static SearchQuery createNumericRangeQuery(long start, long end)
```


Sayısal aralık sorgusu oluşturur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | başlangıç | uzun | Aralığın başlangıç değeri. |
|
|  | bitiş | uzun | Aralığın bitiş değeri. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A numeric range query.

### createDateRangeQuery(Date start, Date end) {#createDateRangeQuery-java.util.Date-java.util.Date-}
```
public static SearchQuery createDateRangeQuery(Date start, Date end)
```


Tarih aralık sorgusu oluşturur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | başlangıç | java.util.Date | Aralığın başlangıç değeri. |
|
|  | bitiş | java.util.Date | Aralığın bitiş değeri. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A date range query.

### createPhraseSearchQuery(SearchQuery[] queries) {#createPhraseSearchQuery-com.groupdocs.search.SearchQuery...-}
```
public static SearchQuery createPhraseSearchQuery(SearchQuery[] queries)
```


İfade arama sorgusu oluşturur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | queries | [SearchQuery\[\]](../../com.groupdocs.search/searchquery) | Alt sorgular. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A phrase search query.

### createAndQuery(SearchQuery[] queries) {#createAndQuery-com.groupdocs.search.SearchQuery---}
```
public static SearchQuery createAndQuery(SearchQuery[] queries)
```


Her orijinal sorgu için bulunacak belgeleri yalnızca bulacak bir birleşik sorgu oluşturur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | queries | [SearchQuery\[\]](../../com.groupdocs.search/searchquery) | Aranacak alan adı. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined AND query.

### createFieldQuery(String fieldName, SearchQuery query) {#createFieldQuery-java.lang.String-com.groupdocs.search.SearchQuery-}
```
public static SearchQuery createFieldQuery(String fieldName, SearchQuery query)
```


Belirtilen sorguya bir alan ekler.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | fieldName | java.lang.String | Aranacak alan adı. |
|
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | Alanı eklemek için sorgu. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A query with the field to search in.

### createNotQuery(SearchQuery query) {#createNotQuery-com.groupdocs.search.SearchQuery-}
```
public static SearchQuery createNotQuery(SearchQuery query)
```


Orijinal sorgu için bulunacak belgelerin tersine, indeksdeki kalan belgeleri bulacak bir ters sorgu oluşturur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | Tersine çevirmek için sorgu. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined NOT query.

### createAndQuery(SearchQuery leftQuery, SearchQuery rightQuery) {#createAndQuery-com.groupdocs.search.SearchQuery-com.groupdocs.search.SearchQuery-}
```
public static SearchQuery createAndQuery(SearchQuery leftQuery, SearchQuery rightQuery)
```


Her orijinal sorgu için bulunacak belgeleri yalnızca bulacak bir birleşik sorgu oluşturur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | leftQuery | [SearchQuery](../../com.groupdocs.search/searchquery) | Sol alt sorgu. |
|
|  | rightQuery | [SearchQuery](../../com.groupdocs.search/searchquery) | Sağ alt sorgu. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined AND query.

### createOrQuery(SearchQuery leftQuery, SearchQuery rightQuery) {#createOrQuery-com.groupdocs.search.SearchQuery-com.groupdocs.search.SearchQuery-}
```
public static SearchQuery createOrQuery(SearchQuery leftQuery, SearchQuery rightQuery)
```


Orijinal sorgulardan en az birinde bulunacak tüm belgeleri bulacak bir birleşik sorgu oluşturur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | leftQuery | [SearchQuery](../../com.groupdocs.search/searchquery) | Sol alt sorgu. |
|
|  | rightQuery | [SearchQuery](../../com.groupdocs.search/searchquery) | Sağ alt sorgu. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined OR query.

### createOrQuery(SearchQuery[] queries) {#createOrQuery-com.groupdocs.search.SearchQuery---}
```
public static SearchQuery createOrQuery(SearchQuery[] queries)
```


Orijinal sorgulardan en az birinde bulunacak tüm belgeleri bulacak bir birleşik sorgu oluşturur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | queries | [SearchQuery\[\]](../../com.groupdocs.search/searchquery) | Alt sorgular. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined OR query.

### createWildcardQuery(int count) {#createWildcardQuery-int-}
```
public static SearchQuery createWildcardQuery(int count)
```


İfade araması için bir joker karakter oluşturur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | sayım | int | Wildcard'taki kelime sayısı. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A wildcard for the phrase search.

### createWildcardQuery(int minCount, int maxCount) {#createWildcardQuery-int-int-}
```
public static SearchQuery createWildcardQuery(int minCount, int maxCount)
```


İfade araması için bir joker karakter oluşturur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | minCount | int | Wildcard'taki minimum kelime sayısı. |
|
|  | maxCount | int | Wildcard'taki maksimum kelime sayısı. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A wildcard for the phrase search.

