---
title: "SearchDocumentFilter"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Bevat methoden voor het maken van zoekdocumentfilters."
type: docs
weight: 24
url: /nl/java/com.groupdocs.search/searchdocumentfilter/
---
**Inheritance:**
java.lang.Object
```
public class SearchDocumentFilter
```

Bevat methoden voor het maken van zoekdocumentfilters.


**Learn more**

* [Document filtering in search result](../https://docs.groupdocs.com/display/searchjava/Document+filtering+in+search+result)
* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [SearchDocumentFilter()](#SearchDocumentFilter--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [createFilePathRegularExpression(String pattern)](#createFilePathRegularExpression-java.lang.String-) | Maakt een filter om documenten over te slaan die niet overeenkomen met een reguliere expressie. |
|
|  | [createFilePathRegularExpression(String pattern, int options)](#createFilePathRegularExpression-java.lang.String-int-) | Maakt een filter om documenten over te slaan die niet overeenkomen met een reguliere expressie. |
|
|  | [createFileExtension(String[] extensions)](#createFileExtension-java.lang.String...-) | Maakt een filter om documenten over te slaan die niet in de opgegeven lijst van mogelijke extensies staan. |
|
|  | [createNot(ISearchDocumentFilter innerFilter)](#createNot-com.groupdocs.search.options.ISearchDocumentFilter-) | Maakt een filter dat een omgekeerde logica heeft ten opzichte van het opgegeven interne filter. |
|
|  | [createAnd(ISearchDocumentFilter[] filters)](#createAnd-com.groupdocs.search.options.ISearchDocumentFilter...-) | Maakt een logische conjunctie van de opgegeven filters. |
|
|  | [createOr(ISearchDocumentFilter[] filters)](#createOr-com.groupdocs.search.options.ISearchDocumentFilter...-) | Maakt een logische disjunctie van de opgegeven filters. |
|
|  | [createAttribute(String[] attributes)](#createAttribute-java.lang.String...-) | Maakt een filter om documenten over te slaan die geen enkele waarde hebben uit de opgegeven lijst van toegestane attributen. |
|
### SearchDocumentFilter() {#SearchDocumentFilter--}
```
public SearchDocumentFilter()
```


### createFilePathRegularExpression(String pattern) {#createFilePathRegularExpression-java.lang.String-}
```
public static ISearchDocumentFilter createFilePathRegularExpression(String pattern)
```


Maakt een filter om documenten over te slaan die niet overeenkomen met een reguliere expressie. De reguliere expressie wordt toegepast op het volledige pad van een document.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | pattern | java.lang.String | Het patroon van de reguliere expressie. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter by file name.

### createFilePathRegularExpression(String pattern, int options) {#createFilePathRegularExpression-java.lang.String-int-}
```
public static ISearchDocumentFilter createFilePathRegularExpression(String pattern, int options)
```


Maakt een filter om documenten over te slaan die niet overeenkomen met een reguliere expressie. De reguliere expressie wordt toegepast op het volledige pad van een document.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | pattern | java.lang.String | Het patroon van de reguliere expressie. |
|
|  | options | int | De opties van de reguliere expressie. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter by file name.

### createFileExtension(String[] extensions) {#createFileExtension-java.lang.String...-}
```
public static ISearchDocumentFilter createFileExtension(String[] extensions)
```


Maakt een filter om documenten over te slaan die niet in de opgegeven lijst van mogelijke extensies staan.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | extensions | java.lang.String[] | De lijst met mogelijke extensies. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter by document extension.

### createNot(ISearchDocumentFilter innerFilter) {#createNot-com.groupdocs.search.options.ISearchDocumentFilter-}
```
public static ISearchDocumentFilter createNot(ISearchDocumentFilter innerFilter)
```


Maakt een filter dat een omgekeerde logica heeft ten opzichte van het opgegeven interne filter.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | innerFilter | [ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) | Het interne zoekdocumentfilter. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - An inverted search document filter.

### createAnd(ISearchDocumentFilter[] filters) {#createAnd-com.groupdocs.search.options.ISearchDocumentFilter...-}
```
public static ISearchDocumentFilter createAnd(ISearchDocumentFilter[] filters)
```


Maakt een logische conjunctie van de opgegeven filters.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | filters | [ISearchDocumentFilter\[\]](../../com.groupdocs.search.options/isearchdocumentfilter) | De zoekdocumentfilters. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter that represents result of conjunction of the specified filters.

### createOr(ISearchDocumentFilter[] filters) {#createOr-com.groupdocs.search.options.ISearchDocumentFilter...-}
```
public static ISearchDocumentFilter createOr(ISearchDocumentFilter[] filters)
```


Maakt een logische disjunctie van de opgegeven filters.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | filters | [ISearchDocumentFilter\[\]](../../com.groupdocs.search.options/isearchdocumentfilter) | De zoekdocumentfilters. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter that represents result of disjunction of the specified filters.

### createAttribute(String[] attributes) {#createAttribute-java.lang.String...-}
```
public static ISearchDocumentFilter createAttribute(String[] attributes)
```


Maakt een filter om documenten over te slaan die geen enkele waarde hebben uit de opgegeven lijst van toegestane attributen.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | attributen | java.lang.String[] | De lijst met toegestane attributen. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter by document attribute.

