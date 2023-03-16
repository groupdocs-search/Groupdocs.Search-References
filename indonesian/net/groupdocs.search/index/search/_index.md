---
title: Search
second_title: GroupDocs.Mencari Referensi .NET API
description: Mencari di index.
type: docs
weight: 220
url: /id/net/groupdocs.search/index/search/
---
## Search(string) {#search_3}

Mencari di index.

```csharp
public SearchResult Search(string query)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| query | String | Permintaan pencarian. |

### Nilai Pengembalian

Hasil pencarian.

### Contoh

Contoh berikut menunjukkan cara melakukan pencarian sederhana.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // Membuat indeks di folder yang ditentukan
index.Add(documentsFolder); // Pengindeksan dokumen dari folder yang ditentukan

SearchResult result = index.Search(query); // Mencari
```

Contoh berikut menunjukkan cara melakukan pencarian Regex.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Membuat indeks di folder yang ditentukan
index.Add(documentsFolder); // Pengindeksan dokumen dari folder yang ditentukan

string query = "^[0-9]{3,}"; // Simbol tanda sisipan di awal kueri penelusuran memberi tahu indeks bahwa ini adalah kueri Regex
SearchResult result = index.Search(query); // Mencari
```

Contoh berikut menunjukkan cara melakukan pencarian segi.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Membuat indeks di folder yang ditentukan
index.Add(documentsFolder); // Pengindeksan dokumen dari folder yang ditentukan

string query = "content:Newton"; // Kata sebelum titik dua dalam kueri berarti nama bidang dokumen yang akan dicari
SearchResult result = index.Search(query); // Mencari
```

### Lihat juga

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [Index](../../index)
* ruang nama [GroupDocs.Search](../../index)
* perakitan [GroupDocs.Search](../../../)

---

## Search(string, SearchOptions) {#search_4}

Mencari di index.

```csharp
public SearchResult Search(string query, SearchOptions options)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| query | String | Permintaan pencarian. |
| options | SearchOptions | Opsi pencarian. |

### Nilai Pengembalian

Hasil pencarian.

### Contoh

Contoh berikut menunjukkan cara melakukan pencarian fuzzy.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Membuat indeks di folder yang ditentukan
index.Add(documentsFolder); // Pengindeksan dokumen dari folder yang ditentukan

SearchOptions options = new SearchOptions();
options.FuzzySearch.Enabled = true; // Mengaktifkan pencarian kabur
options.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1); // Mengatur jumlah kemungkinan perbedaan untuk setiap kata

// Tanda kutip ganda di awal dan akhir memberi tahu indeks bahwa itu adalah permintaan pencarian frase
string query = "\"The Pursuit of Happiness\"";
SearchResult result = index.Search(query, options); // Mencari
```

Contoh berikut menunjukkan cara melakukan pencarian sinonim.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Membuat indeks di folder yang ditentukan
index.Add(documentsFolder); // Pengindeksan dokumen dari folder yang ditentukan

SearchOptions options = new SearchOptions();
options.UseSynonymSearch = true; // Mengaktifkan pencarian sinonim

string query = "cry";
SearchResult result = index.Search(query, options); // Mencari
```

### Lihat juga

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Index](../../index)
* ruang nama [GroupDocs.Search](../../index)
* perakitan [GroupDocs.Search](../../../)

---

## Search(SearchQuery) {#search_1}

Mencari di index.

```csharp
public SearchResult Search(SearchQuery query)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| query | SearchQuery | Permintaan pencarian. |

### Nilai Pengembalian

Hasil pencarian.

### Contoh

Contoh berikut menunjukkan cara melakukan pencarian menggunakan kueri dalam bentuk objek.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Membuat indeks di folder yang ditentukan
index.Add(documentsFolder); // Pengindeksan dokumen dari folder yang ditentukan

// Membuat subquery 1
SearchQuery subquery1 = SearchQuery.CreateWordQuery("accommodation");
subquery1.SearchOptions = new SearchOptions(); // Mengatur opsi pencarian hanya untuk subquery 1
subquery1.SearchOptions.FuzzySearch.Enabled = true; // Mengaktifkan pencarian kabur
subquery1.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(3); // Menetapkan jumlah maksimum perbedaan

// Membuat subquery 2
SearchQuery subquery2 = SearchQuery.CreateNumericRangeQuery(1, 1000000);

// Membuat subquery 3
SearchQuery subquery3 = SearchQuery.CreateRegexQuery(@"(.)\1");

// Menggabungkan subkueri menjadi satu kueri
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

SearchResult result = index.Search(query); // Mencari
```

### Lihat juga

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [Index](../../index)
* ruang nama [GroupDocs.Search](../../index)
* perakitan [GroupDocs.Search](../../../)

---

## Search(SearchQuery, SearchOptions) {#search_2}

Mencari di index.

```csharp
public SearchResult Search(SearchQuery query, SearchOptions options)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| query | SearchQuery | Permintaan pencarian. |
| options | SearchOptions | Opsi pencarian. |

### Nilai Pengembalian

Hasil pencarian.

### Contoh

Contoh berikut menunjukkan cara melakukan pencarian menggunakan kueri dalam bentuk objek.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Membuat indeks di folder yang ditentukan
index.Add(documentsFolder); // Pengindeksan dokumen dari folder yang ditentukan

// Membuat subkueri pencarian rentang tanggal
SearchQuery subquery1 = SearchQuery.CreateDateRangeQuery(new DateTime(2011, 6, 17), new DateTime(2013, 1, 1));

// Membuat subquery dari wildcard dengan jumlah kata yang terlewatkan dari 0 sampai 2
SearchQuery subquery2 = SearchQuery.CreateWildcardQuery(0, 2);

// Membuat subquery dari kata sederhana
SearchQuery subquery3 = SearchQuery.CreateWordQuery("birth");
subquery3.SearchOptions = new SearchOptions(); // Mengatur opsi pencarian hanya untuk subquery 3
subquery3.SearchOptions.FuzzySearch.Enabled = true;
subquery3.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1);

// Menggabungkan subkueri menjadi satu kueri
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

// Membuat objek opsi pencarian dengan peningkatan kapasitas kejadian yang ditemukan
SearchOptions options = new SearchOptions(); // Opsi pencarian keseluruhan
options.MaxOccurrenceCountPerTerm = 1000000;
options.MaxTotalOccurrenceCount = 10000000;

SearchResult result = index.Search(query, options); // Mencari
```

### Lihat juga

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Index](../../index)
* ruang nama [GroupDocs.Search](../../index)
* perakitan [GroupDocs.Search](../../../)

---

## Search(SearchImage, ImageSearchOptions) {#search}

Melakukan pencarian gambar terbalik di indeks.

```csharp
public ImageSearchResult Search(SearchImage image, ImageSearchOptions options)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| image | SearchImage | Gambar untuk dicari. |
| options | ImageSearchOptions | Opsi pencarian gambar. |

### Nilai Pengembalian

Hasil pencarian gambar terbalik.

### Lihat juga

* class [ImageSearchResult](../../../groupdocs.search.results/imagesearchresult)
* class [SearchImage](../../../groupdocs.search.common/searchimage)
* class [ImageSearchOptions](../../../groupdocs.search.options/imagesearchoptions)
* class [Index](../../index)
* ruang nama [GroupDocs.Search](../../index)
* perakitan [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
