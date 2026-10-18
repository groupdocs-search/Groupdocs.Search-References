---
title: "NodeConfigurator"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar söknätverkets nodkonfigurator."
type: docs
weight: 13
url: /sv/java/com.groupdocs.search.scaling.configuring/nodeconfigurator/
---
**Inheritance:**
java.lang.Object
```
public abstract class NodeConfigurator
```

Representerar söknätverkets nodkonfigurator.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [NodeConfigurator()](#NodeConfigurator--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [setTcpEndpoint(String hostNameOrAddress, int port)](#setTcpEndpoint-java.lang.String-int-) | Ställer in TCP‑slutpunkten. |
|
|  | [addLogSink()](#addLogSink--) | Lägger till en loggsänka till sök‑nätverks‑nod. |
|
|  | [addSearcher(String storagePath)](#addSearcher-java.lang.String-) | Lägger till en söktjänst till sök‑nätverks‑nod. |
|
|  | [addIndexer(String storagePath)](#addIndexer-java.lang.String-) | Lägger till en indexeringstjänst till söknetverkets nod. |
|
|  | [addExtractor(String storagePath)](#addExtractor-java.lang.String-) | Lägger till en extraheringstjänst till söknetverkets nod. |
|
|  | [addShard(String storagePath)](#addShard-java.lang.String-) | Lägger till en shardingtjänst till söknetverkets nod. |
|
|  | [completeNode()](#completeNode--) | Slutför konfigurationen av söknetverkets nod. |
|
### NodeConfigurator() {#NodeConfigurator--}
```
public NodeConfigurator()
```


### setTcpEndpoint(String hostNameOrAddress, int port) {#setTcpEndpoint-java.lang.String-int-}
```
public abstract NodeConfigurator setTcpEndpoint(String hostNameOrAddress, int port)
```


Ställer in TCP‑slutpunkten.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | hostNameOrAddress | java.lang.String | Värdnamnet eller adressen. |
|
|  | port | int | Portnumret. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addLogSink() {#addLogSink--}
```
public abstract NodeConfigurator addLogSink()
```


Lägger till en loggsänka till sök‑nätverks‑nod.


**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addSearcher(String storagePath) {#addSearcher-java.lang.String-}
```
public abstract NodeConfigurator addSearcher(String storagePath)
```


Lägger till en söktjänst till sök‑nätverks‑nod.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | storagePath | java.lang.String | Lagringsvägen för tilläggstjänsten. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addIndexer(String storagePath) {#addIndexer-java.lang.String-}
```
public abstract NodeConfigurator addIndexer(String storagePath)
```


Lägger till en indexeringstjänst till söknetverkets nod.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | storagePath | java.lang.String | Lagringsvägen för tilläggstjänsten. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addExtractor(String storagePath) {#addExtractor-java.lang.String-}
```
public abstract NodeConfigurator addExtractor(String storagePath)
```


Lägger till en extraheringstjänst till söknetverkets nod.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | storagePath | java.lang.String | Lagringsvägen för tilläggstjänsten. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addShard(String storagePath) {#addShard-java.lang.String-}
```
public abstract NodeConfigurator addShard(String storagePath)
```


Lägger till en shardingtjänst till söknetverkets nod.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | storagePath | java.lang.String | Lagringsvägen för tilläggstjänsten. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### completeNode() {#completeNode--}
```
public abstract Configurator completeNode()
```


Slutför konfigurationen av söknetverkets nod.


**Returns:**
[Configurator](../../com.groupdocs.search.scaling.configuring/configurator) - The configurator.

