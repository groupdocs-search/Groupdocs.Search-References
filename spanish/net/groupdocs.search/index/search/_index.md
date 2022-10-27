---
title: Search
second_title: GroupDocs.Buscar referencia de API de .NET
description: Búsquedas en index.
type: docs
weight: 220
url: /es/net/groupdocs.search/index/search/
---
## Search(string) {#search_3}

Búsquedas en index.

```csharp
public SearchResult Search(string query)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| query | String | La consulta de búsqueda. |

### Valor_devuelto

El resultado de la búsqueda.

### Ejemplos

El siguiente ejemplo muestra cómo realizar una búsqueda simple.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // Creando índice en la carpeta especificada
index.Add(documentsFolder); // Indexación de documentos de la carpeta especificada

SearchResult result = index.Search(query); // Buscando
```

El siguiente ejemplo muestra cómo realizar la búsqueda Regex.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creando índice en la carpeta especificada
index.Add(documentsFolder); // Indexación de documentos de la carpeta especificada

string query = "^[0-9]{3,}"; // El símbolo de intercalación al comienzo de la consulta de búsqueda le dice al índice que es una consulta Regex
SearchResult result = index.Search(query); // Buscando
```

El siguiente ejemplo muestra cómo realizar una búsqueda por facetas.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creando índice en la carpeta especificada
index.Add(documentsFolder); // Indexación de documentos de la carpeta especificada

string query = "content:Newton"; // La palabra antes de los dos puntos en la consulta significa el nombre del campo del documento para buscar
SearchResult result = index.Search(query); // Buscando
```

### Ver también

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [Index](../../index)
* espacio de nombres [GroupDocs.Search](../../index)
* asamblea [GroupDocs.Search](../../../)

---

## Search(string, SearchOptions) {#search_4}

Búsquedas en index.

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

El siguiente ejemplo muestra cómo realizar una búsqueda aproximada.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creando índice en la carpeta especificada
index.Add(documentsFolder); // Indexación de documentos de la carpeta especificada

SearchOptions options = new SearchOptions();
options.FuzzySearch.Enabled = true; // Habilitando la búsqueda difusa
options.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1); // Establecer el número de diferencias posibles para cada palabra

// Las comillas dobles al principio y al final le dicen al índice que es una consulta de búsqueda de frases
string query = "\"The Pursuit of Happiness\"";
SearchResult result = index.Search(query, options); // Buscando
```

El siguiente ejemplo muestra cómo realizar una búsqueda de sinónimos.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creando índice en la carpeta especificada
index.Add(documentsFolder); // Indexación de documentos de la carpeta especificada

SearchOptions options = new SearchOptions();
options.UseSynonymSearch = true; // Habilitando la búsqueda de sinónimos

string query = "cry";
SearchResult result = index.Search(query, options); // Buscando
```

### Ver también

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Index](../../index)
* espacio de nombres [GroupDocs.Search](../../index)
* asamblea [GroupDocs.Search](../../../)

---

## Search(SearchQuery) {#search_1}

Búsquedas en index.

```csharp
public SearchResult Search(SearchQuery query)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| query | SearchQuery | La consulta de búsqueda. |

### Valor_devuelto

El resultado de la búsqueda.

### Ejemplos

El siguiente ejemplo muestra cómo realizar una búsqueda utilizando una consulta en forma de objeto.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creando índice en la carpeta especificada
index.Add(documentsFolder); // Indexación de documentos de la carpeta especificada

// Creando la subconsulta 1
SearchQuery subquery1 = SearchQuery.CreateWordQuery("accommodation");
subquery1.SearchOptions = new SearchOptions(); // Configuración de opciones de búsqueda solo para la subconsulta 1
subquery1.SearchOptions.FuzzySearch.Enabled = true; // Habilitando la búsqueda difusa
subquery1.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(3); // Establecer el número máximo de diferencias

// Creando la subconsulta 2
SearchQuery subquery2 = SearchQuery.CreateNumericRangeQuery(1, 1000000);

// Creando la subconsulta 3
SearchQuery subquery3 = SearchQuery.CreateRegexQuery(@"(.)\1");

// Combinando subconsultas en una sola consulta
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

SearchResult result = index.Search(query); // Buscando
```

### Ver también

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [Index](../../index)
* espacio de nombres [GroupDocs.Search](../../index)
* asamblea [GroupDocs.Search](../../../)

---

## Search(SearchQuery, SearchOptions) {#search_2}

Búsquedas en index.

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

El siguiente ejemplo muestra cómo realizar una búsqueda utilizando una consulta en forma de objeto.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creando índice en la carpeta especificada
index.Add(documentsFolder); // Indexación de documentos de la carpeta especificada

// Creando una subconsulta de búsqueda de rango de fechas
SearchQuery subquery1 = SearchQuery.CreateDateRangeQuery(new DateTime(2011, 6, 17), new DateTime(2013, 1, 1));

// Creando subconsulta de comodín con número de palabras perdidas de 0 a 2
SearchQuery subquery2 = SearchQuery.CreateWildcardQuery(0, 2);

// Creando una subconsulta de una palabra simple
SearchQuery subquery3 = SearchQuery.CreateWordQuery("birth");
subquery3.SearchOptions = new SearchOptions(); // Configuración de opciones de búsqueda solo para la subconsulta 3
subquery3.SearchOptions.FuzzySearch.Enabled = true;
subquery3.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1);

// Combinando subconsultas en una sola consulta
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

// Creación de objeto de opciones de búsqueda con mayor capacidad de ocurrencias encontradas
SearchOptions options = new SearchOptions(); // Opciones generales de búsqueda
options.MaxOccurrenceCountPerTerm = 1000000;
options.MaxTotalOccurrenceCount = 10000000;

SearchResult result = index.Search(query, options); // Buscando
```

### Ver también

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Index](../../index)
* espacio de nombres [GroupDocs.Search](../../index)
* asamblea [GroupDocs.Search](../../../)

---

## Search(SearchImage, ImageSearchOptions) {#search}

Realiza una búsqueda inversa de imágenes en el índice.

```csharp
public ImageSearchResult Search(SearchImage image, ImageSearchOptions options)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| image | SearchImage | La imagen a buscar. |
| options | ImageSearchOptions | Las opciones de búsqueda de imágenes. |

### Valor_devuelto

El resultado de una búsqueda inversa de imágenes.

### Ver también

* class [ImageSearchResult](../../../groupdocs.search.results/imagesearchresult)
* class [SearchImage](../../../groupdocs.search.common/searchimage)
* class [ImageSearchOptions](../../../groupdocs.search.options/imagesearchoptions)
* class [Index](../../index)
* espacio de nombres [GroupDocs.Search](../../index)
* asamblea [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
