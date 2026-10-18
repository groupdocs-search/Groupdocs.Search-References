---
title: "Searcher"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa un servicio que gestiona consultas de búsqueda a los fragmentos de la red de búsqueda."
type: docs
weight: 12
url: /es/java/com.groupdocs.search.scaling/searcher/
---
**Inheritance:**
java.lang.Object
```
public abstract class Searcher
```

Representa un servicio que gestiona consultas de búsqueda a los fragmentos de la red de búsqueda.

## Constructores

| Constructor | Descripción |
| --- | --- |
| [Searcher()](#Searcher--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
|  | [searchFirst(String query, SearchOptions options)](#searchFirst-java.lang.String-com.groupdocs.search.options.SearchOptions-) | Inicia una búsqueda con una consulta en forma de texto en el índice de búsqueda distribuido. |
|
|  | [searchFirst(SearchQuery query, SearchOptions options)](#searchFirst-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-) | Inicia una búsqueda en el índice de búsqueda distribuido. |
|
|  | [searchFirst(SearchImage image, ImageSearchOptions options)](#searchFirst-com.groupdocs.search.common.SearchImage-com.groupdocs.search.options.ImageSearchOptions-) | Realiza una búsqueda inversa de imágenes en el índice de búsqueda distribuido. |
|
|  | [searchNext(NetworkSearchToken networkSearchToken)](#searchNext-com.groupdocs.search.scaling.results.NetworkSearchToken-) | Continúa una búsqueda en el índice de búsqueda distribuido. |
|
|  | [searchNext(NetworkImageSearchToken networkImageSearchToken)](#searchNext-com.groupdocs.search.scaling.results.NetworkImageSearchToken-) | Continúa una búsqueda inversa de imágenes en el índice de búsqueda distribuido. |
|
|  | [highlight(NetworkFoundDocument document, Highlighter highlighter, HighlightOptions options)](#highlight-com.groupdocs.search.scaling.results.NetworkFoundDocument-com.groupdocs.search.highlighters.Highlighter-com.groupdocs.search.options.HighlightOptions-) | Genera texto con formato HTML con los términos encontrados resaltados. |
|
|  | [getIndexedDocuments(int shardIndex)](#getIndexedDocuments-int-) | Obtiene una matriz de todos los documentos indexados. |
|
|  | [getIndexedDocumentItems(NetworkDocumentInfo documentInfo)](#getIndexedDocumentItems-com.groupdocs.search.scaling.results.NetworkDocumentInfo-) | Obtiene una matriz de elementos anidados del documento especificado (para documentos contenedores como ZIP, OST, PST). |
|
|  | [getDocumentText(NetworkDocumentInfo documentInfo, OutputAdapter adapter)](#getDocumentText-com.groupdocs.search.scaling.results.NetworkDocumentInfo-com.groupdocs.search.common.OutputAdapter-) | Genera el texto de un documento indexado y lo pasa a través de un adaptador de salida. |
|
### Searcher() {#Searcher--}
```
public Searcher()
```


### searchFirst(String query, SearchOptions options) {#searchFirst-java.lang.String-com.groupdocs.search.options.SearchOptions-}
```
public abstract NetworkSearchResult searchFirst(String query, SearchOptions options)
```


Inicia una búsqueda con una consulta en forma de texto en el índice de búsqueda distribuido.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | query | java.lang.String | La consulta de búsqueda. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | Las opciones de búsqueda. |
|

**Returns:**
[NetworkSearchResult](../../com.groupdocs.search.scaling.results/networksearchresult) - The search result.

### searchFirst(SearchQuery query, SearchOptions options) {#searchFirst-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-}
```
public abstract NetworkSearchResult searchFirst(SearchQuery query, SearchOptions options)
```


Inicia una búsqueda en el índice de búsqueda distribuido.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | La consulta de búsqueda. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | Las opciones de búsqueda. |
|

**Returns:**
[NetworkSearchResult](../../com.groupdocs.search.scaling.results/networksearchresult) - The search result.

### searchFirst(SearchImage image, ImageSearchOptions options) {#searchFirst-com.groupdocs.search.common.SearchImage-com.groupdocs.search.options.ImageSearchOptions-}
```
public abstract NetworkImageSearchResult searchFirst(SearchImage image, ImageSearchOptions options)
```


Realiza una búsqueda inversa de imágenes en el índice de búsqueda distribuido.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | image | [SearchImage](../../com.groupdocs.search.common/searchimage) | La imagen a buscar. |
|
|  | options | [ImageSearchOptions](../../com.groupdocs.search.options/imagesearchoptions) | Las opciones de búsqueda de la imagen. |
|

**Returns:**
[NetworkImageSearchResult](../../com.groupdocs.search.scaling.results/networkimagesearchresult) - The reverse image search result.

### searchNext(NetworkSearchToken networkSearchToken) {#searchNext-com.groupdocs.search.scaling.results.NetworkSearchToken-}
```
public abstract NetworkSearchResult searchNext(NetworkSearchToken networkSearchToken)
```


Continúa una búsqueda en el índice de búsqueda distribuido.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | networkSearchToken | [NetworkSearchToken](../../com.groupdocs.search.scaling.results/networksearchtoken) | El token de búsqueda de la red. |
|

**Returns:**
[NetworkSearchResult](../../com.groupdocs.search.scaling.results/networksearchresult) - The search result.

### searchNext(NetworkImageSearchToken networkImageSearchToken) {#searchNext-com.groupdocs.search.scaling.results.NetworkImageSearchToken-}
```
public abstract NetworkImageSearchResult searchNext(NetworkImageSearchToken networkImageSearchToken)
```


Continúa una búsqueda inversa de imágenes en el índice de búsqueda distribuido.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | networkImageSearchToken | [NetworkImageSearchToken](../../com.groupdocs.search.scaling.results/networkimagesearchtoken) | El token de búsqueda de imágenes en red. |
|

**Returns:**
[NetworkImageSearchResult](../../com.groupdocs.search.scaling.results/networkimagesearchresult) - The reverse image search result.

### highlight(NetworkFoundDocument document, Highlighter highlighter, HighlightOptions options) {#highlight-com.groupdocs.search.scaling.results.NetworkFoundDocument-com.groupdocs.search.highlighters.Highlighter-com.groupdocs.search.options.HighlightOptions-}
```
public abstract void highlight(NetworkFoundDocument document, Highlighter highlighter, HighlightOptions options)
```


Genera texto con formato HTML con los términos encontrados resaltados.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | document | [NetworkFoundDocument](../../com.groupdocs.search.scaling.results/networkfounddocument) | El documento encontrado. |
|
|  | highlighter | [Highlighter](../../com.groupdocs.search.highlighters/highlighter) | El resaltador de resultados de búsqueda. |
|
|  | options | [HighlightOptions](../../com.groupdocs.search.options/highlightoptions) | Las opciones de resaltado. |
|

### getIndexedDocuments(int shardIndex) {#getIndexedDocuments-int-}
```
public abstract NetworkDocumentInfo[] getIndexedDocuments(int shardIndex)
```


Obtiene una matriz de todos los documentos indexados.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | shardIndex | int | El índice del fragmento. |
|

**Returns:**
com.groupdocs.search.scaling.results.NetworkDocumentInfo[] - Un arreglo de todos los documentos indexados.

### getIndexedDocumentItems(NetworkDocumentInfo documentInfo) {#getIndexedDocumentItems-com.groupdocs.search.scaling.results.NetworkDocumentInfo-}
```
public abstract NetworkDocumentInfo[] getIndexedDocumentItems(NetworkDocumentInfo documentInfo)
```


Obtiene una matriz de elementos anidados del documento especificado (para documentos contenedores como ZIP, OST, PST).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | documentInfo | [NetworkDocumentInfo](../../com.groupdocs.search.scaling.results/networkdocumentinfo) | La información del documento. |
|

**Returns:**
com.groupdocs.search.scaling.results.NetworkDocumentInfo[] - Un arreglo de elementos de documento.

### getDocumentText(NetworkDocumentInfo documentInfo, OutputAdapter adapter) {#getDocumentText-com.groupdocs.search.scaling.results.NetworkDocumentInfo-com.groupdocs.search.common.OutputAdapter-}
```
public abstract void getDocumentText(NetworkDocumentInfo documentInfo, OutputAdapter adapter)
```


Genera el texto de un documento indexado y lo pasa a través de un adaptador de salida.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | documentInfo | [NetworkDocumentInfo](../../com.groupdocs.search.scaling.results/networkdocumentinfo) | La información del documento indexado. |
|
|  | adapter | [OutputAdapter](../../com.groupdocs.search.common/outputadapter) | El adaptador de salida. |
|

