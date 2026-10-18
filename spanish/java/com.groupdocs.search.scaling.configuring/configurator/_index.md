---
title: "Configurador"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa el configurador de la red de búsqueda."
type: docs
weight: 11
url: /es/java/com.groupdocs.search.scaling.configuring/configurator/
---
**Inheritance:**
java.lang.Object
```
public class Configurator
```

Representa el configurador de la red de búsqueda.

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [Configurator()](#Configurator--) | Inicializa una nueva instancia de la clase Configurator. |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [setIndexSettings()](#setIndexSettings--) | Comienza a configurar los ajustes del índice para cada fragmento en la red de búsqueda. |
|
|  | [addNode(int nodeIndex)](#addNode-int-) | Agrega un nodo a la configuración de la red de búsqueda. |
|
|  | [completeConfiguration()](#completeConfiguration--) | Completa el proceso de configuración y devuelve una instancia de la configuración de la red de búsqueda. |
|
| [getCore()](#getCore--) |  |
### Configurator() {#Configurator--}
```
public Configurator()
```


Inicializa una nueva instancia de la clase Configurator.


### setIndexSettings() {#setIndexSettings--}
```
public IndexSettingsConfigurator setIndexSettings()
```


Comienza a configurar los ajustes del índice para cada fragmento en la red de búsqueda.


**Returns:**
[IndexSettingsConfigurator](../../com.groupdocs.search.scaling.configuring/indexsettingsconfigurator) - The index settings configurator.

### addNode(int nodeIndex) {#addNode-int-}
```
public NodeConfigurator addNode(int nodeIndex)
```


Agrega un nodo a la configuración de la red de búsqueda.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | índiceNodo | int | El índice del nodo. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - The node configurator.

### completeConfiguration() {#completeConfiguration--}
```
public Configuration completeConfiguration()
```


Completa el proceso de configuración y devuelve una instancia de la configuración de la red de búsqueda.


**Returns:**
[Configuration](../../com.groupdocs.search.scaling.configuring/configuration) - The configuration.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
