---
title: "SearchOptions"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "提供搜索操作的选项。"
type: docs
weight: 34
url: /zh/java/com.groupdocs.search.options/searchoptions/
---
**Inheritance:**
java.lang.Object
```
public class SearchOptions
```

提供搜索操作的选项。


**Learn more**

* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [SearchOptions()](#SearchOptions--) | 初始化 SearchOptions 类的新实例。 |
|
|  | [SearchOptions(Object data)](#SearchOptions-java.lang.Object-) | 初始化 SearchOptions 类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getUseSynonymSearch()](#getUseSynonymSearch--) | 获取搜索中使用同义词的标志。 |
|
|  | [setUseSynonymSearch(boolean value)](#setUseSynonymSearch-boolean-) | 设置搜索中使用同义词的标志。 |
|
|  | [getUseHomophoneSearch()](#getUseHomophoneSearch--) | 获取搜索中使用同音词的标志。 |
|
|  | [setUseHomophoneSearch(boolean value)](#setUseHomophoneSearch-boolean-) | 设置搜索中使用同音词的标志。 |
|
|  | [getUseWordFormsSearch()](#getUseWordFormsSearch--) | 获取搜索中使用不同词形的标志。 |
|
|  | [setUseWordFormsSearch(boolean value)](#setUseWordFormsSearch-boolean-) | 设置搜索中使用不同词形的标志。 |
|
|  | [getRetrieveAttributes()](#getRetrieveAttributes--) | 获取检索到的文档关联属性的标志。 |
|
|  | [setRetrieveAttributes(boolean value)](#setRetrieveAttributes-boolean-) | 设置检索到的文档关联属性的标志。 |
|
|  | [getFuzzySearch()](#getFuzzySearch--) | 获取模糊搜索选项。 |
|
|  | [getSpellingCorrector()](#getSpellingCorrector--) | 获取拼写校正选项。 |
|
|  | [getKeyboardLayoutCorrector()](#getKeyboardLayoutCorrector--) | 获取键盘布局校正选项。 |
|
|  | [getUseCaseSensitiveSearch()](#getUseCaseSensitiveSearch--) | 获取区分大小写搜索的标志。 |
|
|  | [setUseCaseSensitiveSearch(boolean value)](#setUseCaseSensitiveSearch-boolean-) | 设置区分大小写搜索的标志。 |
|
|  | [getMaxTotalOccurrenceCount()](#getMaxTotalOccurrenceCount--) | 获取搜索查询中所有词项出现的最大总次数。 |
|
|  | [setMaxTotalOccurrenceCount(int value)](#setMaxTotalOccurrenceCount-int-) | 设置搜索查询中所有词项出现的最大总次数。 |
|
|  | [getMaxOccurrenceCountPerTerm()](#getMaxOccurrenceCountPerTerm--) | 获取搜索查询中每个词项出现的最大次数。 |
|
|  | [setMaxOccurrenceCountPerTerm(int value)](#setMaxOccurrenceCountPerTerm-int-) | 设置搜索查询中每个词项出现的最大次数。 |
|
|  | [getDateFormats()](#getDateFormats--) | 获取日期范围搜索的日期格式集合。 |
|
|  | [isChunkSearch()](#isChunkSearch--) | 获取按块搜索的标志。 |
|
|  | [setChunkSearch(boolean value)](#setChunkSearch-boolean-) | 设置按块搜索的标志。 |
|
|  | [getSearchDocumentFilter()](#getSearchDocumentFilter--) | 获取搜索文档过滤器。 |
|
|  | [setSearchDocumentFilter(ISearchDocumentFilter value)](#setSearchDocumentFilter-com.groupdocs.search.options.ISearchDocumentFilter-) | 设置搜索文档过滤器。 |
|
|  | [getCancellation()](#getCancellation--) | 获取操作取消对象。 |
|
|  | [setCancellation(Cancellation value)](#setCancellation-com.groupdocs.search.common.Cancellation-) | 设置操作取消对象。 |
|
| [getCore()](#getCore--) |  |
### SearchOptions() {#SearchOptions--}
```
public SearchOptions()
```


初始化 SearchOptions 类的新实例。


### SearchOptions(Object data) {#SearchOptions-java.lang.Object-}
```
public SearchOptions(Object data)
```


初始化 SearchOptions 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 数据 | java.lang.Object | 序列化的数据。 |
|

### getUseSynonymSearch() {#getUseSynonymSearch--}
```
public boolean getUseSynonymSearch()
```


获取搜索中使用同义词的标志。默认值为 false。


**Returns:**
布尔值 - 搜索中使用同义词的标志。

### setUseSynonymSearch(boolean value) {#setUseSynonymSearch-boolean-}
```
public void setUseSynonymSearch(boolean value)
```


设置搜索中使用同义词的标志。默认值为 false。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | boolean | 搜索中使用同义词的标志。 |
|

### getUseHomophoneSearch() {#getUseHomophoneSearch--}
```
public boolean getUseHomophoneSearch()
```


获取搜索中使用同音词的标志。默认值为 false。


**Returns:**
布尔值 - 搜索中使用同音词的标志。

### setUseHomophoneSearch(boolean value) {#setUseHomophoneSearch-boolean-}
```
public void setUseHomophoneSearch(boolean value)
```


设置搜索中使用同音词的标志。默认值为 false。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | boolean | 搜索中使用同音词的标志。 |
|

### getUseWordFormsSearch() {#getUseWordFormsSearch--}
```
public boolean getUseWordFormsSearch()
```


获取搜索中使用不同词形的标志。默认值为 false。


**Returns:**
布尔值 - 搜索中使用不同词形的标志。

### setUseWordFormsSearch(boolean value) {#setUseWordFormsSearch-boolean-}
```
public void setUseWordFormsSearch(boolean value)
```


设置搜索中使用不同词形的标志。默认值为 false。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | boolean | 在搜索中使用不同词形的标志。 |
|

### getRetrieveAttributes() {#getRetrieveAttributes--}
```
public boolean getRetrieveAttributes()
```


获取与找到的文档关联的属性检索标志。默认值为 false。


**Returns:**
boolean - 与找到的文档关联的属性检索标志。

### setRetrieveAttributes(boolean value) {#setRetrieveAttributes-boolean-}
```
public void setRetrieveAttributes(boolean value)
```


设置与找到的文档关联的属性检索标志。默认值为 false。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | boolean | 与找到的文档关联的属性检索标志。 |
|

### getFuzzySearch() {#getFuzzySearch--}
```
public FuzzySearchOptions getFuzzySearch()
```


获取模糊搜索选项。


**Returns:**
[FuzzySearchOptions](../../com.groupdocs.search.options/fuzzysearchoptions) - The fuzzy search options.

### getSpellingCorrector() {#getSpellingCorrector--}
```
public SpellingCorrectorOptions getSpellingCorrector()
```


获取拼写校正选项。


**Returns:**
[SpellingCorrectorOptions](../../com.groupdocs.search.options/spellingcorrectoroptions) - The spelling corrector options.

### getKeyboardLayoutCorrector() {#getKeyboardLayoutCorrector--}
```
public KeyboardLayoutCorrectorOptions getKeyboardLayoutCorrector()
```


获取键盘布局校正选项。


**Returns:**
[KeyboardLayoutCorrectorOptions](../../com.groupdocs.search.options/keyboardlayoutcorrectoroptions) - The keyboard layout corrector options.

### getUseCaseSensitiveSearch() {#getUseCaseSensitiveSearch--}
```
public boolean getUseCaseSensitiveSearch()
```


获取区分大小写搜索的标志。默认值为 false。


**Returns:**
boolean - 区分大小写搜索的标志。

### setUseCaseSensitiveSearch(boolean value) {#setUseCaseSensitiveSearch-boolean-}
```
public void setUseCaseSensitiveSearch(boolean value)
```


设置区分大小写搜索的标志。默认值为 false。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | boolean | 区分大小写搜索的标志。 |
|

### getMaxTotalOccurrenceCount() {#getMaxTotalOccurrenceCount--}
```
public int getMaxTotalOccurrenceCount()
```


获取搜索查询中所有词项的最大总出现次数。默认值为 500000。


**Returns:**
int - 最大总出现次数。

### setMaxTotalOccurrenceCount(int value) {#setMaxTotalOccurrenceCount-int-}
```
public void setMaxTotalOccurrenceCount(int value)
```


设置搜索查询中所有词项的最大总出现次数。默认值为 500000。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | int | 最大总出现次数。 |
|

### getMaxOccurrenceCountPerTerm() {#getMaxOccurrenceCountPerTerm--}
```
public int getMaxOccurrenceCountPerTerm()
```


获取搜索查询中每个词项的最大出现次数。默认值为 100000。


**Returns:**
int - 每个词项的最大出现次数。

### setMaxOccurrenceCountPerTerm(int value) {#setMaxOccurrenceCountPerTerm-int-}
```
public void setMaxOccurrenceCountPerTerm(int value)
```


设置搜索查询中每个词项的最大出现次数。默认值为 100000。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | int | 每个词项的最大出现次数。 |
|

### getDateFormats() {#getDateFormats--}
```
public DateFormatCollection getDateFormats()
```


获取日期范围搜索的日期格式集合。默认日期格式为 'dd.MM.yyyy'、'MM/dd/yyyy' 和 'yyyy-MM-dd'。


**Returns:**
[DateFormatCollection](../../com.groupdocs.search.options/dateformatcollection) - The collection of date formats for date range search.


示例演示如何为搜索设置日期格式。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // 在指定文件夹中创建索引
index.add(documentsFolder); // 从指定文件夹索引文档
SearchOptions options = new SearchOptions();
options.getDateFormats().clear(); // 删除默认日期格式
DateFormatElement[] elements = new DateFormatElement[] {
DateFormatElement.getMonthTwoDigits(),
DateFormatElement.getDayOfMonthTwoDigits(),
DateFormatElement.getYearFourDigits(),
};
// 创建日期格式模式 'MM/dd/yyyy'
com.groupdocs.search.DateFormat dateFormat = new com.groupdocs.search.DateFormat(elements, "/");
options.getDateFormats().addItem(dateFormat);
SearchResult result = index.search(query, options); // 在索引中搜索
 
```
 
````


### isChunkSearch() {#isChunkSearch--}
```
public boolean isChunkSearch()
```


获取分块搜索的标志。默认值为 false。


**Returns:**
boolean - 分块搜索的标志。

### setChunkSearch(boolean value) {#setChunkSearch-boolean-}
```
public void setChunkSearch(boolean value)
```


设置分块搜索的标志。默认值为 false。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | boolean | 分块搜索的标志。 |
|

### getSearchDocumentFilter() {#getSearchDocumentFilter--}
```
public ISearchDocumentFilter getSearchDocumentFilter()
```


获取搜索文档过滤器。SearchDocumentFilter 在包含逻辑上工作。使用 SearchDocumentFilter 类创建搜索文档过滤器实例。默认值为 null，表示将返回所有找到的文档。


**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - The search document filter.


示例演示如何设置文档过滤器。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments1\\";
// 在指定文件夹中创建索引
Index index = new Index(indexFolder);
// 索引文档
index.add(documentsFolder);
// 创建一个搜索文档过滤器，以跳过扩展名为 '.doc'、'.docx'、'.rtf' 的文档
SearchOptions options = new SearchOptions();
ISearchDocumentFilter fileExtensionFilter = SearchDocumentFilter.createFileExtension(\".doc\", \".docx\", \".rtf\"); // 创建文件扩展名过滤器
ISearchDocumentFilter invertedFilter = SearchDocumentFilter.createNot(fileExtensionFilter); // 反转文件扩展名过滤器
options.setSearchDocumentFilter(invertedFilter);
// 在索引中搜索
SearchResult result = index.search(\"Einstein\", options);
 
```
 
````


### setSearchDocumentFilter(ISearchDocumentFilter value) {#setSearchDocumentFilter-com.groupdocs.search.options.ISearchDocumentFilter-}
```
public void setSearchDocumentFilter(ISearchDocumentFilter value)
```


设置搜索文档过滤器。SearchDocumentFilter 在包含逻辑上工作。使用 SearchDocumentFilter 类来创建搜索文档过滤器实例。默认值为 null，这意味着将返回所有找到的文档。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | value | [ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) | 搜索文档过滤器。 |


示例演示如何设置文档过滤器。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments1\\";
// 在指定文件夹中创建索引
Index index = new Index(indexFolder);
// 索引文档
index.add(documentsFolder);
// 创建一个搜索文档过滤器，以跳过扩展名为 '.doc'、'.docx'、'.rtf' 的文档
SearchOptions options = new SearchOptions();
ISearchDocumentFilter fileExtensionFilter = SearchDocumentFilter.createFileExtension(\".doc\", \".docx\", \".rtf\"); // 创建文件扩展名过滤器
ISearchDocumentFilter invertedFilter = SearchDocumentFilter.createNot(fileExtensionFilter); // 反转文件扩展名过滤器
options.setSearchDocumentFilter(invertedFilter);
// 在索引中搜索
SearchResult result = index.search(\"Einstein\", options);
 
```
 
````

|

### getCancellation() {#getCancellation--}
```
public Cancellation getCancellation()
```


获取操作取消对象。默认值为 null。


**Returns:**
[Cancellation](../../com.groupdocs.search.common/cancellation) - The operation cancellation object.

### setCancellation(Cancellation value) {#setCancellation-com.groupdocs.search.common.Cancellation-}
```
public void setCancellation(Cancellation value)
```


设置操作取消对象。默认值为 null。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | value | [Cancellation](../../com.groupdocs.search.common/cancellation) | 操作取消对象。 |
|

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
