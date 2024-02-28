---
title: Index
second_title: GroupDocs.Search for .NET API Reference
description: Represents the main class for indexing documents and search through them.
type: docs
weight: 680
url: /net/groupdocs.search/index/
---
## Index class

Represents the main class for indexing documents and search through them.

```csharp
public class Index : IDisposable
```

## Constructors

| Name | Description |
| --- | --- |
| [Index](index#constructor)() | Initializes a new instance of the [`Index`](../index) class in memory. |
| [Index](index#constructor_1)(IndexSettings) | Initializes a new instance of the [`Index`](../index) class in memory with particular index settings. |
| [Index](index#constructor_2)(string) | Initializes a new instance of the [`Index`](../index) class. Creates a new or opens an existing index on disk. |
| [Index](index#constructor_3)(string, bool) | Initializes a new instance of the [`Index`](../index) class. Loads an existing index from disk if *overwriteIfExists* is `false`; creates a new index on disk otherwise. |
| [Index](index#constructor_4)(string, IndexSettings) | Initializes a new instance of the [`Index`](../index) class. Creates a new index with particular settings or opens an existing index on disk. |
| [Index](index#constructor_5)(string, IndexSettings, bool) | Initializes a new instance of the [`Index`](../index) class. Loads an existing index from disk if *overwriteIfExists* is `false`; creates a new index on disk with particular index settings otherwise. |

## Properties

| Name | Description |
| --- | --- |
| [Dictionaries](../../groupdocs.search/index/dictionaries) { get; } | Gets the dictionary repository. |
| [Events](../../groupdocs.search/index/events) { get; } | Gets the event hub for subscribing to events. |
| [IndexInfo](../../groupdocs.search/index/indexinfo) { get; } | Gets the basic information on the index. |
| [IndexSettings](../../groupdocs.search/index/indexsettings) { get; } | Gets the index settings. |
| [Repository](../../groupdocs.search/index/repository) { get; } | Gets the index repository object if the index is contained in it. |

## Methods

| Name | Description |
| --- | --- |
| [Add](../../groupdocs.search/index/add#add_2)(string) | Performs indexing operation. Adds a file or folder by an absolute or relative path. Documents from all subfolders will be indexed. |
| [Add](../../groupdocs.search/index/add#add_4)(string[]) | Performs indexing operation. Adds files or folders by an absolute or relative path. Documents from all subfolders will be indexed. |
| [Add](../../groupdocs.search/index/add#add)(Document[], IndexingOptions) | Performs indexing operation. Adds documents from file system, stream or structure. |
| [Add](../../groupdocs.search/index/add#add_1)(ExtractedData[], IndexingOptions) | Performs indexing operation. Adds the extracted data to the index. |
| [Add](../../groupdocs.search/index/add#add_3)(string, IndexingOptions) | Performs indexing operation. Adds a file or folder by an absolute or relative path. Documents from all subfolders will be indexed. |
| [Add](../../groupdocs.search/index/add#add_5)(string[], IndexingOptions) | Performs indexing operation. Adds files or folders by an absolute or relative path. Documents from all subfolders will be indexed. |
| [ChangeAttributes](../../groupdocs.search/index/changeattributes)(AttributeChangeBatch) | Applies the specified batch of attribute changes to indexed documents without reindexing during the update operation. |
| [CheckSegments](../../groupdocs.search/index/checksegments)(bool) | Checks the index for damaged segment files on the disk. The method fixes index functionality in the presence of damaged segments, if *fixIndexFunctionality* is true; does not fix - otherwise. |
| [Delete](../../groupdocs.search/index/delete#delete_1)(string[], UpdateOptions) | Deletes indexed files or folders from the index. Then updates the index without deleted paths. Note that an individual document cannot be deleted from the index if it was added to the index as part of a folder. |
| [Delete](../../groupdocs.search/index/delete#delete)(UpdateOptions, string[]) | Deletes documents indexed from streams or structures. Then updates the index without deleted documents. |
| [Dispose](../../groupdocs.search/index/dispose)() | Releases all resources used by the [`Index`](../index). |
| [GetAttributes](../../groupdocs.search/index/getattributes)(string) | Gets all the attributes associated with the specified indexed document. |
| [GetDocumentText](../../groupdocs.search/index/getdocumenttext#getdocumenttext)(DocumentInfo, OutputAdapter) | Generates the text of an indexed document and passes it through an output adapter. |
| [GetDocumentText](../../groupdocs.search/index/getdocumenttext#getdocumenttext_1)(DocumentInfo, OutputAdapter, TextOptions) | Generates HTML formatted text for indexed document and transfers it through the output adapter. |
| [GetIndexedDocumentItems](../../groupdocs.search/index/getindexeddocumentitems)(DocumentInfo) | Gets an array of nested items of the specified document (for container documents such as ZIP, OST, PST). |
| [GetIndexedDocuments](../../groupdocs.search/index/getindexeddocuments)() | Gets an array of all indexed documents. |
| [GetIndexedPaths](../../groupdocs.search/index/getindexedpaths)() | Gets an array of indexed paths - documents or folders. |
| [GetIndexingReports](../../groupdocs.search/index/getindexingreports)() | Gets the reports on indexing operations. |
| [GetSearchReports](../../groupdocs.search/index/getsearchreports)() | Gets the reports on search operations. |
| [Highlight](../../groupdocs.search/index/highlight#highlight)(FoundDocument, Highlighter) | Generates HTML formatted text with highlighted found terms. |
| [Highlight](../../groupdocs.search/index/highlight#highlight_1)(FoundDocument, Highlighter, HighlightOptions) | Generates HTML formatted text with highlighted found terms. |
| [Merge](../../groupdocs.search/index/merge#merge)(Index, MergeOptions) | Merges the specified index into the current index. Note that the other index will not be changed. |
| [Merge](../../groupdocs.search/index/merge#merge_1)(IndexRepository, MergeOptions) | Merges indexes from the specified index repository into the current index. Note that indexes in the repository will not be changed. |
| [Notify](../../groupdocs.search/index/notify)(Notification) | Passes the specified notification object to the index to perform the notification. |
| [Optimize](../../groupdocs.search/index/optimize#optimize)() | Minimizes the number of index segments by merging them one with another. This operation improves search performance. |
| [Optimize](../../groupdocs.search/index/optimize#optimize_1)(MergeOptions) | Minimizes the number of index segments by merging them one with another. This operation improves search performance. |
| [Search](../../groupdocs.search/index/search#search_1)(SearchQuery) | Searches in index. |
| [Search](../../groupdocs.search/index/search#search_3)(string) | Searches in index. |
| [Search](../../groupdocs.search/index/search#search)(SearchImage, ImageSearchOptions) | Performs a reverse image search in the index. |
| [Search](../../groupdocs.search/index/search#search_2)(SearchQuery, SearchOptions) | Searches in index. |
| [Search](../../groupdocs.search/index/search#search_4)(string, SearchOptions) | Searches in index. |
| [SearchNext](../../groupdocs.search/index/searchnext#searchnext)(ChunkSearchToken) | Continues the chunk search started with method Search. |
| [SearchNext](../../groupdocs.search/index/searchnext#searchnext_1)(ChunkSearchToken, Cancellation) | Continues the chunk search started with method Search. |
| [Update](../../groupdocs.search/index/update#update)() | Re-indexes documents that have been changed or deleted since last update. Adds new files that have been added to the indexed folders. |
| [Update](../../groupdocs.search/index/update#update_1)(UpdateOptions) | Re-indexes documents that have been changed or deleted since last update. Adds new files that have been added to the indexed folders. |

### Remarks

**Learn more**

* [Creating an index](https://docs.groupdocs.com/display/searchnet/Creating+an+index)
* [Indexing](https://docs.groupdocs.com/display/searchnet/Indexing)
* [Searching](https://docs.groupdocs.com/display/searchnet/Searching)

### Examples

The example demonstrates a typical usage of the class.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

SearchResult result = index.Search(query); // Searching in index
```

### See Also

* namespace [GroupDocs.Search](../../groupdocs.search)
* assembly [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->
