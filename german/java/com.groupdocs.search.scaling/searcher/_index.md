---
title: "Searcher"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt einen Dienst dar, der Suchanfragen an Shards des Suchnetzwerks verwaltet."
type: docs
weight: 12
url: /de/java/com.groupdocs.search.scaling/searcher/
---
**Inheritance:**
java.lang.Object
```
public abstract class Searcher
```

Stellt einen Dienst dar, der Suchanfragen an Shards des Suchnetzwerks verwaltet.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [Searcher()](#Searcher--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [searchFirst(String query, SearchOptions options)](#searchFirst-java.lang.String-com.groupdocs.search.options.SearchOptions-) | Startet eine Suche mit einer Abfrage in Textform im verteilten Suchindex. |
|
|  | [searchFirst(SearchQuery query, SearchOptions options)](#searchFirst-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-) | Startet eine Suche im verteilten Suchindex. |
|
|  | [searchFirst(SearchImage image, ImageSearchOptions options)](#searchFirst-com.groupdocs.search.common.SearchImage-com.groupdocs.search.options.ImageSearchOptions-) | Führt eine umgekehrte Bildsuche im verteilten Suchindex durch. |
|
|  | [searchNext(NetworkSearchToken networkSearchToken)](#searchNext-com.groupdocs.search.scaling.results.NetworkSearchToken-) | Setzt eine Suche im verteilten Suchindex fort. |
|
|  | [searchNext(NetworkImageSearchToken networkImageSearchToken)](#searchNext-com.groupdocs.search.scaling.results.NetworkImageSearchToken-) | Setzt eine umgekehrte Bildsuche im verteilten Suchindex fort. |
|
|  | [highlight(NetworkFoundDocument document, Highlighter highlighter, HighlightOptions options)](#highlight-com.groupdocs.search.scaling.results.NetworkFoundDocument-com.groupdocs.search.highlighters.Highlighter-com.groupdocs.search.options.HighlightOptions-) | Erzeugt HTML-formatierten Text mit hervorgehobenen gefundenen Begriffen. |
|
|  | [getIndexedDocuments(int shardIndex)](#getIndexedDocuments-int-) | Ruft ein Array aller indizierten Dokumente ab. |
|
|  | [getIndexedDocumentItems(NetworkDocumentInfo documentInfo)](#getIndexedDocumentItems-com.groupdocs.search.scaling.results.NetworkDocumentInfo-) | Liefert ein Array verschachtelter Elemente des angegebenen Dokuments (für Containerdokumente wie ZIP, OST, PST). |
|
|  | [getDocumentText(NetworkDocumentInfo documentInfo, OutputAdapter adapter)](#getDocumentText-com.groupdocs.search.scaling.results.NetworkDocumentInfo-com.groupdocs.search.common.OutputAdapter-) | Erzeugt den Text eines indizierten Dokuments und leitet ihn über einen Ausgabeadapter weiter. |
|
### Searcher() {#Searcher--}
```
public Searcher()
```


### searchFirst(String query, SearchOptions options) {#searchFirst-java.lang.String-com.groupdocs.search.options.SearchOptions-}
```
public abstract NetworkSearchResult searchFirst(String query, SearchOptions options)
```


Startet eine Suche mit einer Abfrage in Textform im verteilten Suchindex.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | query | java.lang.String | Die Suchanfrage. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | Die Suchoptionen. |
|

**Returns:**
[NetworkSearchResult](../../com.groupdocs.search.scaling.results/networksearchresult) - The search result.

### searchFirst(SearchQuery query, SearchOptions options) {#searchFirst-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-}
```
public abstract NetworkSearchResult searchFirst(SearchQuery query, SearchOptions options)
```


Startet eine Suche im verteilten Suchindex.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | Die Suchanfrage. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | Die Suchoptionen. |
|

**Returns:**
[NetworkSearchResult](../../com.groupdocs.search.scaling.results/networksearchresult) - The search result.

### searchFirst(SearchImage image, ImageSearchOptions options) {#searchFirst-com.groupdocs.search.common.SearchImage-com.groupdocs.search.options.ImageSearchOptions-}
```
public abstract NetworkImageSearchResult searchFirst(SearchImage image, ImageSearchOptions options)
```


Führt eine umgekehrte Bildsuche im verteilten Suchindex durch.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | image | [SearchImage](../../com.groupdocs.search.common/searchimage) | Das Bild zum Durchsuchen. |
|
|  | options | [ImageSearchOptions](../../com.groupdocs.search.options/imagesearchoptions) | Die Bildsuchoptionen. |
|

**Returns:**
[NetworkImageSearchResult](../../com.groupdocs.search.scaling.results/networkimagesearchresult) - The reverse image search result.

### searchNext(NetworkSearchToken networkSearchToken) {#searchNext-com.groupdocs.search.scaling.results.NetworkSearchToken-}
```
public abstract NetworkSearchResult searchNext(NetworkSearchToken networkSearchToken)
```


Setzt eine Suche im verteilten Suchindex fort.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | networkSearchToken | [NetworkSearchToken](../../com.groupdocs.search.scaling.results/networksearchtoken) | Das Netzwerk-Such-Token. |
|

**Returns:**
[NetworkSearchResult](../../com.groupdocs.search.scaling.results/networksearchresult) - The search result.

### searchNext(NetworkImageSearchToken networkImageSearchToken) {#searchNext-com.groupdocs.search.scaling.results.NetworkImageSearchToken-}
```
public abstract NetworkImageSearchResult searchNext(NetworkImageSearchToken networkImageSearchToken)
```


Setzt eine umgekehrte Bildsuche im verteilten Suchindex fort.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | networkImageSearchToken | [NetworkImageSearchToken](../../com.groupdocs.search.scaling.results/networkimagesearchtoken) | Das Netzwerk‑Bild‑Such‑Token. |
|

**Returns:**
[NetworkImageSearchResult](../../com.groupdocs.search.scaling.results/networkimagesearchresult) - The reverse image search result.

### highlight(NetworkFoundDocument document, Highlighter highlighter, HighlightOptions options) {#highlight-com.groupdocs.search.scaling.results.NetworkFoundDocument-com.groupdocs.search.highlighters.Highlighter-com.groupdocs.search.options.HighlightOptions-}
```
public abstract void highlight(NetworkFoundDocument document, Highlighter highlighter, HighlightOptions options)
```


Erzeugt HTML-formatierten Text mit hervorgehobenen gefundenen Begriffen.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | document | [NetworkFoundDocument](../../com.groupdocs.search.scaling.results/networkfounddocument) | Das gefundene Dokument. |
|
|  | highlighter | [Highlighter](../../com.groupdocs.search.highlighters/highlighter) | Der Hervorheber für Suchergebnisse. |
|
|  | options | [HighlightOptions](../../com.groupdocs.search.options/highlightoptions) | Die Hervorhebungsoptionen. |
|

### getIndexedDocuments(int shardIndex) {#getIndexedDocuments-int-}
```
public abstract NetworkDocumentInfo[] getIndexedDocuments(int shardIndex)
```


Ruft ein Array aller indizierten Dokumente ab.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | shardIndex | int | Der Shard-Index. |
|

**Returns:**
com.groupdocs.search.scaling.results.NetworkDocumentInfo[] - Ein Array aller indizierten Dokumente.

### getIndexedDocumentItems(NetworkDocumentInfo documentInfo) {#getIndexedDocumentItems-com.groupdocs.search.scaling.results.NetworkDocumentInfo-}
```
public abstract NetworkDocumentInfo[] getIndexedDocumentItems(NetworkDocumentInfo documentInfo)
```


Liefert ein Array verschachtelter Elemente des angegebenen Dokuments (für Containerdokumente wie ZIP, OST, PST).


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | documentInfo | [NetworkDocumentInfo](../../com.groupdocs.search.scaling.results/networkdocumentinfo) | Die Dokumentinfo. |
|

**Returns:**
com.groupdocs.search.scaling.results.NetworkDocumentInfo[] - Ein Array von Dokumentelementen.

### getDocumentText(NetworkDocumentInfo documentInfo, OutputAdapter adapter) {#getDocumentText-com.groupdocs.search.scaling.results.NetworkDocumentInfo-com.groupdocs.search.common.OutputAdapter-}
```
public abstract void getDocumentText(NetworkDocumentInfo documentInfo, OutputAdapter adapter)
```


Erzeugt den Text eines indizierten Dokuments und leitet ihn über einen Ausgabeadapter weiter.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | documentInfo | [NetworkDocumentInfo](../../com.groupdocs.search.scaling.results/networkdocumentinfo) | Die indizierte Dokumentinformation. |
|
|  | adapter | [OutputAdapter](../../com.groupdocs.search.common/outputadapter) | Der Ausgabeadapter. |
|

