---
title: "Configurator"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta il configuratore della rete di ricerca."
type: docs
weight: 11
url: /it/java/com.groupdocs.search.scaling.configuring/configurator/
---
**Inheritance:**
java.lang.Object
```
public class Configurator
```

Rappresenta il configuratore della rete di ricerca.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [Configurator()](#Configurator--) | Inizializza una nuova istanza della classe Configurator. |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [setIndexSettings()](#setIndexSettings--) | Inizia a configurare le impostazioni dell'indice per ogni shard nella rete di ricerca. |
|
|  | [addNode(int nodeIndex)](#addNode-int-) | Aggiunge un nodo alla configurazione della rete di ricerca. |
|
|  | [completeConfiguration()](#completeConfiguration--) | Completa il processo di configurazione e restituisce un'istanza della configurazione della rete di ricerca. |
|
| [getCore()](#getCore--) |  |
### Configurator() {#Configurator--}
```
public Configurator()
```


Inizializza una nuova istanza della classe Configurator.


### setIndexSettings() {#setIndexSettings--}
```
public IndexSettingsConfigurator setIndexSettings()
```


Inizia a configurare le impostazioni dell'indice per ogni shard nella rete di ricerca.


**Returns:**
[IndexSettingsConfigurator](../../com.groupdocs.search.scaling.configuring/indexsettingsconfigurator) - The index settings configurator.

### addNode(int nodeIndex) {#addNode-int-}
```
public NodeConfigurator addNode(int nodeIndex)
```


Aggiunge un nodo alla configurazione della rete di ricerca.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | nodeIndex | int | L'indice del nodo. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - The node configurator.

### completeConfiguration() {#completeConfiguration--}
```
public Configuration completeConfiguration()
```


Completa il processo di configurazione e restituisce un'istanza della configurazione della rete di ricerca.


**Returns:**
[Configuration](../../com.groupdocs.search.scaling.configuring/configuration) - The configuration.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
