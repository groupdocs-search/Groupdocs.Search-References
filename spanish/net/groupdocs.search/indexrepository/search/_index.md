---
title: "Buscar"
second_title: "Referencia de la API de GroupDocs.Search para .NET"
description: "Busca en todos los índices del repositorio."
type: docs
weight: 70
url: /es/net/groupdocs.search/indexrepository/search/
---
## Search(string) {#search_2}

Busca en todos los índices del repositorio.

```csharp
public SearchResult Search(string query)
```

| Parameter | Type | Descripción |
| --- | --- | --- |
| consulta | String | La consulta de búsqueda. |

### Valor de retorno

El resultado de búsqueda.

### Ejemplos

El ejemplo muestra cómo realizar una búsqueda en el repositorio de índices.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

IndexRepository repository = new IndexRepository();
Index index = repository.Create(indexFolder); // Creating index
index.Add(documentsFolder); // Indexing documents

SearchResult result = repository.Search(query); // Searching
```

### Ver también

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [IndexRepository](../../indexrepository)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(string, SearchOptions) {#search_3}

Busca en todos los índices del repositorio.

```csharp
public SearchResult Search(string query, SearchOptions options)
```

| Parameter | Type | Descripción |
| --- | --- | --- |
| consulta | String | La consulta de búsqueda. |
| opciones | SearchOptions | Las opciones de búsqueda. |

### Valor de retorno

El resultado de búsqueda.

### Ejemplos

El ejemplo muestra cómo realizar una búsqueda en el repositorio de índices.

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

### Ver también

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [IndexRepository](../../indexrepository)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(SearchQuery) {#search}

Busca en todos los índices del repositorio.

```csharp
public SearchResult Search(SearchQuery query)
```

| Parameter | Type | Descripción |
| --- | --- | --- |
| consulta | SearchQuery | La consulta de búsqueda. |

### Valor de retorno

El resultado de búsqueda.

### Ejemplos

El ejemplo muestra cómo realizar una búsqueda en el repositorio de índices.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

IndexRepository repository = new IndexRepository();
Index index = repository.Create(indexFolder); // Creating index
index.Add(documentsFolder); // Indexing documents

SearchQuery query = SearchQuery.CreateWordQuery("Einstein"); // Creating search query in object form

SearchResult result = repository.Search(query); // Searching
```

### Ver también

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [IndexRepository](../../indexrepository)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(SearchQuery, SearchOptions) {#search_1}

Busca en todos los índices del repositorio.

```csharp
public SearchResult Search(SearchQuery query, SearchOptions options)
```

| Parameter | Type | Descripción |
| --- | --- | --- |
| consulta | SearchQuery | La consulta de búsqueda. |
| opciones | SearchOptions | Las opciones de búsqueda. |

### Valor de retorno

El resultado de búsqueda.

### Ejemplos

El ejemplo muestra cómo realizar una búsqueda en el repositorio de índices.

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

### Ver también

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [IndexRepository](../../indexrepository)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->
