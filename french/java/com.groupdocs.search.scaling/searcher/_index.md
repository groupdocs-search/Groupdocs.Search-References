---
title: "Searcher"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente un service qui gère les requêtes de recherche vers les shards du réseau de recherche."
type: docs
weight: 12
url: /fr/java/com.groupdocs.search.scaling/searcher/
---
**Inheritance:**
java.lang.Object
```
public abstract class Searcher
```

Représente un service qui gère les requêtes de recherche vers les shards du réseau de recherche.

## Constructeurs

| Constructeur | Description |
| --- | --- |
| [Searcher()](#Searcher--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [searchFirst(String query, SearchOptions options)](#searchFirst-java.lang.String-com.groupdocs.search.options.SearchOptions-) | Démarre une recherche avec une requête sous forme de texte dans l'index de recherche distribué. |
|
|  | [searchFirst(SearchQuery query, SearchOptions options)](#searchFirst-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-) | Démarre une recherche dans l'index de recherche distribué. |
|
|  | [searchFirst(SearchImage image, ImageSearchOptions options)](#searchFirst-com.groupdocs.search.common.SearchImage-com.groupdocs.search.options.ImageSearchOptions-) | Effectue une recherche d'image inversée dans l'index de recherche distribué. |
|
|  | [searchNext(NetworkSearchToken networkSearchToken)](#searchNext-com.groupdocs.search.scaling.results.NetworkSearchToken-) | Poursuit une recherche dans l'index de recherche distribué. |
|
|  | [searchNext(NetworkImageSearchToken networkImageSearchToken)](#searchNext-com.groupdocs.search.scaling.results.NetworkImageSearchToken-) | Poursuit une recherche d'image inversée dans l'index de recherche distribué. |
|
|  | [highlight(NetworkFoundDocument document, Highlighter highlighter, HighlightOptions options)](#highlight-com.groupdocs.search.scaling.results.NetworkFoundDocument-com.groupdocs.search.highlighters.Highlighter-com.groupdocs.search.options.HighlightOptions-) | Génère du texte formaté en HTML avec les termes trouvés mis en évidence. |
|
|  | [getIndexedDocuments(int shardIndex)](#getIndexedDocuments-int-) | Obtient un tableau de tous les documents indexés. |
|
|  | [getIndexedDocumentItems(NetworkDocumentInfo documentInfo)](#getIndexedDocumentItems-com.groupdocs.search.scaling.results.NetworkDocumentInfo-) | Obtient un tableau des éléments imbriqués du document spécifié (pour les documents conteneurs tels que ZIP, OST, PST). |
|
|  | [getDocumentText(NetworkDocumentInfo documentInfo, OutputAdapter adapter)](#getDocumentText-com.groupdocs.search.scaling.results.NetworkDocumentInfo-com.groupdocs.search.common.OutputAdapter-) | Génère le texte d'un document indexé et le transmet via un adaptateur de sortie. |
|
### Searcher() {#Searcher--}
```
public Searcher()
```


### searchFirst(String query, SearchOptions options) {#searchFirst-java.lang.String-com.groupdocs.search.options.SearchOptions-}
```
public abstract NetworkSearchResult searchFirst(String query, SearchOptions options)
```


Démarre une recherche avec une requête sous forme de texte dans l'index de recherche distribué.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | query | java.lang.String | La requête de recherche. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | Les options de recherche. |
|

**Returns:**
[NetworkSearchResult](../../com.groupdocs.search.scaling.results/networksearchresult) - The search result.

### searchFirst(SearchQuery query, SearchOptions options) {#searchFirst-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-}
```
public abstract NetworkSearchResult searchFirst(SearchQuery query, SearchOptions options)
```


Démarre une recherche dans l'index de recherche distribué.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | La requête de recherche. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | Les options de recherche. |
|

**Returns:**
[NetworkSearchResult](../../com.groupdocs.search.scaling.results/networksearchresult) - The search result.

### searchFirst(SearchImage image, ImageSearchOptions options) {#searchFirst-com.groupdocs.search.common.SearchImage-com.groupdocs.search.options.ImageSearchOptions-}
```
public abstract NetworkImageSearchResult searchFirst(SearchImage image, ImageSearchOptions options)
```


Effectue une recherche d'image inversée dans l'index de recherche distribué.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | image | [SearchImage](../../com.groupdocs.search.common/searchimage) | L'image à rechercher. |
|
|  | options | [ImageSearchOptions](../../com.groupdocs.search.options/imagesearchoptions) | Les options de recherche d'image. |
|

**Returns:**
[NetworkImageSearchResult](../../com.groupdocs.search.scaling.results/networkimagesearchresult) - The reverse image search result.

### searchNext(NetworkSearchToken networkSearchToken) {#searchNext-com.groupdocs.search.scaling.results.NetworkSearchToken-}
```
public abstract NetworkSearchResult searchNext(NetworkSearchToken networkSearchToken)
```


Poursuit une recherche dans l'index de recherche distribué.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | networkSearchToken | [NetworkSearchToken](../../com.groupdocs.search.scaling.results/networksearchtoken) | Le jeton de recherche du réseau. |
|

**Returns:**
[NetworkSearchResult](../../com.groupdocs.search.scaling.results/networksearchresult) - The search result.

### searchNext(NetworkImageSearchToken networkImageSearchToken) {#searchNext-com.groupdocs.search.scaling.results.NetworkImageSearchToken-}
```
public abstract NetworkImageSearchResult searchNext(NetworkImageSearchToken networkImageSearchToken)
```


Poursuit une recherche d'image inversée dans l'index de recherche distribué.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | networkImageSearchToken | [NetworkImageSearchToken](../../com.groupdocs.search.scaling.results/networkimagesearchtoken) | Le jeton de recherche d'images réseau. |
|

**Returns:**
[NetworkImageSearchResult](../../com.groupdocs.search.scaling.results/networkimagesearchresult) - The reverse image search result.

### highlight(NetworkFoundDocument document, Highlighter highlighter, HighlightOptions options) {#highlight-com.groupdocs.search.scaling.results.NetworkFoundDocument-com.groupdocs.search.highlighters.Highlighter-com.groupdocs.search.options.HighlightOptions-}
```
public abstract void highlight(NetworkFoundDocument document, Highlighter highlighter, HighlightOptions options)
```


Génère du texte formaté en HTML avec les termes trouvés mis en évidence.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | document | [NetworkFoundDocument](../../com.groupdocs.search.scaling.results/networkfounddocument) | Le document trouvé. |
|
|  | highlighter | [Highlighter](../../com.groupdocs.search.highlighters/highlighter) | Le surligneur de résultats de recherche. |
|
|  | options | [HighlightOptions](../../com.groupdocs.search.options/highlightoptions) | Les options de surlignage. |
|

### getIndexedDocuments(int shardIndex) {#getIndexedDocuments-int-}
```
public abstract NetworkDocumentInfo[] getIndexedDocuments(int shardIndex)
```


Obtient un tableau de tous les documents indexés.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | shardIndex | int | L'index de partition. |
|

**Returns:**
com.groupdocs.search.scaling.results.NetworkDocumentInfo[] - Un tableau de tous les documents indexés.

### getIndexedDocumentItems(NetworkDocumentInfo documentInfo) {#getIndexedDocumentItems-com.groupdocs.search.scaling.results.NetworkDocumentInfo-}
```
public abstract NetworkDocumentInfo[] getIndexedDocumentItems(NetworkDocumentInfo documentInfo)
```


Obtient un tableau des éléments imbriqués du document spécifié (pour les documents conteneurs tels que ZIP, OST, PST).


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | documentInfo | [NetworkDocumentInfo](../../com.groupdocs.search.scaling.results/networkdocumentinfo) | Les informations du document. |
|

**Returns:**
com.groupdocs.search.scaling.results.NetworkDocumentInfo[] - Un tableau d'éléments de document.

### getDocumentText(NetworkDocumentInfo documentInfo, OutputAdapter adapter) {#getDocumentText-com.groupdocs.search.scaling.results.NetworkDocumentInfo-com.groupdocs.search.common.OutputAdapter-}
```
public abstract void getDocumentText(NetworkDocumentInfo documentInfo, OutputAdapter adapter)
```


Génère le texte d'un document indexé et le transmet via un adaptateur de sortie.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | documentInfo | [NetworkDocumentInfo](../../com.groupdocs.search.scaling.results/networkdocumentinfo) | Les informations du document indexé. |
|
|  | adapter | [OutputAdapter](../../com.groupdocs.search.common/outputadapter) | L'adaptateur de sortie. |
|

