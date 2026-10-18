---
title: "Searcher"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "検索ネットワークのシャードへの検索クエリを管理するサービスを表します。"
type: docs
weight: 12
url: /ja/java/com.groupdocs.search.scaling/searcher/
---
**Inheritance:**
java.lang.Object
```
public abstract class Searcher
```

検索ネットワークのシャードへの検索クエリを管理するサービスを表します。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [Searcher()](#Searcher--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [searchFirst(String query, SearchOptions options)](#searchFirst-java.lang.String-com.groupdocs.search.options.SearchOptions-) | 分散検索インデックスでテキスト形式のクエリを使用して検索を開始します。 |
|
|  | [searchFirst(SearchQuery query, SearchOptions options)](#searchFirst-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-) | 分散検索インデックスで検索を開始します。 |
|
|  | [searchFirst(SearchImage image, ImageSearchOptions options)](#searchFirst-com.groupdocs.search.common.SearchImage-com.groupdocs.search.options.ImageSearchOptions-) | 分散検索インデックスで逆画像検索を実行します。 |
|
|  | [searchNext(NetworkSearchToken networkSearchToken)](#searchNext-com.groupdocs.search.scaling.results.NetworkSearchToken-) | 分散検索インデックスで検索を継続します。 |
|
|  | [searchNext(NetworkImageSearchToken networkImageSearchToken)](#searchNext-com.groupdocs.search.scaling.results.NetworkImageSearchToken-) | 分散検索インデックスで逆画像検索を継続します。 |
|
|  | [highlight(NetworkFoundDocument document, Highlighter highlighter, HighlightOptions options)](#highlight-com.groupdocs.search.scaling.results.NetworkFoundDocument-com.groupdocs.search.highlighters.Highlighter-com.groupdocs.search.options.HighlightOptions-) | 見つかった用語をハイライトしたHTML形式のテキストを生成します。 |
|
|  | [getIndexedDocuments(int shardIndex)](#getIndexedDocuments-int-) | すべてのインデックス化されたドキュメントの配列を取得します。 |
|
|  | [getIndexedDocumentItems(NetworkDocumentInfo documentInfo)](#getIndexedDocumentItems-com.groupdocs.search.scaling.results.NetworkDocumentInfo-) | 指定されたドキュメントのネストされた項目の配列を取得します（ZIP、OST、PST などのコンテナドキュメント用）。 |
|
|  | [getDocumentText(NetworkDocumentInfo documentInfo, OutputAdapter adapter)](#getDocumentText-com.groupdocs.search.scaling.results.NetworkDocumentInfo-com.groupdocs.search.common.OutputAdapter-) | インデックス化されたドキュメントのテキストを生成し、出力アダプターを介して渡します。 |
|
### Searcher() {#Searcher--}
```
public Searcher()
```


### searchFirst(String query, SearchOptions options) {#searchFirst-java.lang.String-com.groupdocs.search.options.SearchOptions-}
```
public abstract NetworkSearchResult searchFirst(String query, SearchOptions options)
```


分散検索インデックスでテキスト形式のクエリを使用して検索を開始します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | query | java.lang.String | 検索クエリです。 |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | 検索オプションです。 |
|

**Returns:**
[NetworkSearchResult](../../com.groupdocs.search.scaling.results/networksearchresult) - The search result.

### searchFirst(SearchQuery query, SearchOptions options) {#searchFirst-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-}
```
public abstract NetworkSearchResult searchFirst(SearchQuery query, SearchOptions options)
```


分散検索インデックスで検索を開始します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | 検索クエリです。 |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | 検索オプションです。 |
|

**Returns:**
[NetworkSearchResult](../../com.groupdocs.search.scaling.results/networksearchresult) - The search result.

### searchFirst(SearchImage image, ImageSearchOptions options) {#searchFirst-com.groupdocs.search.common.SearchImage-com.groupdocs.search.options.ImageSearchOptions-}
```
public abstract NetworkImageSearchResult searchFirst(SearchImage image, ImageSearchOptions options)
```


分散検索インデックスで逆画像検索を実行します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | image | [SearchImage](../../com.groupdocs.search.common/searchimage) | 検索する画像。 |
|
|  | options | [ImageSearchOptions](../../com.groupdocs.search.options/imagesearchoptions) | 画像検索オプション。 |
|

**Returns:**
[NetworkImageSearchResult](../../com.groupdocs.search.scaling.results/networkimagesearchresult) - The reverse image search result.

### searchNext(NetworkSearchToken networkSearchToken) {#searchNext-com.groupdocs.search.scaling.results.NetworkSearchToken-}
```
public abstract NetworkSearchResult searchNext(NetworkSearchToken networkSearchToken)
```


分散検索インデックスで検索を継続します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | networkSearchToken | [NetworkSearchToken](../../com.groupdocs.search.scaling.results/networksearchtoken) | ネットワーク検索トークン。 |
|

**Returns:**
[NetworkSearchResult](../../com.groupdocs.search.scaling.results/networksearchresult) - The search result.

### searchNext(NetworkImageSearchToken networkImageSearchToken) {#searchNext-com.groupdocs.search.scaling.results.NetworkImageSearchToken-}
```
public abstract NetworkImageSearchResult searchNext(NetworkImageSearchToken networkImageSearchToken)
```


分散検索インデックスで逆画像検索を継続します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | networkImageSearchToken | [NetworkImageSearchToken](../../com.groupdocs.search.scaling.results/networkimagesearchtoken) | ネットワーク画像検索トークン。 |
|

**Returns:**
[NetworkImageSearchResult](../../com.groupdocs.search.scaling.results/networkimagesearchresult) - The reverse image search result.

### highlight(NetworkFoundDocument document, Highlighter highlighter, HighlightOptions options) {#highlight-com.groupdocs.search.scaling.results.NetworkFoundDocument-com.groupdocs.search.highlighters.Highlighter-com.groupdocs.search.options.HighlightOptions-}
```
public abstract void highlight(NetworkFoundDocument document, Highlighter highlighter, HighlightOptions options)
```


見つかった用語をハイライトしたHTML形式のテキストを生成します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | document | [NetworkFoundDocument](../../com.groupdocs.search.scaling.results/networkfounddocument) | 見つかったドキュメントです。 |
|
|  | highlighter | [Highlighter](../../com.groupdocs.search.highlighters/highlighter) | 検索結果ハイライト表示です。 |
|
|  | options | [HighlightOptions](../../com.groupdocs.search.options/highlightoptions) | ハイライトオプションです。 |
|

### getIndexedDocuments(int shardIndex) {#getIndexedDocuments-int-}
```
public abstract NetworkDocumentInfo[] getIndexedDocuments(int shardIndex)
```


すべてのインデックス化されたドキュメントの配列を取得します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | shardIndex | int | シャードインデックス。 |
|

**Returns:**
com.groupdocs.search.scaling.results.NetworkDocumentInfo[] - すべてのインデックスされたドキュメントの配列。

### getIndexedDocumentItems(NetworkDocumentInfo documentInfo) {#getIndexedDocumentItems-com.groupdocs.search.scaling.results.NetworkDocumentInfo-}
```
public abstract NetworkDocumentInfo[] getIndexedDocumentItems(NetworkDocumentInfo documentInfo)
```


指定されたドキュメントのネストされた項目の配列を取得します（ZIP、OST、PST などのコンテナドキュメント用）。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | documentInfo | [NetworkDocumentInfo](../../com.groupdocs.search.scaling.results/networkdocumentinfo) | ドキュメント情報。 |
|

**Returns:**
com.groupdocs.search.scaling.results.NetworkDocumentInfo[] - ドキュメント項目の配列。

### getDocumentText(NetworkDocumentInfo documentInfo, OutputAdapter adapter) {#getDocumentText-com.groupdocs.search.scaling.results.NetworkDocumentInfo-com.groupdocs.search.common.OutputAdapter-}
```
public abstract void getDocumentText(NetworkDocumentInfo documentInfo, OutputAdapter adapter)
```


インデックス化されたドキュメントのテキストを生成し、出力アダプターを介して渡します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | documentInfo | [NetworkDocumentInfo](../../com.groupdocs.search.scaling.results/networkdocumentinfo) | インデックス化されたドキュメント情報です。 |
|
|  | adapter | [OutputAdapter](../../com.groupdocs.search.common/outputadapter) | 出力アダプターです。 |
|

