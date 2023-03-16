---
title: SimilarityLevel
second_title: GroupDocs.Mencari Referensi .NET API
description: Mewakili algoritma pencarian fuzzy yang menentukan tingkat kesamaan. Algoritma tingkat kesamaan menghitung jumlah kesalahan maksimum untuk sebuah kata berbanding terbalik dengan panjang kata.
type: docs
weight: 1050
url: /id/net/groupdocs.search.options/similaritylevel/
---
## SimilarityLevel class

Mewakili algoritma pencarian fuzzy yang menentukan tingkat kesamaan. Algoritma tingkat kesamaan menghitung jumlah kesalahan maksimum untuk sebuah kata berbanding terbalik dengan panjang kata.

```csharp
public class SimilarityLevel : FuzzyAlgorithm
```

## Konstruktor

| Nama | Keterangan |
| --- | --- |
| [SimilarityLevel](similaritylevel)(double) | Menginisialisasi instance baru dari[`SimilarityLevel`](../similaritylevel) kelas. |

## Metode

| Nama | Keterangan |
| --- | --- |
| override [GetMaxMistakeCount](../../groupdocs.search.options/similaritylevel/getmaxmistakecount)(int) | Mendapat jumlah kesalahan maksimum yang diperbolehkan untuk jangka waktu yang ditentukan. |
| override [GetSimilarityLevel](../../groupdocs.search.options/similaritylevel/getsimilaritylevel)(int) | Mendapat nilai tingkat kemiripan untuk panjang istilah yang ditentukan. |

### Perkataan

**Belajarlah lagi**

* [Pencarian kabur](https://docs.groupdocs.com/display/searchnet/Fuzzy+search)

### Contoh

Contoh ini menunjukkan penggunaan umum kelas.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // Membuat indeks di folder yang ditentukan
index.Add(documentsFolder); // Pengindeksan dokumen dari folder yang ditentukan

SearchOptions options = new SearchOptions();
options.FuzzySearch.Enabled = true; // Mengaktifkan pencarian kabur
options.FuzzySearch.FuzzyAlgorithm = new SimilarityLevel(0.8); // Membuat algoritma pencarian fuzzy
// Fungsi ini menetapkan 0 sebagai jumlah kesalahan maksimum untuk kata dari 1 hingga 4 karakter.
// Ini menentukan 1 sebagai jumlah kesalahan maksimum untuk kata-kata dari 5 hingga 9 karakter.
// Ini menentukan 2 sebagai jumlah kesalahan maksimum untuk kata-kata dari 10 hingga 14 karakter. Dan seterusnya.

SearchResult result = index.Search(query, options); // Cari di index
```

### Lihat juga

* class [FuzzyAlgorithm](../fuzzyalgorithm)
* ruang nama [GroupDocs.Search.Options](../../groupdocs.search.options)
* perakitan [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->