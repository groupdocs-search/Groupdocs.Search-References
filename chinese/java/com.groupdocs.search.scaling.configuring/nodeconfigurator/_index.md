---
title: "NodeConfigurator"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示搜索网络节点配置器。"
type: docs
weight: 13
url: /zh/java/com.groupdocs.search.scaling.configuring/nodeconfigurator/
---
**Inheritance:**
java.lang.Object
```
public abstract class NodeConfigurator
```

表示搜索网络节点配置器。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [NodeConfigurator()](#NodeConfigurator--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [setTcpEndpoint(String hostNameOrAddress, int port)](#setTcpEndpoint-java.lang.String-int-) | 设置 TCP 端点。 |
|
|  | [addLogSink()](#addLogSink--) | 向搜索网络节点添加日志接收器。 |
|
|  | [addSearcher(String storagePath)](#addSearcher-java.lang.String-) | 向搜索网络节点添加搜索服务。 |
|
|  | [addIndexer(String storagePath)](#addIndexer-java.lang.String-) | 向搜索网络节点添加索引器服务。 |
|
|  | [addExtractor(String storagePath)](#addExtractor-java.lang.String-) | 向搜索网络节点添加提取器服务。 |
|
|  | [addShard(String storagePath)](#addShard-java.lang.String-) | 向搜索网络节点添加分片服务。 |
|
|  | [completeNode()](#completeNode--) | 完成搜索网络节点的配置。 |
|
### NodeConfigurator() {#NodeConfigurator--}
```
public NodeConfigurator()
```


### setTcpEndpoint(String hostNameOrAddress, int port) {#setTcpEndpoint-java.lang.String-int-}
```
public abstract NodeConfigurator setTcpEndpoint(String hostNameOrAddress, int port)
```


设置 TCP 端点。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | hostNameOrAddress | java.lang.String | 主机名或地址。 |
|
|  | port | int | 端口号。 |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addLogSink() {#addLogSink--}
```
public abstract NodeConfigurator addLogSink()
```


向搜索网络节点添加日志接收器。


**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addSearcher(String storagePath) {#addSearcher-java.lang.String-}
```
public abstract NodeConfigurator addSearcher(String storagePath)
```


向搜索网络节点添加搜索服务。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | storagePath | java.lang.String | 添加服务的存储路径。 |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addIndexer(String storagePath) {#addIndexer-java.lang.String-}
```
public abstract NodeConfigurator addIndexer(String storagePath)
```


向搜索网络节点添加索引器服务。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | storagePath | java.lang.String | 添加服务的存储路径。 |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addExtractor(String storagePath) {#addExtractor-java.lang.String-}
```
public abstract NodeConfigurator addExtractor(String storagePath)
```


向搜索网络节点添加提取器服务。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | storagePath | java.lang.String | 添加服务的存储路径。 |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addShard(String storagePath) {#addShard-java.lang.String-}
```
public abstract NodeConfigurator addShard(String storagePath)
```


向搜索网络节点添加分片服务。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | storagePath | java.lang.String | 添加服务的存储路径。 |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### completeNode() {#completeNode--}
```
public abstract Configurator completeNode()
```


完成搜索网络节点的配置。


**Returns:**
[Configurator](../../com.groupdocs.search.scaling.configuring/configurator) - The configurator.

