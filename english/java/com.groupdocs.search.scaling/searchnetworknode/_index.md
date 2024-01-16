---
title: SearchNetworkNode
second_title: GroupDocs.Search for Java API Reference
description: Represents a search network node that can contain services such as extractor indexer searcher shard.
type: docs
weight: 11
url: /java/com.groupdocs.search.scaling/searchnetworknode/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable
```
public class SearchNetworkNode implements Closeable
```

Represents a search network node that can contain services such as extractor, indexer, searcher, shard.
## Constructors

| Constructor | Description |
| --- | --- |
| [SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings)](#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-) | Initializes a new instance of the  SearchNetworkNode  class. |
| [SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger)](#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-com.groupdocs.search.common.ILogger-) | Initializes a new instance of the  SearchNetworkNode  class. |
| [SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger, Configuration configuration)](#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-com.groupdocs.search.common.ILogger-com.groupdocs.search.scaling.configuring.Configuration-) | Initializes a new instance of the  SearchNetworkNode  class. |
## Methods

| Method | Description |
| --- | --- |
| [start()](#start--) | Starts the functioning of the search network node. |
| [configureAllNodes()](#configureAllNodes--) | Configures all nodes in the search network. |
| [configureNode(int nodeIndex)](#configureNode-int-) | Configures the specified node in the search network. |
| [getCustomExtractors()](#getCustomExtractors--) | Gets the custom extractor collection. |
| [setOcrConnector(IOcrConnector ocrConnector)](#setOcrConnector-com.groupdocs.search.options.IOcrConnector-) | Sets an OCR connector that is used for OCR processing. |
| [setWordFormsProvider(IWordFormsProvider wordFormsProvider)](#setWordFormsProvider-com.groupdocs.search.dictionaries.IWordFormsProvider-) | Sets a word forms provider. |
| [close()](#close--) | Releases all resources used by the  SearchNetworkNode . |
| [getNodeIndex()](#getNodeIndex--) | Gets the index of the search network node. |
| [getEvents()](#getEvents--) | Gets the event hub for subscribing to events. |
| [getIndexer()](#getIndexer--) | Gets the indexer. |
| [getSearcher()](#getSearcher--) | Gets the searcher. |
| [getShardIndices()](#getShardIndices--) | Gets an array of all shard indices in the search network. |
| [getNodeIndex(int serviceIndex)](#getNodeIndex-int-) | Gets the index of the node where the service is located. |
| [getCore()](#getCore--) |  |
### SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings) {#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-}
```
public SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings)
```


Initializes a new instance of the  SearchNetworkNode  class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| nodeIndex | int | The node index. |
| storagePath | java.lang.String | The storage path. |
| networkSettings | [INetworkSettings](../../com.groupdocs.search.scaling.configuring/inetworksettings) | The network settings. |

### SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger) {#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-com.groupdocs.search.common.ILogger-}
```
public SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger)
```


Initializes a new instance of the  SearchNetworkNode  class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| nodeIndex | int | The node index. |
| storagePath | java.lang.String | The storage path. |
| networkSettings | [INetworkSettings](../../com.groupdocs.search.scaling.configuring/inetworksettings) | The network settings. |
| logger | [ILogger](../../com.groupdocs.search.common/ilogger) | The logger. |

### SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger, Configuration configuration) {#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-com.groupdocs.search.common.ILogger-com.groupdocs.search.scaling.configuring.Configuration-}
```
public SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger, Configuration configuration)
```


Initializes a new instance of the  SearchNetworkNode  class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| nodeIndex | int | The node index. |
| storagePath | java.lang.String | The storage path. |
| networkSettings | [INetworkSettings](../../com.groupdocs.search.scaling.configuring/inetworksettings) | The network settings. |
| logger | [ILogger](../../com.groupdocs.search.common/ilogger) | The logger. |
| configuration | [Configuration](../../com.groupdocs.search.scaling.configuring/configuration) | The configuration. |

### start() {#start--}
```
public void start()
```


Starts the functioning of the search network node.

### configureAllNodes() {#configureAllNodes--}
```
public void configureAllNodes()
```


Configures all nodes in the search network.

### configureNode(int nodeIndex) {#configureNode-int-}
```
public void configureNode(int nodeIndex)
```


Configures the specified node in the search network.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| nodeIndex | int | The node index. |

### getCustomExtractors() {#getCustomExtractors--}
```
public CustomExtractorCollection getCustomExtractors()
```


Gets the custom extractor collection. The full example of implementing a custom extractor is presented in documentation for  GroupDocs.Search.Common.IFieldExtractor  interface.

**Returns:**
[CustomExtractorCollection](../../com.groupdocs.search.common/customextractorcollection) - The custom extractor collection.
### setOcrConnector(IOcrConnector ocrConnector) {#setOcrConnector-com.groupdocs.search.options.IOcrConnector-}
```
public void setOcrConnector(IOcrConnector ocrConnector)
```


Sets an OCR connector that is used for OCR processing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| ocrConnector | [IOcrConnector](../../com.groupdocs.search.options/iocrconnector) | The OCR connector. |

### setWordFormsProvider(IWordFormsProvider wordFormsProvider) {#setWordFormsProvider-com.groupdocs.search.dictionaries.IWordFormsProvider-}
```
public void setWordFormsProvider(IWordFormsProvider wordFormsProvider)
```


Sets a word forms provider.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| wordFormsProvider | [IWordFormsProvider](../../com.groupdocs.search.dictionaries/iwordformsprovider) | The word forms provider. |

### close() {#close--}
```
public void close()
```


Releases all resources used by the  SearchNetworkNode .

### getNodeIndex() {#getNodeIndex--}
```
public int getNodeIndex()
```


Gets the index of the search network node.

**Returns:**
int - The index of the search network node.
### getEvents() {#getEvents--}
```
public NodeEventHub getEvents()
```


Gets the event hub for subscribing to events.

**Returns:**
[NodeEventHub](../../com.groupdocs.search.scaling.events/nodeeventhub) - The event hub for subscribing to events.
### getIndexer() {#getIndexer--}
```
public Indexer getIndexer()
```


Gets the indexer.

**Returns:**
[Indexer](../../com.groupdocs.search.scaling/indexer) - The indexer.
### getSearcher() {#getSearcher--}
```
public Searcher getSearcher()
```


Gets the searcher.

**Returns:**
[Searcher](../../com.groupdocs.search.scaling/searcher) - The searcher.
### getShardIndices() {#getShardIndices--}
```
public int[] getShardIndices()
```


Gets an array of all shard indices in the search network.

**Returns:**
int[] - An array of all shard indices in the search network.
### getNodeIndex(int serviceIndex) {#getNodeIndex-int-}
```
public int getNodeIndex(int serviceIndex)
```


Gets the index of the node where the service is located.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| serviceIndex | int | The service index. |

**Returns:**
int - The index of the node where the service is located. If the service index is incorrect, when -1 is returned.
### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
