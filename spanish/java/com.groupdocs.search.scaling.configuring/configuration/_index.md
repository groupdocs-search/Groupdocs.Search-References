---
title: "Configuración"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa una configuración de red de búsqueda."
type: docs
weight: 10
url: /es/java/com.groupdocs.search.scaling.configuring/configuration/
---
**Inheritance:**
java.lang.Object
```
public abstract class Configuration
```

Representa una configuración de red de búsqueda.

## Constructores

| Constructor | Descripción |
| --- | --- |
| [Configuration()](#Configuration--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
|  | [save(String filePath)](#save-java.lang.String-) | Guarda esta configuración en un archivo. |
|
|  | [save(OutputStream stream)](#save-java.io.OutputStream-) | Guarda esta configuración en un flujo. |
|
|  | [load(String filePath)](#load-java.lang.String-) | Carga una configuración de red de búsqueda desde un archivo. |
|
|  | [load(InputStream stream)](#load-java.io.InputStream-) | Carga una configuración de red de búsqueda desde un flujo. |
|
### Configuration() {#Configuration--}
```
public Configuration()
```


### save(String filePath) {#save-java.lang.String-}
```
public abstract void save(String filePath)
```


Guarda esta configuración en un archivo.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | filePath | java.lang.String | El archivo donde guardar. |
|

### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public abstract void save(OutputStream stream)
```


Guarda esta configuración en un flujo.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | stream | java.io.OutputStream | El flujo donde guardar. |
|

### load(String filePath) {#load-java.lang.String-}
```
public static Configuration load(String filePath)
```


Carga una configuración de red de búsqueda desde un archivo.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | filePath | java.lang.String | El archivo desde el cual cargar. |
|

**Returns:**
[Configuration](../../com.groupdocs.search.scaling.configuring/configuration) - The configuration.

### load(InputStream stream) {#load-java.io.InputStream-}
```
public static Configuration load(InputStream stream)
```


Carga una configuración de red de búsqueda desde un flujo.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | stream | java.io.InputStream | El flujo desde el cual cargar. |
|

**Returns:**
[Configuration](../../com.groupdocs.search.scaling.configuring/configuration) - The configuration.

