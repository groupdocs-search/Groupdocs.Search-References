---
title: "NodeConfigurator"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Arama ağı düğüm yapılandırıcısını temsil eder."
type: docs
weight: 13
url: /tr/java/com.groupdocs.search.scaling.configuring/nodeconfigurator/
---
**Inheritance:**
java.lang.Object
```
public abstract class NodeConfigurator
```

Arama ağı düğüm yapılandırıcısını temsil eder.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [NodeConfigurator()](#NodeConfigurator--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [setTcpEndpoint(String hostNameOrAddress, int port)](#setTcpEndpoint-java.lang.String-int-) | TCP uç noktasını ayarlar. |
|
|  | [addLogSink()](#addLogSink--) | Arama ağ düğümüne bir günlük alıcısı ekler. |
|
|  | [addSearcher(String storagePath)](#addSearcher-java.lang.String-) | Arama ağ düğümüne bir arayıcı hizmeti ekler. |
|
|  | [addIndexer(String storagePath)](#addIndexer-java.lang.String-) | Arama ağ düğümüne bir indeksleyici hizmeti ekler. |
|
|  | [addExtractor(String storagePath)](#addExtractor-java.lang.String-) | Arama ağ düğümüne bir çıkarıcı hizmeti ekler. |
|
|  | [addShard(String storagePath)](#addShard-java.lang.String-) | Arama ağ düğümüne bir parça hizmeti ekler. |
|
|  | [completeNode()](#completeNode--) | Arama ağ düğümünün yapılandırmasını tamamlar. |
|
### NodeConfigurator() {#NodeConfigurator--}
```
public NodeConfigurator()
```


### setTcpEndpoint(String hostNameOrAddress, int port) {#setTcpEndpoint-java.lang.String-int-}
```
public abstract NodeConfigurator setTcpEndpoint(String hostNameOrAddress, int port)
```


TCP uç noktasını ayarlar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | hostNameOrAddress | java.lang.String | Ana bilgisayar adı veya adres. |
|
|  | port | int | Bağlantı noktası numarası. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addLogSink() {#addLogSink--}
```
public abstract NodeConfigurator addLogSink()
```


Arama ağ düğümüne bir günlük alıcısı ekler.


**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addSearcher(String storagePath) {#addSearcher-java.lang.String-}
```
public abstract NodeConfigurator addSearcher(String storagePath)
```


Arama ağ düğümüne bir arayıcı hizmeti ekler.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | storagePath | java.lang.String | Ekleme hizmetinin depolama yolu. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addIndexer(String storagePath) {#addIndexer-java.lang.String-}
```
public abstract NodeConfigurator addIndexer(String storagePath)
```


Arama ağ düğümüne bir indeksleyici hizmeti ekler.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | storagePath | java.lang.String | Ekleme hizmetinin depolama yolu. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addExtractor(String storagePath) {#addExtractor-java.lang.String-}
```
public abstract NodeConfigurator addExtractor(String storagePath)
```


Arama ağ düğümüne bir çıkarıcı hizmeti ekler.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | storagePath | java.lang.String | Ekleme hizmetinin depolama yolu. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addShard(String storagePath) {#addShard-java.lang.String-}
```
public abstract NodeConfigurator addShard(String storagePath)
```


Arama ağ düğümüne bir parça hizmeti ekler.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | storagePath | java.lang.String | Ekleme hizmetinin depolama yolu. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### completeNode() {#completeNode--}
```
public abstract Configurator completeNode()
```


Arama ağ düğümünün yapılandırmasını tamamlar.


**Returns:**
[Configurator](../../com.groupdocs.search.scaling.configuring/configurator) - The configurator.

