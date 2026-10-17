---
title: "Configuration"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente une configuration de réseau de recherche."
type: docs
weight: 10
url: /fr/java/com.groupdocs.search.scaling.configuring/configuration/
---
**Inheritance:**
java.lang.Object
```
public abstract class Configuration
```

Représente une configuration de réseau de recherche.

## Constructeurs

| Constructeur | Description |
| --- | --- |
| [Configuration()](#Configuration--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [save(String filePath)](#save-java.lang.String-) | Enregistre cette configuration dans un fichier. |
|
|  | [save(OutputStream stream)](#save-java.io.OutputStream-) | Enregistre cette configuration dans un flux. |
|
|  | [load(String filePath)](#load-java.lang.String-) | Charge une configuration de réseau de recherche depuis un fichier. |
|
|  | [load(InputStream stream)](#load-java.io.InputStream-) | Charge une configuration de réseau de recherche depuis un flux. |
|
### Configuration() {#Configuration--}
```
public Configuration()
```


### save(String filePath) {#save-java.lang.String-}
```
public abstract void save(String filePath)
```


Enregistre cette configuration dans un fichier.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | filePath | java.lang.String | Le fichier où enregistrer. |
|

### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public abstract void save(OutputStream stream)
```


Enregistre cette configuration dans un flux.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | stream | java.io.OutputStream | Le flux où enregistrer. |
|

### load(String filePath) {#load-java.lang.String-}
```
public static Configuration load(String filePath)
```


Charge une configuration de réseau de recherche depuis un fichier.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | filePath | java.lang.String | Le fichier à charger. |
|

**Returns:**
[Configuration](../../com.groupdocs.search.scaling.configuring/configuration) - The configuration.

### load(InputStream stream) {#load-java.io.InputStream-}
```
public static Configuration load(InputStream stream)
```


Charge une configuration de réseau de recherche depuis un flux.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | stream | java.io.InputStream | Le flux à charger. |
|

**Returns:**
[Configuration](../../com.groupdocs.search.scaling.configuring/configuration) - The configuration.

