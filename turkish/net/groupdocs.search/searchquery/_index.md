---
title: SearchQuery
second_title: .NET API Başvurusu için GroupDocs.Search
description: Nesne biçimindeki bir arama sorgusunu temsil eder.
type: docs
weight: 1240
url: /tr/net/groupdocs.search/searchquery/
---
## SearchQuery class

Nesne biçimindeki bir arama sorgusunu temsil eder.

```csharp
public abstract class SearchQuery
```

## Özellikleri

| İsim | Tanım |
| --- | --- |
| virtual [ChildCount](../../groupdocs.search/searchquery/childcount) { get; } | Alt sorguların sayısını alır. |
| virtual [FieldName](../../groupdocs.search/searchquery/fieldname) { get; } | Alan adını alır. |
| virtual [FirstChild](../../groupdocs.search/searchquery/firstchild) { get; } | İlk alt sorguyu alır. |
| [SearchOptions](../../groupdocs.search/searchquery/searchoptions) { get; set; } | Bu arama sorgusunun arama seçeneklerini alır veya ayarlar. |
| virtual [SecondChild](../../groupdocs.search/searchquery/secondchild) { get; } | İkinci alt sorguyu alır. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| static [CreateAndQuery](../../groupdocs.search/searchquery/createandquery)(SearchQuery, SearchQuery) | Yalnızca her orijinal sorgu için bulunabilecek belgeleri bulan birleşik bir sorgu oluşturur. |
| static [CreateDateRangeQuery](../../groupdocs.search/searchquery/createdaterangequery)(DateTime, DateTime) | Bir tarih aralığı sorgusu oluşturur. |
| static [CreateFieldQuery](../../groupdocs.search/searchquery/createfieldquery)(string, SearchQuery) | Belirtilen sorguya bir alan ekler. |
| static [CreateNotQuery](../../groupdocs.search/searchquery/createnotquery)(SearchQuery) | Orijinal sorgu için bulunacak olanlara karşı bir dizindeki geri kalan belgeleri bulan tersine çevrilmiş bir sorgu oluşturur. |
| static [CreateNumericRangeQuery](../../groupdocs.search/searchquery/createnumericrangequery)(long, long) | Sayısal bir aralık sorgusu oluşturur. |
| static [CreateOrQuery](../../groupdocs.search/searchquery/createorquery)(SearchQuery, SearchQuery) | Orijinal sorgulardan en az biri için bulunacak tüm belgeleri bulan birleşik bir sorgu oluşturur. |
| static [CreatePhraseSearchQuery](../../groupdocs.search/searchquery/createphrasesearchquery)(params SearchQuery[]) | Bir ifade arama sorgusu oluşturur. |
| static [CreateRegexQuery](../../groupdocs.search/searchquery/createregexquery#createregexquery)(string) | Düzenli ifade sorgusu oluşturur. |
| static [CreateRegexQuery](../../groupdocs.search/searchquery/createregexquery#createregexquery_1)(string, RegexOptions) | Düzenli ifade sorgusu oluşturur. |
| static [CreateWildcardQuery](../../groupdocs.search/searchquery/createwildcardquery#createwildcardquery)(int) | İfade araması için bir joker karakter oluşturur. |
| static [CreateWildcardQuery](../../groupdocs.search/searchquery/createwildcardquery#createwildcardquery_1)(int, int) | İfade araması için bir joker karakter oluşturur. |
| static [CreateWordPatternQuery](../../groupdocs.search/searchquery/createwordpatternquery)(WordPattern) | Bir sözcük kalıbı sorgusu oluşturur. |
| static [CreateWordQuery](../../groupdocs.search/searchquery/createwordquery)(string) | Basit bir sözcük sorgusu oluşturur. |
| abstract [GetChild](../../groupdocs.search/searchquery/getchild)(int) | Bir dizine göre bir alt sorgu alır. |
| abstract [ToString](../../groupdocs.search/searchquery/tostring)() | a döndürürString akımı temsil eden[`SearchQuery`](../searchquery) örnek. |

### Notlar

**Daha fazla bilgi edin**

* [Aranıyor](https://docs.groupdocs.com/display/searchnet/Searching)
* [Metin ve nesne biçiminde sorgular](https://docs.groupdocs.com/display/searchnet/Queries+in+text+and+object+form)
* [Arama sorgularını nesne biçiminde iç içe yerleştirme](https://docs.groupdocs.com/display/searchnet/Nesting+search+queries+in+object+form)

### Örnekler

Örnek, sınıfın tipik bir kullanımını göstermektedir.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); //Belirtilen klasörde indeks oluşturma
index.Add(documentsFolder); // Belgeleri belirtilen klasörden indeksleme

// Tarih aralığı araması için alt sorgu oluşturma
SearchQuery subquery1 = SearchQuery.CreateDateRangeQuery(new DateTime(2011, 6, 17), new DateTime(2013, 1, 1));

// 0'dan 2'ye kadar kaçırılan kelime sayısına sahip joker alt sorgu oluşturma
SearchQuery subquery2 = SearchQuery.CreateWildcardQuery(0, 2);

// Basit bir kelimenin alt sorgusu oluşturuluyor
SearchQuery subquery3 = SearchQuery.CreateWordQuery("birth");
subquery3.SearchOptions = new SearchOptions(); // Arama seçeneklerini yalnızca alt sorgu 3 için ayarlama
subquery3.SearchOptions.FuzzySearch.Enabled = true;
subquery3.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1);

// Alt sorguları tek bir sorguda birleştirme
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

// Bulunan oluşumların kapasitesi artırılmış arama seçenekleri nesnesi oluşturuluyor
SearchOptions options = new SearchOptions(); // Genel arama seçenekleri
options.MaxOccurrenceCountPerTerm = 1000000;
options.MaxTotalOccurrenceCount = 10000000;

SearchResult result = index.Search(query, options); // Aranıyor
```

### Ayrıca bakınız

* ad alanı [GroupDocs.Search](../../groupdocs.search)
* toplantı [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
