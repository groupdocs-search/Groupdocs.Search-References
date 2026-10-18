---
title: "SimilarityLevel"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa un algoritmo de búsqueda difusa que especifica el nivel de similitud."
type: docs
weight: 35
url: /es/java/com.groupdocs.search.options/similaritylevel/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.options.FuzzyAlgorithm](../../com.groupdocs.search.options/fuzzyalgorithm)
```
public class SimilarityLevel extends FuzzyAlgorithm
```

Representa un algoritmo de búsqueda difusa que especifica el nivel de similitud. El algoritmo de nivel de similitud calcula el número máximo de errores para una palabra de forma inversamente proporcional a la longitud de la palabra.


**Learn more**

* [Fuzzy search](../https://docs.groupdocs.com/display/searchjava/Fuzzy+search)


El ejemplo muestra un uso típico de la clase.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Creando un índice en la carpeta especificada
index.add(documentsFolder); // Indexando documentos de la carpeta especificada
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // Habilitando la búsqueda difusa
options.getFuzzySearch().setFuzzyAlgorithm(new SimilarityLevel(0.8)); // Creando el algoritmo de búsqueda difusa
// Esta función especifica 0 como el número máximo de errores para palabras de 1 a 4 caracteres.
// Especifica 1 como el número máximo de errores para palabras de 5 a 9 caracteres.
// Especifica 2 como el número máximo de errores para palabras de 10 a 14 caracteres. Y así sucesivamente.
SearchResult result = index.search(query, options); // Buscar en el índice
 
```
 
````


## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [SimilarityLevel(double value)](#SimilarityLevel-double-) | Inicializa una nueva instancia de la clase  SimilarityLevel  . |
|
|  | [SimilarityLevel(Object data)](#SimilarityLevel-java.lang.Object-) | Inicializa una nueva instancia de la clase  SimilarityLevel  . |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getSimilarityLevel(int termLength)](#getSimilarityLevel-int-) | Obtiene el valor del nivel de similitud para la longitud de término especificada. |
|
|  | [getMaxMistakeCount(int termLength)](#getMaxMistakeCount-int-) | Obtiene el número máximo permitido de errores para la longitud de término especificada. |
|
### SimilarityLevel(double value) {#SimilarityLevel-double-}
```
public SimilarityLevel(double value)
```


Inicializa una nueva instancia de la clase  SimilarityLevel  .


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | double | El valor del nivel de similitud. |
|

### SimilarityLevel(Object data) {#SimilarityLevel-java.lang.Object-}
```
public SimilarityLevel(Object data)
```


Inicializa una nueva instancia de la clase  SimilarityLevel  .


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | datos | java.lang.Object | Los datos serializados. |
|

### getSimilarityLevel(int termLength) {#getSimilarityLevel-int-}
```
public double getSimilarityLevel(int termLength)
```


Obtiene el valor del nivel de similitud para la longitud de término especificada.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | termLength | int | La longitud del término. |
|

**Returns:**
double - El valor del nivel de similitud.

### getMaxMistakeCount(int termLength) {#getMaxMistakeCount-int-}
```
public int getMaxMistakeCount(int termLength)
```


Obtiene el número máximo permitido de errores para la longitud de término especificada.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | termLength | int | La longitud del término. |
|

**Returns:**
int - El número máximo permitido de errores.

