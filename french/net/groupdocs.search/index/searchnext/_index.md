---
title: "SearchNext"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Poursuit la recherche de fragments démarrée avec la méthode Search."
type: docs
weight: 270
url: /fr/net/groupdocs.search/index/searchnext/
---
## SearchNext(ChunkSearchToken) {#searchnext}

Poursuit la recherche de fragments démarrée avec la méthode Search.

```csharp
public SearchResult SearchNext(ChunkSearchToken chunkSearchToken)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| chunkSearchToken | ChunkSearchToken | Le jeton de recherche de fragment. |

### Valeur de retour

Le résultat de recherche.

### Exemples

L'exemple montre comment effectuer une recherche de fragment.

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

### Voir aussi

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [ChunkSearchToken](../../../groupdocs.search.common/chunksearchtoken)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## SearchNext(ChunkSearchToken, Cancellation) {#searchnext_1}

Poursuit la recherche de fragments démarrée avec la méthode Search.

```csharp
public SearchResult SearchNext(ChunkSearchToken chunkSearchToken, Cancellation cancellation)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| chunkSearchToken | ChunkSearchToken | Le jeton de recherche de fragment. |
| cancellation | Annulation | L'objet d'annulation. |

### Valeur de retour

Le résultat de recherche.

### Exemples

L'exemple montre comment effectuer une recherche en utilisant une requête sous forme d'objet.

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

### Voir aussi

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [ChunkSearchToken](../../../groupdocs.search.common/chunksearchtoken)
* class [Cancellation](../../../groupdocs.search.common/cancellation)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
