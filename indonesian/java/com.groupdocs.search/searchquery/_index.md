---
title: "SearchQuery"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili kueri pencarian dalam bentuk objek."
type: docs
weight: 25
url: /id/java/com.groupdocs.search/searchquery/
---
**Inheritance:**
java.lang.Object
```
public abstract class SearchQuery
```

Mewakili kueri pencarian dalam bentuk objek.


**Learn more**

* [Searching](../https://docs.groupdocs.com/display/searchjava/Searching)
* [Queries in text and object form](../https://docs.groupdocs.com/display/searchjava/Queries+in+text+and+object+form)
* [Nesting search queries in object form](../https://docs.groupdocs.com/display/searchjava/Nesting+search+queries+in+object+form)


Contoh ini menunjukkan penggunaan tipikal kelas tersebut.

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


## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getFieldName()](#getFieldName--) | Mendapatkan nama bidang. |
|
|  | [getChildCount()](#getChildCount--) | Mendapatkan jumlah kueri anak. |
|
|  | [getFirstChild()](#getFirstChild--) | Mendapatkan kueri anak pertama. |
|
|  | [getSecondChild()](#getSecondChild--) | Mendapatkan kueri anak kedua. |
|
|  | [getChild(int index)](#getChild-int-) | Mendapatkan kueri anak berdasarkan indeks. |
|
|  | [getSearchOptions()](#getSearchOptions--) | Mendapatkan atau mengatur opsi pencarian dari kueri pencarian ini. |
|
|  | [setSearchOptions(SearchOptions value)](#setSearchOptions-com.groupdocs.search.options.SearchOptions-) | Mendapatkan atau mengatur opsi pencarian dari kueri pencarian ini. |
|
|  | [toString()](#toString--) | Mengembalikan sebuah  System.String  yang mewakili instance  SearchQuery  saat ini. |
|
|  | [createWordQuery(String term)](#createWordQuery-java.lang.String-) | Membuat kueri kata sederhana. |
|
|  | [createWordPatternQuery(WordPattern pattern)](#createWordPatternQuery-com.groupdocs.search.common.WordPattern-) | Membuat kueri pola kata. |
|
|  | [createRegexQuery(String pattern)](#createRegexQuery-java.lang.String-) | Membuat kueri ekspresi reguler. |
|
|  | [createRegexQuery(String pattern, int options)](#createRegexQuery-java.lang.String-int-) | Membuat kueri ekspresi reguler. |
|
|  | [createNumericRangeQuery(long start, long end)](#createNumericRangeQuery-long-long-) | Membuat kueri rentang numerik. |
|
|  | [createDateRangeQuery(Date start, Date end)](#createDateRangeQuery-java.util.Date-java.util.Date-) | Membuat kueri rentang tanggal. |
|
|  | [createPhraseSearchQuery(SearchQuery[] queries)](#createPhraseSearchQuery-com.groupdocs.search.SearchQuery...-) | Membuat kueri pencarian frasa. |
|
|  | [createAndQuery(SearchQuery[] queries)](#createAndQuery-com.groupdocs.search.SearchQuery---) | Membuat kueri gabungan yang hanya akan menemukan dokumen yang akan ditemukan untuk setiap kueri asli. |
|
|  | [createFieldQuery(String fieldName, SearchQuery query)](#createFieldQuery-java.lang.String-com.groupdocs.search.SearchQuery-) | Menambahkan bidang ke kueri yang ditentukan. |
|
|  | [createNotQuery(SearchQuery query)](#createNotQuery-com.groupdocs.search.SearchQuery-) | Membuat kueri terbalik yang akan menemukan dokumen lainnya dalam indeks dibandingkan dengan yang akan ditemukan untuk kueri asli. |
|
|  | [createAndQuery(SearchQuery leftQuery, SearchQuery rightQuery)](#createAndQuery-com.groupdocs.search.SearchQuery-com.groupdocs.search.SearchQuery-) | Membuat kueri gabungan yang hanya akan menemukan dokumen yang akan ditemukan untuk setiap kueri asli. |
|
|  | [createOrQuery(SearchQuery leftQuery, SearchQuery rightQuery)](#createOrQuery-com.groupdocs.search.SearchQuery-com.groupdocs.search.SearchQuery-) | Membuat kueri gabungan yang akan menemukan semua dokumen yang akan ditemukan setidaknya untuk satu dari kueri asli. |
|
|  | [createOrQuery(SearchQuery[] queries)](#createOrQuery-com.groupdocs.search.SearchQuery---) | Membuat kueri gabungan yang akan menemukan semua dokumen yang akan ditemukan setidaknya untuk satu dari kueri asli. |
|
|  | [createWildcardQuery(int count)](#createWildcardQuery-int-) | Membuat wildcard untuk pencarian frasa. |
|
|  | [createWildcardQuery(int minCount, int maxCount)](#createWildcardQuery-int-int-) | Membuat wildcard untuk pencarian frasa. |
|
### getFieldName() {#getFieldName--}
```
public String getFieldName()
```


Mendapatkan nama bidang.


**Returns:**
java.lang.String - Nama bidang.

### getChildCount() {#getChildCount--}
```
public int getChildCount()
```


Mendapatkan jumlah kueri anak.


**Returns:**
int - Jumlah kueri anak.

### getFirstChild() {#getFirstChild--}
```
public SearchQuery getFirstChild()
```


Mendapatkan kueri anak pertama.


**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - The first child query.

### getSecondChild() {#getSecondChild--}
```
public SearchQuery getSecondChild()
```


Mendapatkan kueri anak kedua.


**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - The second child query.

### getChild(int index) {#getChild-int-}
```
public abstract SearchQuery getChild(int index)
```


Mendapatkan kueri anak berdasarkan indeks.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | indeks | int | Indeks. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A child query corresponding the specified index.

### getSearchOptions() {#getSearchOptions--}
```
public final SearchOptions getSearchOptions()
```


Mendapatkan atau mengatur opsi pencarian dari kueri pencarian ini.


**Returns:**
[SearchOptions](../../com.groupdocs.search.options/searchoptions) - The search options.

### setSearchOptions(SearchOptions value) {#setSearchOptions-com.groupdocs.search.options.SearchOptions-}
```
public final void setSearchOptions(SearchOptions value)
```


Mendapatkan atau mengatur opsi pencarian dari kueri pencarian ini.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | value | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | Opsi pencarian. |
|

### toString() {#toString--}
```
public abstract String toString()
```


Mengembalikan sebuah  System.String  yang mewakili instance  SearchQuery  saat ini.


**Returns:**
java.lang.String - Sebuah System.String yang mewakili instance SearchQuery saat ini.

### createWordQuery(String term) {#createWordQuery-java.lang.String-}
```
public static SearchQuery createWordQuery(String term)
```


Membuat kueri kata sederhana.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | istilah | java.lang.String | Istilah untuk dicari. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A simple word query.

### createWordPatternQuery(WordPattern pattern) {#createWordPatternQuery-com.groupdocs.search.common.WordPattern-}
```
public static SearchQuery createWordPatternQuery(WordPattern pattern)
```


Membuat kueri pola kata.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | pattern | [WordPattern](../../com.groupdocs.search.common/wordpattern) | Pola kata. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A word pattern query.

### createRegexQuery(String pattern) {#createRegexQuery-java.lang.String-}
```
public static SearchQuery createRegexQuery(String pattern)
```


Membuat kueri ekspresi reguler.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | pattern | java.lang.String | Pola ekspresi reguler untuk dicocokkan. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A regular expression query.

### createRegexQuery(String pattern, int options) {#createRegexQuery-java.lang.String-int-}
```
public static SearchQuery createRegexQuery(String pattern, int options)
```


Membuat kueri ekspresi reguler.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | pattern | java.lang.String | Pola ekspresi reguler untuk dicocokkan. |
|
|  | options | int | Kombinasi bitwise dari nilai enumerasi yang memodifikasi ekspresi reguler. Nilai ini harus mengandung flag  RegexOptions.IgnoreCase . |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A regular expression query.

### createNumericRangeQuery(long start, long end) {#createNumericRangeQuery-long-long-}
```
public static SearchQuery createNumericRangeQuery(long start, long end)
```


Membuat kueri rentang numerik.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | mulai | long | Nilai mulai dari rentang. |
|
|  | akhir | long | Nilai akhir dari rentang. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A numeric range query.

### createDateRangeQuery(Date start, Date end) {#createDateRangeQuery-java.util.Date-java.util.Date-}
```
public static SearchQuery createDateRangeQuery(Date start, Date end)
```


Membuat kueri rentang tanggal.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | mulai | java.util.Date | Nilai mulai dari rentang. |
|
|  | akhir | java.util.Date | Nilai akhir dari rentang. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A date range query.

### createPhraseSearchQuery(SearchQuery[] queries) {#createPhraseSearchQuery-com.groupdocs.search.SearchQuery...-}
```
public static SearchQuery createPhraseSearchQuery(SearchQuery[] queries)
```


Membuat kueri pencarian frasa.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | queries | [SearchQuery\[\]](../../com.groupdocs.search/searchquery) | Kueri anak. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A phrase search query.

### createAndQuery(SearchQuery[] queries) {#createAndQuery-com.groupdocs.search.SearchQuery---}
```
public static SearchQuery createAndQuery(SearchQuery[] queries)
```


Membuat kueri gabungan yang hanya akan menemukan dokumen yang akan ditemukan untuk setiap kueri asli.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | queries | [SearchQuery\[\]](../../com.groupdocs.search/searchquery) | Nama bidang untuk dicari. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined AND query.

### createFieldQuery(String fieldName, SearchQuery query) {#createFieldQuery-java.lang.String-com.groupdocs.search.SearchQuery-}
```
public static SearchQuery createFieldQuery(String fieldName, SearchQuery query)
```


Menambahkan bidang ke kueri yang ditentukan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | fieldName | java.lang.String | Nama bidang untuk dicari. |
|
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | Kueri untuk menambahkan bidang. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A query with the field to search in.

### createNotQuery(SearchQuery query) {#createNotQuery-com.groupdocs.search.SearchQuery-}
```
public static SearchQuery createNotQuery(SearchQuery query)
```


Membuat kueri terbalik yang akan menemukan dokumen lainnya dalam indeks dibandingkan dengan yang akan ditemukan untuk kueri asli.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | Kueri untuk membalikkan. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined NOT query.

### createAndQuery(SearchQuery leftQuery, SearchQuery rightQuery) {#createAndQuery-com.groupdocs.search.SearchQuery-com.groupdocs.search.SearchQuery-}
```
public static SearchQuery createAndQuery(SearchQuery leftQuery, SearchQuery rightQuery)
```


Membuat kueri gabungan yang hanya akan menemukan dokumen yang akan ditemukan untuk setiap kueri asli.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | leftQuery | [SearchQuery](../../com.groupdocs.search/searchquery) | Kueri anak kiri. |
|
|  | rightQuery | [SearchQuery](../../com.groupdocs.search/searchquery) | Kueri anak kanan. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined AND query.

### createOrQuery(SearchQuery leftQuery, SearchQuery rightQuery) {#createOrQuery-com.groupdocs.search.SearchQuery-com.groupdocs.search.SearchQuery-}
```
public static SearchQuery createOrQuery(SearchQuery leftQuery, SearchQuery rightQuery)
```


Membuat kueri gabungan yang akan menemukan semua dokumen yang akan ditemukan setidaknya untuk satu dari kueri asli.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | leftQuery | [SearchQuery](../../com.groupdocs.search/searchquery) | Kueri anak kiri. |
|
|  | rightQuery | [SearchQuery](../../com.groupdocs.search/searchquery) | Kueri anak kanan. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined OR query.

### createOrQuery(SearchQuery[] queries) {#createOrQuery-com.groupdocs.search.SearchQuery---}
```
public static SearchQuery createOrQuery(SearchQuery[] queries)
```


Membuat kueri gabungan yang akan menemukan semua dokumen yang akan ditemukan setidaknya untuk satu dari kueri asli.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | queries | [SearchQuery\[\]](../../com.groupdocs.search/searchquery) | Kueri anak. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined OR query.

### createWildcardQuery(int count) {#createWildcardQuery-int-}
```
public static SearchQuery createWildcardQuery(int count)
```


Membuat wildcard untuk pencarian frasa.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | count | int | Jumlah kata dalam wildcard. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A wildcard for the phrase search.

### createWildcardQuery(int minCount, int maxCount) {#createWildcardQuery-int-int-}
```
public static SearchQuery createWildcardQuery(int minCount, int maxCount)
```


Membuat wildcard untuk pencarian frasa.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | minCount | int | Jumlah minimum kata dalam wildcard. |
|
|  | maxCount | int | Jumlah maksimum kata dalam wildcard. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A wildcard for the phrase search.

