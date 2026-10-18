---
title: "Configurator"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Arama ağı yapılandırıcısını temsil eder."
type: docs
weight: 11
url: /tr/java/com.groupdocs.search.scaling.configuring/configurator/
---
**Inheritance:**
java.lang.Object
```
public class Configurator
```

Arama ağı yapılandırıcısını temsil eder.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [Configurator()](#Configurator--) | Configurator sınıfının yeni bir örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [setIndexSettings()](#setIndexSettings--) | Arama ağındaki her parçacık için indeks ayarlarını yapılandırmayı başlatır. |
|
|  | [addNode(int nodeIndex)](#addNode-int-) | Arama ağı yapılandırmasına bir düğüm ekler. |
|
|  | [completeConfiguration()](#completeConfiguration--) | Yapılandırma sürecini tamamlar ve arama ağı yapılandırmasının bir örneğini döndürür. |
|
| [getCore()](#getCore--) |  |
### Configurator() {#Configurator--}
```
public Configurator()
```


Configurator sınıfının yeni bir örneğini başlatır.


### setIndexSettings() {#setIndexSettings--}
```
public IndexSettingsConfigurator setIndexSettings()
```


Arama ağındaki her parçacık için indeks ayarlarını yapılandırmayı başlatır.


**Returns:**
[IndexSettingsConfigurator](../../com.groupdocs.search.scaling.configuring/indexsettingsconfigurator) - The index settings configurator.

### addNode(int nodeIndex) {#addNode-int-}
```
public NodeConfigurator addNode(int nodeIndex)
```


Arama ağı yapılandırmasına bir düğüm ekler.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | nodeIndex | int | Düğüm indeksi. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - The node configurator.

### completeConfiguration() {#completeConfiguration--}
```
public Configuration completeConfiguration()
```


Yapılandırma sürecini tamamlar ve arama ağı yapılandırmasının bir örneğini döndürür.


**Returns:**
[Configuration](../../com.groupdocs.search.scaling.configuring/configuration) - The configuration.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
