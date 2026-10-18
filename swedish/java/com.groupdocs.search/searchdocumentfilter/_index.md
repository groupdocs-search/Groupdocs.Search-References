---
title: "SearchDocumentFilter"
second_title: "GroupDocs.Search för Java API-referens"
description: "Innehåller metoder för att skapa sökdokumentfilter."
type: docs
weight: 24
url: /sv/java/com.groupdocs.search/searchdocumentfilter/
---
**Inheritance:**
java.lang.Object
```
public class SearchDocumentFilter
```

Innehåller metoder för att skapa sökdokumentfilter.


**Learn more**

* [Document filtering in search result](../https://docs.groupdocs.com/display/searchjava/Document+filtering+in+search+result)
* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [SearchDocumentFilter()](#SearchDocumentFilter--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [createFilePathRegularExpression(String pattern)](#createFilePathRegularExpression-java.lang.String-) | Skapar ett filter för att hoppa över dokument som inte matchar ett reguljärt uttryck. |
|
|  | [createFilePathRegularExpression(String pattern, int options)](#createFilePathRegularExpression-java.lang.String-int-) | Skapar ett filter för att hoppa över dokument som inte matchar ett reguljärt uttryck. |
|
|  | [createFileExtension(String[] extensions)](#createFileExtension-java.lang.String...-) | Skapar ett filter för att hoppa över dokument som inte finns i den angivna listan över möjliga filändelser. |
|
|  | [createNot(ISearchDocumentFilter innerFilter)](#createNot-com.groupdocs.search.options.ISearchDocumentFilter-) | Skapar ett filter som har omvänd logik i förhållande till det angivna inre filtret. |
|
|  | [createAnd(ISearchDocumentFilter[] filters)](#createAnd-com.groupdocs.search.options.ISearchDocumentFilter...-) | Skapar en logisk konjunktion av de angivna filtren. |
|
|  | [createOr(ISearchDocumentFilter[] filters)](#createOr-com.groupdocs.search.options.ISearchDocumentFilter...-) | Skapar en logisk disjunktion av de angivna filtren. |
|
|  | [createAttribute(String[] attributes)](#createAttribute-java.lang.String...-) | Skapar ett filter för att hoppa över dokument som inte har något värde från den angivna listan över tillåtna attribut. |
|
### SearchDocumentFilter() {#SearchDocumentFilter--}
```
public SearchDocumentFilter()
```


### createFilePathRegularExpression(String pattern) {#createFilePathRegularExpression-java.lang.String-}
```
public static ISearchDocumentFilter createFilePathRegularExpression(String pattern)
```


Skapar ett filter för att hoppa över dokument som inte matchar ett reguljärt uttryck. Det reguljära uttrycket tillämpas på dokumentets fullständiga sökväg.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | pattern | java.lang.String | Det reguljära uttrycksmönstret. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter by file name.

### createFilePathRegularExpression(String pattern, int options) {#createFilePathRegularExpression-java.lang.String-int-}
```
public static ISearchDocumentFilter createFilePathRegularExpression(String pattern, int options)
```


Skapar ett filter för att hoppa över dokument som inte matchar ett reguljärt uttryck. Det reguljära uttrycket tillämpas på dokumentets fullständiga sökväg.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | pattern | java.lang.String | Det reguljära uttrycksmönstret. |
|
|  | options | int | Alternativen för det reguljära uttrycket. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter by file name.

### createFileExtension(String[] extensions) {#createFileExtension-java.lang.String...-}
```
public static ISearchDocumentFilter createFileExtension(String[] extensions)
```


Skapar ett filter för att hoppa över dokument som inte finns i den angivna listan över möjliga filändelser.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | filändelser | java.lang.String[] | Listan över möjliga tillägg. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter by document extension.

### createNot(ISearchDocumentFilter innerFilter) {#createNot-com.groupdocs.search.options.ISearchDocumentFilter-}
```
public static ISearchDocumentFilter createNot(ISearchDocumentFilter innerFilter)
```


Skapar ett filter som har omvänd logik i förhållande till det angivna inre filtret.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | innerFilter | [ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) | Det inre sökdokumentfiltret. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - An inverted search document filter.

### createAnd(ISearchDocumentFilter[] filters) {#createAnd-com.groupdocs.search.options.ISearchDocumentFilter...-}
```
public static ISearchDocumentFilter createAnd(ISearchDocumentFilter[] filters)
```


Skapar en logisk konjunktion av de angivna filtren.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | filters | [ISearchDocumentFilter\[\]](../../com.groupdocs.search.options/isearchdocumentfilter) | Sökdokumentfiltren. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter that represents result of conjunction of the specified filters.

### createOr(ISearchDocumentFilter[] filters) {#createOr-com.groupdocs.search.options.ISearchDocumentFilter...-}
```
public static ISearchDocumentFilter createOr(ISearchDocumentFilter[] filters)
```


Skapar en logisk disjunktion av de angivna filtren.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | filters | [ISearchDocumentFilter\[\]](../../com.groupdocs.search.options/isearchdocumentfilter) | Sökdokumentfiltren. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter that represents result of disjunction of the specified filters.

### createAttribute(String[] attributes) {#createAttribute-java.lang.String...-}
```
public static ISearchDocumentFilter createAttribute(String[] attributes)
```


Skapar ett filter för att hoppa över dokument som inte har något värde från den angivna listan över tillåtna attribut.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | attribut | java.lang.String[] | Listan över tillåtna attribut. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter by document attribute.

