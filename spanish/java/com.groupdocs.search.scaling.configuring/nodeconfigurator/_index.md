---
title: "NodeConfigurator"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa el configurador del nodo de la red de búsqueda."
type: docs
weight: 13
url: /es/java/com.groupdocs.search.scaling.configuring/nodeconfigurator/
---
**Inheritance:**
java.lang.Object
```
public abstract class NodeConfigurator
```

Representa el configurador del nodo de la red de búsqueda.

## Constructores

| Constructor | Descripción |
| --- | --- |
| [NodeConfigurator()](#NodeConfigurator--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
|  | [setTcpEndpoint(String hostNameOrAddress, int port)](#setTcpEndpoint-java.lang.String-int-) | Establece el punto final TCP. |
|
|  | [addLogSink()](#addLogSink--) | Añade un sumidero de registro al nodo de red de búsqueda. |
|
|  | [addSearcher(String storagePath)](#addSearcher-java.lang.String-) | Añade un servicio de búsqueda al nodo de red de búsqueda. |
|
|  | [addIndexer(String storagePath)](#addIndexer-java.lang.String-) | Agrega un servicio de indexador al nodo de la red de búsqueda. |
|
|  | [addExtractor(String storagePath)](#addExtractor-java.lang.String-) | Agrega un servicio de extractor al nodo de la red de búsqueda. |
|
|  | [addShard(String storagePath)](#addShard-java.lang.String-) | Agrega un servicio de fragmento al nodo de la red de búsqueda. |
|
|  | [completeNode()](#completeNode--) | Completa la configuración del nodo de la red de búsqueda. |
|
### NodeConfigurator() {#NodeConfigurator--}
```
public NodeConfigurator()
```


### setTcpEndpoint(String hostNameOrAddress, int port) {#setTcpEndpoint-java.lang.String-int-}
```
public abstract NodeConfigurator setTcpEndpoint(String hostNameOrAddress, int port)
```


Establece el punto final TCP.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | hostNameOrAddress | java.lang.String | El nombre de host o dirección. |
|
|  | puerto | int | El número de puerto. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addLogSink() {#addLogSink--}
```
public abstract NodeConfigurator addLogSink()
```


Añade un sumidero de registro al nodo de red de búsqueda.


**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addSearcher(String storagePath) {#addSearcher-java.lang.String-}
```
public abstract NodeConfigurator addSearcher(String storagePath)
```


Añade un servicio de búsqueda al nodo de red de búsqueda.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | rutaAlmacenamiento | java.lang.String | La ruta de almacenamiento del servicio de adición. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addIndexer(String storagePath) {#addIndexer-java.lang.String-}
```
public abstract NodeConfigurator addIndexer(String storagePath)
```


Agrega un servicio de indexador al nodo de la red de búsqueda.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | rutaAlmacenamiento | java.lang.String | La ruta de almacenamiento del servicio de adición. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addExtractor(String storagePath) {#addExtractor-java.lang.String-}
```
public abstract NodeConfigurator addExtractor(String storagePath)
```


Agrega un servicio de extractor al nodo de la red de búsqueda.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | rutaAlmacenamiento | java.lang.String | La ruta de almacenamiento del servicio de adición. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addShard(String storagePath) {#addShard-java.lang.String-}
```
public abstract NodeConfigurator addShard(String storagePath)
```


Agrega un servicio de fragmento al nodo de la red de búsqueda.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | rutaAlmacenamiento | java.lang.String | La ruta de almacenamiento del servicio de adición. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### completeNode() {#completeNode--}
```
public abstract Configurator completeNode()
```


Completa la configuración del nodo de la red de búsqueda.


**Returns:**
[Configurator](../../com.groupdocs.search.scaling.configuring/configurator) - The configurator.

