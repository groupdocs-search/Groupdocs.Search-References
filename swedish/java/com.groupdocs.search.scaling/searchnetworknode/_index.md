---
title: "SearchNetworkNode"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar en söknätverksnod som kan innehålla tjänster såsom extraherare, indexerare, sökare och shard."
type: docs
weight: 11
url: /sv/java/com.groupdocs.search.scaling/searchnetworknode/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable
```
public class SearchNetworkNode implements Closeable
```

Representerar en söknätverksnod som kan innehålla tjänster såsom extractor, indexer, searcher, shard.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings)](#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-) | Initierar en ny instans av klassen  SearchNetworkNode . |
|
|  | [SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger)](#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-com.groupdocs.search.common.ILogger-) | Initierar en ny instans av klassen  SearchNetworkNode . |
|
|  | [SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger, Configuration configuration)](#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-com.groupdocs.search.common.ILogger-com.groupdocs.search.scaling.configuring.Configuration-) | Initierar en ny instans av klassen  SearchNetworkNode . |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [start()](#start--) | Startar funktionen för söknätverksnoden. |
|
|  | [configureAllNodes()](#configureAllNodes--) | Konfigurerar alla noder i söknätverket. |
|
|  | [configureNode(int nodeIndex)](#configureNode-int-) | Konfigurerar den angivna noden i söknätverket. |
|
|  | [getCustomExtractors()](#getCustomExtractors--) | Hämtar den anpassade extrahörssamlingen. |
|
|  | [setOcrConnector(IOcrConnector ocrConnector)](#setOcrConnector-com.groupdocs.search.options.IOcrConnector-) | Ställer in en OCR‑anslutning som används för OCR‑behandling. |
|
|  | [setWordFormsProvider(IWordFormsProvider wordFormsProvider)](#setWordFormsProvider-com.groupdocs.search.dictionaries.IWordFormsProvider-) | Ställer in en leverantör av ordformer. |
|
|  | [close()](#close--) | Frigör alla resurser som används av SearchNetworkNode. |
|
|  | [getNodeIndex()](#getNodeIndex--) | Hämtar index för söknätsnod. |
|
|  | [getEvents()](#getEvents--) | Hämtar händelsehubben för att prenumerera på händelser. |
|
|  | [getIndexer()](#getIndexer--) | Hämtar indexeraren. |
|
|  | [getSearcher()](#getSearcher--) | Hämtar sökaren. |
|
|  | [getShardIndices()](#getShardIndices--) | Hämtar en array med alla shard-index i söknätverket. |
|
|  | [getNodeIndex(int serviceIndex)](#getNodeIndex-int-) | Hämtar indexet för noden där tjänsten är placerad. |
|
| [getCore()](#getCore--) |  |
### SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings) {#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-}
```
public SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings)
```


Initierar en ny instans av klassen  SearchNetworkNode .


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | nodeIndex | int | Nodindexet. |
|
|  | storagePath | java.lang.String | Sökvägen för lagring. |
|
|  | networkSettings | [INetworkSettings](../../com.groupdocs.search.scaling.configuring/inetworksettings) | Nätverksinställningarna. |
|

### SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger) {#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-com.groupdocs.search.common.ILogger-}
```
public SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger)
```


Initierar en ny instans av klassen  SearchNetworkNode .


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | nodeIndex | int | Nodindexet. |
|
|  | storagePath | java.lang.String | Sökvägen för lagring. |
|
|  | networkSettings | [INetworkSettings](../../com.groupdocs.search.scaling.configuring/inetworksettings) | Nätverksinställningarna. |
|
|  | logger | [ILogger](../../com.groupdocs.search.common/ilogger) | Loggaren. |
|

### SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger, Configuration configuration) {#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-com.groupdocs.search.common.ILogger-com.groupdocs.search.scaling.configuring.Configuration-}
```
public SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger, Configuration configuration)
```


Initierar en ny instans av klassen  SearchNetworkNode .


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | nodeIndex | int | Nodindexet. |
|
|  | storagePath | java.lang.String | Sökvägen för lagring. |
|
|  | networkSettings | [INetworkSettings](../../com.groupdocs.search.scaling.configuring/inetworksettings) | Nätverksinställningarna. |
|
|  | logger | [ILogger](../../com.groupdocs.search.common/ilogger) | Loggaren. |
|
|  | configuration | [Configuration](../../com.groupdocs.search.scaling.configuring/configuration) | Konfigurationen. |
|

### start() {#start--}
```
public void start()
```


Startar funktionen för söknätverksnoden.


### configureAllNodes() {#configureAllNodes--}
```
public void configureAllNodes()
```


Konfigurerar alla noder i söknätverket.


### configureNode(int nodeIndex) {#configureNode-int-}
```
public void configureNode(int nodeIndex)
```


Konfigurerar den angivna noden i söknätverket.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | nodeIndex | int | Nodindexet. |
|

### getCustomExtractors() {#getCustomExtractors--}
```
public CustomExtractorCollection getCustomExtractors()
```


Hämtar samlingen av anpassade extrahörer. Det fullständiga exemplet på implementering av en anpassad extrahör presenteras i dokumentationen för gränssnittet GroupDocs.Search.Common.IFieldExtractor.


**Returns:**
[CustomExtractorCollection](../../com.groupdocs.search.common/customextractorcollection) - The custom extractor collection.

### setOcrConnector(IOcrConnector ocrConnector) {#setOcrConnector-com.groupdocs.search.options.IOcrConnector-}
```
public void setOcrConnector(IOcrConnector ocrConnector)
```


Ställer in en OCR‑anslutning som används för OCR‑behandling.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | ocrConnector | [IOcrConnector](../../com.groupdocs.search.options/iocrconnector) | OCR-anslutningen. |
|

### setWordFormsProvider(IWordFormsProvider wordFormsProvider) {#setWordFormsProvider-com.groupdocs.search.dictionaries.IWordFormsProvider-}
```
public void setWordFormsProvider(IWordFormsProvider wordFormsProvider)
```


Ställer in en leverantör av ordformer.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | wordFormsProvider | [IWordFormsProvider](../../com.groupdocs.search.dictionaries/iwordformsprovider) | Ordförformsleverantören. |
|

### close() {#close--}
```
public void close()
```


Frigör alla resurser som används av SearchNetworkNode.


### getNodeIndex() {#getNodeIndex--}
```
public int getNodeIndex()
```


Hämtar index för söknätsnod.


**Returns:**
int - Index för söknätsnod.

### getEvents() {#getEvents--}
```
public NodeEventHub getEvents()
```


Hämtar händelsehubben för att prenumerera på händelser.


**Returns:**
[NodeEventHub](../../com.groupdocs.search.scaling.events/nodeeventhub) - The event hub for subscribing to events.

### getIndexer() {#getIndexer--}
```
public Indexer getIndexer()
```


Hämtar indexeraren.


**Returns:**
[Indexer](../../com.groupdocs.search.scaling/indexer) - The indexer.

### getSearcher() {#getSearcher--}
```
public Searcher getSearcher()
```


Hämtar sökaren.


**Returns:**
[Searcher](../../com.groupdocs.search.scaling/searcher) - The searcher.

### getShardIndices() {#getShardIndices--}
```
public int[] getShardIndices()
```


Hämtar en array med alla shard-index i söknätverket.


**Returns:**
int[] - En array med alla shard-index i söknätverket.

### getNodeIndex(int serviceIndex) {#getNodeIndex-int-}
```
public int getNodeIndex(int serviceIndex)
```


Hämtar indexet för noden där tjänsten är placerad.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | serviceIndex | int | Tjänsteindexet. |
|

**Returns:**
int - Indexet för noden där tjänsten är placerad. Om tjänsteindexet är felaktigt returneras -1.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
