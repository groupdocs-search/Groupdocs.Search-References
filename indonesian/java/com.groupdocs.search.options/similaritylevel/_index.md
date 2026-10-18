---
title: "SimilarityLevel"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili algoritma pencarian fuzzy yang menentukan tingkat kemiripan."
type: docs
weight: 35
url: /id/java/com.groupdocs.search.options/similaritylevel/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.options.FuzzyAlgorithm](../../com.groupdocs.search.options/fuzzyalgorithm)
```
public class SimilarityLevel extends FuzzyAlgorithm
```

Mewakili algoritma pencarian fuzzy yang menentukan tingkat kemiripan. Algoritma tingkat kemiripan menghitung jumlah maksimum kesalahan untuk sebuah kata secara berbanding terbalik dengan panjang kata.


**Learn more**

* [Fuzzy search](../https://docs.groupdocs.com/display/searchjava/Fuzzy+search)


Contoh ini menunjukkan penggunaan tipikal kelas tersebut.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Membuat indeks di folder yang ditentukan
index.add(documentsFolder); // Mengindeks dokumen dari folder yang ditentukan
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // Mengaktifkan pencarian fuzzy
options.getFuzzySearch().setFuzzyAlgorithm(new SimilarityLevel(0.8)); // Membuat algoritma pencarian fuzzy
// Fungsi ini menentukan 0 sebagai jumlah maksimum kesalahan untuk kata dengan panjang 1 hingga 4 karakter.
// Ini menentukan 1 sebagai jumlah maksimum kesalahan untuk kata dengan panjang 5 hingga 9 karakter.
// Ini menentukan 2 sebagai jumlah maksimum kesalahan untuk kata dengan panjang 10 hingga 14 karakter. Dan seterusnya.
SearchResult result = index.search(query, options); // Cari di indeks
 
```
 
````


## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [SimilarityLevel(double value)](#SimilarityLevel-double-) | Menginisialisasi instance baru dari kelas  SimilarityLevel . |
|
|  | [SimilarityLevel(Object data)](#SimilarityLevel-java.lang.Object-) | Menginisialisasi instance baru dari kelas  SimilarityLevel . |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getSimilarityLevel(int termLength)](#getSimilarityLevel-int-) | Mendapatkan nilai tingkat kemiripan untuk panjang istilah yang ditentukan. |
|
|  | [getMaxMistakeCount(int termLength)](#getMaxMistakeCount-int-) | Mendapatkan jumlah maksimum kesalahan yang diizinkan untuk panjang istilah yang ditentukan. |
|
### SimilarityLevel(double value) {#SimilarityLevel-double-}
```
public SimilarityLevel(double value)
```


Menginisialisasi instance baru dari kelas  SimilarityLevel .


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | double | Nilai tingkat kemiripan. |
|

### SimilarityLevel(Object data) {#SimilarityLevel-java.lang.Object-}
```
public SimilarityLevel(Object data)
```


Menginisialisasi instance baru dari kelas  SimilarityLevel .


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | data | java.lang.Object | Data yang diserialkan. |
|

### getSimilarityLevel(int termLength) {#getSimilarityLevel-int-}
```
public double getSimilarityLevel(int termLength)
```


Mendapatkan nilai tingkat kemiripan untuk panjang istilah yang ditentukan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | termLength | int | Panjang istilah. |
|

**Returns:**
double - Nilai tingkat kemiripan.

### getMaxMistakeCount(int termLength) {#getMaxMistakeCount-int-}
```
public int getMaxMistakeCount(int termLength)
```


Mendapatkan jumlah maksimum kesalahan yang diizinkan untuk panjang istilah yang ditentukan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | termLength | int | Panjang istilah. |
|

**Returns:**
int - Jumlah kesalahan maksimum yang diizinkan.

