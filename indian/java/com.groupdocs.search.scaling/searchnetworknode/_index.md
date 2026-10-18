---
title: "SearchNetworkNode"
second_title: "GroupDocs.Search for Java API Reference"
description: "एक सर्च नेटवर्क नोड का प्रतिनिधित्व करता है जिसमें एक्सट्रैक्टर, इंडेक्सर, सर्चर, शार्ड जैसी सेवाएँ हो सकती हैं।"
type: docs
weight: 11
url: /hi/java/com.groupdocs.search.scaling/searchnetworknode/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable
```
public class SearchNetworkNode implements Closeable
```

एक खोज नेटवर्क नोड का प्रतिनिधित्व करता है जिसमें एक्सट्रैक्टर, इंडेक्सर, सर्चर, शार्ड जैसी सेवाएँ हो सकती हैं।

## निर्माता

| निर्माता | विवरण |
| --- | --- |
|  | [SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings)](#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-) | SearchNetworkNode वर्ग का एक नया उदाहरण प्रारंभ करता है। |
|
|  | [SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger)](#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-com.groupdocs.search.common.ILogger-) | SearchNetworkNode वर्ग का एक नया उदाहरण प्रारंभ करता है। |
|
|  | [SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger, Configuration configuration)](#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-com.groupdocs.search.common.ILogger-com.groupdocs.search.scaling.configuring.Configuration-) | SearchNetworkNode वर्ग का एक नया उदाहरण प्रारंभ करता है। |
|
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [start()](#start--) | सर्च नेटवर्क नोड के कार्य को शुरू करता है। |
|
|  | [configureAllNodes()](#configureAllNodes--) | खोज नेटवर्क में सभी नोड्स को कॉन्फ़िगर करता है। |
|
|  | [configureNode(int nodeIndex)](#configureNode-int-) | खोज नेटवर्क में निर्दिष्ट नोड को कॉन्फ़िगर करता है। |
|
|  | [getCustomExtractors()](#getCustomExtractors--) | कस्टम एक्सट्रैक्टर संग्रह प्राप्त करता है। |
|
|  | [setOcrConnector(IOcrConnector ocrConnector)](#setOcrConnector-com.groupdocs.search.options.IOcrConnector-) | एक OCR कनेक्टर सेट करता है जो OCR प्रोसेसिंग के लिए उपयोग किया जाता है। |
|
|  | [setWordFormsProvider(IWordFormsProvider wordFormsProvider)](#setWordFormsProvider-com.groupdocs.search.dictionaries.IWordFormsProvider-) | शब्द रूप प्रदाता सेट करता है। |
|
|  | [close()](#close--) | SearchNetworkNode द्वारा उपयोग किए गए सभी संसाधनों को मुक्त करता है। |
|
|  | [getNodeIndex()](#getNodeIndex--) | सर्च नेटवर्क नोड का इंडेक्स प्राप्त करता है। |
|
|  | [getEvents()](#getEvents--) | इवेंट्स की सदस्यता के लिए इवेंट हब प्राप्त करता है। |
|
|  | [getIndexer()](#getIndexer--) | इंडेक्सर प्राप्त करता है। |
|
|  | [getSearcher()](#getSearcher--) | सर्चर प्राप्त करता है। |
|
|  | [getShardIndices()](#getShardIndices--) | खोज नेटवर्क में सभी शार्ड इंडेक्स की एक एरे प्राप्त करता है। |
|
|  | [getNodeIndex(int serviceIndex)](#getNodeIndex-int-) | सेवा स्थित नोड का इंडेक्स प्राप्त करता है। |
|
| [getCore()](#getCore--) |  |
### SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings) {#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-}
```
public SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings)
```


SearchNetworkNode वर्ग का एक नया उदाहरण प्रारंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | nodeIndex | int | नोड इंडेक्स। |
|
|  | storagePath | java.lang.String | संग्रहण पथ। |
|
|  | networkSettings | [INetworkSettings](../../com.groupdocs.search.scaling.configuring/inetworksettings) | नेटवर्क सेटिंग्स। |
|

### SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger) {#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-com.groupdocs.search.common.ILogger-}
```
public SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger)
```


SearchNetworkNode वर्ग का एक नया उदाहरण प्रारंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | nodeIndex | int | नोड इंडेक्स। |
|
|  | storagePath | java.lang.String | संग्रहण पथ। |
|
|  | networkSettings | [INetworkSettings](../../com.groupdocs.search.scaling.configuring/inetworksettings) | नेटवर्क सेटिंग्स। |
|
|  | logger | [ILogger](../../com.groupdocs.search.common/ilogger) | लॉगर। |
|

### SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger, Configuration configuration) {#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-com.groupdocs.search.common.ILogger-com.groupdocs.search.scaling.configuring.Configuration-}
```
public SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger, Configuration configuration)
```


SearchNetworkNode वर्ग का एक नया उदाहरण प्रारंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | nodeIndex | int | नोड इंडेक्स। |
|
|  | storagePath | java.lang.String | संग्रहण पथ। |
|
|  | networkSettings | [INetworkSettings](../../com.groupdocs.search.scaling.configuring/inetworksettings) | नेटवर्क सेटिंग्स। |
|
|  | logger | [ILogger](../../com.groupdocs.search.common/ilogger) | लॉगर। |
|
|  | configuration | [Configuration](../../com.groupdocs.search.scaling.configuring/configuration) | कॉन्फ़िगरेशन। |
|

### start() {#start--}
```
public void start()
```


सर्च नेटवर्क नोड के कार्य को शुरू करता है।


### configureAllNodes() {#configureAllNodes--}
```
public void configureAllNodes()
```


खोज नेटवर्क में सभी नोड्स को कॉन्फ़िगर करता है।


### configureNode(int nodeIndex) {#configureNode-int-}
```
public void configureNode(int nodeIndex)
```


खोज नेटवर्क में निर्दिष्ट नोड को कॉन्फ़िगर करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | nodeIndex | int | नोड इंडेक्स। |
|

### getCustomExtractors() {#getCustomExtractors--}
```
public CustomExtractorCollection getCustomExtractors()
```


कस्टम एक्सट्रैक्टर संग्रह प्राप्त करता है। कस्टम एक्सट्रैक्टर को लागू करने का पूर्ण उदाहरण GroupDocs.Search.Common.IFieldExtractor इंटरफ़ेस के दस्तावेज़ में प्रस्तुत किया गया है।


**Returns:**
[CustomExtractorCollection](../../com.groupdocs.search.common/customextractorcollection) - The custom extractor collection.

### setOcrConnector(IOcrConnector ocrConnector) {#setOcrConnector-com.groupdocs.search.options.IOcrConnector-}
```
public void setOcrConnector(IOcrConnector ocrConnector)
```


एक OCR कनेक्टर सेट करता है जो OCR प्रोसेसिंग के लिए उपयोग किया जाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | ocrConnector | [IOcrConnector](../../com.groupdocs.search.options/iocrconnector) | OCR कनेक्टर। |
|

### setWordFormsProvider(IWordFormsProvider wordFormsProvider) {#setWordFormsProvider-com.groupdocs.search.dictionaries.IWordFormsProvider-}
```
public void setWordFormsProvider(IWordFormsProvider wordFormsProvider)
```


शब्द रूप प्रदाता सेट करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | wordFormsProvider | [IWordFormsProvider](../../com.groupdocs.search.dictionaries/iwordformsprovider) | वर्ड फॉर्म्स प्रोवाइडर। |
|

### close() {#close--}
```
public void close()
```


SearchNetworkNode द्वारा उपयोग किए गए सभी संसाधनों को मुक्त करता है।


### getNodeIndex() {#getNodeIndex--}
```
public int getNodeIndex()
```


सर्च नेटवर्क नोड का इंडेक्स प्राप्त करता है।


**Returns:**
int - सर्च नेटवर्क नोड का इंडेक्स।

### getEvents() {#getEvents--}
```
public NodeEventHub getEvents()
```


इवेंट्स की सदस्यता के लिए इवेंट हब प्राप्त करता है।


**Returns:**
[NodeEventHub](../../com.groupdocs.search.scaling.events/nodeeventhub) - The event hub for subscribing to events.

### getIndexer() {#getIndexer--}
```
public Indexer getIndexer()
```


इंडेक्सर प्राप्त करता है।


**Returns:**
[Indexer](../../com.groupdocs.search.scaling/indexer) - The indexer.

### getSearcher() {#getSearcher--}
```
public Searcher getSearcher()
```


सर्चर प्राप्त करता है।


**Returns:**
[Searcher](../../com.groupdocs.search.scaling/searcher) - The searcher.

### getShardIndices() {#getShardIndices--}
```
public int[] getShardIndices()
```


खोज नेटवर्क में सभी शार्ड इंडेक्स की एक एरे प्राप्त करता है।


**Returns:**
int[] - खोज नेटवर्क में सभी शार्ड इंडेक्स की एक एरे।

### getNodeIndex(int serviceIndex) {#getNodeIndex-int-}
```
public int getNodeIndex(int serviceIndex)
```


सेवा स्थित नोड का इंडेक्स प्राप्त करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | serviceIndex | int | सेवा इंडेक्स। |
|

**Returns:**
int - वह नोड का इंडेक्स जहाँ सेवा स्थित है। यदि सेवा इंडेक्स गलत है, तो -1 लौटाया जाता है।

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
