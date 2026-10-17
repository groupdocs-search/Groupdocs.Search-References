---
title: "IndexSettings"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示允许自定义索引操作的索引设置。"
type: docs
weight: 19
url: /zh/java/com.groupdocs.search/indexsettings/
---
**Inheritance:**
java.lang.Object
```
public class IndexSettings
```

表示允许自定义索引操作的索引设置。


**Learn more**

* [Search index settings](../https://docs.groupdocs.com/display/searchjava/Search+index+settings)


此示例演示了该类的典型用法。

````
 ```

String indexFolder = "c:\\MyIndex\\";
IndexSettings settings = new IndexSettings();
settings.setIndexType(IndexType.CompactIndex); // 设置索引类型
Index index = new Index(indexFolder, settings); // 创建索引
 
```
 
````


## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [IndexSettings()](#IndexSettings--) | 初始化 IndexSettings 类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getInMemoryIndex()](#getInMemoryIndex--) | 获取一个值，指示索引是存储在内存中还是磁盘上。 |
|
|  | [getUseStopWords()](#getUseStopWords--) | 获取一个值，指示是否使用停用词。 |
|
|  | [setUseStopWords(boolean value)](#setUseStopWords-boolean-) | 设置一个值，指示是否使用停用词。 |
|
|  | [getMaxIndexingReportCount()](#getMaxIndexingReportCount--) | 获取索引报告的最大数量。 |
|
|  | [setMaxIndexingReportCount(int value)](#setMaxIndexingReportCount-int-) | 设置索引报告的最大数量。 |
|
|  | [getMaxSearchReportCount()](#getMaxSearchReportCount--) | 获取搜索报告的最大数量。 |
|
|  | [setMaxSearchReportCount(int value)](#setMaxSearchReportCount-int-) | 设置搜索报告的最大数量。 |
|
|  | [getUseCharacterReplacements()](#getUseCharacterReplacements--) | 获取一个值，指示是否使用字符替换。 |
|
|  | [setUseCharacterReplacements(boolean value)](#setUseCharacterReplacements-boolean-) | 设置一个值，指示是否使用字符替换。 |
|
|  | [getDocumentFilter()](#getDocumentFilter--) | 获取文档过滤器。 |
|
|  | [setDocumentFilter(DocumentFilter value)](#setDocumentFilter-com.groupdocs.search.DocumentFilter-) | 设置文档过滤器。 |
|
|  | [getTextStorageSettings()](#getTextStorageSettings--) | 获取文本存储设置。 |
|
|  | [setTextStorageSettings(TextStorageSettings value)](#setTextStorageSettings-com.groupdocs.search.options.TextStorageSettings-) | 设置文本存储设置。 |
|
|  | [getIndexType()](#getIndexType--) | 获取索引类型。 |
|
|  | [setIndexType(IndexType value)](#setIndexType-com.groupdocs.search.options.IndexType-) | 设置索引类型。 |
|
|  | [getSearchThreads()](#getSearchThreads--) | 获取用于搜索的线程数。 |
|
|  | [setSearchThreads(NumberOfThreads value)](#setSearchThreads-com.groupdocs.search.options.NumberOfThreads-) | 设置用于搜索的线程数。 |
|
|  | [getCustomExtractors()](#getCustomExtractors--) | 获取自定义提取器集合。 |
|
|  | [getLogger()](#getLogger--) | 获取用于记录索引中事件和错误的日志记录器。 |
|
|  | [setLogger(ILogger value)](#setLogger-com.groupdocs.search.common.ILogger-) | 设置用于记录索引中事件和错误的日志记录器。 |
|
### IndexSettings() {#IndexSettings--}
```
public IndexSettings()
```


初始化 IndexSettings 类的新实例。


### getInMemoryIndex() {#getInMemoryIndex--}
```
public final boolean getInMemoryIndex()
```


获取一个值，指示索引是存储在内存中还是磁盘上。


**Returns:**
boolean - 表示索引是存储在内存还是磁盘中的值。

### getUseStopWords() {#getUseStopWords--}
```
public final boolean getUseStopWords()
```


获取一个指示是否使用停用词的值。默认值为 true。


**Returns:**
boolean - 表示是否使用停用词的值。

### setUseStopWords(boolean value) {#setUseStopWords-boolean-}
```
public final void setUseStopWords(boolean value)
```


设置一个指示是否使用停用词的值。默认值为 true。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | boolean | 指示是否使用停用词的值。 |
|

### getMaxIndexingReportCount() {#getMaxIndexingReportCount--}
```
public final int getMaxIndexingReportCount()
```


获取索引报告的最大数量。默认值为 5。


**Returns:**
int - 索引报告的最大数量。

### setMaxIndexingReportCount(int value) {#setMaxIndexingReportCount-int-}
```
public final void setMaxIndexingReportCount(int value)
```


设置索引报告的最大数量。默认值为 5。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | int | 索引报告的最大数量。 |
|

### getMaxSearchReportCount() {#getMaxSearchReportCount--}
```
public final int getMaxSearchReportCount()
```


获取搜索报告的最大数量。默认值为 10。


**Returns:**
int - 搜索报告的最大数量。

### setMaxSearchReportCount(int value) {#setMaxSearchReportCount-int-}
```
public final void setMaxSearchReportCount(int value)
```


设置搜索报告的最大数量。默认值为 10。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | int | 搜索报告的最大数量。 |
|

### getUseCharacterReplacements() {#getUseCharacterReplacements--}
```
public final boolean getUseCharacterReplacements()
```


获取一个指示是否使用字符替换的值。默认值为 false。


**Returns:**
boolean - 表示是否使用字符替换的值。

### setUseCharacterReplacements(boolean value) {#setUseCharacterReplacements-boolean-}
```
public final void setUseCharacterReplacements(boolean value)
```


设置一个指示是否使用字符替换的值。默认值为 false。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | boolean | 指示是否使用字符替换的值。 |
|

### getDocumentFilter() {#getDocumentFilter--}
```
public final DocumentFilter getDocumentFilter()
```


获取文档过滤器。DocumentFilter 在包含逻辑上工作。使用 DocumentFilter 类来创建文档过滤器实例。默认值为 null，这意味着所有添加的文档都会被索引。


**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - The document filter.

示例演示如何设置文档过滤器。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// 创建一个过滤器，跳过扩展名为 '.doc'、'.docx'、'.rtf' 的文档
IndexSettings settings = new IndexSettings();
DocumentFilter fileExtensionFilter = DocumentFilter.createFileExtension(".doc", ".docx", ".rtf"); // 创建文件扩展过滤器
DocumentFilter invertedFilter = DocumentFilter.createNot(fileExtensionFilter); // 反转文件扩展过滤器
settings.setDocumentFilter(invertedFilter);
// 在指定文件夹中创建索引
Index index = new Index(indexFolder, settings);
// 索引文档
index.add(documentsFolder);
// 搜索
SearchResult result = index.search("Einstein");
 
```
 
````


### setDocumentFilter(DocumentFilter value) {#setDocumentFilter-com.groupdocs.search.DocumentFilter-}
```
public final void setDocumentFilter(DocumentFilter value)
```


设置文档过滤器。DocumentFilter 在包含逻辑上工作。使用 GroupDocs.Search.Options.DocumentFilter 类来创建文档过滤器实例。默认值为 null，这意味着所有已添加的文档都会被索引。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | value | [DocumentFilter](../../com.groupdocs.search/documentfilter) | 文档过滤器。 |

示例演示如何设置文档过滤器。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// 创建一个过滤器，跳过扩展名为 '.doc'、'.docx'、'.rtf' 的文档
IndexSettings settings = new IndexSettings();
DocumentFilter fileExtensionFilter = DocumentFilter.createFileExtension(".doc", ".docx", ".rtf"); // 创建文件扩展过滤器
DocumentFilter invertedFilter = DocumentFilter.createNot(fileExtensionFilter); // 反转文件扩展过滤器
settings.setDocumentFilter(invertedFilter);
// 在指定文件夹中创建索引
Index index = new Index(indexFolder, settings);
// 索引文档
index.add(documentsFolder);
// 搜索
SearchResult result = index.search("Einstein");
 
```
 
````

|

### getTextStorageSettings() {#getTextStorageSettings--}
```
public final TextStorageSettings getTextStorageSettings()
```


获取文本存储设置。默认值为 null，这意味着文档文本不会被存储。


**Returns:**
[TextStorageSettings](../../com.groupdocs.search.options/textstoragesettings) - The text storage settings.

示例演示如何设置文本存储设置。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// 创建索引设置实例
IndexSettings settings = new IndexSettings();
settings.setTextStorageSettings(new TextStorageSettings(Compression.High)); // 为索引文本存储设置高压缩级别
// 在指定文件夹中创建索引
Index index = new Index(indexFolder, settings);
// 索引文档
index.add(documentsFolder);
// 搜索
SearchResult result = index.search("Einstein");
 
```
 
````


### setTextStorageSettings(TextStorageSettings value) {#setTextStorageSettings-com.groupdocs.search.options.TextStorageSettings-}
```
public final void setTextStorageSettings(TextStorageSettings value)
```


设置文本存储设置。默认值为 null，这意味着文档文本不会被存储。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | value | [TextStorageSettings](../../com.groupdocs.search.options/textstoragesettings) | 文本存储设置。 |

示例演示如何设置文本存储设置。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// 创建索引设置实例
IndexSettings settings = new IndexSettings();
settings.setTextStorageSettings(new TextStorageSettings(Compression.High)); // 为索引文本存储设置高压缩级别
// 在指定文件夹中创建索引
Index index = new Index(indexFolder, settings);
// 索引文档
index.add(documentsFolder);
// 搜索
SearchResult result = index.search("Einstein");
 
```
 
````

|

### getIndexType() {#getIndexType--}
```
public final IndexType getIndexType()
```


获取索引类型。默认值为 GroupDocs.Search.Options.IndexType.NormalIndex。


**Returns:**
[IndexType](../../com.groupdocs.search.options/indextype) - The index type.

### setIndexType(IndexType value) {#setIndexType-com.groupdocs.search.options.IndexType-}
```
public final void setIndexType(IndexType value)
```


设置索引类型。默认值为 GroupDocs.Search.Options.IndexType.NormalIndex。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | value | [IndexType](../../com.groupdocs.search.options/indextype) | 索引类型。 |
|

### getSearchThreads() {#getSearchThreads--}
```
public final NumberOfThreads getSearchThreads()
```


获取搜索使用的线程数。默认值为 GroupDocs.Search.Options.NumberOfThreads.Default，这意味着搜索将使用等于处理器核心数的线程数进行。


**Returns:**
[NumberOfThreads](../../com.groupdocs.search.options/numberofthreads) - The number of threads used for the search.

### setSearchThreads(NumberOfThreads value) {#setSearchThreads-com.groupdocs.search.options.NumberOfThreads-}
```
public final void setSearchThreads(NumberOfThreads value)
```


设置搜索使用的线程数。默认值为 GroupDocs.Search.Options.NumberOfThreads.Default，这意味着搜索将使用等于处理器核心数的线程数进行。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | value | [NumberOfThreads](../../com.groupdocs.search.options/numberofthreads) | 搜索使用的线程数。 |
|

### getCustomExtractors() {#getCustomExtractors--}
```
public final CustomExtractorCollection getCustomExtractors()
```


获取自定义提取器集合。实现自定义提取器的完整示例在 GroupDocs.Search.Common.IFieldExtractor 接口的文档中提供。


**Returns:**
[CustomExtractorCollection](../../com.groupdocs.search.common/customextractorcollection) - The custom extractor collection.

### getLogger() {#getLogger--}
```
public final ILogger getLogger()
```


获取用于在索引中记录事件和错误的日志记录器。请注意，日志记录器不会被保存，必须在每次创建或加载索引时创建并分配。


**Returns:**
[ILogger](../../com.groupdocs.search.common/ilogger) - A logger that is used for logging events and errors in the index.

### setLogger(ILogger value) {#setLogger-com.groupdocs.search.common.ILogger-}
```
public final void setLogger(ILogger value)
```


设置一个用于记录索引中事件和错误的日志记录器。请注意，日志记录器不会被保存，必须在每次创建或加载索引时创建并分配。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | value | [ILogger](../../com.groupdocs.search.common/ilogger) | 用于记录索引中事件和错误的日志记录器。 |
|

