---
title: "SearchNetworkNode"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示一个搜索网络节点，可包含提取器、索引器、搜索器、分片等服务。"
type: docs
weight: 11
url: /zh/java/com.groupdocs.search.scaling/searchnetworknode/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable
```
public class SearchNetworkNode implements Closeable
```

表示可以包含提取器、索引器、搜索器、分片等服务的搜索网络节点。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings)](#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-) | 初始化一个新的 SearchNetworkNode 类实例。 |
|
|  | [SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger)](#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-com.groupdocs.search.common.ILogger-) | 初始化一个新的 SearchNetworkNode 类实例。 |
|
|  | [SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger, Configuration configuration)](#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-com.groupdocs.search.common.ILogger-com.groupdocs.search.scaling.configuring.Configuration-) | 初始化一个新的 SearchNetworkNode 类实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [start()](#start--) | 启动搜索网络节点的功能。 |
|
|  | [configureAllNodes()](#configureAllNodes--) | 配置搜索网络中的所有节点。 |
|
|  | [configureNode(int nodeIndex)](#configureNode-int-) | 配置搜索网络中指定的节点。 |
|
|  | [getCustomExtractors()](#getCustomExtractors--) | 获取自定义提取器集合。 |
|
|  | [setOcrConnector(IOcrConnector ocrConnector)](#setOcrConnector-com.groupdocs.search.options.IOcrConnector-) | 设置用于 OCR 处理的 OCR 连接器。 |
|
|  | [setWordFormsProvider(IWordFormsProvider wordFormsProvider)](#setWordFormsProvider-com.groupdocs.search.dictionaries.IWordFormsProvider-) | 设置词形提供程序。 |
|
|  | [close()](#close--) | 释放 SearchNetworkNode 使用的所有资源。 |
|
|  | [getNodeIndex()](#getNodeIndex--) | 获取搜索网络节点的索引。 |
|
|  | [getEvents()](#getEvents--) | 获取用于订阅事件的事件中心。 |
|
|  | [getIndexer()](#getIndexer--) | 获取索引器。 |
|
|  | [getSearcher()](#getSearcher--) | 获取搜索器。 |
|
|  | [getShardIndices()](#getShardIndices--) | 获取搜索网络中所有分片索引的数组。 |
|
|  | [getNodeIndex(int serviceIndex)](#getNodeIndex-int-) | 获取服务所在节点的索引。 |
|
| [getCore()](#getCore--) |  |
### SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings) {#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-}
```
public SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings)
```


初始化一个新的 SearchNetworkNode 类实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | nodeIndex | int | 节点索引。 |
|
|  | storagePath | java.lang.String | 存储路径。 |
|
|  | networkSettings | [INetworkSettings](../../com.groupdocs.search.scaling.configuring/inetworksettings) | 网络设置。 |
|

### SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger) {#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-com.groupdocs.search.common.ILogger-}
```
public SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger)
```


初始化一个新的 SearchNetworkNode 类实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | nodeIndex | int | 节点索引。 |
|
|  | storagePath | java.lang.String | 存储路径。 |
|
|  | networkSettings | [INetworkSettings](../../com.groupdocs.search.scaling.configuring/inetworksettings) | 网络设置。 |
|
|  | logger | [ILogger](../../com.groupdocs.search.common/ilogger) | 日志记录器。 |
|

### SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger, Configuration configuration) {#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-com.groupdocs.search.common.ILogger-com.groupdocs.search.scaling.configuring.Configuration-}
```
public SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger, Configuration configuration)
```


初始化一个新的 SearchNetworkNode 类实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | nodeIndex | int | 节点索引。 |
|
|  | storagePath | java.lang.String | 存储路径。 |
|
|  | networkSettings | [INetworkSettings](../../com.groupdocs.search.scaling.configuring/inetworksettings) | 网络设置。 |
|
|  | logger | [ILogger](../../com.groupdocs.search.common/ilogger) | 日志记录器。 |
|
|  | configuration | [Configuration](../../com.groupdocs.search.scaling.configuring/configuration) | 配置。 |
|

### start() {#start--}
```
public void start()
```


启动搜索网络节点的功能。


### configureAllNodes() {#configureAllNodes--}
```
public void configureAllNodes()
```


配置搜索网络中的所有节点。


### configureNode(int nodeIndex) {#configureNode-int-}
```
public void configureNode(int nodeIndex)
```


配置搜索网络中指定的节点。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | nodeIndex | int | 节点索引。 |
|

### getCustomExtractors() {#getCustomExtractors--}
```
public CustomExtractorCollection getCustomExtractors()
```


获取自定义提取器集合。实现自定义提取器的完整示例在 GroupDocs.Search.Common.IFieldExtractor 接口的文档中提供。


**Returns:**
[CustomExtractorCollection](../../com.groupdocs.search.common/customextractorcollection) - The custom extractor collection.

### setOcrConnector(IOcrConnector ocrConnector) {#setOcrConnector-com.groupdocs.search.options.IOcrConnector-}
```
public void setOcrConnector(IOcrConnector ocrConnector)
```


设置用于 OCR 处理的 OCR 连接器。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | ocrConnector | [IOcrConnector](../../com.groupdocs.search.options/iocrconnector) | OCR 连接器。 |
|

### setWordFormsProvider(IWordFormsProvider wordFormsProvider) {#setWordFormsProvider-com.groupdocs.search.dictionaries.IWordFormsProvider-}
```
public void setWordFormsProvider(IWordFormsProvider wordFormsProvider)
```


设置词形提供程序。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | wordFormsProvider | [IWordFormsProvider](../../com.groupdocs.search.dictionaries/iwordformsprovider) | 词形提供程序。 |
|

### close() {#close--}
```
public void close()
```


释放 SearchNetworkNode 使用的所有资源。


### getNodeIndex() {#getNodeIndex--}
```
public int getNodeIndex()
```


获取搜索网络节点的索引。


**Returns:**
int - 搜索网络节点的索引。

### getEvents() {#getEvents--}
```
public NodeEventHub getEvents()
```


获取用于订阅事件的事件中心。


**Returns:**
[NodeEventHub](../../com.groupdocs.search.scaling.events/nodeeventhub) - The event hub for subscribing to events.

### getIndexer() {#getIndexer--}
```
public Indexer getIndexer()
```


获取索引器。


**Returns:**
[Indexer](../../com.groupdocs.search.scaling/indexer) - The indexer.

### getSearcher() {#getSearcher--}
```
public Searcher getSearcher()
```


获取搜索器。


**Returns:**
[Searcher](../../com.groupdocs.search.scaling/searcher) - The searcher.

### getShardIndices() {#getShardIndices--}
```
public int[] getShardIndices()
```


获取搜索网络中所有分片索引的数组。


**Returns:**
int[] - 搜索网络中所有分片索引的数组。

### getNodeIndex(int serviceIndex) {#getNodeIndex-int-}
```
public int getNodeIndex(int serviceIndex)
```


获取服务所在节点的索引。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | serviceIndex | int | 服务索引。 |
|

**Returns:**
int - 服务所在节点的索引。如果服务索引不正确，则返回 -1。

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
