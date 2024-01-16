---
title: Configuration
second_title: GroupDocs.Search for Java API Reference
description: Represents a search network configuration.
type: docs
weight: 10
url: /java/com.groupdocs.search.scaling.configuring/configuration/
---
**Inheritance:**
java.lang.Object
```
public abstract class Configuration
```

Represents a search network configuration.
## Constructors

| Constructor | Description |
| --- | --- |
| [Configuration()](#Configuration--) |  |
## Methods

| Method | Description |
| --- | --- |
| [save(String filePath)](#save-java.lang.String-) | Saves this configuration to a file. |
| [save(OutputStream stream)](#save-java.io.OutputStream-) | Saves this configuration to a stream. |
| [load(String filePath)](#load-java.lang.String-) | Loads a search network configuration from a file. |
| [load(InputStream stream)](#load-java.io.InputStream-) | Loads a search network configuration from a stream. |
### Configuration() {#Configuration--}
```
public Configuration()
```


### save(String filePath) {#save-java.lang.String-}
```
public abstract void save(String filePath)
```


Saves this configuration to a file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | The file to save to. |

### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public abstract void save(OutputStream stream)
```


Saves this configuration to a stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | The stream to save to. |

### load(String filePath) {#load-java.lang.String-}
```
public static Configuration load(String filePath)
```


Loads a search network configuration from a file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | The file to load from. |

**Returns:**
[Configuration](../../com.groupdocs.search.scaling.configuring/configuration) - The configuration.
### load(InputStream stream) {#load-java.io.InputStream-}
```
public static Configuration load(InputStream stream)
```


Loads a search network configuration from a stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | The stream to load from. |

**Returns:**
[Configuration](../../com.groupdocs.search.scaling.configuring/configuration) - The configuration.
