---
title: "ImageSearchOptions"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "逆画像検索操作のオプションを提供します。"
type: docs
weight: 24
url: /ja/java/com.groupdocs.search.options/imagesearchoptions/
---
**Inheritance:**
java.lang.Object
```
public class ImageSearchOptions
```

逆画像検索操作のオプションを提供します。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [ImageSearchOptions()](#ImageSearchOptions--) | ImageSearchOptions クラスの新しいインスタンスを初期化します。 |
|
|  | [ImageSearchOptions(Object data)](#ImageSearchOptions-java.lang.Object-) | ImageSearchOptions クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getHashDifferences()](#getHashDifferences--) | 画像ハッシュの不一致ビットの最大数を取得します。 |
|
|  | [setHashDifferences(int value)](#setHashDifferences-int-) | 画像ハッシュの不一致ビットの最大数を設定します。 |
|
|  | [getMaxResultCount()](#getMaxResultCount--) | 画像逆検索リクエストで見つかった画像の最大数を取得します。 |
|
|  | [setMaxResultCount(int value)](#setMaxResultCount-int-) | 画像逆検索リクエストで見つかった画像の最大数を設定します。 |
|
|  | [getSearchDocumentFilter()](#getSearchDocumentFilter--) | 検索ドキュメントフィルターを取得します。 |
|
|  | [setSearchDocumentFilter(ISearchDocumentFilter value)](#setSearchDocumentFilter-com.groupdocs.search.options.ISearchDocumentFilter-) | 検索ドキュメントフィルターを取得または設定します。 |
|
| [getCore()](#getCore--) |  |
### ImageSearchOptions() {#ImageSearchOptions--}
```
public ImageSearchOptions()
```


ImageSearchOptions クラスの新しいインスタンスを初期化します。


### ImageSearchOptions(Object data) {#ImageSearchOptions-java.lang.Object-}
```
public ImageSearchOptions(Object data)
```


ImageSearchOptions クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | データ | java.lang.Object | シリアライズされたデータ。 |
|

### getHashDifferences() {#getHashDifferences--}
```
public int getHashDifferences()
```


画像ハッシュの不一致ビットの最大数を取得します。デフォルト値は 5 です。


**Returns:**
int - 画像ハッシュの不一致ビットの最大数。

### setHashDifferences(int value) {#setHashDifferences-int-}
```
public void setHashDifferences(int value)
```


画像ハッシュの不一致ビットの最大数を設定します。デフォルト値は 5 です。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 値 | int | 画像ハッシュの不一致ビットの最大数。 |
|

### getMaxResultCount() {#getMaxResultCount--}
```
public int getMaxResultCount()
```


画像逆検索リクエストで見つかった画像の最大数を取得します。デフォルト値は 1000 です。


**Returns:**
int - 画像逆検索リクエストで見つかった画像の最大数。

### setMaxResultCount(int value) {#setMaxResultCount-int-}
```
public void setMaxResultCount(int value)
```


画像逆検索リクエストで見つかった画像の最大数を設定します。デフォルト値は 1000 です。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 値 | int | 画像逆検索リクエストで見つかった画像の最大数。 |
|

### getSearchDocumentFilter() {#getSearchDocumentFilter--}
```
public ISearchDocumentFilter getSearchDocumentFilter()
```


検索ドキュメントフィルターを取得します。SearchDocumentFilter は包含ロジックで動作します。検索ドキュメントフィルター インスタンスの作成には GroupDocs.Search.Options.SearchDocumentFilter クラスを使用します。デフォルト値は null で、すべての見つかったドキュメントが返されます。


**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - The search document filter.

### setSearchDocumentFilter(ISearchDocumentFilter value) {#setSearchDocumentFilter-com.groupdocs.search.options.ISearchDocumentFilter-}
```
public void setSearchDocumentFilter(ISearchDocumentFilter value)
```


検索ドキュメントフィルターを取得または設定します。SearchDocumentFilter は包含ロジックで動作します。検索ドキュメントフィルター インスタンスの作成には GroupDocs.Search.Options.SearchDocumentFilter クラスを使用します。デフォルト値は null で、すべての見つかったドキュメントが返されます。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | value | [ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) | 検索ドキュメントフィルター。 |
|

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
