---
title: "検索"
second_title: "GroupDocs.Search for .NET API リファレンス"
description: "インデックス内を検索します。"
type: docs
weight: 260
url: /ja/net/groupdocs.search/index/search/
---
## Search(string) {#search_3}

インデックス内を検索します。

```csharp
public SearchResult Search(string query)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| クエリ | String | 検索クエリです。 |

### 戻り値

検索結果です。

### 例

次の例はシンプル検索を実行する方法を示しています。

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

SearchResult result = index.Search(query); // Searching
```

次の例は正規表現検索を実行する方法を示しています。

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

string query = "^[0-9]{3,}"; // The caret symbol at the beginning of the search query tells the index that it is a Regex query
SearchResult result = index.Search(query); // Searching
```

次の例はファセット検索を実行する方法を示しています。

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

string query = "content:Newton"; // The word before the colon in the query means the document field name to search
SearchResult result = index.Search(query); // Searching
```

### 関連項目

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(string, SearchOptions) {#search_4}

インデックス内を検索します。

```csharp
public SearchResult Search(string query, SearchOptions options)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| クエリ | String | 検索クエリです。 |
| オプション | SearchOptions | 検索オプションです。 |

### 戻り値

検索結果です。

### 例

次の例はファジー検索を実行する方法を示しています。

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

SearchOptions options = new SearchOptions();
options.FuzzySearch.Enabled = true; // Enabling the fuzzy search
options.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1); // Setting the number of possible differences for each word

// 先頭と末尾の二重引用符は、インデックスにフレーズ検索クエリであることを示します。
string query = "\"The Pursuit of Happiness\"";
SearchResult result = index.Search(query, options); // Searching
```

次の例は同義語検索を実行する方法を示しています。

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

### 関連項目

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(SearchQuery) {#search_1}

インデックス内を検索します。

```csharp
public SearchResult Search(SearchQuery query)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| クエリ | SearchQuery | 検索クエリです。 |

### 戻り値

検索結果です。

### 例

次の例はオブジェクト形式のクエリを使用して検索を実行する方法を示しています。

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

// サブクエリ 1 の作成
SearchQuery subquery1 = SearchQuery.CreateWordQuery("accommodation");
subquery1.SearchOptions = new SearchOptions(); // Setting search options only for subquery 1
subquery1.SearchOptions.FuzzySearch.Enabled = true; // Enabling the fuzzy search
subquery1.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(3); // Setting maximum number of differences

// サブクエリ 2 の作成
SearchQuery subquery2 = SearchQuery.CreateNumericRangeQuery(1, 1000000);

// サブクエリ 3 の作成
SearchQuery subquery3 = SearchQuery.CreateRegexQuery(@"(.)\1");

// サブクエリを1つのクエリに結合しています。
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

SearchResult result = index.Search(query); // Searching
```

### 関連項目

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(SearchQuery, SearchOptions) {#search_2}

インデックス内を検索します。

```csharp
public SearchResult Search(SearchQuery query, SearchOptions options)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| クエリ | SearchQuery | 検索クエリです。 |
| オプション | SearchOptions | 検索オプションです。 |

### 戻り値

検索結果です。

### 例

次の例はオブジェクト形式のクエリを使用して検索を実行する方法を示しています。

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

// 日付範囲検索のサブクエリを作成しています。
SearchQuery subquery1 = SearchQuery.CreateDateRangeQuery(new DateTime(2011, 6, 17), new DateTime(2013, 1, 1));

// 0から2までの欠落単語数を持つワイルドカードのサブクエリを作成しています。
SearchQuery subquery2 = SearchQuery.CreateWildcardQuery(0, 2);

// シンプルな単語のサブクエリを作成しています。
SearchQuery subquery3 = SearchQuery.CreateWordQuery("birth");
subquery3.SearchOptions = new SearchOptions(); // Setting search options only for subquery 3
subquery3.SearchOptions.FuzzySearch.Enabled = true;
subquery3.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1);

// サブクエリを1つのクエリに結合しています。
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

// 見つかった出現回数の容量を増加させた検索オプションオブジェクトを作成しています。
SearchOptions options = new SearchOptions(); // Overall search options
options.MaxOccurrenceCountPerTerm = 1000000;
options.MaxTotalOccurrenceCount = 10000000;

SearchResult result = index.Search(query, options); // Searching
```

### 関連項目

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(SearchImage, ImageSearchOptions) {#search}

インデックスで逆画像検索を実行します。

```csharp
public ImageSearchResult Search(SearchImage image, ImageSearchOptions options)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 画像 | SearchImage | 検索対象の画像です。 |
| オプション | ImageSearchOptions | 画像検索オプションです。 |

### 戻り値

逆画像検索の結果です。

### 関連項目

* class [ImageSearchResult](../../../groupdocs.search.results/imagesearchresult)
* class [SearchImage](../../../groupdocs.search.common/searchimage)
* class [ImageSearchOptions](../../../groupdocs.search.options/imagesearchoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->
