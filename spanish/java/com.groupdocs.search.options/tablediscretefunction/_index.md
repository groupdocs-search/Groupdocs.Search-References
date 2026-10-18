---
title: "TableDiscreteFunction"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa el algoritmo de búsqueda difusa que contiene correspondencias entre la longitud de palabras y el número de errores permitidos."
type: docs
weight: 40
url: /es/java/com.groupdocs.search.options/tablediscretefunction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.options.FuzzyAlgorithm](../../com.groupdocs.search.options/fuzzyalgorithm)
```
public class TableDiscreteFunction extends FuzzyAlgorithm
```

Representa el algoritmo de búsqueda difusa que contiene correspondencias entre longitudes de palabras y el número de errores permitidos. Este algoritmo puede especificarse mediante una tabla de valores de salida o mediante una función escalonada.


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
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1, new Step(5, 2), new Step(8, 3))); // Creando el algoritmo de búsqueda difusa
// Esta función especifica 1 como el número máximo de errores para palabras de 1 a 4 caracteres.
// Especifica 2 como el número máximo de errores para palabras de 5 a 7 caracteres.
// Especifica 3 como el número máximo de errores para palabras de 8 caracteres o más.
SearchResult result = index.search(query, options); // Buscar en el índice
 
```
 
````


## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [TableDiscreteFunction(int offsetOfInputs, int[] tableOfOutputs)](#TableDiscreteFunction-int-int---) | Inicializa una nueva instancia de la clase  TableDiscreteFunction . |
|
|  | [TableDiscreteFunction(int firstStepLevel, Step[] steps)](#TableDiscreteFunction-int-com.groupdocs.search.options.Step...-) | Inicializa una nueva instancia de la clase  TableDiscreteFunction . |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getSimilarityLevel(int termLength)](#getSimilarityLevel-int-) | Obtiene un nivel de similitud para la longitud de término especificada. |
|
|  | [getMaxMistakeCount(int termLength)](#getMaxMistakeCount-int-) | Obtiene el número máximo permitido de errores para la longitud de término especificada. |
|
### TableDiscreteFunction(int offsetOfInputs, int[] tableOfOutputs) {#TableDiscreteFunction-int-int---}
```
public TableDiscreteFunction(int offsetOfInputs, int[] tableOfOutputs)
```


Inicializa una nueva instancia de la clase  TableDiscreteFunction .


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | offsetOfInputs | int | El desplazamiento de los índices de la tabla relativo a los valores de entrada. |
|
|  | tableOfOutputs | int[] | La tabla de valores de salida. |
|

### TableDiscreteFunction(int firstStepLevel, Step[] steps) {#TableDiscreteFunction-int-com.groupdocs.search.options.Step...-}
```
public TableDiscreteFunction(int firstStepLevel, Step[] steps)
```


Inicializa una nueva instancia de la clase  TableDiscreteFunction .


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | firstStepLevel | int | El nivel del primer paso de la función escalón. |
|
|  | steps | [Step\[\]](../../com.groupdocs.search.options/step) | Los siguientes pasos de la función escalón. |
|

### getSimilarityLevel(int termLength) {#getSimilarityLevel-int-}
```
public double getSimilarityLevel(int termLength)
```


Obtiene un nivel de similitud para la longitud de término especificada.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | termLength | int | La longitud del término. |
|

**Returns:**
double - Un nivel de similitud.

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
int - Un número máximo permitido de errores.

