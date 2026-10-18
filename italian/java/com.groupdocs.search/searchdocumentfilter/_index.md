---
title: "SearchDocumentFilter"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Contiene metodi per creare filtri di documenti di ricerca."
type: docs
weight: 24
url: /it/java/com.groupdocs.search/searchdocumentfilter/
---
**Inheritance:**
java.lang.Object
```
public class SearchDocumentFilter
```

Contiene metodi per creare filtri di documenti di ricerca.


**Learn more**

* [Document filtering in search result](../https://docs.groupdocs.com/display/searchjava/Document+filtering+in+search+result)
* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [SearchDocumentFilter()](#SearchDocumentFilter--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [createFilePathRegularExpression(String pattern)](#createFilePathRegularExpression-java.lang.String-) | Crea un filtro per saltare i documenti che non corrispondono a un'espressione regolare. |
|
|  | [createFilePathRegularExpression(String pattern, int options)](#createFilePathRegularExpression-java.lang.String-int-) | Crea un filtro per saltare i documenti che non corrispondono a un'espressione regolare. |
|
|  | [createFileExtension(String[] extensions)](#createFileExtension-java.lang.String...-) | Crea un filtro per saltare i documenti che non sono nella lista specificata di possibili estensioni. |
|
|  | [createNot(ISearchDocumentFilter innerFilter)](#createNot-com.groupdocs.search.options.ISearchDocumentFilter-) | Crea un filtro che ha una logica inversa rispetto al filtro interno specificato. |
|
|  | [createAnd(ISearchDocumentFilter[] filters)](#createAnd-com.groupdocs.search.options.ISearchDocumentFilter...-) | Crea una congiunzione logica dei filtri specificati. |
|
|  | [createOr(ISearchDocumentFilter[] filters)](#createOr-com.groupdocs.search.options.ISearchDocumentFilter...-) | Crea una disgiunzione logica dei filtri specificati. |
|
|  | [createAttribute(String[] attributes)](#createAttribute-java.lang.String...-) | Crea un filtro per saltare i documenti che non hanno alcun valore dalla lista specificata di attributi consentiti. |
|
### SearchDocumentFilter() {#SearchDocumentFilter--}
```
public SearchDocumentFilter()
```


### createFilePathRegularExpression(String pattern) {#createFilePathRegularExpression-java.lang.String-}
```
public static ISearchDocumentFilter createFilePathRegularExpression(String pattern)
```


Crea un filtro per saltare i documenti che non corrispondono a un'espressione regolare. L'espressione regolare è applicata al percorso completo di un documento.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | pattern | java.lang.String | Il pattern dell'espressione regolare. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter by file name.

### createFilePathRegularExpression(String pattern, int options) {#createFilePathRegularExpression-java.lang.String-int-}
```
public static ISearchDocumentFilter createFilePathRegularExpression(String pattern, int options)
```


Crea un filtro per saltare i documenti che non corrispondono a un'espressione regolare. L'espressione regolare è applicata al percorso completo di un documento.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | pattern | java.lang.String | Il pattern dell'espressione regolare. |
|
|  | options | int | Le opzioni dell'espressione regolare. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter by file name.

### createFileExtension(String[] extensions) {#createFileExtension-java.lang.String...-}
```
public static ISearchDocumentFilter createFileExtension(String[] extensions)
```


Crea un filtro per saltare i documenti che non sono nella lista specificata di possibili estensioni.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | extensions | java.lang.String[] | Elenco delle possibili estensioni. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter by document extension.

### createNot(ISearchDocumentFilter innerFilter) {#createNot-com.groupdocs.search.options.ISearchDocumentFilter-}
```
public static ISearchDocumentFilter createNot(ISearchDocumentFilter innerFilter)
```


Crea un filtro che ha una logica inversa rispetto al filtro interno specificato.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | innerFilter | [ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) | Il filtro interno dei documenti di ricerca. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - An inverted search document filter.

### createAnd(ISearchDocumentFilter[] filters) {#createAnd-com.groupdocs.search.options.ISearchDocumentFilter...-}
```
public static ISearchDocumentFilter createAnd(ISearchDocumentFilter[] filters)
```


Crea una congiunzione logica dei filtri specificati.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | filters | [ISearchDocumentFilter\[\]](../../com.groupdocs.search.options/isearchdocumentfilter) | I filtri dei documenti di ricerca. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter that represents result of conjunction of the specified filters.

### createOr(ISearchDocumentFilter[] filters) {#createOr-com.groupdocs.search.options.ISearchDocumentFilter...-}
```
public static ISearchDocumentFilter createOr(ISearchDocumentFilter[] filters)
```


Crea una disgiunzione logica dei filtri specificati.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | filters | [ISearchDocumentFilter\[\]](../../com.groupdocs.search.options/isearchdocumentfilter) | I filtri dei documenti di ricerca. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter that represents result of disjunction of the specified filters.

### createAttribute(String[] attributes) {#createAttribute-java.lang.String...-}
```
public static ISearchDocumentFilter createAttribute(String[] attributes)
```


Crea un filtro per saltare i documenti che non hanno alcun valore dalla lista specificata di attributi consentiti.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | attributi | java.lang.String[] | Elenco degli attributi consentiti. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter by document attribute.

