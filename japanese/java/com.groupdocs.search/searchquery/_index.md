---
title: "SearchQuery"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "オブジェクト形式の検索クエリを表します。"
type: docs
weight: 25
url: /ja/java/com.groupdocs.search/searchquery/
---
**Inheritance:**
java.lang.Object
```
public abstract class SearchQuery
```

オブジェクト形式の検索クエリを表します。


**Learn more**

* [Searching](../https://docs.groupdocs.com/display/searchjava/Searching)
* [Queries in text and object form](../https://docs.groupdocs.com/display/searchjava/Queries+in+text+and+object+form)
* [Nesting search queries in object form](../https://docs.groupdocs.com/display/searchjava/Nesting+search+queries+in+object+form)


この例はクラスの典型的な使用方法を示しています。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
 
Index index = new Index(indexFolder); // 指定されたフォルダーにインデックスを作成しています
index.add(documentsFolder); // 指定されたフォルダーからドキュメントをインデックス化しています
 
// 日付範囲検索のサブクエリを作成しています
SearchQuery subquery1 = SearchQuery.createDateRangeQuery(new Date(2011, 6, 17), new Date(2013, 1, 1));
 
// 0から2までの欠落語数を持つワイルドカードのサブクエリを作成しています
SearchQuery subquery2 = SearchQuery.createWildcardQuery(0, 2);
 
// 単語のサブクエリを作成しています
SearchQuery subquery3 = SearchQuery.createWordQuery("birth");
subquery3.setSearchOptions(new SearchOptions()); // サブクエリ3だけの検索オプションを設定しています
subquery3.getSearchOptions().getFuzzySearch().setEnabled(true);
subquery3.getSearchOptions().getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1));
 
// サブクエリを1つのクエリに結合しています
SearchQuery query = SearchQuery.createPhraseSearchQuery(subquery1, subquery2, subquery3);
 
// 検索オプションオブジェクトを作成し、見つかった出現回数の容量を増やします
SearchOptions options = new SearchOptions(); // 全体の検索オプション
options.setMaxOccurrenceCountPerTerm(1000000);
options.setMaxTotalOccurrenceCount(10000000);
 
SearchResult result = index.search(query, options); // 検索中
 
```
 
````


## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getFieldName()](#getFieldName--) | フィールド名を取得します。 |
|
|  | [getChildCount()](#getChildCount--) | 子クエリの数を取得します。 |
|
|  | [getFirstChild()](#getFirstChild--) | 最初の子クエリを取得します。 |
|
|  | [getSecondChild()](#getSecondChild--) | 2番目の子クエリを取得します。 |
|
|  | [getChild(int index)](#getChild-int-) | インデックスで子クエリを取得します。 |
|
|  | [getSearchOptions()](#getSearchOptions--) | この検索クエリの検索オプションを取得または設定します。 |
|
|  | [setSearchOptions(SearchOptions value)](#setSearchOptions-com.groupdocs.search.options.SearchOptions-) | この検索クエリの検索オプションを取得または設定します。 |
|
|  | [toString()](#toString--) | 現在の  SearchQuery  インスタンスを表す  System.String  を返します。 |
|
|  | [createWordQuery(String term)](#createWordQuery-java.lang.String-) | シンプルな単語クエリを作成します。 |
|
|  | [createWordPatternQuery(WordPattern pattern)](#createWordPatternQuery-com.groupdocs.search.common.WordPattern-) | 単語パターンクエリを作成します。 |
|
|  | [createRegexQuery(String pattern)](#createRegexQuery-java.lang.String-) | 正規表現クエリを作成します。 |
|
|  | [createRegexQuery(String pattern, int options)](#createRegexQuery-java.lang.String-int-) | 正規表現クエリを作成します。 |
|
|  | [createNumericRangeQuery(long start, long end)](#createNumericRangeQuery-long-long-) | 数値範囲クエリを作成します。 |
|
|  | [createDateRangeQuery(Date start, Date end)](#createDateRangeQuery-java.util.Date-java.util.Date-) | 日付範囲クエリを作成します。 |
|
|  | [createPhraseSearchQuery(SearchQuery[] queries)](#createPhraseSearchQuery-com.groupdocs.search.SearchQuery...-) | フレーズ検索クエリを作成します。 |
|
|  | [createAndQuery(SearchQuery[] queries)](#createAndQuery-com.groupdocs.search.SearchQuery---) | 元の各クエリで見つかるドキュメントのみを検索する結合クエリを作成します。 |
|
|  | [createFieldQuery(String fieldName, SearchQuery query)](#createFieldQuery-java.lang.String-com.groupdocs.search.SearchQuery-) | 指定されたクエリにフィールドを追加します。 |
|
|  | [createNotQuery(SearchQuery query)](#createNotQuery-com.groupdocs.search.SearchQuery-) | 元のクエリで見つかるドキュメントに対して、インデックス内の残りのドキュメントを検索する反転クエリを作成します。 |
|
|  | [createAndQuery(SearchQuery leftQuery, SearchQuery rightQuery)](#createAndQuery-com.groupdocs.search.SearchQuery-com.groupdocs.search.SearchQuery-) | 元の各クエリで見つかるドキュメントのみを検索する結合クエリを作成します。 |
|
|  | [createOrQuery(SearchQuery leftQuery, SearchQuery rightQuery)](#createOrQuery-com.groupdocs.search.SearchQuery-com.groupdocs.search.SearchQuery-) | 元のクエリのいずれかで少なくとも1つ見つかるすべてのドキュメントを検索する結合クエリを作成します。 |
|
|  | [createOrQuery(SearchQuery[] queries)](#createOrQuery-com.groupdocs.search.SearchQuery---) | 元のクエリのいずれかで少なくとも1つ見つかるすべてのドキュメントを検索する結合クエリを作成します。 |
|
|  | [createWildcardQuery(int count)](#createWildcardQuery-int-) | フレーズ検索用のワイルドカードを作成します。 |
|
|  | [createWildcardQuery(int minCount, int maxCount)](#createWildcardQuery-int-int-) | フレーズ検索用のワイルドカードを作成します。 |
|
### getFieldName() {#getFieldName--}
```
public String getFieldName()
```


フィールド名を取得します。


**Returns:**
java.lang.String - フィールド名です。

### getChildCount() {#getChildCount--}
```
public int getChildCount()
```


子クエリの数を取得します。


**Returns:**
int - 子クエリの数です。

### getFirstChild() {#getFirstChild--}
```
public SearchQuery getFirstChild()
```


最初の子クエリを取得します。


**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - The first child query.

### getSecondChild() {#getSecondChild--}
```
public SearchQuery getSecondChild()
```


2番目の子クエリを取得します。


**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - The second child query.

### getChild(int index) {#getChild-int-}
```
public abstract SearchQuery getChild(int index)
```


インデックスで子クエリを取得します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | インデックス | int | インデックスです。 |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A child query corresponding the specified index.

### getSearchOptions() {#getSearchOptions--}
```
public final SearchOptions getSearchOptions()
```


この検索クエリの検索オプションを取得または設定します。


**Returns:**
[SearchOptions](../../com.groupdocs.search.options/searchoptions) - The search options.

### setSearchOptions(SearchOptions value) {#setSearchOptions-com.groupdocs.search.options.SearchOptions-}
```
public final void setSearchOptions(SearchOptions value)
```


この検索クエリの検索オプションを取得または設定します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | value | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | 検索オプションです。 |
|

### toString() {#toString--}
```
public abstract String toString()
```


現在の  SearchQuery  インスタンスを表す  System.String  を返します。


**Returns:**
java.lang.String - 現在の  SearchQuery  インスタンスを表す  System.String です。

### createWordQuery(String term) {#createWordQuery-java.lang.String-}
```
public static SearchQuery createWordQuery(String term)
```


シンプルな単語クエリを作成します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | term | java.lang.String | 検索対象の term です。 |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A simple word query.

### createWordPatternQuery(WordPattern pattern) {#createWordPatternQuery-com.groupdocs.search.common.WordPattern-}
```
public static SearchQuery createWordPatternQuery(WordPattern pattern)
```


単語パターンクエリを作成します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | pattern | [WordPattern](../../com.groupdocs.search.common/wordpattern) | 単語パターンです。 |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A word pattern query.

### createRegexQuery(String pattern) {#createRegexQuery-java.lang.String-}
```
public static SearchQuery createRegexQuery(String pattern)
```


正規表現クエリを作成します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | パターン | java.lang.String | マッチさせる正規表現パターンです。 |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A regular expression query.

### createRegexQuery(String pattern, int options) {#createRegexQuery-java.lang.String-int-}
```
public static SearchQuery createRegexQuery(String pattern, int options)
```


正規表現クエリを作成します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | パターン | java.lang.String | マッチさせる正規表現パターンです。 |
|
|  | オプション | int | 正規表現を修正する列挙値のビット単位の組み合わせです。この値には RegexOptions.IgnoreCase フラグが含まれている必要があります。 |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A regular expression query.

### createNumericRangeQuery(long start, long end) {#createNumericRangeQuery-long-long-}
```
public static SearchQuery createNumericRangeQuery(long start, long end)
```


数値範囲クエリを作成します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 開始 | long | 範囲の開始値です。 |
|
|  | 終了 | long | 範囲の終了値です。 |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A numeric range query.

### createDateRangeQuery(Date start, Date end) {#createDateRangeQuery-java.util.Date-java.util.Date-}
```
public static SearchQuery createDateRangeQuery(Date start, Date end)
```


日付範囲クエリを作成します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 開始 | java.util.Date | 範囲の開始値です。 |
|
|  | 終了 | java.util.Date | 範囲の終了値です。 |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A date range query.

### createPhraseSearchQuery(SearchQuery[] queries) {#createPhraseSearchQuery-com.groupdocs.search.SearchQuery...-}
```
public static SearchQuery createPhraseSearchQuery(SearchQuery[] queries)
```


フレーズ検索クエリを作成します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | queries | [SearchQuery\[\]](../../com.groupdocs.search/searchquery) | 子クエリです。 |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A phrase search query.

### createAndQuery(SearchQuery[] queries) {#createAndQuery-com.groupdocs.search.SearchQuery---}
```
public static SearchQuery createAndQuery(SearchQuery[] queries)
```


元の各クエリで見つかるドキュメントのみを検索する結合クエリを作成します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | queries | [SearchQuery\[\]](../../com.groupdocs.search/searchquery) | 検索対象のフィールド名です。 |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined AND query.

### createFieldQuery(String fieldName, SearchQuery query) {#createFieldQuery-java.lang.String-com.groupdocs.search.SearchQuery-}
```
public static SearchQuery createFieldQuery(String fieldName, SearchQuery query)
```


指定されたクエリにフィールドを追加します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | fieldName | java.lang.String | 検索対象のフィールド名です。 |
|
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | フィールドを追加するクエリです。 |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A query with the field to search in.

### createNotQuery(SearchQuery query) {#createNotQuery-com.groupdocs.search.SearchQuery-}
```
public static SearchQuery createNotQuery(SearchQuery query)
```


元のクエリで見つかるドキュメントに対して、インデックス内の残りのドキュメントを検索する反転クエリを作成します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | 反転させるクエリです。 |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined NOT query.

### createAndQuery(SearchQuery leftQuery, SearchQuery rightQuery) {#createAndQuery-com.groupdocs.search.SearchQuery-com.groupdocs.search.SearchQuery-}
```
public static SearchQuery createAndQuery(SearchQuery leftQuery, SearchQuery rightQuery)
```


元の各クエリで見つかるドキュメントのみを検索する結合クエリを作成します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | leftQuery | [SearchQuery](../../com.groupdocs.search/searchquery) | 左側の子クエリです。 |
|
|  | rightQuery | [SearchQuery](../../com.groupdocs.search/searchquery) | 右側の子クエリです。 |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined AND query.

### createOrQuery(SearchQuery leftQuery, SearchQuery rightQuery) {#createOrQuery-com.groupdocs.search.SearchQuery-com.groupdocs.search.SearchQuery-}
```
public static SearchQuery createOrQuery(SearchQuery leftQuery, SearchQuery rightQuery)
```


元のクエリのいずれかで少なくとも1つ見つかるすべてのドキュメントを検索する結合クエリを作成します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | leftQuery | [SearchQuery](../../com.groupdocs.search/searchquery) | 左側の子クエリです。 |
|
|  | rightQuery | [SearchQuery](../../com.groupdocs.search/searchquery) | 右側の子クエリです。 |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined OR query.

### createOrQuery(SearchQuery[] queries) {#createOrQuery-com.groupdocs.search.SearchQuery---}
```
public static SearchQuery createOrQuery(SearchQuery[] queries)
```


元のクエリのいずれかで少なくとも1つ見つかるすべてのドキュメントを検索する結合クエリを作成します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | queries | [SearchQuery\[\]](../../com.groupdocs.search/searchquery) | 子クエリです。 |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined OR query.

### createWildcardQuery(int count) {#createWildcardQuery-int-}
```
public static SearchQuery createWildcardQuery(int count)
```


フレーズ検索用のワイルドカードを作成します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | カウント | int | ワイルドカード内の単語数。 |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A wildcard for the phrase search.

### createWildcardQuery(int minCount, int maxCount) {#createWildcardQuery-int-int-}
```
public static SearchQuery createWildcardQuery(int minCount, int maxCount)
```


フレーズ検索用のワイルドカードを作成します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | minCount | int | ワイルドカード内の最小単語数。 |
|
|  | maxCount | int | ワイルドカード内の最大単語数。 |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A wildcard for the phrase search.

