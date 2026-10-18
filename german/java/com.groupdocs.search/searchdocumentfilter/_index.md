---
title: "SearchDocumentFilter"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Enthält Methoden zum Erstellen von Suchdokumentfiltern."
type: docs
weight: 24
url: /de/java/com.groupdocs.search/searchdocumentfilter/
---
**Inheritance:**
java.lang.Object
```
public class SearchDocumentFilter
```

Enthält Methoden zum Erstellen von Suchdokumentfiltern.


**Learn more**

* [Document filtering in search result](../https://docs.groupdocs.com/display/searchjava/Document+filtering+in+search+result)
* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [SearchDocumentFilter()](#SearchDocumentFilter--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [createFilePathRegularExpression(String pattern)](#createFilePathRegularExpression-java.lang.String-) | Erstellt einen Filter, um Dokumente zu überspringen, die nicht einem regulären Ausdruck entsprechen. |
|
|  | [createFilePathRegularExpression(String pattern, int options)](#createFilePathRegularExpression-java.lang.String-int-) | Erstellt einen Filter, um Dokumente zu überspringen, die nicht einem regulären Ausdruck entsprechen. |
|
|  | [createFileExtension(String[] extensions)](#createFileExtension-java.lang.String...-) | Erstellt einen Filter, um Dokumente zu überspringen, die nicht in der angegebenen Liste möglicher Erweiterungen enthalten sind. |
|
|  | [createNot(ISearchDocumentFilter innerFilter)](#createNot-com.groupdocs.search.options.ISearchDocumentFilter-) | Erstellt einen Filter, der eine inverse Logik in Bezug auf den angegebenen inneren Filter hat. |
|
|  | [createAnd(ISearchDocumentFilter[] filters)](#createAnd-com.groupdocs.search.options.ISearchDocumentFilter...-) | Erstellt eine logische Konjunktion der angegebenen Filter. |
|
|  | [createOr(ISearchDocumentFilter[] filters)](#createOr-com.groupdocs.search.options.ISearchDocumentFilter...-) | Erstellt eine logische Disjunktion der angegebenen Filter. |
|
|  | [createAttribute(String[] attributes)](#createAttribute-java.lang.String...-) | Erstellt einen Filter, um Dokumente zu überspringen, die keinen Wert aus der angegebenen Liste zulässiger Attribute besitzen. |
|
### SearchDocumentFilter() {#SearchDocumentFilter--}
```
public SearchDocumentFilter()
```


### createFilePathRegularExpression(String pattern) {#createFilePathRegularExpression-java.lang.String-}
```
public static ISearchDocumentFilter createFilePathRegularExpression(String pattern)
```


Erstellt einen Filter, um Dokumente zu überspringen, die nicht einem regulären Ausdruck entsprechen. Der reguläre Ausdruck wird auf den vollständigen Pfad eines Dokuments angewendet.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | pattern | java.lang.String | Das Muster des regulären Ausdrucks. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter by file name.

### createFilePathRegularExpression(String pattern, int options) {#createFilePathRegularExpression-java.lang.String-int-}
```
public static ISearchDocumentFilter createFilePathRegularExpression(String pattern, int options)
```


Erstellt einen Filter, um Dokumente zu überspringen, die nicht einem regulären Ausdruck entsprechen. Der reguläre Ausdruck wird auf den vollständigen Pfad eines Dokuments angewendet.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | pattern | java.lang.String | Das Muster des regulären Ausdrucks. |
|
|  | options | int | Die Optionen des regulären Ausdrucks. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter by file name.

### createFileExtension(String[] extensions) {#createFileExtension-java.lang.String...-}
```
public static ISearchDocumentFilter createFileExtension(String[] extensions)
```


Erstellt einen Filter, um Dokumente zu überspringen, die nicht in der angegebenen Liste möglicher Erweiterungen enthalten sind.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | extensions | java.lang.String[] | Die Liste der möglichen Erweiterungen. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter by document extension.

### createNot(ISearchDocumentFilter innerFilter) {#createNot-com.groupdocs.search.options.ISearchDocumentFilter-}
```
public static ISearchDocumentFilter createNot(ISearchDocumentFilter innerFilter)
```


Erstellt einen Filter, der eine inverse Logik in Bezug auf den angegebenen inneren Filter hat.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | innerFilter | [ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) | Der innere Suchdokumentfilter. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - An inverted search document filter.

### createAnd(ISearchDocumentFilter[] filters) {#createAnd-com.groupdocs.search.options.ISearchDocumentFilter...-}
```
public static ISearchDocumentFilter createAnd(ISearchDocumentFilter[] filters)
```


Erstellt eine logische Konjunktion der angegebenen Filter.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | filters | [ISearchDocumentFilter\[\]](../../com.groupdocs.search.options/isearchdocumentfilter) | Die Suchdokumentfilter. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter that represents result of conjunction of the specified filters.

### createOr(ISearchDocumentFilter[] filters) {#createOr-com.groupdocs.search.options.ISearchDocumentFilter...-}
```
public static ISearchDocumentFilter createOr(ISearchDocumentFilter[] filters)
```


Erstellt eine logische Disjunktion der angegebenen Filter.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | filters | [ISearchDocumentFilter\[\]](../../com.groupdocs.search.options/isearchdocumentfilter) | Die Suchdokumentfilter. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter that represents result of disjunction of the specified filters.

### createAttribute(String[] attributes) {#createAttribute-java.lang.String...-}
```
public static ISearchDocumentFilter createAttribute(String[] attributes)
```


Erstellt einen Filter, um Dokumente zu überspringen, die keinen Wert aus der angegebenen Liste zulässiger Attribute besitzen.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Attribute | java.lang.String[] | Die Liste der zulässigen Attribute. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter by document attribute.

