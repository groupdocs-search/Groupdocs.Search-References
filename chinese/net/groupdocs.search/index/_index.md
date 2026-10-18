---
title: "Index"
second_title: "GroupDocs.Search for .NET API 参考"
description: "表示用于索引文档并在其上搜索的主类。"
type: docs
weight: 700
url: /zh/net/groupdocs.search/index/
---
## Index class

表示用于索引文档并在其上搜索的主类。

```csharp
public class Index : IDisposable
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [Index](index#constructor)() | 在内存中初始化一个新的 [`Index`](../index) 类实例。 |
| [Index](index#constructor_1)(IndexSettings) | 在内存中使用特定索引设置初始化一个新的 [`Index`](../index) 类实例。 |
| [Index](index#constructor_2)(string) | 初始化一个新的 [`Index`](../index) 类实例。创建一个新的或打开磁盘上已有的索引。 |
| [Index](index#constructor_3)(string, bool) | 初始化 [`Index`](../index) 类的新实例。如果 *overwriteIfExists* 为 `false`，则从磁盘加载现有索引；否则在磁盘上创建新索引。 |
| [Index](index#constructor_4)(string, IndexSettings) | 初始化 [`Index`](../index) 类的新实例。使用特定设置创建新索引或打开磁盘上的现有索引。 |
| [Index](index#constructor_5)(string, IndexSettings, bool) | 初始化 [`Index`](../index) 类的新实例。如果 *overwriteIfExists* 为 `false`，则从磁盘加载现有索引；否则使用特定索引设置在磁盘上创建新索引。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [Dictionaries](../../groupdocs.search/index/dictionaries) { get; } | 获取字典仓库。 |
| [Events](../../groupdocs.search/index/events) { get; } | 获取用于订阅事件的事件中心。 |
| [IndexInfo](../../groupdocs.search/index/indexinfo) { get; } | 获取索引的基本信息。 |
| [IndexSettings](../../groupdocs.search/index/indexsettings) { get; } | 获取索引设置。 |
| [Repository](../../groupdocs.search/index/repository) { get; } | 如果索引包含在其中，则获取索引仓库对象。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| static [LoadIntoMemoryCompletely](../../groupdocs.search/index/loadintomemorycompletely#loadintomemorycompletely)(string) | 将整个索引加载到内存中。对索引的任何更改不会自动保存到原始文件夹。 |
| static [LoadIntoMemoryCompletely](../../groupdocs.search/index/loadintomemorycompletely#loadintomemorycompletely_1)(string, IndexSettings) | 将整个索引加载到内存中。对索引的任何更改不会自动保存到原始文件夹。 |
| [Add](../../groupdocs.search/index/add#add_2)(string) | 执行索引操作。通过绝对或相对路径添加文件或文件夹。所有子文件夹中的文档都将被索引。 |
| [Add](../../groupdocs.search/index/add#add_4)(string[]) | 执行索引操作。通过绝对或相对路径添加文件或文件夹。所有子文件夹中的文档都将被索引。 |
| [Add](../../groupdocs.search/index/add#add)(Document[], IndexingOptions) | 执行索引操作。从文件系统、流或结构中添加文档。 |
| [Add](../../groupdocs.search/index/add#add_1)(ExtractedData[], IndexingOptions) | 执行索引操作。将提取的数据添加到索引中。 |
| [Add](../../groupdocs.search/index/add#add_3)(string, IndexingOptions) | 执行索引操作。通过绝对或相对路径添加文件或文件夹。所有子文件夹中的文档都将被索引。 |
| [Add](../../groupdocs.search/index/add#add_5)(string[], IndexingOptions) | 执行索引操作。通过绝对或相对路径添加文件或文件夹。所有子文件夹中的文档都将被索引。 |
| [ChangeAttributes](../../groupdocs.search/index/changeattributes)(AttributeChangeBatch) | 在更新操作期间，不进行重新索引，将指定批次的属性更改应用于已索引的文档。 |
| [CheckSegments](../../groupdocs.search/index/checksegments)(bool) | 检查磁盘上索引的损坏段文件。如果 *fixIndexFunctionality* 为 true，方法会在存在损坏段的情况下修复索引功能；否则不修复。 |
| [Delete](../../groupdocs.search/index/delete#delete_1)(string[], UpdateOptions) | 从索引中删除已索引的文件或文件夹。然后在不包含已删除路径的情况下更新索引。请注意，如果文档是作为文件夹的一部分添加到索引的，则无法单独删除该文档。 |
| [Delete](../../groupdocs.search/index/delete#delete)(UpdateOptions, string[]) | 删除从流或结构中索引的文档。然后在不包含已删除文档的情况下更新索引。 |
| [Dispose](../../groupdocs.search/index/dispose)() | 释放 [`Index`](../index) 使用的所有资源。 |
| [GetAttributes](../../groupdocs.search/index/getattributes)(string) | 获取与指定已索引文档关联的所有属性。 |
| [GetDocumentText](../../groupdocs.search/index/getdocumenttext#getdocumenttext)(DocumentInfo, OutputAdapter) | 生成已索引文档的文本并通过输出适配器传递。 |
| [GetDocumentText](../../groupdocs.search/index/getdocumenttext#getdocumenttext_1)(DocumentInfo, OutputAdapter, TextOptions) | 为已索引文档生成 HTML 格式的文本并通过输出适配器传输。 |
| [GetIndexedDocument](../../groupdocs.search/index/getindexeddocument)(string) | 通过文档键获取已索引文档。 |
| [GetIndexedDocumentItems](../../groupdocs.search/index/getindexeddocumentitems)(DocumentInfo) | 获取指定文档的嵌套项数组（用于如 ZIP、OST、PST 等容器文档）。 |
| [GetIndexedDocuments](../../groupdocs.search/index/getindexeddocuments)() | 获取所有已索引文档的数组。 |
| [GetIndexedPaths](../../groupdocs.search/index/getindexedpaths)() | 获取已索引路径的数组——文档或文件夹。 |
| [GetIndexingReports](../../groupdocs.search/index/getindexingreports)() | 获取索引操作的报告。 |
| [GetSearchReports](../../groupdocs.search/index/getsearchreports)() | 获取关于搜索操作的报告。 |
| [Highlight](../../groupdocs.search/index/highlight#highlight)(FoundDocument, Highlighter) | 生成带有突出显示的已找到词汇的 HTML 格式文本。 |
| [Highlight](../../groupdocs.search/index/highlight#highlight_1)(FoundDocument, Highlighter, HighlightOptions) | 生成带有突出显示的已找到词汇的 HTML 格式文本。 |
| [Merge](../../groupdocs.search/index/merge#merge)(Index, MergeOptions) | 将指定的索引合并到当前索引中。请注意，另一个索引不会被更改。 |
| [Merge](../../groupdocs.search/index/merge#merge_1)(IndexRepository, MergeOptions) | 将指定索引库中的索引合并到当前索引中。请注意，库中的索引不会被更改。 |
| [Notify](../../groupdocs.search/index/notify)(Notification) | 将指定的通知对象传递给索引以执行通知。 |
| [Optimize](../../groupdocs.search/index/optimize#optimize)() | 通过相互合并来最小化索引段的数量。此操作可提升搜索性能。 |
| [Optimize](../../groupdocs.search/index/optimize#optimize_1)(MergeOptions) | 通过相互合并来最小化索引段的数量。此操作可提升搜索性能。 |
| [SaveTo](../../groupdocs.search/index/saveto)(string) | 将内存中的索引保存到磁盘。同时将常规索引保存到另一个文件夹。不会更改此索引的设置。 |
| [Search](../../groupdocs.search/index/search#search_1)(SearchQuery) | 在索引中搜索。 |
| [Search](../../groupdocs.search/index/search#search_3)(string) | 在索引中搜索。 |
| [Search](../../groupdocs.search/index/search#search)(SearchImage, ImageSearchOptions) | 在索引中执行反向图像搜索。 |
| [Search](../../groupdocs.search/index/search#search_2)(SearchQuery, SearchOptions) | 在索引中搜索。 |
| [Search](../../groupdocs.search/index/search#search_4)(string, SearchOptions) | 在索引中搜索。 |
| [SearchNext](../../groupdocs.search/index/searchnext#searchnext)(ChunkSearchToken) | 继续使用 Search 方法启动的块搜索。 |
| [SearchNext](../../groupdocs.search/index/searchnext#searchnext_1)(ChunkSearchToken, Cancellation) | 继续使用 Search 方法启动的块搜索。 |
| [Update](../../groupdocs.search/index/update#update)() | 重新索引自上次更新后已更改或删除的文档。添加已添加到已索引文件夹中的新文件。 |
| [Update](../../groupdocs.search/index/update#update_1)(UpdateOptions) | 重新索引自上次更新后已更改或删除的文档。添加已添加到已索引文件夹中的新文件。 |

### 备注

**Learn more**

* [Creating an index](https://docs.groupdocs.com/display/searchnet/Creating+an+index)
* [Indexing](https://docs.groupdocs.com/display/searchnet/Indexing)
* [Searching](https://docs.groupdocs.com/display/searchnet/Searching)

### 示例

该示例演示了该类的典型用法。

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

SearchResult result = index.Search(query); // Searching in index
```

### 另见

* namespace [GroupDocs.Search](../../groupdocs.search)
* assembly [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->
