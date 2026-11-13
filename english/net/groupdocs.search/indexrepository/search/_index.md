---
title: Search
second_title: GroupDocs.Search for .NET API Reference
description: Searches in all indexes of the repository.
type: docs
weight: 70
url: /net/groupdocs.search/indexrepository/search/
---

## Search(string) {#search_2}

Searches in all indexes of the repository.

```csharp
public SearchResult Search(string query)
```

| Parameter | Type | Description |
| --- | --- | --- |
| query | String | The search query. |

### Return Value

The search result.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | The query is `null`. |
| ObjectDisposedException | An index of the repository is disposed. |

### Remarks

The errors of the search of an index are reported as [`Search`](../../index/search) reports them: by the [`ErrorOccurred`](../../../groupdocs.search.events/eventhub/erroroccurred) event of the index and of the repository, and in [`Warnings`](../../../groupdocs.search.results/searchresult/warnings) of the result.

### Examples

The example demonstrates how to perform a search in an index repository.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

IndexRepository repository = new IndexRepository();
Index index = repository.Create(indexFolder); // Creating index
index.Add(documentsFolder); // Indexing documents

SearchResult result = repository.Search(query); // Searching
```

### See Also

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [IndexRepository](../../indexrepository)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(string, SearchOptions) {#search_3}

Searches in all indexes of the repository.

```csharp
public SearchResult Search(string query, SearchOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| query | String | The search query. |
| options | SearchOptions | The search options. |

### Return Value

The search result.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | The query is `null`. |
| ObjectDisposedException | An index of the repository is disposed. |

### Remarks

A search by chunks ([`IsChunkSearch`](../../../groupdocs.search.options/searchoptions/ischunksearch)) goes through the chunks of the indexes of the repository, one index after another: the result is a chunk of one index, and [`SearchNext`](../searchnext) continues the search with [`NextChunkSearchToken`](../../../groupdocs.search.results/searchresult/nextchunksearchtoken) of the result. A document that several indexes have is found in a chunk of each of them. The other searches find the documents of all the indexes in one result, and a document that several indexes have is found once.

The errors of the search of an index are reported as [`Search`](../../index/search) reports them: by the [`ErrorOccurred`](../../../groupdocs.search.events/eventhub/erroroccurred) event of the index and of the repository, and in [`Warnings`](../../../groupdocs.search.results/searchresult/warnings) of the result.

### Examples

The example demonstrates how to perform a search in an index repository.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

IndexRepository repository = new IndexRepository();
Index index = repository.Create(indexFolder); // Creating index
index.Add(documentsFolder); // Indexing documents

SearchOptions options = new SearchOptions();
options.UseCaseSensitiveSearch = true; // Setting flag of case sensitive search

SearchResult result = repository.Search(query, options); // Searching
```

### See Also

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [IndexRepository](../../indexrepository)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(SearchQuery) {#search}

Searches in all indexes of the repository.

```csharp
public SearchResult Search(SearchQuery query)
```

| Parameter | Type | Description |
| --- | --- | --- |
| query | SearchQuery | The search query. |

### Return Value

The search result.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | The query is `null`. |
| ArgumentException | The query cannot be the root of a query: it is a wildcard of words, see [`CreateWildcardQuery`](../../searchquery/createwildcardquery). |
| ObjectDisposedException | An index of the repository is disposed. |

### Remarks

The errors of the search of an index are reported as [`Search`](../../index/search) reports them: by the [`ErrorOccurred`](../../../groupdocs.search.events/eventhub/erroroccurred) event of the index and of the repository, and in [`Warnings`](../../../groupdocs.search.results/searchresult/warnings) of the result.

### Examples

The example demonstrates how to perform a search in an index repository.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

IndexRepository repository = new IndexRepository();
Index index = repository.Create(indexFolder); // Creating index
index.Add(documentsFolder); // Indexing documents

SearchQuery query = SearchQuery.CreateWordQuery("Einstein"); // Creating search query in object form

SearchResult result = repository.Search(query); // Searching
```

### See Also

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [IndexRepository](../../indexrepository)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(SearchQuery, SearchOptions) {#search_1}

Searches in all indexes of the repository.

```csharp
public SearchResult Search(SearchQuery query, SearchOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| query | SearchQuery | The search query. |
| options | SearchOptions | The search options. |

### Return Value

The search result.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | The query is `null`. |
| ArgumentException | The query cannot be the root of a query: it is a wildcard of words, see [`CreateWildcardQuery`](../../searchquery/createwildcardquery). |
| ObjectDisposedException | An index of the repository is disposed. |

### Remarks

A search by chunks ([`IsChunkSearch`](../../../groupdocs.search.options/searchoptions/ischunksearch)) goes through the chunks of the indexes of the repository, one index after another: the result is a chunk of one index, and [`SearchNext`](../searchnext) continues the search with [`NextChunkSearchToken`](../../../groupdocs.search.results/searchresult/nextchunksearchtoken) of the result. A document that several indexes have is found in a chunk of each of them. The other searches find the documents of all the indexes in one result, and a document that several indexes have is found once.

The errors of the search of an index are reported as [`Search`](../../index/search) reports them: by the [`ErrorOccurred`](../../../groupdocs.search.events/eventhub/erroroccurred) event of the index and of the repository, and in [`Warnings`](../../../groupdocs.search.results/searchresult/warnings) of the result.

### Examples

The example demonstrates how to perform a search in an index repository.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

IndexRepository repository = new IndexRepository();
Index index = repository.Create(indexFolder); // Creating index
index.Add(documentsFolder); // Indexing documents

SearchOptions options = new SearchOptions();
options.UseCaseSensitiveSearch = true; // Setting flag of case sensitive search

SearchQuery query = SearchQuery.CreateWordQuery("Einstein"); // Creating search query in object form

SearchResult result = repository.Search(query, options); // Searching
```

### See Also

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [IndexRepository](../../indexrepository)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
