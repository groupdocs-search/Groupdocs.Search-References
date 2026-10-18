---
title: "Suche"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Durchsucht alle Indizes des Repositories."
type: docs
weight: 70
url: /de/net/groupdocs.search/indexrepository/search/
---
## Search(string) {#search_2}

Durchsucht alle Indizes des Repositories.

```csharp
public SearchResult Search(string query)
```

| Parameter | Type | Beschreibung |
| --- | --- | --- |
| Abfrage | String | Die Suchabfrage. |

### Rückgabewert

Das Suchergebnis.

### Beispiele

Das Beispiel demonstriert, wie man die Suche im Index-Repository durchführt.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

IndexRepository repository = new IndexRepository();
Index index = repository.Create(indexFolder); // Creating index
index.Add(documentsFolder); // Indexing documents

SearchResult result = repository.Search(query); // Searching
```

### Siehe auch

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [IndexRepository](../../indexrepository)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(string, SearchOptions) {#search_3}

Durchsucht alle Indizes des Repositories.

```csharp
public SearchResult Search(string query, SearchOptions options)
```

| Parameter | Type | Beschreibung |
| --- | --- | --- |
| Abfrage | String | Die Suchabfrage. |
| Optionen | Suchoptionen | Die Suchoptionen. |

### Rückgabewert

Das Suchergebnis.

### Beispiele

Das Beispiel demonstriert, wie man die Suche im Index-Repository durchführt.

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

### Siehe auch

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [IndexRepository](../../indexrepository)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(SearchQuery) {#search}

Durchsucht alle Indizes des Repositories.

```csharp
public SearchResult Search(SearchQuery query)
```

| Parameter | Type | Beschreibung |
| --- | --- | --- |
| Abfrage | SearchQuery | Die Suchabfrage. |

### Rückgabewert

Das Suchergebnis.

### Beispiele

Das Beispiel demonstriert, wie man die Suche im Index-Repository durchführt.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

IndexRepository repository = new IndexRepository();
Index index = repository.Create(indexFolder); // Creating index
index.Add(documentsFolder); // Indexing documents

SearchQuery query = SearchQuery.CreateWordQuery("Einstein"); // Creating search query in object form

SearchResult result = repository.Search(query); // Searching
```

### Siehe auch

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [IndexRepository](../../indexrepository)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(SearchQuery, SearchOptions) {#search_1}

Durchsucht alle Indizes des Repositories.

```csharp
public SearchResult Search(SearchQuery query, SearchOptions options)
```

| Parameter | Type | Beschreibung |
| --- | --- | --- |
| Abfrage | SearchQuery | Die Suchabfrage. |
| Optionen | Suchoptionen | Die Suchoptionen. |

### Rückgabewert

Das Suchergebnis.

### Beispiele

Das Beispiel demonstriert, wie man die Suche im Index-Repository durchführt.

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

### Siehe auch

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [IndexRepository](../../indexrepository)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
