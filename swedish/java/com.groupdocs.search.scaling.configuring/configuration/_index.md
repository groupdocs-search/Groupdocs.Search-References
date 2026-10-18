---
title: "Configuration"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar en konfiguration för ett söknätverk."
type: docs
weight: 10
url: /sv/java/com.groupdocs.search.scaling.configuring/configuration/
---
**Inheritance:**
java.lang.Object
```
public abstract class Configuration
```

Representerar en konfiguration för ett söknätverk.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [Configuration()](#Configuration--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [save(String filePath)](#save-java.lang.String-) | Sparar denna konfiguration till en fil. |
|
|  | [save(OutputStream stream)](#save-java.io.OutputStream-) | Sparar denna konfiguration till en ström. |
|
|  | [load(String filePath)](#load-java.lang.String-) | Läser in en söknätskonfiguration från en fil. |
|
|  | [load(InputStream stream)](#load-java.io.InputStream-) | Läser in en söknätskonfiguration från en ström. |
|
### Configuration() {#Configuration--}
```
public Configuration()
```


### save(String filePath) {#save-java.lang.String-}
```
public abstract void save(String filePath)
```


Sparar denna konfiguration till en fil.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | filePath | java.lang.String | Filen att spara till. |
|

### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public abstract void save(OutputStream stream)
```


Sparar denna konfiguration till en ström.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | ström | java.io.OutputStream | Strömmen att spara till. |
|

### load(String filePath) {#load-java.lang.String-}
```
public static Configuration load(String filePath)
```


Läser in en söknätskonfiguration från en fil.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | filePath | java.lang.String | Filen att läsa in från. |
|

**Returns:**
[Configuration](../../com.groupdocs.search.scaling.configuring/configuration) - The configuration.

### load(InputStream stream) {#load-java.io.InputStream-}
```
public static Configuration load(InputStream stream)
```


Läser in en söknätskonfiguration från en ström.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | ström | java.io.InputStream | Strömmen att läsa från. |
|

**Returns:**
[Configuration](../../com.groupdocs.search.scaling.configuring/configuration) - The configuration.

