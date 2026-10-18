---
title: "IndexSettings"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "インデックス作成操作をカスタマイズできるインデックス設定を表します。"
type: docs
weight: 19
url: /ja/java/com.groupdocs.search/indexsettings/
---
**Inheritance:**
java.lang.Object
```
public class IndexSettings
```

インデックス作成操作をカスタマイズできるインデックス設定を表します。


**Learn more**

* [Search index settings](../https://docs.groupdocs.com/display/searchjava/Search+index+settings)


この例はクラスの典型的な使用方法を示しています。

````
 ```

String indexFolder = "c:\\MyIndex\\";
IndexSettings settings = new IndexSettings();
settings.setIndexType(IndexType.CompactIndex); // インデックスのタイプを設定しています
Index index = new Index(indexFolder, settings); // インデックスを作成しています
 
```
 
````


## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [IndexSettings()](#IndexSettings--) | IndexSettings クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getInMemoryIndex()](#getInMemoryIndex--) | インデックスがメモリ上に保存されているかディスク上に保存されているかを示す値を取得します。 |
|
|  | [getUseStopWords()](#getUseStopWords--) | ストップワードを使用するかどうかを示す値を取得します。 |
|
|  | [setUseStopWords(boolean value)](#setUseStopWords-boolean-) | ストップワードを使用するかどうかを示す値を設定します。 |
|
|  | [getMaxIndexingReportCount()](#getMaxIndexingReportCount--) | インデックス作成レポートの最大数を取得します。 |
|
|  | [setMaxIndexingReportCount(int value)](#setMaxIndexingReportCount-int-) | インデックス作成レポートの最大数を設定します。 |
|
|  | [getMaxSearchReportCount()](#getMaxSearchReportCount--) | 検索レポートの最大数を取得します。 |
|
|  | [setMaxSearchReportCount(int value)](#setMaxSearchReportCount-int-) | 検索レポートの最大数を設定します。 |
|
|  | [getUseCharacterReplacements()](#getUseCharacterReplacements--) | 文字置換を使用するかどうかを示す値を取得します。 |
|
|  | [setUseCharacterReplacements(boolean value)](#setUseCharacterReplacements-boolean-) | 文字置換を使用するかどうかを示す値を設定します。 |
|
|  | [getDocumentFilter()](#getDocumentFilter--) | ドキュメントフィルタを取得します。 |
|
|  | [setDocumentFilter(DocumentFilter value)](#setDocumentFilter-com.groupdocs.search.DocumentFilter-) | ドキュメントフィルタを設定します。 |
|
|  | [getTextStorageSettings()](#getTextStorageSettings--) | テキストストレージ設定を取得します。 |
|
|  | [setTextStorageSettings(TextStorageSettings value)](#setTextStorageSettings-com.groupdocs.search.options.TextStorageSettings-) | テキストストレージ設定を設定します。 |
|
|  | [getIndexType()](#getIndexType--) | インデックスタイプを取得します。 |
|
|  | [setIndexType(IndexType value)](#setIndexType-com.groupdocs.search.options.IndexType-) | インデックスタイプを設定します。 |
|
|  | [getSearchThreads()](#getSearchThreads--) | 検索に使用されるスレッド数を取得します。 |
|
|  | [setSearchThreads(NumberOfThreads value)](#setSearchThreads-com.groupdocs.search.options.NumberOfThreads-) | 検索に使用されるスレッド数を設定します。 |
|
|  | [getCustomExtractors()](#getCustomExtractors--) | カスタム抽出器コレクションを取得します。 |
|
|  | [getLogger()](#getLogger--) | インデックス内のイベントとエラーのログ記録に使用されるロガーを取得します。 |
|
|  | [setLogger(ILogger value)](#setLogger-com.groupdocs.search.common.ILogger-) | インデックス内のイベントとエラーのログ記録に使用されるロガーを設定します。 |
|
### IndexSettings() {#IndexSettings--}
```
public IndexSettings()
```


IndexSettings クラスの新しいインスタンスを初期化します。


### getInMemoryIndex() {#getInMemoryIndex--}
```
public final boolean getInMemoryIndex()
```


インデックスがメモリ上に保存されているかディスク上に保存されているかを示す値を取得します。


**Returns:**
boolean - インデックスがメモリ上に保存されているかディスク上に保存されているかを示す値。

### getUseStopWords() {#getUseStopWords--}
```
public final boolean getUseStopWords()
```


ストップワードを使用するかどうかを示す値を取得します。デフォルト値は true です。


**Returns:**
boolean - ストップワードを使用するかどうかを示す値です。

### setUseStopWords(boolean value) {#setUseStopWords-boolean-}
```
public final void setUseStopWords(boolean value)
```


ストップワードを使用するかどうかを示す値を設定します。デフォルト値は true です。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 値 | boolean | ストップワードを使用するかどうかを示す値です。 |
|

### getMaxIndexingReportCount() {#getMaxIndexingReportCount--}
```
public final int getMaxIndexingReportCount()
```


インデックス作成レポートの最大数を取得します。デフォルト値は 5 です。


**Returns:**
int - インデックス作成レポートの最大数です。

### setMaxIndexingReportCount(int value) {#setMaxIndexingReportCount-int-}
```
public final void setMaxIndexingReportCount(int value)
```


インデックス作成レポートの最大数を設定します。デフォルト値は 5 です。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 値 | int | インデックス作成レポートの最大数です。 |
|

### getMaxSearchReportCount() {#getMaxSearchReportCount--}
```
public final int getMaxSearchReportCount()
```


検索レポートの最大数を取得します。デフォルト値は 10 です。


**Returns:**
int - 検索レポートの最大数です。

### setMaxSearchReportCount(int value) {#setMaxSearchReportCount-int-}
```
public final void setMaxSearchReportCount(int value)
```


検索レポートの最大数を設定します。デフォルト値は 10 です。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 値 | int | 検索レポートの最大数です。 |
|

### getUseCharacterReplacements() {#getUseCharacterReplacements--}
```
public final boolean getUseCharacterReplacements()
```


文字置換を使用するかどうかを示す値を取得します。デフォルト値は false です。


**Returns:**
boolean - 文字置換を使用するかどうかを示す値です。

### setUseCharacterReplacements(boolean value) {#setUseCharacterReplacements-boolean-}
```
public final void setUseCharacterReplacements(boolean value)
```


文字置換を使用するかどうかを示す値を設定します。デフォルト値は false です。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 値 | boolean | 文字置換を使用するかどうかを示す値です。 |
|

### getDocumentFilter() {#getDocumentFilter--}
```
public final DocumentFilter getDocumentFilter()
```


ドキュメントフィルタを取得します。DocumentFilter は包含ロジックで動作します。ドキュメントフィルタインスタンスを作成するには DocumentFilter クラスを使用してください。デフォルト値は null で、これは追加されたすべてのドキュメントがインデックスされることを意味します。


**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - The document filter.

この例はドキュメントフィルタの設定方法を示しています。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// 拡張子が '.doc', '.docx', '.rtf' のドキュメントをスキップするフィルタを作成しています
IndexSettings settings = new IndexSettings();
DocumentFilter fileExtensionFilter = DocumentFilter.createFileExtension(".doc", ".docx", ".rtf"); // ファイル拡張子フィルタを作成しています
DocumentFilter invertedFilter = DocumentFilter.createNot(fileExtensionFilter); // ファイル拡張子フィルタを反転しています
settings.setDocumentFilter(invertedFilter);
// 指定されたフォルダーにインデックスを作成しています
Index index = new Index(indexFolder, settings);
// ドキュメントをインデックスしています
index.add(documentsFolder);
// 検索
SearchResult result = index.search("Einstein");
 
```
 
````


### setDocumentFilter(DocumentFilter value) {#setDocumentFilter-com.groupdocs.search.DocumentFilter-}
```
public final void setDocumentFilter(DocumentFilter value)
```


ドキュメントフィルタを設定します。  DocumentFilter  は包含ロジックで動作します。  GroupDocs.Search.Options.DocumentFilter  クラスを使用してドキュメントフィルタのインスタンスを作成します。 デフォルト値は  null  で、すべての追加されたドキュメントがインデックスされることを意味します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | value | [DocumentFilter](../../com.groupdocs.search/documentfilter) | ドキュメントフィルタです。 |

この例はドキュメントフィルタの設定方法を示しています。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// 拡張子が '.doc', '.docx', '.rtf' のドキュメントをスキップするフィルタを作成しています
IndexSettings settings = new IndexSettings();
DocumentFilter fileExtensionFilter = DocumentFilter.createFileExtension(".doc", ".docx", ".rtf"); // ファイル拡張子フィルタを作成しています
DocumentFilter invertedFilter = DocumentFilter.createNot(fileExtensionFilter); // ファイル拡張子フィルタを反転しています
settings.setDocumentFilter(invertedFilter);
// 指定されたフォルダーにインデックスを作成しています
Index index = new Index(indexFolder, settings);
// ドキュメントをインデックスしています
index.add(documentsFolder);
// 検索
SearchResult result = index.search("Einstein");
 
```
 
````

|

### getTextStorageSettings() {#getTextStorageSettings--}
```
public final TextStorageSettings getTextStorageSettings()
```


テキストストレージ設定を取得します。 デフォルト値は  null  で、ドキュメントテキストが保存されないことを意味します。


**Returns:**
[TextStorageSettings](../../com.groupdocs.search.options/textstoragesettings) - The text storage settings.

この例はテキストストレージ設定の設定方法を示しています。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// インデックス設定インスタンスの作成
IndexSettings settings = new IndexSettings();
settings.setTextStorageSettings(new TextStorageSettings(Compression.High)); // インデックステキストストレージの高圧縮レベルを設定
// 指定されたフォルダーにインデックスを作成しています
Index index = new Index(indexFolder, settings);
// ドキュメントをインデックスしています
index.add(documentsFolder);
// 検索
SearchResult result = index.search("Einstein");
 
```
 
````


### setTextStorageSettings(TextStorageSettings value) {#setTextStorageSettings-com.groupdocs.search.options.TextStorageSettings-}
```
public final void setTextStorageSettings(TextStorageSettings value)
```


テキストストレージ設定を設定します。 デフォルト値は  null  で、ドキュメントテキストが保存されないことを意味します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | value | [TextStorageSettings](../../com.groupdocs.search.options/textstoragesettings) | テキストストレージ設定です。 |

この例はテキストストレージ設定の設定方法を示しています。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// インデックス設定インスタンスの作成
IndexSettings settings = new IndexSettings();
settings.setTextStorageSettings(new TextStorageSettings(Compression.High)); // インデックステキストストレージの高圧縮レベルを設定
// 指定されたフォルダーにインデックスを作成しています
Index index = new Index(indexFolder, settings);
// ドキュメントをインデックスしています
index.add(documentsFolder);
// 検索
SearchResult result = index.search("Einstein");
 
```
 
````

|

### getIndexType() {#getIndexType--}
```
public final IndexType getIndexType()
```


インデックスタイプを取得します。 デフォルト値は  GroupDocs.Search.Options.IndexType.NormalIndex  です。


**Returns:**
[IndexType](../../com.groupdocs.search.options/indextype) - The index type.

### setIndexType(IndexType value) {#setIndexType-com.groupdocs.search.options.IndexType-}
```
public final void setIndexType(IndexType value)
```


インデックスタイプを設定します。 デフォルト値は  GroupDocs.Search.Options.IndexType.NormalIndex  です。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | value | [IndexType](../../com.groupdocs.search.options/indextype) | インデックスタイプです。 |
|

### getSearchThreads() {#getSearchThreads--}
```
public final NumberOfThreads getSearchThreads()
```


検索に使用されるスレッド数を取得します。 デフォルト値は  GroupDocs.Search.Options.NumberOfThreads.Default  で、検索はプロセッサコア数と同じ数のスレッドで実行されることを意味します。


**Returns:**
[NumberOfThreads](../../com.groupdocs.search.options/numberofthreads) - The number of threads used for the search.

### setSearchThreads(NumberOfThreads value) {#setSearchThreads-com.groupdocs.search.options.NumberOfThreads-}
```
public final void setSearchThreads(NumberOfThreads value)
```


検索に使用されるスレッド数を設定します。 デフォルト値は  GroupDocs.Search.Options.NumberOfThreads.Default  で、検索はプロセッサコア数と同じ数のスレッドで実行されることを意味します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | value | [NumberOfThreads](../../com.groupdocs.search.options/numberofthreads) | 検索に使用されるスレッド数です。 |
|

### getCustomExtractors() {#getCustomExtractors--}
```
public final CustomExtractorCollection getCustomExtractors()
```


カスタムエクストラクタコレクションを取得します。 カスタムエクストラクタの実装例は  GroupDocs.Search.Common.IFieldExtractor  インターフェイスのドキュメントに示されています。


**Returns:**
[CustomExtractorCollection](../../com.groupdocs.search.common/customextractorcollection) - The custom extractor collection.

### getLogger() {#getLogger--}
```
public final ILogger getLogger()
```


インデックス内のイベントとエラーを記録するために使用されるロガーを取得します。 ロガーは保存されず、インデックスが作成またはロードされるたびに作成して割り当てる必要があることに注意してください。


**Returns:**
[ILogger](../../com.groupdocs.search.common/ilogger) - A logger that is used for logging events and errors in the index.

### setLogger(ILogger value) {#setLogger-com.groupdocs.search.common.ILogger-}
```
public final void setLogger(ILogger value)
```


インデックス内のイベントとエラーを記録するために使用されるロガーを設定します。 ロガーは保存されず、インデックスが作成またはロードされるたびに作成して割り当てる必要があることに注意してください。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | value | [ILogger](../../com.groupdocs.search.common/ilogger) | インデックス内のイベントとエラーを記録するために使用されるロガーです。 |
|

