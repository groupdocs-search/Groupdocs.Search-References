---
title: "Zoeker"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt een service voor die zoekopdrachten naar shards van het zoeknetwerk beheert."
type: docs
weight: 12
url: /nl/java/com.groupdocs.search.scaling/searcher/
---
**Inheritance:**
java.lang.Object
```
public abstract class Searcher
```

Stelt een service voor die zoekopdrachten naar shards van het zoeknetwerk beheert.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [Searcher()](#Searcher--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [searchFirst(String query, SearchOptions options)](#searchFirst-java.lang.String-com.groupdocs.search.options.SearchOptions-) | Start een zoekopdracht met een query in tekstvorm in de gedistribueerde zoekindex. |
|
|  | [searchFirst(SearchQuery query, SearchOptions options)](#searchFirst-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-) | Start een zoekopdracht in de gedistribueerde zoekindex. |
|
|  | [searchFirst(SearchImage image, ImageSearchOptions options)](#searchFirst-com.groupdocs.search.common.SearchImage-com.groupdocs.search.options.ImageSearchOptions-) | Voert een omgekeerde afbeeldingzoekopdracht uit in de gedistribueerde zoekindex. |
|
|  | [searchNext(NetworkSearchToken networkSearchToken)](#searchNext-com.groupdocs.search.scaling.results.NetworkSearchToken-) | Vervolg een zoekopdracht in de gedistribueerde zoekindex. |
|
|  | [searchNext(NetworkImageSearchToken networkImageSearchToken)](#searchNext-com.groupdocs.search.scaling.results.NetworkImageSearchToken-) | Vervolg een omgekeerde afbeeldingzoekopdracht in de gedistribueerde zoekindex. |
|
|  | [highlight(NetworkFoundDocument document, Highlighter highlighter, HighlightOptions options)](#highlight-com.groupdocs.search.scaling.results.NetworkFoundDocument-com.groupdocs.search.highlighters.Highlighter-com.groupdocs.search.options.HighlightOptions-) | Genereert HTML-geformatteerde tekst met gemarkeerde gevonden termen. |
|
|  | [getIndexedDocuments(int shardIndex)](#getIndexedDocuments-int-) | Haalt een array op van alle geïndexeerde documenten. |
|
|  | [getIndexedDocumentItems(NetworkDocumentInfo documentInfo)](#getIndexedDocumentItems-com.groupdocs.search.scaling.results.NetworkDocumentInfo-) | Haalt een array op van geneste items van het opgegeven document (voor containerdocumenten zoals ZIP, OST, PST). |
|
|  | [getDocumentText(NetworkDocumentInfo documentInfo, OutputAdapter adapter)](#getDocumentText-com.groupdocs.search.scaling.results.NetworkDocumentInfo-com.groupdocs.search.common.OutputAdapter-) | Genereert de tekst van een geïndexeerd document en geeft deze door aan een outputadapter. |
|
### Searcher() {#Searcher--}
```
public Searcher()
```


### searchFirst(String query, SearchOptions options) {#searchFirst-java.lang.String-com.groupdocs.search.options.SearchOptions-}
```
public abstract NetworkSearchResult searchFirst(String query, SearchOptions options)
```


Start een zoekopdracht met een query in tekstvorm in de gedistribueerde zoekindex.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | query | java.lang.String | De zoekopdracht. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | De zoekopties. |
|

**Returns:**
[NetworkSearchResult](../../com.groupdocs.search.scaling.results/networksearchresult) - The search result.

### searchFirst(SearchQuery query, SearchOptions options) {#searchFirst-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-}
```
public abstract NetworkSearchResult searchFirst(SearchQuery query, SearchOptions options)
```


Start een zoekopdracht in de gedistribueerde zoekindex.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | De zoekopdracht. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | De zoekopties. |
|

**Returns:**
[NetworkSearchResult](../../com.groupdocs.search.scaling.results/networksearchresult) - The search result.

### searchFirst(SearchImage image, ImageSearchOptions options) {#searchFirst-com.groupdocs.search.common.SearchImage-com.groupdocs.search.options.ImageSearchOptions-}
```
public abstract NetworkImageSearchResult searchFirst(SearchImage image, ImageSearchOptions options)
```


Voert een omgekeerde afbeeldingzoekopdracht uit in de gedistribueerde zoekindex.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | image | [SearchImage](../../com.groupdocs.search.common/searchimage) | De afbeelding om te zoeken. |
|
|  | options | [ImageSearchOptions](../../com.groupdocs.search.options/imagesearchoptions) | De zoekopties voor de afbeelding. |
|

**Returns:**
[NetworkImageSearchResult](../../com.groupdocs.search.scaling.results/networkimagesearchresult) - The reverse image search result.

### searchNext(NetworkSearchToken networkSearchToken) {#searchNext-com.groupdocs.search.scaling.results.NetworkSearchToken-}
```
public abstract NetworkSearchResult searchNext(NetworkSearchToken networkSearchToken)
```


Vervolg een zoekopdracht in de gedistribueerde zoekindex.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | networkSearchToken | [NetworkSearchToken](../../com.groupdocs.search.scaling.results/networksearchtoken) | Het netwerkszoek-token. |
|

**Returns:**
[NetworkSearchResult](../../com.groupdocs.search.scaling.results/networksearchresult) - The search result.

### searchNext(NetworkImageSearchToken networkImageSearchToken) {#searchNext-com.groupdocs.search.scaling.results.NetworkImageSearchToken-}
```
public abstract NetworkImageSearchResult searchNext(NetworkImageSearchToken networkImageSearchToken)
```


Vervolg een omgekeerde afbeeldingzoekopdracht in de gedistribueerde zoekindex.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | networkImageSearchToken | [NetworkImageSearchToken](../../com.groupdocs.search.scaling.results/networkimagesearchtoken) | Het netwerkafbeelding-zoek-token. |
|

**Returns:**
[NetworkImageSearchResult](../../com.groupdocs.search.scaling.results/networkimagesearchresult) - The reverse image search result.

### highlight(NetworkFoundDocument document, Highlighter highlighter, HighlightOptions options) {#highlight-com.groupdocs.search.scaling.results.NetworkFoundDocument-com.groupdocs.search.highlighters.Highlighter-com.groupdocs.search.options.HighlightOptions-}
```
public abstract void highlight(NetworkFoundDocument document, Highlighter highlighter, HighlightOptions options)
```


Genereert HTML-geformatteerde tekst met gemarkeerde gevonden termen.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | document | [NetworkFoundDocument](../../com.groupdocs.search.scaling.results/networkfounddocument) | Het gevonden document. |
|
|  | highlighter | [Highlighter](../../com.groupdocs.search.highlighters/highlighter) | De markeerder voor zoekresultaten. |
|
|  | options | [HighlightOptions](../../com.groupdocs.search.options/highlightoptions) | De highlight-opties. |
|

### getIndexedDocuments(int shardIndex) {#getIndexedDocuments-int-}
```
public abstract NetworkDocumentInfo[] getIndexedDocuments(int shardIndex)
```


Haalt een array op van alle geïndexeerde documenten.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | shardIndex | int | De shard-index. |
|

**Returns:**
com.groupdocs.search.scaling.results.NetworkDocumentInfo[] - Een array van alle geïndexeerde documenten.

### getIndexedDocumentItems(NetworkDocumentInfo documentInfo) {#getIndexedDocumentItems-com.groupdocs.search.scaling.results.NetworkDocumentInfo-}
```
public abstract NetworkDocumentInfo[] getIndexedDocumentItems(NetworkDocumentInfo documentInfo)
```


Haalt een array op van geneste items van het opgegeven document (voor containerdocumenten zoals ZIP, OST, PST).


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | documentInfo | [NetworkDocumentInfo](../../com.groupdocs.search.scaling.results/networkdocumentinfo) | De documentinformatie. |
|

**Returns:**
com.groupdocs.search.scaling.results.NetworkDocumentInfo[] - Een array van documentitems.

### getDocumentText(NetworkDocumentInfo documentInfo, OutputAdapter adapter) {#getDocumentText-com.groupdocs.search.scaling.results.NetworkDocumentInfo-com.groupdocs.search.common.OutputAdapter-}
```
public abstract void getDocumentText(NetworkDocumentInfo documentInfo, OutputAdapter adapter)
```


Genereert de tekst van een geïndexeerd document en geeft deze door aan een outputadapter.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | documentInfo | [NetworkDocumentInfo](../../com.groupdocs.search.scaling.results/networkdocumentinfo) | De geïndexeerde documentinfo. |
|
|  | adapter | [OutputAdapter](../../com.groupdocs.search.common/outputadapter) | De output-adapter. |
|

