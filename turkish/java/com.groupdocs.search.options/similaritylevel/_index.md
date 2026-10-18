---
title: "SimilarityLevel"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Benzerlik seviyesini belirten bulanık arama algoritmasını temsil eder."
type: docs
weight: 35
url: /tr/java/com.groupdocs.search.options/similaritylevel/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.options.FuzzyAlgorithm](../../com.groupdocs.search.options/fuzzyalgorithm)
```
public class SimilarityLevel extends FuzzyAlgorithm
```

Bulanık aramanın benzerlik seviyesini belirten bir algoritmayı temsil eder. Benzerlik seviyesi algoritması, bir kelimenin hata sayısını kelime uzunluğunun ters orantılı olarak maksimum hatalar olarak hesaplar.


**Learn more**

* [Fuzzy search](../https://docs.groupdocs.com/display/searchjava/Fuzzy+search)


Örnek, sınıfın tipik bir kullanımını gösterir.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Belirtilen klasörde bir indeks oluşturuluyor
index.add(documentsFolder); // Belirtilen klasörden belgeleri indeksleme
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // Bulanık aramayı etkinleştiriyor
options.getFuzzySearch().setFuzzyAlgorithm(new SimilarityLevel(0.8)); // Bulanık arama algoritması oluşturuluyor
// Bu işlev, 1 ila 4 karakter uzunluğundaki kelimeler için maksimum hata sayısını 0 olarak belirler.
// 5 ila 9 karakter uzunluğundaki kelimeler için maksimum hata sayısını 1 olarak belirler.
// 10 ila 14 karakter uzunluğundaki kelimeler için maksimum hata sayısını 2 olarak belirler. Ve buna benzer şekilde devam eder.
SearchResult result = index.search(query, options); // İndekste arama
 
```
 
````


## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [SimilarityLevel(double value)](#SimilarityLevel-double-) | SimilarityLevel sınıfının yeni bir örneğini başlatır. |
|
|  | [SimilarityLevel(Object data)](#SimilarityLevel-java.lang.Object-) | SimilarityLevel sınıfının yeni bir örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getSimilarityLevel(int termLength)](#getSimilarityLevel-int-) | Belirtilen terim uzunluğu için benzerlik seviyesi değerini alır. |
|
|  | [getMaxMistakeCount(int termLength)](#getMaxMistakeCount-int-) | Belirtilen terim uzunluğu için izin verilen maksimum hata sayısını alır. |
|
### SimilarityLevel(double value) {#SimilarityLevel-double-}
```
public SimilarityLevel(double value)
```


SimilarityLevel sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | double | Benzerlik seviyesi değeri. |
|

### SimilarityLevel(Object data) {#SimilarityLevel-java.lang.Object-}
```
public SimilarityLevel(Object data)
```


SimilarityLevel sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | veri | java.lang.Object | Serileştirilmiş veri. |
|

### getSimilarityLevel(int termLength) {#getSimilarityLevel-int-}
```
public double getSimilarityLevel(int termLength)
```


Belirtilen terim uzunluğu için benzerlik seviyesi değerini alır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | termLength | int | Terim uzunluğu. |
|

**Returns:**
double - Benzerlik seviyesi değeri.

### getMaxMistakeCount(int termLength) {#getMaxMistakeCount-int-}
```
public int getMaxMistakeCount(int termLength)
```


Belirtilen terim uzunluğu için izin verilen maksimum hata sayısını alır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | termLength | int | Terim uzunluğu. |
|

**Returns:**
int - İzin verilen maksimum hata sayısı.

