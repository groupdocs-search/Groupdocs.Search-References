---
title: Search
second_title: GroupDocs.Search for .NET API 参考
description: 在索引中搜索
type: docs
weight: 220
url: /zh/net/groupdocs.search/index/search/
---
## Search(string) {#search_3}

在索引中搜索。

```csharp
public SearchResult Search(string query)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| query | String | 搜索查询。 |

### 返回值

搜索结果。

### 例子

以下示例演示如何执行简单搜索。

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // 在指定文件夹中创建索引
index.Add(documentsFolder); // 索引指定文件夹中的文档

SearchResult result = index.Search(query); // 搜索
```

以下示例演示了如何执行正则表达式搜索。

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // 在指定文件夹中创建索引
index.Add(documentsFolder); // 索引指定文件夹中的文档

string query = "^[0-9]{3,}"; // 搜索查询开头的插入符号告诉索引它是一个正则表达式查询
SearchResult result = index.Search(query); // 搜索
```

以下示例演示如何执行分面搜索。

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // 在指定文件夹中创建索引
index.Add(documentsFolder); // 索引指定文件夹中的文档

string query = "content:Newton"; // 查询中冒号前的单词表示要搜索的文档字段名
SearchResult result = index.Search(query); // 搜索
```

### 也可以看看

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [Index](../../index)
* 命名空间 [GroupDocs.Search](../../index)
* 部件 [GroupDocs.Search](../../../)

---

## Search(string, SearchOptions) {#search_4}

在索引中搜索。

```csharp
public SearchResult Search(string query, SearchOptions options)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| query | String | 搜索查询。 |
| options | SearchOptions | 搜索选项。 |

### 返回值

搜索结果。

### 例子

以下示例演示如何执行模糊搜索。

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // 在指定文件夹中创建索引
index.Add(documentsFolder); // 索引指定文件夹中的文档

SearchOptions options = new SearchOptions();
options.FuzzySearch.Enabled = true; // 启用模糊搜索
options.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1); // 设置每个单词的可能差异数

// 开头和结尾的双引号告诉索引它是词组搜索查询
string query = "\"The Pursuit of Happiness\"";
SearchResult result = index.Search(query, options); // 搜索
```

以下示例演示如何执行同义词搜索。

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // 在指定文件夹中创建索引
index.Add(documentsFolder); // 索引指定文件夹中的文档

SearchOptions options = new SearchOptions();
options.UseSynonymSearch = true; // 启用同义词搜索

string query = "cry";
SearchResult result = index.Search(query, options); // 搜索
```

### 也可以看看

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Index](../../index)
* 命名空间 [GroupDocs.Search](../../index)
* 部件 [GroupDocs.Search](../../../)

---

## Search(SearchQuery) {#search_1}

在索引中搜索。

```csharp
public SearchResult Search(SearchQuery query)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| query | SearchQuery | 搜索查询。 |

### 返回值

搜索结果。

### 例子

以下示例演示如何使用对象形式的查询执行搜索。

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // 在指定文件夹中创建索引
index.Add(documentsFolder); // 索引指定文件夹中的文档

// 创建子查询 1
SearchQuery subquery1 = SearchQuery.CreateWordQuery("accommodation");
subquery1.SearchOptions = new SearchOptions(); // 仅为子查询 1 设置搜索选项
subquery1.SearchOptions.FuzzySearch.Enabled = true; // 启用模糊搜索
subquery1.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(3); // 设置最大差异数

// 创建子查询 2
SearchQuery subquery2 = SearchQuery.CreateNumericRangeQuery(1, 1000000);

// 创建子查询 3
SearchQuery subquery3 = SearchQuery.CreateRegexQuery(@"(.)\1");

// 将子查询合并为一个查询
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

SearchResult result = index.Search(query); // 搜索
```

### 也可以看看

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [Index](../../index)
* 命名空间 [GroupDocs.Search](../../index)
* 部件 [GroupDocs.Search](../../../)

---

## Search(SearchQuery, SearchOptions) {#search_2}

在索引中搜索。

```csharp
public SearchResult Search(SearchQuery query, SearchOptions options)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| query | SearchQuery | 搜索查询。 |
| options | SearchOptions | 搜索选项。 |

### 返回值

搜索结果。

### 例子

以下示例演示如何使用对象形式的查询执行搜索。

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // 在指定文件夹中创建索引
index.Add(documentsFolder); // 索引指定文件夹中的文档

// 创建日期范围搜索的子查询
SearchQuery subquery1 = SearchQuery.CreateDateRangeQuery(new DateTime(2011, 6, 17), new DateTime(2013, 1, 1));

// 创建通配符的子查询，遗漏单词数从 0 到 2
SearchQuery subquery2 = SearchQuery.CreateWildcardQuery(0, 2);

// 创建简单单词的子查询
SearchQuery subquery3 = SearchQuery.CreateWordQuery("birth");
subquery3.SearchOptions = new SearchOptions(); // 仅为子查询 3 设置搜索选项
subquery3.SearchOptions.FuzzySearch.Enabled = true;
subquery3.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1);

// 将子查询合并为一个查询
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

// 创建搜索选项对象，增加找到的事件的容量
SearchOptions options = new SearchOptions(); // 整体搜索选项
options.MaxOccurrenceCountPerTerm = 1000000;
options.MaxTotalOccurrenceCount = 10000000;

SearchResult result = index.Search(query, options); // 搜索
```

### 也可以看看

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Index](../../index)
* 命名空间 [GroupDocs.Search](../../index)
* 部件 [GroupDocs.Search](../../../)

---

## Search(SearchImage, ImageSearchOptions) {#search}

在索引中执行反向图像搜索。

```csharp
public ImageSearchResult Search(SearchImage image, ImageSearchOptions options)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| image | SearchImage | 要搜索的图像。 |
| options | ImageSearchOptions | 图像搜索选项。 |

### 返回值

反向图像搜索的结果。

### 也可以看看

* class [ImageSearchResult](../../../groupdocs.search.results/imagesearchresult)
* class [SearchImage](../../../groupdocs.search.common/searchimage)
* class [ImageSearchOptions](../../../groupdocs.search.options/imagesearchoptions)
* class [Index](../../index)
* 命名空间 [GroupDocs.Search](../../index)
* 部件 [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
