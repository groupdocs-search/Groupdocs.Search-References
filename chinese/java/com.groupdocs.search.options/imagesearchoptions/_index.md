---
title: "ImageSearchOptions"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "提供反向图像搜索操作的选项。"
type: docs
weight: 24
url: /zh/java/com.groupdocs.search.options/imagesearchoptions/
---
**Inheritance:**
java.lang.Object
```
public class ImageSearchOptions
```

提供反向图像搜索操作的选项。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [ImageSearchOptions()](#ImageSearchOptions--) | 初始化 ImageSearchOptions 类的新实例。 |
|
|  | [ImageSearchOptions(Object data)](#ImageSearchOptions-java.lang.Object-) | 初始化 ImageSearchOptions 类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getHashDifferences()](#getHashDifferences--) | 获取图像哈希中最大不匹配位数。 |
|
|  | [setHashDifferences(int value)](#setHashDifferences-int-) | 设置图像哈希中最大不匹配位数。 |
|
|  | [getMaxResultCount()](#getMaxResultCount--) | 获取图像反向搜索请求的最大找到的图像数量。 |
|
|  | [setMaxResultCount(int value)](#setMaxResultCount-int-) | 设置图像反向搜索请求的最大找到的图像数量。 |
|
|  | [getSearchDocumentFilter()](#getSearchDocumentFilter--) | 获取搜索文档过滤器。 |
|
|  | [setSearchDocumentFilter(ISearchDocumentFilter value)](#setSearchDocumentFilter-com.groupdocs.search.options.ISearchDocumentFilter-) | 获取或设置搜索文档过滤器。 |
|
| [getCore()](#getCore--) |  |
### ImageSearchOptions() {#ImageSearchOptions--}
```
public ImageSearchOptions()
```


初始化 ImageSearchOptions 类的新实例。


### ImageSearchOptions(Object data) {#ImageSearchOptions-java.lang.Object-}
```
public ImageSearchOptions(Object data)
```


初始化 ImageSearchOptions 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 数据 | java.lang.Object | 序列化的数据。 |
|

### getHashDifferences() {#getHashDifferences--}
```
public int getHashDifferences()
```


获取图像哈希中最大不匹配位数。默认值为 5。


**Returns:**
int - 图像哈希中最大不匹配位的数量。

### setHashDifferences(int value) {#setHashDifferences-int-}
```
public void setHashDifferences(int value)
```


设置图像哈希中最大不匹配位的数量。默认值为 5。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | int | 图像哈希中最大不匹配位的数量。 |
|

### getMaxResultCount() {#getMaxResultCount--}
```
public int getMaxResultCount()
```


获取图像反向搜索请求中找到的最大图像数量。默认值为 1000。


**Returns:**
int - 图像反向搜索请求中找到的最大图像数量。

### setMaxResultCount(int value) {#setMaxResultCount-int-}
```
public void setMaxResultCount(int value)
```


设置图像反向搜索请求中找到的最大图像数量。默认值为 1000。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | int | 图像反向搜索请求中找到的最大图像数量。 |
|

### getSearchDocumentFilter() {#getSearchDocumentFilter--}
```
public ISearchDocumentFilter getSearchDocumentFilter()
```


获取搜索文档过滤器。SearchDocumentFilter 在包含逻辑上工作。使用 GroupDocs.Search.Options.SearchDocumentFilter 类来创建搜索文档过滤器实例。默认值为 null，这意味着将返回所有找到的文档。


**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - The search document filter.

### setSearchDocumentFilter(ISearchDocumentFilter value) {#setSearchDocumentFilter-com.groupdocs.search.options.ISearchDocumentFilter-}
```
public void setSearchDocumentFilter(ISearchDocumentFilter value)
```


获取或设置搜索文档过滤器。SearchDocumentFilter 在包含逻辑上工作。使用 GroupDocs.Search.Options.SearchDocumentFilter 类来创建搜索文档过滤器实例。默认值为 null，这意味着将返回所有找到的文档。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | value | [ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) | 搜索文档过滤器。 |
|

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
