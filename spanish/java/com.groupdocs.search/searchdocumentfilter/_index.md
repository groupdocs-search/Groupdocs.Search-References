---
title: "SearchDocumentFilter"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Contiene métodos para crear filtros de documentos de búsqueda."
type: docs
weight: 24
url: /es/java/com.groupdocs.search/searchdocumentfilter/
---
**Inheritance:**
java.lang.Object
```
public class SearchDocumentFilter
```

Contiene métodos para crear filtros de documentos de búsqueda.


**Learn more**

* [Document filtering in search result](../https://docs.groupdocs.com/display/searchjava/Document+filtering+in+search+result)
* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## Constructores

| Constructor | Descripción |
| --- | --- |
| [SearchDocumentFilter()](#SearchDocumentFilter--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
|  | [createFilePathRegularExpression(String pattern)](#createFilePathRegularExpression-java.lang.String-) | Crea un filtro para omitir documentos que no coinciden con una expresión regular. |
|
|  | [createFilePathRegularExpression(String pattern, int options)](#createFilePathRegularExpression-java.lang.String-int-) | Crea un filtro para omitir documentos que no coinciden con una expresión regular. |
|
|  | [createFileExtension(String[] extensions)](#createFileExtension-java.lang.String...-) | Crea un filtro para omitir documentos que no están en la lista especificada de extensiones posibles. |
|
|  | [createNot(ISearchDocumentFilter innerFilter)](#createNot-com.groupdocs.search.options.ISearchDocumentFilter-) | Crea un filtro que tiene lógica inversa en relación con el filtro interno especificado. |
|
|  | [createAnd(ISearchDocumentFilter[] filters)](#createAnd-com.groupdocs.search.options.ISearchDocumentFilter...-) | Crea una conjunción lógica de los filtros especificados. |
|
|  | [createOr(ISearchDocumentFilter[] filters)](#createOr-com.groupdocs.search.options.ISearchDocumentFilter...-) | Crea una disyunción lógica de los filtros especificados. |
|
|  | [createAttribute(String[] attributes)](#createAttribute-java.lang.String...-) | Crea un filtro para omitir documentos que no tienen ningún valor de la lista especificada de atributos permitidos. |
|
### SearchDocumentFilter() {#SearchDocumentFilter--}
```
public SearchDocumentFilter()
```


### createFilePathRegularExpression(String pattern) {#createFilePathRegularExpression-java.lang.String-}
```
public static ISearchDocumentFilter createFilePathRegularExpression(String pattern)
```


Crea un filtro para omitir documentos que no coinciden con una expresión regular. La expresión regular se aplica a la ruta completa de un documento.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | pattern | java.lang.String | El patrón de expresión regular. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter by file name.

### createFilePathRegularExpression(String pattern, int options) {#createFilePathRegularExpression-java.lang.String-int-}
```
public static ISearchDocumentFilter createFilePathRegularExpression(String pattern, int options)
```


Crea un filtro para omitir documentos que no coinciden con una expresión regular. La expresión regular se aplica a la ruta completa de un documento.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | pattern | java.lang.String | El patrón de expresión regular. |
|
|  | options | int | Las opciones de expresión regular. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter by file name.

### createFileExtension(String[] extensions) {#createFileExtension-java.lang.String...-}
```
public static ISearchDocumentFilter createFileExtension(String[] extensions)
```


Crea un filtro para omitir documentos que no están en la lista especificada de extensiones posibles.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | extensions | java.lang.String[] | La lista de extensiones posibles. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter by document extension.

### createNot(ISearchDocumentFilter innerFilter) {#createNot-com.groupdocs.search.options.ISearchDocumentFilter-}
```
public static ISearchDocumentFilter createNot(ISearchDocumentFilter innerFilter)
```


Crea un filtro que tiene lógica inversa en relación con el filtro interno especificado.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | innerFilter | [ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) | El filtro interno de documentos de búsqueda. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - An inverted search document filter.

### createAnd(ISearchDocumentFilter[] filters) {#createAnd-com.groupdocs.search.options.ISearchDocumentFilter...-}
```
public static ISearchDocumentFilter createAnd(ISearchDocumentFilter[] filters)
```


Crea una conjunción lógica de los filtros especificados.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | filters | [ISearchDocumentFilter\[\]](../../com.groupdocs.search.options/isearchdocumentfilter) | Los filtros de documentos de búsqueda. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter that represents result of conjunction of the specified filters.

### createOr(ISearchDocumentFilter[] filters) {#createOr-com.groupdocs.search.options.ISearchDocumentFilter...-}
```
public static ISearchDocumentFilter createOr(ISearchDocumentFilter[] filters)
```


Crea una disyunción lógica de los filtros especificados.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | filters | [ISearchDocumentFilter\[\]](../../com.groupdocs.search.options/isearchdocumentfilter) | Los filtros de documentos de búsqueda. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter that represents result of disjunction of the specified filters.

### createAttribute(String[] attributes) {#createAttribute-java.lang.String...-}
```
public static ISearchDocumentFilter createAttribute(String[] attributes)
```


Crea un filtro para omitir documentos que no tienen ningún valor de la lista especificada de atributos permitidos.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | atributos | java.lang.String[] | La lista de atributos permitidos. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter by document attribute.

