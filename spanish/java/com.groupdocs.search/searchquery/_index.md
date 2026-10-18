---
title: "SearchQuery"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa una consulta de búsqueda en forma de objeto."
type: docs
weight: 25
url: /es/java/com.groupdocs.search/searchquery/
---
**Inheritance:**
java.lang.Object
```
public abstract class SearchQuery
```

Representa una consulta de búsqueda en forma de objeto.


**Learn more**

* [Searching](../https://docs.groupdocs.com/display/searchjava/Searching)
* [Queries in text and object form](../https://docs.groupdocs.com/display/searchjava/Queries+in+text+and+object+form)
* [Nesting search queries in object form](../https://docs.groupdocs.com/display/searchjava/Nesting+search+queries+in+object+form)


El ejemplo muestra un uso típico de la clase.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
 
Index index = new Index(indexFolder); // Creando índice en la carpeta especificada
index.add(documentsFolder); // Indexando documentos de la carpeta especificada
 
// Creando subconsulta de búsqueda por rango de fechas
SearchQuery subquery1 = SearchQuery.createDateRangeQuery(new Date(2011, 6, 17), new Date(2013, 1, 1));
 
// Creando subconsulta de comodín con número de palabras omitidas de 0 a 2
SearchQuery subquery2 = SearchQuery.createWildcardQuery(0, 2);
 
// Creando subconsulta de palabra simple
SearchQuery subquery3 = SearchQuery.createWordQuery("birth");
subquery3.setSearchOptions(new SearchOptions()); // Configurando opciones de búsqueda solo para la subconsulta 3
subquery3.getSearchOptions().getFuzzySearch().setEnabled(true);
subquery3.getSearchOptions().getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1));
 
// Combinando subconsultas en una sola consulta
SearchQuery query = SearchQuery.createPhraseSearchQuery(subquery1, subquery2, subquery3);
 
// Creando objeto de opciones de búsqueda con mayor capacidad de ocurrencias encontradas
SearchOptions options = new SearchOptions(); // Opciones de búsqueda generales
options.setMaxOccurrenceCountPerTerm(1000000);
options.setMaxTotalOccurrenceCount(10000000);
 
SearchResult result = index.search(query, options); // Buscando
 
```
 
````


## Métodos

| Método | Descripción |
| --- | --- |
|  | [getFieldName()](#getFieldName--) | Obtiene el nombre del campo. |
|
|  | [getChildCount()](#getChildCount--) | Obtiene el número de consultas hijas. |
|
|  | [getFirstChild()](#getFirstChild--) | Obtiene la primera consulta hija. |
|
|  | [getSecondChild()](#getSecondChild--) | Obtiene la segunda consulta hija. |
|
|  | [getChild(int index)](#getChild-int-) | Obtiene una consulta hija por un índice. |
|
|  | [getSearchOptions()](#getSearchOptions--) | Obtiene o establece las opciones de búsqueda de esta seach query. |
|
|  | [setSearchOptions(SearchOptions value)](#setSearchOptions-com.groupdocs.search.options.SearchOptions-) | Obtiene o establece las opciones de búsqueda de esta seach query. |
|
|  | [toString()](#toString--) | Devuelve un  System.String  que representa la instancia actual de  SearchQuery. |
|
|  | [createWordQuery(String term)](#createWordQuery-java.lang.String-) | Crea una consulta de palabra simple. |
|
|  | [createWordPatternQuery(WordPattern pattern)](#createWordPatternQuery-com.groupdocs.search.common.WordPattern-) | Crea una consulta de patrón de palabra. |
|
|  | [createRegexQuery(String pattern)](#createRegexQuery-java.lang.String-) | Crea una consulta de expresión regular. |
|
|  | [createRegexQuery(String pattern, int options)](#createRegexQuery-java.lang.String-int-) | Crea una consulta de expresión regular. |
|
|  | [createNumericRangeQuery(long start, long end)](#createNumericRangeQuery-long-long-) | Crea una consulta de rango numérico. |
|
|  | [createDateRangeQuery(Date start, Date end)](#createDateRangeQuery-java.util.Date-java.util.Date-) | Crea una consulta de rango de fechas. |
|
|  | [createPhraseSearchQuery(SearchQuery[] queries)](#createPhraseSearchQuery-com.groupdocs.search.SearchQuery...-) | Crea una consulta de búsqueda de frase. |
|
|  | [createAndQuery(SearchQuery[] queries)](#createAndQuery-com.groupdocs.search.SearchQuery---) | Crea una consulta combinada que encontrará solo los documentos que se encontrarán para cada consulta original. |
|
|  | [createFieldQuery(String fieldName, SearchQuery query)](#createFieldQuery-java.lang.String-com.groupdocs.search.SearchQuery-) | Agrega un campo a la consulta especificada. |
|
|  | [createNotQuery(SearchQuery query)](#createNotQuery-com.groupdocs.search.SearchQuery-) | Crea una consulta invertida que encontrará los documentos restantes en un índice frente a los que se encontrarán para la consulta original. |
|
|  | [createAndQuery(SearchQuery leftQuery, SearchQuery rightQuery)](#createAndQuery-com.groupdocs.search.SearchQuery-com.groupdocs.search.SearchQuery-) | Crea una consulta combinada que encontrará solo los documentos que se encontrarán para cada consulta original. |
|
|  | [createOrQuery(SearchQuery leftQuery, SearchQuery rightQuery)](#createOrQuery-com.groupdocs.search.SearchQuery-com.groupdocs.search.SearchQuery-) | Crea una consulta combinada que encontrará todos los documentos que se encontrarán al menos en una de las consultas originales. |
|
|  | [createOrQuery(SearchQuery[] queries)](#createOrQuery-com.groupdocs.search.SearchQuery---) | Crea una consulta combinada que encontrará todos los documentos que se encontrarán al menos en una de las consultas originales. |
|
|  | [createWildcardQuery(int count)](#createWildcardQuery-int-) | Crea un comodín para la búsqueda de frase. |
|
|  | [createWildcardQuery(int minCount, int maxCount)](#createWildcardQuery-int-int-) | Crea un comodín para la búsqueda de frase. |
|
### getFieldName() {#getFieldName--}
```
public String getFieldName()
```


Obtiene el nombre del campo.


**Returns:**
java.lang.String - El nombre del campo.

### getChildCount() {#getChildCount--}
```
public int getChildCount()
```


Obtiene el número de consultas hijas.


**Returns:**
int - El número de consultas secundarias.

### getFirstChild() {#getFirstChild--}
```
public SearchQuery getFirstChild()
```


Obtiene la primera consulta hija.


**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - The first child query.

### getSecondChild() {#getSecondChild--}
```
public SearchQuery getSecondChild()
```


Obtiene la segunda consulta hija.


**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - The second child query.

### getChild(int index) {#getChild-int-}
```
public abstract SearchQuery getChild(int index)
```


Obtiene una consulta hija por un índice.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | índice | int | El índice. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A child query corresponding the specified index.

### getSearchOptions() {#getSearchOptions--}
```
public final SearchOptions getSearchOptions()
```


Obtiene o establece las opciones de búsqueda de esta seach query.


**Returns:**
[SearchOptions](../../com.groupdocs.search.options/searchoptions) - The search options.

### setSearchOptions(SearchOptions value) {#setSearchOptions-com.groupdocs.search.options.SearchOptions-}
```
public final void setSearchOptions(SearchOptions value)
```


Obtiene o establece las opciones de búsqueda de esta seach query.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | value | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | Las opciones de búsqueda. |
|

### toString() {#toString--}
```
public abstract String toString()
```


Devuelve un  System.String  que representa la instancia actual de  SearchQuery.


**Returns:**
java.lang.String - Un  System.String  que representa la instancia actual de  SearchQuery.

### createWordQuery(String term) {#createWordQuery-java.lang.String-}
```
public static SearchQuery createWordQuery(String term)
```


Crea una consulta de palabra simple.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | término | java.lang.String | El término a buscar. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A simple word query.

### createWordPatternQuery(WordPattern pattern) {#createWordPatternQuery-com.groupdocs.search.common.WordPattern-}
```
public static SearchQuery createWordPatternQuery(WordPattern pattern)
```


Crea una consulta de patrón de palabra.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | pattern | [WordPattern](../../com.groupdocs.search.common/wordpattern) | El patrón de palabra. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A word pattern query.

### createRegexQuery(String pattern) {#createRegexQuery-java.lang.String-}
```
public static SearchQuery createRegexQuery(String pattern)
```


Crea una consulta de expresión regular.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | pattern | java.lang.String | El patrón de expresión regular a coincidir. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A regular expression query.

### createRegexQuery(String pattern, int options) {#createRegexQuery-java.lang.String-int-}
```
public static SearchQuery createRegexQuery(String pattern, int options)
```


Crea una consulta de expresión regular.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | pattern | java.lang.String | El patrón de expresión regular a coincidir. |
|
|  | options | int | Una combinación bit a bit de los valores de enumeración que modifican la expresión regular. Este valor debe contener  RegexOptions.IgnoreCase  bandera. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A regular expression query.

### createNumericRangeQuery(long start, long end) {#createNumericRangeQuery-long-long-}
```
public static SearchQuery createNumericRangeQuery(long start, long end)
```


Crea una consulta de rango numérico.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | inicio | long | El valor de inicio de un rango. |
|
|  | fin | long | El valor final de un rango. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A numeric range query.

### createDateRangeQuery(Date start, Date end) {#createDateRangeQuery-java.util.Date-java.util.Date-}
```
public static SearchQuery createDateRangeQuery(Date start, Date end)
```


Crea una consulta de rango de fechas.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | inicio | java.util.Date | El valor de inicio de un rango. |
|
|  | fin | java.util.Date | El valor final de un rango. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A date range query.

### createPhraseSearchQuery(SearchQuery[] queries) {#createPhraseSearchQuery-com.groupdocs.search.SearchQuery...-}
```
public static SearchQuery createPhraseSearchQuery(SearchQuery[] queries)
```


Crea una consulta de búsqueda de frase.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | queries | [SearchQuery\[\]](../../com.groupdocs.search/searchquery) | Las consultas secundarias. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A phrase search query.

### createAndQuery(SearchQuery[] queries) {#createAndQuery-com.groupdocs.search.SearchQuery---}
```
public static SearchQuery createAndQuery(SearchQuery[] queries)
```


Crea una consulta combinada que encontrará solo los documentos que se encontrarán para cada consulta original.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | queries | [SearchQuery\[\]](../../com.groupdocs.search/searchquery) | El nombre del campo en el que buscar. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined AND query.

### createFieldQuery(String fieldName, SearchQuery query) {#createFieldQuery-java.lang.String-com.groupdocs.search.SearchQuery-}
```
public static SearchQuery createFieldQuery(String fieldName, SearchQuery query)
```


Agrega un campo a la consulta especificada.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | fieldName | java.lang.String | El nombre del campo en el que buscar. |
|
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | La consulta para agregar el campo. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A query with the field to search in.

### createNotQuery(SearchQuery query) {#createNotQuery-com.groupdocs.search.SearchQuery-}
```
public static SearchQuery createNotQuery(SearchQuery query)
```


Crea una consulta invertida que encontrará los documentos restantes en un índice frente a los que se encontrarán para la consulta original.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | La consulta para invertir. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined NOT query.

### createAndQuery(SearchQuery leftQuery, SearchQuery rightQuery) {#createAndQuery-com.groupdocs.search.SearchQuery-com.groupdocs.search.SearchQuery-}
```
public static SearchQuery createAndQuery(SearchQuery leftQuery, SearchQuery rightQuery)
```


Crea una consulta combinada que encontrará solo los documentos que se encontrarán para cada consulta original.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | leftQuery | [SearchQuery](../../com.groupdocs.search/searchquery) | La consulta del hijo izquierdo. |
|
|  | rightQuery | [SearchQuery](../../com.groupdocs.search/searchquery) | La consulta del hijo derecho. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined AND query.

### createOrQuery(SearchQuery leftQuery, SearchQuery rightQuery) {#createOrQuery-com.groupdocs.search.SearchQuery-com.groupdocs.search.SearchQuery-}
```
public static SearchQuery createOrQuery(SearchQuery leftQuery, SearchQuery rightQuery)
```


Crea una consulta combinada que encontrará todos los documentos que se encontrarán al menos en una de las consultas originales.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | leftQuery | [SearchQuery](../../com.groupdocs.search/searchquery) | La consulta del hijo izquierdo. |
|
|  | rightQuery | [SearchQuery](../../com.groupdocs.search/searchquery) | La consulta del hijo derecho. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined OR query.

### createOrQuery(SearchQuery[] queries) {#createOrQuery-com.groupdocs.search.SearchQuery---}
```
public static SearchQuery createOrQuery(SearchQuery[] queries)
```


Crea una consulta combinada que encontrará todos los documentos que se encontrarán al menos en una de las consultas originales.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | queries | [SearchQuery\[\]](../../com.groupdocs.search/searchquery) | Las consultas secundarias. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined OR query.

### createWildcardQuery(int count) {#createWildcardQuery-int-}
```
public static SearchQuery createWildcardQuery(int count)
```


Crea un comodín para la búsqueda de frase.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | count | int | El número de palabras en el comodín. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A wildcard for the phrase search.

### createWildcardQuery(int minCount, int maxCount) {#createWildcardQuery-int-int-}
```
public static SearchQuery createWildcardQuery(int minCount, int maxCount)
```


Crea un comodín para la búsqueda de frase.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | minCount | int | El número mínimo de palabras en el comodín. |
|
|  | maxCount | int | El número máximo de palabras en el comodín. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A wildcard for the phrase search.

