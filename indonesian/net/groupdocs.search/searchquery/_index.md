---
title: "SearchQuery"
second_title: "Referensi API GroupDocs.Search untuk .NET"
description: "Mewakili kueri pencarian dalam bentuk objek."
type: docs
weight: 1580
url: /id/net/groupdocs.search/searchquery/
---
## SearchQuery class

Mewakili kueri pencarian dalam bentuk objek.

```csharp
public abstract class SearchQuery
```

## Properti

| Nama | Deskripsi |
| --- | --- |
| virtual [ChildCount](../../groupdocs.search/searchquery/childcount) { get; } | Mendapatkan jumlah kueri anak. |
| virtual [FieldName](../../groupdocs.search/searchquery/fieldname) { get; } | Mendapatkan nama bidang. |
| virtual [FirstChild](../../groupdocs.search/searchquery/firstchild) { get; } | Mendapatkan kueri anak pertama. |
| [SearchOptions](../../groupdocs.search/searchquery/searchoptions) { get; set; } | Mendapatkan atau mengatur opsi pencarian kueri ini. |
| virtual [SecondChild](../../groupdocs.search/searchquery/secondchild) { get; } | Mendapatkan kueri anak kedua. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| static [CreateAndQuery](../../groupdocs.search/searchquery/createandquery#createandquery_1)(params SearchQuery[]) | Membuat kueri gabungan yang hanya akan menemukan dokumen yang akan ditemukan untuk setiap kueri asli. |
| static [CreateAndQuery](../../groupdocs.search/searchquery/createandquery#createandquery)(SearchQuery, SearchQuery) | Membuat kueri gabungan yang hanya akan menemukan dokumen yang akan ditemukan untuk setiap kueri asli. |
| static [CreateDateRangeQuery](../../groupdocs.search/searchquery/createdaterangequery)(DateTime, DateTime) | Membuat kueri rentang tanggal. |
| static [CreateFieldQuery](../../groupdocs.search/searchquery/createfieldquery)(string, SearchQuery) | Menambahkan bidang ke kueri yang ditentukan. |
| static [CreateNotQuery](../../groupdocs.search/searchquery/createnotquery)(SearchQuery) | Membuat kueri terbalik yang akan menemukan dokumen lain dalam indeks dibandingkan dengan yang akan ditemukan oleh kueri asli. |
| static [CreateNumericRangeQuery](../../groupdocs.search/searchquery/createnumericrangequery)(long, long) | Membuat kueri rentang numerik. |
| static [CreateOrQuery](../../groupdocs.search/searchquery/createorquery#createorquery_1)(params SearchQuery[]) | Membuat kueri gabungan yang akan menemukan semua dokumen yang akan ditemukan setidaknya oleh salah satu kueri asli. |
| static [CreateOrQuery](../../groupdocs.search/searchquery/createorquery#createorquery)(SearchQuery, SearchQuery) | Membuat kueri gabungan yang akan menemukan semua dokumen yang akan ditemukan setidaknya oleh salah satu kueri asli. |
| static [CreatePhraseSearchQuery](../../groupdocs.search/searchquery/createphrasesearchquery)(params SearchQuery[]) | Membuat kueri pencarian frasa. |
| static [CreateRegexQuery](../../groupdocs.search/searchquery/createregexquery#createregexquery)(string) | Membuat kueri ekspresi reguler. |
| static [CreateRegexQuery](../../groupdocs.search/searchquery/createregexquery#createregexquery_1)(string, RegexOptions) | Membuat kueri ekspresi reguler. |
| static [CreateWildcardQuery](../../groupdocs.search/searchquery/createwildcardquery#createwildcardquery)(int) | Membuat wildcard untuk pencarian frasa. |
| static [CreateWildcardQuery](../../groupdocs.search/searchquery/createwildcardquery#createwildcardquery_1)(int, int) | Membuat wildcard untuk pencarian frasa. |
| static [CreateWordPatternQuery](../../groupdocs.search/searchquery/createwordpatternquery)(WordPattern) | Membuat kueri pola kata. |
| static [CreateWordQuery](../../groupdocs.search/searchquery/createwordquery)(string) | Membuat kueri kata sederhana. |
| abstract [GetChild](../../groupdocs.search/searchquery/getchild)(int) | Mendapatkan kueri anak berdasarkan indeks. |
| abstract [ToString](../../groupdocs.search/searchquery/tostring)() | Mengembalikan sebuah String yang mewakili instance [`SearchQuery`](../searchquery) saat ini. |

### Catatan

**Learn more**

* [Searching](https://docs.groupdocs.com/display/searchnet/Searching)
* [Queries in text and object form](https://docs.groupdocs.com/display/searchnet/Queries+in+text+and+object+form)
* [Nesting search queries in object form](https://docs.groupdocs.com/display/searchnet/Nesting+search+queries+in+object+form)

### Contoh

Contoh ini menunjukkan penggunaan tipikal dari kelas tersebut.

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

* namespace [GroupDocs.Search](../../groupdocs.search)
* assembly [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->
