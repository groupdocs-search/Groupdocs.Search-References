---
title: "ImageSearchOptions"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Fournit des options pour l'opération de recherche d'images inversée."
type: docs
weight: 24
url: /fr/java/com.groupdocs.search.options/imagesearchoptions/
---
**Inheritance:**
java.lang.Object
```
public class ImageSearchOptions
```

Fournit des options pour l'opération de recherche d'images inversée.

## Constructeurs

| Constructeur | Description |
| --- | --- |
|  | [ImageSearchOptions()](#ImageSearchOptions--) | Initialise une nouvelle instance de la classe  ImageSearchOptions  . |
|
|  | [ImageSearchOptions(Object data)](#ImageSearchOptions-java.lang.Object-) | Initialise une nouvelle instance de la classe  ImageSearchOptions  . |
|
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getHashDifferences()](#getHashDifferences--) | Obtient le nombre maximal de bits non correspondants dans le hachage d'image. |
|
|  | [setHashDifferences(int value)](#setHashDifferences-int-) | Définit le nombre maximal de bits non correspondants dans le hachage d'image. |
|
|  | [getMaxResultCount()](#getMaxResultCount--) | Obtient le nombre maximal d'images trouvées pour une requête de recherche d'image inversée. |
|
|  | [setMaxResultCount(int value)](#setMaxResultCount-int-) | Définit le nombre maximal d'images trouvées pour une requête de recherche d'image inversée. |
|
|  | [getSearchDocumentFilter()](#getSearchDocumentFilter--) | Obtient le filtre de document de recherche. |
|
|  | [setSearchDocumentFilter(ISearchDocumentFilter value)](#setSearchDocumentFilter-com.groupdocs.search.options.ISearchDocumentFilter-) | Obtient ou définit le filtre de document de recherche. |
|
| [getCore()](#getCore--) |  |
### ImageSearchOptions() {#ImageSearchOptions--}
```
public ImageSearchOptions()
```


Initialise une nouvelle instance de la classe  ImageSearchOptions  .


### ImageSearchOptions(Object data) {#ImageSearchOptions-java.lang.Object-}
```
public ImageSearchOptions(Object data)
```


Initialise une nouvelle instance de la classe  ImageSearchOptions  .


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | données | java.lang.Object | Les données sérialisées. |
|

### getHashDifferences() {#getHashDifferences--}
```
public int getHashDifferences()
```


Obtient le nombre maximal de bits non correspondants dans le hachage d'image. La valeur par défaut est  5 .


**Returns:**
int - Le nombre maximal de bits non correspondants dans le hachage d'image.

### setHashDifferences(int value) {#setHashDifferences-int-}
```
public void setHashDifferences(int value)
```


Définit le nombre maximal de bits non correspondants dans le hachage d'image. La valeur par défaut est 5.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | int | Le nombre maximal de bits non correspondants dans le hachage d'image. |
|

### getMaxResultCount() {#getMaxResultCount--}
```
public int getMaxResultCount()
```


Obtient le nombre maximal d'images trouvées pour une requête de recherche d'image inversée. La valeur par défaut est 1000.


**Returns:**
int - Le nombre maximal d'images trouvées pour une requête de recherche d'image inversée.

### setMaxResultCount(int value) {#setMaxResultCount-int-}
```
public void setMaxResultCount(int value)
```


Définit le nombre maximal d'images trouvées pour une requête de recherche d'image inversée. La valeur par défaut est 1000.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | int | Le nombre maximal d'images trouvées pour une requête de recherche d'image inversée. |
|

### getSearchDocumentFilter() {#getSearchDocumentFilter--}
```
public ISearchDocumentFilter getSearchDocumentFilter()
```


Obtient le filtre de document de recherche.  SearchDocumentFilter  fonctionne selon la logique d'inclusion. Utilisez la classe  GroupDocs.Search.Options.SearchDocumentFilter  pour créer des instances de filtre de document de recherche. La valeur par défaut est null, ce qui signifie que tous les documents trouvés seront retournés.


**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - The search document filter.

### setSearchDocumentFilter(ISearchDocumentFilter value) {#setSearchDocumentFilter-com.groupdocs.search.options.ISearchDocumentFilter-}
```
public void setSearchDocumentFilter(ISearchDocumentFilter value)
```


Obtient ou définit le filtre de document de recherche.  SearchDocumentFilter  fonctionne selon la logique d'inclusion. Utilisez la classe  GroupDocs.Search.Options.SearchDocumentFilter  pour créer des instances de filtre de document de recherche. La valeur par défaut est null, ce qui signifie que tous les documents trouvés seront retournés.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | value | [ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) | Le filtre de document de recherche. |
|

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
