---
title: "Searcher"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta un servizio che gestisce le query di ricerca verso i shard della rete di ricerca."
type: docs
weight: 12
url: /it/java/com.groupdocs.search.scaling/searcher/
---
**Inheritance:**
java.lang.Object
```
public abstract class Searcher
```

Rappresenta un servizio che gestisce le query di ricerca verso i shard della rete di ricerca.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [Searcher()](#Searcher--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [searchFirst(String query, SearchOptions options)](#searchFirst-java.lang.String-com.groupdocs.search.options.SearchOptions-) | Avvia una ricerca con una query in forma di testo nell'indice di ricerca distribuito. |
|
|  | [searchFirst(SearchQuery query, SearchOptions options)](#searchFirst-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-) | Avvia una ricerca nell'indice di ricerca distribuito. |
|
|  | [searchFirst(SearchImage image, ImageSearchOptions options)](#searchFirst-com.groupdocs.search.common.SearchImage-com.groupdocs.search.options.ImageSearchOptions-) | Esegue una ricerca inversa di immagini nell'indice di ricerca distribuito. |
|
|  | [searchNext(NetworkSearchToken networkSearchToken)](#searchNext-com.groupdocs.search.scaling.results.NetworkSearchToken-) | Continua una ricerca nell'indice di ricerca distribuito. |
|
|  | [searchNext(NetworkImageSearchToken networkImageSearchToken)](#searchNext-com.groupdocs.search.scaling.results.NetworkImageSearchToken-) | Continua una ricerca inversa di immagini nell'indice di ricerca distribuito. |
|
|  | [highlight(NetworkFoundDocument document, Highlighter highlighter, HighlightOptions options)](#highlight-com.groupdocs.search.scaling.results.NetworkFoundDocument-com.groupdocs.search.highlighters.Highlighter-com.groupdocs.search.options.HighlightOptions-) | Genera testo formattato in HTML con i termini trovati evidenziati. |
|
|  | [getIndexedDocuments(int shardIndex)](#getIndexedDocuments-int-) | Ottiene un array di tutti i documenti indicizzati. |
|
|  | [getIndexedDocumentItems(NetworkDocumentInfo documentInfo)](#getIndexedDocumentItems-com.groupdocs.search.scaling.results.NetworkDocumentInfo-) | Ottiene un array di elementi nidificati del documento specificato (per documenti contenitore come ZIP, OST, PST). |
|
|  | [getDocumentText(NetworkDocumentInfo documentInfo, OutputAdapter adapter)](#getDocumentText-com.groupdocs.search.scaling.results.NetworkDocumentInfo-com.groupdocs.search.common.OutputAdapter-) | Genera il testo di un documento indicizzato e lo passa attraverso un adattatore di output. |
|
### Searcher() {#Searcher--}
```
public Searcher()
```


### searchFirst(String query, SearchOptions options) {#searchFirst-java.lang.String-com.groupdocs.search.options.SearchOptions-}
```
public abstract NetworkSearchResult searchFirst(String query, SearchOptions options)
```


Avvia una ricerca con una query in forma di testo nell'indice di ricerca distribuito.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | query | java.lang.String | La query di ricerca. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | Le opzioni di ricerca. |
|

**Returns:**
[NetworkSearchResult](../../com.groupdocs.search.scaling.results/networksearchresult) - The search result.

### searchFirst(SearchQuery query, SearchOptions options) {#searchFirst-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-}
```
public abstract NetworkSearchResult searchFirst(SearchQuery query, SearchOptions options)
```


Avvia una ricerca nell'indice di ricerca distribuito.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | La query di ricerca. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | Le opzioni di ricerca. |
|

**Returns:**
[NetworkSearchResult](../../com.groupdocs.search.scaling.results/networksearchresult) - The search result.

### searchFirst(SearchImage image, ImageSearchOptions options) {#searchFirst-com.groupdocs.search.common.SearchImage-com.groupdocs.search.options.ImageSearchOptions-}
```
public abstract NetworkImageSearchResult searchFirst(SearchImage image, ImageSearchOptions options)
```


Esegue una ricerca inversa di immagini nell'indice di ricerca distribuito.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | image | [SearchImage](../../com.groupdocs.search.common/searchimage) | L'immagine da cercare. |
|
|  | options | [ImageSearchOptions](../../com.groupdocs.search.options/imagesearchoptions) | Le opzioni di ricerca dell'immagine. |
|

**Returns:**
[NetworkImageSearchResult](../../com.groupdocs.search.scaling.results/networkimagesearchresult) - The reverse image search result.

### searchNext(NetworkSearchToken networkSearchToken) {#searchNext-com.groupdocs.search.scaling.results.NetworkSearchToken-}
```
public abstract NetworkSearchResult searchNext(NetworkSearchToken networkSearchToken)
```


Continua una ricerca nell'indice di ricerca distribuito.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | networkSearchToken | [NetworkSearchToken](../../com.groupdocs.search.scaling.results/networksearchtoken) | Il token di ricerca di rete. |
|

**Returns:**
[NetworkSearchResult](../../com.groupdocs.search.scaling.results/networksearchresult) - The search result.

### searchNext(NetworkImageSearchToken networkImageSearchToken) {#searchNext-com.groupdocs.search.scaling.results.NetworkImageSearchToken-}
```
public abstract NetworkImageSearchResult searchNext(NetworkImageSearchToken networkImageSearchToken)
```


Continua una ricerca inversa di immagini nell'indice di ricerca distribuito.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | networkImageSearchToken | [NetworkImageSearchToken](../../com.groupdocs.search.scaling.results/networkimagesearchtoken) | Il token di ricerca immagine di rete. |
|

**Returns:**
[NetworkImageSearchResult](../../com.groupdocs.search.scaling.results/networkimagesearchresult) - The reverse image search result.

### highlight(NetworkFoundDocument document, Highlighter highlighter, HighlightOptions options) {#highlight-com.groupdocs.search.scaling.results.NetworkFoundDocument-com.groupdocs.search.highlighters.Highlighter-com.groupdocs.search.options.HighlightOptions-}
```
public abstract void highlight(NetworkFoundDocument document, Highlighter highlighter, HighlightOptions options)
```


Genera testo formattato in HTML con i termini trovati evidenziati.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | document | [NetworkFoundDocument](../../com.groupdocs.search.scaling.results/networkfounddocument) | Il documento trovato. |
|
|  | highlighter | [Highlighter](../../com.groupdocs.search.highlighters/highlighter) | L'evidenziatore del risultato di ricerca. |
|
|  | options | [HighlightOptions](../../com.groupdocs.search.options/highlightoptions) | Le opzioni di evidenziazione. |
|

### getIndexedDocuments(int shardIndex) {#getIndexedDocuments-int-}
```
public abstract NetworkDocumentInfo[] getIndexedDocuments(int shardIndex)
```


Ottiene un array di tutti i documenti indicizzati.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | shardIndex | int | L'indice dello shard. |
|

**Returns:**
com.groupdocs.search.scaling.results.NetworkDocumentInfo[] - Un array di tutti i documenti indicizzati.

### getIndexedDocumentItems(NetworkDocumentInfo documentInfo) {#getIndexedDocumentItems-com.groupdocs.search.scaling.results.NetworkDocumentInfo-}
```
public abstract NetworkDocumentInfo[] getIndexedDocumentItems(NetworkDocumentInfo documentInfo)
```


Ottiene un array di elementi nidificati del documento specificato (per documenti contenitore come ZIP, OST, PST).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | documentInfo | [NetworkDocumentInfo](../../com.groupdocs.search.scaling.results/networkdocumentinfo) | Le informazioni del documento. |
|

**Returns:**
com.groupdocs.search.scaling.results.NetworkDocumentInfo[] - Un array di elementi di un documento.

### getDocumentText(NetworkDocumentInfo documentInfo, OutputAdapter adapter) {#getDocumentText-com.groupdocs.search.scaling.results.NetworkDocumentInfo-com.groupdocs.search.common.OutputAdapter-}
```
public abstract void getDocumentText(NetworkDocumentInfo documentInfo, OutputAdapter adapter)
```


Genera il testo di un documento indicizzato e lo passa attraverso un adattatore di output.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | documentInfo | [NetworkDocumentInfo](../../com.groupdocs.search.scaling.results/networkdocumentinfo) | Le informazioni del documento indicizzato. |
|
|  | adapter | [OutputAdapter](../../com.groupdocs.search.common/outputadapter) | L'adattatore di output. |
|

