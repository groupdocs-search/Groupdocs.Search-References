---
title: Searcher
second_title: GroupDocs.Search for Java API Reference
description: Represents a service that manages search queries to shards of the search network.
type: docs
weight: 12
url: /java/com.groupdocs.search.scaling/searcher/
---
**Inheritance:**
java.lang.Object
```
public abstract class Searcher
```

Represents a service that manages search queries to shards of the search network.
## Constructors

| Constructor | Description |
| --- | --- |
| [Searcher()](#Searcher--) |  |
## Methods

| Method | Description |
| --- | --- |
| [searchFirst(SearchQuery query, SearchOptions options)](#searchFirst-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-) | Starts a search in the distributed search index. |
| [searchFirst(SearchImage image, ImageSearchOptions options)](#searchFirst-com.groupdocs.search.common.SearchImage-com.groupdocs.search.options.ImageSearchOptions-) | Performs a reverse image search in the distributed search index. |
| [searchNext(NetworkSearchToken networkSearchToken)](#searchNext-com.groupdocs.search.scaling.results.NetworkSearchToken-) | Continues a search in the distributed search index. |
| [searchNext(NetworkImageSearchToken networkImageSearchToken)](#searchNext-com.groupdocs.search.scaling.results.NetworkImageSearchToken-) | Continues a reverse image search in the distributed search index. |
| [highlight(NetworkFoundDocument document, Highlighter highlighter, HighlightOptions options)](#highlight-com.groupdocs.search.scaling.results.NetworkFoundDocument-com.groupdocs.search.highlighters.Highlighter-com.groupdocs.search.options.HighlightOptions-) | Generates HTML formatted text with highlighted found terms. |
| [getIndexedDocuments(int shardIndex)](#getIndexedDocuments-int-) | Gets an array of all indexed documents. |
| [getIndexedDocumentItems(NetworkDocumentInfo documentInfo)](#getIndexedDocumentItems-com.groupdocs.search.scaling.results.NetworkDocumentInfo-) | Gets an array of nested items of the specified document (for container documents such as ZIP, OST, PST). |
| [getDocumentText(NetworkDocumentInfo documentInfo, OutputAdapter adapter)](#getDocumentText-com.groupdocs.search.scaling.results.NetworkDocumentInfo-com.groupdocs.search.common.OutputAdapter-) | Generates the text of an indexed document and passes it through an output adapter. |
### Searcher() {#Searcher--}
```
public Searcher()
```


### searchFirst(SearchQuery query, SearchOptions options) {#searchFirst-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-}
```
public abstract NetworkSearchResult searchFirst(SearchQuery query, SearchOptions options)
```


Starts a search in the distributed search index.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| query | [SearchQuery](../../com.groupdocs.search/searchquery) | The search query. |
| options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | The search options. |

**Returns:**
[NetworkSearchResult](../../com.groupdocs.search.scaling.results/networksearchresult) - The search result.
### searchFirst(SearchImage image, ImageSearchOptions options) {#searchFirst-com.groupdocs.search.common.SearchImage-com.groupdocs.search.options.ImageSearchOptions-}
```
public abstract NetworkImageSearchResult searchFirst(SearchImage image, ImageSearchOptions options)
```


Performs a reverse image search in the distributed search index.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| image | [SearchImage](../../com.groupdocs.search.common/searchimage) | The image to search. |
| options | [ImageSearchOptions](../../com.groupdocs.search.options/imagesearchoptions) | The image search options. |

**Returns:**
[NetworkImageSearchResult](../../com.groupdocs.search.scaling.results/networkimagesearchresult) - The reverse image search result.
### searchNext(NetworkSearchToken networkSearchToken) {#searchNext-com.groupdocs.search.scaling.results.NetworkSearchToken-}
```
public abstract NetworkSearchResult searchNext(NetworkSearchToken networkSearchToken)
```


Continues a search in the distributed search index.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| networkSearchToken | [NetworkSearchToken](../../com.groupdocs.search.scaling.results/networksearchtoken) | The network search token. |

**Returns:**
[NetworkSearchResult](../../com.groupdocs.search.scaling.results/networksearchresult) - The search result.
### searchNext(NetworkImageSearchToken networkImageSearchToken) {#searchNext-com.groupdocs.search.scaling.results.NetworkImageSearchToken-}
```
public abstract NetworkImageSearchResult searchNext(NetworkImageSearchToken networkImageSearchToken)
```


Continues a reverse image search in the distributed search index.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| networkImageSearchToken | [NetworkImageSearchToken](../../com.groupdocs.search.scaling.results/networkimagesearchtoken) | The network image search token. |

**Returns:**
[NetworkImageSearchResult](../../com.groupdocs.search.scaling.results/networkimagesearchresult) - The reverse image search result.
### highlight(NetworkFoundDocument document, Highlighter highlighter, HighlightOptions options) {#highlight-com.groupdocs.search.scaling.results.NetworkFoundDocument-com.groupdocs.search.highlighters.Highlighter-com.groupdocs.search.options.HighlightOptions-}
```
public abstract void highlight(NetworkFoundDocument document, Highlighter highlighter, HighlightOptions options)
```


Generates HTML formatted text with highlighted found terms.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| document | [NetworkFoundDocument](../../com.groupdocs.search.scaling.results/networkfounddocument) | The found document. |
| highlighter | [Highlighter](../../com.groupdocs.search.highlighters/highlighter) | The search result highlighter. |
| options | [HighlightOptions](../../com.groupdocs.search.options/highlightoptions) | The highlight options. |

### getIndexedDocuments(int shardIndex) {#getIndexedDocuments-int-}
```
public abstract NetworkDocumentInfo[] getIndexedDocuments(int shardIndex)
```


Gets an array of all indexed documents.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| shardIndex | int | The shard index. |

**Returns:**
com.groupdocs.search.scaling.results.NetworkDocumentInfo[] - An array of all indexed documents.
### getIndexedDocumentItems(NetworkDocumentInfo documentInfo) {#getIndexedDocumentItems-com.groupdocs.search.scaling.results.NetworkDocumentInfo-}
```
public abstract NetworkDocumentInfo[] getIndexedDocumentItems(NetworkDocumentInfo documentInfo)
```


Gets an array of nested items of the specified document (for container documents such as ZIP, OST, PST).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| documentInfo | [NetworkDocumentInfo](../../com.groupdocs.search.scaling.results/networkdocumentinfo) | The document info. |

**Returns:**
com.groupdocs.search.scaling.results.NetworkDocumentInfo[] - An array of a document items.
### getDocumentText(NetworkDocumentInfo documentInfo, OutputAdapter adapter) {#getDocumentText-com.groupdocs.search.scaling.results.NetworkDocumentInfo-com.groupdocs.search.common.OutputAdapter-}
```
public abstract void getDocumentText(NetworkDocumentInfo documentInfo, OutputAdapter adapter)
```


Generates the text of an indexed document and passes it through an output adapter.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| documentInfo | [NetworkDocumentInfo](../../com.groupdocs.search.scaling.results/networkdocumentinfo) | The indexed document info. |
| adapter | [OutputAdapter](../../com.groupdocs.search.common/outputadapter) | The output adapter. |

