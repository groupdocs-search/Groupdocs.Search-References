---
title: "Recherche"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Recherche dans tous les index du référentiel."
type: docs
weight: 70
url: /fr/net/groupdocs.search/indexrepository/search/
---
## Search(string) {#search_2}

Recherche dans tous les index du référentiel.

```csharp
public SearchResult Search(string query)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| requête | String | La requête de recherche. |

### Valeur de retour

Le résultat de recherche.

### Exemples

L'exemple montre comment effectuer une recherche dans le référentiel d'index.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

IndexRepository repository = new IndexRepository();
Index index = repository.Create(indexFolder); // Creating index
index.Add(documentsFolder); // Indexing documents

SearchResult result = repository.Search(query); // Searching
```

### Voir aussi

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [IndexRepository](../../indexrepository)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(string, SearchOptions) {#search_3}

Recherche dans tous les index du référentiel.

```csharp
public SearchResult Search(string query, SearchOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| requête | String | La requête de recherche. |
| options | SearchOptions | Les options de recherche. |

### Valeur de retour

Le résultat de recherche.

### Exemples

L'exemple montre comment effectuer une recherche dans le référentiel d'index.

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

### Voir aussi

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [IndexRepository](../../indexrepository)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(SearchQuery) {#search}

Recherche dans tous les index du référentiel.

```csharp
public SearchResult Search(SearchQuery query)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| requête | SearchQuery | La requête de recherche. |

### Valeur de retour

Le résultat de recherche.

### Exemples

L'exemple montre comment effectuer une recherche dans le référentiel d'index.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

IndexRepository repository = new IndexRepository();
Index index = repository.Create(indexFolder); // Creating index
index.Add(documentsFolder); // Indexing documents

SearchQuery query = SearchQuery.CreateWordQuery("Einstein"); // Creating search query in object form

SearchResult result = repository.Search(query); // Searching
```

### Voir aussi

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [IndexRepository](../../indexrepository)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(SearchQuery, SearchOptions) {#search_1}

Recherche dans tous les index du référentiel.

```csharp
public SearchResult Search(SearchQuery query, SearchOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| requête | SearchQuery | La requête de recherche. |
| options | SearchOptions | Les options de recherche. |

### Valeur de retour

Le résultat de recherche.

### Exemples

L'exemple montre comment effectuer une recherche dans le référentiel d'index.

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

### Voir aussi

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [IndexRepository](../../indexrepository)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
