---
title: "Configurator"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt de zoeknetwerkconfigurator voor."
type: docs
weight: 11
url: /nl/java/com.groupdocs.search.scaling.configuring/configurator/
---
**Inheritance:**
java.lang.Object
```
public class Configurator
```

Stelt de zoeknetwerkconfigurator voor.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [Configurator()](#Configurator--) | Initialiseert een nieuw exemplaar van de Configurator‑klasse. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [setIndexSettings()](#setIndexSettings--) | Start met het configureren van de indexinstellingen voor elke shard in het zoeknetwerk. |
|
|  | [addNode(int nodeIndex)](#addNode-int-) | Voegt een knooppunt toe aan de configuratie van het zoeknetwerk. |
|
|  | [completeConfiguration()](#completeConfiguration--) | Rondt het configuratieproces af en retourneert een exemplaar van de configuratie van het zoeknetwerk. |
|
| [getCore()](#getCore--) |  |
### Configurator() {#Configurator--}
```
public Configurator()
```


Initialiseert een nieuw exemplaar van de Configurator‑klasse.


### setIndexSettings() {#setIndexSettings--}
```
public IndexSettingsConfigurator setIndexSettings()
```


Start met het configureren van de indexinstellingen voor elke shard in het zoeknetwerk.


**Returns:**
[IndexSettingsConfigurator](../../com.groupdocs.search.scaling.configuring/indexsettingsconfigurator) - The index settings configurator.

### addNode(int nodeIndex) {#addNode-int-}
```
public NodeConfigurator addNode(int nodeIndex)
```


Voegt een knooppunt toe aan de configuratie van het zoeknetwerk.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | nodeIndex | int | De knooppuntindex. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - The node configurator.

### completeConfiguration() {#completeConfiguration--}
```
public Configuration completeConfiguration()
```


Rondt het configuratieproces af en retourneert een exemplaar van de configuratie van het zoeknetwerk.


**Returns:**
[Configuration](../../com.groupdocs.search.scaling.configuring/configuration) - The configuration.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
