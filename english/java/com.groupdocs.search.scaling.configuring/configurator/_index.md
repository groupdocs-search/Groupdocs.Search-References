---
title: Configurator
second_title: GroupDocs.Search for Java API Reference
description: Represents the search network configurator.
type: docs
weight: 11
url: /java/com.groupdocs.search.scaling.configuring/configurator/
---
**Inheritance:**
java.lang.Object
```
public class Configurator
```

Represents the search network configurator.
## Constructors

| Constructor | Description |
| --- | --- |
| [Configurator()](#Configurator--) | Initializes a new instance of the  Configurator  class. |
## Methods

| Method | Description |
| --- | --- |
| [setIndexSettings()](#setIndexSettings--) | Starts configuring the index settings for each shard in the search network. |
| [addNode(int nodeIndex)](#addNode-int-) | Adds a node to the search network configuration. |
| [completeConfiguration()](#completeConfiguration--) | Completes the configuration process and returns an instance of the search network configuration. |
| [getCore()](#getCore--) |  |
### Configurator() {#Configurator--}
```
public Configurator()
```


Initializes a new instance of the  Configurator  class.

### setIndexSettings() {#setIndexSettings--}
```
public IndexSettingsConfigurator setIndexSettings()
```


Starts configuring the index settings for each shard in the search network.

**Returns:**
[IndexSettingsConfigurator](../../com.groupdocs.search.scaling.configuring/indexsettingsconfigurator) - The index settings configurator.
### addNode(int nodeIndex) {#addNode-int-}
```
public NodeConfigurator addNode(int nodeIndex)
```


Adds a node to the search network configuration.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| nodeIndex | int | The node index. |

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - The node configurator.
### completeConfiguration() {#completeConfiguration--}
```
public Configuration completeConfiguration()
```


Completes the configuration process and returns an instance of the search network configuration.

**Returns:**
[Configuration](../../com.groupdocs.search.scaling.configuring/configuration) - The configuration.
### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
