---
title: "SearchNetworkNode"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt einen Suchnetzwerkknoten dar, der Dienste wie Extraktor, Indexer, Searcher und Shard enthalten kann."
type: docs
weight: 11
url: /de/java/com.groupdocs.search.scaling/searchnetworknode/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable
```
public class SearchNetworkNode implements Closeable
```

Stellt einen Knoten des Suchnetzwerks dar, der Dienste wie extractor, indexer, searcher, shard enthalten kann.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings)](#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-) | Initialisiert eine neue Instanz der  SearchNetworkNode  Klasse. |
|
|  | [SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger)](#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-com.groupdocs.search.common.ILogger-) | Initialisiert eine neue Instanz der  SearchNetworkNode  Klasse. |
|
|  | [SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger, Configuration configuration)](#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-com.groupdocs.search.common.ILogger-com.groupdocs.search.scaling.configuring.Configuration-) | Initialisiert eine neue Instanz der  SearchNetworkNode  Klasse. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [start()](#start--) | Startet die Funktionsweise des Suchnetzwerkknotens. |
|
|  | [configureAllNodes()](#configureAllNodes--) | Konfiguriert alle Knoten im Suchnetzwerk. |
|
|  | [configureNode(int nodeIndex)](#configureNode-int-) | Konfiguriert den angegebenen Knoten im Suchnetzwerk. |
|
|  | [getCustomExtractors()](#getCustomExtractors--) | Liefert die benutzerdefinierte Extraktorsammlung. |
|
|  | [setOcrConnector(IOcrConnector ocrConnector)](#setOcrConnector-com.groupdocs.search.options.IOcrConnector-) | Legt einen OCR‑Connector fest, der für die OCR‑Verarbeitung verwendet wird. |
|
|  | [setWordFormsProvider(IWordFormsProvider wordFormsProvider)](#setWordFormsProvider-com.groupdocs.search.dictionaries.IWordFormsProvider-) | Setzt einen Wortformen‑Provider. |
|
|  | [close()](#close--) | Gibt alle vom SearchNetworkNode verwendeten Ressourcen frei. |
|
|  | [getNodeIndex()](#getNodeIndex--) | Ermittelt den Index des Suchnetzwerk-Knotens. |
|
|  | [getEvents()](#getEvents--) | Ermittelt den Ereignis‑Hub zum Abonnieren von Ereignissen. |
|
|  | [getIndexer()](#getIndexer--) | Liefert den Indexer. |
|
|  | [getSearcher()](#getSearcher--) | Liefert den Sucher. |
|
|  | [getShardIndices()](#getShardIndices--) | Liefert ein Array aller Shard-Indizes im Suchnetzwerk. |
|
|  | [getNodeIndex(int serviceIndex)](#getNodeIndex-int-) | Liefert den Index des Knotens, an dem der Dienst befindet. |
|
| [getCore()](#getCore--) |  |
### SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings) {#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-}
```
public SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings)
```


Initialisiert eine neue Instanz der  SearchNetworkNode  Klasse.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | nodeIndex | int | Der Knotenindex. |
|
|  | storagePath | java.lang.String | Der Speicherpfad. |
|
|  | networkSettings | [INetworkSettings](../../com.groupdocs.search.scaling.configuring/inetworksettings) | Die Netzwerkeinstellungen. |
|

### SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger) {#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-com.groupdocs.search.common.ILogger-}
```
public SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger)
```


Initialisiert eine neue Instanz der  SearchNetworkNode  Klasse.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | nodeIndex | int | Der Knotenindex. |
|
|  | storagePath | java.lang.String | Der Speicherpfad. |
|
|  | networkSettings | [INetworkSettings](../../com.groupdocs.search.scaling.configuring/inetworksettings) | Die Netzwerkeinstellungen. |
|
|  | logger | [ILogger](../../com.groupdocs.search.common/ilogger) | Der Logger. |
|

### SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger, Configuration configuration) {#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-com.groupdocs.search.common.ILogger-com.groupdocs.search.scaling.configuring.Configuration-}
```
public SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger, Configuration configuration)
```


Initialisiert eine neue Instanz der  SearchNetworkNode  Klasse.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | nodeIndex | int | Der Knotenindex. |
|
|  | storagePath | java.lang.String | Der Speicherpfad. |
|
|  | networkSettings | [INetworkSettings](../../com.groupdocs.search.scaling.configuring/inetworksettings) | Die Netzwerkeinstellungen. |
|
|  | logger | [ILogger](../../com.groupdocs.search.common/ilogger) | Der Logger. |
|
|  | configuration | [Configuration](../../com.groupdocs.search.scaling.configuring/configuration) | Die Konfiguration. |
|

### start() {#start--}
```
public void start()
```


Startet die Funktionsweise des Suchnetzwerkknotens.


### configureAllNodes() {#configureAllNodes--}
```
public void configureAllNodes()
```


Konfiguriert alle Knoten im Suchnetzwerk.


### configureNode(int nodeIndex) {#configureNode-int-}
```
public void configureNode(int nodeIndex)
```


Konfiguriert den angegebenen Knoten im Suchnetzwerk.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | nodeIndex | int | Der Knotenindex. |
|

### getCustomExtractors() {#getCustomExtractors--}
```
public CustomExtractorCollection getCustomExtractors()
```


Ruft die Sammlung benutzerdefinierter Extraktoren ab. Das vollständige Beispiel für die Implementierung eines benutzerdefinierten Extraktors wird in der Dokumentation für die  GroupDocs.Search.Common.IFieldExtractor  Schnittstelle vorgestellt.


**Returns:**
[CustomExtractorCollection](../../com.groupdocs.search.common/customextractorcollection) - The custom extractor collection.

### setOcrConnector(IOcrConnector ocrConnector) {#setOcrConnector-com.groupdocs.search.options.IOcrConnector-}
```
public void setOcrConnector(IOcrConnector ocrConnector)
```


Legt einen OCR‑Connector fest, der für die OCR‑Verarbeitung verwendet wird.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | ocrConnector | [IOcrConnector](../../com.groupdocs.search.options/iocrconnector) | Der OCR-Connector. |
|

### setWordFormsProvider(IWordFormsProvider wordFormsProvider) {#setWordFormsProvider-com.groupdocs.search.dictionaries.IWordFormsProvider-}
```
public void setWordFormsProvider(IWordFormsProvider wordFormsProvider)
```


Setzt einen Wortformen‑Provider.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | wordFormsProvider | [IWordFormsProvider](../../com.groupdocs.search.dictionaries/iwordformsprovider) | Der Wortformen-Provider. |
|

### close() {#close--}
```
public void close()
```


Gibt alle vom SearchNetworkNode verwendeten Ressourcen frei.


### getNodeIndex() {#getNodeIndex--}
```
public int getNodeIndex()
```


Ermittelt den Index des Suchnetzwerk-Knotens.


**Returns:**
int - Der Index des Suchnetzwerk-Knotens.

### getEvents() {#getEvents--}
```
public NodeEventHub getEvents()
```


Ermittelt den Ereignis‑Hub zum Abonnieren von Ereignissen.


**Returns:**
[NodeEventHub](../../com.groupdocs.search.scaling.events/nodeeventhub) - The event hub for subscribing to events.

### getIndexer() {#getIndexer--}
```
public Indexer getIndexer()
```


Liefert den Indexer.


**Returns:**
[Indexer](../../com.groupdocs.search.scaling/indexer) - The indexer.

### getSearcher() {#getSearcher--}
```
public Searcher getSearcher()
```


Liefert den Sucher.


**Returns:**
[Searcher](../../com.groupdocs.search.scaling/searcher) - The searcher.

### getShardIndices() {#getShardIndices--}
```
public int[] getShardIndices()
```


Liefert ein Array aller Shard-Indizes im Suchnetzwerk.


**Returns:**
int[] - Ein Array aller Shard-Indizes im Suchnetzwerk.

### getNodeIndex(int serviceIndex) {#getNodeIndex-int-}
```
public int getNodeIndex(int serviceIndex)
```


Liefert den Index des Knotens, an dem der Dienst befindet.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | serviceIndex | int | Der Dienstindex. |
|

**Returns:**
int - Der Index des Knotens, an dem der Dienst befindet. Wenn der Dienstindex inkorrekt ist, wird -1 zurückgegeben.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
