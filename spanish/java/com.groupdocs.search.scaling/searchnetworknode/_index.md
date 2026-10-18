---
title: "SearchNetworkNode"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa un nodo de red de búsqueda que puede contener servicios como extractor, indexador, buscador, fragmento."
type: docs
weight: 11
url: /es/java/com.groupdocs.search.scaling/searchnetworknode/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable
```
public class SearchNetworkNode implements Closeable
```

Representa un nodo de la red de búsqueda que puede contener servicios como extractor, indexador, buscador, fragmento.

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings)](#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-) | Inicializa una nueva instancia de la clase  SearchNetworkNode. |
|
|  | [SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger)](#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-com.groupdocs.search.common.ILogger-) | Inicializa una nueva instancia de la clase  SearchNetworkNode. |
|
|  | [SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger, Configuration configuration)](#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-com.groupdocs.search.common.ILogger-com.groupdocs.search.scaling.configuring.Configuration-) | Inicializa una nueva instancia de la clase  SearchNetworkNode. |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [start()](#start--) | Inicia el funcionamiento del nodo de la red de búsqueda. |
|
|  | [configureAllNodes()](#configureAllNodes--) | Configura todos los nodos en la red de búsqueda. |
|
|  | [configureNode(int nodeIndex)](#configureNode-int-) | Configura el nodo especificado en la red de búsqueda. |
|
|  | [getCustomExtractors()](#getCustomExtractors--) | Obtiene la colección de extractores personalizados. |
|
|  | [setOcrConnector(IOcrConnector ocrConnector)](#setOcrConnector-com.groupdocs.search.options.IOcrConnector-) | Establece un conector OCR que se utiliza para el procesamiento OCR. |
|
|  | [setWordFormsProvider(IWordFormsProvider wordFormsProvider)](#setWordFormsProvider-com.groupdocs.search.dictionaries.IWordFormsProvider-) | Establece un proveedor de formas de palabras. |
|
|  | [close()](#close--) | Libera todos los recursos utilizados por el SearchNetworkNode. |
|
|  | [getNodeIndex()](#getNodeIndex--) | Obtiene el índice del nodo de la red de búsqueda. |
|
|  | [getEvents()](#getEvents--) | Obtiene el hub de eventos para suscribirse a eventos. |
|
|  | [getIndexer()](#getIndexer--) | Obtiene el indexador. |
|
|  | [getSearcher()](#getSearcher--) | Obtiene el buscador. |
|
|  | [getShardIndices()](#getShardIndices--) | Obtiene una matriz de todos los índices de fragmentos en la red de búsqueda. |
|
|  | [getNodeIndex(int serviceIndex)](#getNodeIndex-int-) | Obtiene el índice del nodo donde se encuentra el servicio. |
|
| [getCore()](#getCore--) |  |
### SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings) {#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-}
```
public SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings)
```


Inicializa una nueva instancia de la clase  SearchNetworkNode.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | índiceNodo | int | El índice del nodo. |
|
|  | rutaAlmacenamiento | java.lang.String | La ruta de almacenamiento. |
|
|  | networkSettings | [INetworkSettings](../../com.groupdocs.search.scaling.configuring/inetworksettings) | La configuración de la red. |
|

### SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger) {#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-com.groupdocs.search.common.ILogger-}
```
public SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger)
```


Inicializa una nueva instancia de la clase  SearchNetworkNode.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | índiceNodo | int | El índice del nodo. |
|
|  | rutaAlmacenamiento | java.lang.String | La ruta de almacenamiento. |
|
|  | networkSettings | [INetworkSettings](../../com.groupdocs.search.scaling.configuring/inetworksettings) | La configuración de la red. |
|
|  | logger | [ILogger](../../com.groupdocs.search.common/ilogger) | El registrador. |
|

### SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger, Configuration configuration) {#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-com.groupdocs.search.common.ILogger-com.groupdocs.search.scaling.configuring.Configuration-}
```
public SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger, Configuration configuration)
```


Inicializa una nueva instancia de la clase  SearchNetworkNode.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | índiceNodo | int | El índice del nodo. |
|
|  | rutaAlmacenamiento | java.lang.String | La ruta de almacenamiento. |
|
|  | networkSettings | [INetworkSettings](../../com.groupdocs.search.scaling.configuring/inetworksettings) | La configuración de la red. |
|
|  | logger | [ILogger](../../com.groupdocs.search.common/ilogger) | El registrador. |
|
|  | configuration | [Configuration](../../com.groupdocs.search.scaling.configuring/configuration) | La configuración. |
|

### start() {#start--}
```
public void start()
```


Inicia el funcionamiento del nodo de la red de búsqueda.


### configureAllNodes() {#configureAllNodes--}
```
public void configureAllNodes()
```


Configura todos los nodos en la red de búsqueda.


### configureNode(int nodeIndex) {#configureNode-int-}
```
public void configureNode(int nodeIndex)
```


Configura el nodo especificado en la red de búsqueda.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | índiceNodo | int | El índice del nodo. |
|

### getCustomExtractors() {#getCustomExtractors--}
```
public CustomExtractorCollection getCustomExtractors()
```


Obtiene la colección de extractores personalizados. El ejemplo completo de implementación de un extractor personalizado se presenta en la documentación de la interfaz GroupDocs.Search.Common.IFieldExtractor.


**Returns:**
[CustomExtractorCollection](../../com.groupdocs.search.common/customextractorcollection) - The custom extractor collection.

### setOcrConnector(IOcrConnector ocrConnector) {#setOcrConnector-com.groupdocs.search.options.IOcrConnector-}
```
public void setOcrConnector(IOcrConnector ocrConnector)
```


Establece un conector OCR que se utiliza para el procesamiento OCR.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | ocrConnector | [IOcrConnector](../../com.groupdocs.search.options/iocrconnector) | El conector OCR. |
|

### setWordFormsProvider(IWordFormsProvider wordFormsProvider) {#setWordFormsProvider-com.groupdocs.search.dictionaries.IWordFormsProvider-}
```
public void setWordFormsProvider(IWordFormsProvider wordFormsProvider)
```


Establece un proveedor de formas de palabras.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | wordFormsProvider | [IWordFormsProvider](../../com.groupdocs.search.dictionaries/iwordformsprovider) | El proveedor de formas de palabras. |
|

### close() {#close--}
```
public void close()
```


Libera todos los recursos utilizados por el SearchNetworkNode.


### getNodeIndex() {#getNodeIndex--}
```
public int getNodeIndex()
```


Obtiene el índice del nodo de la red de búsqueda.


**Returns:**
int - El índice del nodo de la red de búsqueda.

### getEvents() {#getEvents--}
```
public NodeEventHub getEvents()
```


Obtiene el hub de eventos para suscribirse a eventos.


**Returns:**
[NodeEventHub](../../com.groupdocs.search.scaling.events/nodeeventhub) - The event hub for subscribing to events.

### getIndexer() {#getIndexer--}
```
public Indexer getIndexer()
```


Obtiene el indexador.


**Returns:**
[Indexer](../../com.groupdocs.search.scaling/indexer) - The indexer.

### getSearcher() {#getSearcher--}
```
public Searcher getSearcher()
```


Obtiene el buscador.


**Returns:**
[Searcher](../../com.groupdocs.search.scaling/searcher) - The searcher.

### getShardIndices() {#getShardIndices--}
```
public int[] getShardIndices()
```


Obtiene una matriz de todos los índices de fragmentos en la red de búsqueda.


**Returns:**
int[] - Una matriz de todos los índices de fragmentos en la red de búsqueda.

### getNodeIndex(int serviceIndex) {#getNodeIndex-int-}
```
public int getNodeIndex(int serviceIndex)
```


Obtiene el índice del nodo donde se encuentra el servicio.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | serviceIndex | int | El índice del servicio. |
|

**Returns:**
int - El índice del nodo donde se encuentra el servicio. Si el índice del servicio es incorrecto, se devuelve -1.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
