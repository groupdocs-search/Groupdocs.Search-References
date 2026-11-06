---
title: "SearchQuery"
second_title: "GroupDocs.Search için .NET API Referansı"
description: "Arama sorgusunu nesne biçiminde temsil eder."
type: docs
weight: 1580
url: /tr/net/groupdocs.search/searchquery/
---
## SearchQuery class

Arama sorgusunu nesne biçiminde temsil eder.

```csharp
public abstract class SearchQuery
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| virtual [ChildCount](../../groupdocs.search/searchquery/childcount) { get; } | Alt sorguların sayısını alır. |
| virtual [FieldName](../../groupdocs.search/searchquery/fieldname) { get; } | Alan adını alır. |
| virtual [FirstChild](../../groupdocs.search/searchquery/firstchild) { get; } | İlk alt sorguyu alır. |
| [SearchOptions](../../groupdocs.search/searchquery/searchoptions) { get; set; } | Bu arama sorgusunun arama seçeneklerini alır veya ayarlar. |
| virtual [SecondChild](../../groupdocs.search/searchquery/secondchild) { get; } | İkinci alt sorguyu alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| static [CreateAndQuery](../../groupdocs.search/searchquery/createandquery#createandquery_1)(params SearchQuery[]) | Her orijinal sorgu için bulunacak belgeleri yalnızca bulacak bir birleşik sorgu oluşturur. |
| static [CreateAndQuery](../../groupdocs.search/searchquery/createandquery#createandquery)(SearchQuery, SearchQuery) | Her orijinal sorgu için bulunacak belgeleri yalnızca bulacak bir birleşik sorgu oluşturur. |
| static [CreateDateRangeQuery](../../groupdocs.search/searchquery/createdaterangequery)(DateTime, DateTime) | Bir tarih aralığı sorgusu oluşturur. |
| static [CreateFieldQuery](../../groupdocs.search/searchquery/createfieldquery)(string, SearchQuery) | Belirtilen sorguya bir alan ekler. |
| static [CreateNotQuery](../../groupdocs.search/searchquery/createnotquery)(SearchQuery) | Orijinal sorgu için bulunacak belgelerin dışında indeksdeki kalan belgeleri bulacak ters bir sorgu oluşturur. |
| static [CreateNumericRangeQuery](../../groupdocs.search/searchquery/createnumericrangequery)(long, long) | Sayısal aralık sorgusu oluşturur. |
| static [CreateOrQuery](../../groupdocs.search/searchquery/createorquery#createorquery_1)(params SearchQuery[]) | Orijinal sorgulardan en az birinde bulunacak tüm belgeleri bulacak birleşik bir sorgu oluşturur. |
| static [CreateOrQuery](../../groupdocs.search/searchquery/createorquery#createorquery)(SearchQuery, SearchQuery) | Orijinal sorgulardan en az birinde bulunacak tüm belgeleri bulacak birleşik bir sorgu oluşturur. |
| static [CreatePhraseSearchQuery](../../groupdocs.search/searchquery/createphrasesearchquery)(params SearchQuery[]) | İfade arama sorgusu oluşturur. |
| static [CreateRegexQuery](../../groupdocs.search/searchquery/createregexquery#createregexquery)(string) | Düzenli ifade sorgusu oluşturur. |
| static [CreateRegexQuery](../../groupdocs.search/searchquery/createregexquery#createregexquery_1)(string, RegexOptions) | Düzenli ifade sorgusu oluşturur. |
| static [CreateWildcardQuery](../../groupdocs.search/searchquery/createwildcardquery#createwildcardquery)(int) | İfade araması için bir joker karakter oluşturur. |
| static [CreateWildcardQuery](../../groupdocs.search/searchquery/createwildcardquery#createwildcardquery_1)(int, int) | İfade araması için bir joker karakter oluşturur. |
| static [CreateWordPatternQuery](../../groupdocs.search/searchquery/createwordpatternquery)(WordPattern) | Kelime deseni sorgusu oluşturur. |
| static [CreateWordQuery](../../groupdocs.search/searchquery/createwordquery)(string) | Basit kelime sorgusu oluşturur. |
| abstract [GetChild](../../groupdocs.search/searchquery/getchild)(int) | Bir indeksle alt sorgu alır. |
| abstract [ToString](../../groupdocs.search/searchquery/tostring)() | Geçerli [`SearchQuery`](../searchquery) örneğini temsil eden bir String döndürür. |

### Açıklamalar

**Learn more**

* [Searching](https://docs.groupdocs.com/display/searchnet/Searching)
* [Queries in text and object form](https://docs.groupdocs.com/display/searchnet/Queries+in+text+and+object+form)
* [Nesting search queries in object form](https://docs.groupdocs.com/display/searchnet/Nesting+search+queries+in+object+form)

### Örnekler

Bu örnek, sınıfın tipik bir kullanımını gösterir.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

// Tarih aralığı aramasının alt sorgusunu oluşturma
SearchQuery subquery1 = SearchQuery.CreateDateRangeQuery(new DateTime(2011, 6, 17), new DateTime(2013, 1, 1));

// 0 ile 2 arasında kaçırılan kelime sayısıyla joker karakterin alt sorgusunu oluşturma
SearchQuery subquery2 = SearchQuery.CreateWildcardQuery(0, 2);

// Basit kelimenin alt sorgusunu oluşturma
SearchQuery subquery3 = SearchQuery.CreateWordQuery("birth");
subquery3.SearchOptions = new SearchOptions(); // Setting search options only for subquery 3
subquery3.SearchOptions.FuzzySearch.Enabled = true;
subquery3.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1);

// Alt sorguları tek bir sorguya birleştirme
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

// Bulunan oluşumların artırılmış kapasitesine sahip arama seçenekleri nesnesi oluşturma
SearchOptions options = new SearchOptions(); // Overall search options
options.MaxOccurrenceCountPerTerm = 1000000;
options.MaxTotalOccurrenceCount = 10000000;

SearchResult result = index.Search(query, options); // Searching
```

### Ayrıca Bakınız

* namespace [GroupDocs.Search](../../groupdocs.search)
* assembly [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->
