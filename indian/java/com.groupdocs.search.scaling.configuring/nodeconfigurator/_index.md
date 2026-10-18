---
title: "NodeConfigurator"
second_title: "GroupDocs.Search for Java API Reference"
description: "खोज नेटवर्क नोड कॉन्फ़िगरेटर का प्रतिनिधित्व करता है।"
type: docs
weight: 13
url: /hi/java/com.groupdocs.search.scaling.configuring/nodeconfigurator/
---
**Inheritance:**
java.lang.Object
```
public abstract class NodeConfigurator
```

खोज नेटवर्क नोड कॉन्फ़िगरेटर का प्रतिनिधित्व करता है।

## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [NodeConfigurator()](#NodeConfigurator--) |  |
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [setTcpEndpoint(String hostNameOrAddress, int port)](#setTcpEndpoint-java.lang.String-int-) | TCP एंडपॉइंट सेट करता है। |
|
|  | [addLogSink()](#addLogSink--) | सर्च नेटवर्क नोड में लॉग सिंक जोड़ता है। |
|
|  | [addSearcher(String storagePath)](#addSearcher-java.lang.String-) | सर्च नेटवर्क नोड में सर्चर सेवा जोड़ता है। |
|
|  | [addIndexer(String storagePath)](#addIndexer-java.lang.String-) | खोज नेटवर्क नोड में एक इंडेक्सर सेवा जोड़ता है। |
|
|  | [addExtractor(String storagePath)](#addExtractor-java.lang.String-) | खोज नेटवर्क नोड में एक एक्सट्रैक्टर सेवा जोड़ता है। |
|
|  | [addShard(String storagePath)](#addShard-java.lang.String-) | खोज नेटवर्क नोड में एक शार्ड सेवा जोड़ता है। |
|
|  | [completeNode()](#completeNode--) | खोज नेटवर्क नोड की कॉन्फ़िगरेशन पूरी करता है। |
|
### NodeConfigurator() {#NodeConfigurator--}
```
public NodeConfigurator()
```


### setTcpEndpoint(String hostNameOrAddress, int port) {#setTcpEndpoint-java.lang.String-int-}
```
public abstract NodeConfigurator setTcpEndpoint(String hostNameOrAddress, int port)
```


TCP एंडपॉइंट सेट करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | hostNameOrAddress | java.lang.String | होस्ट नाम या पता। |
|
|  | port | int | पोर्ट संख्या। |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addLogSink() {#addLogSink--}
```
public abstract NodeConfigurator addLogSink()
```


सर्च नेटवर्क नोड में लॉग सिंक जोड़ता है।


**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addSearcher(String storagePath) {#addSearcher-java.lang.String-}
```
public abstract NodeConfigurator addSearcher(String storagePath)
```


सर्च नेटवर्क नोड में सर्चर सेवा जोड़ता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | storagePath | java.lang.String | जोड़ने वाली सेवा का स्टोरेज पथ। |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addIndexer(String storagePath) {#addIndexer-java.lang.String-}
```
public abstract NodeConfigurator addIndexer(String storagePath)
```


खोज नेटवर्क नोड में एक इंडेक्सर सेवा जोड़ता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | storagePath | java.lang.String | जोड़ने वाली सेवा का स्टोरेज पथ। |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addExtractor(String storagePath) {#addExtractor-java.lang.String-}
```
public abstract NodeConfigurator addExtractor(String storagePath)
```


खोज नेटवर्क नोड में एक एक्सट्रैक्टर सेवा जोड़ता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | storagePath | java.lang.String | जोड़ने वाली सेवा का स्टोरेज पथ। |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addShard(String storagePath) {#addShard-java.lang.String-}
```
public abstract NodeConfigurator addShard(String storagePath)
```


खोज नेटवर्क नोड में एक शार्ड सेवा जोड़ता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | storagePath | java.lang.String | जोड़ने वाली सेवा का स्टोरेज पथ। |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### completeNode() {#completeNode--}
```
public abstract Configurator completeNode()
```


खोज नेटवर्क नोड की कॉन्फ़िगरेशन पूरी करता है।


**Returns:**
[Configurator](../../com.groupdocs.search.scaling.configuring/configurator) - The configurator.

