---
title: "SearchNetworkNode"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta un nodo della rete di ricerca che può contenere servizi come estrattore, indicizzatore, ricercatore, shard."
type: docs
weight: 11
url: /it/java/com.groupdocs.search.scaling/searchnetworknode/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable
```
public class SearchNetworkNode implements Closeable
```

Rappresenta un nodo della rete di ricerca che può contenere servizi come estrattore, indicizzatore, ricercatore, shard.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings)](#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-) | Inizializza una nuova istanza della classe  SearchNetworkNode. |
|
|  | [SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger)](#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-com.groupdocs.search.common.ILogger-) | Inizializza una nuova istanza della classe  SearchNetworkNode. |
|
|  | [SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger, Configuration configuration)](#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-com.groupdocs.search.common.ILogger-com.groupdocs.search.scaling.configuring.Configuration-) | Inizializza una nuova istanza della classe  SearchNetworkNode. |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [start()](#start--) | Avvia il funzionamento del nodo della rete di ricerca. |
|
|  | [configureAllNodes()](#configureAllNodes--) | Configura tutti i nodi nella rete di ricerca. |
|
|  | [configureNode(int nodeIndex)](#configureNode-int-) | Configura il nodo specificato nella rete di ricerca. |
|
|  | [getCustomExtractors()](#getCustomExtractors--) | Ottiene la raccolta di estrattori personalizzati. |
|
|  | [setOcrConnector(IOcrConnector ocrConnector)](#setOcrConnector-com.groupdocs.search.options.IOcrConnector-) | Imposta un connettore OCR utilizzato per l'elaborazione OCR. |
|
|  | [setWordFormsProvider(IWordFormsProvider wordFormsProvider)](#setWordFormsProvider-com.groupdocs.search.dictionaries.IWordFormsProvider-) | Imposta un provider di forme di parole. |
|
|  | [close()](#close--) | Rilascia tutte le risorse utilizzate da SearchNetworkNode. |
|
|  | [getNodeIndex()](#getNodeIndex--) | Restituisce l'indice del nodo della rete di ricerca. |
|
|  | [getEvents()](#getEvents--) | Ottiene il hub degli eventi per iscriversi agli eventi. |
|
|  | [getIndexer()](#getIndexer--) | Ottiene l'indicizzatore. |
|
|  | [getSearcher()](#getSearcher--) | Ottiene il ricercatore. |
|
|  | [getShardIndices()](#getShardIndices--) | Ottiene un array di tutti gli indici di shard nella rete di ricerca. |
|
|  | [getNodeIndex(int serviceIndex)](#getNodeIndex-int-) | Ottiene l'indice del nodo in cui si trova il servizio. |
|
| [getCore()](#getCore--) |  |
### SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings) {#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-}
```
public SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings)
```


Inizializza una nuova istanza della classe  SearchNetworkNode.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | nodeIndex | int | L'indice del nodo. |
|
|  | storagePath | java.lang.String | Il percorso di archiviazione. |
|
|  | networkSettings | [INetworkSettings](../../com.groupdocs.search.scaling.configuring/inetworksettings) | Le impostazioni di rete. |
|

### SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger) {#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-com.groupdocs.search.common.ILogger-}
```
public SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger)
```


Inizializza una nuova istanza della classe  SearchNetworkNode.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | nodeIndex | int | L'indice del nodo. |
|
|  | storagePath | java.lang.String | Il percorso di archiviazione. |
|
|  | networkSettings | [INetworkSettings](../../com.groupdocs.search.scaling.configuring/inetworksettings) | Le impostazioni di rete. |
|
|  | logger | [ILogger](../../com.groupdocs.search.common/ilogger) | Il logger. |
|

### SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger, Configuration configuration) {#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-com.groupdocs.search.common.ILogger-com.groupdocs.search.scaling.configuring.Configuration-}
```
public SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger, Configuration configuration)
```


Inizializza una nuova istanza della classe  SearchNetworkNode.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | nodeIndex | int | L'indice del nodo. |
|
|  | storagePath | java.lang.String | Il percorso di archiviazione. |
|
|  | networkSettings | [INetworkSettings](../../com.groupdocs.search.scaling.configuring/inetworksettings) | Le impostazioni di rete. |
|
|  | logger | [ILogger](../../com.groupdocs.search.common/ilogger) | Il logger. |
|
|  | configuration | [Configuration](../../com.groupdocs.search.scaling.configuring/configuration) | La configurazione. |
|

### start() {#start--}
```
public void start()
```


Avvia il funzionamento del nodo della rete di ricerca.


### configureAllNodes() {#configureAllNodes--}
```
public void configureAllNodes()
```


Configura tutti i nodi nella rete di ricerca.


### configureNode(int nodeIndex) {#configureNode-int-}
```
public void configureNode(int nodeIndex)
```


Configura il nodo specificato nella rete di ricerca.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | nodeIndex | int | L'indice del nodo. |
|

### getCustomExtractors() {#getCustomExtractors--}
```
public CustomExtractorCollection getCustomExtractors()
```


Ottiene la collezione di estrattori personalizzati. L'esempio completo di implementazione di un estrattore personalizzato è presentato nella documentazione dell'interfaccia  GroupDocs.Search.Common.IFieldExtractor .


**Returns:**
[CustomExtractorCollection](../../com.groupdocs.search.common/customextractorcollection) - The custom extractor collection.

### setOcrConnector(IOcrConnector ocrConnector) {#setOcrConnector-com.groupdocs.search.options.IOcrConnector-}
```
public void setOcrConnector(IOcrConnector ocrConnector)
```


Imposta un connettore OCR utilizzato per l'elaborazione OCR.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | ocrConnector | [IOcrConnector](../../com.groupdocs.search.options/iocrconnector) | Il connettore OCR. |
|

### setWordFormsProvider(IWordFormsProvider wordFormsProvider) {#setWordFormsProvider-com.groupdocs.search.dictionaries.IWordFormsProvider-}
```
public void setWordFormsProvider(IWordFormsProvider wordFormsProvider)
```


Imposta un provider di forme di parole.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | wordFormsProvider | [IWordFormsProvider](../../com.groupdocs.search.dictionaries/iwordformsprovider) | Il provider di forme di parole. |
|

### close() {#close--}
```
public void close()
```


Rilascia tutte le risorse utilizzate da SearchNetworkNode.


### getNodeIndex() {#getNodeIndex--}
```
public int getNodeIndex()
```


Restituisce l'indice del nodo della rete di ricerca.


**Returns:**
int - L'indice del nodo della rete di ricerca.

### getEvents() {#getEvents--}
```
public NodeEventHub getEvents()
```


Ottiene il hub degli eventi per iscriversi agli eventi.


**Returns:**
[NodeEventHub](../../com.groupdocs.search.scaling.events/nodeeventhub) - The event hub for subscribing to events.

### getIndexer() {#getIndexer--}
```
public Indexer getIndexer()
```


Ottiene l'indicizzatore.


**Returns:**
[Indexer](../../com.groupdocs.search.scaling/indexer) - The indexer.

### getSearcher() {#getSearcher--}
```
public Searcher getSearcher()
```


Ottiene il ricercatore.


**Returns:**
[Searcher](../../com.groupdocs.search.scaling/searcher) - The searcher.

### getShardIndices() {#getShardIndices--}
```
public int[] getShardIndices()
```


Ottiene un array di tutti gli indici di shard nella rete di ricerca.


**Returns:**
int[] - Un array di tutti gli indici di shard nella rete di ricerca.

### getNodeIndex(int serviceIndex) {#getNodeIndex-int-}
```
public int getNodeIndex(int serviceIndex)
```


Ottiene l'indice del nodo in cui si trova il servizio.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | serviceIndex | int | L'indice del servizio. |
|

**Returns:**
int - L'indice del nodo in cui si trova il servizio. Se l'indice del servizio è errato, viene restituito -1.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
