---
title: "Configurator"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente le configurateur du réseau de recherche."
type: docs
weight: 11
url: /fr/java/com.groupdocs.search.scaling.configuring/configurator/
---
**Inheritance:**
java.lang.Object
```
public class Configurator
```

Représente le configurateur du réseau de recherche.

## Constructeurs

| Constructeur | Description |
| --- | --- |
|  | [Configurator()](#Configurator--) | Initialise une nouvelle instance de la classe Configurator. |
|
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [setIndexSettings()](#setIndexSettings--) | Commence à configurer les paramètres d'index pour chaque fragment du réseau de recherche. |
|
|  | [addNode(int nodeIndex)](#addNode-int-) | Ajoute un nœud à la configuration du réseau de recherche. |
|
|  | [completeConfiguration()](#completeConfiguration--) | Termine le processus de configuration et renvoie une instance de la configuration du réseau de recherche. |
|
| [getCore()](#getCore--) |  |
### Configurator() {#Configurator--}
```
public Configurator()
```


Initialise une nouvelle instance de la classe Configurator.


### setIndexSettings() {#setIndexSettings--}
```
public IndexSettingsConfigurator setIndexSettings()
```


Commence à configurer les paramètres d'index pour chaque fragment du réseau de recherche.


**Returns:**
[IndexSettingsConfigurator](../../com.groupdocs.search.scaling.configuring/indexsettingsconfigurator) - The index settings configurator.

### addNode(int nodeIndex) {#addNode-int-}
```
public NodeConfigurator addNode(int nodeIndex)
```


Ajoute un nœud à la configuration du réseau de recherche.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | nodeIndex | int | L'index du nœud. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - The node configurator.

### completeConfiguration() {#completeConfiguration--}
```
public Configuration completeConfiguration()
```


Termine le processus de configuration et renvoie une instance de la configuration du réseau de recherche.


**Returns:**
[Configuration](../../com.groupdocs.search.scaling.configuring/configuration) - The configuration.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
