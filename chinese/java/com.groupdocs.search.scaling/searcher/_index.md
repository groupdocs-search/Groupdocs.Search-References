---
title: "Searcher"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示管理向搜索网络分片发送搜索查询的服务。"
type: docs
weight: 12
url: /zh/java/com.groupdocs.search.scaling/searcher/
---
**Inheritance:**
java.lang.Object
```
public abstract class Searcher
```

表示管理向搜索网络分片发送搜索查询的服务。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [Searcher()](#Searcher--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [searchFirst(String query, SearchOptions options)](#searchFirst-java.lang.String-com.groupdocs.search.options.SearchOptions-) | 在分布式搜索索引中使用文本形式的查询启动搜索。 |
|
|  | [searchFirst(SearchQuery query, SearchOptions options)](#searchFirst-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-) | 在分布式搜索索引中启动搜索。 |
|
|  | [searchFirst(SearchImage image, ImageSearchOptions options)](#searchFirst-com.groupdocs.search.common.SearchImage-com.groupdocs.search.options.ImageSearchOptions-) | 在分布式搜索索引中执行反向图像搜索。 |
|
|  | [searchNext(NetworkSearchToken networkSearchToken)](#searchNext-com.groupdocs.search.scaling.results.NetworkSearchToken-) | 继续在分布式搜索索引中进行搜索。 |
|
|  | [searchNext(NetworkImageSearchToken networkImageSearchToken)](#searchNext-com.groupdocs.search.scaling.results.NetworkImageSearchToken-) | 继续在分布式搜索索引中进行反向图像搜索。 |
|
|  | [highlight(NetworkFoundDocument document, Highlighter highlighter, HighlightOptions options)](#highlight-com.groupdocs.search.scaling.results.NetworkFoundDocument-com.groupdocs.search.highlighters.Highlighter-com.groupdocs.search.options.HighlightOptions-) | 生成带有高亮显示的找到的词的 HTML 格式文本。 |
|
|  | [getIndexedDocuments(int shardIndex)](#getIndexedDocuments-int-) | 获取所有已索引文档的数组。 |
|
|  | [getIndexedDocumentItems(NetworkDocumentInfo documentInfo)](#getIndexedDocumentItems-com.groupdocs.search.scaling.results.NetworkDocumentInfo-) | 获取指定文档的嵌套项数组（用于 ZIP、OST、PST 等容器文档）。 |
|
|  | [getDocumentText(NetworkDocumentInfo documentInfo, OutputAdapter adapter)](#getDocumentText-com.groupdocs.search.scaling.results.NetworkDocumentInfo-com.groupdocs.search.common.OutputAdapter-) | 生成已索引文档的文本并通过输出适配器传递。 |
|
### Searcher() {#Searcher--}
```
public Searcher()
```


### searchFirst(String query, SearchOptions options) {#searchFirst-java.lang.String-com.groupdocs.search.options.SearchOptions-}
```
public abstract NetworkSearchResult searchFirst(String query, SearchOptions options)
```


在分布式搜索索引中使用文本形式的查询启动搜索。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | query | java.lang.String | 搜索查询。 |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | 搜索选项。 |
|

**Returns:**
[NetworkSearchResult](../../com.groupdocs.search.scaling.results/networksearchresult) - The search result.

### searchFirst(SearchQuery query, SearchOptions options) {#searchFirst-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-}
```
public abstract NetworkSearchResult searchFirst(SearchQuery query, SearchOptions options)
```


在分布式搜索索引中启动搜索。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | 搜索查询。 |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | 搜索选项。 |
|

**Returns:**
[NetworkSearchResult](../../com.groupdocs.search.scaling.results/networksearchresult) - The search result.

### searchFirst(SearchImage image, ImageSearchOptions options) {#searchFirst-com.groupdocs.search.common.SearchImage-com.groupdocs.search.options.ImageSearchOptions-}
```
public abstract NetworkImageSearchResult searchFirst(SearchImage image, ImageSearchOptions options)
```


在分布式搜索索引中执行反向图像搜索。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | image | [SearchImage](../../com.groupdocs.search.common/searchimage) | 要搜索的图像。 |
|
|  | options | [ImageSearchOptions](../../com.groupdocs.search.options/imagesearchoptions) | 图像搜索选项。 |
|

**Returns:**
[NetworkImageSearchResult](../../com.groupdocs.search.scaling.results/networkimagesearchresult) - The reverse image search result.

### searchNext(NetworkSearchToken networkSearchToken) {#searchNext-com.groupdocs.search.scaling.results.NetworkSearchToken-}
```
public abstract NetworkSearchResult searchNext(NetworkSearchToken networkSearchToken)
```


继续在分布式搜索索引中进行搜索。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | networkSearchToken | [NetworkSearchToken](../../com.groupdocs.search.scaling.results/networksearchtoken) | 网络搜索令牌。 |
|

**Returns:**
[NetworkSearchResult](../../com.groupdocs.search.scaling.results/networksearchresult) - The search result.

### searchNext(NetworkImageSearchToken networkImageSearchToken) {#searchNext-com.groupdocs.search.scaling.results.NetworkImageSearchToken-}
```
public abstract NetworkImageSearchResult searchNext(NetworkImageSearchToken networkImageSearchToken)
```


继续在分布式搜索索引中进行反向图像搜索。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | networkImageSearchToken | [NetworkImageSearchToken](../../com.groupdocs.search.scaling.results/networkimagesearchtoken) | 网络图像搜索令牌。 |
|

**Returns:**
[NetworkImageSearchResult](../../com.groupdocs.search.scaling.results/networkimagesearchresult) - The reverse image search result.

### highlight(NetworkFoundDocument document, Highlighter highlighter, HighlightOptions options) {#highlight-com.groupdocs.search.scaling.results.NetworkFoundDocument-com.groupdocs.search.highlighters.Highlighter-com.groupdocs.search.options.HighlightOptions-}
```
public abstract void highlight(NetworkFoundDocument document, Highlighter highlighter, HighlightOptions options)
```


生成带有高亮显示的找到的词的 HTML 格式文本。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | document | [NetworkFoundDocument](../../com.groupdocs.search.scaling.results/networkfounddocument) | 找到的文档。 |
|
|  | highlighter | [Highlighter](../../com.groupdocs.search.highlighters/highlighter) | 搜索结果高亮显示器。 |
|
|  | options | [HighlightOptions](../../com.groupdocs.search.options/highlightoptions) | 高亮选项。 |
|

### getIndexedDocuments(int shardIndex) {#getIndexedDocuments-int-}
```
public abstract NetworkDocumentInfo[] getIndexedDocuments(int shardIndex)
```


获取所有已索引文档的数组。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | shardIndex | int | 分片索引。 |
|

**Returns:**
com.groupdocs.search.scaling.results.NetworkDocumentInfo[] - 所有已索引文档的数组。

### getIndexedDocumentItems(NetworkDocumentInfo documentInfo) {#getIndexedDocumentItems-com.groupdocs.search.scaling.results.NetworkDocumentInfo-}
```
public abstract NetworkDocumentInfo[] getIndexedDocumentItems(NetworkDocumentInfo documentInfo)
```


获取指定文档的嵌套项数组（用于 ZIP、OST、PST 等容器文档）。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | documentInfo | [NetworkDocumentInfo](../../com.groupdocs.search.scaling.results/networkdocumentinfo) | 文档信息。 |
|

**Returns:**
com.groupdocs.search.scaling.results.NetworkDocumentInfo[] - 文档项的数组。

### getDocumentText(NetworkDocumentInfo documentInfo, OutputAdapter adapter) {#getDocumentText-com.groupdocs.search.scaling.results.NetworkDocumentInfo-com.groupdocs.search.common.OutputAdapter-}
```
public abstract void getDocumentText(NetworkDocumentInfo documentInfo, OutputAdapter adapter)
```


生成已索引文档的文本并通过输出适配器传递。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | documentInfo | [NetworkDocumentInfo](../../com.groupdocs.search.scaling.results/networkdocumentinfo) | 已索引的文档信息。 |
|
|  | adapter | [OutputAdapter](../../com.groupdocs.search.common/outputadapter) | 输出适配器。 |
|

