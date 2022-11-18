---
title: Search
second_title: .NET API Başvurusu için GroupDocs.Search
description: index. içinde arama yapar
type: docs
weight: 220
url: /tr/net/groupdocs.search/index/search/
---
## Search(string) {#search_3}

index. içinde arama yapar

```csharp
public SearchResult Search(string query)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| query | String | Arama sorgusu. |

### Geri dönüş değeri

Arama sonucu.

### Örnekler

Aşağıdaki örnek, basit aramanın nasıl gerçekleştirileceğini gösterir.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); //Belirtilen klasörde indeks oluşturma
index.Add(documentsFolder); // Belgeleri belirtilen klasörden indeksleme

SearchResult result = index.Search(query); // Aranıyor
```

Aşağıdaki örnek, normal ifade aramasının nasıl gerçekleştirileceğini gösterir.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); //Belirtilen klasörde indeks oluşturma
index.Add(documentsFolder); // Belgeleri belirtilen klasörden indeksleme

string query = "^[0-9]{3,}"; // Arama sorgusunun başındaki şapka simgesi, dizine bunun bir Regex sorgusu olduğunu söyler
SearchResult result = index.Search(query); // Aranıyor
```

Aşağıdaki örnek, çok yönlü aramanın nasıl gerçekleştirileceğini gösterir.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); //Belirtilen klasörde indeks oluşturma
index.Add(documentsFolder); // Belgeleri belirtilen klasörden indeksleme

string query = "content:Newton"; // Sorguda iki noktadan önceki kelime, aranacak belge alanı adı anlamına gelir
SearchResult result = index.Search(query); // Aranıyor
```

### Ayrıca bakınız

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [Index](../../index)
* ad alanı [GroupDocs.Search](../../index)
* toplantı [GroupDocs.Search](../../../)

---

## Search(string, SearchOptions) {#search_4}

index. içinde arama yapar

```csharp
public SearchResult Search(string query, SearchOptions options)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| query | String | Arama sorgusu. |
| options | SearchOptions | Arama seçenekleri. |

### Geri dönüş değeri

Arama sonucu.

### Örnekler

Aşağıdaki örnek bulanık aramanın nasıl gerçekleştirileceğini gösterir.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); //Belirtilen klasörde indeks oluşturma
index.Add(documentsFolder); // Belgeleri belirtilen klasörden indeksleme

SearchOptions options = new SearchOptions();
options.FuzzySearch.Enabled = true; // Bulanık aramayı etkinleştirme
options.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1); // Her kelime için olası farkların sayısını ayarlıyoruz

// Başında ve sonunda çift tırnak, dizine bunun öbek arama sorgusu olduğunu söyler
string query = "\"The Pursuit of Happiness\"";
SearchResult result = index.Search(query, options); // Aranıyor
```

Aşağıdaki örnek, eşanlamlı aramanın nasıl gerçekleştirileceğini gösterir.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); //Belirtilen klasörde indeks oluşturma
index.Add(documentsFolder); // Belgeleri belirtilen klasörden indeksleme

SearchOptions options = new SearchOptions();
options.UseSynonymSearch = true; // Eşanlamlı aramayı etkinleştirme

string query = "cry";
SearchResult result = index.Search(query, options); // Aranıyor
```

### Ayrıca bakınız

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Index](../../index)
* ad alanı [GroupDocs.Search](../../index)
* toplantı [GroupDocs.Search](../../../)

---

## Search(SearchQuery) {#search_1}

index. içinde arama yapar

```csharp
public SearchResult Search(SearchQuery query)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| query | SearchQuery | Arama sorgusu. |

### Geri dönüş değeri

Arama sonucu.

### Örnekler

Aşağıdaki örnek, nesne biçiminde sorgu kullanarak aramanın nasıl gerçekleştirileceğini gösterir.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); //Belirtilen klasörde indeks oluşturma
index.Add(documentsFolder); // Belgeleri belirtilen klasörden indeksleme

// Alt sorgu 1 oluşturuluyor
SearchQuery subquery1 = SearchQuery.CreateWordQuery("accommodation");
subquery1.SearchOptions = new SearchOptions(); // Arama seçeneklerini yalnızca alt sorgu 1 için ayarlama
subquery1.SearchOptions.FuzzySearch.Enabled = true; // Bulanık aramayı etkinleştirme
subquery1.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(3); // Maksimum fark sayısı ayarlanıyor

// Alt sorgu 2 oluşturuluyor
SearchQuery subquery2 = SearchQuery.CreateNumericRangeQuery(1, 1000000);

// Alt sorgu oluşturma 3
SearchQuery subquery3 = SearchQuery.CreateRegexQuery(@"(.)\1");

// Alt sorguları tek bir sorguda birleştirme
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

SearchResult result = index.Search(query); // Aranıyor
```

### Ayrıca bakınız

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [Index](../../index)
* ad alanı [GroupDocs.Search](../../index)
* toplantı [GroupDocs.Search](../../../)

---

## Search(SearchQuery, SearchOptions) {#search_2}

index. içinde arama yapar

```csharp
public SearchResult Search(SearchQuery query, SearchOptions options)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| query | SearchQuery | Arama sorgusu. |
| options | SearchOptions | Arama seçenekleri. |

### Geri dönüş değeri

Arama sonucu.

### Örnekler

Aşağıdaki örnek, nesne biçiminde sorgu kullanarak aramanın nasıl gerçekleştirileceğini gösterir.

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

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Index](../../index)
* ad alanı [GroupDocs.Search](../../index)
* toplantı [GroupDocs.Search](../../../)

---

## Search(SearchImage, ImageSearchOptions) {#search}

Dizinde ters görüntü araması gerçekleştirir.

```csharp
public ImageSearchResult Search(SearchImage image, ImageSearchOptions options)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| image | SearchImage | Aranacak resim. |
| options | ImageSearchOptions | Görsel arama seçenekleri. |

### Geri dönüş değeri

Tersine görsel aramanın sonucu.

### Ayrıca bakınız

* class [ImageSearchResult](../../../groupdocs.search.results/imagesearchresult)
* class [SearchImage](../../../groupdocs.search.common/searchimage)
* class [ImageSearchOptions](../../../groupdocs.search.options/imagesearchoptions)
* class [Index](../../index)
* ad alanı [GroupDocs.Search](../../index)
* toplantı [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
