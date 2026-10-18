---
title: "SearchNetworkNode"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Bir çıkarıcı, indeksleyici, arayıcı ve parça gibi hizmetleri içerebilen bir arama ağı düğümünü temsil eder."
type: docs
weight: 11
url: /tr/java/com.groupdocs.search.scaling/searchnetworknode/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable
```
public class SearchNetworkNode implements Closeable
```

Çıkarıcı, indeksleyici, arayıcı, parça gibi hizmetleri içerebilen bir arama ağı düğümünü temsil eder.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings)](#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-) | SearchNetworkNode sınıfının yeni bir örneğini başlatır. |
|
|  | [SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger)](#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-com.groupdocs.search.common.ILogger-) | SearchNetworkNode sınıfının yeni bir örneğini başlatır. |
|
|  | [SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger, Configuration configuration)](#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-com.groupdocs.search.common.ILogger-com.groupdocs.search.scaling.configuring.Configuration-) | SearchNetworkNode sınıfının yeni bir örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [start()](#start--) | Arama ağı düğümünün işlevselliğini başlatır. |
|
|  | [configureAllNodes()](#configureAllNodes--) | Arama ağındaki tüm düğümleri yapılandırır. |
|
|  | [configureNode(int nodeIndex)](#configureNode-int-) | Arama ağındaki belirtilen düğümü yapılandırır. |
|
|  | [getCustomExtractors()](#getCustomExtractors--) | Özel çıkarıcı koleksiyonunu alır. |
|
|  | [setOcrConnector(IOcrConnector ocrConnector)](#setOcrConnector-com.groupdocs.search.options.IOcrConnector-) | OCR işleme için kullanılan bir OCR bağlayıcısını ayarlar. |
|
|  | [setWordFormsProvider(IWordFormsProvider wordFormsProvider)](#setWordFormsProvider-com.groupdocs.search.dictionaries.IWordFormsProvider-) | Kelime biçimleri sağlayıcısını ayarlar. |
|
|  | [close()](#close--) | SearchNetworkNode tarafından kullanılan tüm kaynakları serbest bırakır. |
|
|  | [getNodeIndex()](#getNodeIndex--) | Arama ağı düğümünün dizinini alır. |
|
|  | [getEvents()](#getEvents--) | Etkinliklere abone olmak için olay merkezini alır. |
|
|  | [getIndexer()](#getIndexer--) | İndeksleyiciyi alır. |
|
|  | [getSearcher()](#getSearcher--) | Arayıcıyı alır. |
|
|  | [getShardIndices()](#getShardIndices--) | Arama ağındaki tüm parça indekslerinin bir dizisini alır. |
|
|  | [getNodeIndex(int serviceIndex)](#getNodeIndex-int-) | Hizmetin bulunduğu düğümün indeksini alır. |
|
| [getCore()](#getCore--) |  |
### SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings) {#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-}
```
public SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings)
```


SearchNetworkNode sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | nodeIndex | int | Düğüm indeksi. |
|
|  | storagePath | java.lang.String | Depolama yolu. |
|
|  | networkSettings | [INetworkSettings](../../com.groupdocs.search.scaling.configuring/inetworksettings) | Ağ ayarları. |
|

### SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger) {#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-com.groupdocs.search.common.ILogger-}
```
public SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger)
```


SearchNetworkNode sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | nodeIndex | int | Düğüm indeksi. |
|
|  | storagePath | java.lang.String | Depolama yolu. |
|
|  | networkSettings | [INetworkSettings](../../com.groupdocs.search.scaling.configuring/inetworksettings) | Ağ ayarları. |
|
|  | logger | [ILogger](../../com.groupdocs.search.common/ilogger) | Günlükleyici. |
|

### SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger, Configuration configuration) {#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-com.groupdocs.search.common.ILogger-com.groupdocs.search.scaling.configuring.Configuration-}
```
public SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger, Configuration configuration)
```


SearchNetworkNode sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | nodeIndex | int | Düğüm indeksi. |
|
|  | storagePath | java.lang.String | Depolama yolu. |
|
|  | networkSettings | [INetworkSettings](../../com.groupdocs.search.scaling.configuring/inetworksettings) | Ağ ayarları. |
|
|  | logger | [ILogger](../../com.groupdocs.search.common/ilogger) | Günlükleyici. |
|
|  | configuration | [Configuration](../../com.groupdocs.search.scaling.configuring/configuration) | Yapılandırma. |
|

### start() {#start--}
```
public void start()
```


Arama ağı düğümünün işlevselliğini başlatır.


### configureAllNodes() {#configureAllNodes--}
```
public void configureAllNodes()
```


Arama ağındaki tüm düğümleri yapılandırır.


### configureNode(int nodeIndex) {#configureNode-int-}
```
public void configureNode(int nodeIndex)
```


Arama ağındaki belirtilen düğümü yapılandırır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | nodeIndex | int | Düğüm indeksi. |
|

### getCustomExtractors() {#getCustomExtractors--}
```
public CustomExtractorCollection getCustomExtractors()
```


Özel çıkarıcı koleksiyonunu alır. Özel bir çıkarıcı uygulamanın tam örneği, GroupDocs.Search.Common.IFieldExtractor arayüzü için belgelerde sunulmuştur.


**Returns:**
[CustomExtractorCollection](../../com.groupdocs.search.common/customextractorcollection) - The custom extractor collection.

### setOcrConnector(IOcrConnector ocrConnector) {#setOcrConnector-com.groupdocs.search.options.IOcrConnector-}
```
public void setOcrConnector(IOcrConnector ocrConnector)
```


OCR işleme için kullanılan bir OCR bağlayıcısını ayarlar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | ocrConnector | [IOcrConnector](../../com.groupdocs.search.options/iocrconnector) | OCR bağlayıcısı. |
|

### setWordFormsProvider(IWordFormsProvider wordFormsProvider) {#setWordFormsProvider-com.groupdocs.search.dictionaries.IWordFormsProvider-}
```
public void setWordFormsProvider(IWordFormsProvider wordFormsProvider)
```


Kelime biçimleri sağlayıcısını ayarlar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | wordFormsProvider | [IWordFormsProvider](../../com.groupdocs.search.dictionaries/iwordformsprovider) | Kelime biçimleri sağlayıcısı. |
|

### close() {#close--}
```
public void close()
```


SearchNetworkNode tarafından kullanılan tüm kaynakları serbest bırakır.


### getNodeIndex() {#getNodeIndex--}
```
public int getNodeIndex()
```


Arama ağı düğümünün dizinini alır.


**Returns:**
int - Arama ağı düğümünün dizini.

### getEvents() {#getEvents--}
```
public NodeEventHub getEvents()
```


Etkinliklere abone olmak için olay merkezini alır.


**Returns:**
[NodeEventHub](../../com.groupdocs.search.scaling.events/nodeeventhub) - The event hub for subscribing to events.

### getIndexer() {#getIndexer--}
```
public Indexer getIndexer()
```


İndeksleyiciyi alır.


**Returns:**
[Indexer](../../com.groupdocs.search.scaling/indexer) - The indexer.

### getSearcher() {#getSearcher--}
```
public Searcher getSearcher()
```


Arayıcıyı alır.


**Returns:**
[Searcher](../../com.groupdocs.search.scaling/searcher) - The searcher.

### getShardIndices() {#getShardIndices--}
```
public int[] getShardIndices()
```


Arama ağındaki tüm parça indekslerinin bir dizisini alır.


**Returns:**
int[] - Arama ağındaki tüm parçacık indekslerinin bir dizisi.

### getNodeIndex(int serviceIndex) {#getNodeIndex-int-}
```
public int getNodeIndex(int serviceIndex)
```


Hizmetin bulunduğu düğümün indeksini alır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | serviceIndex | int | Servis indeksi. |
|

**Returns:**
int - Servisin bulunduğu düğümün indeksi. Servis indeksi yanlışsa, -1 döndürülür.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
