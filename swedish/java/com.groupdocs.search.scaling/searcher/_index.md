---
title: "Searcher"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar en tjänst som hanterar sökfrågor till shards i söknätverket."
type: docs
weight: 12
url: /sv/java/com.groupdocs.search.scaling/searcher/
---
**Inheritance:**
java.lang.Object
```
public abstract class Searcher
```

Representerar en tjänst som hanterar sökfrågor till shards i söknätverket.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [Searcher()](#Searcher--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [searchFirst(String query, SearchOptions options)](#searchFirst-java.lang.String-com.groupdocs.search.options.SearchOptions-) | Startar en sökning med en fråga i textform i det distribuerade sökindexet. |
|
|  | [searchFirst(SearchQuery query, SearchOptions options)](#searchFirst-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-) | Startar en sökning i det distribuerade sökindexet. |
|
|  | [searchFirst(SearchImage image, ImageSearchOptions options)](#searchFirst-com.groupdocs.search.common.SearchImage-com.groupdocs.search.options.ImageSearchOptions-) | Utför en omvänd bildsökning i det distribuerade sökindexet. |
|
|  | [searchNext(NetworkSearchToken networkSearchToken)](#searchNext-com.groupdocs.search.scaling.results.NetworkSearchToken-) | Fortsätter en sökning i det distribuerade sökindexet. |
|
|  | [searchNext(NetworkImageSearchToken networkImageSearchToken)](#searchNext-com.groupdocs.search.scaling.results.NetworkImageSearchToken-) | Fortsätter en omvänd bildsökning i det distribuerade sökindexet. |
|
|  | [highlight(NetworkFoundDocument document, Highlighter highlighter, HighlightOptions options)](#highlight-com.groupdocs.search.scaling.results.NetworkFoundDocument-com.groupdocs.search.highlighters.Highlighter-com.groupdocs.search.options.HighlightOptions-) | Genererar HTML-formaterad text med markerade hittade termer. |
|
|  | [getIndexedDocuments(int shardIndex)](#getIndexedDocuments-int-) | Hämtar en array med alla indexerade dokument. |
|
|  | [getIndexedDocumentItems(NetworkDocumentInfo documentInfo)](#getIndexedDocumentItems-com.groupdocs.search.scaling.results.NetworkDocumentInfo-) | Hämtar en array med nästlade objekt i det angivna dokumentet (för container-dokument som ZIP, OST, PST). |
|
|  | [getDocumentText(NetworkDocumentInfo documentInfo, OutputAdapter adapter)](#getDocumentText-com.groupdocs.search.scaling.results.NetworkDocumentInfo-com.groupdocs.search.common.OutputAdapter-) | Genererar texten för ett indexerat dokument och skickar den genom en utdataadapter. |
|
### Searcher() {#Searcher--}
```
public Searcher()
```


### searchFirst(String query, SearchOptions options) {#searchFirst-java.lang.String-com.groupdocs.search.options.SearchOptions-}
```
public abstract NetworkSearchResult searchFirst(String query, SearchOptions options)
```


Startar en sökning med en fråga i textform i det distribuerade sökindexet.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | query | java.lang.String | Sökfrågan. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | Sökalternativen. |
|

**Returns:**
[NetworkSearchResult](../../com.groupdocs.search.scaling.results/networksearchresult) - The search result.

### searchFirst(SearchQuery query, SearchOptions options) {#searchFirst-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-}
```
public abstract NetworkSearchResult searchFirst(SearchQuery query, SearchOptions options)
```


Startar en sökning i det distribuerade sökindexet.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | Sökfrågan. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | Sökalternativen. |
|

**Returns:**
[NetworkSearchResult](../../com.groupdocs.search.scaling.results/networksearchresult) - The search result.

### searchFirst(SearchImage image, ImageSearchOptions options) {#searchFirst-com.groupdocs.search.common.SearchImage-com.groupdocs.search.options.ImageSearchOptions-}
```
public abstract NetworkImageSearchResult searchFirst(SearchImage image, ImageSearchOptions options)
```


Utför en omvänd bildsökning i det distribuerade sökindexet.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | image | [SearchImage](../../com.groupdocs.search.common/searchimage) | Bilden att söka. |
|
|  | options | [ImageSearchOptions](../../com.groupdocs.search.options/imagesearchoptions) | Sökalternativen för bilden. |
|

**Returns:**
[NetworkImageSearchResult](../../com.groupdocs.search.scaling.results/networkimagesearchresult) - The reverse image search result.

### searchNext(NetworkSearchToken networkSearchToken) {#searchNext-com.groupdocs.search.scaling.results.NetworkSearchToken-}
```
public abstract NetworkSearchResult searchNext(NetworkSearchToken networkSearchToken)
```


Fortsätter en sökning i det distribuerade sökindexet.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | networkSearchToken | [NetworkSearchToken](../../com.groupdocs.search.scaling.results/networksearchtoken) | Nätverkssökningstoken. |
|

**Returns:**
[NetworkSearchResult](../../com.groupdocs.search.scaling.results/networksearchresult) - The search result.

### searchNext(NetworkImageSearchToken networkImageSearchToken) {#searchNext-com.groupdocs.search.scaling.results.NetworkImageSearchToken-}
```
public abstract NetworkImageSearchResult searchNext(NetworkImageSearchToken networkImageSearchToken)
```


Fortsätter en omvänd bildsökning i det distribuerade sökindexet.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | networkImageSearchToken | [NetworkImageSearchToken](../../com.groupdocs.search.scaling.results/networkimagesearchtoken) | Nätverksbildsökningstoken. |
|

**Returns:**
[NetworkImageSearchResult](../../com.groupdocs.search.scaling.results/networkimagesearchresult) - The reverse image search result.

### highlight(NetworkFoundDocument document, Highlighter highlighter, HighlightOptions options) {#highlight-com.groupdocs.search.scaling.results.NetworkFoundDocument-com.groupdocs.search.highlighters.Highlighter-com.groupdocs.search.options.HighlightOptions-}
```
public abstract void highlight(NetworkFoundDocument document, Highlighter highlighter, HighlightOptions options)
```


Genererar HTML-formaterad text med markerade hittade termer.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | document | [NetworkFoundDocument](../../com.groupdocs.search.scaling.results/networkfounddocument) | Det hittade dokumentet. |
|
|  | highlighter | [Highlighter](../../com.groupdocs.search.highlighters/highlighter) | Sökresultatets markerare. |
|
|  | options | [HighlightOptions](../../com.groupdocs.search.options/highlightoptions) | Markeringsalternativen. |
|

### getIndexedDocuments(int shardIndex) {#getIndexedDocuments-int-}
```
public abstract NetworkDocumentInfo[] getIndexedDocuments(int shardIndex)
```


Hämtar en array med alla indexerade dokument.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | shardIndex | int | Shard-indexet. |
|

**Returns:**
com.groupdocs.search.scaling.results.NetworkDocumentInfo[] - En array av alla indexerade dokument.

### getIndexedDocumentItems(NetworkDocumentInfo documentInfo) {#getIndexedDocumentItems-com.groupdocs.search.scaling.results.NetworkDocumentInfo-}
```
public abstract NetworkDocumentInfo[] getIndexedDocumentItems(NetworkDocumentInfo documentInfo)
```


Hämtar en array med nästlade objekt i det angivna dokumentet (för container-dokument som ZIP, OST, PST).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | documentInfo | [NetworkDocumentInfo](../../com.groupdocs.search.scaling.results/networkdocumentinfo) | Dokumentinformationen. |
|

**Returns:**
com.groupdocs.search.scaling.results.NetworkDocumentInfo[] - En array av dokumentobjekt.

### getDocumentText(NetworkDocumentInfo documentInfo, OutputAdapter adapter) {#getDocumentText-com.groupdocs.search.scaling.results.NetworkDocumentInfo-com.groupdocs.search.common.OutputAdapter-}
```
public abstract void getDocumentText(NetworkDocumentInfo documentInfo, OutputAdapter adapter)
```


Genererar texten för ett indexerat dokument och skickar den genom en utdataadapter.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | documentInfo | [NetworkDocumentInfo](../../com.groupdocs.search.scaling.results/networkdocumentinfo) | Den indexerade dokumentinformationen. |
|
|  | adapter | [OutputAdapter](../../com.groupdocs.search.common/outputadapter) | Utdataadaptern. |
|

