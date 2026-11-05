---
title: "SearchNetworkNode"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет узел поисковой сети, который может содержать такие сервисы, как извлекатель, индексатор, поисковик, шард."
type: docs
weight: 11
url: /ru/java/com.groupdocs.search.scaling/searchnetworknode/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable
```
public class SearchNetworkNode implements Closeable
```

Представляет узел поисковой сети, который может содержать такие сервисы, как extractor, indexer, searcher, shard.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings)](#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-) | Инициализирует новый экземпляр класса  SearchNetworkNode . |
|
|  | [SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger)](#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-com.groupdocs.search.common.ILogger-) | Инициализирует новый экземпляр класса  SearchNetworkNode . |
|
|  | [SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger, Configuration configuration)](#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-com.groupdocs.search.common.ILogger-com.groupdocs.search.scaling.configuring.Configuration-) | Инициализирует новый экземпляр класса  SearchNetworkNode . |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [start()](#start--) | Запускает работу узла поисковой сети. |
|
|  | [configureAllNodes()](#configureAllNodes--) | Настраивает все узлы в поисковой сети. |
|
|  | [configureNode(int nodeIndex)](#configureNode-int-) | Настраивает указанный узел в поисковой сети. |
|
|  | [getCustomExtractors()](#getCustomExtractors--) | Получает пользовательскую коллекцию извлекателей. |
|
|  | [setOcrConnector(IOcrConnector ocrConnector)](#setOcrConnector-com.groupdocs.search.options.IOcrConnector-) | Устанавливает OCR‑коннектор, используемый для обработки OCR. |
|
|  | [setWordFormsProvider(IWordFormsProvider wordFormsProvider)](#setWordFormsProvider-com.groupdocs.search.dictionaries.IWordFormsProvider-) | Устанавливает поставщик форм слов. |
|
|  | [close()](#close--) | Освобождает все ресурсы, используемые SearchNetworkNode. |
|
|  | [getNodeIndex()](#getNodeIndex--) | Получает индекс узла поисковой сети. |
|
|  | [getEvents()](#getEvents--) | Получает центр событий для подписки на события. |
|
|  | [getIndexer()](#getIndexer--) | Получает индексатор. |
|
|  | [getSearcher()](#getSearcher--) | Получает поисковик. |
|
|  | [getShardIndices()](#getShardIndices--) | Получает массив всех индексов шарда в поисковой сети. |
|
|  | [getNodeIndex(int serviceIndex)](#getNodeIndex-int-) | Получает индекс узла, где находится сервис. |
|
| [getCore()](#getCore--) |  |
### SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings) {#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-}
```
public SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings)
```


Инициализирует новый экземпляр класса  SearchNetworkNode .


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | nodeIndex | int | Индекс узла. |
|
|  | storagePath | java.lang.String | Путь к хранилищу. |
|
|  | networkSettings | [INetworkSettings](../../com.groupdocs.search.scaling.configuring/inetworksettings) | Настройки сети. |
|

### SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger) {#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-com.groupdocs.search.common.ILogger-}
```
public SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger)
```


Инициализирует новый экземпляр класса  SearchNetworkNode .


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | nodeIndex | int | Индекс узла. |
|
|  | storagePath | java.lang.String | Путь к хранилищу. |
|
|  | networkSettings | [INetworkSettings](../../com.groupdocs.search.scaling.configuring/inetworksettings) | Настройки сети. |
|
|  | logger | [ILogger](../../com.groupdocs.search.common/ilogger) | Логгер. |
|

### SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger, Configuration configuration) {#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-com.groupdocs.search.common.ILogger-com.groupdocs.search.scaling.configuring.Configuration-}
```
public SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger, Configuration configuration)
```


Инициализирует новый экземпляр класса  SearchNetworkNode .


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | nodeIndex | int | Индекс узла. |
|
|  | storagePath | java.lang.String | Путь к хранилищу. |
|
|  | networkSettings | [INetworkSettings](../../com.groupdocs.search.scaling.configuring/inetworksettings) | Настройки сети. |
|
|  | logger | [ILogger](../../com.groupdocs.search.common/ilogger) | Логгер. |
|
|  | configuration | [Configuration](../../com.groupdocs.search.scaling.configuring/configuration) | Конфигурация. |
|

### start() {#start--}
```
public void start()
```


Запускает работу узла поисковой сети.


### configureAllNodes() {#configureAllNodes--}
```
public void configureAllNodes()
```


Настраивает все узлы в поисковой сети.


### configureNode(int nodeIndex) {#configureNode-int-}
```
public void configureNode(int nodeIndex)
```


Настраивает указанный узел в поисковой сети.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | nodeIndex | int | Индекс узла. |
|

### getCustomExtractors() {#getCustomExtractors--}
```
public CustomExtractorCollection getCustomExtractors()
```


Получает коллекцию пользовательских извлекателей. Полный пример реализации пользовательского извлекателя представлен в документации для интерфейса  GroupDocs.Search.Common.IFieldExtractor .


**Returns:**
[CustomExtractorCollection](../../com.groupdocs.search.common/customextractorcollection) - The custom extractor collection.

### setOcrConnector(IOcrConnector ocrConnector) {#setOcrConnector-com.groupdocs.search.options.IOcrConnector-}
```
public void setOcrConnector(IOcrConnector ocrConnector)
```


Устанавливает OCR‑коннектор, используемый для обработки OCR.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | ocrConnector | [IOcrConnector](../../com.groupdocs.search.options/iocrconnector) | Коннектор OCR. |
|

### setWordFormsProvider(IWordFormsProvider wordFormsProvider) {#setWordFormsProvider-com.groupdocs.search.dictionaries.IWordFormsProvider-}
```
public void setWordFormsProvider(IWordFormsProvider wordFormsProvider)
```


Устанавливает поставщик форм слов.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | wordFormsProvider | [IWordFormsProvider](../../com.groupdocs.search.dictionaries/iwordformsprovider) | Провайдер словоформ. |
|

### close() {#close--}
```
public void close()
```


Освобождает все ресурсы, используемые SearchNetworkNode.


### getNodeIndex() {#getNodeIndex--}
```
public int getNodeIndex()
```


Получает индекс узла поисковой сети.


**Returns:**
int - Индекс узла поисковой сети.

### getEvents() {#getEvents--}
```
public NodeEventHub getEvents()
```


Получает центр событий для подписки на события.


**Returns:**
[NodeEventHub](../../com.groupdocs.search.scaling.events/nodeeventhub) - The event hub for subscribing to events.

### getIndexer() {#getIndexer--}
```
public Indexer getIndexer()
```


Получает индексатор.


**Returns:**
[Indexer](../../com.groupdocs.search.scaling/indexer) - The indexer.

### getSearcher() {#getSearcher--}
```
public Searcher getSearcher()
```


Получает поисковик.


**Returns:**
[Searcher](../../com.groupdocs.search.scaling/searcher) - The searcher.

### getShardIndices() {#getShardIndices--}
```
public int[] getShardIndices()
```


Получает массив всех индексов шарда в поисковой сети.


**Returns:**
`int[]` - Массив всех индексов шарда в поисковой сети.

### getNodeIndex(int serviceIndex) {#getNodeIndex-int-}
```
public int getNodeIndex(int serviceIndex)
```


Получает индекс узла, где находится сервис.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | serviceIndex | int | Индекс сервиса. |
|

**Returns:**
`int` - Индекс узла, где находится сервис. Если индекс сервиса некорректен, возвращается -1.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
