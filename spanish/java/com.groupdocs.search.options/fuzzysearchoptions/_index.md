---
title: "FuzzySearchOptions"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Proporciona opciones de la búsqueda difusa."
type: docs
weight: 21
url: /es/java/com.groupdocs.search.options/fuzzysearchoptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class FuzzySearchOptions
```

Proporciona opciones de la búsqueda difusa.


**Learn more**

* [Fuzzy search](../https://docs.groupdocs.com/display/searchjava/Fuzzy+search)
* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## Constructores

| Constructor | Descripción |
| --- | --- |
| [FuzzySearchOptions()](#FuzzySearchOptions--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getEnabled()](#getEnabled--) | Obtiene un valor que indica si la función de búsqueda difusa está habilitada. |
|
|  | [setEnabled(boolean value)](#setEnabled-boolean-) | Establece un valor que indica si la función de búsqueda difusa está habilitada. |
|
|  | [getFuzzyAlgorithm()](#getFuzzyAlgorithm--) | Obtiene el algoritmo de búsqueda difusa. |
|
|  | [setFuzzyAlgorithm(FuzzyAlgorithm value)](#setFuzzyAlgorithm-com.groupdocs.search.options.FuzzyAlgorithm-) | Establece el algoritmo de búsqueda difusa. |
|
|  | [getOnlyBestResults()](#getOnlyBestResults--) | Obtiene un valor que indica si solo se devolverán los mejores resultados. |
|
|  | [setOnlyBestResults(boolean value)](#setOnlyBestResults-boolean-) | Establece un valor que indica si solo se devolverán los mejores resultados. |
|
|  | [getOnlyBestResultsRange()](#getOnlyBestResultsRange--) | Obtiene el exceso máximo del número mínimo de errores que se encuentran. |
|
|  | [setOnlyBestResultsRange(byte value)](#setOnlyBestResultsRange-byte-) | Establece el exceso máximo del número mínimo de errores que se encuentran. |
|
|  | [getConsiderTranspositions()](#getConsiderTranspositions--) | Obtiene un valor que indica si el algoritmo de búsqueda difusa debe considerar la transposición de dos caracteres adyacentes como un solo error. |
|
|  | [setConsiderTranspositions(boolean value)](#setConsiderTranspositions-boolean-) | Establece un valor que indica si el algoritmo de búsqueda difusa debe considerar la transposición de dos caracteres adyacentes como un solo error. |
|
### FuzzySearchOptions() {#FuzzySearchOptions--}
```
public FuzzySearchOptions()
```


### getEnabled() {#getEnabled--}
```
public abstract boolean getEnabled()
```


Obtiene un valor que indica si la función de búsqueda difusa está habilitada. El valor predeterminado es  false .


**Returns:**
boolean - Un valor que indica si la función de búsqueda difusa está habilitada.

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public abstract void setEnabled(boolean value)
```


Establece un valor que indica si la función de búsqueda difusa está habilitada. El valor predeterminado es  false .


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | boolean | Un valor que indica si la función de búsqueda difusa está habilitada. |
|

### getFuzzyAlgorithm() {#getFuzzyAlgorithm--}
```
public abstract FuzzyAlgorithm getFuzzyAlgorithm()
```


Obtiene el algoritmo de búsqueda difusa. Los algoritmos de búsqueda difusa disponibles actualmente son  SimilarityLevel  y  TableDiscreteFunction . El valor predeterminado es una instancia de  SimilarityLevel  con un valor de nivel de similitud de  0.5 .


**Returns:**
[FuzzyAlgorithm](../../com.groupdocs.search.options/fuzzyalgorithm) - The fuzzy search algorithm.


El ejemplo muestra cómo establecer el algoritmo de búsqueda difusa.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Creando un índice en la carpeta especificada
index.add(documentsFolder); // Indexando documentos de la carpeta especificada
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // Habilitando la búsqueda difusa
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1, new Step(5, 2), new Step(8, 3))); // Creando el algoritmo de búsqueda difusa
// Esta función especifica 1 como el número máximo de errores para palabras de 1 a 4 caracteres.
// Especifica 2 como el número máximo de errores para palabras de 5 a 7 caracteres.
// Especifica 3 como el número máximo de errores para palabras de 8 caracteres o más.
SearchResult result = index.search(query, options); // Buscar en el índice
 
```
 
````


### setFuzzyAlgorithm(FuzzyAlgorithm value) {#setFuzzyAlgorithm-com.groupdocs.search.options.FuzzyAlgorithm-}
```
public abstract void setFuzzyAlgorithm(FuzzyAlgorithm value)
```


Establece el algoritmo de búsqueda difusa. Los algoritmos de búsqueda difusa disponibles actualmente son  SimilarityLevel  y  TableDiscreteFunction . El valor predeterminado es una instancia de  SimilarityLevel  con un valor de nivel de similitud de  0.5 .


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | value | [FuzzyAlgorithm](../../com.groupdocs.search.options/fuzzyalgorithm) | El algoritmo de búsqueda difusa. |


El ejemplo muestra cómo establecer el algoritmo de búsqueda difusa.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Creando un índice en la carpeta especificada
index.add(documentsFolder); // Indexando documentos de la carpeta especificada
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // Habilitando la búsqueda difusa
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1, new Step(5, 2), new Step(8, 3))); // Creando el algoritmo de búsqueda difusa
// Esta función especifica 1 como el número máximo de errores para palabras de 1 a 4 caracteres.
// Especifica 2 como el número máximo de errores para palabras de 5 a 7 caracteres.
// Especifica 3 como el número máximo de errores para palabras de 8 caracteres o más.
SearchResult result = index.search(query, options); // Buscar en el índice
 
```
 
````

|

### getOnlyBestResults() {#getOnlyBestResults--}
```
public abstract boolean getOnlyBestResults()
```


Obtiene un valor que indica si solo se devolverán los mejores resultados. El valor predeterminado es  false .


**Returns:**
boolean -  true  si solo se devolverán los mejores resultados; de lo contrario  false .

### setOnlyBestResults(boolean value) {#setOnlyBestResults-boolean-}
```
public abstract void setOnlyBestResults(boolean value)
```


Establece un valor que indica si solo se devolverán los mejores resultados. El valor predeterminado es  false .


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | boolean | true  si solo se devolverán los mejores resultados; de lo contrario  false . |
|

### getOnlyBestResultsRange() {#getOnlyBestResultsRange--}
```
public abstract byte getOnlyBestResultsRange()
```


Obtiene el exceso máximo del número mínimo de errores que se encuentran. El valor predeterminado es  0 .


**Returns:**
byte - El exceso máximo del número mínimo de errores encontrados.

### setOnlyBestResultsRange(byte value) {#setOnlyBestResultsRange-byte-}
```
public abstract void setOnlyBestResultsRange(byte value)
```


Establece el exceso máximo del número mínimo de errores que se encuentran. El valor predeterminado es  0 .


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | byte | El exceso máximo del número mínimo de errores encontrados. |
|

### getConsiderTranspositions() {#getConsiderTranspositions--}
```
public abstract boolean getConsiderTranspositions()
```


Obtiene un valor que indica si el algoritmo de búsqueda difusa debe considerar la transposición de dos caracteres adyacentes como un solo error. El valor predeterminado es  true .


**Returns:**
boolean -  true  si el algoritmo de búsqueda difusa considera transposiciones; de lo contrario  false .

### setConsiderTranspositions(boolean value) {#setConsiderTranspositions-boolean-}
```
public abstract void setConsiderTranspositions(boolean value)
```


Establece un valor que indica si el algoritmo de búsqueda difusa debe considerar la transposición de dos caracteres adyacentes como un solo error. El valor predeterminado es  true .


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | boolean | :  true  si el algoritmo de búsqueda difusa considera transposiciones; de lo contrario  false . |
|

