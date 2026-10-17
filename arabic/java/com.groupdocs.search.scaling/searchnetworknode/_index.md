---
title: "SearchNetworkNode"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل عقدة شبكة البحث التي يمكن أن تحتوي على خدمات مثل المستخرج، الفهرس، الباحث، الشريحة."
type: docs
weight: 11
url: /ar/java/com.groupdocs.search.scaling/searchnetworknode/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable
```
public class SearchNetworkNode implements Closeable
```

يمثل عقدة شبكة البحث التي يمكن أن تحتوي على خدمات مثل extractor, indexer, searcher, shard.

## المنشئات

| منشئ | الوصف |
| --- | --- |
|  | [SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings)](#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-) | يُنشئ مثلاً جديداً من الفئة  SearchNetworkNode . |
|
|  | [SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger)](#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-com.groupdocs.search.common.ILogger-) | يُنشئ مثلاً جديداً من الفئة  SearchNetworkNode . |
|
|  | [SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger, Configuration configuration)](#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-com.groupdocs.search.common.ILogger-com.groupdocs.search.scaling.configuring.Configuration-) | يُنشئ مثلاً جديداً من الفئة  SearchNetworkNode . |
|
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [start()](#start--) | يبدأ تشغيل عقدة شبكة البحث. |
|
|  | [configureAllNodes()](#configureAllNodes--) | يضبط جميع العقد في شبكة البحث. |
|
|  | [configureNode(int nodeIndex)](#configureNode-int-) | يضبط العقدة المحددة في شبكة البحث. |
|
|  | [getCustomExtractors()](#getCustomExtractors--) | يحصل على مجموعة المستخرج المخصصة. |
|
|  | [setOcrConnector(IOcrConnector ocrConnector)](#setOcrConnector-com.groupdocs.search.options.IOcrConnector-) | يضبط موصل OCR يُستخدم لمعالجة OCR. |
|
|  | [setWordFormsProvider(IWordFormsProvider wordFormsProvider)](#setWordFormsProvider-com.groupdocs.search.dictionaries.IWordFormsProvider-) | يضبط مزود صيغ الكلمات. |
|
|  | [close()](#close--) | يطلق جميع الموارد المستخدمة من قبل  SearchNetworkNode . |
|
|  | [getNodeIndex()](#getNodeIndex--) | يحصل على فهرس عقدة شبكة البحث. |
|
|  | [getEvents()](#getEvents--) | يحصل على مركز الأحداث للاشتراك في الأحداث. |
|
|  | [getIndexer()](#getIndexer--) | يحصل على المفهرس. |
|
|  | [getSearcher()](#getSearcher--) | يحصل على الباحث. |
|
|  | [getShardIndices()](#getShardIndices--) | يحصل على مصفوفة جميع مؤشرات الشرائح في شبكة البحث. |
|
|  | [getNodeIndex(int serviceIndex)](#getNodeIndex-int-) | يحصل على فهرس العقدة التي يقع فيها الخدمة. |
|
| [getCore()](#getCore--) |  |
### SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings) {#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-}
```
public SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings)
```


يُنشئ مثلاً جديداً من الفئة  SearchNetworkNode .


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | nodeIndex | int | فهرس العقدة. |
|
|  | storagePath | java.lang.String | مسار التخزين. |
|
|  | networkSettings | [INetworkSettings](../../com.groupdocs.search.scaling.configuring/inetworksettings) | إعدادات الشبكة. |
|

### SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger) {#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-com.groupdocs.search.common.ILogger-}
```
public SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger)
```


يُنشئ مثلاً جديداً من الفئة  SearchNetworkNode .


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | nodeIndex | int | فهرس العقدة. |
|
|  | storagePath | java.lang.String | مسار التخزين. |
|
|  | networkSettings | [INetworkSettings](../../com.groupdocs.search.scaling.configuring/inetworksettings) | إعدادات الشبكة. |
|
|  | logger | [ILogger](../../com.groupdocs.search.common/ilogger) | المسجل. |
|

### SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger, Configuration configuration) {#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-com.groupdocs.search.common.ILogger-com.groupdocs.search.scaling.configuring.Configuration-}
```
public SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger, Configuration configuration)
```


يُنشئ مثلاً جديداً من الفئة  SearchNetworkNode .


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | nodeIndex | int | فهرس العقدة. |
|
|  | storagePath | java.lang.String | مسار التخزين. |
|
|  | networkSettings | [INetworkSettings](../../com.groupdocs.search.scaling.configuring/inetworksettings) | إعدادات الشبكة. |
|
|  | logger | [ILogger](../../com.groupdocs.search.common/ilogger) | المسجل. |
|
|  | configuration | [Configuration](../../com.groupdocs.search.scaling.configuring/configuration) | التكوين. |
|

### start() {#start--}
```
public void start()
```


يبدأ تشغيل عقدة شبكة البحث.


### configureAllNodes() {#configureAllNodes--}
```
public void configureAllNodes()
```


يضبط جميع العقد في شبكة البحث.


### configureNode(int nodeIndex) {#configureNode-int-}
```
public void configureNode(int nodeIndex)
```


يضبط العقدة المحددة في شبكة البحث.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | nodeIndex | int | فهرس العقدة. |
|

### getCustomExtractors() {#getCustomExtractors--}
```
public CustomExtractorCollection getCustomExtractors()
```


يحصل على مجموعة المستخرج المخصص. المثال الكامل لتطبيق مستخرج مخصص مُقدم في وثائق الواجهة  GroupDocs.Search.Common.IFieldExtractor .


**Returns:**
[CustomExtractorCollection](../../com.groupdocs.search.common/customextractorcollection) - The custom extractor collection.

### setOcrConnector(IOcrConnector ocrConnector) {#setOcrConnector-com.groupdocs.search.options.IOcrConnector-}
```
public void setOcrConnector(IOcrConnector ocrConnector)
```


يضبط موصل OCR يُستخدم لمعالجة OCR.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | ocrConnector | [IOcrConnector](../../com.groupdocs.search.options/iocrconnector) | موصل OCR. |
|

### setWordFormsProvider(IWordFormsProvider wordFormsProvider) {#setWordFormsProvider-com.groupdocs.search.dictionaries.IWordFormsProvider-}
```
public void setWordFormsProvider(IWordFormsProvider wordFormsProvider)
```


يضبط مزود صيغ الكلمات.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | wordFormsProvider | [IWordFormsProvider](../../com.groupdocs.search.dictionaries/iwordformsprovider) | مزوّد صيغ الكلمات. |
|

### close() {#close--}
```
public void close()
```


يطلق جميع الموارد المستخدمة من قبل  SearchNetworkNode .


### getNodeIndex() {#getNodeIndex--}
```
public int getNodeIndex()
```


يحصل على فهرس عقدة شبكة البحث.


**Returns:**
int - فهرس عقدة شبكة البحث.

### getEvents() {#getEvents--}
```
public NodeEventHub getEvents()
```


يحصل على مركز الأحداث للاشتراك في الأحداث.


**Returns:**
[NodeEventHub](../../com.groupdocs.search.scaling.events/nodeeventhub) - The event hub for subscribing to events.

### getIndexer() {#getIndexer--}
```
public Indexer getIndexer()
```


يحصل على المفهرس.


**Returns:**
[Indexer](../../com.groupdocs.search.scaling/indexer) - The indexer.

### getSearcher() {#getSearcher--}
```
public Searcher getSearcher()
```


يحصل على الباحث.


**Returns:**
[Searcher](../../com.groupdocs.search.scaling/searcher) - The searcher.

### getShardIndices() {#getShardIndices--}
```
public int[] getShardIndices()
```


يحصل على مصفوفة جميع مؤشرات الشرائح في شبكة البحث.


**Returns:**
int[] - مصفوفة تحتوي على جميع مؤشرات الشظايا في شبكة البحث.

### getNodeIndex(int serviceIndex) {#getNodeIndex-int-}
```
public int getNodeIndex(int serviceIndex)
```


يحصل على فهرس العقدة التي يقع فيها الخدمة.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | serviceIndex | int | فهرس الخدمة. |
|

**Returns:**
int - فهرس العقدة التي يقع فيها الخدمة. إذا كان فهرس الخدمة غير صحيح، يتم إرجاع -1.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
