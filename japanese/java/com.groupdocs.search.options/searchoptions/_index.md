---
title: "SearchOptions"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "検索操作のオプションを提供します。"
type: docs
weight: 34
url: /ja/java/com.groupdocs.search.options/searchoptions/
---
**Inheritance:**
java.lang.Object
```
public class SearchOptions
```

検索操作のオプションを提供します。


**Learn more**

* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [SearchOptions()](#SearchOptions--) | SearchOptions クラスの新しいインスタンスを初期化します。 |
|
|  | [SearchOptions(Object data)](#SearchOptions-java.lang.Object-) | SearchOptions クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getUseSynonymSearch()](#getUseSynonymSearch--) | 検索で同義語を使用するフラグを取得します。 |
|
|  | [setUseSynonymSearch(boolean value)](#setUseSynonymSearch-boolean-) | 検索で同義語を使用するフラグを設定します。 |
|
|  | [getUseHomophoneSearch()](#getUseHomophoneSearch--) | 検索で同音異義語を使用するフラグを取得します。 |
|
|  | [setUseHomophoneSearch(boolean value)](#setUseHomophoneSearch-boolean-) | 検索で同音異義語を使用するフラグを設定します。 |
|
|  | [getUseWordFormsSearch()](#getUseWordFormsSearch--) | 検索で異なる語形を使用するフラグを取得します。 |
|
|  | [setUseWordFormsSearch(boolean value)](#setUseWordFormsSearch-boolean-) | 検索で異なる語形を使用するフラグを設定します。 |
|
|  | [getRetrieveAttributes()](#getRetrieveAttributes--) | 見つかったドキュメントに関連付けられた属性を取得するフラグを取得します。 |
|
|  | [setRetrieveAttributes(boolean value)](#setRetrieveAttributes-boolean-) | 見つかったドキュメントに関連付けられた属性を取得するフラグを設定します。 |
|
|  | [getFuzzySearch()](#getFuzzySearch--) | ファジー検索オプションを取得します。 |
|
|  | [getSpellingCorrector()](#getSpellingCorrector--) | スペル補正オプションを取得します。 |
|
|  | [getKeyboardLayoutCorrector()](#getKeyboardLayoutCorrector--) | キーボードレイアウト補正オプションを取得します。 |
|
|  | [getUseCaseSensitiveSearch()](#getUseCaseSensitiveSearch--) | 大文字と小文字を区別する検索のフラグを取得します。 |
|
|  | [setUseCaseSensitiveSearch(boolean value)](#setUseCaseSensitiveSearch-boolean-) | 大文字と小文字を区別する検索のフラグを設定します。 |
|
|  | [getMaxTotalOccurrenceCount()](#getMaxTotalOccurrenceCount--) | 検索クエリ内のすべての語句の出現回数の合計最大数を取得します。 |
|
|  | [setMaxTotalOccurrenceCount(int value)](#setMaxTotalOccurrenceCount-int-) | 検索クエリ内のすべての語句の出現回数の合計の最大値を設定します。 |
|
|  | [getMaxOccurrenceCountPerTerm()](#getMaxOccurrenceCountPerTerm--) | 検索クエリ内の各語句の出現回数の最大数を取得します。 |
|
|  | [setMaxOccurrenceCountPerTerm(int value)](#setMaxOccurrenceCountPerTerm-int-) | 検索クエリ内の各語句の出現回数の最大数を設定します。 |
|
|  | [getDateFormats()](#getDateFormats--) | 日付範囲検索用の日付形式のコレクションを取得します。 |
|
|  | [isChunkSearch()](#isChunkSearch--) | チャンク単位で検索するフラグを取得します。 |
|
|  | [setChunkSearch(boolean value)](#setChunkSearch-boolean-) | チャンク単位で検索するフラグを設定します。 |
|
|  | [getSearchDocumentFilter()](#getSearchDocumentFilter--) | 検索ドキュメントフィルターを取得します。 |
|
|  | [setSearchDocumentFilter(ISearchDocumentFilter value)](#setSearchDocumentFilter-com.groupdocs.search.options.ISearchDocumentFilter-) | 検索ドキュメントフィルタを設定します。 |
|
|  | [getCancellation()](#getCancellation--) | 操作のキャンセルオブジェクトを取得します。 |
|
|  | [setCancellation(Cancellation value)](#setCancellation-com.groupdocs.search.common.Cancellation-) | 操作のキャンセルオブジェクトを設定します。 |
|
| [getCore()](#getCore--) |  |
### SearchOptions() {#SearchOptions--}
```
public SearchOptions()
```


SearchOptions クラスの新しいインスタンスを初期化します。


### SearchOptions(Object data) {#SearchOptions-java.lang.Object-}
```
public SearchOptions(Object data)
```


SearchOptions クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | データ | java.lang.Object | シリアライズされたデータ。 |
|

### getUseSynonymSearch() {#getUseSynonymSearch--}
```
public boolean getUseSynonymSearch()
```


検索で同義語を使用するフラグを取得します。デフォルト値は  false です。


**Returns:**
boolean - 検索で同義語を使用するフラグです。

### setUseSynonymSearch(boolean value) {#setUseSynonymSearch-boolean-}
```
public void setUseSynonymSearch(boolean value)
```


検索で同義語を使用するフラグを設定します。デフォルト値は  false です。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 値 | boolean | 検索で同義語を使用するフラグです。 |
|

### getUseHomophoneSearch() {#getUseHomophoneSearch--}
```
public boolean getUseHomophoneSearch()
```


検索で同音異義語を使用するフラグを取得します。デフォルト値は  false です。


**Returns:**
boolean - 検索で同音異義語を使用するフラグです。

### setUseHomophoneSearch(boolean value) {#setUseHomophoneSearch-boolean-}
```
public void setUseHomophoneSearch(boolean value)
```


検索で同音異義語を使用するフラグを設定します。デフォルト値は  false です。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 値 | boolean | 検索で同音異義語を使用するフラグです。 |
|

### getUseWordFormsSearch() {#getUseWordFormsSearch--}
```
public boolean getUseWordFormsSearch()
```


検索で異なる語形を使用するフラグを取得します。デフォルト値は  false です。


**Returns:**
boolean - 検索で異なる語形を使用するフラグです。

### setUseWordFormsSearch(boolean value) {#setUseWordFormsSearch-boolean-}
```
public void setUseWordFormsSearch(boolean value)
```


検索で異なる語形を使用するフラグを設定します。デフォルト値は  false です。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 値 | boolean | 検索で異なる語形を使用するフラグです。 |
|

### getRetrieveAttributes() {#getRetrieveAttributes--}
```
public boolean getRetrieveAttributes()
```


見つかったドキュメントに関連付けられた属性を取得するフラグを取得します。デフォルト値は  false です。


**Returns:**
boolean - 見つかったドキュメントに関連付けられた属性を取得するフラグです。

### setRetrieveAttributes(boolean value) {#setRetrieveAttributes-boolean-}
```
public void setRetrieveAttributes(boolean value)
```


見つかったドキュメントに関連付けられた属性を取得するフラグを設定します。デフォルト値は  false です。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 値 | boolean | 見つかったドキュメントに関連付けられた属性を取得するフラグです。 |
|

### getFuzzySearch() {#getFuzzySearch--}
```
public FuzzySearchOptions getFuzzySearch()
```


ファジー検索オプションを取得します。


**Returns:**
[FuzzySearchOptions](../../com.groupdocs.search.options/fuzzysearchoptions) - The fuzzy search options.

### getSpellingCorrector() {#getSpellingCorrector--}
```
public SpellingCorrectorOptions getSpellingCorrector()
```


スペル補正オプションを取得します。


**Returns:**
[SpellingCorrectorOptions](../../com.groupdocs.search.options/spellingcorrectoroptions) - The spelling corrector options.

### getKeyboardLayoutCorrector() {#getKeyboardLayoutCorrector--}
```
public KeyboardLayoutCorrectorOptions getKeyboardLayoutCorrector()
```


キーボードレイアウト補正オプションを取得します。


**Returns:**
[KeyboardLayoutCorrectorOptions](../../com.groupdocs.search.options/keyboardlayoutcorrectoroptions) - The keyboard layout corrector options.

### getUseCaseSensitiveSearch() {#getUseCaseSensitiveSearch--}
```
public boolean getUseCaseSensitiveSearch()
```


大文字と小文字を区別する検索のフラグを取得します。デフォルト値は  false です。


**Returns:**
boolean - 大文字と小文字を区別する検索のフラグです。

### setUseCaseSensitiveSearch(boolean value) {#setUseCaseSensitiveSearch-boolean-}
```
public void setUseCaseSensitiveSearch(boolean value)
```


ケースセンシティブ検索のフラグを設定します。デフォルト値は false です。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 値 | boolean | ケースセンシティブ検索のフラグ。 |
|

### getMaxTotalOccurrenceCount() {#getMaxTotalOccurrenceCount--}
```
public int getMaxTotalOccurrenceCount()
```


検索クエリ内のすべての語句の最大総出現回数を取得します。デフォルト値は 500000 です。


**Returns:**
int - 最大総出現回数。

### setMaxTotalOccurrenceCount(int value) {#setMaxTotalOccurrenceCount-int-}
```
public void setMaxTotalOccurrenceCount(int value)
```


検索クエリ内のすべての語句の最大総出現回数を設定します。デフォルト値は 500000 です。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 値 | int | 最大総出現回数。 |
|

### getMaxOccurrenceCountPerTerm() {#getMaxOccurrenceCountPerTerm--}
```
public int getMaxOccurrenceCountPerTerm()
```


検索クエリ内の各語句の最大出現回数を取得します。デフォルト値は 100000 です。


**Returns:**
int - 各語句の最大出現回数。

### setMaxOccurrenceCountPerTerm(int value) {#setMaxOccurrenceCountPerTerm-int-}
```
public void setMaxOccurrenceCountPerTerm(int value)
```


検索クエリ内の各語句の最大出現回数を設定します。デフォルト値は 100000 です。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 値 | int | 各語句の最大出現回数。 |
|

### getDateFormats() {#getDateFormats--}
```
public DateFormatCollection getDateFormats()
```


日付範囲検索用の日付形式コレクションを取得します。デフォルトの日付形式は 'dd.MM.yyyy'、'MM/dd/yyyy'、'yyyy-MM-dd' です。


**Returns:**
[DateFormatCollection](../../com.groupdocs.search.options/dateformatcollection) - The collection of date formats for date range search.


この例は検索用の日付形式の設定方法を示しています。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // 指定されたフォルダーにインデックスを作成しています
index.add(documentsFolder); // 指定されたフォルダーからドキュメントをインデックス化しています
SearchOptions options = new SearchOptions();
options.getDateFormats().clear(); // デフォルトの日付形式を削除
DateFormatElement[] elements = new DateFormatElement[] {
DateFormatElement.getMonthTwoDigits(),
DateFormatElement.getDayOfMonthTwoDigits(),
DateFormatElement.getYearFourDigits(),
};
// 'MM/dd/yyyy' の日付フォーマットパターンを作成
com.groupdocs.search.DateFormat dateFormat = new com.groupdocs.search.DateFormat(elements, "/");
options.getDateFormats().addItem(dateFormat);
SearchResult result = index.search(query, options); // インデックス内を検索
 
```
 
````


### isChunkSearch() {#isChunkSearch--}
```
public boolean isChunkSearch()
```


チャンク単位検索のフラグを取得します。デフォルト値は false です。


**Returns:**
boolean - チャンク単位検索のフラグ。

### setChunkSearch(boolean value) {#setChunkSearch-boolean-}
```
public void setChunkSearch(boolean value)
```


チャンク単位検索のフラグを設定します。デフォルト値は false です。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 値 | boolean | チャンク単位検索のフラグ。 |
|

### getSearchDocumentFilter() {#getSearchDocumentFilter--}
```
public ISearchDocumentFilter getSearchDocumentFilter()
```


検索ドキュメントフィルタを取得します。SearchDocumentFilter は包含ロジックで動作します。検索ドキュメントフィルタインスタンスの作成には SearchDocumentFilter クラスを使用してください。デフォルト値は null で、これはすべての見つかったドキュメントが返されることを意味します。


**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - The search document filter.


この例はドキュメントフィルタの設定方法を示しています。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments1\\";
// 指定されたフォルダーにインデックスを作成しています
Index index = new Index(indexFolder);
// ドキュメントをインデックスしています
index.add(documentsFolder);
// 拡張子が '.doc'、'.docx'、'.rtf' のドキュメントをスキップする検索ドキュメントフィルタを作成しています
SearchOptions options = new SearchOptions();
ISearchDocumentFilter fileExtensionFilter = SearchDocumentFilter.createFileExtension(".doc", ".docx", ".rtf"); // ファイル拡張子フィルタを作成
ISearchDocumentFilter invertedFilter = SearchDocumentFilter.createNot(fileExtensionFilter); // ファイル拡張子フィルタを反転
options.setSearchDocumentFilter(invertedFilter);
// インデックス内を検索
SearchResult result = index.search("Einstein", options);
 
```
 
````


### setSearchDocumentFilter(ISearchDocumentFilter value) {#setSearchDocumentFilter-com.groupdocs.search.options.ISearchDocumentFilter-}
```
public void setSearchDocumentFilter(ISearchDocumentFilter value)
```


検索ドキュメントフィルタを設定します。SearchDocumentFilter は包含ロジックで動作します。検索ドキュメントフィルタインスタンスの作成には SearchDocumentFilter クラスを使用してください。デフォルト値は null で、これはすべての見つかったドキュメントが返されることを意味します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | value | [ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) | 検索ドキュメントフィルター。 |


この例はドキュメントフィルタの設定方法を示しています。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments1\\";
// 指定されたフォルダーにインデックスを作成しています
Index index = new Index(indexFolder);
// ドキュメントをインデックスしています
index.add(documentsFolder);
// 拡張子が '.doc'、'.docx'、'.rtf' のドキュメントをスキップする検索ドキュメントフィルタを作成しています
SearchOptions options = new SearchOptions();
ISearchDocumentFilter fileExtensionFilter = SearchDocumentFilter.createFileExtension(".doc", ".docx", ".rtf"); // ファイル拡張子フィルタを作成
ISearchDocumentFilter invertedFilter = SearchDocumentFilter.createNot(fileExtensionFilter); // ファイル拡張子フィルタを反転
options.setSearchDocumentFilter(invertedFilter);
// インデックス内を検索
SearchResult result = index.search("Einstein", options);
 
```
 
````

|

### getCancellation() {#getCancellation--}
```
public Cancellation getCancellation()
```


操作のキャンセルオブジェクトを取得します。デフォルト値は null です。


**Returns:**
[Cancellation](../../com.groupdocs.search.common/cancellation) - The operation cancellation object.

### setCancellation(Cancellation value) {#setCancellation-com.groupdocs.search.common.Cancellation-}
```
public void setCancellation(Cancellation value)
```


操作のキャンセルオブジェクトを設定します。デフォルト値は null です。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | value | [Cancellation](../../com.groupdocs.search.common/cancellation) | 操作のキャンセルオブジェクト。 |
|

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
