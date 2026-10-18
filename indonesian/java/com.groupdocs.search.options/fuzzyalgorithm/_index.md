---
title: "FuzzyAlgorithm"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili kelas dasar untuk algoritma pencarian fuzzy."
type: docs
weight: 20
url: /id/java/com.groupdocs.search.options/fuzzyalgorithm/
---
**Inheritance:**
java.lang.Object
```
public abstract class FuzzyAlgorithm
```

Mewakili kelas dasar untuk algoritma pencarian fuzzy.


**Learn more**

* [Fuzzy search](../https://docs.groupdocs.com/display/searchjava/Fuzzy+search)

## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getSimilarityLevel(int termLength)](#getSimilarityLevel-int-) | Mendapatkan tingkat kemiripan untuk panjang istilah yang ditentukan. |
|
|  | [getMaxMistakeCount(int termLength)](#getMaxMistakeCount-int-) | Mendapatkan jumlah maksimum kesalahan yang diizinkan untuk panjang istilah yang ditentukan. |
|
| [getCore()](#getCore--) |  |
### getSimilarityLevel(int termLength) {#getSimilarityLevel-int-}
```
public abstract double getSimilarityLevel(int termLength)
```


Mendapatkan tingkat kemiripan untuk panjang istilah yang ditentukan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | termLength | int | Panjang istilah. |
|

**Returns:**
double - Tingkat kemiripan.

### getMaxMistakeCount(int termLength) {#getMaxMistakeCount-int-}
```
public abstract int getMaxMistakeCount(int termLength)
```


Mendapatkan jumlah maksimum kesalahan yang diizinkan untuk panjang istilah yang ditentukan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | termLength | int | Panjang istilah. |
|

**Returns:**
int - Jumlah kesalahan maksimum yang diizinkan.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
