---
title: "Configuration"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta una configurazione della rete di ricerca."
type: docs
weight: 10
url: /it/java/com.groupdocs.search.scaling.configuring/configuration/
---
**Inheritance:**
java.lang.Object
```
public abstract class Configuration
```

Rappresenta una configurazione della rete di ricerca.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [Configuration()](#Configuration--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [save(String filePath)](#save-java.lang.String-) | Salva questa configurazione su un file. |
|
|  | [save(OutputStream stream)](#save-java.io.OutputStream-) | Salva questa configurazione su uno stream. |
|
|  | [load(String filePath)](#load-java.lang.String-) | Carica una configurazione di rete di ricerca da un file. |
|
|  | [load(InputStream stream)](#load-java.io.InputStream-) | Carica una configurazione di rete di ricerca da uno stream. |
|
### Configuration() {#Configuration--}
```
public Configuration()
```


### save(String filePath) {#save-java.lang.String-}
```
public abstract void save(String filePath)
```


Salva questa configurazione su un file.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | filePath | java.lang.String | Il file su cui salvare. |
|

### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public abstract void save(OutputStream stream)
```


Salva questa configurazione su uno stream.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | stream | java.io.OutputStream | Lo stream su cui salvare. |
|

### load(String filePath) {#load-java.lang.String-}
```
public static Configuration load(String filePath)
```


Carica una configurazione di rete di ricerca da un file.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | filePath | java.lang.String | Il file da cui caricare. |
|

**Returns:**
[Configuration](../../com.groupdocs.search.scaling.configuring/configuration) - The configuration.

### load(InputStream stream) {#load-java.io.InputStream-}
```
public static Configuration load(InputStream stream)
```


Carica una configurazione di rete di ricerca da uno stream.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | stream | java.io.InputStream | Il flusso da caricare. |
|

**Returns:**
[Configuration](../../com.groupdocs.search.scaling.configuring/configuration) - The configuration.

