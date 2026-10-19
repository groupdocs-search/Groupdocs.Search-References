---
title: "Cari"
second_title: "Referensi API GroupDocs.Search untuk .NET"
description: "Mencari dalam indeks."
type: docs
weight: 260
url: /id/net/groupdocs.search/index/search/
---
## Search(string) {#search_3}

Mencari dalam indeks.

```csharp
public SearchResult Search(string query)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| kueri | String | Kueri pencarian. |

### Nilai Kembali

Hasil pencarian.

### Contoh

Contoh berikut menunjukkan cara melakukan pencarian sederhana.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

SearchResult result = index.Search(query); // Searching
```

Contoh berikut menunjukkan cara melakukan pencarian Regex.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

string query = "^[0-9]{3,}"; // The caret symbol at the beginning of the search query tells the index that it is a Regex query
SearchResult result = index.Search(query); // Searching
```

Contoh berikut menunjukkan cara melakukan pencarian berfaset.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

string query = "content:Newton"; // The word before the colon in the query means the document field name to search
SearchResult result = index.Search(query); // Searching
```

### Lihat Juga

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(string, SearchOptions) {#search_4}

Mencari dalam indeks.

```csharp
public SearchResult Search(string query, SearchOptions options)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| kueri | String | Kueri pencarian. |
| opsi | SearchOptions | Opsi pencarian. |

### Nilai Kembali

Hasil pencarian.

### Contoh

Contoh berikut menunjukkan cara melakukan pencarian fuzzy.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

SearchOptions options = new SearchOptions();
options.FuzzySearch.Enabled = true; // Enabling the fuzzy search
options.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1); // Setting the number of possible differences for each word

// Kutip ganda di awal dan akhir memberi tahu indeks bahwa itu adalah kueri pencarian frasa
string query = "\"The Pursuit of Happiness\"";
SearchResult result = index.Search(query, options); // Searching
```

Contoh berikut menunjukkan cara melakukan pencarian sinonim.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

SearchOptions options = new SearchOptions();
options.UseSynonymSearch = true; // Enabling the synonym search

string query = "cry";
SearchResult result = index.Search(query, options); // Searching
```

### Lihat Juga

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(SearchQuery) {#search_1}

Mencari dalam indeks.

```csharp
public SearchResult Search(SearchQuery query)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| kueri | SearchQuery | Kueri pencarian. |

### Nilai Kembali

Hasil pencarian.

### Contoh

Contoh berikut menunjukkan cara melakukan pencarian menggunakan kueri dalam bentuk objek.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

// Membuat subkueri 1
SearchQuery subquery1 = SearchQuery.CreateWordQuery("accommodation");
subquery1.SearchOptions = new SearchOptions(); // Setting search options only for subquery 1
subquery1.SearchOptions.FuzzySearch.Enabled = true; // Enabling the fuzzy search
subquery1.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(3); // Setting maximum number of differences

// Membuat subkueri 2
SearchQuery subquery2 = SearchQuery.CreateNumericRangeQuery(1, 1000000);

// Membuat subkueri 3
SearchQuery subquery3 = SearchQuery.CreateRegexQuery(@"(.)\1");

// Menggabungkan subkueri menjadi satu kueri
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

SearchResult result = index.Search(query); // Searching
```

### Lihat Juga

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(SearchQuery, SearchOptions) {#search_2}

Mencari dalam indeks.

```csharp
public SearchResult Search(SearchQuery query, SearchOptions options)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| kueri | SearchQuery | Kueri pencarian. |
| opsi | SearchOptions | Opsi pencarian. |

### Nilai Kembali

Hasil pencarian.

### Contoh

Contoh berikut menunjukkan cara melakukan pencarian menggunakan kueri dalam bentuk objek.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

// Membuat subkueri pencarian rentang tanggal
SearchQuery subquery1 = SearchQuery.CreateDateRangeQuery(new DateTime(2011, 6, 17), new DateTime(2013, 1, 1));

// Membuat subkueri wildcard dengan jumlah kata yang terlewat dari 0 hingga 2
SearchQuery subquery2 = SearchQuery.CreateWildcardQuery(0, 2);

// Membuat subkueri kata sederhana
SearchQuery subquery3 = SearchQuery.CreateWordQuery("birth");
subquery3.SearchOptions = new SearchOptions(); // Setting search options only for subquery 3
subquery3.SearchOptions.FuzzySearch.Enabled = true;
subquery3.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1);

// Menggabungkan subkueri menjadi satu kueri
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

// Membuat objek opsi pencarian dengan kapasitas peningkatan untuk temuan yang ditemukan
SearchOptions options = new SearchOptions(); // Overall search options
options.MaxOccurrenceCountPerTerm = 1000000;
options.MaxTotalOccurrenceCount = 10000000;

SearchResult result = index.Search(query, options); // Searching
```

### Lihat Juga

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(SearchImage, ImageSearchOptions) {#search}

Melakukan pencarian gambar terbalik dalam indeks.

```csharp
public ImageSearchResult Search(SearchImage image, ImageSearchOptions options)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| gambar | SearchImage | Gambar untuk pencarian. |
| opsi | ImageSearchOptions | Opsi pencarian gambar. |

### Nilai Kembali

Hasil pencarian gambar terbalik.

### Lihat Juga

* class [ImageSearchResult](../../../groupdocs.search.results/imagesearchresult)
* class [SearchImage](../../../groupdocs.search.common/searchimage)
* class [ImageSearchOptions](../../../groupdocs.search.options/imagesearchoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->
