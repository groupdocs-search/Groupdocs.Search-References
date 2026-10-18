---
title: "搜索"
second_title: "GroupDocs.Search for .NET API 参考"
description: "在索引中搜索。"
type: docs
weight: 260
url: /zh/net/groupdocs.search/index/search/
---
## Search(string) {#search_3}

在索引中搜索。

```csharp
public SearchResult Search(string query)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 查询 | 字符串 | 搜索查询。 |

### 返回值

搜索结果。

### 示例

下面的示例演示如何执行简单搜索。

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

SearchResult result = index.Search(query); // Searching
```

下面的示例演示如何执行正则表达式搜索。

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

string query = "^[0-9]{3,}"; // The caret symbol at the beginning of the search query tells the index that it is a Regex query
SearchResult result = index.Search(query); // Searching
```

下面的示例演示如何执行分面搜索。

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

string query = "content:Newton"; // The word before the colon in the query means the document field name to search
SearchResult result = index.Search(query); // Searching
```

### 另见

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(string, SearchOptions) {#search_4}

在索引中搜索。

```csharp
public SearchResult Search(string query, SearchOptions options)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 查询 | 字符串 | 搜索查询。 |
| 选项 | SearchOptions | 搜索选项。 |

### 返回值

搜索结果。

### 示例

下面的示例演示如何执行模糊搜索。

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

SearchOptions options = new SearchOptions();
options.FuzzySearch.Enabled = true; // Enabling the fuzzy search
options.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1); // Setting the number of possible differences for each word

// 开头和结尾的双引号告诉索引这是短语搜索查询
string query = "\"The Pursuit of Happiness\"";
SearchResult result = index.Search(query, options); // Searching
```

下面的示例演示如何执行同义词搜索。

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

### 另见

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(SearchQuery) {#search_1}

在索引中搜索。

```csharp
public SearchResult Search(SearchQuery query)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 查询 | SearchQuery | 搜索查询。 |

### 返回值

搜索结果。

### 示例

下面的示例演示如何使用对象形式的查询执行搜索。

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

// 创建子查询 1
SearchQuery subquery1 = SearchQuery.CreateWordQuery("accommodation");
subquery1.SearchOptions = new SearchOptions(); // Setting search options only for subquery 1
subquery1.SearchOptions.FuzzySearch.Enabled = true; // Enabling the fuzzy search
subquery1.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(3); // Setting maximum number of differences

// 创建子查询 2
SearchQuery subquery2 = SearchQuery.CreateNumericRangeQuery(1, 1000000);

// 创建子查询 3
SearchQuery subquery3 = SearchQuery.CreateRegexQuery(@"(.)\1");

// 将子查询合并为一个查询
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

SearchResult result = index.Search(query); // Searching
```

### 另见

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(SearchQuery, SearchOptions) {#search_2}

在索引中搜索。

```csharp
public SearchResult Search(SearchQuery query, SearchOptions options)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 查询 | SearchQuery | 搜索查询。 |
| 选项 | SearchOptions | 搜索选项。 |

### 返回值

搜索结果。

### 示例

下面的示例演示如何使用对象形式的查询执行搜索。

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

// 创建日期范围搜索的子查询
SearchQuery subquery1 = SearchQuery.CreateDateRangeQuery(new DateTime(2011, 6, 17), new DateTime(2013, 1, 1));

// 创建通配符子查询，漏词数量从 0 到 2
SearchQuery subquery2 = SearchQuery.CreateWildcardQuery(0, 2);

// 创建简单单词的子查询
SearchQuery subquery3 = SearchQuery.CreateWordQuery("birth");
subquery3.SearchOptions = new SearchOptions(); // Setting search options only for subquery 3
subquery3.SearchOptions.FuzzySearch.Enabled = true;
subquery3.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1);

// 将子查询合并为一个查询
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

// 创建搜索选项对象，增加已找到出现次数的容量
SearchOptions options = new SearchOptions(); // Overall search options
options.MaxOccurrenceCountPerTerm = 1000000;
options.MaxTotalOccurrenceCount = 10000000;

SearchResult result = index.Search(query, options); // Searching
```

### 另见

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(SearchImage, ImageSearchOptions) {#search}

在索引中执行反向图像搜索。

```csharp
public ImageSearchResult Search(SearchImage image, ImageSearchOptions options)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 图像 | SearchImage | 要搜索的图像。 |
| 选项 | ImageSearchOptions | 图像搜索选项。 |

### 返回值

反向图像搜索的结果。

### 另见

* class [ImageSearchResult](../../../groupdocs.search.results/imagesearchresult)
* class [SearchImage](../../../groupdocs.search.common/searchimage)
* class [ImageSearchOptions](../../../groupdocs.search.options/imagesearchoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->
