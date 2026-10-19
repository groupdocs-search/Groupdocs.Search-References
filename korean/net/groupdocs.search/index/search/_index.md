---
title: "검색"
second_title: "GroupDocs.Search 용 .NET API Reference"
description: "인덱스를 검색합니다."
type: docs
weight: 260
url: /ko/net/groupdocs.search/index/search/
---
## Search(string) {#search_3}

인덱스를 검색합니다.

```csharp
public SearchResult Search(string query)
```

| Parameter | Type | 설명 |
| --- | --- | --- |
| 쿼리 | String | 검색 쿼리입니다. |

### 반환 값

검색 결과입니다.

### 예제

다음 예제는 간단한 검색을 수행하는 방법을 보여줍니다.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

SearchResult result = index.Search(query); // Searching
```

다음 예제는 정규식 검색을 수행하는 방법을 보여줍니다.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

string query = "^[0-9]{3,}"; // The caret symbol at the beginning of the search query tells the index that it is a Regex query
SearchResult result = index.Search(query); // Searching
```

다음 예제는 팩시드 검색을 수행하는 방법을 보여줍니다.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

string query = "content:Newton"; // The word before the colon in the query means the document field name to search
SearchResult result = index.Search(query); // Searching
```

### 또 보기

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(string, SearchOptions) {#search_4}

인덱스를 검색합니다.

```csharp
public SearchResult Search(string query, SearchOptions options)
```

| Parameter | Type | 설명 |
| --- | --- | --- |
| 쿼리 | String | 검색 쿼리입니다. |
| options | SearchOptions | 검색 옵션입니다. |

### 반환 값

검색 결과입니다.

### 예제

다음 예제는 퍼지 검색을 수행하는 방법을 보여줍니다.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

SearchOptions options = new SearchOptions();
options.FuzzySearch.Enabled = true; // Enabling the fuzzy search
options.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1); // Setting the number of possible differences for each word

// 시작과 끝에 있는 큰따옴표는 인덱스에 이것이 구문 검색 쿼리임을 알려줍니다.
string query = "\"The Pursuit of Happiness\"";
SearchResult result = index.Search(query, options); // Searching
```

다음 예제는 동의어 검색을 수행하는 방법을 보여줍니다.

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

### 또 보기

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(SearchQuery) {#search_1}

인덱스를 검색합니다.

```csharp
public SearchResult Search(SearchQuery query)
```

| Parameter | Type | 설명 |
| --- | --- | --- |
| 쿼리 | SearchQuery | 검색 쿼리입니다. |

### 반환 값

검색 결과입니다.

### 예제

다음 예제는 객체 형태의 쿼리를 사용하여 검색을 수행하는 방법을 보여줍니다.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

// 하위 쿼리 1 생성
SearchQuery subquery1 = SearchQuery.CreateWordQuery("accommodation");
subquery1.SearchOptions = new SearchOptions(); // Setting search options only for subquery 1
subquery1.SearchOptions.FuzzySearch.Enabled = true; // Enabling the fuzzy search
subquery1.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(3); // Setting maximum number of differences

// 하위 쿼리 2 생성
SearchQuery subquery2 = SearchQuery.CreateNumericRangeQuery(1, 1000000);

// 하위 쿼리 3 생성
SearchQuery subquery3 = SearchQuery.CreateRegexQuery(@"(.)\1");

// 하위 쿼리를 하나의 쿼리로 결합합니다
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

SearchResult result = index.Search(query); // Searching
```

### 또 보기

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(SearchQuery, SearchOptions) {#search_2}

인덱스를 검색합니다.

```csharp
public SearchResult Search(SearchQuery query, SearchOptions options)
```

| Parameter | Type | 설명 |
| --- | --- | --- |
| 쿼리 | SearchQuery | 검색 쿼리입니다. |
| options | SearchOptions | 검색 옵션입니다. |

### 반환 값

검색 결과입니다.

### 예제

다음 예제는 객체 형태의 쿼리를 사용하여 검색을 수행하는 방법을 보여줍니다.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

// 날짜 범위 검색의 하위 쿼리를 생성합니다
SearchQuery subquery1 = SearchQuery.CreateDateRangeQuery(new DateTime(2011, 6, 17), new DateTime(2013, 1, 1));

// 0에서 2까지 누락된 단어 수를 가진 와일드카드의 하위 쿼리를 생성합니다
SearchQuery subquery2 = SearchQuery.CreateWildcardQuery(0, 2);

// 단순 단어의 하위 쿼리를 생성합니다
SearchQuery subquery3 = SearchQuery.CreateWordQuery("birth");
subquery3.SearchOptions = new SearchOptions(); // Setting search options only for subquery 3
subquery3.SearchOptions.FuzzySearch.Enabled = true;
subquery3.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1);

// 하위 쿼리를 하나의 쿼리로 결합합니다
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

// 검색 결과 발생 횟수 용량이 증가된 검색 옵션 객체를 생성합니다
SearchOptions options = new SearchOptions(); // Overall search options
options.MaxOccurrenceCountPerTerm = 1000000;
options.MaxTotalOccurrenceCount = 10000000;

SearchResult result = index.Search(query, options); // Searching
```

### 또 보기

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(SearchImage, ImageSearchOptions) {#search}

인덱스에서 역 이미지 검색을 수행합니다.

```csharp
public ImageSearchResult Search(SearchImage image, ImageSearchOptions options)
```

| Parameter | Type | 설명 |
| --- | --- | --- |
| 이미지 | SearchImage | 검색할 이미지입니다. |
| options | ImageSearchOptions | 이미지 검색 옵션입니다. |

### 반환 값

역 이미지 검색 결과입니다.

### 또 보기

* class [ImageSearchResult](../../../groupdocs.search.results/imagesearchresult)
* class [SearchImage](../../../groupdocs.search.common/searchimage)
* class [ImageSearchOptions](../../../groupdocs.search.options/imagesearchoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->
