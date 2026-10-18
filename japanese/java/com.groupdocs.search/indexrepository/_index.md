---
title: "IndexRepository"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "複数のインデックスを結合し、共通の操作を実行するためのコンテナを表します。"
type: docs
weight: 18
url: /ja/java/com.groupdocs.search/indexrepository/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable
```
public class IndexRepository implements Closeable
```

複数のインデックスを結合し、共通の操作を実行するためのコンテナを表します。


**Learn more**

* [Search index repository](../https://docs.groupdocs.com/display/searchjava/Search+index+repository)


この例はクラスの典型的な使用方法を示しています。

````
 ```

String indexFolder1 = "c:\\MyIndex\\";
String indexFolder2 = "c:\\MyIndex\\";
String query = "Einstein";
IndexRepository repository = new IndexRepository();
repository.addToRepository(indexFolder1); // 既存のインデックスをロードしています
repository.addToRepository(indexFolder2); // 別の既存インデックスをロードしています
SearchResult result = repository.search(query); // リポジトリのインデックスを検索しています
 
```
 
````


## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [IndexRepository()](#IndexRepository--) | 新しいインスタンスを初期化します |
IndexRepository
クラス。
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getEvents()](#getEvents--) | イベントの購読用ハブを取得します。 |
|
|  | [getIndexes()](#getIndexes--) | この中に含まれるインデックスを取得します |
IndexRepository
.
|
|  | [close()](#close--) | 使用されているすべてのリソースを解放します |
IndexRepository
.
|
|  | [create()](#create--) | メモリ内に新しいインデックスを作成します。 |
|
|  | [create(IndexSettings settings)](#create-com.groupdocs.search.IndexSettings-) | メモリ内に新しいインデックスを作成します。 |
|
|  | [create(String indexFolder)](#create-java.lang.String-) | ディスク上に新しいインデックスを作成します。 |
|
|  | [create(String indexFolder, IndexSettings settings)](#create-java.lang.String-com.groupdocs.search.IndexSettings-) | ディスク上に新しいインデックスを作成します。 |
|
|  | [addToRepository(Index index)](#addToRepository-com.groupdocs.search.Index-) | インデックスリポジトリにインデックスを追加します。 |
|
|  | [addToRepository(String indexFolder)](#addToRepository-java.lang.String-) | インデックスリポジトリを開き、インデックスを追加します。 |
|
|  | [update()](#update--) | リポジトリ内のすべてのインデックスを更新します。 |
|
|  | [update(UpdateOptions options)](#update-com.groupdocs.search.options.UpdateOptions-) | リポジトリ内のすべてのインデックスを更新します。 |
|
|  | [search(String query)](#search-java.lang.String-) | リポジトリのすべてのインデックスを検索します。 |
|
|  | [search(String query, SearchOptions options)](#search-java.lang.String-com.groupdocs.search.options.SearchOptions-) | リポジトリのすべてのインデックスを検索します。 |
|
|  | [search(SearchQuery query)](#search-com.groupdocs.search.SearchQuery-) | リポジトリのすべてのインデックスを検索します。 |
|
|  | [search(SearchQuery query, SearchOptions options)](#search-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-) | リポジトリのすべてのインデックスを検索します。 |
|
### IndexRepository() {#IndexRepository--}
```
public IndexRepository()
```


新しいインスタンスを初期化します
IndexRepository
クラス。


### getEvents() {#getEvents--}
```
public final EventHub getEvents()
```


イベントの購読用ハブを取得します。


**Returns:**
[EventHub](../../com.groupdocs.search.events/eventhub) - The event hub for subscribing to events.

### getIndexes() {#getIndexes--}
```
public final Index[] getIndexes()
```


この中に含まれるインデックスを取得します
IndexRepository
.


**Returns:**
com.groupdocs.search.Index[] - インデックス。

### close() {#close--}
```
public final void close()
```


使用されているすべてのリソースを解放します
IndexRepository
.


### create() {#create--}
```
public final Index create()
```


メモリ内に新しいインデックスを作成します。


**Returns:**
[Index](../../com.groupdocs.search/index) - The created index.

この例は、インデックスリポジトリを介してメモリ内にインデックスを作成する方法を示しています。

````
 ```

IndexRepository indexRepository = new IndexRepository();
Index index = indexRepository.create();
 
```
 
````


### create(IndexSettings settings) {#create-com.groupdocs.search.IndexSettings-}
```
public final Index create(IndexSettings settings)
```


メモリ内に新しいインデックスを作成します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | インデックスの設定。 |

この例は、インデックスリポジトリを介してメモリ内にインデックスを作成する方法を示しています。

````
 ```

IndexRepository indexRepository = new IndexRepository();
IndexSettings settings = new IndexSettings();
settings.setUseStopWords(false); // インデックス作成時にストップワードの使用を無効にします
Index index = indexRepository.create(settings);
 
```
 
````

|

**Returns:**
[Index](../../com.groupdocs.search/index) - The created index.

### create(String indexFolder) {#create-java.lang.String-}
```
public final Index create(String indexFolder)
```


ディスク上に新しいインデックスを作成します。
インデックス作成前にインデックスフォルダーがクリーンアップされます。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | indexFolder | java.lang.String | インデックスフォルダー。 |

この例は、インデックスリポジトリを介してディスク上にインデックスを作成する方法を示しています。

````
 ```

String indexFolder = "c:\\MyIndex\\";
IndexRepository indexRepository = new IndexRepository();
Index index = indexRepository.create(indexFolder);
 
```
 
````

|

**Returns:**
[Index](../../com.groupdocs.search/index) - The created index.

### create(String indexFolder, IndexSettings settings) {#create-java.lang.String-com.groupdocs.search.IndexSettings-}
```
public final Index create(String indexFolder, IndexSettings settings)
```


ディスク上に新しいインデックスを作成します。
インデックス作成前にインデックスフォルダーがクリーンアップされます。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | indexFolder | java.lang.String | インデックスフォルダー。 |
|
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | インデックスの設定。 |

この例は、インデックスリポジトリを介してディスク上にインデックスを作成する方法を示しています。

````
 ```

String indexFolder = "c:\\MyIndex\\";
IndexRepository indexRepository = new IndexRepository();
IndexSettings settings = new IndexSettings();
settings.setUseStopWords(false); // インデックス作成時にストップワードの使用を無効にします
Index index = indexRepository.create(indexFolder, settings);
 
```
 
````

|

**Returns:**
[Index](../../com.groupdocs.search/index) - The created index.

### addToRepository(Index index) {#addToRepository-com.groupdocs.search.Index-}
```
public final void addToRepository(Index index)
```


インデックスリポジトリにインデックスを追加します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | index | [Index](../../com.groupdocs.search/index) | 追加するインデックス。 |

この例は、インデックスリポジトリにインデックスを追加する方法を示しています。

````
 ```

Index index = new Index();
IndexRepository indexRepository = new IndexRepository();
indexRepository.addToRepository(index);
 
```
 
````

|

### addToRepository(String indexFolder) {#addToRepository-java.lang.String-}
```
public final void addToRepository(String indexFolder)
```


インデックスリポジトリを開き、インデックスを追加します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | indexFolder | java.lang.String | インデックスフォルダー。 |

この例は、インデックスリポジトリにインデックスを追加する方法を示しています。

````
 ```

String indexFolder = "c:\\MyIndex\\";
IndexRepository indexRepository = new IndexRepository();
indexRepository.addToRepository(indexFolder);
 
```
 
````

|

### update() {#update--}
```
public final void update()
```


リポジトリ内のすべてのインデックスを更新します。

この例は、リポジトリ内のインデックスを更新する方法を示しています。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // インデックスを作成しています
index.add(documentsFolder); // ドキュメントをインデックス化しています
// ドキュメントフォルダーからドキュメントを削除するか、変更するか、フォルダーに新しいドキュメントを追加します
repository.update();
 
```
 
````



### update(UpdateOptions options) {#update-com.groupdocs.search.options.UpdateOptions-}
```
public final void update(UpdateOptions options)
```


リポジトリ内のすべてのインデックスを更新します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | options | [UpdateOptions](../../com.groupdocs.search.options/updateoptions) | 更新オプションです。 |

この例は、リポジトリ内のインデックスを更新する方法を示しています。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // インデックスを作成しています
index.add(documentsFolder); // ドキュメントをインデックス化しています
// ドキュメントフォルダーからドキュメントを削除するか、変更するか、フォルダーに新しいドキュメントを追加します
UpdateOptions options = new UpdateOptions();
options.setThreads(2); // インデックス作成スレッド数を設定しています
repository.update(options);
 
```
 
````

|

### search(String query) {#search-java.lang.String-}
```
public final SearchResult search(String query)
```


リポジトリのすべてのインデックスを検索します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | query | java.lang.String | 検索クエリです。 |

この例は、インデックスリポジトリで検索を実行する方法を示しています。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // インデックスを作成しています
index.add(documentsFolder); // ドキュメントをインデックス化しています
SearchResult result = repository.search(query); // 検索中
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(String query, SearchOptions options) {#search-java.lang.String-com.groupdocs.search.options.SearchOptions-}
```
public final SearchResult search(String query, SearchOptions options)
```


リポジトリのすべてのインデックスを検索します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | query | java.lang.String | 検索クエリです。 |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | 検索オプションです。 |

この例は、インデックスリポジトリで検索を実行する方法を示しています。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // インデックスを作成しています
index.add(documentsFolder); // ドキュメントをインデックス化しています
SearchOptions options = new SearchOptions();
options.setUseCaseSensitiveSearch(true); // 大文字小文字を区別する検索フラグを設定しています
SearchResult result = repository.search(query, options); // 検索中
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchQuery query) {#search-com.groupdocs.search.SearchQuery-}
```
public final SearchResult search(SearchQuery query)
```


リポジトリのすべてのインデックスを検索します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | 検索クエリです。 |

この例は、インデックスリポジトリで検索を実行する方法を示しています。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // インデックスを作成しています
index.add(documentsFolder); // ドキュメントをインデックス化しています
SearchQuery query = SearchQuery.createWordQuery("Einstein"); // オブジェクト形式で検索クエリを作成しています
SearchResult result = repository.search(query); // 検索中
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchQuery query, SearchOptions options) {#search-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-}
```
public final SearchResult search(SearchQuery query, SearchOptions options)
```


リポジトリのすべてのインデックスを検索します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | 検索クエリです。 |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | 検索オプションです。 |

この例は、インデックスリポジトリで検索を実行する方法を示しています。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // インデックスを作成しています
index.add(documentsFolder); // ドキュメントをインデックス化しています
SearchOptions options = new SearchOptions();
options.setUseCaseSensitiveSearch(true); // 大文字小文字を区別する検索フラグを設定しています
SearchQuery query = SearchQuery.createWordQuery("Einstein"); // オブジェクト形式で検索クエリを作成しています
SearchResult result = repository.search(query, options); // 検索中
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

