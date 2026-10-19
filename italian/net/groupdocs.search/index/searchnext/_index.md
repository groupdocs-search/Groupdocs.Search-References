---
title: "SearchNext"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Continua la ricerca a blocchi avviata con il metodo Search."
type: docs
weight: 270
url: /it/net/groupdocs.search/index/searchnext/
---
## SearchNext(ChunkSearchToken) {#searchnext}

Continua la ricerca a blocchi avviata con il metodo Search.

```csharp
public SearchResult SearchNext(ChunkSearchToken chunkSearchToken)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| chunkSearchToken | ChunkSearchToken | Il token di ricerca del blocco. |

### Valore di ritorno

Il risultato della ricerca.

### Esempi

L'esempio dimostra come eseguire la ricerca a blocchi.

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

### Vedi anche

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [ChunkSearchToken](../../../groupdocs.search.common/chunksearchtoken)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## SearchNext(ChunkSearchToken, Cancellation) {#searchnext_1}

Continua la ricerca a blocchi avviata con il metodo Search.

```csharp
public SearchResult SearchNext(ChunkSearchToken chunkSearchToken, Cancellation cancellation)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| chunkSearchToken | ChunkSearchToken | Il token di ricerca del blocco. |
| cancellation | Cancellation | L'oggetto di cancellazione. |

### Valore di ritorno

Il risultato della ricerca.

### Esempi

L'esempio dimostra come eseguire la ricerca utilizzando una query in forma di oggetto.

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

### Vedi anche

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [ChunkSearchToken](../../../groupdocs.search.common/chunksearchtoken)
* class [Cancellation](../../../groupdocs.search.common/cancellation)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
