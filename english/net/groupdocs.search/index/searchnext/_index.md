---
title: SearchNext
second_title: GroupDocs.Search for .NET API Reference
description: Continues the chunk search started with the Search method.
type: docs
weight: 270
url: /net/groupdocs.search/index/searchnext/
---

## SearchNext(ChunkSearchToken) {#searchnext}

Continues the chunk search started with the Search method.

```csharp
public SearchResult SearchNext(ChunkSearchToken chunkSearchToken)
```

| Parameter | Type | Description |
| --- | --- | --- |
| chunkSearchToken | ChunkSearchToken | The chunk search token. |

### Return Value

The search result.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | The chunk search token is `null`. |
| ObjectDisposedException | The index is disposed. |

### Remarks

The errors of the search of a chunk are reported as [`Search`](../search) reports them: by the [`ErrorOccurred`](../../../groupdocs.search.events/eventhub/erroroccurred) event of the index, and in [`Warnings`](../../../groupdocs.search.results/searchresult/warnings) of the result. The method throws an exception only for an argument that is not valid and for a disposed index. An error that stops the search gives an empty result without the token of the next chunk, so the search by chunks ends; a part of the index that cannot be read is passed over, and [`Truncated`](../../../groupdocs.search.results/searchresult/truncated) of the result is `true`.

### Examples

The example demonstrates how to perform chunk search.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

SearchOptions options = new SearchOptions();
options.IsChunkSearch = true; // Enabling chunk search

SearchResult result = index.Search(query, options); // Starting chunk search
Console.WriteLine("Document count: " + result.DocumentCount);
Console.WriteLine("Occurrence count: " + result.OccurrenceCount);

while (result.NextChunkSearchToken != null)
{
    result = index.SearchNext(result.NextChunkSearchToken); // Continuing chunk search
    Console.WriteLine("Document count: " + result.DocumentCount);
    Console.WriteLine("Occurrence count: " + result.OccurrenceCount);
}
```

### See Also

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [ChunkSearchToken](../../../groupdocs.search.common/chunksearchtoken)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## SearchNext(ChunkSearchToken, Cancellation) {#searchnext_1}

Continues the chunk search started with the Search method.

```csharp
public SearchResult SearchNext(ChunkSearchToken chunkSearchToken, Cancellation cancellation)
```

| Parameter | Type | Description |
| --- | --- | --- |
| chunkSearchToken | ChunkSearchToken | The chunk search token. |
| cancellation | Cancellation | The cancellation object. |

### Return Value

The search result.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | The chunk search token is `null`. |
| ObjectDisposedException | The index is disposed. |

### Remarks

The errors of the search of a chunk are reported as [`Search`](../search) reports them: by the [`ErrorOccurred`](../../../groupdocs.search.events/eventhub/erroroccurred) event of the index, and in [`Warnings`](../../../groupdocs.search.results/searchresult/warnings) of the result. The method throws an exception only for an argument that is not valid and for a disposed index. An error that stops the search gives an empty result without the token of the next chunk, so the search by chunks ends; a part of the index that cannot be read is passed over, and [`Truncated`](../../../groupdocs.search.results/searchresult/truncated) of the result is `true`.

### Examples

The example demonstrates how to perform chunk search with a cancellation object.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

Cancellation cancellation = new Cancellation(); // This cancellation object aborts all search continuations if canceled
SearchOptions options = new SearchOptions();
options.IsChunkSearch = true; // Enabling chunk search
options.Cancellation = cancellation;

SearchResult result = index.Search(query, options); // Starting chunk search
Console.WriteLine("Document count: " + result.DocumentCount);
Console.WriteLine("Occurrence count: " + result.OccurrenceCount);

while (result.NextChunkSearchToken != null)
{
    result = index.SearchNext(result.NextChunkSearchToken, cancellation); // Continuing chunk search
    Console.WriteLine("Document count: " + result.DocumentCount);
    Console.WriteLine("Occurrence count: " + result.OccurrenceCount);
}
```

### See Also

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [ChunkSearchToken](../../../groupdocs.search.common/chunksearchtoken)
* class [Cancellation](../../../groupdocs.search.common/cancellation)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
