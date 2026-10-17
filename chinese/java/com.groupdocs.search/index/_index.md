---
title: "Index"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示用于索引文档并在其中搜索的主类。"
type: docs
weight: 17
url: /zh/java/com.groupdocs.search/index/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable
```
public class Index implements Closeable
```

表示用于索引文档并在其中搜索的主类。


**Learn more**

* [Creating an index](../https://docs.groupdocs.com/display/searchjava/Creating+an+index)
* [Indexing](../https://docs.groupdocs.com/display/searchjava/Indexing)
* [Searching](../https://docs.groupdocs.com/display/searchjava/Searching)


此示例演示了该类的典型用法。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // 在指定文件夹中创建索引
index.add(documentsFolder); // 从指定文件夹索引文档
SearchResult result = index.search(query); // 在索引中搜索
 
```
 
````


## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [Index()](#Index--) | 在内存中初始化  Index  类的新实例。 |
|
|  | [Index(IndexSettings settings)](#Index-com.groupdocs.search.IndexSettings-) | 在内存中使用特定的索引设置初始化  Index  类的新实例。 |
|
|  | [Index(String indexFolder)](#Index-java.lang.String-) | 初始化  Index  类的新实例。 |
|
|  | [Index(String indexFolder, IndexSettings settings)](#Index-java.lang.String-com.groupdocs.search.IndexSettings-) | 初始化一个新的实例 |
Index
类。
|
|  | [Index(String indexFolder, boolean overwriteIfExists)](#Index-java.lang.String-boolean-) | 初始化一个新的实例 |
Index
类。
|
|  | [Index(String indexFolder, IndexSettings settings, boolean overwriteIfExists)](#Index-java.lang.String-com.groupdocs.search.IndexSettings-boolean-) | 初始化一个新的实例 |
Index
类。
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getEvents()](#getEvents--) | 获取用于订阅事件的事件中心。 |
|
|  | [getIndexInfo()](#getIndexInfo--) | 获取索引的基本信息。 |
|
|  | [getRepository()](#getRepository--) | 如果索引包含在其中，则获取索引仓库对象。 |
|
|  | [getIndexSettings()](#getIndexSettings--) | 获取索引设置。 |
|
|  | [getDictionaries()](#getDictionaries--) | 获取字典仓库。 |
|
|  | [close()](#close--) | 释放所使用的所有资源 |
Index
.
|
|  | [add(String path)](#add-java.lang.String-) | 执行索引操作。 |
|
|  | [add(String path, IndexingOptions options)](#add-java.lang.String-com.groupdocs.search.options.IndexingOptions-) | 执行索引操作。 |
|
|  | [add(String[] paths)](#add-java.lang.String---) | 执行索引操作。 |
|
|  | [add(String[] paths, IndexingOptions options)](#add-java.lang.String---com.groupdocs.search.options.IndexingOptions-) | 执行索引操作。 |
|
|  | [add(Document[] documents, IndexingOptions options)](#add-com.groupdocs.search.Document---com.groupdocs.search.options.IndexingOptions-) | 执行索引操作。 |
|
|  | [add(ExtractedData[] data, IndexingOptions options)](#add-com.groupdocs.search.ExtractedData---com.groupdocs.search.options.IndexingOptions-) | 执行索引操作。 |
|
|  | [update()](#update--) | 重新索引自上次更新后已更改或删除的文档。 |
|
|  | [update(UpdateOptions options)](#update-com.groupdocs.search.options.UpdateOptions-) | 重新索引自上次更新后已更改或删除的文档。 |
|
|  | [getIndexingReports()](#getIndexingReports--) | 获取有关索引操作的报告。 |
|
|  | [getSearchReports()](#getSearchReports--) | 获取有关搜索操作的报告。 |
|
|  | [search(String query)](#search-java.lang.String-) | 在索引中搜索。 |
|
|  | [search(String query, SearchOptions options)](#search-java.lang.String-com.groupdocs.search.options.SearchOptions-) | 在索引中搜索。 |
|
|  | [search(SearchQuery query)](#search-com.groupdocs.search.SearchQuery-) | 在索引中搜索。 |
|
|  | [search(SearchQuery query, SearchOptions options)](#search-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-) | 在索引中搜索。 |
|
|  | [search(SearchImage image, ImageSearchOptions options)](#search-com.groupdocs.search.common.SearchImage-com.groupdocs.search.options.ImageSearchOptions-) | 在索引中执行反向图像搜索。 |
|
|  | [searchNext(ChunkSearchToken chunkSearchToken)](#searchNext-com.groupdocs.search.common.ChunkSearchToken-) | 继续使用 Search 方法启动的块搜索。 |
|
|  | [searchNext(ChunkSearchToken chunkSearchToken, Cancellation cancellation)](#searchNext-com.groupdocs.search.common.ChunkSearchToken-com.groupdocs.search.common.Cancellation-) | 继续使用 Search 方法启动的块搜索。 |
|
|  | [optimize()](#optimize--) | 通过将它们相互合并来最小化索引段的数量。 |
|
|  | [optimize(MergeOptions options)](#optimize-com.groupdocs.search.options.MergeOptions-) | 通过将它们相互合并来最小化索引段的数量。 |
|
|  | [merge(Index index, MergeOptions options)](#merge-com.groupdocs.search.Index-com.groupdocs.search.options.MergeOptions-) | 将指定的索引合并到当前索引中。 |
|
|  | [merge(IndexRepository repository, MergeOptions options)](#merge-com.groupdocs.search.IndexRepository-com.groupdocs.search.options.MergeOptions-) | 将指定索引库中的索引合并到当前索引中。 |
|
|  | [highlight(FoundDocument document, Highlighter highlighter)](#highlight-com.groupdocs.search.results.FoundDocument-com.groupdocs.search.highlighters.Highlighter-) | 生成带有高亮显示的找到的词的 HTML 格式文本。 |
|
|  | [highlight(FoundDocument document, Highlighter highlighter, HighlightOptions options)](#highlight-com.groupdocs.search.results.FoundDocument-com.groupdocs.search.highlighters.Highlighter-com.groupdocs.search.options.HighlightOptions-) | 生成带有高亮显示的找到的词的 HTML 格式文本。 |
|
|  | [getIndexedDocuments()](#getIndexedDocuments--) | 获取所有已索引文档的数组。 |
|
|  | [getIndexedDocumentItems(DocumentInfo documentInfo)](#getIndexedDocumentItems-com.groupdocs.search.results.DocumentInfo-) | 获取文档项的数组。 |
|
|  | [GetIndexedDocument(String documentKey)](#GetIndexedDocument-java.lang.String-) | 通过文档键获取已索引的文档。 |
|
|  | [getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter)](#getDocumentText-com.groupdocs.search.results.DocumentInfo-com.groupdocs.search.common.OutputAdapter-) | 生成已索引文档的文本并通过输出适配器传递。 |
|
|  | [getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter, TextOptions options)](#getDocumentText-com.groupdocs.search.results.DocumentInfo-com.groupdocs.search.common.OutputAdapter-com.groupdocs.search.options.TextOptions-) | 为已索引文档生成 HTML 格式文本并通过输出适配器传输。 |
|
|  | [getIndexedPaths()](#getIndexedPaths--) | 获取已索引路径的数组——文档或文件夹。 |
|
|  | [delete(String[] paths, UpdateOptions options)](#delete-java.lang.String---com.groupdocs.search.options.UpdateOptions-) | 从索引中删除已索引的文件或文件夹。 |
|
|  | [delete(UpdateOptions options, String[] documentKeys)](#delete-com.groupdocs.search.options.UpdateOptions-java.lang.String---) | 删除从流或结构中索引的文档。 |
|
|  | [notifyIndex(Notification notification)](#notifyIndex-com.groupdocs.search.Notification-) | 将指定的通知对象传递给索引以执行通知。 |
|
|  | [changeAttributes(AttributeChangeBatch batch)](#changeAttributes-com.groupdocs.search.common.AttributeChangeBatch-) | 在更新操作期间，应用指定的属性更改批次到已索引文档，而无需重新索引。 |
|
|  | [getAttributes(String path)](#getAttributes-java.lang.String-) | 获取与指定已索引文档关联的所有属性。 |
|
|  | [loadIntoMemoryCompletely(String indexFolder)](#loadIntoMemoryCompletely-java.lang.String-) | 将整个索引加载到内存中。 |
|
|  | [loadIntoMemoryCompletely(String indexFolder, IndexSettings settings)](#loadIntoMemoryCompletely-java.lang.String-com.groupdocs.search.IndexSettings-) | 将整个索引加载到内存中。 |
|
### Index() {#Index--}
```
public Index()
```


在内存中初始化  Index  类的新实例。


示例演示如何在内存中创建索引而不将文件保存到磁盘。

````
 ```

Index index = new Index();
 
```
 
````



### Index(IndexSettings settings) {#Index-com.groupdocs.search.IndexSettings-}
```
public Index(IndexSettings settings)
```


在内存中使用特定的索引设置初始化  Index  类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | 索引设置对象。 |


示例演示如何在内存中创建索引而不将文件保存到磁盘，并使用特定的索引设置。

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


初始化 Index 类的新实例。创建一个新索引或打开磁盘上已有的索引。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | indexFolder | java.lang.String | 索引文件夹路径。 |


示例演示如何在磁盘上创建索引或打开已有的索引。

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


初始化一个新的实例
Index
类。
使用特定设置创建新索引或打开磁盘上已有的索引。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | indexFolder | java.lang.String | 索引文件夹路径。 |
|
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | 索引设置对象。 |

示例演示如何使用特定索引设置在磁盘上创建索引。

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


初始化一个新的实例
Index
类。
如果从磁盘加载已有索引
overwriteIfExists
是
false
;
否则在磁盘上创建新索引。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | indexFolder | java.lang.String | 索引文件夹路径。 |
|
|  | overwriteIfExists | boolean | 覆盖索引文件夹的标志。 |

示例演示如何在已包含另一个索引的文件夹中创建新索引。

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


初始化一个新的实例
Index
类。
如果从磁盘加载已有索引
overwriteIfExists
是
false
;
否则使用特定索引设置在磁盘上创建新索引。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | indexFolder | java.lang.String | 索引文件夹路径。 |
|
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | 索引设置对象。 |
|
|  | overwriteIfExists | boolean | 覆盖索引文件夹的标志。 |

示例演示如何使用特定索引设置在磁盘上创建索引。

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


获取用于订阅事件的事件中心。


**Returns:**
[EventHub](../../com.groupdocs.search.events/eventhub) - The event hub for subscribing to events.

### getIndexInfo() {#getIndexInfo--}
```
public final IndexInfo getIndexInfo()
```


获取索引的基本信息。


**Returns:**
[IndexInfo](../../com.groupdocs.search.common/indexinfo) - The basic information on the index.

### getRepository() {#getRepository--}
```
public final IndexRepository getRepository()
```


如果索引包含在其中，则获取索引仓库对象。


**Returns:**
[IndexRepository](../../com.groupdocs.search/indexrepository) - The index repository object.

### getIndexSettings() {#getIndexSettings--}
```
public final IndexSettings getIndexSettings()
```


获取索引设置。


**Returns:**
[IndexSettings](../../com.groupdocs.search/indexsettings) - The index settings.

### getDictionaries() {#getDictionaries--}
```
public final DictionaryRepository getDictionaries()
```


获取字典仓库。


**Returns:**
[DictionaryRepository](../../com.groupdocs.search.dictionaries/dictionaryrepository) - The dictionary repository.

### close() {#close--}
```
public final void close()
```


释放所使用的所有资源
Index
.


### add(String path) {#add-java.lang.String-}
```
public final void add(String path)
```


执行索引操作。
通过绝对或相对路径添加文件或文件夹。
所有子文件夹中的文档将被索引。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | path | java.lang.String | 要索引的文件或文件夹的路径。 |

示例演示如何向索引添加文档。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String folderPath = "c:\\MyDocuments\\";
String filePath = "c:\\Documents\\MyFile.txt";
Index index = new Index(indexFolder); // 在指定文件夹中创建索引
index.add(folderPath); // 在指定文件夹中建立索引的文档
index.add(filePath); // 对指定文档建立索引
 
```
 
````

|

### add(String path, IndexingOptions options) {#add-java.lang.String-com.groupdocs.search.options.IndexingOptions-}
```
public final void add(String path, IndexingOptions options)
```


执行索引操作。
通过绝对或相对路径添加文件或文件夹。
所有子文件夹中的文档将被索引。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | path | java.lang.String | 要索引的文件或文件夹的路径。 |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | 索引选项。 |

示例演示了如何使用特定的索引选项将文档添加到索引中。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String folderPath = "c:\\MyDocuments\\";
String filePath = "c:\\Documents\\MyFile.txt";
Index index = new Index(indexFolder); // 在指定文件夹中创建索引
IndexingOptions options = new IndexingOptions();
options.setThreads(2); // 设置索引线程的数量
index.add(folderPath, options); // 在指定文件夹中建立索引的文档
index.add(filePath, options); // 对指定文档建立索引
 
```
 
````

|

### add(String[] paths) {#add-java.lang.String---}
```
public final void add(String[] paths)
```


执行索引操作。
通过绝对或相对路径添加文件或文件夹。
所有子文件夹中的文档将被索引。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 路径 | java.lang.String[] | 要索引的文件或文件夹的路径。 |

示例演示如何向索引添加文档。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String folderPath = "c:\\MyDocuments\\";
String filePath = "c:\\Documents\\MyFile.txt";
Index index = new Index(indexFolder); // 在指定文件夹中创建索引
String[] paths = new String[] { folderPath, filePath };
index.add(paths); // 对指定路径下的文档建立索引
 
```
 
````

|

### add(String[] paths, IndexingOptions options) {#add-java.lang.String---com.groupdocs.search.options.IndexingOptions-}
```
public final void add(String[] paths, IndexingOptions options)
```


执行索引操作。
通过绝对或相对路径添加文件或文件夹。
所有子文件夹中的文档将被索引。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 路径 | java.lang.String[] | 要索引的文件或文件夹的路径。 |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | 索引选项。 |

示例演示了如何使用特定的索引选项将文档添加到索引中。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String folderPath = "c:\\MyDocuments\\";
String filePath = "c:\\Documents\\MyFile.txt";
Index index = new Index(indexFolder); // 在指定文件夹中创建索引
IndexingOptions options = new IndexingOptions();
options.setThreads(2); // 设置索引线程的数量
String[] paths = new String[] { folderPath, filePath };
index.add(paths, options); // 对指定路径下的文档建立索引
 
```
 
````

|

### add(Document[] documents, IndexingOptions options) {#add-com.groupdocs.search.Document---com.groupdocs.search.options.IndexingOptions-}
```
public final void add(Document[] documents, IndexingOptions options)
```


执行索引操作。
从文件系统、流或结构中添加文档。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | documents | [Document\[\]](../../com.groupdocs.search/document) | 来自文件系统、流或结构的文档。 |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | 索引选项。 |
|

### add(ExtractedData[] data, IndexingOptions options) {#add-com.groupdocs.search.ExtractedData---com.groupdocs.search.options.IndexingOptions-}
```
public final void add(ExtractedData[] data, IndexingOptions options)
```


执行索引操作。
将提取的数据添加到索引中。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | data | [ExtractedData\[\]](../../com.groupdocs.search/extracteddata) | 提取的数据。 |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | 索引选项。 |
|

### update() {#update--}
```
public final void update()
```


重新索引自上次更新后已更改或删除的文档。
添加已添加到已索引文件夹中的新文件。

示例演示了如何更新索引。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // 在指定文件夹中创建索引
index.add(documentsFolder); // 从指定文件夹索引文档
// 删除文档文件夹中的文档，或修改它们，或向文件夹添加新文档
index.update(); // 更新索引
 
```
 
````



### update(UpdateOptions options) {#update-com.groupdocs.search.options.UpdateOptions-}
```
public final void update(UpdateOptions options)
```


重新索引自上次更新后已更改或删除的文档。
添加已添加到已索引文件夹中的新文件。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | options | [UpdateOptions](../../com.groupdocs.search.options/updateoptions) | 更新选项。 |

示例演示了如何使用特定的更新选项更新索引。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // 在指定文件夹中创建索引
index.add(documentsFolder); // 从指定文件夹索引文档
// 删除文档文件夹中的文档，或修改它们，或向文件夹添加新文档
UpdateOptions options = new UpdateOptions();
options.setThreads(2); // 设置索引线程的数量
index.update(options); // 更新索引
 
```
 
````

|

### getIndexingReports() {#getIndexingReports--}
```
public final IndexingReport[] getIndexingReports()
```


获取有关索引操作的报告。


**Returns:**
com.groupdocs.search.common.IndexingReport[] - 索引报告。

示例演示了如何获取索引报告。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // 在指定文件夹中创建索引
index.add(documentsFolder); // 从指定文件夹索引文档
IndexingReport[] reports = index.getIndexingReports(); // 获取索引报告
 
```
 
````


### getSearchReports() {#getSearchReports--}
```
public final SearchReport[] getSearchReports()
```


获取有关搜索操作的报告。


**Returns:**
com.groupdocs.search.common.SearchReport[] - 搜索报告。

该示例演示如何获取搜索报告。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query1 = "Einstein";
String query2 = "Newton";
Index index = new Index(indexFolder); // 在指定文件夹中创建索引
index.add(documentsFolder); // 从指定文件夹索引文档
SearchResult result1 = index.search(query1); // 搜索
SearchResult result2 = index.search(query2);
SearchResult result3 = index.search(query1 + " & " + query2);
SearchReport[] reports = index.getSearchReports(); // 获取搜索报告
 
```
 
````


### search(String query) {#search-java.lang.String-}
```
public final SearchResult search(String query)
```


在索引中搜索。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | query | java.lang.String | 搜索查询。 |

以下示例演示如何执行简单搜索。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // 在指定文件夹中创建索引
index.add(documentsFolder); // 从指定文件夹索引文档
SearchResult result = index.search(query); // 搜索
 
```
 
````

以下示例演示如何执行正则表达式搜索。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // 在指定文件夹中创建索引
index.add(documentsFolder); // 从指定文件夹索引文档
String query = "^[0-9]{3,}"; // 搜索查询开头的插入符号告诉索引这是一个正则表达式查询
SearchResult result = index.search(query); // 搜索
 
```
 
````

以下示例演示如何执行分面搜索。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // 在指定文件夹中创建索引
index.add(documentsFolder); // 从指定文件夹索引文档
String query = "content:Newton"; // 查询中冒号前的单词表示要搜索的文档字段名称
SearchResult result = index.search(query); // 搜索
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(String query, SearchOptions options) {#search-java.lang.String-com.groupdocs.search.options.SearchOptions-}
```
public final SearchResult search(String query, SearchOptions options)
```


在索引中搜索。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | query | java.lang.String | 搜索查询。 |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | 搜索选项。 |

以下示例演示如何执行模糊搜索。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // 在指定文件夹中创建索引
index.add(documentsFolder); // 从指定文件夹索引文档
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // 启用模糊搜索
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1)); // 设置每个单词可能的差异数量
// 开头和结尾的双引号告诉索引这是短语搜索查询
String query = "\"The Pursuit of Happiness\"";
SearchResult result = index.search(query, options); // 正在搜索
 
```
 
````

以下示例演示如何执行同义词搜索。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // 在指定文件夹中创建索引
index.add(documentsFolder); // 从指定文件夹索引文档
SearchOptions options = new SearchOptions();
options.setUseSynonymSearch(true); // 启用同义词搜索
String query = "cry";
SearchResult result = index.search(query, options); // 正在搜索
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchQuery query) {#search-com.groupdocs.search.SearchQuery-}
```
public final SearchResult search(SearchQuery query)
```


在索引中搜索。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | 搜索查询。 |

以下示例演示如何使用对象形式的查询执行搜索。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // 在指定文件夹中创建索引
index.add(documentsFolder); // 从指定文件夹索引文档
// 创建子查询 1
SearchQuery subquery1 = SearchQuery.createWordQuery("accommodation");
subquery1.setSearchOptions(new SearchOptions()); // 仅为子查询 1 设置搜索选项
subquery1.getSearchOptions().getFuzzySearch().setEnabled(true); // 启用模糊搜索
subquery1.getSearchOptions().getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3)); // 设置最大差异数
// 创建子查询 2
SearchQuery subquery2 = SearchQuery.createNumericRangeQuery(1, 1000000);
// 创建子查询 3
SearchQuery subquery3 = SearchQuery.createRegexQuery("(.)\\1");
// 将子查询组合成一个查询
SearchQuery query = SearchQuery.createPhraseSearchQuery(subquery1, subquery2, subquery3);
SearchResult result = index.search(query); // 搜索
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchQuery query, SearchOptions options) {#search-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-}
```
public final SearchResult search(SearchQuery query, SearchOptions options)
```


在索引中搜索。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | 搜索查询。 |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | 搜索选项。 |

以下示例演示如何使用对象形式的查询执行搜索。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // 在指定文件夹中创建索引
index.add(documentsFolder); // 从指定文件夹索引文档
// 创建日期范围搜索的子查询
SearchQuery subquery1 = SearchQuery.createDateRangeQuery(new Date(2011, 6, 17), new Date(2013, 1, 1));
// 创建通配符子查询，漏词数量从 0 到 2
SearchQuery subquery2 = SearchQuery.createWildcardQuery(0, 2);
// 创建简单词的子查询
SearchQuery subquery3 = SearchQuery.createWordQuery("birth");
subquery3.setSearchOptions(new SearchOptions()); // 仅为子查询 3 设置搜索选项
subquery3.getSearchOptions().getFuzzySearch().setEnabled(true);
subquery3.getSearchOptions().getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1));
// 将子查询组合成一个查询
SearchQuery query = SearchQuery.createPhraseSearchQuery(subquery1, subquery2, subquery3);
// 创建搜索选项对象，增加已发现出现次数的容量
SearchOptions options = new SearchOptions(); // 整体搜索选项
options.setMaxOccurrenceCountPerTerm(1000000);
options.setMaxTotalOccurrenceCount(10000000);
SearchResult result = index.search(query, options); // 正在搜索
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchImage image, ImageSearchOptions options) {#search-com.groupdocs.search.common.SearchImage-com.groupdocs.search.options.ImageSearchOptions-}
```
public final ImageSearchResult search(SearchImage image, ImageSearchOptions options)
```


在索引中执行反向图像搜索。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | image | [SearchImage](../../com.groupdocs.search.common/searchimage) | 要搜索的图像。 |
|
|  | options | [ImageSearchOptions](../../com.groupdocs.search.options/imagesearchoptions) | 图像搜索选项。 |
|

**Returns:**
[ImageSearchResult](../../com.groupdocs.search.results/imagesearchresult) - The result of a reverse image search.

### searchNext(ChunkSearchToken chunkSearchToken) {#searchNext-com.groupdocs.search.common.ChunkSearchToken-}
```
public final SearchResult searchNext(ChunkSearchToken chunkSearchToken)
```


继续使用 Search 方法启动的块搜索。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | chunkSearchToken | [ChunkSearchToken](../../com.groupdocs.search.common/chunksearchtoken) | 块搜索令牌。 |

示例演示如何执行块搜索。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // 在指定文件夹中创建索引
index.add(documentsFolder); // 从指定文件夹索引文档
SearchOptions options = new SearchOptions();
options.setChunkSearch(true); // 启用块搜索
SearchResult result = index.search(query, options); // 开始块搜索
System.out.println("Document count: " + result.getDocumentCount());
System.out.println("Occurrence count: " + result.getOccurrenceCount());
while (result.getNextChunkSearchToken() != null) {
result = index.searchNext(result.getNextChunkSearchToken()); // 继续块搜索
System.out.println("Document count: " + result.getDocumentCount());
System.out.println("Occurrence count: " + result.getOccurrenceCount());
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


继续使用 Search 方法启动的块搜索。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | chunkSearchToken | [ChunkSearchToken](../../com.groupdocs.search.common/chunksearchtoken) | 块搜索令牌。 |
|
|  | cancellation | [Cancellation](../../com.groupdocs.search.common/cancellation) | 取消对象。 |

示例演示如何使用对象形式的查询执行搜索。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // 在指定文件夹中创建索引
index.add(documentsFolder); // 从指定文件夹索引文档
Cancellation cancellation = new Cancellation(); // 如果被取消，此取消对象会中止所有搜索的后续操作
SearchOptions options = new SearchOptions();
options.setChunkSearch(true); // 启用块搜索
options.setCancellation(cancellation);
SearchResult result = index.search(query, options); // 开始块搜索
System.out.println("Document count: " + result.getDocumentCount());
System.out.println("Occurrence count: " + result.getOccurrenceCount());
while (result.getNextChunkSearchToken() != null) {
result = index.searchNext(result.getNextChunkSearchToken(), cancellation); // 继续块搜索
System.out.println("Document count: " + result.getDocumentCount());
System.out.println("Occurrence count: " + result.getOccurrenceCount());
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


通过将它们相互合并来最小化索引段的数量。
此操作提升搜索性能。

示例演示如何合并索引的段。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
String documentsFolder3 = "c:\\MyDocuments3\\";
Index index = new Index(indexFolder); // 在指定文件夹中创建索引
index.add(documentsFolder1); // 从指定文件夹索引文档
index.add(documentsFolder2); // 每次调用 AddToIndex 都会在索引中创建至少一个新段
index.add(documentsFolder3);
// 合并索引的段
index.optimize();
 
```
 
````



### optimize(MergeOptions options) {#optimize-com.groupdocs.search.options.MergeOptions-}
```
public final void optimize(MergeOptions options)
```


通过将它们相互合并来最小化索引段的数量。
此操作提升搜索性能。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | options | [MergeOptions](../../com.groupdocs.search.options/mergeoptions) | 合并选项。 |

示例演示了如何使用特定的合并选项合并索引的段。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
String documentsFolder3 = "c:\\MyDocuments3\\";
Index index = new Index(indexFolder); // 在指定文件夹中创建索引
index.add(documentsFolder1); // 从指定文件夹索引文档
index.add(documentsFolder2); // 每次调用 AddToIndex 都会在索引中创建至少一个新段
index.add(documentsFolder3);
MergeOptions options = new MergeOptions();
options.setAsync(true); // 异步操作
options.setCancellation(new Cancellation()); // 创建取消对象
// 合并索引的段
index.optimize(options); // 此方法将在操作完成前返回
options.getCancellation().cancelAfter(10000); // 将操作的最大持续时间设置为 10 秒
 
```
 
````

|

### merge(Index index, MergeOptions options) {#merge-com.groupdocs.search.Index-com.groupdocs.search.options.MergeOptions-}
```
public final void merge(Index index, MergeOptions options)
```


将指定的索引合并到当前索引中。
请注意，另一个索引不会被更改。


如果另一个索引有先前的版本，必须在合并之前进行更新
IndexUpdater
.


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | index | [Index](../../com.groupdocs.search/index) | 要合并进入的索引。 |
|
|  | options | [MergeOptions](../../com.groupdocs.search.options/mergeoptions) | 合并选项。 |

示例演示了如何将索引合并到当前索引中。

````
 ```

String indexFolder1 = "c:\\MyIndex1\\";
String indexFolder2 = "c:\\MyIndex2\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
Index index1 = new Index(indexFolder1); // 创建 index1
index1.add(documentsFolder1); // 索引文档
Index index2 = new Index(indexFolder2); // 创建 index2
index2.add(documentsFolder2); // 索引文档
MergeOptions options = new MergeOptions();
options.setCancellation(new Cancellation()); // 创建取消对象
// 将 index2 合并到 index1。请注意，index2 文件不会被更改。
index1.merge(index2, options);
 
```
 
````

|

### merge(IndexRepository repository, MergeOptions options) {#merge-com.groupdocs.search.IndexRepository-com.groupdocs.search.options.MergeOptions-}
```
public final void merge(IndexRepository repository, MergeOptions options)
```


将指定索引库中的索引合并到当前索引中。
请注意，仓库中的索引将不会被更改。


如果其他索引有之前的版本，则必须在合并之前进行更新。
IndexUpdater
.


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | repository | [IndexRepository](../../com.groupdocs.search/indexrepository) | 要合并到的索引仓库。 |
|
|  | options | [MergeOptions](../../com.groupdocs.search.options/mergeoptions) | 合并选项。 |

示例演示了如何将索引仓库合并到当前索引中。

````
 ```

String indexFolder1 = "c:\\MyIndex1\\";
String indexFolder2 = "c:\\MyIndex2\\";
String indexFolder3 = "c:\\MyIndex3\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
String documentsFolder3 = "c:\\MyDocuments3\\";
Index index1 = new Index(indexFolder1); // 创建 index1
index1.add(documentsFolder1); // 索引文档
IndexRepository repository = new IndexRepository(); // 创建索引仓库
Index index2 = repository.create(indexFolder2); // 创建 index2
index2.add(documentsFolder2); // 索引文档
Index index3 = repository.create(indexFolder3); // 创建 index3
index3.add(documentsFolder3); // 索引文档
MergeOptions options = new MergeOptions();
options.setCancellation(new Cancellation()); // 创建取消对象
// 将索引仓库中的所有索引合并到 index1。请注意，index2 和 index3 将不会被更改。
index1.merge(repository, options);
 
```
 
````

|

### highlight(FoundDocument document, Highlighter highlighter) {#highlight-com.groupdocs.search.results.FoundDocument-com.groupdocs.search.highlighters.Highlighter-}
```
public final void highlight(FoundDocument document, Highlighter highlighter)
```


生成带有高亮显示的找到的词的 HTML 格式文本。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | document | [FoundDocument](../../com.groupdocs.search.results/founddocument) | 找到的文档。 |
|
|  | highlighter | [Highlighter](../../com.groupdocs.search.highlighters/highlighter) | 搜索结果高亮显示器。 |

示例演示了如何在 HTML 格式的文本中高亮出现的内容。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentFolder = "c:\\MyDocuments\\";
// 创建索引
Index index = new Index(indexFolder);
// 索引来自指定文件夹的文档
index.add(documentFolder);
// 搜索单词 'eternity'
SearchResult result = index.search("eternity");
// 高亮文本中的出现位置
if (result.getDocumentCount() > 0) {
FoundDocument document = result.getFoundDocument(0); // 获取第一个找到的文档
OutputAdapter outputAdapter = new FileOutputAdapter("c:\\Highlighted.html"); // 创建输出适配器到文件
Highlighter highlighter = new HtmlHighlighter(outputAdapter); // 创建高亮对象
index.highlight(document, highlighter); // 生成带有高亮出现的HTML格式文本
}
 
```
 
````

|

### highlight(FoundDocument document, Highlighter highlighter, HighlightOptions options) {#highlight-com.groupdocs.search.results.FoundDocument-com.groupdocs.search.highlighters.Highlighter-com.groupdocs.search.options.HighlightOptions-}
```
public final void highlight(FoundDocument document, Highlighter highlighter, HighlightOptions options)
```


生成带有高亮显示的找到的词的 HTML 格式文本。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | document | [FoundDocument](../../com.groupdocs.search.results/founddocument) | 找到的文档。 |
|
|  | highlighter | [Highlighter](../../com.groupdocs.search.highlighters/highlighter) | 搜索结果高亮显示器。 |
|
|  | options | [HighlightOptions](../../com.groupdocs.search.options/highlightoptions) | 高亮选项。 |

示例演示了如何在 HTML 格式的文本中高亮出现的内容。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentFolder = "c:\\MyDocuments\\";
// 创建索引
Index index = new Index(indexFolder);
// 索引来自指定文件夹的文档
index.add(documentFolder);
// 搜索单词 'eternity'
SearchResult result = index.search("eternity");
// 高亮文本中的出现位置
if (result.getDocumentCount() > 0) {
FoundDocument document = result.getFoundDocument(0); // 获取第一个找到的文档
OutputAdapter outputAdapter = new FileOutputAdapter("c:\\Highlighted.html"); // 创建输出适配器到文件
Highlighter highlighter = new HtmlHighlighter(outputAdapter); // 创建高亮对象
HighlightOptions options = new HighlightOptions(); // 创建高亮选项对象
options.setTermsBefore(5);
options.setTermsAfter(5);
options.setTermsTotal(15);
index.highlight(document, highlighter, options); // 生成带有高亮出现的HTML格式文本
}
 
```
 
````

|

### getIndexedDocuments() {#getIndexedDocuments--}
```
public final DocumentInfo[] getIndexedDocuments()
```


获取所有已索引文档的数组。


**Returns:**
com.groupdocs.search.results.DocumentInfo[] - 所有已索引文档的数组。

该示例演示如何从索引中获取已索引文档的列表。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// 在指定文件夹中创建索引
Index index = new Index(indexFolder);
// 索引来自指定文件夹的文档
index.add(documentsFolder);
// 获取已索引文档的列表
DocumentInfo[] documents = index.getIndexedDocuments();
 
```
 
````


### getIndexedDocumentItems(DocumentInfo documentInfo) {#getIndexedDocumentItems-com.groupdocs.search.results.DocumentInfo-}
```
public final DocumentInfo[] getIndexedDocumentItems(DocumentInfo documentInfo)
```


获取文档项的数组。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | documentInfo | [DocumentInfo](../../com.groupdocs.search.results/documentinfo) | 文档信息。 |

该示例演示如何从索引中获取已索引文档的项目列表。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// 在指定文件夹中创建索引
Index index = new Index(indexFolder);
// 索引来自指定文件夹的文档
index.add(documentsFolder);
// 获取已索引文档的列表
DocumentInfo[] documents = index.getIndexedDocuments();
for (int i = 0; i < documents.length; i++) {
DocumentInfo document = documents[i];
System.out.println(document.getFilePath());
DocumentInfo[] items = index.getIndexedDocumentItems(document); // 获取文档项的列表
for (int j = 0; j < items.length; j++) {
DocumentInfo item = items[j];
System.out.println("\t" + item.getInnerPath());
}
}
 
```
 
````

|

**Returns:**
com.groupdocs.search.results.DocumentInfo[] - 文档项的数组。

### GetIndexedDocument(String documentKey) {#GetIndexedDocument-java.lang.String-}
```
public DocumentInfo GetIndexedDocument(String documentKey)
```


通过文档键获取已索引的文档。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 文档键 | java.lang.String | 文档键。 |
|

**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - The indexed document.

### getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter) {#getDocumentText-com.groupdocs.search.results.DocumentInfo-com.groupdocs.search.common.OutputAdapter-}
```
public final void getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter)
```


生成已索引文档的文本并通过输出适配器传递。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | documentInfo | [DocumentInfo](../../com.groupdocs.search.results/documentinfo) | 已索引的文档信息。 |
|
|  | adapter | [OutputAdapter](../../com.groupdocs.search.common/outputadapter) | 输出适配器。 |

该示例演示如何从索引中获取已索引文档的文本。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// 在指定文件夹中创建索引
Index index = new Index(indexFolder);
// 索引来自指定文件夹的文档
index.add(documentsFolder);
// 获取已索引文档的列表
DocumentInfo[] documents = index.getIndexedDocuments();
// 获取文档文本
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


为已索引文档生成 HTML 格式文本并通过输出适配器传输。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | documentInfo | [DocumentInfo](../../com.groupdocs.search.results/documentinfo) | 已索引的文档信息。 |
|
|  | adapter | [OutputAdapter](../../com.groupdocs.search.common/outputadapter) | 输出适配器。 |
|
|  | options | [TextOptions](../../com.groupdocs.search.options/textoptions) | 文本检索选项。 |
|

### getIndexedPaths() {#getIndexedPaths--}
```
public final String[] getIndexedPaths()
```


获取已索引路径的数组——文档或文件夹。


**Returns:**
java.lang.String[] - 索引路径的数组。

### delete(String[] paths, UpdateOptions options) {#delete-java.lang.String---com.groupdocs.search.options.UpdateOptions-}
```
public final DeleteResult delete(String[] paths, UpdateOptions options)
```


从索引中删除已索引的文件或文件夹。然后在没有已删除路径的情况下更新索引。
请注意，如果单个文档是作为文件夹的一部分添加到索引中的，则无法从索引中删除该文档。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 路径 | java.lang.String[] | 要删除的文件或文件夹的路径。 |
|
|  | options | [UpdateOptions](../../com.groupdocs.search.options/updateoptions) | 更新选项。 |

示例演示如何从索引中删除已索引的路径。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder1 = "c:\\MyDocuments\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
// 在指定文件夹中创建索引
Index index = new Index(indexFolder);
// 从指定文件夹索引文档
index.add(documentsFolder1);
index.add(documentsFolder2);
// 从索引获取已索引的路径
String[] indexedPaths1 = index.getIndexedPaths();
// 将已索引的路径写入控制台
System.out.println("已索引的路径：");
for (String path : indexedPaths1) {
System.out.println("\t" + path);
}
// 从索引中删除索引路径
DeleteResult deleteResult = index.delete(new String[] { documentsFolder1 }, new UpdateOptions());
// 删除后获取已索引的路径
String[] indexedPaths2 = index.getIndexedPaths();
System.out.println("\n已删除的路径: " + deleteResult.getSuccessCount());
System.out.println("\nIndexed paths:");
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


删除从流或结构中索引的文档。然后在不包含已删除文档的情况下更新索引。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | options | [UpdateOptions](../../com.groupdocs.search.options/updateoptions) | 更新选项。 |
|
|  | documentKeys | java.lang.String[] | 从流或结构中添加的文档的键。 |
|

**Returns:**
[DeleteResult](../../com.groupdocs.search.results/deleteresult) - An object describing the result of deleting documents from the index.

### notifyIndex(Notification notification) {#notifyIndex-com.groupdocs.search.Notification-}
```
public final boolean notifyIndex(Notification notification)
```


将指定的通知对象传递给索引以执行通知。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | notification | [Notification](../../com.groupdocs.search/notification) | 通知对象。 |
|

**Returns:**
boolean - 如果通知成功执行则返回  true ，否则返回  false 。

### changeAttributes(AttributeChangeBatch batch) {#changeAttributes-com.groupdocs.search.common.AttributeChangeBatch-}
```
public final void changeAttributes(AttributeChangeBatch batch)
```


在更新操作期间，应用指定的属性更改批次到已索引文档，而无需重新索引。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | batch | [AttributeChangeBatch](../../com.groupdocs.search.common/attributechangebatch) | 属性更改批次。 |
|

### getAttributes(String path) {#getAttributes-java.lang.String-}
```
public final String[] getAttributes(String path)
```


获取与指定已索引文档关联的所有属性。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | path | java.lang.String | 文档路径。 |
|

**Returns:**
java.lang.String[] - 与文档关联的属性。

### loadIntoMemoryCompletely(String indexFolder) {#loadIntoMemoryCompletely-java.lang.String-}
```
public static Index loadIntoMemoryCompletely(String indexFolder)
```


将整个索引加载到内存中。
对索引的任何更改都不会自动保存到原始文件夹。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | indexFolder | java.lang.String | 索引文件夹路径。 |
|

**Returns:**
[Index](../../com.groupdocs.search/index) - The loaded in-memory index.

### loadIntoMemoryCompletely(String indexFolder, IndexSettings settings) {#loadIntoMemoryCompletely-java.lang.String-com.groupdocs.search.IndexSettings-}
```
public static Index loadIntoMemoryCompletely(String indexFolder, IndexSettings settings)
```


将整个索引加载到内存中。
对索引的任何更改都不会自动保存到原始文件夹。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | indexFolder | java.lang.String | 索引文件夹路径。 |
|
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | 索引设置对象。 |
|

**Returns:**
[Index](../../com.groupdocs.search/index) - The loaded in-memory index.

