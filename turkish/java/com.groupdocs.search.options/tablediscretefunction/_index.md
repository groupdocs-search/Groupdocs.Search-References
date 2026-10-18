---
title: "TableDiscreteFunction"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Kelime uzunlukları ile izin verilen hata sayısı arasındaki karşılıkları içeren bulanık arama algoritmasını temsil eder."
type: docs
weight: 40
url: /tr/java/com.groupdocs.search.options/tablediscretefunction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.options.FuzzyAlgorithm](../../com.groupdocs.search.options/fuzzyalgorithm)
```
public class TableDiscreteFunction extends FuzzyAlgorithm
```

Kelime uzunlukları ile izin verilen hata sayısı arasındaki ilişkileri içeren bulanık arama algoritmasını temsil eder. Bu algoritma, çıktı değerleri tablosu veya bir adım fonksiyonu ile belirtilebilir.


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
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1, new Step(5, 2), new Step(8, 3))); // Bulanık arama algoritması oluşturuluyor
// Bu işlev, 1 ila 4 karakter uzunluğundaki kelimeler için maksimum hata sayısını 1 olarak belirler.
// 5 ila 7 karakter uzunluğundaki kelimeler için maksimum hata sayısını 2 olarak belirler.
// 8 ve daha fazla karakter uzunluğundaki kelimeler için maksimum hata sayısını 3 olarak belirler.
SearchResult result = index.search(query, options); // İndekste arama
 
```
 
````


## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [TableDiscreteFunction(int offsetOfInputs, int[] tableOfOutputs)](#TableDiscreteFunction-int-int---) | TableDiscreteFunction sınıfının yeni bir örneğini başlatır. |
|
|  | [TableDiscreteFunction(int firstStepLevel, Step[] steps)](#TableDiscreteFunction-int-com.groupdocs.search.options.Step...-) | TableDiscreteFunction sınıfının yeni bir örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getSimilarityLevel(int termLength)](#getSimilarityLevel-int-) | Belirtilen terim uzunluğu için bir benzerlik seviyesi alır. |
|
|  | [getMaxMistakeCount(int termLength)](#getMaxMistakeCount-int-) | Belirtilen terim uzunluğu için izin verilen maksimum hata sayısını alır. |
|
### TableDiscreteFunction(int offsetOfInputs, int[] tableOfOutputs) {#TableDiscreteFunction-int-int---}
```
public TableDiscreteFunction(int offsetOfInputs, int[] tableOfOutputs)
```


TableDiscreteFunction sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | offsetOfInputs | int | Tablo indislerinin giriş değerlerine göre ofseti. |
|
|  | tableOfOutputs | int[] | Çıktı değerlerinin tablosu. |
|

### TableDiscreteFunction(int firstStepLevel, Step[] steps) {#TableDiscreteFunction-int-com.groupdocs.search.options.Step...-}
```
public TableDiscreteFunction(int firstStepLevel, Step[] steps)
```


TableDiscreteFunction sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | firstStepLevel | int | Adım fonksiyonunun ilk adımının seviyesi. |
|
|  | steps | [Step\[\]](../../com.groupdocs.search.options/step) | Adım fonksiyonunun sonraki adımları. |
|

### getSimilarityLevel(int termLength) {#getSimilarityLevel-int-}
```
public double getSimilarityLevel(int termLength)
```


Belirtilen terim uzunluğu için bir benzerlik seviyesi alır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | termLength | int | Terim uzunluğu. |
|

**Returns:**
double - Bir benzerlik seviyesi.

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

