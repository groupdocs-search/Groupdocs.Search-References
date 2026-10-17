---
title: "IndexRepository"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示用于组合多个索引并对其执行通用操作的容器。"
type: docs
weight: 18
url: /zh/java/com.groupdocs.search/indexrepository/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable
```
public class IndexRepository implements Closeable
```

表示用于组合多个索引并对其执行通用操作的容器。


**Learn more**

* [Search index repository](../https://docs.groupdocs.com/display/searchjava/Search+index+repository)


此示例演示了该类的典型用法。

````
 ```

String indexFolder1 = "c:\\MyIndex\\";
String indexFolder2 = "c:\\MyIndex\\";
String query = "Einstein";
IndexRepository repository = new IndexRepository();
repository.addToRepository(indexFolder1); // 加载现有索引
repository.addToRepository(indexFolder2); // 加载另一个现有索引
SearchResult result = repository.search(query); // 在仓库的索引中搜索
 
```
 
````


## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [IndexRepository()](#IndexRepository--) | 初始化一个新的实例 |
IndexRepository
类。
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getEvents()](#getEvents--) | 获取用于订阅事件的事件中心。 |
|
|  | [getIndexes()](#getIndexes--) | 获取此对象包含的索引 |
IndexRepository
.
|
|  | [close()](#close--) | 释放所使用的所有资源 |
IndexRepository
.
|
|  | [create()](#create--) | 在内存中创建一个新索引。 |
|
|  | [create(IndexSettings settings)](#create-com.groupdocs.search.IndexSettings-) | 在内存中创建一个新索引。 |
|
|  | [create(String indexFolder)](#create-java.lang.String-) | 在磁盘上创建一个新索引。 |
|
|  | [create(String indexFolder, IndexSettings settings)](#create-java.lang.String-com.groupdocs.search.IndexSettings-) | 在磁盘上创建一个新索引。 |
|
|  | [addToRepository(Index index)](#addToRepository-com.groupdocs.search.Index-) | 向索引仓库添加一个索引。 |
|
|  | [addToRepository(String indexFolder)](#addToRepository-java.lang.String-) | 打开并向索引仓库添加一个索引。 |
|
|  | [update()](#update--) | 更新仓库中的所有索引。 |
|
|  | [update(UpdateOptions options)](#update-com.groupdocs.search.options.UpdateOptions-) | 更新仓库中的所有索引。 |
|
|  | [search(String query)](#search-java.lang.String-) | 在仓库的所有索引中搜索。 |
|
|  | [search(String query, SearchOptions options)](#search-java.lang.String-com.groupdocs.search.options.SearchOptions-) | 在仓库的所有索引中搜索。 |
|
|  | [search(SearchQuery query)](#search-com.groupdocs.search.SearchQuery-) | 在仓库的所有索引中搜索。 |
|
|  | [search(SearchQuery query, SearchOptions options)](#search-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-) | 在仓库的所有索引中搜索。 |
|
### IndexRepository() {#IndexRepository--}
```
public IndexRepository()
```


初始化一个新的实例
IndexRepository
类。


### getEvents() {#getEvents--}
```
public final EventHub getEvents()
```


获取用于订阅事件的事件中心。


**Returns:**
[EventHub](../../com.groupdocs.search.events/eventhub) - The event hub for subscribing to events.

### getIndexes() {#getIndexes--}
```
public final Index[] getIndexes()
```


获取此对象包含的索引
IndexRepository
.


**Returns:**
com.groupdocs.search.Index[] - 索引。

### close() {#close--}
```
public final void close()
```


释放所使用的所有资源
IndexRepository
.


### create() {#create--}
```
public final Index create()
```


在内存中创建一个新索引。


**Returns:**
[Index](../../com.groupdocs.search/index) - The created index.

示例演示如何通过索引仓库在内存中创建索引。

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


在内存中创建一个新索引。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | 索引设置。 |

示例演示如何通过索引仓库在内存中创建索引。

````
 ```

IndexRepository indexRepository = new IndexRepository();
IndexSettings settings = new IndexSettings();
settings.setUseStopWords(false); // 在索引期间禁用停用词的使用
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


在磁盘上创建一个新索引。
索引文件夹将在创建索引之前被清理。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | indexFolder | java.lang.String | 索引文件夹。 |

示例演示如何通过索引仓库在磁盘上创建索引。

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


在磁盘上创建一个新索引。
索引文件夹将在创建索引之前被清理。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | indexFolder | java.lang.String | 索引文件夹。 |
|
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | 索引设置。 |

示例演示如何通过索引仓库在磁盘上创建索引。

````
 ```

String indexFolder = "c:\\MyIndex\\";
IndexRepository indexRepository = new IndexRepository();
IndexSettings settings = new IndexSettings();
settings.setUseStopWords(false); // 在索引期间禁用停用词的使用
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


向索引仓库添加一个索引。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | index | [Index](../../com.groupdocs.search/index) | 要添加的索引。 |

示例演示如何向索引仓库添加索引。

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


打开并向索引仓库添加一个索引。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | indexFolder | java.lang.String | 索引文件夹。 |

示例演示如何向索引仓库添加索引。

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


更新仓库中的所有索引。

该示例演示如何在仓库中更新索引。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // 创建索引
index.add(documentsFolder); // 索引文档
// 删除文档文件夹中的文档，或修改它们，或向文件夹添加新文档
repository.update();
 
```
 
````



### update(UpdateOptions options) {#update-com.groupdocs.search.options.UpdateOptions-}
```
public final void update(UpdateOptions options)
```


更新仓库中的所有索引。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | options | [UpdateOptions](../../com.groupdocs.search.options/updateoptions) | 更新选项。 |

该示例演示如何在仓库中更新索引。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // 创建索引
index.add(documentsFolder); // 索引文档
// 删除文档文件夹中的文档，或修改它们，或向文件夹添加新文档
UpdateOptions options = new UpdateOptions();
options.setThreads(2); // 设置索引线程的数量
repository.update(options);
 
```
 
````

|

### search(String query) {#search-java.lang.String-}
```
public final SearchResult search(String query)
```


在仓库的所有索引中搜索。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | query | java.lang.String | 搜索查询。 |

该示例演示如何在索引仓库中执行搜索。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // 创建索引
index.add(documentsFolder); // 索引文档
SearchResult result = repository.search(query); // 搜索中
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(String query, SearchOptions options) {#search-java.lang.String-com.groupdocs.search.options.SearchOptions-}
```
public final SearchResult search(String query, SearchOptions options)
```


在仓库的所有索引中搜索。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | query | java.lang.String | 搜索查询。 |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | 搜索选项。 |

该示例演示如何在索引仓库中执行搜索。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // 创建索引
index.add(documentsFolder); // 索引文档
SearchOptions options = new SearchOptions();
options.setUseCaseSensitiveSearch(true); // 设置区分大小写搜索的标志
SearchResult result = repository.search(query, options); // 搜索中
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchQuery query) {#search-com.groupdocs.search.SearchQuery-}
```
public final SearchResult search(SearchQuery query)
```


在仓库的所有索引中搜索。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | 搜索查询。 |

该示例演示如何在索引仓库中执行搜索。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // 创建索引
index.add(documentsFolder); // 索引文档
SearchQuery query = SearchQuery.createWordQuery("Einstein"); // 以对象形式创建搜索查询
SearchResult result = repository.search(query); // 搜索中
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchQuery query, SearchOptions options) {#search-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-}
```
public final SearchResult search(SearchQuery query, SearchOptions options)
```


在仓库的所有索引中搜索。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | 搜索查询。 |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | 搜索选项。 |

该示例演示如何在索引仓库中执行搜索。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // 创建索引
index.add(documentsFolder); // 索引文档
SearchOptions options = new SearchOptions();
options.setUseCaseSensitiveSearch(true); // 设置区分大小写搜索的标志
SearchQuery query = SearchQuery.createWordQuery("Einstein"); // 以对象形式创建搜索查询
SearchResult result = repository.search(query, options); // 搜索中
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

