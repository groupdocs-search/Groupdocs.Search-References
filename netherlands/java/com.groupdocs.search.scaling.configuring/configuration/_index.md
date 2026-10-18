---
title: "Configuration"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt een zoeknetwerkconfiguratie voor."
type: docs
weight: 10
url: /nl/java/com.groupdocs.search.scaling.configuring/configuration/
---
**Inheritance:**
java.lang.Object
```
public abstract class Configuration
```

Stelt een zoeknetwerkconfiguratie voor.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [Configuration()](#Configuration--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [save(String filePath)](#save-java.lang.String-) | Slaat deze configuratie op in een bestand. |
|
|  | [save(OutputStream stream)](#save-java.io.OutputStream-) | Slaat deze configuratie op in een stream. |
|
|  | [load(String filePath)](#load-java.lang.String-) | Laadt een zoeknetwerkconfiguratie uit een bestand. |
|
|  | [load(InputStream stream)](#load-java.io.InputStream-) | Laadt een zoeknetwerkconfiguratie uit een stream. |
|
### Configuration() {#Configuration--}
```
public Configuration()
```


### save(String filePath) {#save-java.lang.String-}
```
public abstract void save(String filePath)
```


Slaat deze configuratie op in een bestand.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | filePath | java.lang.String | Het bestand om op te slaan. |
|

### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public abstract void save(OutputStream stream)
```


Slaat deze configuratie op in een stream.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | stream | java.io.OutputStream | De stream om op te slaan. |
|

### load(String filePath) {#load-java.lang.String-}
```
public static Configuration load(String filePath)
```


Laadt een zoeknetwerkconfiguratie uit een bestand.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | filePath | java.lang.String | Het bestand om te laden. |
|

**Returns:**
[Configuration](../../com.groupdocs.search.scaling.configuring/configuration) - The configuration.

### load(InputStream stream) {#load-java.io.InputStream-}
```
public static Configuration load(InputStream stream)
```


Laadt een zoeknetwerkconfiguratie uit een stream.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | stream | java.io.InputStream | De stream om van te laden. |
|

**Returns:**
[Configuration](../../com.groupdocs.search.scaling.configuring/configuration) - The configuration.

