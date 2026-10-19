---
title: "Buscar"
second_title: "Referencia de la API de GroupDocs.Search para .NET"
description: "Busca en el índice."
type: docs
weight: 260
url: /es/net/groupdocs.search/index/search/
---
## Search(string) {#search_3}

Busca en el índice.

```csharp
public SearchResult Search(string query)
```

| Parameter | Type | Descripción |
| --- | --- | --- |
| consulta | String | La consulta de búsqueda. |

### Valor de retorno

El resultado de búsqueda.

### Ejemplos

El siguiente ejemplo muestra cómo realizar una búsqueda simple.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

SearchResult result = index.Search(query); // Searching
```

El siguiente ejemplo muestra cómo realizar una búsqueda con expresiones regulares.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

string query = "^[0-9]{3,}"; // The caret symbol at the beginning of the search query tells the index that it is a Regex query
SearchResult result = index.Search(query); // Searching
```

El siguiente ejemplo muestra cómo realizar una búsqueda facetada.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

string query = "content:Newton"; // The word before the colon in the query means the document field name to search
SearchResult result = index.Search(query); // Searching
```

### Ver también

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(string, SearchOptions) {#search_4}

Busca en el índice.

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

El siguiente ejemplo muestra cómo realizar una búsqueda difusa.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

SearchOptions options = new SearchOptions();
options.FuzzySearch.Enabled = true; // Enabling the fuzzy search
options.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1); // Setting the number of possible differences for each word

// Las comillas dobles al principio y al final indican al índice que es una consulta de búsqueda por frase
string query = "\"The Pursuit of Happiness\"";
SearchResult result = index.Search(query, options); // Searching
```

El siguiente ejemplo muestra cómo realizar una búsqueda de sinónimos.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

SearchOptions options = new SearchOptions();
options.UseSynonymSearch = true; // Enabling the synonym search

string query = "cry";
SearchResult result = index.Search(query, options); // Searching
```

### Ver también

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(SearchQuery) {#search_1}

Busca en el índice.

```csharp
public SearchResult Search(SearchQuery query)
```

| Parameter | Type | Descripción |
| --- | --- | --- |
| consulta | SearchQuery | La consulta de búsqueda. |

### Valor de retorno

El resultado de búsqueda.

### Ejemplos

El siguiente ejemplo muestra cómo realizar una búsqueda usando una consulta en forma de objeto.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

// Creando subconsulta 1
SearchQuery subquery1 = SearchQuery.CreateWordQuery("accommodation");
subquery1.SearchOptions = new SearchOptions(); // Setting search options only for subquery 1
subquery1.SearchOptions.FuzzySearch.Enabled = true; // Enabling the fuzzy search
subquery1.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(3); // Setting maximum number of differences

// Creando subconsulta 2
SearchQuery subquery2 = SearchQuery.CreateNumericRangeQuery(1, 1000000);

// Creando subconsulta 3
SearchQuery subquery3 = SearchQuery.CreateRegexQuery(@"(.)\1");

// Combinando subconsultas en una sola consulta
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

SearchResult result = index.Search(query); // Searching
```

### Ver también

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(SearchQuery, SearchOptions) {#search_2}

Busca en el índice.

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

El siguiente ejemplo muestra cómo realizar una búsqueda usando una consulta en forma de objeto.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

// Creando subconsulta de búsqueda de rango de fechas
SearchQuery subquery1 = SearchQuery.CreateDateRangeQuery(new DateTime(2011, 6, 17), new DateTime(2013, 1, 1));

// Creando subconsulta de comodín con número de palabras omitidas de 0 a 2
SearchQuery subquery2 = SearchQuery.CreateWildcardQuery(0, 2);

// Creando subconsulta de palabra simple
SearchQuery subquery3 = SearchQuery.CreateWordQuery("birth");
subquery3.SearchOptions = new SearchOptions(); // Setting search options only for subquery 3
subquery3.SearchOptions.FuzzySearch.Enabled = true;
subquery3.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1);

// Combinando subconsultas en una sola consulta
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

// Creando objeto de opciones de búsqueda con mayor capacidad de ocurrencias encontradas
SearchOptions options = new SearchOptions(); // Overall search options
options.MaxOccurrenceCountPerTerm = 1000000;
options.MaxTotalOccurrenceCount = 10000000;

SearchResult result = index.Search(query, options); // Searching
```

### Ver también

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(SearchImage, ImageSearchOptions) {#search}

Realiza una búsqueda inversa de imágenes en el índice.

```csharp
public ImageSearchResult Search(SearchImage image, ImageSearchOptions options)
```

| Parameter | Type | Descripción |
| --- | --- | --- |
| imagen | SearchImage | La imagen a buscar. |
| opciones | ImageSearchOptions | Las opciones de búsqueda de imágenes. |

### Valor de retorno

El resultado de una búsqueda inversa de imágenes.

### Ver también

* class [ImageSearchResult](../../../groupdocs.search.results/imagesearchresult)
* class [SearchImage](../../../groupdocs.search.common/searchimage)
* class [ImageSearchOptions](../../../groupdocs.search.options/imagesearchoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->
