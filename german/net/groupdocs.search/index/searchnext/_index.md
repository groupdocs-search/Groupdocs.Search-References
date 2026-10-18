---
title: "SearchNext"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Setzt die Chunk‑Suche fort, die mit der Methode Search gestartet wurde."
type: docs
weight: 270
url: /de/net/groupdocs.search/index/searchnext/
---
## SearchNext(ChunkSearchToken) {#searchnext}

Setzt die Chunk‑Suche fort, die mit der Methode Search gestartet wurde.

```csharp
public SearchResult SearchNext(ChunkSearchToken chunkSearchToken)
```

| Parameter | Type | Beschreibung |
| --- | --- | --- |
| chunkSearchToken | ChunkSearchToken | Das Chunk-Such-Token. |

### Rückgabewert

Das Suchergebnis.

### Beispiele

Das Beispiel zeigt, wie man eine Chunk-Suche durchführt.

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

### Siehe auch

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [ChunkSearchToken](../../../groupdocs.search.common/chunksearchtoken)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## SearchNext(ChunkSearchToken, Cancellation) {#searchnext_1}

Setzt die Chunk‑Suche fort, die mit der Methode Search gestartet wurde.

```csharp
public SearchResult SearchNext(ChunkSearchToken chunkSearchToken, Cancellation cancellation)
```

| Parameter | Type | Beschreibung |
| --- | --- | --- |
| chunkSearchToken | ChunkSearchToken | Das Chunk-Such-Token. |
| Abbruch | Cancellation | Das Abbruchobjekt. |

### Rückgabewert

Das Suchergebnis.

### Beispiele

Das Beispiel zeigt, wie man eine Suche mit einer Abfrage in Objektform durchführt.

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

### Siehe auch

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [ChunkSearchToken](../../../groupdocs.search.common/chunksearchtoken)
* class [Cancellation](../../../groupdocs.search.common/cancellation)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
