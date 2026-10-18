---
title: "FuzzySearchOptions"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Bulanık arama için seçenekler sağlar."
type: docs
weight: 21
url: /tr/java/com.groupdocs.search.options/fuzzysearchoptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class FuzzySearchOptions
```

Bulanık arama için seçenekler sağlar.


**Learn more**

* [Fuzzy search](../https://docs.groupdocs.com/display/searchjava/Fuzzy+search)
* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [FuzzySearchOptions()](#FuzzySearchOptions--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getEnabled()](#getEnabled--) | Bulanık arama özelliğinin etkin olup olmadığını gösteren bir değer alır. |
|
|  | [setEnabled(boolean value)](#setEnabled-boolean-) | Bulanık arama özelliğinin etkin olup olmadığını gösteren bir değer ayarlar. |
|
|  | [getFuzzyAlgorithm()](#getFuzzyAlgorithm--) | Bulanık arama algoritmasını alır. |
|
|  | [setFuzzyAlgorithm(FuzzyAlgorithm value)](#setFuzzyAlgorithm-com.groupdocs.search.options.FuzzyAlgorithm-) | Bulanık arama algoritmasını ayarlar. |
|
|  | [getOnlyBestResults()](#getOnlyBestResults--) | Yalnızca en iyi sonuçların döndürüleceğini gösteren bir değeri alır. |
|
|  | [setOnlyBestResults(boolean value)](#setOnlyBestResults-boolean-) | Yalnızca en iyi sonuçların döndürüleceğini gösteren bir değeri ayarlar. |
|
|  | [getOnlyBestResultsRange()](#getOnlyBestResultsRange--) | Bulunan minimum hata sayısının üstündeki maksimum aşımı alır. |
|
|  | [setOnlyBestResultsRange(byte value)](#setOnlyBestResultsRange-byte-) | Bulunan minimum hata sayısının üstündeki maksimum aşımı ayarlar. |
|
|  | [getConsiderTranspositions()](#getConsiderTranspositions--) | Bulanık arama algoritmasının iki yan yana karakterin yer değiştirmesini tek bir hata olarak değerlendirmesi gerekip gerekmediğini gösteren bir değer alır. |
|
|  | [setConsiderTranspositions(boolean value)](#setConsiderTranspositions-boolean-) | Bulanık arama algoritmasının iki yan yana karakterin yer değiştirmesini tek bir hata olarak değerlendirmesi gerekip gerekmediğini gösteren bir değer ayarlar. |
|
### FuzzySearchOptions() {#FuzzySearchOptions--}
```
public FuzzySearchOptions()
```


### getEnabled() {#getEnabled--}
```
public abstract boolean getEnabled()
```


Bulanık arama özelliğinin etkin olup olmadığını gösteren bir değer alır. Varsayılan değer false.


**Returns:**
boolean - Bulanık arama özelliğinin etkin olup olmadığını gösteren bir değer.

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public abstract void setEnabled(boolean value)
```


Bulanık arama özelliğinin etkin olup olmadığını gösteren bir değer ayarlar. Varsayılan değer false.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | boolean | Bulanık arama özelliğinin etkin olup olmadığını gösteren bir değer. |
|

### getFuzzyAlgorithm() {#getFuzzyAlgorithm--}
```
public abstract FuzzyAlgorithm getFuzzyAlgorithm()
```


Bulanık arama algoritmasını alır. Şu anda mevcut olan bulanık arama algoritmaları SimilarityLevel ve TableDiscreteFunction'dır. Varsayılan değer, benzerlik seviyesi değeri 0.5 olan bir SimilarityLevel örneğidir.


**Returns:**
[FuzzyAlgorithm](../../com.groupdocs.search.options/fuzzyalgorithm) - The fuzzy search algorithm.


Örnek, bulanık arama algoritmasının nasıl ayarlanacağını gösterir.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Belirtilen klasörde bir indeks oluşturuluyor
index.add(documentsFolder); // Belirtilen klasörden belgeleri indeksleme
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // Bulanık aramayı etkinleştiriyor
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1, new Step(5, 2), new Step(8, 3))); // Bulanık arama algoritması oluşturuluyor
// Bu işlev, 1 ila 4 karakter uzunluğundaki kelimeler için maksimum hata sayısını 1 olarak belirler.
// 5 ila 7 karakter uzunluğundaki kelimeler için maksimum hata sayısını 2 olarak belirler.
// 8 ve daha fazla karakter uzunluğundaki kelimeler için maksimum hata sayısını 3 olarak belirler.
SearchResult result = index.search(query, options); // İndekste arama
 
```
 
````


### setFuzzyAlgorithm(FuzzyAlgorithm value) {#setFuzzyAlgorithm-com.groupdocs.search.options.FuzzyAlgorithm-}
```
public abstract void setFuzzyAlgorithm(FuzzyAlgorithm value)
```


Bulanık arama algoritmasını ayarlar. Şu anda mevcut olan bulanık arama algoritmaları SimilarityLevel ve TableDiscreteFunction'dır. Varsayılan değer, benzerlik seviyesi değeri 0.5 olan bir SimilarityLevel örneğidir.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | value | [FuzzyAlgorithm](../../com.groupdocs.search.options/fuzzyalgorithm) | Bulanık arama algoritması. |


Örnek, bulanık arama algoritmasının nasıl ayarlanacağını gösterir.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Belirtilen klasörde bir indeks oluşturuluyor
index.add(documentsFolder); // Belirtilen klasörden belgeleri indeksleme
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // Bulanık aramayı etkinleştiriyor
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1, new Step(5, 2), new Step(8, 3))); // Bulanık arama algoritması oluşturuluyor
// Bu işlev, 1 ila 4 karakter uzunluğundaki kelimeler için maksimum hata sayısını 1 olarak belirler.
// 5 ila 7 karakter uzunluğundaki kelimeler için maksimum hata sayısını 2 olarak belirler.
// 8 ve daha fazla karakter uzunluğundaki kelimeler için maksimum hata sayısını 3 olarak belirler.
SearchResult result = index.search(query, options); // İndekste arama
 
```
 
````

|

### getOnlyBestResults() {#getOnlyBestResults--}
```
public abstract boolean getOnlyBestResults()
```


Yalnızca en iyi sonuçların döndürüleceğini gösteren bir değeri alır. Varsayılan değer false.


**Returns:**
boolean - true if only the best results will be returned; otherwise false.

### setOnlyBestResults(boolean value) {#setOnlyBestResults-boolean-}
```
public abstract void setOnlyBestResults(boolean value)
```


Yalnızca en iyi sonuçların döndürüleceğini gösteren bir değeri ayarlar. Varsayılan değer false.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | boolean | yalnızca en iyi sonuçların döndürüleceği durumda true; aksi takdirde false. |
|

### getOnlyBestResultsRange() {#getOnlyBestResultsRange--}
```
public abstract byte getOnlyBestResultsRange()
```


Bulunan en az hata sayısının maksimum aşımını alır. Varsayılan değer 0'dır.


**Returns:**
byte - Bulunan en az hata sayısının maksimum aşımı.

### setOnlyBestResultsRange(byte value) {#setOnlyBestResultsRange-byte-}
```
public abstract void setOnlyBestResultsRange(byte value)
```


Bulunan en az hata sayısının maksimum aşımını ayarlar. Varsayılan değer 0'dır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | byte | Bulunan en az hata sayısının maksimum aşımı. |
|

### getConsiderTranspositions() {#getConsiderTranspositions--}
```
public abstract boolean getConsiderTranspositions()
```


Bulanık arama algoritmasının iki yan yana karakterin yer değiştirmesini tek bir hata olarak değerlendirip değerlendirmediğini gösteren bir değer alır. Varsayılan değer true.


**Returns:**
boolean - true eğer bulanık arama algoritması yer değiştirmeleri dikkate alıyorsa; aksi takdirde false.

### setConsiderTranspositions(boolean value) {#setConsiderTranspositions-boolean-}
```
public abstract void setConsiderTranspositions(boolean value)
```


Bulanık arama algoritmasının iki yan yana karakterin yer değiştirmesini tek bir hata olarak değerlendirip değerlendirmediğini gösteren bir değer ayarlar. Varsayılan değer true.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | boolean | : true eğer bulanık arama algoritması yer değiştirmeleri dikkate alıyorsa; aksi takdirde false. |
|

