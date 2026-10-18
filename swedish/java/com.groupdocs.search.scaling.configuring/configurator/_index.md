---
title: "Configurator"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar söknätverkets konfigurator."
type: docs
weight: 11
url: /sv/java/com.groupdocs.search.scaling.configuring/configurator/
---
**Inheritance:**
java.lang.Object
```
public class Configurator
```

Representerar söknätverkets konfigurator.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [Configurator()](#Configurator--) | Initierar en ny instans av klassen Configurator. |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [setIndexSettings()](#setIndexSettings--) | Startar konfiguration av indexinställningarna för varje shard i söknetverket. |
|
|  | [addNode(int nodeIndex)](#addNode-int-) | Lägger till en nod i söknetverkets konfiguration. |
|
|  | [completeConfiguration()](#completeConfiguration--) | Slutför konfigurationsprocessen och returnerar en instans av söknetverkets konfiguration. |
|
| [getCore()](#getCore--) |  |
### Configurator() {#Configurator--}
```
public Configurator()
```


Initierar en ny instans av klassen Configurator.


### setIndexSettings() {#setIndexSettings--}
```
public IndexSettingsConfigurator setIndexSettings()
```


Startar konfiguration av indexinställningarna för varje shard i söknetverket.


**Returns:**
[IndexSettingsConfigurator](../../com.groupdocs.search.scaling.configuring/indexsettingsconfigurator) - The index settings configurator.

### addNode(int nodeIndex) {#addNode-int-}
```
public NodeConfigurator addNode(int nodeIndex)
```


Lägger till en nod i söknetverkets konfiguration.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | nodeIndex | int | Nodindexet. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - The node configurator.

### completeConfiguration() {#completeConfiguration--}
```
public Configuration completeConfiguration()
```


Slutför konfigurationsprocessen och returnerar en instans av söknetverkets konfiguration.


**Returns:**
[Configuration](../../com.groupdocs.search.scaling.configuring/configuration) - The configuration.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
