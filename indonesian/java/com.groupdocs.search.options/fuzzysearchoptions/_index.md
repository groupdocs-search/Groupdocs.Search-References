---
title: "FuzzySearchOptions"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Menyediakan opsi pencarian fuzzy."
type: docs
weight: 21
url: /id/java/com.groupdocs.search.options/fuzzysearchoptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class FuzzySearchOptions
```

Menyediakan opsi pencarian fuzzy.


**Learn more**

* [Fuzzy search](../https://docs.groupdocs.com/display/searchjava/Fuzzy+search)
* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [FuzzySearchOptions()](#FuzzySearchOptions--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getEnabled()](#getEnabled--) | Mendapatkan nilai yang menunjukkan apakah fitur pencarian fuzzy diaktifkan. |
|
|  | [setEnabled(boolean value)](#setEnabled-boolean-) | Mengatur nilai yang menunjukkan apakah fitur pencarian fuzzy diaktifkan. |
|
|  | [getFuzzyAlgorithm()](#getFuzzyAlgorithm--) | Mengambil algoritma pencarian fuzzy. |
|
|  | [setFuzzyAlgorithm(FuzzyAlgorithm value)](#setFuzzyAlgorithm-com.groupdocs.search.options.FuzzyAlgorithm-) | Mengatur algoritma pencarian fuzzy. |
|
|  | [getOnlyBestResults()](#getOnlyBestResults--) | Mendapatkan nilai yang menunjukkan apakah hanya hasil terbaik yang akan dikembalikan. |
|
|  | [setOnlyBestResults(boolean value)](#setOnlyBestResults-boolean-) | Mengatur nilai yang menunjukkan apakah hanya hasil terbaik yang akan dikembalikan. |
|
|  | [getOnlyBestResultsRange()](#getOnlyBestResultsRange--) | Mendapatkan kelebihan maksimum dari jumlah minimum kesalahan yang ditemukan. |
|
|  | [setOnlyBestResultsRange(byte value)](#setOnlyBestResultsRange-byte-) | Mengatur kelebihan maksimum dari jumlah minimum kesalahan yang ditemukan. |
|
|  | [getConsiderTranspositions()](#getConsiderTranspositions--) | Mengambil nilai yang menunjukkan apakah algoritma pencarian fuzzy harus mempertimbangkan pertukaran dua karakter berdekatan sebagai satu kesalahan. |
|
|  | [setConsiderTranspositions(boolean value)](#setConsiderTranspositions-boolean-) | Mengatur nilai yang menunjukkan apakah algoritma pencarian fuzzy harus mempertimbangkan pertukaran dua karakter berdekatan sebagai satu kesalahan. |
|
### FuzzySearchOptions() {#FuzzySearchOptions--}
```
public FuzzySearchOptions()
```


### getEnabled() {#getEnabled--}
```
public abstract boolean getEnabled()
```


Mengambil nilai yang menunjukkan apakah fitur pencarian fuzzy diaktifkan. Nilai default adalah false.


**Returns:**
boolean - Nilai yang menunjukkan apakah fitur pencarian fuzzy diaktifkan.

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public abstract void setEnabled(boolean value)
```


Mengatur nilai yang menunjukkan apakah fitur pencarian fuzzy diaktifkan. Nilai default adalah false.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | boolean | Nilai yang menunjukkan apakah fitur pencarian fuzzy diaktifkan. |
|

### getFuzzyAlgorithm() {#getFuzzyAlgorithm--}
```
public abstract FuzzyAlgorithm getFuzzyAlgorithm()
```


Mengambil algoritma pencarian fuzzy. Algoritma pencarian fuzzy yang saat ini tersedia adalah SimilarityLevel dan TableDiscreteFunction. Nilai default adalah sebuah instance dari SimilarityLevel dengan nilai tingkat kemiripan 0.5.


**Returns:**
[FuzzyAlgorithm](../../com.groupdocs.search.options/fuzzyalgorithm) - The fuzzy search algorithm.


Contoh ini menunjukkan cara mengatur algoritma pencarian fuzzy.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Membuat indeks di folder yang ditentukan
index.add(documentsFolder); // Mengindeks dokumen dari folder yang ditentukan
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // Mengaktifkan pencarian fuzzy
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1, new Step(5, 2), new Step(8, 3))); // Membuat algoritma pencarian fuzzy
// Fungsi ini menentukan 1 sebagai jumlah maksimum kesalahan untuk kata dengan panjang 1 hingga 4 karakter.
// Menentukan 2 sebagai jumlah maksimum kesalahan untuk kata dengan panjang 5 hingga 7 karakter.
// Menentukan 3 sebagai jumlah maksimum kesalahan untuk kata dengan panjang 8 karakter ke atas.
SearchResult result = index.search(query, options); // Cari di indeks
 
```
 
````


### setFuzzyAlgorithm(FuzzyAlgorithm value) {#setFuzzyAlgorithm-com.groupdocs.search.options.FuzzyAlgorithm-}
```
public abstract void setFuzzyAlgorithm(FuzzyAlgorithm value)
```


Mengatur algoritma pencarian fuzzy. Algoritma pencarian fuzzy yang saat ini tersedia adalah SimilarityLevel dan TableDiscreteFunction. Nilai default adalah sebuah instance dari SimilarityLevel dengan nilai tingkat kemiripan 0.5.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | value | [FuzzyAlgorithm](../../com.groupdocs.search.options/fuzzyalgorithm) | Algoritma pencarian fuzzy. |


Contoh ini menunjukkan cara mengatur algoritma pencarian fuzzy.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Membuat indeks di folder yang ditentukan
index.add(documentsFolder); // Mengindeks dokumen dari folder yang ditentukan
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // Mengaktifkan pencarian fuzzy
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1, new Step(5, 2), new Step(8, 3))); // Membuat algoritma pencarian fuzzy
// Fungsi ini menentukan 1 sebagai jumlah maksimum kesalahan untuk kata dengan panjang 1 hingga 4 karakter.
// Menentukan 2 sebagai jumlah maksimum kesalahan untuk kata dengan panjang 5 hingga 7 karakter.
// Menentukan 3 sebagai jumlah maksimum kesalahan untuk kata dengan panjang 8 karakter ke atas.
SearchResult result = index.search(query, options); // Cari di indeks
 
```
 
````

|

### getOnlyBestResults() {#getOnlyBestResults--}
```
public abstract boolean getOnlyBestResults()
```


Mendapatkan nilai yang menunjukkan apakah hanya hasil terbaik yang akan dikembalikan. Nilai default adalah  false .


**Returns:**
boolean -  true  jika hanya hasil terbaik yang akan dikembalikan; jika tidak  false .

### setOnlyBestResults(boolean value) {#setOnlyBestResults-boolean-}
```
public abstract void setOnlyBestResults(boolean value)
```


Mengatur nilai yang menunjukkan apakah hanya hasil terbaik yang akan dikembalikan. Nilai default adalah  false .


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | boolean | true  jika hanya hasil terbaik yang akan dikembalikan; jika tidak  false . |
|

### getOnlyBestResultsRange() {#getOnlyBestResultsRange--}
```
public abstract byte getOnlyBestResultsRange()
```


Mendapatkan kelebihan maksimum dari jumlah minimum kesalahan yang ditemukan. Nilai default adalah  0 .


**Returns:**
byte - Kelebihan maksimum dari jumlah minimum kesalahan yang ditemukan.

### setOnlyBestResultsRange(byte value) {#setOnlyBestResultsRange-byte-}
```
public abstract void setOnlyBestResultsRange(byte value)
```


Mengatur kelebihan maksimum dari jumlah minimum kesalahan yang ditemukan. Nilai default adalah  0 .


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | byte | Kelebihan maksimum dari jumlah minimum kesalahan yang ditemukan. |
|

### getConsiderTranspositions() {#getConsiderTranspositions--}
```
public abstract boolean getConsiderTranspositions()
```


Mengambil nilai yang menunjukkan apakah algoritma pencarian fuzzy harus mempertimbangkan pertukaran dua karakter berdekatan sebagai satu kesalahan. Nilai default adalah true.


**Returns:**
boolean - true jika algoritma pencarian fuzzy mempertimbangkan pertukaran; jika tidak false.

### setConsiderTranspositions(boolean value) {#setConsiderTranspositions-boolean-}
```
public abstract void setConsiderTranspositions(boolean value)
```


Mengatur nilai yang menunjukkan apakah algoritma pencarian fuzzy harus mempertimbangkan pertukaran dua karakter berdekatan sebagai satu kesalahan. Nilai default adalah true.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | boolean | : true jika algoritma pencarian fuzzy mempertimbangkan pertukaran; jika tidak false. |
|

