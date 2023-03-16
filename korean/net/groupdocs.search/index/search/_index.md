---
title: Search
second_title: GroupDocs..NET API 참조 검색
description: 인덱스에서 검색합니다.
type: docs
weight: 220
url: /ko/net/groupdocs.search/index/search/
---
## Search(string) {#search_3}

인덱스에서 검색합니다.

```csharp
public SearchResult Search(string query)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| query | String | 검색어입니다. |

### 반환 값

검색 결과입니다.

### 예

다음 예제는 단순 검색을 수행하는 방법을 보여줍니다.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // 지정된 폴더에 인덱스 생성
index.Add(documentsFolder); // 지정된 폴더에서 문서 인덱싱

SearchResult result = index.Search(query); // 검색 중
```

다음 예는 Regex 검색을 수행하는 방법을 보여줍니다.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // 지정된 폴더에 인덱스 생성
index.Add(documentsFolder); // 지정된 폴더에서 문서 인덱싱

string query = "^[0-9]{3,}"; // 검색 쿼리 시작 부분의 캐럿 기호는 색인에 Regex 쿼리임을 알려줍니다.
SearchResult result = index.Search(query); // 검색 중
```

다음 예는 패싯 검색을 수행하는 방법을 보여줍니다.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // 지정된 폴더에 인덱스 생성
index.Add(documentsFolder); // 지정된 폴더에서 문서 인덱싱

string query = "content:Newton"; // 쿼리에서 콜론 앞의 단어는 검색할 문서 필드 이름을 의미합니다.
SearchResult result = index.Search(query); // 검색 중
```

### 또한보십시오

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [Index](../../index)
* 네임스페이스 [GroupDocs.Search](../../index)
* 집회 [GroupDocs.Search](../../../)

---

## Search(string, SearchOptions) {#search_4}

인덱스에서 검색합니다.

```csharp
public SearchResult Search(string query, SearchOptions options)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| query | String | 검색어입니다. |
| options | SearchOptions | 검색 옵션. |

### 반환 값

검색 결과입니다.

### 예

다음 예제는 퍼지 검색을 수행하는 방법을 보여줍니다.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // 지정된 폴더에 인덱스 생성
index.Add(documentsFolder); // 지정된 폴더에서 문서 인덱싱

SearchOptions options = new SearchOptions();
options.FuzzySearch.Enabled = true; // 퍼지 검색 활성화
options.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1); // 각 단어에 대해 가능한 차이점 수 설정

// 시작과 끝의 큰따옴표는 색인에 구문 검색 쿼리임을 알려줍니다.
string query = "\"The Pursuit of Happiness\"";
SearchResult result = index.Search(query, options); // 검색 중
```

다음 예는 동의어 검색을 수행하는 방법을 보여줍니다.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // 지정된 폴더에 인덱스 생성
index.Add(documentsFolder); // 지정된 폴더에서 문서 인덱싱

SearchOptions options = new SearchOptions();
options.UseSynonymSearch = true; // 동의어 검색 활성화

string query = "cry";
SearchResult result = index.Search(query, options); // 검색 중
```

### 또한보십시오

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Index](../../index)
* 네임스페이스 [GroupDocs.Search](../../index)
* 집회 [GroupDocs.Search](../../../)

---

## Search(SearchQuery) {#search_1}

인덱스에서 검색합니다.

```csharp
public SearchResult Search(SearchQuery query)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| query | SearchQuery | 검색어입니다. |

### 반환 값

검색 결과입니다.

### 예

다음 예제에서는 쿼리를 사용하여 개체 형태로 검색하는 방법을 보여줍니다.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // 지정된 폴더에 인덱스 생성
index.Add(documentsFolder); // 지정된 폴더에서 문서 인덱싱

// 서브쿼리 1 생성
SearchQuery subquery1 = SearchQuery.CreateWordQuery("accommodation");
subquery1.SearchOptions = new SearchOptions(); // 서브 쿼리 1에만 검색 옵션 설정
subquery1.SearchOptions.FuzzySearch.Enabled = true; // 퍼지 검색 활성화
subquery1.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(3); // 최대 차이 수 설정

// 서브쿼리 2 생성
SearchQuery subquery2 = SearchQuery.CreateNumericRangeQuery(1, 1000000);

// 서브 쿼리 3 생성
SearchQuery subquery3 = SearchQuery.CreateRegexQuery(@"(.)\1");

// 하위 쿼리를 하나의 쿼리로 결합
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

SearchResult result = index.Search(query); // 검색 중
```

### 또한보십시오

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [Index](../../index)
* 네임스페이스 [GroupDocs.Search](../../index)
* 집회 [GroupDocs.Search](../../../)

---

## Search(SearchQuery, SearchOptions) {#search_2}

인덱스에서 검색합니다.

```csharp
public SearchResult Search(SearchQuery query, SearchOptions options)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| query | SearchQuery | 검색어입니다. |
| options | SearchOptions | 검색 옵션. |

### 반환 값

검색 결과입니다.

### 예

다음 예제에서는 쿼리를 사용하여 개체 형태로 검색하는 방법을 보여줍니다.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // 지정된 폴더에 인덱스 생성
index.Add(documentsFolder); // 지정된 폴더에서 문서 인덱싱

// 날짜 범위 검색 서브쿼리 생성
SearchQuery subquery1 = SearchQuery.CreateDateRangeQuery(new DateTime(2011, 6, 17), new DateTime(2013, 1, 1));

// 0에서 2까지 놓친 단어 수로 와일드 카드의 하위 쿼리 생성
SearchQuery subquery2 = SearchQuery.CreateWildcardQuery(0, 2);

//단순단어 서브쿼리 생성
SearchQuery subquery3 = SearchQuery.CreateWordQuery("birth");
subquery3.SearchOptions = new SearchOptions(); // 하위 쿼리 3에만 검색 옵션 설정
subquery3.SearchOptions.FuzzySearch.Enabled = true;
subquery3.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1);

// 하위 쿼리를 하나의 쿼리로 결합
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

// 발견된 항목의 증가된 용량으로 검색 옵션 객체 생성
SearchOptions options = new SearchOptions(); // 전체 검색 옵션
options.MaxOccurrenceCountPerTerm = 1000000;
options.MaxTotalOccurrenceCount = 10000000;

SearchResult result = index.Search(query, options); // 검색 중
```

### 또한보십시오

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Index](../../index)
* 네임스페이스 [GroupDocs.Search](../../index)
* 집회 [GroupDocs.Search](../../../)

---

## Search(SearchImage, ImageSearchOptions) {#search}

인덱스에서 역방향 이미지 검색을 수행합니다.

```csharp
public ImageSearchResult Search(SearchImage image, ImageSearchOptions options)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| image | SearchImage | 검색할 이미지입니다. |
| options | ImageSearchOptions | 이미지 검색 옵션. |

### 반환 값

역 이미지 검색 결과입니다.

### 또한보십시오

* class [ImageSearchResult](../../../groupdocs.search.results/imagesearchresult)
* class [SearchImage](../../../groupdocs.search.common/searchimage)
* class [ImageSearchOptions](../../../groupdocs.search.options/imagesearchoptions)
* class [Index](../../index)
* 네임스페이스 [GroupDocs.Search](../../index)
* 집회 [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
