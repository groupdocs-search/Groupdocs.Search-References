---
title: SearchQuery
second_title: GroupDocs.Buscar referencia de API de .NET
description: Representa una consulta de búsqueda en forma de objeto.
type: docs
weight: 1200
url: /es/net/groupdocs.search/searchquery/
---
## SearchQuery class

Representa una consulta de búsqueda en forma de objeto.

```csharp
public abstract class SearchQuery
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| virtual [ChildCount](../../groupdocs.search/searchquery/childcount) { get; } | Obtiene el número de consultas secundarias. |
| virtual [FieldName](../../groupdocs.search/searchquery/fieldname) { get; } | Obtiene el nombre del campo. |
| virtual [FirstChild](../../groupdocs.search/searchquery/firstchild) { get; } | Obtiene la primera consulta secundaria. |
| [SearchOptions](../../groupdocs.search/searchquery/searchoptions) { get; set; } | Obtiene o establece las opciones de búsqueda de esta consulta de búsqueda. |
| virtual [SecondChild](../../groupdocs.search/searchquery/secondchild) { get; } | Obtiene la segunda consulta secundaria. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| static [CreateAndQuery](../../groupdocs.search/searchquery/createandquery)(SearchQuery, SearchQuery) | Crea una consulta combinada que encontrará solo los documentos que se encontrarán para cada consulta original. |
| static [CreateDateRangeQuery](../../groupdocs.search/searchquery/createdaterangequery)(DateTime, DateTime) | Crea una consulta de intervalo de fechas. |
| static [CreateFieldQuery](../../groupdocs.search/searchquery/createfieldquery)(string, SearchQuery) | Agrega un campo a la consulta especificada. |
| static [CreateNotQuery](../../groupdocs.search/searchquery/createnotquery)(SearchQuery) | Crea una consulta invertida que encontrará el resto de documentos en un índice contra los que se encontrarán para la consulta original. |
| static [CreateNumericRangeQuery](../../groupdocs.search/searchquery/createnumericrangequery)(long, long) | Crea una consulta de rango numérico. |
| static [CreateOrQuery](../../groupdocs.search/searchquery/createorquery)(SearchQuery, SearchQuery) | Crea una consulta combinada que encontrará todos los documentos que se encontrarán al menos para una de las consultas originales. |
| static [CreatePhraseSearchQuery](../../groupdocs.search/searchquery/createphrasesearchquery)(params SearchQuery[]) | Crea una consulta de búsqueda de frase. |
| static [CreateRegexQuery](../../groupdocs.search/searchquery/createregexquery#createregexquery)(string) | Crea una consulta de expresión regular. |
| static [CreateRegexQuery](../../groupdocs.search/searchquery/createregexquery#createregexquery_1)(string, RegexOptions) | Crea una consulta de expresión regular. |
| static [CreateWildcardQuery](../../groupdocs.search/searchquery/createwildcardquery#createwildcardquery)(int) | Crea un comodín para la búsqueda de frase. |
| static [CreateWildcardQuery](../../groupdocs.search/searchquery/createwildcardquery#createwildcardquery_1)(int, int) | Crea un comodín para la búsqueda de frase. |
| static [CreateWordPatternQuery](../../groupdocs.search/searchquery/createwordpatternquery)(WordPattern) | Crea una consulta de patrón de palabras. |
| static [CreateWordQuery](../../groupdocs.search/searchquery/createwordquery)(string) | Crea una consulta de palabra simple. |
| abstract [GetChild](../../groupdocs.search/searchquery/getchild)(int) | Obtiene una consulta secundaria por un índice. |
| abstract [ToString](../../groupdocs.search/searchquery/tostring)() | Devuelve unString que representa la corriente[`SearchQuery`](../searchquery) instancia. |

### Observaciones

**Aprende más**

* [buscando](https://docs.groupdocs.com/display/searchnet/Searching)
* [Consultas en forma de texto y objeto](https://docs.groupdocs.com/display/searchnet/Queries+in+text+and+object+form)
* [Consultas de búsqueda anidadas en forma de objeto](https://docs.groupdocs.com/display/searchnet/Nesting+search+queries+in+object+form)

### Ejemplos

El ejemplo demuestra un uso típico de la clase.

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

* espacio de nombres [GroupDocs.Search](../../groupdocs.search)
* asamblea [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
