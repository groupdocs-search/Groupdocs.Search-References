---
title: "NodeConfigurator"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente le configurateur du nœud du réseau de recherche."
type: docs
weight: 13
url: /fr/java/com.groupdocs.search.scaling.configuring/nodeconfigurator/
---
**Inheritance:**
java.lang.Object
```
public abstract class NodeConfigurator
```

Représente le configurateur du nœud du réseau de recherche.

## Constructeurs

| Constructeur | Description |
| --- | --- |
| [NodeConfigurator()](#NodeConfigurator--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [setTcpEndpoint(String hostNameOrAddress, int port)](#setTcpEndpoint-java.lang.String-int-) | Définit le point de terminaison TCP. |
|
|  | [addLogSink()](#addLogSink--) | Ajoute un puits de journalisation au nœud du réseau de recherche. |
|
|  | [addSearcher(String storagePath)](#addSearcher-java.lang.String-) | Ajoute un service de recherche au nœud du réseau de recherche. |
|
|  | [addIndexer(String storagePath)](#addIndexer-java.lang.String-) | Ajoute un service d'indexeur au nœud du réseau de recherche. |
|
|  | [addExtractor(String storagePath)](#addExtractor-java.lang.String-) | Ajoute un service d'extracteur au nœud du réseau de recherche. |
|
|  | [addShard(String storagePath)](#addShard-java.lang.String-) | Ajoute un service de fragment au nœud du réseau de recherche. |
|
|  | [completeNode()](#completeNode--) | Termine la configuration du nœud du réseau de recherche. |
|
### NodeConfigurator() {#NodeConfigurator--}
```
public NodeConfigurator()
```


### setTcpEndpoint(String hostNameOrAddress, int port) {#setTcpEndpoint-java.lang.String-int-}
```
public abstract NodeConfigurator setTcpEndpoint(String hostNameOrAddress, int port)
```


Définit le point de terminaison TCP.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | hostNameOrAddress | java.lang.String | Le nom d'hôte ou l'adresse. |
|
|  | port | int | Le numéro de port. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addLogSink() {#addLogSink--}
```
public abstract NodeConfigurator addLogSink()
```


Ajoute un puits de journalisation au nœud du réseau de recherche.


**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addSearcher(String storagePath) {#addSearcher-java.lang.String-}
```
public abstract NodeConfigurator addSearcher(String storagePath)
```


Ajoute un service de recherche au nœud du réseau de recherche.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | storagePath | java.lang.String | Le chemin de stockage du service d'ajout. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addIndexer(String storagePath) {#addIndexer-java.lang.String-}
```
public abstract NodeConfigurator addIndexer(String storagePath)
```


Ajoute un service d'indexeur au nœud du réseau de recherche.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | storagePath | java.lang.String | Le chemin de stockage du service d'ajout. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addExtractor(String storagePath) {#addExtractor-java.lang.String-}
```
public abstract NodeConfigurator addExtractor(String storagePath)
```


Ajoute un service d'extracteur au nœud du réseau de recherche.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | storagePath | java.lang.String | Le chemin de stockage du service d'ajout. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addShard(String storagePath) {#addShard-java.lang.String-}
```
public abstract NodeConfigurator addShard(String storagePath)
```


Ajoute un service de fragment au nœud du réseau de recherche.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | storagePath | java.lang.String | Le chemin de stockage du service d'ajout. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### completeNode() {#completeNode--}
```
public abstract Configurator completeNode()
```


Termine la configuration du nœud du réseau de recherche.


**Returns:**
[Configurator](../../com.groupdocs.search.scaling.configuring/configurator) - The configurator.

