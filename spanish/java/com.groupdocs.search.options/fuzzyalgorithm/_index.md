---
title: "FuzzyAlgorithm"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa la clase base para algoritmos de búsqueda difusa."
type: docs
weight: 20
url: /es/java/com.groupdocs.search.options/fuzzyalgorithm/
---
**Inheritance:**
java.lang.Object
```
public abstract class FuzzyAlgorithm
```

Representa la clase base para algoritmos de búsqueda difusa.


**Learn more**

* [Fuzzy search](../https://docs.groupdocs.com/display/searchjava/Fuzzy+search)

## Métodos

| Método | Descripción |
| --- | --- |
|  | [getSimilarityLevel(int termLength)](#getSimilarityLevel-int-) | Obtiene el nivel de similitud para la longitud de término especificada. |
|
|  | [getMaxMistakeCount(int termLength)](#getMaxMistakeCount-int-) | Obtiene el número máximo permitido de errores para la longitud de término especificada. |
|
| [getCore()](#getCore--) |  |
### getSimilarityLevel(int termLength) {#getSimilarityLevel-int-}
```
public abstract double getSimilarityLevel(int termLength)
```


Obtiene el nivel de similitud para la longitud de término especificada.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | termLength | int | La longitud del término. |
|

**Returns:**
double - El nivel de similitud.

### getMaxMistakeCount(int termLength) {#getMaxMistakeCount-int-}
```
public abstract int getMaxMistakeCount(int termLength)
```


Obtiene el número máximo permitido de errores para la longitud de término especificada.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | termLength | int | La longitud del término. |
|

**Returns:**
int - El número máximo permitido de errores.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
