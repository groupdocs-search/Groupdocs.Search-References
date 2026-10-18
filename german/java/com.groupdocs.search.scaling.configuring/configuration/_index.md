---
title: "Configuration"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt eine Suchnetzwerkkonfiguration dar."
type: docs
weight: 10
url: /de/java/com.groupdocs.search.scaling.configuring/configuration/
---
**Inheritance:**
java.lang.Object
```
public abstract class Configuration
```

Stellt eine Suchnetzwerkkonfiguration dar.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [Configuration()](#Configuration--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [save(String filePath)](#save-java.lang.String-) | Speichert diese Konfiguration in einer Datei. |
|
|  | [save(OutputStream stream)](#save-java.io.OutputStream-) | Speichert diese Konfiguration in einen Stream. |
|
|  | [load(String filePath)](#load-java.lang.String-) | Lädt eine Suchnetzwerk-Konfiguration aus einer Datei. |
|
|  | [load(InputStream stream)](#load-java.io.InputStream-) | Lädt eine Suchnetzwerk-Konfiguration aus einem Stream. |
|
### Configuration() {#Configuration--}
```
public Configuration()
```


### save(String filePath) {#save-java.lang.String-}
```
public abstract void save(String filePath)
```


Speichert diese Konfiguration in einer Datei.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | filePath | java.lang.String | Die Datei, in die gespeichert werden soll. |
|

### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public abstract void save(OutputStream stream)
```


Speichert diese Konfiguration in einen Stream.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | stream | java.io.OutputStream | Der Stream, in den gespeichert werden soll. |
|

### load(String filePath) {#load-java.lang.String-}
```
public static Configuration load(String filePath)
```


Lädt eine Suchnetzwerk-Konfiguration aus einer Datei.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | filePath | java.lang.String | Die Datei, aus der geladen werden soll. |
|

**Returns:**
[Configuration](../../com.groupdocs.search.scaling.configuring/configuration) - The configuration.

### load(InputStream stream) {#load-java.io.InputStream-}
```
public static Configuration load(InputStream stream)
```


Lädt eine Suchnetzwerk-Konfiguration aus einem Stream.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | stream | java.io.InputStream | Der Stream, aus dem geladen wird. |
|

**Returns:**
[Configuration](../../com.groupdocs.search.scaling.configuring/configuration) - The configuration.

