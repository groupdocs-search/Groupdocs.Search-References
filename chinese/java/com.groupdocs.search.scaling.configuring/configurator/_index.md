---
title: "Configurator"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示搜索网络配置器。"
type: docs
weight: 11
url: /zh/java/com.groupdocs.search.scaling.configuring/configurator/
---
**Inheritance:**
java.lang.Object
```
public class Configurator
```

表示搜索网络配置器。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [Configurator()](#Configurator--) | 初始化一个新的  Configurator  类实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [setIndexSettings()](#setIndexSettings--) | 开始为搜索网络中的每个分片配置索引设置。 |
|
|  | [addNode(int nodeIndex)](#addNode-int-) | 向搜索网络配置中添加节点。 |
|
|  | [completeConfiguration()](#completeConfiguration--) | 完成配置过程并返回搜索网络配置的实例。 |
|
| [getCore()](#getCore--) |  |
### Configurator() {#Configurator--}
```
public Configurator()
```


初始化一个新的  Configurator  类实例。


### setIndexSettings() {#setIndexSettings--}
```
public IndexSettingsConfigurator setIndexSettings()
```


开始为搜索网络中的每个分片配置索引设置。


**Returns:**
[IndexSettingsConfigurator](../../com.groupdocs.search.scaling.configuring/indexsettingsconfigurator) - The index settings configurator.

### addNode(int nodeIndex) {#addNode-int-}
```
public NodeConfigurator addNode(int nodeIndex)
```


向搜索网络配置中添加节点。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | nodeIndex | int | 节点索引。 |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - The node configurator.

### completeConfiguration() {#completeConfiguration--}
```
public Configuration completeConfiguration()
```


完成配置过程并返回搜索网络配置的实例。


**Returns:**
[Configuration](../../com.groupdocs.search.scaling.configuring/configuration) - The configuration.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
