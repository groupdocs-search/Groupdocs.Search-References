---
title: "NodeConfigurator"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt den Konfigurator für Knoten des Suchnetzwerks dar."
type: docs
weight: 13
url: /de/java/com.groupdocs.search.scaling.configuring/nodeconfigurator/
---
**Inheritance:**
java.lang.Object
```
public abstract class NodeConfigurator
```

Stellt den Konfigurator für Knoten des Suchnetzwerks dar.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [NodeConfigurator()](#NodeConfigurator--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [setTcpEndpoint(String hostNameOrAddress, int port)](#setTcpEndpoint-java.lang.String-int-) | Legt den TCP-Endpunkt fest. |
|
|  | [addLogSink()](#addLogSink--) | Fügt dem Suchnetzwerkknoten einen Log‑Sink hinzu. |
|
|  | [addSearcher(String storagePath)](#addSearcher-java.lang.String-) | Fügt dem Suchnetzwerkknoten einen Sucher‑Dienst hinzu. |
|
|  | [addIndexer(String storagePath)](#addIndexer-java.lang.String-) | Fügt dem Suchnetzwerkknoten einen Indexer-Dienst hinzu. |
|
|  | [addExtractor(String storagePath)](#addExtractor-java.lang.String-) | Fügt dem Suchnetzwerkknoten einen Extraktionsdienst hinzu. |
|
|  | [addShard(String storagePath)](#addShard-java.lang.String-) | Fügt dem Suchnetzwerkknoten einen Shard-Dienst hinzu. |
|
|  | [completeNode()](#completeNode--) | Vollständigt die Konfiguration des Suchnetzwerkknotens. |
|
### NodeConfigurator() {#NodeConfigurator--}
```
public NodeConfigurator()
```


### setTcpEndpoint(String hostNameOrAddress, int port) {#setTcpEndpoint-java.lang.String-int-}
```
public abstract NodeConfigurator setTcpEndpoint(String hostNameOrAddress, int port)
```


Legt den TCP-Endpunkt fest.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | hostNameOrAddress | java.lang.String | Der Hostname oder die Adresse. |
|
|  | port | int | Die Portnummer. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addLogSink() {#addLogSink--}
```
public abstract NodeConfigurator addLogSink()
```


Fügt dem Suchnetzwerkknoten einen Log‑Sink hinzu.


**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addSearcher(String storagePath) {#addSearcher-java.lang.String-}
```
public abstract NodeConfigurator addSearcher(String storagePath)
```


Fügt dem Suchnetzwerkknoten einen Sucher‑Dienst hinzu.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | storagePath | java.lang.String | Der Speicherpfad des Hinzufügungsdienstes. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addIndexer(String storagePath) {#addIndexer-java.lang.String-}
```
public abstract NodeConfigurator addIndexer(String storagePath)
```


Fügt dem Suchnetzwerkknoten einen Indexer-Dienst hinzu.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | storagePath | java.lang.String | Der Speicherpfad des Hinzufügungsdienstes. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addExtractor(String storagePath) {#addExtractor-java.lang.String-}
```
public abstract NodeConfigurator addExtractor(String storagePath)
```


Fügt dem Suchnetzwerkknoten einen Extraktionsdienst hinzu.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | storagePath | java.lang.String | Der Speicherpfad des Hinzufügungsdienstes. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addShard(String storagePath) {#addShard-java.lang.String-}
```
public abstract NodeConfigurator addShard(String storagePath)
```


Fügt dem Suchnetzwerkknoten einen Shard-Dienst hinzu.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | storagePath | java.lang.String | Der Speicherpfad des Hinzufügungsdienstes. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### completeNode() {#completeNode--}
```
public abstract Configurator completeNode()
```


Vollständigt die Konfiguration des Suchnetzwerkknotens.


**Returns:**
[Configurator](../../com.groupdocs.search.scaling.configuring/configurator) - The configurator.

