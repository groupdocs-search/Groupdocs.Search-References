---
title: NodeConfigurator
second_title: GroupDocs.Search for Java API Reference
description: Represents the search network node configurator.
type: docs
weight: 12
url: /java/com.groupdocs.search.scaling.configuring/nodeconfigurator/
---
**Inheritance:**
java.lang.Object
```
public abstract class NodeConfigurator
```

Represents the search network node configurator.
## Constructors

| Constructor | Description |
| --- | --- |
| [NodeConfigurator()](#NodeConfigurator--) |  |
## Methods

| Method | Description |
| --- | --- |
| [setTcpEndpoint(String hostNameOrAddress, int port)](#setTcpEndpoint-java.lang.String-int-) | Sets the TCP endpoint. |
| [addLogSink()](#addLogSink--) | Adds a log sink to the search network node. |
| [addSearcher(String storagePath)](#addSearcher-java.lang.String-) | Adds a searcher service to the search network node. |
| [addIndexer(String storagePath)](#addIndexer-java.lang.String-) | Adds an indexer service to the search network node. |
| [addExtractor(String storagePath)](#addExtractor-java.lang.String-) | Adds an extractor service to the search network node. |
| [addShard(String storagePath)](#addShard-java.lang.String-) | Adds a shard service to the search network node. |
| [completeNode()](#completeNode--) | Completes the configuration of the search network node. |
### NodeConfigurator() {#NodeConfigurator--}
```
public NodeConfigurator()
```


### setTcpEndpoint(String hostNameOrAddress, int port) {#setTcpEndpoint-java.lang.String-int-}
```
public abstract NodeConfigurator setTcpEndpoint(String hostNameOrAddress, int port)
```


Sets the TCP endpoint.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| hostNameOrAddress | java.lang.String | The host name or address. |
| port | int | The port number. |

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.
### addLogSink() {#addLogSink--}
```
public abstract NodeConfigurator addLogSink()
```


Adds a log sink to the search network node.

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.
### addSearcher(String storagePath) {#addSearcher-java.lang.String-}
```
public abstract NodeConfigurator addSearcher(String storagePath)
```


Adds a searcher service to the search network node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| storagePath | java.lang.String | The storage path of the adding service. |

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.
### addIndexer(String storagePath) {#addIndexer-java.lang.String-}
```
public abstract NodeConfigurator addIndexer(String storagePath)
```


Adds an indexer service to the search network node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| storagePath | java.lang.String | The storage path of the adding service. |

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.
### addExtractor(String storagePath) {#addExtractor-java.lang.String-}
```
public abstract NodeConfigurator addExtractor(String storagePath)
```


Adds an extractor service to the search network node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| storagePath | java.lang.String | The storage path of the adding service. |

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.
### addShard(String storagePath) {#addShard-java.lang.String-}
```
public abstract NodeConfigurator addShard(String storagePath)
```


Adds a shard service to the search network node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| storagePath | java.lang.String | The storage path of the adding service. |

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.
### completeNode() {#completeNode--}
```
public abstract Configurator completeNode()
```


Completes the configuration of the search network node.

**Returns:**
[Configurator](../../com.groupdocs.search.scaling.configuring/configurator) - The configurator.
