---
title: Index
second_title: GroupDocs.Search for .NET API 参考
description: 表示索引文档并搜索它们的主类
type: docs
weight: 680
url: /zh/net/groupdocs.search/index/
---
## Index class

表示索引文档并搜索它们的主类。

```csharp
public class Index : IDisposable
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [Index](index#constructor)() | 初始化一个新的实例[`Index`](../index)内存中的类. |
| [Index](index#constructor_1)(IndexSettings) | 初始化一个新的实例[`Index`](../index)内存中具有特定索引设置的类. |
| [Index](index#constructor_2)(string) | 初始化一个新的实例[`Index`](../index) class. 在磁盘上创建新索引或打开现有索引. |
| [Index](index#constructor_3)(string, bool) | 初始化一个新的实例[`Index`](../index) class. 从磁盘加载现有索引，如果*overwriteIfExists*是`错误的`; 否则在磁盘上创建一个新索引。 |
| [Index](index#constructor_4)(string, IndexSettings) | 初始化一个新的实例[`Index`](../index) class. 创建具有特定设置的新索引或打开磁盘上的现有索引. |
| [Index](index#constructor_5)(string, IndexSettings, bool) | 初始化一个新的实例[`Index`](../index) class. 从磁盘加载现有索引，如果*overwriteIfExists*是`错误的` ; 在磁盘上使用特定索引设置创建新索引，否则。 |

## 特性

| 姓名 | 描述 |
| --- | --- |
| [Dictionaries](../../groupdocs.search/index/dictionaries) { get; } | 获取字典存储库。 |
| [Events](../../groupdocs.search/index/events) { get; } | 获取用于订阅事件的事件中心。 |
| [IndexInfo](../../groupdocs.search/index/indexinfo) { get; } | 获取索引的基本信息。 |
| [IndexSettings](../../groupdocs.search/index/indexsettings) { get; } | 获取索引设置。 |
| [Repository](../../groupdocs.search/index/repository) { get; } | 如果索引包含在其中，则获取索引存储库对象。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [Add](../../groupdocs.search/index/add#add_2)(string) | 执行索引操作。 通过绝对或相对路径添加文件或文件夹。 所有子文件夹中的文档都将被索引。 |
| [Add](../../groupdocs.search/index/add#add_4)(string[]) | 执行索引操作。 通过绝对或相对路径添加文件或文件夹。 所有子文件夹中的文档都将被索引。 |
| [Add](../../groupdocs.search/index/add#add)(Document[], IndexingOptions) | 执行索引操作。 从文件系统、流或结构添加文档。 |
| [Add](../../groupdocs.search/index/add#add_1)(ExtractedData[], IndexingOptions) | 执行索引操作。 将提取的数据添加到索引中。 |
| [Add](../../groupdocs.search/index/add#add_3)(string, IndexingOptions) | 执行索引操作。 通过绝对或相对路径添加文件或文件夹。 所有子文件夹中的文档都将被索引。 |
| [Add](../../groupdocs.search/index/add#add_5)(string[], IndexingOptions) | 执行索引操作。 通过绝对或相对路径添加文件或文件夹。 所有子文件夹中的文档都将被索引。 |
| [ChangeAttributes](../../groupdocs.search/index/changeattributes)(AttributeChangeBatch) | 在更新操作期间将指定批次的属性更改应用于索引文档而不重新编制索引。 |
| [Delete](../../groupdocs.search/index/delete#delete_1)(string[], UpdateOptions) | 从索引中删除索引文件或文件夹。然后在不删除路径的情况下更新索引。 请注意，如果单个文档作为文件夹的一部分添加到索引中，则不能从索引中删除它。 |
| [Delete](../../groupdocs.search/index/delete#delete)(UpdateOptions, string[]) | 删除从流或结构中索引的文档。然后在不删除文件的情况下更新索引。 |
| [Dispose](../../groupdocs.search/index/dispose)() | 释放所有使用的资源[`Index`](../index). |
| [GetAttributes](../../groupdocs.search/index/getattributes)(string) | 获取与指定索引文档关联的所有属性。 |
| [GetDocumentText](../../groupdocs.search/index/getdocumenttext#getdocumenttext)(DocumentInfo, OutputAdapter) | 为索引文档生成 HTML 格式的文本并通过输出适配器传输它。 |
| [GetDocumentText](../../groupdocs.search/index/getdocumenttext#getdocumenttext_1)(DocumentInfo, OutputAdapter, TextOptions) | 为索引文档生成 HTML 格式的文本并通过输出适配器传输它。 |
| [GetIndexedDocumentItems](../../groupdocs.search/index/getindexeddocumentitems)(DocumentInfo) | 获取指定文档的嵌套项数组（对于 ZIP、OST、PST 等容器文档）。 |
| [GetIndexedDocuments](../../groupdocs.search/index/getindexeddocuments)() | 获取所有索引文档的数组。 |
| [GetIndexedPaths](../../groupdocs.search/index/getindexedpaths)() | 获取索引路径数组 - 文档或文件夹。 |
| [GetIndexingReports](../../groupdocs.search/index/getindexingreports)() | 获取有关索引操作的报告。 |
| [GetSearchReports](../../groupdocs.search/index/getsearchreports)() | 获取有关搜索操作的报告。 |
| [Highlight](../../groupdocs.search/index/highlight#highlight)(FoundDocument, Highlighter) | 生成带有突出显示的找到的术语的 HTML 格式文本。 |
| [Highlight](../../groupdocs.search/index/highlight#highlight_1)(FoundDocument, Highlighter, HighlightOptions) | 生成带有突出显示的找到的术语的 HTML 格式文本。 |
| [Merge](../../groupdocs.search/index/merge#merge)(Index, MergeOptions) | 将指定的索引合并到当前索引中。 注意不会改变其他索引。 |
| [Merge](../../groupdocs.search/index/merge#merge_1)(IndexRepository, MergeOptions) | 将指定索引存储库中的索引合并到当前索引中。 注意存储库中的索引不会被更改。 |
| [Notify](../../groupdocs.search/index/notify)(Notification) | 将指定的通知对象传递给索引执行通知。 |
| [Optimize](../../groupdocs.search/index/optimize#optimize)() | 通过将索引段与另一个合并来最小化索引段的数量。 此操作提高了搜索性能。 |
| [Optimize](../../groupdocs.search/index/optimize#optimize_1)(MergeOptions) | 通过将索引段与另一个合并来最小化索引段的数量。 此操作提高了搜索性能。 |
| [Search](../../groupdocs.search/index/search#search_1)(SearchQuery) | 在索引中搜索。 |
| [Search](../../groupdocs.search/index/search#search_3)(string) | 在索引中搜索。 |
| [Search](../../groupdocs.search/index/search#search)(SearchImage, ImageSearchOptions) | 在索引中执行反向图像搜索。 |
| [Search](../../groupdocs.search/index/search#search_2)(SearchQuery, SearchOptions) | 在索引中搜索。 |
| [Search](../../groupdocs.search/index/search#search_4)(string, SearchOptions) | 在索引中搜索。 |
| [SearchNext](../../groupdocs.search/index/searchnext#searchnext)(ChunkSearchToken) | 继续使用 Search 方法开始的块搜索。 |
| [SearchNext](../../groupdocs.search/index/searchnext#searchnext_1)(ChunkSearchToken, Cancellation) | 继续使用 Search 方法开始的块搜索。 |
| [Update](../../groupdocs.search/index/update#update)() | 重新索引自上次更新以来已更改或删除的文档。 添加已添加到索引文件夹的新文件。 |
| [Update](../../groupdocs.search/index/update#update_1)(UpdateOptions) | 重新索引自上次更新以来已更改或删除的文档。 添加已添加到索引文件夹的新文件。 |

### 评论

**了解更多**

* [创建索引](https://docs.groupdocs.com/display/searchnet/Creating+an+index)
* [索引](https://docs.groupdocs.com/display/searchnet/Indexing)
* [搜索中](https://docs.groupdocs.com/display/searchnet/Searching)

### 例子

该示例演示了该类的典型用法。

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // 在指定文件夹中创建索引
index.Add(documentsFolder); // 索引指定文件夹中的文档

SearchResult result = index.Search(query); // 在索引中搜索
```

### 也可以看看

* 命名空间 [GroupDocs.Search](../../groupdocs.search)
* 部件 [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
