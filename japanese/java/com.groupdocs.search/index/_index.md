---
title: "Index"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "ドキュメントのインデックス作成と検索を行うメインクラスを表します。"
type: docs
weight: 17
url: /ja/java/com.groupdocs.search/index/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable
```
public class Index implements Closeable
```

ドキュメントのインデックス作成と検索を行うメインクラスを表します。


**Learn more**

* [Creating an index](../https://docs.groupdocs.com/display/searchjava/Creating+an+index)
* [Indexing](../https://docs.groupdocs.com/display/searchjava/Indexing)
* [Searching](../https://docs.groupdocs.com/display/searchjava/Searching)


この例はクラスの典型的な使用方法を示しています。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // 指定されたフォルダーにインデックスを作成しています
index.add(documentsFolder); // 指定されたフォルダーからドキュメントをインデックス化しています
SearchResult result = index.search(query); // インデックスを検索しています
 
```
 
````


## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [Index()](#Index--) | メモリ内で  Index  クラスの新しいインスタンスを初期化します。 |
|
|  | [Index(IndexSettings settings)](#Index-com.groupdocs.search.IndexSettings-) | メモリ内で特定のインデックス設定を使用して  Index  クラスの新しいインスタンスを初期化します。 |
|
|  | [Index(String indexFolder)](#Index-java.lang.String-) |   Index  クラスの新しいインスタンスを初期化します。 |
|
|  | [Index(String indexFolder, IndexSettings settings)](#Index-java.lang.String-com.groupdocs.search.IndexSettings-) | 新しいインスタンスを初期化します |
Index
クラス。
|
|  | [Index(String indexFolder, boolean overwriteIfExists)](#Index-java.lang.String-boolean-) | 新しいインスタンスを初期化します |
Index
クラス。
|
|  | [Index(String indexFolder, IndexSettings settings, boolean overwriteIfExists)](#Index-java.lang.String-com.groupdocs.search.IndexSettings-boolean-) | 新しいインスタンスを初期化します |
Index
クラス。
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getEvents()](#getEvents--) | イベントの購読用ハブを取得します。 |
|
|  | [getIndexInfo()](#getIndexInfo--) | インデックスの基本情報を取得します。 |
|
|  | [getRepository()](#getRepository--) | インデックスが含まれている場合、インデックスリポジトリオブジェクトを取得します。 |
|
|  | [getIndexSettings()](#getIndexSettings--) | インデックス設定を取得します。 |
|
|  | [getDictionaries()](#getDictionaries--) | 辞書リポジトリを取得します。 |
|
|  | [close()](#close--) | 使用されているすべてのリソースを解放します |
Index
.
|
|  | [add(String path)](#add-java.lang.String-) | インデックス作成操作を実行します。 |
|
|  | [add(String path, IndexingOptions options)](#add-java.lang.String-com.groupdocs.search.options.IndexingOptions-) | インデックス作成操作を実行します。 |
|
|  | [add(String[] paths)](#add-java.lang.String---) | インデックス作成操作を実行します。 |
|
|  | [add(String[] paths, IndexingOptions options)](#add-java.lang.String---com.groupdocs.search.options.IndexingOptions-) | インデックス作成操作を実行します。 |
|
|  | [add(Document[] documents, IndexingOptions options)](#add-com.groupdocs.search.Document---com.groupdocs.search.options.IndexingOptions-) | インデックス作成操作を実行します。 |
|
|  | [add(ExtractedData[] data, IndexingOptions options)](#add-com.groupdocs.search.ExtractedData---com.groupdocs.search.options.IndexingOptions-) | インデックス作成操作を実行します。 |
|
|  | [update()](#update--) | 前回の更新以降に変更または削除されたドキュメントを再インデックスします。 |
|
|  | [update(UpdateOptions options)](#update-com.groupdocs.search.options.UpdateOptions-) | 前回の更新以降に変更または削除されたドキュメントを再インデックスします。 |
|
|  | [getIndexingReports()](#getIndexingReports--) | インデックス作成操作に関するレポートを取得します。 |
|
|  | [getSearchReports()](#getSearchReports--) | 検索操作に関するレポートを取得します。 |
|
|  | [search(String query)](#search-java.lang.String-) | インデックスを検索します。 |
|
|  | [search(String query, SearchOptions options)](#search-java.lang.String-com.groupdocs.search.options.SearchOptions-) | インデックスを検索します。 |
|
|  | [search(SearchQuery query)](#search-com.groupdocs.search.SearchQuery-) | インデックスを検索します。 |
|
|  | [search(SearchQuery query, SearchOptions options)](#search-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-) | インデックスを検索します。 |
|
|  | [search(SearchImage image, ImageSearchOptions options)](#search-com.groupdocs.search.common.SearchImage-com.groupdocs.search.options.ImageSearchOptions-) | インデックスで逆画像検索を実行します。 |
|
|  | [searchNext(ChunkSearchToken chunkSearchToken)](#searchNext-com.groupdocs.search.common.ChunkSearchToken-) | メソッド Search で開始されたチャンク検索を続行します。 |
|
|  | [searchNext(ChunkSearchToken chunkSearchToken, Cancellation cancellation)](#searchNext-com.groupdocs.search.common.ChunkSearchToken-com.groupdocs.search.common.Cancellation-) | メソッド Search で開始されたチャンク検索を続行します。 |
|
|  | [optimize()](#optimize--) | インデックスセグメントの数を、セグメント同士をマージすることで最小化します。 |
|
|  | [optimize(MergeOptions options)](#optimize-com.groupdocs.search.options.MergeOptions-) | インデックスセグメントの数を、セグメント同士をマージすることで最小化します。 |
|
|  | [merge(Index index, MergeOptions options)](#merge-com.groupdocs.search.Index-com.groupdocs.search.options.MergeOptions-) | 指定されたインデックスを現在のインデックスにマージします。 |
|
|  | [merge(IndexRepository repository, MergeOptions options)](#merge-com.groupdocs.search.IndexRepository-com.groupdocs.search.options.MergeOptions-) | 指定されたインデックスリポジトリからインデックスを現在のインデックスにマージします。 |
|
|  | [highlight(FoundDocument document, Highlighter highlighter)](#highlight-com.groupdocs.search.results.FoundDocument-com.groupdocs.search.highlighters.Highlighter-) | 見つかった用語をハイライトしたHTML形式のテキストを生成します。 |
|
|  | [highlight(FoundDocument document, Highlighter highlighter, HighlightOptions options)](#highlight-com.groupdocs.search.results.FoundDocument-com.groupdocs.search.highlighters.Highlighter-com.groupdocs.search.options.HighlightOptions-) | 見つかった用語をハイライトしたHTML形式のテキストを生成します。 |
|
|  | [getIndexedDocuments()](#getIndexedDocuments--) | すべてのインデックス化されたドキュメントの配列を取得します。 |
|
|  | [getIndexedDocumentItems(DocumentInfo documentInfo)](#getIndexedDocumentItems-com.groupdocs.search.results.DocumentInfo-) | ドキュメント項目の配列を取得します。 |
|
|  | [GetIndexedDocument(String documentKey)](#GetIndexedDocument-java.lang.String-) | ドキュメントキーでインデックス化されたドキュメントを取得します。 |
|
|  | [getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter)](#getDocumentText-com.groupdocs.search.results.DocumentInfo-com.groupdocs.search.common.OutputAdapter-) | インデックス化されたドキュメントのテキストを生成し、出力アダプターを介して渡します。 |
|
|  | [getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter, TextOptions options)](#getDocumentText-com.groupdocs.search.results.DocumentInfo-com.groupdocs.search.common.OutputAdapter-com.groupdocs.search.options.TextOptions-) | インデックス化されたドキュメントのHTML形式テキストを生成し、出力アダプターを介して転送します。 |
|
|  | [getIndexedPaths()](#getIndexedPaths--) | インデックス化されたパス（ドキュメントまたはフォルダー）の配列を取得します。 |
|
|  | [delete(String[] paths, UpdateOptions options)](#delete-java.lang.String---com.groupdocs.search.options.UpdateOptions-) | インデックスからインデックス化されたファイルまたはフォルダーを削除します。 |
|
|  | [delete(UpdateOptions options, String[] documentKeys)](#delete-com.groupdocs.search.options.UpdateOptions-java.lang.String---) | ストリームまたは構造からインデックス化されたドキュメントを削除します。 |
|
|  | [notifyIndex(Notification notification)](#notifyIndex-com.groupdocs.search.Notification-) | 指定された通知オブジェクトをインデックスに渡して通知を実行します。 |
|
|  | [changeAttributes(AttributeChangeBatch batch)](#changeAttributes-com.groupdocs.search.common.AttributeChangeBatch-) | 更新操作中に再インデックス化せずに、指定された属性変更のバッチをインデックス化されたドキュメントに適用します。 |
|
|  | [getAttributes(String path)](#getAttributes-java.lang.String-) | 指定されたインデックス化ドキュメントに関連付けられたすべての属性を取得します。 |
|
|  | [loadIntoMemoryCompletely(String indexFolder)](#loadIntoMemoryCompletely-java.lang.String-) | インデックス全体をメモリにロードします。 |
|
|  | [loadIntoMemoryCompletely(String indexFolder, IndexSettings settings)](#loadIntoMemoryCompletely-java.lang.String-com.groupdocs.search.IndexSettings-) | インデックス全体をメモリにロードします。 |
|
### Index() {#Index--}
```
public Index()
```


メモリ内で  Index  クラスの新しいインスタンスを初期化します。


この例は、ファイルをディスクに保存せずにメモリ内でインデックスを作成する方法を示しています。

````
 ```

Index index = new Index();
 
```
 
````



### Index(IndexSettings settings) {#Index-com.groupdocs.search.IndexSettings-}
```
public Index(IndexSettings settings)
```


メモリ内で特定のインデックス設定を使用して  Index  クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | インデックス設定オブジェクトです。 |


この例は、特定のインデックス設定を使用して、ファイルをディスクに保存せずにメモリ内でインデックスを作成する方法を示しています。

````
 ```

IndexSettings settings = new IndexSettings();
settings.setIndexType(IndexType.CompactIndex);
Index index = new Index(settings);
 
```
 
````

|

### Index(String indexFolder) {#Index-java.lang.String-}
```
public Index(String indexFolder)
```


Index クラスの新しいインスタンスを初期化します。ディスク上に新しいインデックスを作成するか、既存のインデックスを開きます。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | indexFolder | java.lang.String | インデックスフォルダーのパスです。 |


この例は、ディスク上にインデックスを作成するか、既存のインデックスを開く方法を示しています。

````
 ```

String indexFolder = "c:\\MyIndex\\";
Index index = new Index(indexFolder);
 
```
 
````

|

### Index(String indexFolder, IndexSettings settings) {#Index-java.lang.String-com.groupdocs.search.IndexSettings-}
```
public Index(String indexFolder, IndexSettings settings)
```


新しいインスタンスを初期化します
Index
クラス。
特定の設定で新しいインデックスを作成するか、ディスク上の既存インデックスを開きます。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | indexFolder | java.lang.String | インデックスフォルダーのパスです。 |
|
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | インデックス設定オブジェクトです。 |

この例は、特定のインデックス設定を使用してディスク上にインデックスを作成する方法を示しています。

````
 ```

String indexFolder = "c:\\MyIndex\\";
IndexSettings settings = new IndexSettings();
settings.setIndexType(IndexType.CompactIndex);
Index index = new Index(indexFolder, settings);
 
```
 
````

|

### Index(String indexFolder, boolean overwriteIfExists) {#Index-java.lang.String-boolean-}
```
public Index(String indexFolder, boolean overwriteIfExists)
```


新しいインスタンスを初期化します
Index
クラス。
ディスクから既存のインデックスをロードします if
overwriteIfExists
は
false
;
それ以外の場合はディスク上に新しいインデックスを作成します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | indexFolder | java.lang.String | インデックスフォルダーのパスです。 |
|
|  | overwriteIfExists | boolean | インデックスフォルダーを上書きするフラグです。 |

この例は、既に別のインデックスが含まれているフォルダー内に新しいインデックスを作成する方法を示しています。

````
 ```

String indexFolder = "c:\\MyIndex\\";
Index index = new Index(indexFolder, true);
 
```
 
````

|

### Index(String indexFolder, IndexSettings settings, boolean overwriteIfExists) {#Index-java.lang.String-com.groupdocs.search.IndexSettings-boolean-}
```
public Index(String indexFolder, IndexSettings settings, boolean overwriteIfExists)
```


新しいインスタンスを初期化します
Index
クラス。
ディスクから既存のインデックスをロードします if
overwriteIfExists
は
false
;
それ以外の場合は、特定のインデックス設定でディスク上に新しいインデックスを作成します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | indexFolder | java.lang.String | インデックスフォルダーのパスです。 |
|
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | インデックス設定オブジェクトです。 |
|
|  | overwriteIfExists | boolean | インデックスフォルダーを上書きするフラグです。 |

この例は、特定のインデックス設定を使用してディスク上にインデックスを作成する方法を示しています。

````
 ```

String indexFolder = "c:\\MyIndex\\";
IndexSettings settings = new IndexSettings();
settings.setIndexType(IndexType.CompactIndex);
Index index = new Index(indexFolder, settings, true);
 
```
 
````

|

### getEvents() {#getEvents--}
```
public final EventHub getEvents()
```


イベントの購読用ハブを取得します。


**Returns:**
[EventHub](../../com.groupdocs.search.events/eventhub) - The event hub for subscribing to events.

### getIndexInfo() {#getIndexInfo--}
```
public final IndexInfo getIndexInfo()
```


インデックスの基本情報を取得します。


**Returns:**
[IndexInfo](../../com.groupdocs.search.common/indexinfo) - The basic information on the index.

### getRepository() {#getRepository--}
```
public final IndexRepository getRepository()
```


インデックスが含まれている場合、インデックスリポジトリオブジェクトを取得します。


**Returns:**
[IndexRepository](../../com.groupdocs.search/indexrepository) - The index repository object.

### getIndexSettings() {#getIndexSettings--}
```
public final IndexSettings getIndexSettings()
```


インデックス設定を取得します。


**Returns:**
[IndexSettings](../../com.groupdocs.search/indexsettings) - The index settings.

### getDictionaries() {#getDictionaries--}
```
public final DictionaryRepository getDictionaries()
```


辞書リポジトリを取得します。


**Returns:**
[DictionaryRepository](../../com.groupdocs.search.dictionaries/dictionaryrepository) - The dictionary repository.

### close() {#close--}
```
public final void close()
```


使用されているすべてのリソースを解放します
Index
.


### add(String path) {#add-java.lang.String-}
```
public final void add(String path)
```


インデックス作成操作を実行します。
絶対パスまたは相対パスでファイルまたはフォルダーを追加します。
すべてのサブフォルダーのドキュメントがインデックスされます。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | path | java.lang.String | インデックス対象のファイルまたはフォルダーへのパスです。 |

この例は、インデックスにドキュメントを追加する方法を示しています。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String folderPath = "c:\\MyDocuments\\";
String filePath = "c:\\Documents\\MyFile.txt";
Index index = new Index(indexFolder); // 指定されたフォルダーにインデックスを作成しています
index.add(folderPath); // 指定されたフォルダー内のドキュメントをインデックス化
index.add(filePath); // 指定されたドキュメントをインデックス化
 
```
 
````

|

### add(String path, IndexingOptions options) {#add-java.lang.String-com.groupdocs.search.options.IndexingOptions-}
```
public final void add(String path, IndexingOptions options)
```


インデックス作成操作を実行します。
絶対パスまたは相対パスでファイルまたはフォルダーを追加します。
すべてのサブフォルダーのドキュメントがインデックスされます。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | path | java.lang.String | インデックス対象のファイルまたはフォルダーへのパスです。 |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | インデックスオプションです。 |

この例は、特定のインデックスオプションを使用してインデックスにドキュメントを追加する方法を示しています。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String folderPath = "c:\\MyDocuments\\";
String filePath = "c:\\Documents\\MyFile.txt";
Index index = new Index(indexFolder); // 指定されたフォルダーにインデックスを作成しています
IndexingOptions options = new IndexingOptions();
options.setThreads(2); // インデックス作成スレッド数を設定しています
index.add(folderPath, options); // 指定されたフォルダー内のドキュメントをインデックス化
index.add(filePath, options); // 指定されたドキュメントをインデックス化
 
```
 
````

|

### add(String[] paths) {#add-java.lang.String---}
```
public final void add(String[] paths)
```


インデックス作成操作を実行します。
絶対パスまたは相対パスでファイルまたはフォルダーを追加します。
すべてのサブフォルダーのドキュメントがインデックスされます。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | パス | java.lang.String[] | インデックス作成対象のファイルまたはフォルダーへのパスです。 |

この例は、インデックスにドキュメントを追加する方法を示しています。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String folderPath = "c:\\MyDocuments\\";
String filePath = "c:\\Documents\\MyFile.txt";
Index index = new Index(indexFolder); // 指定されたフォルダーにインデックスを作成しています
String[] paths = new String[] { folderPath, filePath };
index.add(paths); // 指定されたパスのドキュメントをインデックス作成
 
```
 
````

|

### add(String[] paths, IndexingOptions options) {#add-java.lang.String---com.groupdocs.search.options.IndexingOptions-}
```
public final void add(String[] paths, IndexingOptions options)
```


インデックス作成操作を実行します。
絶対パスまたは相対パスでファイルまたはフォルダーを追加します。
すべてのサブフォルダーのドキュメントがインデックスされます。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | パス | java.lang.String[] | インデックス作成対象のファイルまたはフォルダーへのパスです。 |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | インデックスオプションです。 |

この例は、特定のインデックスオプションを使用してインデックスにドキュメントを追加する方法を示しています。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String folderPath = "c:\\MyDocuments\\";
String filePath = "c:\\Documents\\MyFile.txt";
Index index = new Index(indexFolder); // 指定されたフォルダーにインデックスを作成しています
IndexingOptions options = new IndexingOptions();
options.setThreads(2); // インデックス作成スレッド数を設定しています
String[] paths = new String[] { folderPath, filePath };
index.add(paths, options); // 指定されたパスのドキュメントをインデックス作成
 
```
 
````

|

### add(Document[] documents, IndexingOptions options) {#add-com.groupdocs.search.Document---com.groupdocs.search.options.IndexingOptions-}
```
public final void add(Document[] documents, IndexingOptions options)
```


インデックス作成操作を実行します。
ファイルシステム、ストリーム、または構造からドキュメントを追加します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | documents | [Document\[\]](../../com.groupdocs.search/document) | ファイルシステム、ストリーム、または構造からのドキュメントです。 |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | インデックスオプションです。 |
|

### add(ExtractedData[] data, IndexingOptions options) {#add-com.groupdocs.search.ExtractedData---com.groupdocs.search.options.IndexingOptions-}
```
public final void add(ExtractedData[] data, IndexingOptions options)
```


インデックス作成操作を実行します。
抽出されたデータをインデックスに追加します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | data | [ExtractedData\[\]](../../com.groupdocs.search/extracteddata) | 抽出されたデータです。 |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | インデックスオプションです。 |
|

### update() {#update--}
```
public final void update()
```


前回の更新以降に変更または削除されたドキュメントを再インデックスします。
インデックスされたフォルダーに追加された新しいファイルを追加します。

この例はインデックスの更新方法を示しています。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // 指定されたフォルダーにインデックスを作成しています
index.add(documentsFolder); // 指定されたフォルダーからドキュメントをインデックス化しています
// ドキュメントフォルダーからドキュメントを削除するか、変更するか、フォルダーに新しいドキュメントを追加します
index.update(); // インデックスを更新しています
 
```
 
````



### update(UpdateOptions options) {#update-com.groupdocs.search.options.UpdateOptions-}
```
public final void update(UpdateOptions options)
```


前回の更新以降に変更または削除されたドキュメントを再インデックスします。
インデックスされたフォルダーに追加された新しいファイルを追加します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | options | [UpdateOptions](../../com.groupdocs.search.options/updateoptions) | 更新オプションです。 |

この例は特定の更新オプションを使用してインデックスを更新する方法を示しています。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // 指定されたフォルダーにインデックスを作成しています
index.add(documentsFolder); // 指定されたフォルダーからドキュメントをインデックス化しています
// ドキュメントフォルダーからドキュメントを削除するか、変更するか、フォルダーに新しいドキュメントを追加します
UpdateOptions options = new UpdateOptions();
options.setThreads(2); // インデックス作成スレッド数を設定しています
index.update(options); // インデックスを更新しています
 
```
 
````

|

### getIndexingReports() {#getIndexingReports--}
```
public final IndexingReport[] getIndexingReports()
```


インデックス作成操作に関するレポートを取得します。


**Returns:**
com.groupdocs.search.common.IndexingReport[] - インデックスレポートです。

この例はインデックスレポートの取得方法を示しています。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // 指定されたフォルダーにインデックスを作成しています
index.add(documentsFolder); // 指定されたフォルダーからドキュメントをインデックス化しています
IndexingReport[] reports = index.getIndexingReports(); // インデックスレポートを取得しています
 
```
 
````


### getSearchReports() {#getSearchReports--}
```
public final SearchReport[] getSearchReports()
```


検索操作に関するレポートを取得します。


**Returns:**
com.groupdocs.search.common.SearchReport[] - 検索レポートです。

この例は検索レポートの取得方法を示しています。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query1 = \"Einstein\";
String query2 = \"Newton\";
Index index = new Index(indexFolder); // 指定されたフォルダーにインデックスを作成しています
index.add(documentsFolder); // 指定されたフォルダーからドキュメントをインデックス化しています
SearchResult result1 = index.search(query1); // 検索しています
SearchResult result2 = index.search(query2);
SearchResult result3 = index.search(query1 + \" & \" + query2);
SearchReport[] reports = index.getSearchReports(); // 検索レポートを取得しています
 
```
 
````


### search(String query) {#search-java.lang.String-}
```
public final SearchResult search(String query)
```


インデックスを検索します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | query | java.lang.String | 検索クエリです。 |

次の例はシンプル検索を実行する方法を示しています。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // 指定されたフォルダーにインデックスを作成しています
index.add(documentsFolder); // 指定されたフォルダーからドキュメントをインデックス化しています
SearchResult result = index.search(query); // 検索中
 
```
 
````

次の例は正規表現検索を実行する方法を示しています。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // 指定されたフォルダーにインデックスを作成しています
index.add(documentsFolder); // 指定されたフォルダーからドキュメントをインデックス化しています
String query = \"^[0-9]{3,}\"; // 検索クエリの先頭にあるキャレット記号は、インデックスに正規表現クエリであることを示します
SearchResult result = index.search(query); // 検索中
 
```
 
````

次の例はファセット検索を実行する方法を示しています。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // 指定されたフォルダーにインデックスを作成しています
index.add(documentsFolder); // 指定されたフォルダーからドキュメントをインデックス化しています
String query = \"content:Newton\"; // クエリ内のコロンの前の単語は、検索対象のドキュメントフィールド名を意味します
SearchResult result = index.search(query); // 検索中
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(String query, SearchOptions options) {#search-java.lang.String-com.groupdocs.search.options.SearchOptions-}
```
public final SearchResult search(String query, SearchOptions options)
```


インデックスを検索します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | query | java.lang.String | 検索クエリです。 |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | 検索オプションです。 |

次の例はファジー検索を実行する方法を示しています。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // 指定されたフォルダーにインデックスを作成しています
index.add(documentsFolder); // 指定されたフォルダーからドキュメントをインデックス化しています
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // ファジー検索を有効にしています
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1)); // 各単語の許容できる差分数を設定しています
// 先頭と末尾の二重引用符は、インデックスにフレーズ検索クエリであることを示します
String query = \"\\\"The Pursuit of Happiness\\\"\";
SearchResult result = index.search(query, options); // 検索中
 
```
 
````

次の例は同義語検索を実行する方法を示しています。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // 指定されたフォルダーにインデックスを作成しています
index.add(documentsFolder); // 指定されたフォルダーからドキュメントをインデックス化しています
SearchOptions options = new SearchOptions();
options.setUseSynonymSearch(true); // 同義語検索を有効にしています
String query = \"cry\";
SearchResult result = index.search(query, options); // 検索中
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchQuery query) {#search-com.groupdocs.search.SearchQuery-}
```
public final SearchResult search(SearchQuery query)
```


インデックスを検索します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | 検索クエリです。 |

次の例はオブジェクト形式のクエリを使用した検索を実行する方法を示しています。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // 指定されたフォルダーにインデックスを作成しています
index.add(documentsFolder); // 指定されたフォルダーからドキュメントをインデックス化しています
// サブクエリ1を作成
SearchQuery subquery1 = SearchQuery.createWordQuery(\"accommodation\");
subquery1.setSearchOptions(new SearchOptions()); // サブクエリ1のみに検索オプションを設定しています
subquery1.getSearchOptions().getFuzzySearch().setEnabled(true); // ファジー検索を有効にしています
subquery1.getSearchOptions().getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3)); // 許容できる最大差分数を設定しています
// サブクエリ2を作成
SearchQuery subquery2 = SearchQuery.createNumericRangeQuery(1, 1000000);
// サブクエリ3を作成
SearchQuery subquery3 = SearchQuery.createRegexQuery(\"(.)\\\\1\");
// サブクエリを1つのクエリに結合しています
SearchQuery query = SearchQuery.createPhraseSearchQuery(subquery1, subquery2, subquery3);
SearchResult result = index.search(query); // 検索中
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchQuery query, SearchOptions options) {#search-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-}
```
public final SearchResult search(SearchQuery query, SearchOptions options)
```


インデックスを検索します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | 検索クエリです。 |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | 検索オプションです。 |

次の例はオブジェクト形式のクエリを使用した検索を実行する方法を示しています。

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

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchImage image, ImageSearchOptions options) {#search-com.groupdocs.search.common.SearchImage-com.groupdocs.search.options.ImageSearchOptions-}
```
public final ImageSearchResult search(SearchImage image, ImageSearchOptions options)
```


インデックスで逆画像検索を実行します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | image | [SearchImage](../../com.groupdocs.search.common/searchimage) | 検索する画像。 |
|
|  | options | [ImageSearchOptions](../../com.groupdocs.search.options/imagesearchoptions) | 画像検索オプション。 |
|

**Returns:**
[ImageSearchResult](../../com.groupdocs.search.results/imagesearchresult) - The result of a reverse image search.

### searchNext(ChunkSearchToken chunkSearchToken) {#searchNext-com.groupdocs.search.common.ChunkSearchToken-}
```
public final SearchResult searchNext(ChunkSearchToken chunkSearchToken)
```


メソッド Search で開始されたチャンク検索を続行します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | chunkSearchToken | [ChunkSearchToken](../../com.groupdocs.search.common/chunksearchtoken) | チャンク検索トークン。 |

この例はチャンク検索の実行方法を示しています。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // 指定されたフォルダーにインデックスを作成しています
index.add(documentsFolder); // 指定されたフォルダーからドキュメントをインデックス化しています
SearchOptions options = new SearchOptions();
options.setChunkSearch(true); // チャンク検索を有効にする
SearchResult result = index.search(query, options); // チャンク検索を開始
System.out.println("ドキュメント数: " + result.getDocumentCount());
System.out.println("出現回数: " + result.getOccurrenceCount());
while (result.getNextChunkSearchToken() != null) {
result = index.searchNext(result.getNextChunkSearchToken()); // チャンク検索を継続
System.out.println("ドキュメント数: " + result.getDocumentCount());
System.out.println("出現回数: " + result.getOccurrenceCount());
}
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### searchNext(ChunkSearchToken chunkSearchToken, Cancellation cancellation) {#searchNext-com.groupdocs.search.common.ChunkSearchToken-com.groupdocs.search.common.Cancellation-}
```
public final SearchResult searchNext(ChunkSearchToken chunkSearchToken, Cancellation cancellation)
```


メソッド Search で開始されたチャンク検索を続行します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | chunkSearchToken | [ChunkSearchToken](../../com.groupdocs.search.common/chunksearchtoken) | チャンク検索トークン。 |
|
|  | cancellation | [Cancellation](../../com.groupdocs.search.common/cancellation) | キャンセルオブジェクト。 |

この例はオブジェクト形式のクエリを使用した検索の実行方法を示しています。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // 指定されたフォルダーにインデックスを作成しています
index.add(documentsFolder); // 指定されたフォルダーからドキュメントをインデックス化しています
Cancellation cancellation = new Cancellation(); // このキャンセルオブジェクトは、キャンセルされた場合にすべての検索継続を中止します
SearchOptions options = new SearchOptions();
options.setChunkSearch(true); // チャンク検索を有効にする
options.setCancellation(cancellation);
SearchResult result = index.search(query, options); // チャンク検索を開始
System.out.println("ドキュメント数: " + result.getDocumentCount());
System.out.println("出現回数: " + result.getOccurrenceCount());
while (result.getNextChunkSearchToken() != null) {
result = index.searchNext(result.getNextChunkSearchToken(), cancellation); // チャンク検索を継続
System.out.println("ドキュメント数: " + result.getDocumentCount());
System.out.println("出現回数: " + result.getOccurrenceCount());
}
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### optimize() {#optimize--}
```
public final void optimize()
```


インデックスセグメントの数を、セグメント同士をマージすることで最小化します。
この操作は検索パフォーマンスを向上させます。

この例はインデックスのセグメントをマージする方法を示しています。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
String documentsFolder3 = "c:\\MyDocuments3\\";
Index index = new Index(indexFolder); // 指定されたフォルダーにインデックスを作成しています
index.add(documentsFolder1); // 指定されたフォルダーからドキュメントをインデックス化
index.add(documentsFolder2); // AddToIndex の各呼び出しは、インデックスに少なくとも1つの新しいセグメントを作成します
index.add(documentsFolder3);
// インデックスのセグメントをマージ
index.optimize();
 
```
 
````



### optimize(MergeOptions options) {#optimize-com.groupdocs.search.options.MergeOptions-}
```
public final void optimize(MergeOptions options)
```


インデックスセグメントの数を、セグメント同士をマージすることで最小化します。
この操作は検索パフォーマンスを向上させます。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | options | [MergeOptions](../../com.groupdocs.search.options/mergeoptions) | マージオプションです。 |

この例は、特定のマージオプションを使用してインデックスのセグメントをマージする方法を示しています。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
String documentsFolder3 = "c:\\MyDocuments3\\";
Index index = new Index(indexFolder); // 指定されたフォルダーにインデックスを作成しています
index.add(documentsFolder1); // 指定されたフォルダーからドキュメントをインデックス化
index.add(documentsFolder2); // AddToIndex の各呼び出しは、インデックスに少なくとも1つの新しいセグメントを作成します
index.add(documentsFolder3);
MergeOptions options = new MergeOptions();
options.setAsync(true); // 非同期操作
options.setCancellation(new Cancellation()); // キャンセルオブジェクトを作成
// インデックスのセグメントをマージ
index.optimize(options); // このメソッドは操作が完了する前に戻ります
options.getCancellation().cancelAfter(10000); // 操作の最大期間を10秒に設定
 
```
 
````

|

### merge(Index index, MergeOptions options) {#merge-com.groupdocs.search.Index-com.groupdocs.search.options.MergeOptions-}
```
public final void merge(Index index, MergeOptions options)
```


指定されたインデックスを現在のインデックスにマージします。
他のインデックスは変更されないことに注意してください。


他のインデックスに以前のバージョンがある場合、マージする前に更新する必要があります
IndexUpdater
.


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | index | [Index](../../com.groupdocs.search/index) | マージ先のインデックスです。 |
|
|  | options | [MergeOptions](../../com.groupdocs.search.options/mergeoptions) | マージオプションです。 |

この例は、インデックスを現在のインデックスにマージする方法を示しています。

````
 ```

String indexFolder1 = "c:\\MyIndex1\\";
String indexFolder2 = "c:\\MyIndex2\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
Index index1 = new Index(indexFolder1); // index1 を作成
index1.add(documentsFolder1); // ドキュメントをインデックス化
Index index2 = new Index(indexFolder2); // index2 を作成
index2.add(documentsFolder2); // ドキュメントをインデックス化
MergeOptions options = new MergeOptions();
options.setCancellation(new Cancellation()); // キャンセルオブジェクトを作成
// index2 を index1 にマージしています。index2 のファイルは変更されないことに注意してください。
index1.merge(index2, options);
 
```
 
````

|

### merge(IndexRepository repository, MergeOptions options) {#merge-com.groupdocs.search.IndexRepository-com.groupdocs.search.options.MergeOptions-}
```
public final void merge(IndexRepository repository, MergeOptions options)
```


指定されたインデックスリポジトリからインデックスを現在のインデックスにマージします。
リポジトリ内のインデックスは変更されないことに注意してください。


他のインデックスに以前のバージョンがある場合、マージする前に更新する必要があります
IndexUpdater
.


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | repository | [IndexRepository](../../com.groupdocs.search/indexrepository) | マージ先のインデックスリポジトリです。 |
|
|  | options | [MergeOptions](../../com.groupdocs.search.options/mergeoptions) | マージオプションです。 |

この例は、インデックスリポジトリを現在のインデックスにマージする方法を示しています。

````
 ```

String indexFolder1 = "c:\\MyIndex1\\";
String indexFolder2 = "c:\\MyIndex2\\";
String indexFolder3 = "c:\\MyIndex3\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
String documentsFolder3 = "c:\\MyDocuments3\\";
Index index1 = new Index(indexFolder1); // index1 を作成
index1.add(documentsFolder1); // ドキュメントをインデックス化
IndexRepository repository = new IndexRepository(); // インデックスリポジトリを作成
Index index2 = repository.create(indexFolder2); // index2 を作成
index2.add(documentsFolder2); // ドキュメントをインデックス化
Index index3 = repository.create(indexFolder3); // index3 を作成
index3.add(documentsFolder3); // ドキュメントをインデックス化
MergeOptions options = new MergeOptions();
options.setCancellation(new Cancellation()); // キャンセルオブジェクトを作成
// インデックスリポジトリ内のすべてのインデックスを index1 にマージします。index2 と index3 は変更されません。
index1.merge(repository, options);
 
```
 
````

|

### highlight(FoundDocument document, Highlighter highlighter) {#highlight-com.groupdocs.search.results.FoundDocument-com.groupdocs.search.highlighters.Highlighter-}
```
public final void highlight(FoundDocument document, Highlighter highlighter)
```


見つかった用語をハイライトしたHTML形式のテキストを生成します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | document | [FoundDocument](../../com.groupdocs.search.results/founddocument) | 見つかったドキュメントです。 |
|
|  | highlighter | [Highlighter](../../com.groupdocs.search.highlighters/highlighter) | 検索結果ハイライト表示です。 |

この例は、HTML 形式のテキストで出現箇所をハイライトする方法を示しています。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentFolder = "c:\\MyDocuments\\";
// インデックスを作成
Index index = new Index(indexFolder);
// 指定されたフォルダーからドキュメントをインデックス化
index.add(documentFolder);
// 'eternity' という単語を検索
SearchResult result = index.search("eternity");
// テキスト内の出現箇所をハイライト
if (result.getDocumentCount() > 0) {
FoundDocument document = result.getFoundDocument(0); // 最初に見つかったドキュメントを取得
OutputAdapter outputAdapter = new FileOutputAdapter("c:\\Highlighted.html"); // ファイルへの出力アダプタを作成
Highlighter highlighter = new HtmlHighlighter(outputAdapter); // ハイライトオブジェクトを作成
index.highlight(document, highlighter); // ハイライトされた出現箇所を含む HTML 形式のテキストを生成
}
 
```
 
````

|

### highlight(FoundDocument document, Highlighter highlighter, HighlightOptions options) {#highlight-com.groupdocs.search.results.FoundDocument-com.groupdocs.search.highlighters.Highlighter-com.groupdocs.search.options.HighlightOptions-}
```
public final void highlight(FoundDocument document, Highlighter highlighter, HighlightOptions options)
```


見つかった用語をハイライトしたHTML形式のテキストを生成します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | document | [FoundDocument](../../com.groupdocs.search.results/founddocument) | 見つかったドキュメントです。 |
|
|  | highlighter | [Highlighter](../../com.groupdocs.search.highlighters/highlighter) | 検索結果ハイライト表示です。 |
|
|  | options | [HighlightOptions](../../com.groupdocs.search.options/highlightoptions) | ハイライトオプションです。 |

この例は、HTML 形式のテキストで出現箇所をハイライトする方法を示しています。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentFolder = "c:\\MyDocuments\\";
// インデックスを作成
Index index = new Index(indexFolder);
// 指定されたフォルダーからドキュメントをインデックス化
index.add(documentFolder);
// 'eternity' という単語を検索
SearchResult result = index.search("eternity");
// テキスト内の出現箇所をハイライト
if (result.getDocumentCount() > 0) {
FoundDocument document = result.getFoundDocument(0); // 最初に見つかったドキュメントを取得
OutputAdapter outputAdapter = new FileOutputAdapter("c:\\Highlighted.html"); // ファイルへの出力アダプタを作成
Highlighter highlighter = new HtmlHighlighter(outputAdapter); // ハイライトオブジェクトを作成
HighlightOptions options = new HighlightOptions(); // ハイライトオプションオブジェクトを作成
options.setTermsBefore(5);
options.setTermsAfter(5);
options.setTermsTotal(15);
index.highlight(document, highlighter, options); // ハイライトされた出現箇所を含むHTML形式のテキストを生成
}
 
```
 
````

|

### getIndexedDocuments() {#getIndexedDocuments--}
```
public final DocumentInfo[] getIndexedDocuments()
```


すべてのインデックス化されたドキュメントの配列を取得します。


**Returns:**
com.groupdocs.search.results.DocumentInfo[] - すべてのインデックス化されたドキュメントの配列です。

この例は、インデックスからインデックス化されたドキュメントのリストを取得する方法を示しています。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// 指定されたフォルダーにインデックスを作成しています
Index index = new Index(indexFolder);
// 指定されたフォルダーからドキュメントをインデックス化
index.add(documentsFolder);
// インデックス化されたドキュメントのリストを取得
DocumentInfo[] documents = index.getIndexedDocuments();
 
```
 
````


### getIndexedDocumentItems(DocumentInfo documentInfo) {#getIndexedDocumentItems-com.groupdocs.search.results.DocumentInfo-}
```
public final DocumentInfo[] getIndexedDocumentItems(DocumentInfo documentInfo)
```


ドキュメント項目の配列を取得します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | documentInfo | [DocumentInfo](../../com.groupdocs.search.results/documentinfo) | ドキュメント情報です。 |

この例は、インデックスからインデックス化されたドキュメントの項目リストを取得する方法を示しています。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// 指定されたフォルダーにインデックスを作成しています
Index index = new Index(indexFolder);
// 指定されたフォルダーからドキュメントをインデックス化
index.add(documentsFolder);
// インデックス化されたドキュメントのリストを取得
DocumentInfo[] documents = index.getIndexedDocuments();
for (int i = 0; i < documents.length; i++) {
DocumentInfo document = documents[i];
System.out.println(document.getFilePath());
DocumentInfo[] items = index.getIndexedDocumentItems(document); // ドキュメント項目のリストを取得
for (int j = 0; j < items.length; j++) {
DocumentInfo item = items[j];
System.out.println("\t" + item.getInnerPath());
}
}
 
```
 
````

|

**Returns:**
com.groupdocs.search.results.DocumentInfo[] - ドキュメント項目の配列です。

### GetIndexedDocument(String documentKey) {#GetIndexedDocument-java.lang.String-}
```
public DocumentInfo GetIndexedDocument(String documentKey)
```


ドキュメントキーでインデックス化されたドキュメントを取得します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | documentKey | java.lang.String | ドキュメントキーです。 |
|

**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - The indexed document.

### getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter) {#getDocumentText-com.groupdocs.search.results.DocumentInfo-com.groupdocs.search.common.OutputAdapter-}
```
public final void getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter)
```


インデックス化されたドキュメントのテキストを生成し、出力アダプターを介して渡します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | documentInfo | [DocumentInfo](../../com.groupdocs.search.results/documentinfo) | インデックス化されたドキュメント情報です。 |
|
|  | adapter | [OutputAdapter](../../com.groupdocs.search.common/outputadapter) | 出力アダプターです。 |

この例は、インデックスからインデックス化されたドキュメントのテキストを取得する方法を示しています。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// 指定されたフォルダーにインデックスを作成しています
Index index = new Index(indexFolder);
// 指定されたフォルダーからドキュメントをインデックス化
index.add(documentsFolder);
// インデックス化されたドキュメントのリストを取得
DocumentInfo[] documents = index.getIndexedDocuments();
// ドキュメントテキストを取得
if (documents.length > 0) {
FileOutputAdapter outputAdapter = new FileOutputAdapter("C:\\Text.html");
index.getDocumentText(documents[0], outputAdapter);
}
 
```
 
````

|

### getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter, TextOptions options) {#getDocumentText-com.groupdocs.search.results.DocumentInfo-com.groupdocs.search.common.OutputAdapter-com.groupdocs.search.options.TextOptions-}
```
public final void getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter, TextOptions options)
```


インデックス化されたドキュメントのHTML形式テキストを生成し、出力アダプターを介して転送します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | documentInfo | [DocumentInfo](../../com.groupdocs.search.results/documentinfo) | インデックス化されたドキュメント情報です。 |
|
|  | adapter | [OutputAdapter](../../com.groupdocs.search.common/outputadapter) | 出力アダプターです。 |
|
|  | options | [TextOptions](../../com.groupdocs.search.options/textoptions) | テキスト取得オプションです。 |
|

### getIndexedPaths() {#getIndexedPaths--}
```
public final String[] getIndexedPaths()
```


インデックス化されたパス（ドキュメントまたはフォルダー）の配列を取得します。


**Returns:**
java.lang.String[] - インデックス化されたパスの配列です。

### delete(String[] paths, UpdateOptions options) {#delete-java.lang.String---com.groupdocs.search.options.UpdateOptions-}
```
public final DeleteResult delete(String[] paths, UpdateOptions options)
```


インデックスからインデックス化されたファイルまたはフォルダーを削除します。その後、削除されたパスを除外してインデックスを更新します。
フォルダーの一部としてインデックスに追加された場合、個々のドキュメントはインデックスから削除できないことに注意してください。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | パス | java.lang.String[] | 削除するファイルまたはフォルダーのパス。 |
|
|  | options | [UpdateOptions](../../com.groupdocs.search.options/updateoptions) | 更新オプションです。 |

この例は、インデックスからインデックスされたパスを削除する方法を示しています。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder1 = "c:\\MyDocuments\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
// 指定されたフォルダーにインデックスを作成しています
Index index = new Index(indexFolder);
// 指定されたフォルダーからドキュメントをインデックス化
index.add(documentsFolder1);
index.add(documentsFolder2);
// インデックスからインデックスされたパスを取得
String[] indexedPaths1 = index.getIndexedPaths();
// コンソールにインデックスされたパスを書き込む
System.out.println("インデックスされたパス:");
for (String path : indexedPaths1) {
System.out.println("\t" + path);
}
// インデックスからインデックスパスを削除
DeleteResult deleteResult = index.delete(new String[] { documentsFolder1 }, new UpdateOptions());
// 削除後にインデックスされたパスを取得
String[] indexedPaths2 = index.getIndexedPaths();
System.out.println("\n削除されたパス: " + deleteResult.getSuccessCount());
System.out.println("\nインデックスされたパス:");
for (String path : indexedPaths2) {
System.out.println("\t" + path);
}
 
```
 
````

|

**Returns:**
[DeleteResult](../../com.groupdocs.search.results/deleteresult) - An object describing the result of deleting files or folders from the index.

### delete(UpdateOptions options, String[] documentKeys) {#delete-com.groupdocs.search.options.UpdateOptions-java.lang.String---}
```
public final DeleteResult delete(UpdateOptions options, String[] documentKeys)
```


ストリームまたは構造体からインデックスされたドキュメントを削除します。その後、削除されたドキュメントなしでインデックスを更新します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | options | [UpdateOptions](../../com.groupdocs.search.options/updateoptions) | 更新オプションです。 |
|
|  | documentKeys | java.lang.String[] | ストリームまたは構造体から追加されたドキュメントのキー。 |
|

**Returns:**
[DeleteResult](../../com.groupdocs.search.results/deleteresult) - An object describing the result of deleting documents from the index.

### notifyIndex(Notification notification) {#notifyIndex-com.groupdocs.search.Notification-}
```
public final boolean notifyIndex(Notification notification)
```


指定された通知オブジェクトをインデックスに渡して通知を実行します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | notification | [Notification](../../com.groupdocs.search/notification) | 通知オブジェクト。 |
|

**Returns:**
boolean - 通知が正常に実行された場合は true を返し、そうでない場合は false を返します。

### changeAttributes(AttributeChangeBatch batch) {#changeAttributes-com.groupdocs.search.common.AttributeChangeBatch-}
```
public final void changeAttributes(AttributeChangeBatch batch)
```


更新操作中に再インデックス化せずに、指定された属性変更のバッチをインデックス化されたドキュメントに適用します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | batch | [AttributeChangeBatch](../../com.groupdocs.search.common/attributechangebatch) | 属性変更バッチ。 |
|

### getAttributes(String path) {#getAttributes-java.lang.String-}
```
public final String[] getAttributes(String path)
```


指定されたインデックス化ドキュメントに関連付けられたすべての属性を取得します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | path | java.lang.String | ドキュメントのパス。 |
|

**Returns:**
java.lang.String[] - ドキュメントに関連付けられた属性。

### loadIntoMemoryCompletely(String indexFolder) {#loadIntoMemoryCompletely-java.lang.String-}
```
public static Index loadIntoMemoryCompletely(String indexFolder)
```


インデックス全体をメモリにロードします。
インデックスへの変更は自動的に元のフォルダーに保存されません。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | indexFolder | java.lang.String | インデックスフォルダーのパスです。 |
|

**Returns:**
[Index](../../com.groupdocs.search/index) - The loaded in-memory index.

### loadIntoMemoryCompletely(String indexFolder, IndexSettings settings) {#loadIntoMemoryCompletely-java.lang.String-com.groupdocs.search.IndexSettings-}
```
public static Index loadIntoMemoryCompletely(String indexFolder, IndexSettings settings)
```


インデックス全体をメモリにロードします。
インデックスへの変更は自動的に元のフォルダーに保存されません。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | indexFolder | java.lang.String | インデックスフォルダーのパスです。 |
|
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | インデックス設定オブジェクトです。 |
|

**Returns:**
[Index](../../com.groupdocs.search/index) - The loaded in-memory index.

