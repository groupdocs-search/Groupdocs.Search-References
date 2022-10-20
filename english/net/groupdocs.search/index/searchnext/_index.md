---
title: SearchNext
second_title: GroupDocs.Search for .NET API Reference
description: Continues the chunk search started with method Search.
type: docs
weight: 230
url: /net/groupdocs.search/index/searchnext/
---
## SearchNext(ChunkSearchToken) {#searchnext}

Continues the chunk search started with method Search.

```csharp
public SearchResult SearchNext(ChunkSearchToken chunkSearchToken)
```

| Parameter | Type | Description |
| --- | --- | --- |
| chunkSearchToken | ChunkSearchToken | The chunk search token. |

### Return Value

The search result.

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
* namespace [GroupDocs.Search](../../index)
* assembly [GroupDocs.Search](../../../)

---

## SearchNext(ChunkSearchToken, Cancellation) {#searchnext_1}

Continues the chunk search started with method Search.

```csharp
public SearchResult SearchNext(ChunkSearchToken chunkSearchToken, Cancellation cancellation)
```

| Parameter | Type | Description |
| --- | --- | --- |
| chunkSearchToken | ChunkSearchToken | The chunk search token. |
| cancellation | Cancellation | The cancellation object. |

### Return Value

The search result.

### Examples

The example demonstrates how to perform search using query in object form.

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
* namespace [GroupDocs.Search](../../index)
* assembly [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->