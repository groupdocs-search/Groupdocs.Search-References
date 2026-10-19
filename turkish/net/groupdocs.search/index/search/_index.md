---
title: "Ara"
second_title: "GroupDocs.Search için .NET API Referansı"
description: "Dizinde arama yapar."
type: docs
weight: 260
url: /tr/net/groupdocs.search/index/search/
---
## Search(string) {#search_3}

Dizinde arama yapar.

```csharp
public SearchResult Search(string query)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sorgu | String | Arama sorgusu. |

### Dönüş Değeri

Arama sonucu.

### Örnekler

Aşağıdaki örnek, basit aramanın nasıl yapılacağını gösterir.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

SearchResult result = index.Search(query); // Searching
```

Aşağıdaki örnek, Regex aramasının nasıl yapılacağını gösterir.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

string query = "^[0-9]{3,}"; // The caret symbol at the beginning of the search query tells the index that it is a Regex query
SearchResult result = index.Search(query); // Searching
```

Aşağıdaki örnek, çok yönlü aramanın nasıl yapılacağını gösterir.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

string query = "content:Newton"; // The word before the colon in the query means the document field name to search
SearchResult result = index.Search(query); // Searching
```

### Ayrıca Bakınız

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(string, SearchOptions) {#search_4}

Dizinde arama yapar.

```csharp
public SearchResult Search(string query, SearchOptions options)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sorgu | String | Arama sorgusu. |
| seçenekler | SearchOptions | Arama seçenekleri. |

### Dönüş Değeri

Arama sonucu.

### Örnekler

Aşağıdaki örnek, bulanık aramanın nasıl yapılacağını gösterir.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

SearchOptions options = new SearchOptions();
options.FuzzySearch.Enabled = true; // Enabling the fuzzy search
options.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1); // Setting the number of possible differences for each word

// Başlangıç ve sonda çift tırnak işaretleri, dizine bunun bir ifade arama sorgusu olduğunu söyler
string query = "\"The Pursuit of Happiness\"";
SearchResult result = index.Search(query, options); // Searching
```

Aşağıdaki örnek, eşanlamlı aramanın nasıl yapılacağını gösterir.

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

### Ayrıca Bakınız

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(SearchQuery) {#search_1}

Dizinde arama yapar.

```csharp
public SearchResult Search(SearchQuery query)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sorgu | SearchQuery | Arama sorgusu. |

### Dönüş Değeri

Arama sonucu.

### Örnekler

Aşağıdaki örnek, sorgunun nesne biçiminde kullanılarak aramanın nasıl yapılacağını gösterir.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

// Alt sorgu 1 oluşturma
SearchQuery subquery1 = SearchQuery.CreateWordQuery("accommodation");
subquery1.SearchOptions = new SearchOptions(); // Setting search options only for subquery 1
subquery1.SearchOptions.FuzzySearch.Enabled = true; // Enabling the fuzzy search
subquery1.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(3); // Setting maximum number of differences

// Alt sorgu 2 oluşturma
SearchQuery subquery2 = SearchQuery.CreateNumericRangeQuery(1, 1000000);

// Alt sorgu 3 oluşturma
SearchQuery subquery3 = SearchQuery.CreateRegexQuery(@"(.)\1");

// Alt sorguları tek bir sorguya birleştirme
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

SearchResult result = index.Search(query); // Searching
```

### Ayrıca Bakınız

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(SearchQuery, SearchOptions) {#search_2}

Dizinde arama yapar.

```csharp
public SearchResult Search(SearchQuery query, SearchOptions options)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sorgu | SearchQuery | Arama sorgusu. |
| seçenekler | SearchOptions | Arama seçenekleri. |

### Dönüş Değeri

Arama sonucu.

### Örnekler

Aşağıdaki örnek, sorgunun nesne biçiminde kullanılarak aramanın nasıl yapılacağını gösterir.

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

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(SearchImage, ImageSearchOptions) {#search}

Dizinde ters görüntü araması gerçekleştirir.

```csharp
public ImageSearchResult Search(SearchImage image, ImageSearchOptions options)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| görüntü | SearchImage | Aranacak görüntü. |
| seçenekler | ImageSearchOptions | Görüntü arama seçenekleri. |

### Dönüş Değeri

Ters görüntü aramasının sonucu.

### Ayrıca Bakınız

* class [ImageSearchResult](../../../groupdocs.search.results/imagesearchresult)
* class [SearchImage](../../../groupdocs.search.common/searchimage)
* class [ImageSearchOptions](../../../groupdocs.search.options/imagesearchoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->
