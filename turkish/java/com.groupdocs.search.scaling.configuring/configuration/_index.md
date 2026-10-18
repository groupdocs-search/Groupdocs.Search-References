---
title: "Yapılandırma"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Arama ağı yapılandırmasını temsil eder."
type: docs
weight: 10
url: /tr/java/com.groupdocs.search.scaling.configuring/configuration/
---
**Inheritance:**
java.lang.Object
```
public abstract class Configuration
```

Arama ağı yapılandırmasını temsil eder.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [Configuration()](#Configuration--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [save(String filePath)](#save-java.lang.String-) | Bu yapılandırmayı bir dosyaya kaydeder. |
|
|  | [save(OutputStream stream)](#save-java.io.OutputStream-) | Bu yapılandırmayı bir akışa kaydeder. |
|
|  | [load(String filePath)](#load-java.lang.String-) | Bir dosyadan arama ağı yapılandırması yükler. |
|
|  | [load(InputStream stream)](#load-java.io.InputStream-) | Bir akıştan arama ağı yapılandırması yükler. |
|
### Configuration() {#Configuration--}
```
public Configuration()
```


### save(String filePath) {#save-java.lang.String-}
```
public abstract void save(String filePath)
```


Bu yapılandırmayı bir dosyaya kaydeder.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | filePath | java.lang.String | Kaydedilecek dosya. |
|

### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public abstract void save(OutputStream stream)
```


Bu yapılandırmayı bir akışa kaydeder.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | stream | java.io.OutputStream | Kaydedilecek akış. |
|

### load(String filePath) {#load-java.lang.String-}
```
public static Configuration load(String filePath)
```


Bir dosyadan arama ağı yapılandırması yükler.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | filePath | java.lang.String | Yüklenecek dosya. |
|

**Returns:**
[Configuration](../../com.groupdocs.search.scaling.configuring/configuration) - The configuration.

### load(InputStream stream) {#load-java.io.InputStream-}
```
public static Configuration load(InputStream stream)
```


Bir akıştan arama ağı yapılandırması yükler.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | stream | java.io.InputStream | Yüklenecek akış. |
|

**Returns:**
[Configuration](../../com.groupdocs.search.scaling.configuring/configuration) - The configuration.

