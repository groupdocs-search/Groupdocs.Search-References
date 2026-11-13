---
title: SearchNext
second_title: GroupDocs.Search for .NET API Reference
description: Continues the search by chunks of the repository started with the Search method.
type: docs
weight: 80
url: /net/groupdocs.search/indexrepository/searchnext/
---

## SearchNext(ChunkSearchToken) {#searchnext}

Continues the search by chunks of the repository started with the Search method.

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
| ArgumentException | The chunk search token is not a token of a search by chunks of the repository. |
| ObjectDisposedException | The index of the next chunk is disposed. |

### Remarks

The chunks of the indexes of the repository follow one another: the next chunk of the same index, or the first chunk of the next index. The search goes through the indexes that the repository had when the search started, and [`NextChunkSearchToken`](../../../groupdocs.search.results/searchresult/nextchunksearchtoken) is `null` after the last chunk of the last index.

The errors of the search of a chunk are reported as [`SearchNext`](../../index/searchnext) reports them: by the [`ErrorOccurred`](../../../groupdocs.search.events/eventhub/erroroccurred) event of the index and of the repository, and in [`Warnings`](../../../groupdocs.search.results/searchresult/warnings) of the result.

### Examples

The example demonstrates how to perform a search by chunks in an index repository.

```csharp
string indexFolder1 = @"c:\MyIndex1\";
string indexFolder2 = @"c:\MyIndex2\";
string documentsFolder1 = @"c:\MyDocuments1\";
string documentsFolder2 = @"c:\MyDocuments2\";
string query = "Einstein";

IndexRepository repository = new IndexRepository();
Index index1 = repository.Create(indexFolder1); // Creating the first index
index1.Add(documentsFolder1); // Indexing documents
Index index2 = repository.Create(indexFolder2); // Creating the second index
index2.Add(documentsFolder2);

SearchOptions options = new SearchOptions();
options.IsChunkSearch = true; // Enabling the search by chunks

SearchResult result = repository.Search(query, options); // Starting the search by chunks
Console.WriteLine("Document count: " + result.DocumentCount);

while (result.NextChunkSearchToken != null)
{
    result = repository.SearchNext(result.NextChunkSearchToken); // Continuing the search by chunks
    Console.WriteLine("Document count: " + result.DocumentCount);
}
```

### See Also

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [ChunkSearchToken](../../../groupdocs.search.common/chunksearchtoken)
* class [IndexRepository](../../indexrepository)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## SearchNext(ChunkSearchToken, Cancellation) {#searchnext_1}

Continues the search by chunks of the repository started with the Search method.

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
| ArgumentException | The chunk search token is not a token of a search by chunks of the repository. |
| ObjectDisposedException | The index of the next chunk is disposed. |

### Remarks

The chunks of the indexes of the repository follow one another: the next chunk of the same index, or the first chunk of the next index. The search goes through the indexes that the repository had when the search started, and [`NextChunkSearchToken`](../../../groupdocs.search.results/searchresult/nextchunksearchtoken) is `null` after the last chunk of the last index.

The errors of the search of a chunk are reported as [`SearchNext`](../../index/searchnext) reports them: by the [`ErrorOccurred`](../../../groupdocs.search.events/eventhub/erroroccurred) event of the index and of the repository, and in [`Warnings`](../../../groupdocs.search.results/searchresult/warnings) of the result.

### Examples

The example demonstrates how to perform a search by chunks in an index repository.

```csharp
string indexFolder1 = @"c:\MyIndex1\";
string indexFolder2 = @"c:\MyIndex2\";
string documentsFolder1 = @"c:\MyDocuments1\";
string documentsFolder2 = @"c:\MyDocuments2\";
string query = "Einstein";

IndexRepository repository = new IndexRepository();
Index index1 = repository.Create(indexFolder1); // Creating the first index
index1.Add(documentsFolder1); // Indexing documents
Index index2 = repository.Create(indexFolder2); // Creating the second index
index2.Add(documentsFolder2);

Cancellation cancellation = new Cancellation(); // The cancellation of the search and of its continuations
SearchOptions options = new SearchOptions();
options.IsChunkSearch = true; // Enabling the search by chunks
options.Cancellation = cancellation;

SearchResult result = repository.Search(query, options); // Starting the search by chunks
Console.WriteLine("Document count: " + result.DocumentCount);

while (result.NextChunkSearchToken != null)
{
    // Continuing the search by chunks
    result = repository.SearchNext(result.NextChunkSearchToken, cancellation);
    Console.WriteLine("Document count: " + result.DocumentCount);
}
```

### See Also

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [ChunkSearchToken](../../../groupdocs.search.common/chunksearchtoken)
* class [Cancellation](../../../groupdocs.search.common/cancellation)
* class [IndexRepository](../../indexrepository)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
