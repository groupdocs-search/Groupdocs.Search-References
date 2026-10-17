---
title: "SearchNetworkNode"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente un nœud du réseau de recherche qui peut contenir des services tels que l'extracteur, l'indexeur, le chercheur, la partition."
type: docs
weight: 11
url: /fr/java/com.groupdocs.search.scaling/searchnetworknode/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable
```
public class SearchNetworkNode implements Closeable
```

Représente un nœud du réseau de recherche qui peut contenir des services tels que extracteur, indexeur, chercheur, shard.

## Constructeurs

| Constructeur | Description |
| --- | --- |
|  | [SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings)](#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-) | Initialise une nouvelle instance de la classe  SearchNetworkNode  . |
|
|  | [SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger)](#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-com.groupdocs.search.common.ILogger-) | Initialise une nouvelle instance de la classe  SearchNetworkNode  . |
|
|  | [SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger, Configuration configuration)](#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-com.groupdocs.search.common.ILogger-com.groupdocs.search.scaling.configuring.Configuration-) | Initialise une nouvelle instance de la classe  SearchNetworkNode  . |
|
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [start()](#start--) | Démarre le fonctionnement du nœud du réseau de recherche. |
|
|  | [configureAllNodes()](#configureAllNodes--) | Configure tous les nœuds du réseau de recherche. |
|
|  | [configureNode(int nodeIndex)](#configureNode-int-) | Configure le nœud spécifié du réseau de recherche. |
|
|  | [getCustomExtractors()](#getCustomExtractors--) | Obtient la collection d'extracteurs personnalisés. |
|
|  | [setOcrConnector(IOcrConnector ocrConnector)](#setOcrConnector-com.groupdocs.search.options.IOcrConnector-) | Définit un connecteur OCR utilisé pour le traitement OCR. |
|
|  | [setWordFormsProvider(IWordFormsProvider wordFormsProvider)](#setWordFormsProvider-com.groupdocs.search.dictionaries.IWordFormsProvider-) | Définit un fournisseur de formes de mots. |
|
|  | [close()](#close--) | Libère toutes les ressources utilisées par le  SearchNetworkNode . |
|
|  | [getNodeIndex()](#getNodeIndex--) | Obtient l'index du nœud du réseau de recherche. |
|
|  | [getEvents()](#getEvents--) | Obtient le hub d'événements pour s'abonner aux événements. |
|
|  | [getIndexer()](#getIndexer--) | Obtient l'indexeur. |
|
|  | [getSearcher()](#getSearcher--) | Obtient le moteur de recherche. |
|
|  | [getShardIndices()](#getShardIndices--) | Obtient un tableau de tous les indices de fragments du réseau de recherche. |
|
|  | [getNodeIndex(int serviceIndex)](#getNodeIndex-int-) | Obtient l'indice du nœud où le service est situé. |
|
| [getCore()](#getCore--) |  |
### SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings) {#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-}
```
public SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings)
```


Initialise une nouvelle instance de la classe  SearchNetworkNode  .


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | nodeIndex | int | L'index du nœud. |
|
|  | storagePath | java.lang.String | Le chemin de stockage. |
|
|  | networkSettings | [INetworkSettings](../../com.groupdocs.search.scaling.configuring/inetworksettings) | Les paramètres du réseau. |
|

### SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger) {#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-com.groupdocs.search.common.ILogger-}
```
public SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger)
```


Initialise une nouvelle instance de la classe  SearchNetworkNode  .


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | nodeIndex | int | L'index du nœud. |
|
|  | storagePath | java.lang.String | Le chemin de stockage. |
|
|  | networkSettings | [INetworkSettings](../../com.groupdocs.search.scaling.configuring/inetworksettings) | Les paramètres du réseau. |
|
|  | logger | [ILogger](../../com.groupdocs.search.common/ilogger) | Le journal. |
|

### SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger, Configuration configuration) {#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-com.groupdocs.search.common.ILogger-com.groupdocs.search.scaling.configuring.Configuration-}
```
public SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger, Configuration configuration)
```


Initialise une nouvelle instance de la classe  SearchNetworkNode  .


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | nodeIndex | int | L'index du nœud. |
|
|  | storagePath | java.lang.String | Le chemin de stockage. |
|
|  | networkSettings | [INetworkSettings](../../com.groupdocs.search.scaling.configuring/inetworksettings) | Les paramètres du réseau. |
|
|  | logger | [ILogger](../../com.groupdocs.search.common/ilogger) | Le journal. |
|
|  | configuration | [Configuration](../../com.groupdocs.search.scaling.configuring/configuration) | La configuration. |
|

### start() {#start--}
```
public void start()
```


Démarre le fonctionnement du nœud du réseau de recherche.


### configureAllNodes() {#configureAllNodes--}
```
public void configureAllNodes()
```


Configure tous les nœuds du réseau de recherche.


### configureNode(int nodeIndex) {#configureNode-int-}
```
public void configureNode(int nodeIndex)
```


Configure le nœud spécifié du réseau de recherche.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | nodeIndex | int | L'index du nœud. |
|

### getCustomExtractors() {#getCustomExtractors--}
```
public CustomExtractorCollection getCustomExtractors()
```


Obtient la collection d'extracteurs personnalisés. L'exemple complet d'implémentation d'un extracteur personnalisé est présenté dans la documentation de l'interface  GroupDocs.Search.Common.IFieldExtractor .


**Returns:**
[CustomExtractorCollection](../../com.groupdocs.search.common/customextractorcollection) - The custom extractor collection.

### setOcrConnector(IOcrConnector ocrConnector) {#setOcrConnector-com.groupdocs.search.options.IOcrConnector-}
```
public void setOcrConnector(IOcrConnector ocrConnector)
```


Définit un connecteur OCR utilisé pour le traitement OCR.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | ocrConnector | [IOcrConnector](../../com.groupdocs.search.options/iocrconnector) | Le connecteur OCR. |
|

### setWordFormsProvider(IWordFormsProvider wordFormsProvider) {#setWordFormsProvider-com.groupdocs.search.dictionaries.IWordFormsProvider-}
```
public void setWordFormsProvider(IWordFormsProvider wordFormsProvider)
```


Définit un fournisseur de formes de mots.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | wordFormsProvider | [IWordFormsProvider](../../com.groupdocs.search.dictionaries/iwordformsprovider) | Le fournisseur de formes de mots. |
|

### close() {#close--}
```
public void close()
```


Libère toutes les ressources utilisées par le  SearchNetworkNode .


### getNodeIndex() {#getNodeIndex--}
```
public int getNodeIndex()
```


Obtient l'index du nœud du réseau de recherche.


**Returns:**
int - L'index du nœud du réseau de recherche.

### getEvents() {#getEvents--}
```
public NodeEventHub getEvents()
```


Obtient le hub d'événements pour s'abonner aux événements.


**Returns:**
[NodeEventHub](../../com.groupdocs.search.scaling.events/nodeeventhub) - The event hub for subscribing to events.

### getIndexer() {#getIndexer--}
```
public Indexer getIndexer()
```


Obtient l'indexeur.


**Returns:**
[Indexer](../../com.groupdocs.search.scaling/indexer) - The indexer.

### getSearcher() {#getSearcher--}
```
public Searcher getSearcher()
```


Obtient le moteur de recherche.


**Returns:**
[Searcher](../../com.groupdocs.search.scaling/searcher) - The searcher.

### getShardIndices() {#getShardIndices--}
```
public int[] getShardIndices()
```


Obtient un tableau de tous les indices de fragments du réseau de recherche.


**Returns:**
int[] - Un tableau de tous les indices de fragments du réseau de recherche.

### getNodeIndex(int serviceIndex) {#getNodeIndex-int-}
```
public int getNodeIndex(int serviceIndex)
```


Obtient l'indice du nœud où le service est situé.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | serviceIndex | int | L'indice du service. |
|

**Returns:**
int - L'indice du nœud où le service est situé. Si l'indice du service est incorrect, -1 est renvoyé.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
