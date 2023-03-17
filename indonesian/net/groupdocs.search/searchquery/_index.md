---
title: SearchQuery
second_title: GroupDocs.Mencari Referensi .NET API
description: Mewakili permintaan pencarian dalam bentuk objek.
type: docs
weight: 1240
url: /id/net/groupdocs.search/searchquery/
---
## SearchQuery class

Mewakili permintaan pencarian dalam bentuk objek.

```csharp
public abstract class SearchQuery
```

## Properti

| Nama | Keterangan |
| --- | --- |
| virtual [ChildCount](../../groupdocs.search/searchquery/childcount) { get; } | Mendapat jumlah kueri turunan. |
| virtual [FieldName](../../groupdocs.search/searchquery/fieldname) { get; } | Mendapatkan nama bidang. |
| virtual [FirstChild](../../groupdocs.search/searchquery/firstchild) { get; } | Mendapat kueri anak pertama. |
| [SearchOptions](../../groupdocs.search/searchquery/searchoptions) { get; set; } | Mendapat atau menyetel opsi pencarian dari kueri penelusuran ini. |
| virtual [SecondChild](../../groupdocs.search/searchquery/secondchild) { get; } | Mendapat kueri anak kedua. |

## Metode

| Nama | Keterangan |
| --- | --- |
| static [CreateAndQuery](../../groupdocs.search/searchquery/createandquery)(SearchQuery, SearchQuery) | Membuat kueri gabungan yang hanya akan menemukan dokumen yang akan ditemukan untuk setiap kueri asli. |
| static [CreateDateRangeQuery](../../groupdocs.search/searchquery/createdaterangequery)(DateTime, DateTime) | Membuat kueri rentang tanggal. |
| static [CreateFieldQuery](../../groupdocs.search/searchquery/createfieldquery)(string, SearchQuery) | Menambahkan bidang ke kueri yang ditentukan. |
| static [CreateNotQuery](../../groupdocs.search/searchquery/createnotquery)(SearchQuery) | Membuat kueri terbalik yang akan menemukan dokumen lainnya dalam indeks terhadap yang akan ditemukan untuk kueri asli. |
| static [CreateNumericRangeQuery](../../groupdocs.search/searchquery/createnumericrangequery)(long, long) | Membuat kueri rentang numerik. |
| static [CreateOrQuery](../../groupdocs.search/searchquery/createorquery)(SearchQuery, SearchQuery) | Membuat kueri gabungan yang akan menemukan semua dokumen yang akan ditemukan setidaknya untuk salah satu kueri asli. |
| static [CreatePhraseSearchQuery](../../groupdocs.search/searchquery/createphrasesearchquery)(params SearchQuery[]) | Membuat kueri penelusuran frasa. |
| static [CreateRegexQuery](../../groupdocs.search/searchquery/createregexquery#createregexquery)(string) | Membuat kueri ekspresi reguler. |
| static [CreateRegexQuery](../../groupdocs.search/searchquery/createregexquery#createregexquery_1)(string, RegexOptions) | Membuat kueri ekspresi reguler. |
| static [CreateWildcardQuery](../../groupdocs.search/searchquery/createwildcardquery#createwildcardquery)(int) | Membuat wildcard untuk pencarian frase. |
| static [CreateWildcardQuery](../../groupdocs.search/searchquery/createwildcardquery#createwildcardquery_1)(int, int) | Membuat wildcard untuk pencarian frase. |
| static [CreateWordPatternQuery](../../groupdocs.search/searchquery/createwordpatternquery)(WordPattern) | Membuat kueri pola kata. |
| static [CreateWordQuery](../../groupdocs.search/searchquery/createwordquery)(string) | Membuat kueri kata sederhana. |
| abstract [GetChild](../../groupdocs.search/searchquery/getchild)(int) | Mendapat kueri turunan berdasarkan indeks. |
| abstract [ToString](../../groupdocs.search/searchquery/tostring)() | Mengembalikan aString yang mewakili arus[`SearchQuery`](../searchquery) contoh. |

### Perkataan

**Belajarlah lagi**

* [Mencari](https://docs.groupdocs.com/display/searchnet/Searching)
* [Query dalam bentuk teks dan objek](https://docs.groupdocs.com/display/searchnet/Queries+in+text+and+object+form)
* [Permintaan pencarian bersarang dalam bentuk objek](https://docs.groupdocs.com/display/searchnet/Nesting+search+queries+in+object+form)

### Contoh

Contoh ini menunjukkan penggunaan umum kelas.

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

* ruang nama [GroupDocs.Search](../../groupdocs.search)
* perakitan [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
