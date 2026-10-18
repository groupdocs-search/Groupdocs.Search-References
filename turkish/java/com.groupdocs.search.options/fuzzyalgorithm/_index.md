---
title: "FuzzyAlgorithm"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Bulanık arama algoritmaları için temel sınıfı temsil eder."
type: docs
weight: 20
url: /tr/java/com.groupdocs.search.options/fuzzyalgorithm/
---
**Inheritance:**
java.lang.Object
```
public abstract class FuzzyAlgorithm
```

Bulanık arama algoritmaları için temel sınıfı temsil eder.


**Learn more**

* [Fuzzy search](../https://docs.groupdocs.com/display/searchjava/Fuzzy+search)

## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getSimilarityLevel(int termLength)](#getSimilarityLevel-int-) | Belirtilen terim uzunluğu için benzerlik seviyesini alır. |
|
|  | [getMaxMistakeCount(int termLength)](#getMaxMistakeCount-int-) | Belirtilen terim uzunluğu için izin verilen maksimum hata sayısını alır. |
|
| [getCore()](#getCore--) |  |
### getSimilarityLevel(int termLength) {#getSimilarityLevel-int-}
```
public abstract double getSimilarityLevel(int termLength)
```


Belirtilen terim uzunluğu için benzerlik seviyesini alır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | termLength | int | Terim uzunluğu. |
|

**Returns:**
double - Benzerlik seviyesi.

### getMaxMistakeCount(int termLength) {#getMaxMistakeCount-int-}
```
public abstract int getMaxMistakeCount(int termLength)
```


Belirtilen terim uzunluğu için izin verilen maksimum hata sayısını alır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | termLength | int | Terim uzunluğu. |
|

**Returns:**
int - İzin verilen maksimum hata sayısı.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
