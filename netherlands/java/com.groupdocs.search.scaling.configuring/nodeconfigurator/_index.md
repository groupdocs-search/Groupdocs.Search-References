---
title: "NodeConfigurator"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt de zoeknetwerkknooppuntconfigurator voor."
type: docs
weight: 13
url: /nl/java/com.groupdocs.search.scaling.configuring/nodeconfigurator/
---
**Inheritance:**
java.lang.Object
```
public abstract class NodeConfigurator
```

Stelt de zoeknetwerkknooppuntconfigurator voor.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [NodeConfigurator()](#NodeConfigurator--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [setTcpEndpoint(String hostNameOrAddress, int port)](#setTcpEndpoint-java.lang.String-int-) | Stelt het TCP-eindpunt in. |
|
|  | [addLogSink()](#addLogSink--) | Voegt een logsink toe aan de zoeknetwerkknoop. |
|
|  | [addSearcher(String storagePath)](#addSearcher-java.lang.String-) | Voegt een zoekservice toe aan de zoeknetwerkknoop. |
|
|  | [addIndexer(String storagePath)](#addIndexer-java.lang.String-) | Voegt een indexeerdienst toe aan het zoeknetwerk‑knooppunt. |
|
|  | [addExtractor(String storagePath)](#addExtractor-java.lang.String-) | Voegt een extractiedienst toe aan het zoeknetwerk‑knooppunt. |
|
|  | [addShard(String storagePath)](#addShard-java.lang.String-) | Voegt een shard‑dienst toe aan het zoeknetwerk‑knooppunt. |
|
|  | [completeNode()](#completeNode--) | Rondt de configuratie van het zoeknetwerk‑knooppunt af. |
|
### NodeConfigurator() {#NodeConfigurator--}
```
public NodeConfigurator()
```


### setTcpEndpoint(String hostNameOrAddress, int port) {#setTcpEndpoint-java.lang.String-int-}
```
public abstract NodeConfigurator setTcpEndpoint(String hostNameOrAddress, int port)
```


Stelt het TCP-eindpunt in.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | hostNameOrAddress | java.lang.String | De hostnaam of het adres. |
|
|  | port | int | Het poortnummer. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addLogSink() {#addLogSink--}
```
public abstract NodeConfigurator addLogSink()
```


Voegt een logsink toe aan de zoeknetwerkknoop.


**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addSearcher(String storagePath) {#addSearcher-java.lang.String-}
```
public abstract NodeConfigurator addSearcher(String storagePath)
```


Voegt een zoekservice toe aan de zoeknetwerkknoop.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | storagePath | java.lang.String | Het opslagpad van de toevoegingsservice. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addIndexer(String storagePath) {#addIndexer-java.lang.String-}
```
public abstract NodeConfigurator addIndexer(String storagePath)
```


Voegt een indexeerdienst toe aan het zoeknetwerk‑knooppunt.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | storagePath | java.lang.String | Het opslagpad van de toevoegingsservice. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addExtractor(String storagePath) {#addExtractor-java.lang.String-}
```
public abstract NodeConfigurator addExtractor(String storagePath)
```


Voegt een extractiedienst toe aan het zoeknetwerk‑knooppunt.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | storagePath | java.lang.String | Het opslagpad van de toevoegingsservice. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addShard(String storagePath) {#addShard-java.lang.String-}
```
public abstract NodeConfigurator addShard(String storagePath)
```


Voegt een shard‑dienst toe aan het zoeknetwerk‑knooppunt.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | storagePath | java.lang.String | Het opslagpad van de toevoegingsservice. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### completeNode() {#completeNode--}
```
public abstract Configurator completeNode()
```


Rondt de configuratie van het zoeknetwerk‑knooppunt af.


**Returns:**
[Configurator](../../com.groupdocs.search.scaling.configuring/configurator) - The configurator.

