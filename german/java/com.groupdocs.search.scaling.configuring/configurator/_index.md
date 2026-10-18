---
title: "Configurator"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt den Suchnetzwerkkonfigurator dar."
type: docs
weight: 11
url: /de/java/com.groupdocs.search.scaling.configuring/configurator/
---
**Inheritance:**
java.lang.Object
```
public class Configurator
```

Stellt den Suchnetzwerkkonfigurator dar.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [Configurator()](#Configurator--) | Initialisiert eine neue Instanz der  Configurator  Klasse. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [setIndexSettings()](#setIndexSettings--) | Beginnt mit der Konfiguration der Indexeinstellungen für jeden Shard im Suchnetzwerk. |
|
|  | [addNode(int nodeIndex)](#addNode-int-) | Fügt der Suchnetzwerkkonfiguration einen Knoten hinzu. |
|
|  | [completeConfiguration()](#completeConfiguration--) | Vollständigt den Konfigurationsvorgang und gibt eine Instanz der Suchnetzwerkkonfiguration zurück. |
|
| [getCore()](#getCore--) |  |
### Configurator() {#Configurator--}
```
public Configurator()
```


Initialisiert eine neue Instanz der  Configurator  Klasse.


### setIndexSettings() {#setIndexSettings--}
```
public IndexSettingsConfigurator setIndexSettings()
```


Beginnt mit der Konfiguration der Indexeinstellungen für jeden Shard im Suchnetzwerk.


**Returns:**
[IndexSettingsConfigurator](../../com.groupdocs.search.scaling.configuring/indexsettingsconfigurator) - The index settings configurator.

### addNode(int nodeIndex) {#addNode-int-}
```
public NodeConfigurator addNode(int nodeIndex)
```


Fügt der Suchnetzwerkkonfiguration einen Knoten hinzu.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | nodeIndex | int | Der Knotenindex. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - The node configurator.

### completeConfiguration() {#completeConfiguration--}
```
public Configuration completeConfiguration()
```


Vollständigt den Konfigurationsvorgang und gibt eine Instanz der Suchnetzwerkkonfiguration zurück.


**Returns:**
[Configuration](../../com.groupdocs.search.scaling.configuring/configuration) - The configuration.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
