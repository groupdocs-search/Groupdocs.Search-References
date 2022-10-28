---
title: Search
second_title: GroupDocs.Buscar referencia de API de .NET
description: Busca en todos los índices del repositorio.
type: docs
weight: 70
url: /es/net/groupdocs.search/indexrepository/search/
---
## Search(string) {#search_2}

Busca en todos los índices del repositorio.

```csharp
public SearchResult Search(string query)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| query | String | La consulta de búsqueda. |

### Valor_devuelto

El resultado de la búsqueda.

### Ejemplos

El ejemplo demuestra cómo realizar una búsqueda en el repositorio de índices.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

IndexRepository repository = new IndexRepository();
Index index = repository.Create(indexFolder); // Creando índice
index.Add(documentsFolder); // Indexación de documentos

SearchResult result = repository.Search(query); // Buscando
```

### Ver también

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [IndexRepository](../../indexrepository)
* espacio de nombres [GroupDocs.Search](../../indexrepository)
* asamblea [GroupDocs.Search](../../../)

---

## Search(string, SearchOptions) {#search_3}

Busca en todos los índices del repositorio.

```csharp
public SearchResult Search(string query, SearchOptions options)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| query | String | La consulta de búsqueda. |
| options | SearchOptions | Las opciones de búsqueda. |

### Valor_devuelto

El resultado de la búsqueda.

### Ejemplos

El ejemplo demuestra cómo realizar una búsqueda en el repositorio de índices.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

IndexRepository repository = new IndexRepository();
Index index = repository.Create(indexFolder); // Creando índice
index.Add(documentsFolder); // Indexación de documentos

SearchOptions options = new SearchOptions();
options.UseCaseSensitiveSearch = true; // Establecer el indicador de búsqueda sensible a mayúsculas y minúsculas

SearchResult result = repository.Search(query, options); // Buscando
```

### Ver también

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [IndexRepository](../../indexrepository)
* espacio de nombres [GroupDocs.Search](../../indexrepository)
* asamblea [GroupDocs.Search](../../../)

---

## Search(SearchQuery) {#search}

Busca en todos los índices del repositorio.

```csharp
public SearchResult Search(SearchQuery query)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| query | SearchQuery | La consulta de búsqueda. |

### Valor_devuelto

El resultado de la búsqueda.

### Ejemplos

El ejemplo demuestra cómo realizar una búsqueda en el repositorio de índices.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

IndexRepository repository = new IndexRepository();
Index index = repository.Create(indexFolder); // Creando índice
index.Add(documentsFolder); // Indexación de documentos

SearchQuery query = SearchQuery.CreateWordQuery("Einstein"); // Crear consulta de búsqueda en forma de objeto

SearchResult result = repository.Search(query); // Buscando
```

### Ver también

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [IndexRepository](../../indexrepository)
* espacio de nombres [GroupDocs.Search](../../indexrepository)
* asamblea [GroupDocs.Search](../../../)

---

## Search(SearchQuery, SearchOptions) {#search_1}

Busca en todos los índices del repositorio.

```csharp
public SearchResult Search(SearchQuery query, SearchOptions options)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| query | SearchQuery | La consulta de búsqueda. |
| options | SearchOptions | Las opciones de búsqueda. |

### Valor_devuelto

El resultado de la búsqueda.

### Ejemplos

El ejemplo demuestra cómo realizar una búsqueda en el repositorio de índices.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

IndexRepository repository = new IndexRepository();
Index index = repository.Create(indexFolder); // Creando índice
index.Add(documentsFolder); // Indexación de documentos

SearchOptions options = new SearchOptions();
options.UseCaseSensitiveSearch = true; // Establecer el indicador de búsqueda sensible a mayúsculas y minúsculas

SearchQuery query = SearchQuery.CreateWordQuery("Einstein"); // Crear consulta de búsqueda en forma de objeto

SearchResult result = repository.Search(query, options); // Buscando
```

### Ver también

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [IndexRepository](../../indexrepository)
* espacio de nombres [GroupDocs.Search](../../indexrepository)
* asamblea [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
