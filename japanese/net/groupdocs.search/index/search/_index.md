---
title: Search
second_title: GroupDocs.Search for .NET API リファレンス
description: index. で検索します
type: docs
weight: 220
url: /ja/net/groupdocs.search/index/search/
---
## Search(string) {#search_3}

index. で検索します。

```csharp
public SearchResult Search(string query)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| query | String | 検索クエリ。 |

### 戻り値

検索結果。

### 例

次の例は、単純な検索を実行する方法を示しています。

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // 指定したフォルダにインデックスを作成
index.Add(documentsFolder); // 指定されたフォルダからのドキュメントのインデックス作成

SearchResult result = index.Search(query); // 検索中
```

次の例は、正規表現検索を実行する方法を示しています。

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // 指定したフォルダにインデックスを作成
index.Add(documentsFolder); // 指定されたフォルダからのドキュメントのインデックス作成

string query = "^[0-9]{3,}"; // 検索クエリの先頭にあるキャレット記号は、それが正規表現クエリであることをインデックスに伝えます
SearchResult result = index.Search(query); // 検索中
```

次の例は、ファセット検索を実行する方法を示しています。

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // 指定したフォルダにインデックスを作成
index.Add(documentsFolder); // 指定されたフォルダからのドキュメントのインデックス作成

string query = "content:Newton"; // クエリのコロンの前の単語は、検索するドキュメント フィールド名を意味します
SearchResult result = index.Search(query); // 検索中
```

### 関連項目

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [Index](../../index)
* 名前空間 [GroupDocs.Search](../../index)
* 組み立て [GroupDocs.Search](../../../)

---

## Search(string, SearchOptions) {#search_4}

index. で検索します。

```csharp
public SearchResult Search(string query, SearchOptions options)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| query | String | 検索クエリ。 |
| options | SearchOptions | 検索オプション。 |

### 戻り値

検索結果。

### 例

次の例は、あいまい検索の実行方法を示しています。

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // 指定したフォルダにインデックスを作成
index.Add(documentsFolder); // 指定されたフォルダからのドキュメントのインデックス作成

SearchOptions options = new SearchOptions();
options.FuzzySearch.Enabled = true; // あいまい検索を有効にする
options.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1); // 各単語の可能な違いの数を設定する

// 先頭と末尾の二重引用符は、フレーズ検索クエリであることをインデックスに伝えます
string query = "\"The Pursuit of Happiness\"";
SearchResult result = index.Search(query, options); // 検索中
```

次の例は、類義語検索の実行方法を示しています。

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // 指定したフォルダにインデックスを作成
index.Add(documentsFolder); // 指定されたフォルダからのドキュメントのインデックス作成

SearchOptions options = new SearchOptions();
options.UseSynonymSearch = true; // 同義語検索を有効にする

string query = "cry";
SearchResult result = index.Search(query, options); // 検索中
```

### 関連項目

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Index](../../index)
* 名前空間 [GroupDocs.Search](../../index)
* 組み立て [GroupDocs.Search](../../../)

---

## Search(SearchQuery) {#search_1}

index. で検索します。

```csharp
public SearchResult Search(SearchQuery query)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| query | SearchQuery | 検索クエリ。 |

### 戻り値

検索結果。

### 例

次の例は、オブジェクト形式のクエリを使用して検索を実行する方法を示しています。

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // 指定したフォルダにインデックスを作成
index.Add(documentsFolder); // 指定されたフォルダからのドキュメントのインデックス作成

// サブクエリ 1 の作成
SearchQuery subquery1 = SearchQuery.CreateWordQuery("accommodation");
subquery1.SearchOptions = new SearchOptions(); // サブクエリ 1 のみに検索オプションを設定
subquery1.SearchOptions.FuzzySearch.Enabled = true; // あいまい検索を有効にする
subquery1.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(3); // 差分の最大数を設定

// サブクエリ 2 の作成
SearchQuery subquery2 = SearchQuery.CreateNumericRangeQuery(1, 1000000);

// サブクエリ 3 の作成
SearchQuery subquery3 = SearchQuery.CreateRegexQuery(@"(.)\1");

// サブクエリを 1 つのクエリに結合
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

SearchResult result = index.Search(query); // 検索中
```

### 関連項目

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [Index](../../index)
* 名前空間 [GroupDocs.Search](../../index)
* 組み立て [GroupDocs.Search](../../../)

---

## Search(SearchQuery, SearchOptions) {#search_2}

index. で検索します。

```csharp
public SearchResult Search(SearchQuery query, SearchOptions options)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| query | SearchQuery | 検索クエリ。 |
| options | SearchOptions | 検索オプション。 |

### 戻り値

検索結果。

### 例

次の例は、オブジェクト形式のクエリを使用して検索を実行する方法を示しています。

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // 指定したフォルダにインデックスを作成
index.Add(documentsFolder); // 指定されたフォルダからのドキュメントのインデックス作成

// 日付範囲検索のサブクエリ作成
SearchQuery subquery1 = SearchQuery.CreateDateRangeQuery(new DateTime(2011, 6, 17), new DateTime(2013, 1, 1));

// 単語数が 0 から 2 のワイルドカードのサブクエリを作成
SearchQuery subquery2 = SearchQuery.CreateWildcardQuery(0, 2);

// 単純な単語のサブクエリを作成
SearchQuery subquery3 = SearchQuery.CreateWordQuery("birth");
subquery3.SearchOptions = new SearchOptions(); // サブクエリ 3 のみに検索オプションを設定
subquery3.SearchOptions.FuzzySearch.Enabled = true;
subquery3.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1);

// サブクエリを 1 つのクエリに結合
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

// 見つかったオカレンスの容量を増やした検索オプション オブジェクトを作成する
SearchOptions options = new SearchOptions(); // 全体的な検索オプション
options.MaxOccurrenceCountPerTerm = 1000000;
options.MaxTotalOccurrenceCount = 10000000;

SearchResult result = index.Search(query, options); // 検索中
```

### 関連項目

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Index](../../index)
* 名前空間 [GroupDocs.Search](../../index)
* 組み立て [GroupDocs.Search](../../../)

---

## Search(SearchImage, ImageSearchOptions) {#search}

インデックスで画像の逆検索を実行します。

```csharp
public ImageSearchResult Search(SearchImage image, ImageSearchOptions options)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| image | SearchImage | 検索する画像。 |
| options | ImageSearchOptions | 画像検索オプション。 |

### 戻り値

逆画像検索の結果です。

### 関連項目

* class [ImageSearchResult](../../../groupdocs.search.results/imagesearchresult)
* class [SearchImage](../../../groupdocs.search.common/searchimage)
* class [ImageSearchOptions](../../../groupdocs.search.options/imagesearchoptions)
* class [Index](../../index)
* 名前空間 [GroupDocs.Search](../../index)
* 組み立て [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
