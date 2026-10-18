---
title: "TableDiscreteFunction"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili algoritma pencarian fuzzy yang berisi korespondensi antara panjang kata dan jumlah kesalahan yang diizinkan."
type: docs
weight: 40
url: /id/java/com.groupdocs.search.options/tablediscretefunction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.options.FuzzyAlgorithm](../../com.groupdocs.search.options/fuzzyalgorithm)
```
public class TableDiscreteFunction extends FuzzyAlgorithm
```

Mewakili algoritma pencarian fuzzy yang berisi korespondensi antara panjang kata dan jumlah kesalahan yang diizinkan. Algoritma ini dapat ditentukan dengan tabel nilai keluaran atau dengan fungsi langkah.


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
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1, new Step(5, 2), new Step(8, 3))); // Membuat algoritma pencarian fuzzy
// Fungsi ini menentukan 1 sebagai jumlah maksimum kesalahan untuk kata dengan panjang 1 hingga 4 karakter.
// Menentukan 2 sebagai jumlah maksimum kesalahan untuk kata dengan panjang 5 hingga 7 karakter.
// Menentukan 3 sebagai jumlah maksimum kesalahan untuk kata dengan panjang 8 karakter ke atas.
SearchResult result = index.search(query, options); // Cari di indeks
 
```
 
````


## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [TableDiscreteFunction(int offsetOfInputs, int[] tableOfOutputs)](#TableDiscreteFunction-int-int---) | Menginisialisasi instance baru dari kelas  TableDiscreteFunction  . |
|
|  | [TableDiscreteFunction(int firstStepLevel, Step[] steps)](#TableDiscreteFunction-int-com.groupdocs.search.options.Step...-) | Menginisialisasi instance baru dari kelas  TableDiscreteFunction  . |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getSimilarityLevel(int termLength)](#getSimilarityLevel-int-) | Mendapatkan tingkat kemiripan untuk panjang istilah yang ditentukan. |
|
|  | [getMaxMistakeCount(int termLength)](#getMaxMistakeCount-int-) | Mendapatkan jumlah maksimum kesalahan yang diizinkan untuk panjang istilah yang ditentukan. |
|
### TableDiscreteFunction(int offsetOfInputs, int[] tableOfOutputs) {#TableDiscreteFunction-int-int---}
```
public TableDiscreteFunction(int offsetOfInputs, int[] tableOfOutputs)
```


Menginisialisasi instance baru dari kelas  TableDiscreteFunction  .


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | offsetOfInputs | int | Offset tabel indeks relatif terhadap nilai input. |
|
|  | tableOfOutputs | int[] | Tabel nilai keluaran. |
|

### TableDiscreteFunction(int firstStepLevel, Step[] steps) {#TableDiscreteFunction-int-com.groupdocs.search.options.Step...-}
```
public TableDiscreteFunction(int firstStepLevel, Step[] steps)
```


Menginisialisasi instance baru dari kelas  TableDiscreteFunction  .


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | firstStepLevel | int | Tingkat langkah pertama dari fungsi langkah. |
|
|  | steps | [Step\[\]](../../com.groupdocs.search.options/step) | Langkah selanjutnya dari fungsi langkah. |
|

### getSimilarityLevel(int termLength) {#getSimilarityLevel-int-}
```
public double getSimilarityLevel(int termLength)
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
public int getMaxMistakeCount(int termLength)
```


Mendapatkan jumlah maksimum kesalahan yang diizinkan untuk panjang istilah yang ditentukan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | termLength | int | Panjang istilah. |
|

**Returns:**
int - Jumlah maksimum kesalahan yang diizinkan.

