---
title: "SearchDocumentFilter"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Contient des méthodes pour créer des filtres de documents de recherche."
type: docs
weight: 24
url: /fr/java/com.groupdocs.search/searchdocumentfilter/
---
**Inheritance:**
java.lang.Object
```
public class SearchDocumentFilter
```

Contient des méthodes pour créer des filtres de documents de recherche.


**Learn more**

* [Document filtering in search result](../https://docs.groupdocs.com/display/searchjava/Document+filtering+in+search+result)
* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## Constructeurs

| Constructeur | Description |
| --- | --- |
| [SearchDocumentFilter()](#SearchDocumentFilter--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [createFilePathRegularExpression(String pattern)](#createFilePathRegularExpression-java.lang.String-) | Crée un filtre pour ignorer les documents qui ne correspondent pas à une expression régulière. |
|
|  | [createFilePathRegularExpression(String pattern, int options)](#createFilePathRegularExpression-java.lang.String-int-) | Crée un filtre pour ignorer les documents qui ne correspondent pas à une expression régulière. |
|
|  | [createFileExtension(String[] extensions)](#createFileExtension-java.lang.String...-) | Crée un filtre pour ignorer les documents qui ne figurent pas dans la liste spécifiée des extensions possibles. |
|
|  | [createNot(ISearchDocumentFilter innerFilter)](#createNot-com.groupdocs.search.options.ISearchDocumentFilter-) | Crée un filtre dont la logique est inverse par rapport au filtre interne spécifié. |
|
|  | [createAnd(ISearchDocumentFilter[] filters)](#createAnd-com.groupdocs.search.options.ISearchDocumentFilter...-) | Crée une conjonction logique des filtres spécifiés. |
|
|  | [createOr(ISearchDocumentFilter[] filters)](#createOr-com.groupdocs.search.options.ISearchDocumentFilter...-) | Crée une disjonction logique des filtres spécifiés. |
|
|  | [createAttribute(String[] attributes)](#createAttribute-java.lang.String...-) | Crée un filtre pour ignorer les documents qui n'ont aucune valeur dans la liste spécifiée des attributs autorisés. |
|
### SearchDocumentFilter() {#SearchDocumentFilter--}
```
public SearchDocumentFilter()
```


### createFilePathRegularExpression(String pattern) {#createFilePathRegularExpression-java.lang.String-}
```
public static ISearchDocumentFilter createFilePathRegularExpression(String pattern)
```


Crée un filtre pour ignorer les documents qui ne correspondent pas à une expression régulière. L'expression régulière est appliquée au chemin complet d'un document.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | motif | java.lang.String | Le motif de l'expression régulière. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter by file name.

### createFilePathRegularExpression(String pattern, int options) {#createFilePathRegularExpression-java.lang.String-int-}
```
public static ISearchDocumentFilter createFilePathRegularExpression(String pattern, int options)
```


Crée un filtre pour ignorer les documents qui ne correspondent pas à une expression régulière. L'expression régulière est appliquée au chemin complet d'un document.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | motif | java.lang.String | Le motif de l'expression régulière. |
|
|  | options | int | Les options de l'expression régulière. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter by file name.

### createFileExtension(String[] extensions) {#createFileExtension-java.lang.String...-}
```
public static ISearchDocumentFilter createFileExtension(String[] extensions)
```


Crée un filtre pour ignorer les documents qui ne figurent pas dans la liste spécifiée des extensions possibles.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | extensions | java.lang.String[] | La liste des extensions possibles. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter by document extension.

### createNot(ISearchDocumentFilter innerFilter) {#createNot-com.groupdocs.search.options.ISearchDocumentFilter-}
```
public static ISearchDocumentFilter createNot(ISearchDocumentFilter innerFilter)
```


Crée un filtre dont la logique est inverse par rapport au filtre interne spécifié.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | innerFilter | [ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) | Le filtre interne de document de recherche. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - An inverted search document filter.

### createAnd(ISearchDocumentFilter[] filters) {#createAnd-com.groupdocs.search.options.ISearchDocumentFilter...-}
```
public static ISearchDocumentFilter createAnd(ISearchDocumentFilter[] filters)
```


Crée une conjonction logique des filtres spécifiés.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | filters | [ISearchDocumentFilter\[\]](../../com.groupdocs.search.options/isearchdocumentfilter) | Les filtres de document de recherche. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter that represents result of conjunction of the specified filters.

### createOr(ISearchDocumentFilter[] filters) {#createOr-com.groupdocs.search.options.ISearchDocumentFilter...-}
```
public static ISearchDocumentFilter createOr(ISearchDocumentFilter[] filters)
```


Crée une disjonction logique des filtres spécifiés.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | filters | [ISearchDocumentFilter\[\]](../../com.groupdocs.search.options/isearchdocumentfilter) | Les filtres de document de recherche. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter that represents result of disjunction of the specified filters.

### createAttribute(String[] attributes) {#createAttribute-java.lang.String...-}
```
public static ISearchDocumentFilter createAttribute(String[] attributes)
```


Crée un filtre pour ignorer les documents qui n'ont aucune valeur dans la liste spécifiée des attributs autorisés.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | attributs | java.lang.String[] | La liste des attributs autorisés. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter by document attribute.

