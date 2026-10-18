---
title: "SearchNetworkNode"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt een zoeknetwerkknooppunt voor dat services kan bevatten zoals extractor, indexer, searcher, shard."
type: docs
weight: 11
url: /nl/java/com.groupdocs.search.scaling/searchnetworknode/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable
```
public class SearchNetworkNode implements Closeable
```

Stelt een knooppunt van het zoeknetwerk voor dat services zoals extractor, indexer, searcher, shard kan bevatten.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings)](#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-) | Initialiseert een nieuw exemplaar van de  SearchNetworkNode  klasse. |
|
|  | [SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger)](#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-com.groupdocs.search.common.ILogger-) | Initialiseert een nieuw exemplaar van de  SearchNetworkNode  klasse. |
|
|  | [SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger, Configuration configuration)](#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-com.groupdocs.search.common.ILogger-com.groupdocs.search.scaling.configuring.Configuration-) | Initialiseert een nieuw exemplaar van de  SearchNetworkNode  klasse. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [start()](#start--) | Start de werking van het zoeknetwerkknooppunt. |
|
|  | [configureAllNodes()](#configureAllNodes--) | Configureert alle knooppunten in het zoeknetwerk. |
|
|  | [configureNode(int nodeIndex)](#configureNode-int-) | Configureert de opgegeven knoop in het zoeknetwerk. |
|
|  | [getCustomExtractors()](#getCustomExtractors--) | Haalt de aangepaste extractorcollectie op. |
|
|  | [setOcrConnector(IOcrConnector ocrConnector)](#setOcrConnector-com.groupdocs.search.options.IOcrConnector-) | Stelt een OCR-connector in die wordt gebruikt voor OCR-verwerking. |
|
|  | [setWordFormsProvider(IWordFormsProvider wordFormsProvider)](#setWordFormsProvider-com.groupdocs.search.dictionaries.IWordFormsProvider-) | Stelt een provider voor woordvormen in. |
|
|  | [close()](#close--) | Vrijgeeft alle resources die door de SearchNetworkNode worden gebruikt. |
|
|  | [getNodeIndex()](#getNodeIndex--) | Haalt de index van het zoeknetwerk‑knooppunt op. |
|
|  | [getEvents()](#getEvents--) | Haalt de event-hub op voor het abonneren op gebeurtenissen. |
|
|  | [getIndexer()](#getIndexer--) | Haalt de indexer op. |
|
|  | [getSearcher()](#getSearcher--) | Haalt de zoeker op. |
|
|  | [getShardIndices()](#getShardIndices--) | Haalt een array van alle shard-indexen in het zoeknetwerk op. |
|
|  | [getNodeIndex(int serviceIndex)](#getNodeIndex-int-) | Haalt de index op van de node waar de service zich bevindt. |
|
| [getCore()](#getCore--) |  |
### SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings) {#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-}
```
public SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings)
```


Initialiseert een nieuw exemplaar van de  SearchNetworkNode  klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | nodeIndex | int | De knooppuntindex. |
|
|  | storagePath | java.lang.String | Het opslagpad. |
|
|  | networkSettings | [INetworkSettings](../../com.groupdocs.search.scaling.configuring/inetworksettings) | De netwerkinstellingen. |
|

### SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger) {#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-com.groupdocs.search.common.ILogger-}
```
public SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger)
```


Initialiseert een nieuw exemplaar van de  SearchNetworkNode  klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | nodeIndex | int | De knooppuntindex. |
|
|  | storagePath | java.lang.String | Het opslagpad. |
|
|  | networkSettings | [INetworkSettings](../../com.groupdocs.search.scaling.configuring/inetworksettings) | De netwerkinstellingen. |
|
|  | logger | [ILogger](../../com.groupdocs.search.common/ilogger) | De logger. |
|

### SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger, Configuration configuration) {#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-com.groupdocs.search.common.ILogger-com.groupdocs.search.scaling.configuring.Configuration-}
```
public SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger, Configuration configuration)
```


Initialiseert een nieuw exemplaar van de  SearchNetworkNode  klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | nodeIndex | int | De knooppuntindex. |
|
|  | storagePath | java.lang.String | Het opslagpad. |
|
|  | networkSettings | [INetworkSettings](../../com.groupdocs.search.scaling.configuring/inetworksettings) | De netwerkinstellingen. |
|
|  | logger | [ILogger](../../com.groupdocs.search.common/ilogger) | De logger. |
|
|  | configuration | [Configuration](../../com.groupdocs.search.scaling.configuring/configuration) | De configuratie. |
|

### start() {#start--}
```
public void start()
```


Start de werking van het zoeknetwerkknooppunt.


### configureAllNodes() {#configureAllNodes--}
```
public void configureAllNodes()
```


Configureert alle knooppunten in het zoeknetwerk.


### configureNode(int nodeIndex) {#configureNode-int-}
```
public void configureNode(int nodeIndex)
```


Configureert de opgegeven knoop in het zoeknetwerk.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | nodeIndex | int | De knooppuntindex. |
|

### getCustomExtractors() {#getCustomExtractors--}
```
public CustomExtractorCollection getCustomExtractors()
```


Haalt de collectie van aangepaste extractors op. Het volledige voorbeeld van het implementeren van een aangepaste extractor wordt gepresenteerd in de documentatie voor de  GroupDocs.Search.Common.IFieldExtractor  interface.


**Returns:**
[CustomExtractorCollection](../../com.groupdocs.search.common/customextractorcollection) - The custom extractor collection.

### setOcrConnector(IOcrConnector ocrConnector) {#setOcrConnector-com.groupdocs.search.options.IOcrConnector-}
```
public void setOcrConnector(IOcrConnector ocrConnector)
```


Stelt een OCR-connector in die wordt gebruikt voor OCR-verwerking.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | ocrConnector | [IOcrConnector](../../com.groupdocs.search.options/iocrconnector) | De OCR-connector. |
|

### setWordFormsProvider(IWordFormsProvider wordFormsProvider) {#setWordFormsProvider-com.groupdocs.search.dictionaries.IWordFormsProvider-}
```
public void setWordFormsProvider(IWordFormsProvider wordFormsProvider)
```


Stelt een provider voor woordvormen in.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | wordFormsProvider | [IWordFormsProvider](../../com.groupdocs.search.dictionaries/iwordformsprovider) | De provider van woordvormen. |
|

### close() {#close--}
```
public void close()
```


Vrijgeeft alle resources die door de SearchNetworkNode worden gebruikt.


### getNodeIndex() {#getNodeIndex--}
```
public int getNodeIndex()
```


Haalt de index van het zoeknetwerk‑knooppunt op.


**Returns:**
int - De index van het zoeknetwerk‑knooppunt.

### getEvents() {#getEvents--}
```
public NodeEventHub getEvents()
```


Haalt de event-hub op voor het abonneren op gebeurtenissen.


**Returns:**
[NodeEventHub](../../com.groupdocs.search.scaling.events/nodeeventhub) - The event hub for subscribing to events.

### getIndexer() {#getIndexer--}
```
public Indexer getIndexer()
```


Haalt de indexer op.


**Returns:**
[Indexer](../../com.groupdocs.search.scaling/indexer) - The indexer.

### getSearcher() {#getSearcher--}
```
public Searcher getSearcher()
```


Haalt de zoeker op.


**Returns:**
[Searcher](../../com.groupdocs.search.scaling/searcher) - The searcher.

### getShardIndices() {#getShardIndices--}
```
public int[] getShardIndices()
```


Haalt een array van alle shard-indexen in het zoeknetwerk op.


**Returns:**
int[] - Een array van alle shard-indexen in het zoeknetwerk.

### getNodeIndex(int serviceIndex) {#getNodeIndex-int-}
```
public int getNodeIndex(int serviceIndex)
```


Haalt de index op van de node waar de service zich bevindt.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | serviceIndex | int | De service-index. |
|

**Returns:**
int - De index van de node waar de service zich bevindt. Als de service-index onjuist is, wordt -1 geretourneerd.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
