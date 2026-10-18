---
title: "ImageSearchOptions"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Proporciona opciones para la operación de búsqueda inversa de imágenes."
type: docs
weight: 24
url: /es/java/com.groupdocs.search.options/imagesearchoptions/
---
**Inheritance:**
java.lang.Object
```
public class ImageSearchOptions
```

Proporciona opciones para la operación de búsqueda inversa de imágenes.

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [ImageSearchOptions()](#ImageSearchOptions--) | Inicializa una nueva instancia de la clase  ImageSearchOptions . |
|
|  | [ImageSearchOptions(Object data)](#ImageSearchOptions-java.lang.Object-) | Inicializa una nueva instancia de la clase  ImageSearchOptions . |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getHashDifferences()](#getHashDifferences--) | Obtiene el número máximo de bits no coincidentes en el hash de la imagen. |
|
|  | [setHashDifferences(int value)](#setHashDifferences-int-) | Establece el número máximo de bits no coincidentes en el hash de la imagen. |
|
|  | [getMaxResultCount()](#getMaxResultCount--) | Obtiene el número máximo de imágenes encontradas para una solicitud de búsqueda inversa de imagen. |
|
|  | [setMaxResultCount(int value)](#setMaxResultCount-int-) | Establece el número máximo de imágenes encontradas para una solicitud de búsqueda inversa de imagen. |
|
|  | [getSearchDocumentFilter()](#getSearchDocumentFilter--) | Obtiene el filtro de documento de búsqueda. |
|
|  | [setSearchDocumentFilter(ISearchDocumentFilter value)](#setSearchDocumentFilter-com.groupdocs.search.options.ISearchDocumentFilter-) | Obtiene o establece el filtro de documento de búsqueda. |
|
| [getCore()](#getCore--) |  |
### ImageSearchOptions() {#ImageSearchOptions--}
```
public ImageSearchOptions()
```


Inicializa una nueva instancia de la clase  ImageSearchOptions .


### ImageSearchOptions(Object data) {#ImageSearchOptions-java.lang.Object-}
```
public ImageSearchOptions(Object data)
```


Inicializa una nueva instancia de la clase  ImageSearchOptions .


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | datos | java.lang.Object | Los datos serializados. |
|

### getHashDifferences() {#getHashDifferences--}
```
public int getHashDifferences()
```


Obtiene el número máximo de bits no coincidentes en el hash de la imagen. El valor predeterminado es  5 .


**Returns:**
int - El número máximo de bits no coincidentes en el hash de la imagen.

### setHashDifferences(int value) {#setHashDifferences-int-}
```
public void setHashDifferences(int value)
```


Establece el número máximo de bits no coincidentes en el hash de la imagen. El valor predeterminado es 5.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | int | El número máximo de bits no coincidentes en el hash de la imagen. |
|

### getMaxResultCount() {#getMaxResultCount--}
```
public int getMaxResultCount()
```


Obtiene el número máximo de imágenes encontradas para una solicitud de búsqueda inversa de imágenes. El valor predeterminado es 1000.


**Returns:**
int - El número máximo de imágenes encontradas para una solicitud de búsqueda inversa de imágenes.

### setMaxResultCount(int value) {#setMaxResultCount-int-}
```
public void setMaxResultCount(int value)
```


Establece el número máximo de imágenes encontradas para una solicitud de búsqueda inversa de imágenes. El valor predeterminado es 1000.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | int | El número máximo de imágenes encontradas para una solicitud de búsqueda inversa de imágenes. |
|

### getSearchDocumentFilter() {#getSearchDocumentFilter--}
```
public ISearchDocumentFilter getSearchDocumentFilter()
```


Obtiene el filtro de documento de búsqueda.  SearchDocumentFilter  funciona con la lógica de inclusión. Use la clase  GroupDocs.Search.Options.SearchDocumentFilter  para crear instancias del filtro de documento de búsqueda. El valor predeterminado es null, lo que significa que se devolverán todos los documentos encontrados.


**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - The search document filter.

### setSearchDocumentFilter(ISearchDocumentFilter value) {#setSearchDocumentFilter-com.groupdocs.search.options.ISearchDocumentFilter-}
```
public void setSearchDocumentFilter(ISearchDocumentFilter value)
```


Obtiene o establece el filtro de documento de búsqueda.  SearchDocumentFilter  funciona con la lógica de inclusión. Use la clase  GroupDocs.Search.Options.SearchDocumentFilter  para crear instancias del filtro de documento de búsqueda. El valor predeterminado es null, lo que significa que se devolverán todos los documentos encontrados.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | value | [ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) | El filtro de documento de búsqueda. |
|

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
