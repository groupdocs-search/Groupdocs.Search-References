---
title: "Cerca"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Cerca in tutti gli indici del repository."
type: docs
weight: 70
url: /it/net/groupdocs.search/indexrepository/search/
---
## Search(string) {#search_2}

Cerca in tutti gli indici del repository.

```csharp
public SearchResult Search(string query)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| query | String | La query di ricerca. |

### Valore di ritorno

Il risultato della ricerca.

### Esempi

L'esempio dimostra come eseguire la ricerca nel index repository.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

IndexRepository repository = new IndexRepository();
Index index = repository.Create(indexFolder); // Creating index
index.Add(documentsFolder); // Indexing documents

SearchResult result = repository.Search(query); // Searching
```

### Vedi anche

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [IndexRepository](../../indexrepository)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(string, SearchOptions) {#search_3}

Cerca in tutti gli indici del repository.

```csharp
public SearchResult Search(string query, SearchOptions options)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| query | String | La query di ricerca. |
| opzioni | SearchOptions | Le opzioni di ricerca. |

### Valore di ritorno

Il risultato della ricerca.

### Esempi

L'esempio dimostra come eseguire la ricerca nel index repository.

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

### Vedi anche

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [IndexRepository](../../indexrepository)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(SearchQuery) {#search}

Cerca in tutti gli indici del repository.

```csharp
public SearchResult Search(SearchQuery query)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| query | SearchQuery | La query di ricerca. |

### Valore di ritorno

Il risultato della ricerca.

### Esempi

L'esempio dimostra come eseguire la ricerca nel index repository.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

IndexRepository repository = new IndexRepository();
Index index = repository.Create(indexFolder); // Creating index
index.Add(documentsFolder); // Indexing documents

SearchQuery query = SearchQuery.CreateWordQuery("Einstein"); // Creating search query in object form

SearchResult result = repository.Search(query); // Searching
```

### Vedi anche

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [IndexRepository](../../indexrepository)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(SearchQuery, SearchOptions) {#search_1}

Cerca in tutti gli indici del repository.

```csharp
public SearchResult Search(SearchQuery query, SearchOptions options)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| query | SearchQuery | La query di ricerca. |
| opzioni | SearchOptions | Le opzioni di ricerca. |

### Valore di ritorno

Il risultato della ricerca.

### Esempi

L'esempio dimostra come eseguire la ricerca nel index repository.

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

### Vedi anche

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [IndexRepository](../../indexrepository)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
