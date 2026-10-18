---
title: "NodeConfigurator"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta il configuratore del nodo della rete di ricerca."
type: docs
weight: 13
url: /it/java/com.groupdocs.search.scaling.configuring/nodeconfigurator/
---
**Inheritance:**
java.lang.Object
```
public abstract class NodeConfigurator
```

Rappresenta il configuratore del nodo della rete di ricerca.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [NodeConfigurator()](#NodeConfigurator--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [setTcpEndpoint(String hostNameOrAddress, int port)](#setTcpEndpoint-java.lang.String-int-) | Imposta il punto finale TCP. |
|
|  | [addLogSink()](#addLogSink--) | Aggiunge un sink di log al nodo di rete di ricerca. |
|
|  | [addSearcher(String storagePath)](#addSearcher-java.lang.String-) | Aggiunge un servizio di ricerca al nodo di rete di ricerca. |
|
|  | [addIndexer(String storagePath)](#addIndexer-java.lang.String-) | Aggiunge un servizio di indicizzazione al nodo della rete di ricerca. |
|
|  | [addExtractor(String storagePath)](#addExtractor-java.lang.String-) | Aggiunge un servizio di estrazione al nodo della rete di ricerca. |
|
|  | [addShard(String storagePath)](#addShard-java.lang.String-) | Aggiunge un servizio di shard al nodo della rete di ricerca. |
|
|  | [completeNode()](#completeNode--) | Completa la configurazione del nodo della rete di ricerca. |
|
### NodeConfigurator() {#NodeConfigurator--}
```
public NodeConfigurator()
```


### setTcpEndpoint(String hostNameOrAddress, int port) {#setTcpEndpoint-java.lang.String-int-}
```
public abstract NodeConfigurator setTcpEndpoint(String hostNameOrAddress, int port)
```


Imposta il punto finale TCP.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | hostNameOrAddress | java.lang.String | Il nome host o l'indirizzo. |
|
|  | port | int | Il numero di porta. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addLogSink() {#addLogSink--}
```
public abstract NodeConfigurator addLogSink()
```


Aggiunge un sink di log al nodo di rete di ricerca.


**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addSearcher(String storagePath) {#addSearcher-java.lang.String-}
```
public abstract NodeConfigurator addSearcher(String storagePath)
```


Aggiunge un servizio di ricerca al nodo di rete di ricerca.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | storagePath | java.lang.String | Il percorso di archiviazione del servizio di aggiunta. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addIndexer(String storagePath) {#addIndexer-java.lang.String-}
```
public abstract NodeConfigurator addIndexer(String storagePath)
```


Aggiunge un servizio di indicizzazione al nodo della rete di ricerca.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | storagePath | java.lang.String | Il percorso di archiviazione del servizio di aggiunta. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addExtractor(String storagePath) {#addExtractor-java.lang.String-}
```
public abstract NodeConfigurator addExtractor(String storagePath)
```


Aggiunge un servizio di estrazione al nodo della rete di ricerca.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | storagePath | java.lang.String | Il percorso di archiviazione del servizio di aggiunta. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addShard(String storagePath) {#addShard-java.lang.String-}
```
public abstract NodeConfigurator addShard(String storagePath)
```


Aggiunge un servizio di shard al nodo della rete di ricerca.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | storagePath | java.lang.String | Il percorso di archiviazione del servizio di aggiunta. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### completeNode() {#completeNode--}
```
public abstract Configurator completeNode()
```


Completa la configurazione del nodo della rete di ricerca.


**Returns:**
[Configurator](../../com.groupdocs.search.scaling.configuring/configurator) - The configurator.

